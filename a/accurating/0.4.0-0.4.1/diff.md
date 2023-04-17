# Comparing `tmp/accurating-0.4.0.tar.gz` & `tmp/accurating-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.0.tar", max compression
+gzip compressed data, was "accurating-0.4.1.tar", max compression
```

## Comparing `accurating-0.4.0.tar` & `accurating-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.0/LICENSE
--rw-r--r--   0        0        0     5964 2023-04-16 21:30:01.981248 accurating-0.4.0/README.md
--rw-r--r--   0        0        0      113 2023-04-17 00:59:29.785562 accurating-0.4.0/accurating/__init__.py
--rw-r--r--   0        0        0     8271 2023-04-17 01:12:08.446217 accurating-0.4.0/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.0/accurating/tests/__init__.py
--rw-r--r--   0        0        0     2152 2023-04-17 03:27:19.264149 accurating-0.4.0/accurating/tests/model_test.py
--rw-r--r--   0        0        0      517 2023-04-17 03:30:40.900862 accurating-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6417 1970-01-01 00:00:00.000000 accurating-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5964 2023-04-16 21:30:01.981248 accurating-0.4.1/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.1/accurating/__init__.py
+-rw-r--r--   0        0        0     8271 2023-04-17 01:12:08.446217 accurating-0.4.1/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.1/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     2152 2023-04-17 03:27:19.264149 accurating-0.4.1/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      632 2023-04-17 04:10:00.673880 accurating-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6611 1970-01-01 00:00:00.000000 accurating-0.4.1/PKG-INFO
```

### Comparing `accurating-0.4.0/LICENSE` & `accurating-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.0/README.md` & `accurating-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `accurating-0.4.0/accurating/model.py` & `accurating-0.4.1/accurating/model.py`

 * *Files identical despite different names*

### Comparing `accurating-0.4.0/accurating/tests/model_test.py` & `accurating-0.4.1/accurating/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `accurating-0.4.0/pyproject.toml` & `accurating-0.4.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
-name = "accurating"
-version = "0.4.0"
-description = ""
+name = "AccuRating"
+version = "0.4.1"
+description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
+homepage = "https://github.com/lukaszlew/accurating"
+documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jax = "^0.4.8"
 pytest = "^6.2.5"
 jaxlib = "^0.4.7"
 
@@ -18,10 +20,7 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
-
-[project.urls]
-"Homepage" = "https://github.com/lukaszlew/accurating"
```

### Comparing `accurating-0.4.0/PKG-INFO` & `accurating-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.0
-Summary: 
+Version: 0.4.1
+Summary: AccuRating is a library for accurate player ranking based on match results.
+Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: pytest (>=6.2.5,<7.0.0)
+Project-URL: Documentation, https://lukaszlew.github.io/accurating/
 Description-Content-Type: text/markdown
 
 # AccuRating
 
 Library computing accurate ratings based on match results.
 
 ## Usage
```

