# Comparing `tmp/currentime-1.0.0.tar.gz` & `tmp/currentime-1.1.0.tar.gz`

## Comparing `currentime-1.0.0.tar` & `currentime-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 currentime-1.0.0/README copy.md
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 currentime-1.0.0/src/CurrentTime.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 currentime-1.0.0/src/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 currentime-1.0.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 currentime-1.0.0/LICENSE
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 currentime-1.0.0/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 currentime-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 currentime-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 currentime-1.1.0/src/CurrentTime.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 currentime-1.1.0/src/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 currentime-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 currentime-1.1.0/LICENSE
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 currentime-1.1.0/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 currentime-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 currentime-1.1.0/PKG-INFO
```

### Comparing `currentime-1.0.0/src/CurrentTime.py` & `currentime-1.1.0/src/CurrentTime.py`

 * *Files identical despite different names*

### Comparing `currentime-1.0.0/LICENSE` & `currentime-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `currentime-1.0.0/pyproject.toml` & `currentime-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CurrenTime"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Scott Zachariae", email="scott.zachariae@outlook.com" },
 ]
 description = "A small and simple package to get current Date and Time"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `currentime-1.0.0/PKG-INFO` & `currentime-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,30 @@
 Metadata-Version: 2.1
 Name: CurrenTime
-Version: 1.0.0
+Version: 1.1.0
 Summary: A small and simple package to get current Date and Time
 Project-URL: Homepage, https://github.com/NotScottt/CurrenTime
 Author-email: Scott Zachariae <scott.zachariae@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-Hello,
+## About
 
-this is my simple python package to display and print the current Time. I'm using the datetime module for my script.
+Very simple Python script to display the current Time. 
+Simply install it via pip with 
+
+
+## Pip
+```
+  pip install CurrenTime
+ ```
+  
+
+or
+[Link to my project on PyIp](https://pypi.org/project/CurrenTime/)
+
+## Note
+this is a very simple library, i may upgrade it later.
```

