# Comparing `tmp/pysparkler-0.4.dev1681747316.tar.gz` & `tmp/pysparkler-0.4.dev1681762692.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.4.dev1681747316.tar", max compression
+gzip compressed data, was "pysparkler-0.4.dev1681762692.tar", max compression
```

## Comparing `pysparkler-0.4.dev1681747316.tar` & `pysparkler-0.4.dev1681762692.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     9111 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/README.md
--rw-r--r--   0        0        0     1203 2023-04-17 16:01:57.251088 pysparkler-0.4.dev1681747316/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/__init__.py
--rw-r--r--   0        0        0     4374 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/api.py
--rw-r--r--   0        0        0     6057 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/cli.py
--rw-r--r--   0        0        0     2204 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10438 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4263 2023-04-17 16:01:49.046404 pysparkler-0.4.dev1681747316/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681747316/PKG-INFO
+-rw-r--r--   0        0        0     9111 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/README.md
+-rw-r--r--   0        0        0     1203 2023-04-17 20:18:12.434202 pysparkler-0.4.dev1681762692/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4490 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/api.py
+-rw-r--r--   0        0        0     6057 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/cli.py
+-rw-r--r--   0        0        0     4556 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2204 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10438 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3967 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4263 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681762692/PKG-INFO
```

### Comparing `pysparkler-0.4.dev1681747316/README.md` & `pysparkler-0.4.dev1681762692/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/pyproject.toml` & `pysparkler-0.4.dev1681762692/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.4.dev1681747316"
+version = "0.4.dev1681762692"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/__init__.py` & `pysparkler-0.4.dev1681762692/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/api.py` & `pysparkler-0.4.dev1681762692/pysparkler/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  under the License.
 #
 import json
 
 import libcst as cst
 import nbformat
 
+from pysparkler.pyspark_22_to_23 import pyspark_22_to_23_transformers
 from pysparkler.pyspark_23_to_24 import pyspark_23_to_24_transformers
 from pysparkler.pyspark_24_to_30 import pyspark_24_to_30_transformers
 from pysparkler.pyspark_31_to_32 import pyspark_31_to_32_transformers
 from pysparkler.pyspark_32_to_33 import pyspark_32_to_33_transformers
 
 
 class PySparkler:
@@ -35,14 +36,15 @@
         self.from_pyspark = from_pyspark
         self.to_pyspark = to_pyspark
         self.dry_run = dry_run
 
     @property
     def transformers(self):
         return [
+            *pyspark_22_to_23_transformers(),
             *pyspark_23_to_24_transformers(),
             *pyspark_24_to_30_transformers(),
             *pyspark_31_to_32_transformers(),
             *pyspark_32_to_33_transformers(),
         ]
 
     def upgrade_script(self, input_file: str, output_file: str | None = None) -> str:
```

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/base.py` & `pysparkler-0.4.dev1681762692/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/cli.py` & `pysparkler-0.4.dev1681762692/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.4.dev1681762692/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.4.dev1681762692/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.4.dev1681762692/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.4.dev1681762692/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681747316/PKG-INFO` & `pysparkler-0.4.dev1681762692/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.4.dev1681747316
+Version: 0.4.dev1681762692
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

