# Comparing `tmp/loganmatic-0.0.6.tar.gz` & `tmp/loganmatic-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loganmatic-0.0.6.tar", last modified: Mon Apr 17 02:31:37 2023, max compression
+gzip compressed data, was "loganmatic-0.0.7.tar", last modified: Mon Apr 17 02:40:14 2023, max compression
```

## Comparing `loganmatic-0.0.6.tar` & `loganmatic-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:31:37.396233 loganmatic-0.0.6/
--rw-rw-rw-   0        0        0     1091 2023-04-17 02:13:26.000000 loganmatic-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      923 2023-04-17 02:31:37.395093 loganmatic-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-04-17 02:13:06.000000 loganmatic-0.0.6/README.md
--rw-rw-rw-   0        0        0      648 2023-04-17 02:30:40.000000 loganmatic-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 02:31:37.397089 loganmatic-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 02:31:37.365740 loganmatic-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 02:31:37.374140 loganmatic-0.0.6/src/loganmatic/
--rw-rw-rw-   0        0        0      968 2023-04-17 02:31:00.000000 loganmatic-0.0.6/src/loganmatic/__init__.py
--rw-rw-rw-   0        0        0      968 2023-04-17 02:06:13.000000 loganmatic-0.0.6/src/loganmatic/loganmatic.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:31:37.394098 loganmatic-0.0.6/src/loganmatic.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-17 02:31:37.000000 loganmatic-0.0.6/src/loganmatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-17 02:31:37.000000 loganmatic-0.0.6/src/loganmatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:31:37.000000 loganmatic-0.0.6/src/loganmatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 02:31:37.000000 loganmatic-0.0.6/src/loganmatic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 02:40:14.658750 loganmatic-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 02:13:26.000000 loganmatic-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:40:14.657471 loganmatic-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-17 02:13:06.000000 loganmatic-0.0.7/README.md
+-rw-rw-rw-   0        0        0      648 2023-04-17 02:39:37.000000 loganmatic-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 02:40:14.658995 loganmatic-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 02:40:14.627046 loganmatic-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 02:40:14.635856 loganmatic-0.0.7/src/loganmatic/
+-rw-rw-rw-   0        0        0        0 2023-04-17 02:39:22.000000 loganmatic-0.0.7/src/loganmatic/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-17 02:06:13.000000 loganmatic-0.0.7/src/loganmatic/loganmatic.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:40:14.654880 loganmatic-0.0.7/src/loganmatic.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:40:14.000000 loganmatic-0.0.7/src/loganmatic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-17 02:40:14.000000 loganmatic-0.0.7/src/loganmatic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 02:40:14.000000 loganmatic-0.0.7/src/loganmatic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 02:40:14.000000 loganmatic-0.0.7/src/loganmatic.egg-info/top_level.txt
```

### Comparing `loganmatic-0.0.6/LICENSE` & `loganmatic-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `loganmatic-0.0.6/PKG-INFO` & `loganmatic-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loganmatic
-Version: 0.0.6
+Version: 0.0.7
 Summary: Biblioteca de matematica com algumas funções para facilitar calculos
 Author-email: Gabriel Logan <author@example.com>
 Project-URL: Homepage, https://github.com/gabriel-logan/Math_Lib_Js
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `loganmatic-0.0.6/pyproject.toml` & `loganmatic-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loganmatic"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Gabriel Logan", email="author@example.com" },
 ]
 description = "Biblioteca de matematica com algumas funções para facilitar calculos"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loganmatic-0.0.6/src/loganmatic/__init__.py` & `loganmatic-0.0.7/src/loganmatic/loganmatic.py`

 * *Files identical despite different names*

### Comparing `loganmatic-0.0.6/src/loganmatic.egg-info/PKG-INFO` & `loganmatic-0.0.7/src/loganmatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loganmatic
-Version: 0.0.6
+Version: 0.0.7
 Summary: Biblioteca de matematica com algumas funções para facilitar calculos
 Author-email: Gabriel Logan <author@example.com>
 Project-URL: Homepage, https://github.com/gabriel-logan/Math_Lib_Js
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

