# Comparing `tmp/cwsearch_utils-0.0.4-py3-none-any.whl.zip` & `tmp/cwsearch_utils-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4814 bytes, number of entries: 7
+Zip file size: 4997 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 04:52 cwsearch_utils/__init__.py
 -rw-rw-r--  2.0 unx     7097 b- defN 23-Apr-09 04:52 cwsearch_utils/aggregate.py
--rw-rw-r--  2.0 unx     4326 b- defN 23-Apr-10 02:36 cwsearch_utils/infinstor_lock.py
--rw-rw-r--  2.0 unx      570 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-10 02:36 cwsearch_utils-0.0.4.dist-info/RECORD
-7 files, 12678 bytes uncompressed, 3778 bytes compressed:  70.2%
+-rw-rw-r--  2.0 unx     4723 b- defN 23-Apr-17 18:25 cwsearch_utils/infinstor_lock.py
+-rw-rw-r--  2.0 unx      570 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      578 b- defN 23-Apr-17 18:55 cwsearch_utils-0.1.0.dist-info/RECORD
+7 files, 13075 bytes uncompressed, 3961 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: cwsearch_utils/aggregate.py
 Comment: 
 
 Filename: cwsearch_utils/infinstor_lock.py
 Comment: 
 
-Filename: cwsearch_utils-0.0.4.dist-info/METADATA
+Filename: cwsearch_utils-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: cwsearch_utils-0.0.4.dist-info/WHEEL
+Filename: cwsearch_utils-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: cwsearch_utils-0.0.4.dist-info/top_level.txt
+Filename: cwsearch_utils-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cwsearch_utils-0.0.4.dist-info/RECORD
+Filename: cwsearch_utils-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cwsearch_utils/infinstor_lock.py

```diff
@@ -1,16 +1,17 @@
 import datetime
 import tempfile
 import json
 import os
+import sqlite3
 
 def set_start(s3client, bucket, prefix, infinstor_time_spec):
     import botocore
     # this is not really a locking mechanism - the prev ddb conditional put based code was
-    status_object_name = f"{prefix}/index/{infinstor_time_spec}/names.json.creating"
+    status_object_name = f"{prefix}/index/{infinstor_time_spec}/names.db.creating"
     try:
         metadata = s3client.head_object(Bucket=bucket, Key=status_object_name)
         creation_time = metadata['LastModified']
         tnow = datetime.datetime.utcnow()
         delta = tnow - creation_time
         if delta.total_seconds() > 900:
             print(f"Status object {creation_time} older than 900 seconds {tnow} for {infinstor_time_spec}. This lambda invocation continuing ..")
@@ -30,52 +31,65 @@
         response = s3client.upload_file(tfile, bucket, status_object_name)
         print(f"{status_object_name} does not exist. This lambda invocation successfully created status object {status_object_name} and continuing..")
         return True
     except botocore.exceptions.ClientError as e:
         print(f"Caught {e} while creating status file {status_object_name}. This lambda invocation exiting..")
         return False
 
+def load_from_db(fn, tag):
+    rv = {}
+    con = sqlite3.connect(fn)
+    cur = con.cursor()
+    if not tag:
+        tag = 'notag'
+    print(f'load_from_db: Loading fn={fn}, tag={tag}')
+    res = cur.execute(f"SELECT name, timestamp, link, msg FROM links WHERE tag='{tag}'")
+    while one_entry = res.fetchone():
+        name = one_entry[0]
+        if name in rv:
+            rv[name].append((one_entry[1], one_entry[2], one_entry[3]))
+        else:
+            rv[name] = [(one_entry[1], one_entry[2], one_entry[3])]
+    return rv
+
 # returns 'NotPresent'|'Creating'|'Ready'|'CreationFailed', names|None
-def get_cache_entry(bucket, prefix, infinstor_time_spec, head_only):
+def get_cache_entry(bucket, prefix, infinstor_time_spec, tag, head_only):
     import boto3
     import botocore
     s3client = boto3.client('s3')
-    object_name = f"{prefix}/index/{infinstor_time_spec}/names.json"
+    object_name = f"{prefix}/index/{infinstor_time_spec}/names.db"
 
     if head_only:
-        lfn = "/tmp/names.json"
         try:
             metadata = s3client.head_object(Bucket=bucket, Key=object_name)
             return 'Ready', {}
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == "404":
                 print(f"{object_name} does not exist. Trying status object")
             else:
                 print(f"Caught {e} while reading {object_name}. Returning NotPresent")
                 return 'NotPresent', None
     else:
-        lfn = "/tmp/names.json"
+        lfn = "/tmp/names.db"
         try:
             s3client.download_file(bucket, object_name, lfn)
-            with open(lfn, 'r') as fp:
-                dct = json.load(fp)
-                print(f"Loaded json file {len(dct)} entries from {object_name}")
+            dct = load_from_db(lfn, tag)
             os.remove(lfn)
             if dct:
                 return 'Ready', dct
             else:
                 return 'Ready', {}
         except botocore.exceptions.ClientError as e:
             if e.response['Error']['Code'] == "404":
                 print(f"{object_name} does not exist. Trying status object")
             else:
                 print(f"Caught {e} while reading {object_name}. Returning NotPresent")
                 return 'NotPresent', None
 
-    status_object_name = f"{prefix}/index/{infinstor_time_spec}/names.json.creating"
+    status_object_name = f"{prefix}/index/{infinstor_time_spec}/names.db.creating"
     try:
         metadata = s3client.head_object(Bucket=bucket, Key=status_object_name)
         creation_time = metadata['LastModified']
         tnow = datetime.datetime.utcnow()
         delta = creation_time - tnow
         if delta.total_seconds() > 900:
             print(f"Status object {creation_time} older than 900 seconds {tnow} for {infinstor_time_spec}. CreationFailed..")
```

## Comparing `cwsearch_utils-0.0.4.dist-info/METADATA` & `cwsearch_utils-0.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwsearch-utils
-Version: 0.0.4
+Version: 0.1.0
 Summary: InfinStor InfinLogs CloudWatch Search Utilities
 Home-page: https://infinstor.com/
 Author: InfinStor, Inc.
 Author-email: support@infinstor.com
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

