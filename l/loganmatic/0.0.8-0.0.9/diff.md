# Comparing `tmp/loganmatic-0.0.8.tar.gz` & `tmp/loganmatic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loganmatic-0.0.8.tar", last modified: Mon Apr 17 02:45:46 2023, max compression
+gzip compressed data, was "loganmatic-0.0.9.tar", last modified: Mon Apr 17 02:49:27 2023, max compression
```

## Comparing `loganmatic-0.0.8.tar` & `loganmatic-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:45:46.931340 loganmatic-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-04-17 02:13:26.000000 loganmatic-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      923 2023-04-17 02:45:46.929990 loganmatic-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-04-17 02:13:06.000000 loganmatic-0.0.8/README.md
--rw-rw-rw-   0        0        0      648 2023-04-17 02:44:59.000000 loganmatic-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 02:45:46.931584 loganmatic-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 02:45:46.903254 loganmatic-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 02:45:46.911238 loganmatic-0.0.8/src/loganmatic/
--rw-rw-rw-   0        0        0       17 2023-04-17 02:45:19.000000 loganmatic-0.0.8/src/loganmatic/__init__.py
--rw-rw-rw-   0        0        0      968 2023-04-17 02:06:13.000000 loganmatic-0.0.8/src/loganmatic/loganmatic.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:45:46.928518 loganmatic-0.0.8/src/loganmatic.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-17 02:45:46.000000 loganmatic-0.0.8/src/loganmatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-17 02:45:46.000000 loganmatic-0.0.8/src/loganmatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:45:46.000000 loganmatic-0.0.8/src/loganmatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 02:45:46.000000 loganmatic-0.0.8/src/loganmatic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 02:49:27.534958 loganmatic-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 02:13:26.000000 loganmatic-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:49:27.534017 loganmatic-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-17 02:13:06.000000 loganmatic-0.0.9/README.md
+-rw-rw-rw-   0        0        0      648 2023-04-17 02:48:15.000000 loganmatic-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 02:49:27.535066 loganmatic-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 02:49:27.505844 loganmatic-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 02:49:27.513882 loganmatic-0.0.9/src/loganmatic/
+-rw-rw-rw-   0        0        0      110 2023-04-17 02:48:32.000000 loganmatic-0.0.9/src/loganmatic/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-17 02:06:13.000000 loganmatic-0.0.9/src/loganmatic/loganmatic.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:49:27.532618 loganmatic-0.0.9/src/loganmatic.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:49:27.000000 loganmatic-0.0.9/src/loganmatic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-17 02:49:27.000000 loganmatic-0.0.9/src/loganmatic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 02:49:27.000000 loganmatic-0.0.9/src/loganmatic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 02:49:27.000000 loganmatic-0.0.9/src/loganmatic.egg-info/top_level.txt
```

### Comparing `loganmatic-0.0.8/LICENSE` & `loganmatic-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `loganmatic-0.0.8/PKG-INFO` & `loganmatic-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loganmatic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Biblioteca de matematica com algumas funções para facilitar calculos
 Author-email: Gabriel Logan <author@example.com>
 Project-URL: Homepage, https://github.com/gabriel-logan/Math_Lib_Js
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `loganmatic-0.0.8/pyproject.toml` & `loganmatic-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loganmatic"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Gabriel Logan", email="author@example.com" },
 ]
 description = "Biblioteca de matematica com algumas funções para facilitar calculos"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loganmatic-0.0.8/src/loganmatic/loganmatic.py` & `loganmatic-0.0.9/src/loganmatic/loganmatic.py`

 * *Files identical despite different names*

### Comparing `loganmatic-0.0.8/src/loganmatic.egg-info/PKG-INFO` & `loganmatic-0.0.9/src/loganmatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loganmatic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Biblioteca de matematica com algumas funções para facilitar calculos
 Author-email: Gabriel Logan <author@example.com>
 Project-URL: Homepage, https://github.com/gabriel-logan/Math_Lib_Js
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

