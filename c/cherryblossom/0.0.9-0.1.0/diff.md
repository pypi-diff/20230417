# Comparing `tmp/cherryblossom-0.0.9.tar.gz` & `tmp/cherryblossom-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherryblossom-0.0.9.tar", last modified: Mon Apr 17 05:41:50 2023, max compression
+gzip compressed data, was "cherryblossom-0.1.0.tar", last modified: Mon Apr 17 20:05:12 2023, max compression
```

## Comparing `cherryblossom-0.0.9.tar` & `cherryblossom-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.044320 cherryblossom-0.0.9/
--rw-r--r--   0 arjun      (501) staff       (20)       32 2023-04-17 05:21:05.000000 cherryblossom-0.0.9/MANIFEST.in
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:41:50.044164 cherryblossom-0.0.9/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.0.9/README.md
--rw-r--r--   0 arjun      (501) staff       (20)     1538 2023-04-17 05:41:29.000000 cherryblossom-0.0.9/pyproject.toml
--rw-r--r--   0 arjun      (501) staff       (20)       38 2023-04-17 05:41:50.044362 cherryblossom-0.0.9/setup.cfg
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.036424 cherryblossom-0.0.9/src/
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.042896 cherryblossom-0.0.9/src/cherryblossom/
--rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.0.9/src/cherryblossom/.key
--rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.0.9/src/cherryblossom/Analyzer.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.0.9/src/cherryblossom/Blossom.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.0.9/src/cherryblossom/Channels.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.0.9/src/cherryblossom/Chat.py
--rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.0.9/src/cherryblossom/DB.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.0.9/src/cherryblossom/Data.py
--rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.0.9/src/cherryblossom/Functions.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.0.9/src/cherryblossom/GPTModel.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.0.9/src/cherryblossom/Index.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.0.9/src/cherryblossom/Plots.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.0.9/src/cherryblossom/Timezone.py
--rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.0.9/src/cherryblossom/__init__.py
--rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.0.9/src/cherryblossom/get_file.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.0.9/src/cherryblossom/imports.py
--rw-r--r--   0 arjun      (501) staff       (20)      540 2023-04-17 01:03:06.000000 cherryblossom-0.0.9/src/cherryblossom/main.py
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.043936 cherryblossom-0.0.9/src/cherryblossom.egg-info/
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)      690 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/SOURCES.txt
--rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/dependency_links.txt
--rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/requires.txt
--rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/top_level.txt
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 20:05:12.800040 cherryblossom-0.1.0/
+-rw-r--r--   0 arjun      (501) staff       (20)       32 2023-04-17 05:21:05.000000 cherryblossom-0.1.0/MANIFEST.in
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 20:05:12.799895 cherryblossom-0.1.0/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.1.0/README.md
+-rw-r--r--   0 arjun      (501) staff       (20)     1520 2023-04-17 20:04:08.000000 cherryblossom-0.1.0/pyproject.toml
+-rw-r--r--   0 arjun      (501) staff       (20)       38 2023-04-17 20:05:12.800080 cherryblossom-0.1.0/setup.cfg
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 20:05:12.789989 cherryblossom-0.1.0/src/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 20:05:12.798874 cherryblossom-0.1.0/src/cherryblossom/
+-rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.1.0/src/cherryblossom/.key
+-rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.1.0/src/cherryblossom/Analyzer.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.1.0/src/cherryblossom/Blossom.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.1.0/src/cherryblossom/Channels.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.1.0/src/cherryblossom/Chat.py
+-rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.1.0/src/cherryblossom/DB.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.1.0/src/cherryblossom/Data.py
+-rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.1.0/src/cherryblossom/Functions.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.1.0/src/cherryblossom/GPTModel.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.1.0/src/cherryblossom/Index.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.1.0/src/cherryblossom/Plots.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.1.0/src/cherryblossom/Timezone.py
+-rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.1.0/src/cherryblossom/__init__.py
+-rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.1.0/src/cherryblossom/get_file.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.1.0/src/cherryblossom/imports.py
+-rw-r--r--   0 arjun      (501) staff       (20)      541 2023-04-17 20:03:56.000000 cherryblossom-0.1.0/src/cherryblossom/main.py
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 20:05:12.799703 cherryblossom-0.1.0/src/cherryblossom.egg-info/
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 20:05:12.000000 cherryblossom-0.1.0/src/cherryblossom.egg-info/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)      713 2023-04-17 20:05:12.000000 cherryblossom-0.1.0/src/cherryblossom.egg-info/SOURCES.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 20:05:12.000000 cherryblossom-0.1.0/src/cherryblossom.egg-info/dependency_links.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 20:05:12.000000 cherryblossom-0.1.0/src/cherryblossom.egg-info/requires.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 20:05:12.000000 cherryblossom-0.1.0/src/cherryblossom.egg-info/top_level.txt
```

### Comparing `cherryblossom-0.0.9/pyproject.toml` & `cherryblossom-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 include-package-data = true
 
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-cherryblossom = ["src/cherryblossom/.key", "src/cherryblossom/*.py"]
+cherryblossom = [".key", "src/cherryblossom/*.py"]
 
 [project]
 name = "cherryblossom"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Arjun Naik", email="arjunsatishnaik@gmail.com" },
 ]
 description = "CherryBlossom: an API for Nosedive AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cherryblossom-0.0.9/src/cherryblossom/.key` & `cherryblossom-0.1.0/src/cherryblossom/.key`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.9/src/cherryblossom/get_file.py` & `cherryblossom-0.1.0/src/cherryblossom/get_file.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.9/src/cherryblossom/main.py` & `cherryblossom-0.1.0/src/cherryblossom/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,14 @@
     print('Loading...', end = '\r')
     print()
     from .Analyzer import Analyzer
     from .Blossom import Blossom
     from .Channels import Channels
     from .Chat import Chat
     from .Data import Data
-    from .Functions import Functions
+    #from .Functions import Functions
     from .GPTModel import GPTModel
     from .Index import Index
     from .Plots import Plots
     from .Timezone import Timezone
 else:
     print("You must agree to the Terms of Service.")
```

### Comparing `cherryblossom-0.0.9/src/cherryblossom.egg-info/SOURCES.txt` & `cherryblossom-0.1.0/src/cherryblossom.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 pyproject.toml
 ./src/cherryblossom/.key
+src/cherryblossom/.key
 src/cherryblossom/Analyzer.py
 src/cherryblossom/Blossom.py
 src/cherryblossom/Channels.py
 src/cherryblossom/Chat.py
 src/cherryblossom/DB.py
 src/cherryblossom/Data.py
 src/cherryblossom/Functions.py
```

