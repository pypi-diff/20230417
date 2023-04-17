# Comparing `tmp/export_ease-0.0.4.tar.gz` & `tmp/export_ease-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ease-0.0.4.tar", last modified: Sun Apr 16 23:11:49 2023, max compression
+gzip compressed data, was "export_ease-0.0.5.tar", last modified: Mon Apr 17 01:35:35 2023, max compression
```

## Comparing `export_ease-0.0.4.tar` & `export_ease-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.647182 export_ease-0.0.4/
--rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.4/LICENSE
--rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 23:11:49.647056 export_ease-0.0.4/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)     4253 2023-04-16 22:09:55.000000 export_ease-0.0.4/README.md
--rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-16 23:10:45.000000 export_ease-0.0.4/pyproject.toml
--rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-16 23:11:49.647220 export_ease-0.0.4/setup.cfg
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.645294 export_ease-0.0.4/src/
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.646323 export_ease-0.0.4/src/export_ease/
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.4/src/export_ease/__init__.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.4/src/export_ease/comtrade.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 23:10:39.000000 export_ease-0.0.4/src/export_ease/imf.py
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 23:11:49.646878 export_ease-0.0.4/src/export_ease.egg-info/
--rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/SOURCES.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/dependency_links.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-16 23:11:49.000000 export_ease-0.0.4/src/export_ease.egg-info/top_level.txt
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.846650 export_ease-0.0.5/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.5/LICENSE
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-17 01:35:35.846496 export_ease-0.0.5/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4253 2023-04-16 22:09:55.000000 export_ease-0.0.5/README.md
+-rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-17 01:35:19.000000 export_ease-0.0.5/pyproject.toml
+-rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-17 01:35:35.846692 export_ease-0.0.5/setup.cfg
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.845024 export_ease-0.0.5/src/
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.845770 export_ease-0.0.5/src/export_ease/
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.5/src/export_ease/__init__.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.5/src/export_ease/comtrade.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 23:10:39.000000 export_ease-0.0.5/src/export_ease/imf.py
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-17 01:35:35.846307 export_ease-0.0.5/src/export_ease.egg-info/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4779 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/SOURCES.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/dependency_links.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-17 01:35:35.000000 export_ease-0.0.5/src/export_ease.egg-info/top_level.txt
```

### Comparing `export_ease-0.0.4/LICENSE` & `export_ease-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.4/PKG-INFO` & `export_ease-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export_ease
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `export_ease-0.0.4/README.md` & `export_ease-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.4/pyproject.toml` & `export_ease-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "export_ease"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Paul Dilly", email="paul.dilly@duke.edu" },
 ]
 description = "A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `export_ease-0.0.4/src/export_ease/comtrade.py` & `export_ease-0.0.5/src/export_ease/comtrade.py`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.4/src/export_ease/imf.py` & `export_ease-0.0.5/src/export_ease/imf.py`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.4/src/export_ease.egg-info/PKG-INFO` & `export_ease-0.0.5/src/export_ease.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export-ease
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

