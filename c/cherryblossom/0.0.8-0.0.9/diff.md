# Comparing `tmp/cherryblossom-0.0.8.tar.gz` & `tmp/cherryblossom-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherryblossom-0.0.8.tar", last modified: Mon Apr 17 05:16:07 2023, max compression
+gzip compressed data, was "cherryblossom-0.0.9.tar", last modified: Mon Apr 17 05:41:50 2023, max compression
```

## Comparing `cherryblossom-0.0.8.tar` & `cherryblossom-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:16:07.037879 cherryblossom-0.0.8/
--rw-r--r--   0 arjun      (501) staff       (20)       30 2023-04-17 05:13:05.000000 cherryblossom-0.0.8/MANIFEST.in
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:16:07.037719 cherryblossom-0.0.8/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.0.8/README.md
--rw-r--r--   0 arjun      (501) staff       (20)     1529 2023-04-17 05:14:59.000000 cherryblossom-0.0.8/pyproject.toml
--rw-r--r--   0 arjun      (501) staff       (20)       38 2023-04-17 05:16:07.037918 cherryblossom-0.0.8/setup.cfg
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:16:07.029959 cherryblossom-0.0.8/src/
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:16:07.036598 cherryblossom-0.0.8/src/cherryblossom/
--rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.0.8/src/cherryblossom/.key
--rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.0.8/src/cherryblossom/Analyzer.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.0.8/src/cherryblossom/Blossom.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.0.8/src/cherryblossom/Channels.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.0.8/src/cherryblossom/Chat.py
--rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.0.8/src/cherryblossom/DB.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.0.8/src/cherryblossom/Data.py
--rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.0.8/src/cherryblossom/Functions.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.0.8/src/cherryblossom/GPTModel.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.0.8/src/cherryblossom/Index.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.0.8/src/cherryblossom/Plots.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.0.8/src/cherryblossom/Timezone.py
--rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.0.8/src/cherryblossom/__init__.py
--rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.0.8/src/cherryblossom/get_file.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.0.8/src/cherryblossom/imports.py
--rw-r--r--   0 arjun      (501) staff       (20)      540 2023-04-17 01:03:06.000000 cherryblossom-0.0.8/src/cherryblossom/main.py
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:16:07.037525 cherryblossom-0.0.8/src/cherryblossom.egg-info/
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:16:07.000000 cherryblossom-0.0.8/src/cherryblossom.egg-info/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)      688 2023-04-17 05:16:07.000000 cherryblossom-0.0.8/src/cherryblossom.egg-info/SOURCES.txt
--rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 05:16:07.000000 cherryblossom-0.0.8/src/cherryblossom.egg-info/dependency_links.txt
--rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 05:16:07.000000 cherryblossom-0.0.8/src/cherryblossom.egg-info/requires.txt
--rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 05:16:07.000000 cherryblossom-0.0.8/src/cherryblossom.egg-info/top_level.txt
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.044320 cherryblossom-0.0.9/
+-rw-r--r--   0 arjun      (501) staff       (20)       32 2023-04-17 05:21:05.000000 cherryblossom-0.0.9/MANIFEST.in
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:41:50.044164 cherryblossom-0.0.9/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.0.9/README.md
+-rw-r--r--   0 arjun      (501) staff       (20)     1538 2023-04-17 05:41:29.000000 cherryblossom-0.0.9/pyproject.toml
+-rw-r--r--   0 arjun      (501) staff       (20)       38 2023-04-17 05:41:50.044362 cherryblossom-0.0.9/setup.cfg
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.036424 cherryblossom-0.0.9/src/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.042896 cherryblossom-0.0.9/src/cherryblossom/
+-rw-r--r--   0 arjun      (501) staff       (20)     4601 2023-04-16 02:36:30.000000 cherryblossom-0.0.9/src/cherryblossom/.key
+-rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.0.9/src/cherryblossom/Analyzer.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.0.9/src/cherryblossom/Blossom.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.0.9/src/cherryblossom/Channels.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.0.9/src/cherryblossom/Chat.py
+-rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.0.9/src/cherryblossom/DB.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.0.9/src/cherryblossom/Data.py
+-rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.0.9/src/cherryblossom/Functions.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.0.9/src/cherryblossom/GPTModel.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.0.9/src/cherryblossom/Index.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.0.9/src/cherryblossom/Plots.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.0.9/src/cherryblossom/Timezone.py
+-rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.0.9/src/cherryblossom/__init__.py
+-rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.0.9/src/cherryblossom/get_file.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.0.9/src/cherryblossom/imports.py
+-rw-r--r--   0 arjun      (501) staff       (20)      540 2023-04-17 01:03:06.000000 cherryblossom-0.0.9/src/cherryblossom/main.py
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:41:50.043936 cherryblossom-0.0.9/src/cherryblossom.egg-info/
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)      690 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/SOURCES.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/dependency_links.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/requires.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 05:41:50.000000 cherryblossom-0.0.9/src/cherryblossom.egg-info/top_level.txt
```

### Comparing `cherryblossom-0.0.8/pyproject.toml` & `cherryblossom-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -31,23 +31,24 @@
 
 [tool.setuptools]
 # ...
 # By default, include-package-data is true in pyproject.toml, so you do
 # NOT have to specify this line.
 include-package-data = true
 
+
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-mypkg = ["src/cherryblossom/.key", "src/cherryblossom/*.py"]
+cherryblossom = ["src/cherryblossom/.key", "src/cherryblossom/*.py"]
 
 [project]
 name = "cherryblossom"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Arjun Naik", email="arjunsatishnaik@gmail.com" },
 ]
 description = "CherryBlossom: an API for Nosedive AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cherryblossom-0.0.8/src/cherryblossom/.key` & `cherryblossom-0.0.9/src/cherryblossom/.key`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.8/src/cherryblossom/get_file.py` & `cherryblossom-0.0.9/src/cherryblossom/get_file.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.8/src/cherryblossom/main.py` & `cherryblossom-0.0.9/src/cherryblossom/main.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.8/src/cherryblossom.egg-info/SOURCES.txt` & `cherryblossom-0.0.9/src/cherryblossom.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 README.md
 pyproject.toml
-src/cherryblossom/.key
+./src/cherryblossom/.key
 src/cherryblossom/Analyzer.py
 src/cherryblossom/Blossom.py
 src/cherryblossom/Channels.py
 src/cherryblossom/Chat.py
 src/cherryblossom/DB.py
 src/cherryblossom/Data.py
 src/cherryblossom/Functions.py
```

