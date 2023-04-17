# Comparing `tmp/macrometa-target-collection-0.0.53.tar.gz` & `tmp/macrometa-target-collection-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.53.tar", last modified: Wed Apr 12 18:13:16 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.54.tar", last modified: Mon Apr 17 02:56:42 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.53.tar` & `macrometa-target-collection-0.0.54.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:13:16.749469 macrometa-target-collection-0.0.53/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13888 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 18:13:16.000000 macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 18:12:57.000000 macrometa-target-collection-0.0.53/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 18:13:16.753469 macrometa-target-collection-0.0.53/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:56:42.577530 macrometa-target-collection-0.0.54/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-17 02:56:13.000000 macrometa-target-collection-0.0.54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-17 02:56:42.577530 macrometa-target-collection-0.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 02:56:13.000000 macrometa-target-collection-0.0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:56:42.577530 macrometa-target-collection-0.0.54/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-17 02:56:13.000000 macrometa-target-collection-0.0.54/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13888 2023-04-17 02:56:13.000000 macrometa-target-collection-0.0.54/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:56:42.577530 macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-17 02:56:42.000000 macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-17 02:56:42.000000 macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:56:42.000000 macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 02:56:42.000000 macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 02:56:42.000000 macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 02:56:42.000000 macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-17 02:56:13.000000 macrometa-target-collection-0.0.54/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 02:56:42.577530 macrometa-target-collection-0.0.54/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.53/LICENSE` & `macrometa-target-collection-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.53/PKG-INFO` & `macrometa-target-collection-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.53
+Version: 0.0.54
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.53/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.54/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.53/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.54/macrometa_target_collection/main.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.53/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.54/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.53
+Version: 0.0.54
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.53/pyproject.toml` & `macrometa-target-collection-0.0.54/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.53"
+version = "0.0.54"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     'pipelinewise-singer-python==1.2.0',
     'adjust-precision-for-schema==0.3.4',
     'pyc8==0.17.1',
-    'c8connector==0.0.15',
+    'c8connector==0.0.19',
     'prometheus-client==0.16.0'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Operating System :: OS Independent",
 ]
```

