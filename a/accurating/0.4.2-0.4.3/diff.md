# Comparing `tmp/accurating-0.4.2.tar.gz` & `tmp/accurating-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.2.tar", max compression
+gzip compressed data, was "accurating-0.4.3.tar", max compression
```

## Comparing `accurating-0.4.2.tar` & `accurating-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.2/LICENSE
--rw-r--r--   0        0        0     5964 2023-04-16 21:30:01.981248 accurating-0.4.2/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.2/accurating/__init__.py
--rw-r--r--   0        0        0     8407 2023-04-17 05:13:50.431970 accurating-0.4.2/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.2/accurating/tests/__init__.py
--rw-r--r--   0        0        0     2471 2023-04-17 05:14:30.265058 accurating-0.4.2/accurating/tests/model_test.py
--rw-r--r--   0        0        0      632 2023-04-17 05:15:29.458691 accurating-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6611 1970-01-01 00:00:00.000000 accurating-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.3/LICENSE
+-rw-r--r--   0        0        0     5964 2023-04-16 21:30:01.981248 accurating-0.4.3/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.3/accurating/__init__.py
+-rw-r--r--   0        0        0     8407 2023-04-17 05:13:50.431970 accurating-0.4.3/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.3/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     2471 2023-04-17 05:14:30.265058 accurating-0.4.3/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      632 2023-04-17 05:29:08.737759 accurating-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6572 1970-01-01 00:00:00.000000 accurating-0.4.3/PKG-INFO
```

### Comparing `accurating-0.4.2/LICENSE` & `accurating-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.2/README.md` & `accurating-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `accurating-0.4.2/accurating/model.py` & `accurating-0.4.3/accurating/model.py`

 * *Files identical despite different names*

### Comparing `accurating-0.4.2/accurating/tests/model_test.py` & `accurating-0.4.3/accurating/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `accurating-0.4.2/pyproject.toml` & `accurating-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.4.2"
+version = "0.4.3"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jax = "^0.4.8"
-pytest = "^6.2.5"
 jaxlib = "^0.4.7"
 
 [tool.poetry.group.dev.dependencies]
 pdoc = "^13.1.0"
+pytest = "^6.2.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
```

### Comparing `accurating-0.4.2/PKG-INFO` & `accurating-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.2
+Version: 0.4.3
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
-Requires-Dist: pytest (>=6.2.5,<7.0.0)
 Project-URL: Documentation, https://lukaszlew.github.io/accurating/
 Description-Content-Type: text/markdown
 
 # AccuRating
 
 Library computing accurate ratings based on match results.
```

