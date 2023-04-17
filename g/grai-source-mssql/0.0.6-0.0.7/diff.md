# Comparing `tmp/grai_source_mssql-0.0.6.tar.gz` & `tmp/grai_source_mssql-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_mssql-0.0.6.tar", max compression
+gzip compressed data, was "grai_source_mssql-0.0.7.tar", max compression
```

## Comparing `grai_source_mssql-0.0.6.tar` & `grai_source_mssql-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      685 2023-03-24 13:31:20.633291 grai_source_mssql-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      139 2023-02-13 20:16:22.722173 grai_source_mssql-0.0.6/src/grai_source_mssql/__init__.py
--rw-r--r--   0        0        0     6235 2023-03-23 17:15:13.134256 grai_source_mssql-0.0.6/src/grai_source_mssql/adapters.py
--rw-r--r--   0        0        0     1302 2023-02-13 20:16:22.722839 grai_source_mssql-0.0.6/src/grai_source_mssql/base.py
--rw-r--r--   0        0        0    10658 2023-02-14 16:39:18.548229 grai_source_mssql-0.0.6/src/grai_source_mssql/loader.py
--rw-r--r--   0        0        0     4298 2023-02-14 16:39:18.548342 grai_source_mssql-0.0.6/src/grai_source_mssql/models.py
--rw-r--r--   0        0        0      180 2023-02-13 20:16:22.723121 grai_source_mssql-0.0.6/src/grai_source_mssql/package_definitions.py
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.6/setup.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      685 2023-04-17 19:09:03.819395 grai_source_mssql-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-02-13 20:16:22.722173 grai_source_mssql-0.0.7/src/grai_source_mssql/__init__.py
+-rw-r--r--   0        0        0     6355 2023-04-17 19:09:03.819560 grai_source_mssql-0.0.7/src/grai_source_mssql/adapters.py
+-rw-r--r--   0        0        0     1302 2023-02-13 20:16:22.722839 grai_source_mssql-0.0.7/src/grai_source_mssql/base.py
+-rw-r--r--   0        0        0    10658 2023-02-14 16:39:18.548229 grai_source_mssql-0.0.7/src/grai_source_mssql/loader.py
+-rw-r--r--   0        0        0     4298 2023-02-14 16:39:18.548342 grai_source_mssql-0.0.7/src/grai_source_mssql/models.py
+-rw-r--r--   0        0        0      180 2023-02-13 20:16:22.723121 grai_source_mssql-0.0.7/src/grai_source_mssql/package_definitions.py
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.7/setup.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_mssql-0.0.7/PKG-INFO
```

### Comparing `grai_source_mssql-0.0.6/pyproject.toml` & `grai_source_mssql-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_mssql"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_mssql", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_mssql-0.0.6/src/grai_source_mssql/adapters.py` & `grai_source_mssql-0.0.7/src/grai_source_mssql/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,21 @@
     data = {
         "schema": current.table_schema,
     }
     return data
 
 
 def build_metadata(obj, version):
+    integration_meta = build_app_metadata(obj, version)
+    base_metadata = build_grai_metadata(obj, version)
+    integration_meta["grai"] = base_metadata
+
     return {
-        base_config.metadata_id: build_grai_metadata(obj, version),
-        config.metadata_id: build_app_metadata(obj, version),
+        base_config.metadata_id: base_metadata,
+        config.metadata_id: integration_meta,
     }
 
 
 @multimethod
 def adapt_to_client(current: Any, desired: Any):
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
```

### Comparing `grai_source_mssql-0.0.6/src/grai_source_mssql/base.py` & `grai_source_mssql-0.0.7/src/grai_source_mssql/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.6/src/grai_source_mssql/loader.py` & `grai_source_mssql-0.0.7/src/grai_source_mssql/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.6/src/grai_source_mssql/models.py` & `grai_source_mssql-0.0.7/src/grai_source_mssql/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_mssql-0.0.6/setup.py` & `grai_source_mssql-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'grai-schemas>=0.1.8,<0.2.0',
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
  'pyodbc>=4.0.35,<5.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-mssql',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_mssql-0.0.6/PKG-INFO` & `grai_source_mssql-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-mssql
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

