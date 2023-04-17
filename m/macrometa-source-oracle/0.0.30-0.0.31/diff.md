# Comparing `tmp/macrometa-source-oracle-0.0.30.tar.gz` & `tmp/macrometa-source-oracle-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-oracle-0.0.30.tar", max compression
+gzip compressed data, was "macrometa-source-oracle-0.0.31.tar", max compression
```

## Comparing `macrometa-source-oracle-0.0.30.tar` & `macrometa-source-oracle-0.0.31.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     9713 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/LICENSE
--rw-r--r--   0        0        0     1715 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/README.md
--rw-r--r--   0        0        0    42351 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/macrometa_source_oracle/__init__.py
--rwxr-xr-x   0        0        0     7417 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/macrometa_source_oracle/connection.py
--rwxr-xr-x   0        0        0        0 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/macrometa_source_oracle/sync_strategies/__init__.py
--rwxr-xr-x   0        0        0     4779 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/macrometa_source_oracle/sync_strategies/common.py
--rwxr-xr-x   0        0        0     4874 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/macrometa_source_oracle/sync_strategies/full_table.py
--rwxr-xr-x   0        0        0    17662 2023-04-04 16:13:09.361228 macrometa-source-oracle-0.0.30/macrometa_source_oracle/sync_strategies/log_based.py
--rw-r--r--   0        0        0     1561 2023-04-04 16:13:09.433230 macrometa-source-oracle-0.0.30/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.30/setup.py
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.30/PKG-INFO
+-rwxr-xr-x   0        0        0     9713 2023-04-17 02:54:19.725700 macrometa-source-oracle-0.0.31/LICENSE
+-rw-r--r--   0        0        0     1715 2023-04-17 02:54:19.725700 macrometa-source-oracle-0.0.31/README.md
+-rw-r--r--   0        0        0    42351 2023-04-17 02:54:19.729700 macrometa-source-oracle-0.0.31/macrometa_source_oracle/__init__.py
+-rwxr-xr-x   0        0        0     7417 2023-04-17 02:54:19.729700 macrometa-source-oracle-0.0.31/macrometa_source_oracle/connection.py
+-rwxr-xr-x   0        0        0        0 2023-04-17 02:54:19.729700 macrometa-source-oracle-0.0.31/macrometa_source_oracle/sync_strategies/__init__.py
+-rwxr-xr-x   0        0        0     4779 2023-04-17 02:54:19.729700 macrometa-source-oracle-0.0.31/macrometa_source_oracle/sync_strategies/common.py
+-rwxr-xr-x   0        0        0     4874 2023-04-17 02:54:19.729700 macrometa-source-oracle-0.0.31/macrometa_source_oracle/sync_strategies/full_table.py
+-rwxr-xr-x   0        0        0    17662 2023-04-17 02:54:19.729700 macrometa-source-oracle-0.0.31/macrometa_source_oracle/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     1561 2023-04-17 02:54:19.809700 macrometa-source-oracle-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.31/setup.py
+-rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 macrometa-source-oracle-0.0.31/PKG-INFO
```

### Comparing `macrometa-source-oracle-0.0.30/LICENSE` & `macrometa-source-oracle-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.30/README.md` & `macrometa-source-oracle-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.30/macrometa_source_oracle/__init__.py` & `macrometa-source-oracle-0.0.31/macrometa_source_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.30/macrometa_source_oracle/connection.py` & `macrometa-source-oracle-0.0.31/macrometa_source_oracle/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.30/macrometa_source_oracle/sync_strategies/common.py` & `macrometa-source-oracle-0.0.31/macrometa_source_oracle/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.30/macrometa_source_oracle/sync_strategies/full_table.py` & `macrometa-source-oracle-0.0.31/macrometa_source_oracle/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.30/macrometa_source_oracle/sync_strategies/log_based.py` & `macrometa-source-oracle-0.0.31/macrometa_source_oracle/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-oracle-0.0.30/pyproject.toml` & `macrometa-source-oracle-0.0.31/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-oracle"
-version='0.0.30'
+version='0.0.31'
 description = "Macrometa source oracle connector for reading from oracle databases."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 readme = "README.md"
 homepage = "https://www.macrometa.com/"
 keywords = [
     "ELT",
@@ -25,15 +25,15 @@
 ]
 packages = [
     { include = "macrometa_source_oracle" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-c8connector = "0.0.15"
+c8connector = "0.0.19"
 pipelinewise-singer-python = "1.2.0"
 oracledb = "^1.2.2"
 strict-rfc3339 = "^0.7"
 
 [tool.poetry.scripts]
 macrometa-source-oracle = "macrometa_source_oracle:main"
```

### Comparing `macrometa-source-oracle-0.0.30/setup.py` & `macrometa-source-oracle-0.0.31/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['macrometa_source_oracle', 'macrometa_source_oracle.sync_strategies']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['c8connector==0.0.15',
+['c8connector==0.0.19',
  'oracledb>=1.2.2,<2.0.0',
  'pipelinewise-singer-python==1.2.0',
  'strict-rfc3339>=0.7,<0.8']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-oracle = macrometa_source_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-oracle',
-    'version': '0.0.30',
+    'version': '0.0.31',
     'description': 'Macrometa source oracle connector for reading from oracle databases.',
     'long_description': '# macrometa-source-oracle\n\nMacrometa source connector that extracts data from a [Oracle](https://www.oracle.com/database/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).\n\n## How to use it\n\n### Install and Run\n\nFirst, make sure Python 3 is installed on your system or follow these\ninstallation instructions for [Mac](http://docs.python-guide.org/en/latest/starting/install3/osx/) or\n[Ubuntu](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-local-programming-environment-on-ubuntu-16-04).\n\n\nIt\'s recommended to use a virtualenv:\n\n```bash\n  python3 -m venv venv\n  pip install macrometa-source-oracle\n```\n\nor from source using,\n1. Install poetry using https://python-poetry.org/docs/#installation\n2. Run \n    ```bash\n    poetry build\n    pip install dist/macrometa_source_oracle-<version>*.whl\n    ```\n\n### Configuration\n\nRunning the the macrometa source connector independently requires a `config.json` file. \n\nExample configuration:\n\n```json\n{\n  "host": "dev.oracledb.io",\n  "port": 1521,\n  "user": "C##HELLO",\n  "password": "password",\n  "service_name": "ORCLCDB",\n  "filter_schema": "C##HELLO",\n  "filter_table": "CUSTOMERS",\n  "default_replication_method": "LOG_BASED",\n  "pdb_name": "ORCLPDB1",\n  "multitenant": true,\n  "scn_window_size": 10\n}\n```\n\nYou can run a discover run using the previous `config.json` file to acquire all the tables definition\n \n```\nmacrometa-source-oracle --config /tmp/config.json --discover >> /tmp/catalog.json\n```\n\nThen use the catalog.json to run a full export:\n\n```\nmacrometa-source-oracle --config /tmp/config.json --catalog /tmp/catalog.json\n```\n\n',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.macrometa.com/',
```

### Comparing `macrometa-source-oracle-0.0.30/PKG-INFO` & `macrometa-source-oracle-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-oracle
-Version: 0.0.30
+Version: 0.0.31
 Summary: Macrometa source oracle connector for reading from oracle databases.
 Home-page: https://www.macrometa.com/
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Oracle,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: c8connector (==0.0.15)
+Requires-Dist: c8connector (==0.0.19)
 Requires-Dist: oracledb (>=1.2.2,<2.0.0)
 Requires-Dist: pipelinewise-singer-python (==1.2.0)
 Requires-Dist: strict-rfc3339 (>=0.7,<0.8)
 Project-URL: Bug Tracker, https://github.com/Macrometacorp/macrometa-source-oracle/issues
 Description-Content-Type: text/markdown
 
 # macrometa-source-oracle
```

