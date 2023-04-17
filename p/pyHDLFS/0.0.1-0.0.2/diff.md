# Comparing `tmp/pyhdlfs-0.0.1.tar.gz` & `tmp/pyhdlfs-0.0.2.tar.gz`

## Comparing `pyhdlfs-0.0.1.tar` & `pyhdlfs-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 pyhdlfs-0.0.1/hdlfs_doc.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhdlfs-0.0.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0    11774 2020-02-02 00:00:00.000000 pyhdlfs-0.0.1/hdlfs/hdlfs.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pyhdlfs-0.0.1/.gitignore
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 pyhdlfs-0.0.1/README.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pyhdlfs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 pyhdlfs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/hdlfs_doc.md
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/LICENSES/MIT.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/hdlfs/__init__.py
+-rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/hdlfs/hdlfs.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/tests/test_pyhdlfs.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/.gitignore
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/README.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/PKG-INFO
```

### Comparing `pyhdlfs-0.0.1/hdlfs_doc.md` & `pyhdlfs-0.0.2/hdlfs_doc.md`

 * *Files identical despite different names*

### Comparing `pyhdlfs-0.0.1/LICENSES/MIT.txt` & `pyhdlfs-0.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyhdlfs-0.0.1/hdlfs/hdlfs.py` & `pyhdlfs-0.0.2/hdlfs/hdlfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 import json
 import re
 import logging
 from pathlib import PurePath, Path
 import requests_pkcs12
 import requests
 
-from dotenv import dotenv_values
-
 logging.basicConfig(level=logging.INFO)
 
 
 def get_path_content(response: dict) -> list:
     """
     Extracts the path items from response of LISTSTATUS API
     :param response: Response from LISTSTATUS
@@ -237,65 +235,12 @@
 @hdlfs_api(method='get', operation='GETRESTORESNAPSHOTSTATUS')
 def get_operations_status(endpoint, certificate, password, token='', verify=True):
     return {'params': {'token': token},
             'headers': {'Content-Type': 'application/json'}}
 
 
 def main():
-
-    # Credentials
-    env_vals = dotenv_values('.env')
-    keystore = "config/keystore.p12"
-
-    cert = '/Users/d051079/certs/thh.crt'
-    key = '/Users/d051079/certs/thh.key'
-
-    connections_file = "config/connections.json"
-
-    with open(connections_file) as js:
-        connections = json.load(js)
-    connections = connections["CoolR"]
-    url = connections['bronze']['endpoint']
-
-    # r = list_files(url, path=path, password=key, certificate=cert, verify=False)
-    #
-    # for f in r['FileStatuses']['FileStatus']:
-    #     print(f"{f['pathSuffix']} - {f['type']}")
-
-    filenr = 10
-    file1 = f'/testdata/sub1/file{filenr}.txt'
-    r = upload(url, data='This is a test-file', path=file1, password=key, certificate=cert, verify=False)
-    print(f"Upload {file1}: {r}")
-
-    file2 = f'/testdata/file{filenr}.txt'
-    r = rename(url, path=file1, destination=file2, password=key, certificate=cert, verify=False)
-    print(f"Renaming {file1} -> {file2}: {r}")
-
-    file3 = f'/testdata/file{filenr}-copy.txt'
-    r = copy(url, path=file2, destination=file3, password=key, certificate=cert, verify=False)
-    print(f"Copy {file2} -> {file3}: {r}")
-
-    path = 'testdata'
-    r = list_path(url, path=path, password=key, certificate=cert, verify=False)
-    print(f"List Folder {path}: {get_path_content(r)}")
-
-    path_sub1 = 'testdata/sub1'
-    r = list_path(url, path=path_sub1, password=key, certificate=cert, verify=False)
-    print(f"List Folder {path_sub1}: {get_path_content(r)}")
-
-    r = file_status(url, path=file3, password=key, certificate=cert, verify=False)
-    print(f"File Status {file3}: {r}")
-
-    path = 'testdata'
-    r = list_path_recursive(url, path=path, password=key, certificate=cert, startAfter=None, verify=False)
-    print(f"List Recursive Folder {path}: {get_recursive_path_content(r)}")
-    #ic(r)
-
-    r = whoami(url, password=key, certificate=cert, verify=False)
-    print(f"Whoami: {r}")
-
-    # r = delete(url, path=file2, password=key, certificate=cert, verify=False)
-    # print(f"After \'Delete\' {file2} List Folder {path}: {get_files(r)}")
+    pass
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyhdlfs-0.0.1/.gitignore` & `pyhdlfs-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyhdlfs-0.0.1/README.md` & `pyhdlfs-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhdlfs-0.0.1/pyproject.toml` & `pyhdlfs-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests_pkcs12", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyHDLFS"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Thorsten Hapke", email="thorsten.hapke@sap.com" },
 ]
 description = "Python wrapper to SAP HDLFS API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyhdlfs-0.0.1/PKG-INFO` & `pyhdlfs-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHDLFS
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper to SAP HDLFS API
 Project-URL: Homepage, https://github.tools.sap/hda-xpm-frontrunner/pyhdlfs
 Author-email: Thorsten Hapke <thorsten.hapke@sap.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

