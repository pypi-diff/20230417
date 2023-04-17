# Comparing `tmp/macrometa-source-postgres-0.0.39.tar.gz` & `tmp/macrometa-source-postgres-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.39.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.40.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.39.tar` & `macrometa-source-postgres-0.0.40.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/LICENSE
--rw-r--r--   0        0        0    35130 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28921 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3650 2023-04-04 15:44:47.614923 macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1510 2023-04-04 15:44:47.950925 macrometa-source-postgres-0.0.39/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.39/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.39/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/LICENSE
+-rw-r--r--   0        0        0    35130 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     8974 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28921 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3650 2023-04-17 02:54:52.210824 macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1510 2023-04-17 02:54:52.450822 macrometa-source-postgres-0.0.40/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.40/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.40/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.39/LICENSE` & `macrometa-source-postgres-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.40/macrometa_source_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.40/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.40/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.40/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.39/pyproject.toml` & `macrometa-source-postgres-0.0.40/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.39'
+version='0.0.40'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
@@ -24,15 +24,15 @@
     { include = "macrometa_source_postgres" },
     { include = "sync_strategies", from = "macrometa_source_postgres" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.11"
 pipelinewise-singer-python = "1.2.0"
-c8connector = "0.0.15"
+c8connector = "0.0.19"
 psycopg2-binary = "2.9.3"
 strict-rfc3339 = "0.7"
 
 [tool.poetry.scripts]
 # CLI declaration
 macrometa-source-postgres = 'macrometa_source_postgres:main'
```

### Comparing `macrometa-source-postgres-0.0.39/setup.py` & `macrometa-source-postgres-0.0.40/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,26 +9,26 @@
  'macrometa_source_postgres.sync_strategies',
  'sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector==0.0.15',
+['c8connector==0.0.19',
  'pipelinewise-singer-python==1.2.0',
  'psycopg2-binary==2.9.3',
  'strict-rfc3339==0.7']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.39',
+    'version': '0.0.40',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.39/PKG-INFO` & `macrometa-source-postgres-0.0.40/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.39
+Version: 0.0.40
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: c8connector (==0.0.15)
+Requires-Dist: c8connector (==0.0.19)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: psycopg2-binary (==2.9.3)
 Requires-Dist: strict-rfc3339 (==0.7)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-postgres/issues
```

