# Comparing `tmp/grai_source_fivetran-0.0.2.tar.gz` & `tmp/grai_source_fivetran-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.0.2.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.0.3.tar", max compression
```

## Comparing `grai_source_fivetran-0.0.2.tar` & `grai_source_fivetran-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      879 2023-03-24 13:31:01.178811 grai_source_fivetran-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.2/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     6418 2023-03-23 17:36:29.525139 grai_source_fivetran-0.0.2/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     1425 2023-02-14 16:39:18.543003 grai_source_fivetran-0.0.2/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.2/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.2/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.2/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    12057 2023-02-14 16:39:18.545562 grai_source_fivetran-0.0.2/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.2/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.2/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.2/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.2/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.2/setup.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      879 2023-04-17 19:09:03.815258 grai_source_fivetran-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-02-14 16:39:18.542655 grai_source_fivetran-0.0.3/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     6538 2023-04-17 19:09:03.815632 grai_source_fivetran-0.0.3/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     1425 2023-02-14 16:39:18.543003 grai_source_fivetran-0.0.3/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.543040 grai_source_fivetran-0.0.3/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   436632 2023-02-14 16:39:18.545031 grai_source_fivetran-0.0.3/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    42232 2023-02-14 16:39:18.545359 grai_source_fivetran-0.0.3/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    12057 2023-02-14 16:39:18.545562 grai_source_fivetran-0.0.3/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     1668 2023-02-14 16:39:18.545711 grai_source_fivetran-0.0.3/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     4751 2023-02-14 16:39:18.545877 grai_source_fivetran-0.0.3/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      186 2023-02-14 16:39:18.546106 grai_source_fivetran-0.0.3/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 16:39:18.546143 grai_source_fivetran-0.0.3/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.3/setup.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 grai_source_fivetran-0.0.3/PKG-INFO
```

### Comparing `grai_source_fivetran-0.0.2/pyproject.toml` & `grai_source_fivetran-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 [tool.poetry.dependencies]
```

### Comparing `grai_source_fivetran-0.0.2/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.0.3/src/grai_source_fivetran/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,21 @@
     data = {
         "schema": current.schema_name,
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

### Comparing `grai_source_fivetran-0.0.2/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.0.3/src/grai_source_fivetran/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.2/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.0.3/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.2/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.0.3/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.2/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.0.3/src/grai_source_fivetran/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.2/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.0.3/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.2/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.0.3/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.0.2/setup.py` & `grai_source_fivetran-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'multimethod>=1.8,<2.0',
  'pydantic>=1.9.1,<2.0.0',
  'python-dotenv>=0.21.1,<0.22.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'grai-source-fivetran',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': 'None',
     'author': 'Ian Eaves',
     'author_email': 'ian@grai.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `grai_source_fivetran-0.0.2/PKG-INFO` & `grai_source_fivetran-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

