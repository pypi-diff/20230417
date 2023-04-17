# Comparing `tmp/propertysync-0.4.0.tar.gz` & `tmp/propertysync-0.4.1.tar.gz`

## Comparing `propertysync-0.4.0.tar` & `propertysync-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 propertysync-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/__about__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/__init__.py
--rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/api.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/batch.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/document.py
--rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/search.py
--rw-r--r--   0        0        0    15625 2020-02-02 00:00:00.000000 propertysync-0.4.0/propertysync/titlesearch_batch.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.4.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.4.0/LICENSE
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.4.0/README.md
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 propertysync-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 propertysync-0.4.1/propertysync/__about__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 propertysync-0.4.1/propertysync/__init__.py
+-rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 propertysync-0.4.1/propertysync/api.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 propertysync-0.4.1/propertysync/batch.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 propertysync-0.4.1/propertysync/document.py
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 propertysync-0.4.1/propertysync/search.py
+-rw-r--r--   0        0        0    15969 2020-02-02 00:00:00.000000 propertysync-0.4.1/propertysync/titlesearch_batch.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 propertysync-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 propertysync-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 propertysync-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 propertysync-0.4.1/README.md
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 propertysync-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 propertysync-0.4.1/PKG-INFO
```

### Comparing `propertysync-0.4.0/CHANGELOG.md` & `propertysync-0.4.1/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,33 +8,38 @@
 ## [Unreleased]
 
 ### Added
 ### Fixed
 ### Changed
 ### Removed
 
-## [0.4.0] - 2023-04-26
+## [0.4.1] - 2023-04-17
+
+### Changed
+- Minor adjustments to TitleSearchBatch helper for default naming and date format
+
+## [0.4.0] - 2023-04-17
 
 ### Added
 - Added TitleSearchBatch helper to convert from titlesearch format to batch format
 
-## [0.3.0] - 2023-04-26
+## [0.3.0] - 2023-04-14
 
 ### Added
 - Added support to document and batch classes to support find and replace
 
-## [0.2.1] - 2023-04-26
+## [0.2.1] - 2023-04-14
 
 ### Added
 - Added optional save_to_search and wait_time parameters to create_batch_from_json method that allows you to submit a batch, wait for it's documents to be processed and save the batch to search making those documents live in the plant.
 
 ### Fixed
 - Corrected package requirements
 
-## [0.1.0] - 2023-04-25
+## [0.1.0] - 2023-04-13
 
 ### Added
 - Added instrument_numbers method to Batch class to return a list of instrument numbers
 - Add govLot to acreage searches
 - Added package specific documentation
 
 ### Fixed
```

### Comparing `propertysync-0.4.0/propertysync/api.py` & `propertysync-0.4.1/propertysync/api.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.0/propertysync/batch.py` & `propertysync-0.4.1/propertysync/batch.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.0/propertysync/document.py` & `propertysync-0.4.1/propertysync/document.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.0/propertysync/search.py` & `propertysync-0.4.1/propertysync/search.py`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.0/propertysync/titlesearch_batch.py` & `propertysync-0.4.1/propertysync/titlesearch_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,20 @@
         for field in fields:
             if row[field]:
                 return True
         return False
 
     def parse_date(self, value):
         if value:
-            time = datetime.strptime(value, '%m%d%Y')
-            return time.strftime('%Y-%m-%d')
+            # try to convert value to a date, if this throws an exception, then just return the value
+            try:
+                time = datetime.strptime(value, '%m%d%Y')
+                return time.strftime('%Y-%m-%d')
+            except:
+                return value
         return value
 
     def parse_party_name(self, value):
         split_name = {
             'name_last': None,
             'name_first': None,
             'name_middle': None,
@@ -197,17 +201,21 @@
                 record_info['govLot'] = [
                     {"rangeAction": None, "rangeMax": row['lot'], "rangeMin": row['lot'], "rangePrecision": None}
                 ]
 
         record['acreageLegal'].append(record_info)
 
 
-    def convert_batch(self, batchFilePath, batchName = 'TitleSearch Batch'):
+    def convert_batch(self, batchFilePath, batchName = None):
         records = []
 
+        # if batchName is not provided, use the filename without the extension
+        if not batchName:
+            batchName = os.path.splitext(os.path.basename(batchFilePath))[0]
+
         csv.register_dialect('piper', delimiter='|', quoting=csv.QUOTE_NONE)
 
         # read batch file
         with open(batchFilePath) as csvf:
             batchReader = csv.DictReader(csvf, fieldnames=self.batch_fields, dialect='piper')
             prev_id = None
             curr_id = None
```

### Comparing `propertysync-0.4.0/LICENSE` & `propertysync-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.0/README.md` & `propertysync-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.0/pyproject.toml` & `propertysync-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propertysync-0.4.0/PKG-INFO` & `propertysync-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propertysync
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for interacting with the PropertySync API.
 Project-URL: Documentation, https://developer.propertysync.com/python/index.html
 Author-email: Rob Martinson <rob@limelyte.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

