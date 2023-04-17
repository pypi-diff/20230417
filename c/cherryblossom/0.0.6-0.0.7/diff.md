# Comparing `tmp/cherryblossom-0.0.6.tar.gz` & `tmp/cherryblossom-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherryblossom-0.0.6.tar", last modified: Mon Apr 17 05:03:47 2023, max compression
+gzip compressed data, was "cherryblossom-0.0.7.tar", last modified: Mon Apr 17 05:06:15 2023, max compression
```

## Comparing `cherryblossom-0.0.6.tar` & `cherryblossom-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:03:47.675432 cherryblossom-0.0.6/
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:03:47.675282 cherryblossom-0.0.6/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.0.6/README.md
--rw-r--r--   0 arjun      (501) staff       (20)     1494 2023-04-17 05:03:07.000000 cherryblossom-0.0.6/pyproject.toml
--rw-r--r--   0 arjun      (501) staff       (20)       38 2023-04-17 05:03:47.675472 cherryblossom-0.0.6/setup.cfg
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:03:47.668272 cherryblossom-0.0.6/src/
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:03:47.674047 cherryblossom-0.0.6/src/cherryblossom/
--rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.0.6/src/cherryblossom/Analyzer.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.0.6/src/cherryblossom/Blossom.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.0.6/src/cherryblossom/Channels.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.0.6/src/cherryblossom/Chat.py
--rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.0.6/src/cherryblossom/DB.py
--rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.0.6/src/cherryblossom/Data.py
--rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.0.6/src/cherryblossom/Functions.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.0.6/src/cherryblossom/GPTModel.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.0.6/src/cherryblossom/Index.py
--rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.0.6/src/cherryblossom/Plots.py
--rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.0.6/src/cherryblossom/Timezone.py
--rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.0.6/src/cherryblossom/__init__.py
--rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.0.6/src/cherryblossom/get_file.py
--rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.0.6/src/cherryblossom/imports.py
--rw-r--r--   0 arjun      (501) staff       (20)      540 2023-04-17 01:03:06.000000 cherryblossom-0.0.6/src/cherryblossom/main.py
-drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:03:47.675090 cherryblossom-0.0.6/src/cherryblossom.egg-info/
--rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:03:47.000000 cherryblossom-0.0.6/src/cherryblossom.egg-info/PKG-INFO
--rw-r--r--   0 arjun      (501) staff       (20)      653 2023-04-17 05:03:47.000000 cherryblossom-0.0.6/src/cherryblossom.egg-info/SOURCES.txt
--rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 05:03:47.000000 cherryblossom-0.0.6/src/cherryblossom.egg-info/dependency_links.txt
--rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 05:03:47.000000 cherryblossom-0.0.6/src/cherryblossom.egg-info/requires.txt
--rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 05:03:47.000000 cherryblossom-0.0.6/src/cherryblossom.egg-info/top_level.txt
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:06:15.574472 cherryblossom-0.0.7/
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:06:15.574299 cherryblossom-0.0.7/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)       13 2023-04-16 05:11:44.000000 cherryblossom-0.0.7/README.md
+-rw-r--r--   0 arjun      (501) staff       (20)     1529 2023-04-17 05:05:45.000000 cherryblossom-0.0.7/pyproject.toml
+-rw-r--r--   0 arjun      (501) staff       (20)       38 2023-04-17 05:06:15.574515 cherryblossom-0.0.7/setup.cfg
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:06:15.568645 cherryblossom-0.0.7/src/
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:06:15.573108 cherryblossom-0.0.7/src/cherryblossom/
+-rw-r--r--   0 arjun      (501) staff       (20)       82 2023-04-17 01:04:25.000000 cherryblossom-0.0.7/src/cherryblossom/Analyzer.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:04:20.000000 cherryblossom-0.0.7/src/cherryblossom/Blossom.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:17.000000 cherryblossom-0.0.7/src/cherryblossom/Channels.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:04:00.000000 cherryblossom-0.0.7/src/cherryblossom/Chat.py
+-rw-r--r--   0 arjun      (501) staff       (20)       64 2023-04-17 01:03:39.000000 cherryblossom-0.0.7/src/cherryblossom/DB.py
+-rw-r--r--   0 arjun      (501) staff       (20)       76 2023-04-17 01:03:43.000000 cherryblossom-0.0.7/src/cherryblossom/Data.py
+-rw-r--r--   0 arjun      (501) staff       (20)       81 2023-04-17 01:03:33.000000 cherryblossom-0.0.7/src/cherryblossom/Functions.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:03:25.000000 cherryblossom-0.0.7/src/cherryblossom/GPTModel.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:03:20.000000 cherryblossom-0.0.7/src/cherryblossom/Index.py
+-rw-r--r--   0 arjun      (501) staff       (20)       77 2023-04-17 01:04:04.000000 cherryblossom-0.0.7/src/cherryblossom/Plots.py
+-rw-r--r--   0 arjun      (501) staff       (20)       80 2023-04-17 01:04:04.000000 cherryblossom-0.0.7/src/cherryblossom/Timezone.py
+-rw-r--r--   0 arjun      (501) staff       (20)       19 2023-04-17 01:04:31.000000 cherryblossom-0.0.7/src/cherryblossom/__init__.py
+-rw-r--r--   0 arjun      (501) staff       (20)     1213 2023-04-16 04:16:55.000000 cherryblossom-0.0.7/src/cherryblossom/get_file.py
+-rw-r--r--   0 arjun      (501) staff       (20)       79 2023-04-17 01:03:19.000000 cherryblossom-0.0.7/src/cherryblossom/imports.py
+-rw-r--r--   0 arjun      (501) staff       (20)      540 2023-04-17 01:03:06.000000 cherryblossom-0.0.7/src/cherryblossom/main.py
+drwxr-xr-x   0 arjun      (501) staff       (20)        0 2023-04-17 05:06:15.574018 cherryblossom-0.0.7/src/cherryblossom.egg-info/
+-rw-r--r--   0 arjun      (501) staff       (20)      396 2023-04-17 05:06:15.000000 cherryblossom-0.0.7/src/cherryblossom.egg-info/PKG-INFO
+-rw-r--r--   0 arjun      (501) staff       (20)      653 2023-04-17 05:06:15.000000 cherryblossom-0.0.7/src/cherryblossom.egg-info/SOURCES.txt
+-rw-r--r--   0 arjun      (501) staff       (20)        1 2023-04-17 05:06:15.000000 cherryblossom-0.0.7/src/cherryblossom.egg-info/dependency_links.txt
+-rw-r--r--   0 arjun      (501) staff       (20)      101 2023-04-17 05:06:15.000000 cherryblossom-0.0.7/src/cherryblossom.egg-info/requires.txt
+-rw-r--r--   0 arjun      (501) staff       (20)       14 2023-04-17 05:06:15.000000 cherryblossom-0.0.7/src/cherryblossom.egg-info/top_level.txt
```

### Comparing `cherryblossom-0.0.6/pyproject.toml` & `cherryblossom-0.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 # NOT have to specify this line.
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-mypkg = ["*.key", "*.py"]
+mypkg = ["src/cherryblossom/.key", "src/cherryblossom/*.py"]
 
 [project]
 name = "cherryblossom"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Arjun Naik", email="arjunsatishnaik@gmail.com" },
 ]
 description = "CherryBlossom: an API for Nosedive AI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cherryblossom-0.0.6/src/cherryblossom/get_file.py` & `cherryblossom-0.0.7/src/cherryblossom/get_file.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.6/src/cherryblossom/main.py` & `cherryblossom-0.0.7/src/cherryblossom/main.py`

 * *Files identical despite different names*

### Comparing `cherryblossom-0.0.6/src/cherryblossom.egg-info/SOURCES.txt` & `cherryblossom-0.0.7/src/cherryblossom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

