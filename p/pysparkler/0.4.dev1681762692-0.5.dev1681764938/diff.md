# Comparing `tmp/pysparkler-0.4.dev1681762692.tar.gz` & `tmp/pysparkler-0.5.dev1681764938.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.4.dev1681762692.tar", max compression
+gzip compressed data, was "pysparkler-0.5.dev1681764938.tar", max compression
```

## Comparing `pysparkler-0.4.dev1681762692.tar` & `pysparkler-0.5.dev1681764938.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     9111 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/README.md
--rw-r--r--   0        0        0     1203 2023-04-17 20:18:12.434202 pysparkler-0.4.dev1681762692/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/__init__.py
--rw-r--r--   0        0        0     4490 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/api.py
--rw-r--r--   0        0        0     6057 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/cli.py
--rw-r--r--   0        0        0     4556 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2204 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10438 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4263 2023-04-17 20:18:05.666027 pysparkler-0.4.dev1681762692/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681762692/PKG-INFO
+-rw-r--r--   0        0        0     9111 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/README.md
+-rw-r--r--   0        0        0     1203 2023-04-17 20:55:38.407690 pysparkler-0.5.dev1681764938/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4490 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/api.py
+-rw-r--r--   0        0        0     6057 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/cli.py
+-rw-r--r--   0        0        0     4556 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2204 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10438 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3967 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4263 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.5.dev1681764938/PKG-INFO
```

### Comparing `pysparkler-0.4.dev1681762692/README.md` & `pysparkler-0.5.dev1681764938/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 |-------------------------------------------------|-----------|----------------------------------------------------------------------------------------------------------------------------------------------|
 | Upgrading from PySpark 3.3 to 3.4               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-3-to-3-4)               |
 | Upgrading from PySpark 3.2 to 3.3               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-2-to-3-3)               |
 | Upgrading from PySpark 3.1 to 3.2               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-1-to-3-2)               |
 | Upgrading from PySpark 2.4 to 3.0               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-4-to-3-0)               |
 | Upgrading from PySpark 2.3 to 2.4               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-to-2-4)               |
 | Upgrading from PySpark 2.3.0 to 2.3.1 and above | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-0-to-2-3-1-and-above) |
-| Upgrading from PySpark 2.2 to 2.3               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-2-to-2-3)               |
+| Upgrading from PySpark 2.2 to 2.3               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-2-to-2-3)               |
 | Upgrading from PySpark 1.4 to 1.5               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-4-to-1-5)               |
 | Upgrading from PySpark 1.0-1.2 to 1.3           | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-0-1-2-to-1-3)           |
 
 ## Features Supported
 
 The tool supports the following features:
```

### Comparing `pysparkler-0.4.dev1681762692/pyproject.toml` & `pysparkler-0.5.dev1681764938/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.4.dev1681762692"
+version = "0.5.dev1681764938"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/__init__.py` & `pysparkler-0.5.dev1681764938/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/api.py` & `pysparkler-0.5.dev1681764938/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/base.py` & `pysparkler-0.5.dev1681764938/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/cli.py` & `pysparkler-0.5.dev1681764938/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.5.dev1681764938/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.5.dev1681764938/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.5.dev1681764938/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.5.dev1681764938/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.5.dev1681764938/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681762692/PKG-INFO` & `pysparkler-0.5.dev1681764938/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.4.dev1681762692
+Version: 0.5.dev1681764938
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
@@ -52,15 +52,15 @@
 |-------------------------------------------------|-----------|----------------------------------------------------------------------------------------------------------------------------------------------|
 | Upgrading from PySpark 3.3 to 3.4               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-3-to-3-4)               |
 | Upgrading from PySpark 3.2 to 3.3               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-2-to-3-3)               |
 | Upgrading from PySpark 3.1 to 3.2               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-1-to-3-2)               |
 | Upgrading from PySpark 2.4 to 3.0               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-4-to-3-0)               |
 | Upgrading from PySpark 2.3 to 2.4               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-to-2-4)               |
 | Upgrading from PySpark 2.3.0 to 2.3.1 and above | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-0-to-2-3-1-and-above) |
-| Upgrading from PySpark 2.2 to 2.3               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-2-to-2-3)               |
+| Upgrading from PySpark 2.2 to 2.3               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-2-to-2-3)               |
 | Upgrading from PySpark 1.4 to 1.5               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-4-to-1-5)               |
 | Upgrading from PySpark 1.0-1.2 to 1.3           | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-0-1-2-to-1-3)           |
 
 ## Features Supported
 
 The tool supports the following features:
```

