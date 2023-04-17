# Comparing `tmp/macrometa-source-mongo-0.0.32.tar.gz` & `tmp/macrometa-source-mongo-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.32.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.33.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.32.tar` & `macrometa-source-mongo-0.0.33.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/LICENSE
--rw-r--r--   0        0        0    21337 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6470 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0     1151 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     8097 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     6267 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-04-17 02:53:48.378630 macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1546 2023-04-17 02:53:48.618631 macrometa-source-mongo-0.0.32/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.32/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.32/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/LICENSE
+-rw-r--r--   0        0        0    21337 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6470 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0     1151 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     8097 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-04-17 09:51:24.291643 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-04-17 09:51:24.295642 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     6267 2023-04-17 09:51:24.295642 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-04-17 09:51:24.295642 macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-04-17 09:51:24.531543 macrometa-source-mongo-0.0.33/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.33/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.33/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.32/LICENSE` & `macrometa-source-mongo-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.33/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.32/pyproject.toml` & `macrometa-source-mongo-0.0.33/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.32'
+version='0.0.33'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -24,15 +24,15 @@
     { include = "macrometa_source_mongo" },
     { include = "sync_strategies", from = "macrometa_source_mongo" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = "0.0.19"
+c8connector = ">=0.0.20"
 pymongo = {version = "^4.0",extras = ["srv"]}
 tzlocal = "2.1.*"
 terminaltables = "3.1.*"
 dnspython = "2.1.*"
 
 [tool.poetry.scripts]
 # CLI declaration
```

### Comparing `macrometa-source-mongo-0.0.32/setup.py` & `macrometa-source-mongo-0.0.33/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
  'macrometa_source_mongo.sync_strategies',
  'sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector==0.0.19',
+['c8connector>=0.0.20',
  'dnspython>=2.1.0,<2.2.0',
  'pipelinewise-singer-python==1.2.0',
  'pymongo[srv]>=4.0,<5.0',
  'terminaltables>=3.1.0,<3.2.0',
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.32',
+    'version': '0.0.33',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.32/PKG-INFO` & `macrometa-source-mongo-0.0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.32
+Version: 0.0.33
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: c8connector (==0.0.19)
+Requires-Dist: c8connector (>=0.0.20)
 Requires-Dist: dnspython (>=2.1.0,<2.2.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: pymongo[srv] (>=4.0,<5.0)
 Requires-Dist: terminaltables (>=3.1.0,<3.2.0)
 Requires-Dist: tzlocal (>=2.1.0,<2.2.0)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-mongo/issues
```

