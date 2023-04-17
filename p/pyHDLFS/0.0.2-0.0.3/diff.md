# Comparing `tmp/pyhdlfs-0.0.2.tar.gz` & `tmp/pyhdlfs-0.0.3.tar.gz`

## Comparing `pyhdlfs-0.0.2.tar` & `pyhdlfs-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/hdlfs_doc.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/LICENSES/MIT.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/hdlfs/__init__.py
--rw-r--r--   0        0        0     9668 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/hdlfs/hdlfs.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/tests/test_pyhdlfs.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/.gitignore
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/README.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 pyhdlfs-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/hdlfs_doc.md
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/LICENSES/MIT.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/hdlfs/__init__.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/hdlfs/hdlfs.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/tests/test_pyhdlfs.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/.gitignore
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/README.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 pyhdlfs-0.0.3/PKG-INFO
```

### Comparing `pyhdlfs-0.0.2/hdlfs_doc.md` & `pyhdlfs-0.0.3/hdlfs_doc.md`

 * *Files identical despite different names*

### Comparing `pyhdlfs-0.0.2/LICENSES/MIT.txt` & `pyhdlfs-0.0.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyhdlfs-0.0.2/hdlfs/hdlfs.py` & `pyhdlfs-0.0.3/hdlfs/hdlfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             data = updated.pop('data', None)
             suffix = PurePath(certificate).suffix
             if suffix in ['.crt', '.pem']:
                 r = requests.request(method, endpoint, cert=(certificate, password), headers=headers, params=params,
                                      data=data, verify=verify)
             elif suffix in ['.pkcs12', '.p12', '.pfx']:
                 r = requests_pkcs12.request(method, endpoint, pkcs12_filename=certificate, pkcs12_password=password,
-                                            params=params, pkcs12_data=data, verify=verify)
+                                            headers=headers, params=params, data=data, verify=verify)
 
             if r.status_code not in [200, 201]:
                 raise ValueError(f"Unsuccessful API-call - Status code: {r.status_code} - {r.text}")
             return json.loads(r.text)
 
         return call_api
     return inner_hdlfs_api
```

### Comparing `pyhdlfs-0.0.2/tests/test_pyhdlfs.py` & `pyhdlfs-0.0.3/tests/test_pyhdlfs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 
 import json
 from dotenv import dotenv_values
 
 from hdlfs.hdlfs import *
 
 # Credentials
-env_vals = dotenv_values('.env')
+passphrase = dotenv_values('.env')['keystore_pwd']
 keystore = "config/keystore.p12"
 
 cert = '/Users/d051079/certs/thh.crt'
 key = '/Users/d051079/certs/thh.key'
 
+WITH_PKCS = False
+if WITH_PKCS:
+    print("With Keystore")
+    key = passphrase
+    cert = keystore
+else:
+    print("With Certificate")
+
 connections_file = "config/connections.json"
 
 with open(connections_file) as js:
     connections = json.load(js)
 connections = connections["CoolR"]
 url = connections['bronze']['endpoint']
```

### Comparing `pyhdlfs-0.0.2/.gitignore` & `pyhdlfs-0.0.3/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Local Mac
 .DS_Store
 config/
+.idea
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `pyhdlfs-0.0.2/README.md` & `pyhdlfs-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # PyHDLFS
 
 PythonAPI for SAP HDLFS using the [RestAPI](https://help.sap.com/doc/9d084a41830f46d6904fd4c23cd4bbfa/2023_1_QRC/en-US/html/index.html)
 
-Status: In Progress, unsupported
+For authentication both options are supported: key/certification and keystore/passphrase. The suffix of the certification 
+file is used for selecting the authentication method. 
 
-by Thorsten Hapke, thorsten.hapke@sap.com
+- Certification: .crt or .pem
+- Keystore: .pkcs12, .p12 or .pfx
 
+Status: In Progress, unsupported
 
-[Documentation](hdlfs_doc.md)
+[Generated Documentation](hdlfs_doc.md) 
 
 # Table of Contents
 
 * [hdlfs](#hdlfs)
   * [get\_path\_content](#hdlfs.get_path_content)
   * [get\_recursive\_path\_content](#hdlfs.get_recursive_path_content)
   * [hdlfs\_api](#hdlfs.hdlfs_api)
@@ -21,17 +24,14 @@
   * [delete](#hdlfs.delete)
   * [file\_status](#hdlfs.file_status)
   * [list\_path](#hdlfs.list_path)
   * [list\_path\_recursive](#hdlfs.list_path_recursive)
   * [whoami](#hdlfs.whoami)
   * [get\_operations\_status](#hdlfs.get_operations_status)
 
-<a id="__init__"></a>
-
-# \_\_init\_\_
 
 <a id="hdlfs"></a>
 
 # hdlfs
 
 <a id="hdlfs.get_path_content"></a>
```

### Comparing `pyhdlfs-0.0.2/pyproject.toml` & `pyhdlfs-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "requests_pkcs12", "requests"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyHDLFS"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Thorsten Hapke", email="thorsten.hapke@sap.com" },
 ]
 description = "Python wrapper to SAP HDLFS API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyhdlfs-0.0.2/PKG-INFO` & `pyhdlfs-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: pyHDLFS
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python wrapper to SAP HDLFS API
 Project-URL: Homepage, https://github.tools.sap/hda-xpm-frontrunner/pyhdlfs
 Author-email: Thorsten Hapke <thorsten.hapke@sap.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # PyHDLFS
 
 PythonAPI for SAP HDLFS using the [RestAPI](https://help.sap.com/doc/9d084a41830f46d6904fd4c23cd4bbfa/2023_1_QRC/en-US/html/index.html)
 
-Status: In Progress, unsupported
+For authentication both options are supported: key/certification and keystore/passphrase. The suffix of the certification 
+file is used for selecting the authentication method. 
 
-by Thorsten Hapke, thorsten.hapke@sap.com
+- Certification: .crt or .pem
+- Keystore: .pkcs12, .p12 or .pfx
 
+Status: In Progress, unsupported
 
-[Documentation](hdlfs_doc.md)
+[Generated Documentation](hdlfs_doc.md) 
 
 # Table of Contents
 
 * [hdlfs](#hdlfs)
   * [get\_path\_content](#hdlfs.get_path_content)
   * [get\_recursive\_path\_content](#hdlfs.get_recursive_path_content)
   * [hdlfs\_api](#hdlfs.hdlfs_api)
@@ -33,17 +36,14 @@
   * [delete](#hdlfs.delete)
   * [file\_status](#hdlfs.file_status)
   * [list\_path](#hdlfs.list_path)
   * [list\_path\_recursive](#hdlfs.list_path_recursive)
   * [whoami](#hdlfs.whoami)
   * [get\_operations\_status](#hdlfs.get_operations_status)
 
-<a id="__init__"></a>
-
-# \_\_init\_\_
 
 <a id="hdlfs"></a>
 
 # hdlfs
 
 <a id="hdlfs.get_path_content"></a>
```

