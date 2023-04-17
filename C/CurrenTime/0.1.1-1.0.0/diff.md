# Comparing `tmp/currentime-0.1.1.tar.gz` & `tmp/currentime-1.0.0.tar.gz`

## Comparing `currentime-0.1.1.tar` & `currentime-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 currentime-0.1.1/CurrenTime/CurrentTime.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 currentime-0.1.1/CurrenTime/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 currentime-0.1.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 currentime-0.1.1/LICENSE
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 currentime-0.1.1/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 currentime-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 currentime-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 currentime-1.0.0/README copy.md
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 currentime-1.0.0/src/CurrentTime.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 currentime-1.0.0/src/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 currentime-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 currentime-1.0.0/LICENSE
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 currentime-1.0.0/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 currentime-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 currentime-1.0.0/PKG-INFO
```

### Comparing `currentime-0.1.1/CurrenTime/CurrentTime.py` & `currentime-1.0.0/src/CurrentTime.py`

 * *Files identical despite different names*

### Comparing `currentime-0.1.1/LICENSE` & `currentime-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `currentime-0.1.1/pyproject.toml` & `currentime-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CurrenTime"
-version = "0.1.1"
+version = "1.0.0"
 authors = [
   { name="Scott Zachariae", email="scott.zachariae@outlook.com" },
 ]
 description = "A small and simple package to get current Date and Time"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `currentime-0.1.1/PKG-INFO` & `currentime-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CurrenTime
-Version: 0.1.1
+Version: 1.0.0
 Summary: A small and simple package to get current Date and Time
 Project-URL: Homepage, https://github.com/NotScottt/CurrenTime
 Author-email: Scott Zachariae <scott.zachariae@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

