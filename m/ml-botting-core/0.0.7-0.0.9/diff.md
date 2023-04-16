# Comparing `tmp/ml_botting_core-0.0.7.tar.gz` & `tmp/ml_botting_core-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-0.0.7.tar", last modified: Sun Apr 16 22:55:38 2023, max compression
+gzip compressed data, was "ml_botting_core-0.0.9.tar", last modified: Sun Apr 16 23:17:04 2023, max compression
```

## Comparing `ml_botting_core-0.0.7.tar` & `ml_botting_core-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.735451 ml_botting_core-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/classification/universal_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/regression/universal_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/universal_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/classification/universal_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/regression/universal_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/src/ml_botting_core/universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.254568 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 23:17:04.000000 ml_botting_core-0.0.9/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:17:04.258569 ml_botting_core-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 23:16:36.000000 ml_botting_core-0.0.9/tests/test_init.py
```

### Comparing `ml_botting_core-0.0.7/LICENSE` & `ml_botting_core-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml_botting_core-0.0.7/PKG-INFO` & `ml_botting_core-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_botting_core
-Version: 0.0.7
+Version: 0.0.9
 Summary: Making ML more accessible to botting apps
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml_botting_core-0.0.7/setup.cfg` & `ml_botting_core-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ml_botting_core
-version = 0.0.7
+version = 0.0.9
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml_botting_core
 project_urls =
```

### Comparing `ml_botting_core-0.0.7/src/ml_botting_core/universal_predictor.py` & `ml_botting_core-0.0.9/src/ml_botting_core/universal_predictor.py`

 * *Files identical despite different names*

### Comparing `ml_botting_core-0.0.7/src/ml_botting_core.egg-info/PKG-INFO` & `ml_botting_core-0.0.9/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-botting-core
-Version: 0.0.7
+Version: 0.0.9
 Summary: Making ML more accessible to botting apps
 Home-page: https://github.com/darkmatter2222/ml_botting_core
 Author: Ryan Susman
 Author-email: ryansusman@gmail.com
 Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

