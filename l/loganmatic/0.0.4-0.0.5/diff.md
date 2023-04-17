# Comparing `tmp/loganmatic-0.0.4.tar.gz` & `tmp/loganmatic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loganmatic-0.0.4.tar", last modified: Mon Apr 17 02:14:51 2023, max compression
+gzip compressed data, was "loganmatic-0.0.5.tar", last modified: Mon Apr 17 02:28:00 2023, max compression
```

## Comparing `loganmatic-0.0.4.tar` & `loganmatic-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.912364 loganmatic-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-17 02:13:26.000000 loganmatic-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      923 2023-04-17 02:14:51.910367 loganmatic-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-04-17 02:13:06.000000 loganmatic-0.0.4/README.md
--rw-rw-rw-   0        0        0      648 2023-04-17 02:12:16.000000 loganmatic-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 02:14:51.914388 loganmatic-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.880193 loganmatic-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.887376 loganmatic-0.0.4/src/loganmatic/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:04:58.000000 loganmatic-0.0.4/src/loganmatic/__init__.py
--rw-rw-rw-   0        0        0      968 2023-04-17 02:06:13.000000 loganmatic-0.0.4/src/loganmatic/loganmatic.py
-drwxrwxrwx   0        0        0        0 2023-04-17 02:14:51.907463 loganmatic-0.0.4/src/loganmatic.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 02:14:51.000000 loganmatic-0.0.4/src/loganmatic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 02:28:00.624690 loganmatic-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 02:13:26.000000 loganmatic-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:28:00.623803 loganmatic-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-04-17 02:13:06.000000 loganmatic-0.0.5/README.md
+-rw-rw-rw-   0        0        0      648 2023-04-17 02:27:34.000000 loganmatic-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 02:28:00.624932 loganmatic-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 02:28:00.595001 loganmatic-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 02:28:00.602028 loganmatic-0.0.5/src/loganmatic/
+-rw-rw-rw-   0        0        0       17 2023-04-17 02:25:49.000000 loganmatic-0.0.5/src/loganmatic/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-17 02:06:13.000000 loganmatic-0.0.5/src/loganmatic/loganmatic.py
+drwxrwxrwx   0        0        0        0 2023-04-17 02:28:00.621807 loganmatic-0.0.5/src/loganmatic.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-17 02:28:00.000000 loganmatic-0.0.5/src/loganmatic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-17 02:28:00.000000 loganmatic-0.0.5/src/loganmatic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 02:28:00.000000 loganmatic-0.0.5/src/loganmatic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-17 02:28:00.000000 loganmatic-0.0.5/src/loganmatic.egg-info/top_level.txt
```

### Comparing `loganmatic-0.0.4/LICENSE` & `loganmatic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `loganmatic-0.0.4/PKG-INFO` & `loganmatic-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loganmatic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Biblioteca de matematica com algumas funções para facilitar calculos
 Author-email: Gabriel Logan <author@example.com>
 Project-URL: Homepage, https://github.com/gabriel-logan/Math_Lib_Js
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `loganmatic-0.0.4/pyproject.toml` & `loganmatic-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loganmatic"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Gabriel Logan", email="author@example.com" },
 ]
 description = "Biblioteca de matematica com algumas funções para facilitar calculos"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loganmatic-0.0.4/src/loganmatic/loganmatic.py` & `loganmatic-0.0.5/src/loganmatic/loganmatic.py`

 * *Files identical despite different names*

### Comparing `loganmatic-0.0.4/src/loganmatic.egg-info/PKG-INFO` & `loganmatic-0.0.5/src/loganmatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loganmatic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Biblioteca de matematica com algumas funções para facilitar calculos
 Author-email: Gabriel Logan <author@example.com>
 Project-URL: Homepage, https://github.com/gabriel-logan/Math_Lib_Js
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

