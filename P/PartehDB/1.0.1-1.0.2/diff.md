# Comparing `tmp/PartehDB-1.0.1.tar.gz` & `tmp/PartehDB-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PartehDB-1.0.1.tar", last modified: Mon Apr 17 00:09:33 2023, max compression
+gzip compressed data, was "PartehDB-1.0.2.tar", last modified: Mon Apr 17 01:18:03 2023, max compression
```

## Comparing `PartehDB-1.0.1.tar` & `PartehDB-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 00:09:34.000000 PartehDB-1.0.1/
--rw-rw-rw-   0        0        0     1093 2023-04-17 00:06:48.000000 PartehDB-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      659 2023-04-17 00:09:34.000000 PartehDB-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-04-17 00:05:38.000000 PartehDB-1.0.1/README.md
--rw-rw-rw-   0        0        0      642 2023-04-17 00:00:20.000000 PartehDB-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 00:09:34.000000 PartehDB-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 00:09:34.000000 PartehDB-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 00:09:34.000000 PartehDB-1.0.1/src/PartehDB/
--rw-rw-rw-   0        0        0        0 2023-04-16 23:53:08.000000 PartehDB-1.0.1/src/PartehDB/__init__.py
--rw-rw-rw-   0        0        0      704 2023-04-17 00:05:52.000000 PartehDB-1.0.1/src/PartehDB/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 00:09:34.000000 PartehDB-1.0.1/src/PartehDB.egg-info/
--rw-rw-rw-   0        0        0      659 2023-04-17 00:09:34.000000 PartehDB-1.0.1/src/PartehDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-04-17 00:09:34.000000 PartehDB-1.0.1/src/PartehDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 00:09:34.000000 PartehDB-1.0.1/src/PartehDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 00:09:34.000000 PartehDB-1.0.1/src/PartehDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 01:18:04.000000 PartehDB-1.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-04-17 00:06:48.000000 PartehDB-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      659 2023-04-17 01:18:04.000000 PartehDB-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-04-17 00:05:38.000000 PartehDB-1.0.2/README.md
+-rw-rw-rw-   0        0        0      642 2023-04-17 01:13:12.000000 PartehDB-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 01:18:04.000000 PartehDB-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 01:18:04.000000 PartehDB-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 01:18:04.000000 PartehDB-1.0.2/src/PartehDB/
+-rw-rw-rw-   0        0        0       25 2023-04-17 01:14:10.000000 PartehDB-1.0.2/src/PartehDB/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-04-17 00:05:52.000000 PartehDB-1.0.2/src/PartehDB/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:18:04.000000 PartehDB-1.0.2/src/PartehDB.egg-info/
+-rw-rw-rw-   0        0        0      659 2023-04-17 01:18:04.000000 PartehDB-1.0.2/src/PartehDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-17 01:18:04.000000 PartehDB-1.0.2/src/PartehDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:18:04.000000 PartehDB-1.0.2/src/PartehDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 01:18:04.000000 PartehDB-1.0.2/src/PartehDB.egg-info/top_level.txt
```

### Comparing `PartehDB-1.0.1/LICENSE` & `PartehDB-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PartehDB-1.0.1/PKG-INFO` & `PartehDB-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PartehDB
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python library that lets you create a custom database.
 Author-email: PartehPackages <parteh0754.coding.guy@gmail.com>
 Project-URL: Homepage, https://www.youtube.com/watch?v=a3Z7zEc7AXQ
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=a3Z7zEc7AXQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PartehDB-1.0.1/pyproject.toml` & `PartehDB-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "PartehDB"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="PartehPackages", email="parteh0754.coding.guy@gmail.com" },
 ]
 description = "A python library that lets you create a custom database."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `PartehDB-1.0.1/src/PartehDB/main.py` & `PartehDB-1.0.2/src/PartehDB/main.py`

 * *Files identical despite different names*

### Comparing `PartehDB-1.0.1/src/PartehDB.egg-info/PKG-INFO` & `PartehDB-1.0.2/src/PartehDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PartehDB
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python library that lets you create a custom database.
 Author-email: PartehPackages <parteh0754.coding.guy@gmail.com>
 Project-URL: Homepage, https://www.youtube.com/watch?v=a3Z7zEc7AXQ
 Project-URL: Bug Tracker, https://www.youtube.com/watch?v=a3Z7zEc7AXQ
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

