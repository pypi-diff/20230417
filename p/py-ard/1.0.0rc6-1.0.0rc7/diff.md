# Comparing `tmp/py-ard-1.0.0rc6.tar.gz` & `tmp/py-ard-1.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ard-1.0.0rc6.tar", last modified: Wed Apr  5 14:00:18 2023, max compression
+gzip compressed data, was "py-ard-1.0.0rc7.tar", last modified: Mon Apr 17 19:05:16 2023, max compression
```

## Comparing `py-ard-1.0.0rc6.tar` & `py-ard-1.0.0rc7.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:00:18.277225 py-ard-1.0.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19827 2023-04-05 14:00:18.277225 py-ard-1.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:00:18.277225 py-ard-1.0.0rc6/py_ard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19827 2023-04-05 14:00:18.000000 py-ard-1.0.0rc6/py_ard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-05 14:00:18.000000 py-ard-1.0.0rc6/py_ard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:00:18.000000 py-ard-1.0.0rc6/py_ard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 14:00:18.000000 py-ard-1.0.0rc6/py_ard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 14:00:18.000000 py-ard-1.0.0rc6/py_ard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 14:00:18.000000 py-ard-1.0.0rc6/py_ard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:00:18.277225 py-ard-1.0.0rc6/pyard/
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/CWD2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27740 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/ard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/blender.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/broad_splits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16015 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/dna_relshp.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/drbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/pyard/smart_sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 14:00:18.277225 py-ard-1.0.0rc6/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/scripts/pyard
--rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/scripts/pyard-import
--rwxr-xr-x   0 runner    (1001) docker     (123)    15408 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/scripts/pyard-reduce-csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/scripts/pyard-status
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-05 14:00:18.281225 py-ard-1.0.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-05 14:00:09.000000 py-ard-1.0.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.213231 py-ard-1.0.0rc7/py_ard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/pyard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/CWD2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27740 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/ard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/broad_splits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16015 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/dna_relshp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/drbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/smart_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard-import
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15408 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard-reduce-csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard-status
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/setup.py
```

### Comparing `py-ard-1.0.0rc6/CONTRIBUTING.rst` & `py-ard-1.0.0rc7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/COPYING` & `py-ard-1.0.0rc7/COPYING`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/LICENSE` & `py-ard-1.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/PKG-INFO` & `py-ard-1.0.0rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.0.0rc6
+Version: 1.0.0rc7
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
         
@@ -42,14 +42,16 @@
         `py-ard` works with Python 3.8 and higher.
         
         ### Install from PyPi
         
         ```shell
         pip install py-ard
         ```
+        Note: With `py-ard` version *1.0.0* and higher, the redux API has changed. If your use requires the older API, please install with `pip install py-ard==0.9.2`
+        
         
         ### Install With Homebrew
         
         On macOS, `py-ard` can be installed using Homebrew package manager.
         This is very handy for using the command line versions of the tool without having to create virtual environments.
         
         First time, you'd need to tap the `nmdp-bioinformatics` tap.
```

### Comparing `py-ard-1.0.0rc6/README.md` & `py-ard-1.0.0rc7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 `py-ard` works with Python 3.8 and higher.
 
 ### Install from PyPi
 
 ```shell
 pip install py-ard
 ```
+Note: With `py-ard` version *1.0.0* and higher, the redux API has changed. If your use requires the older API, please install with `pip install py-ard==0.9.2`
+
 
 ### Install With Homebrew
 
 On macOS, `py-ard` can be installed using Homebrew package manager.
 This is very handy for using the command line versions of the tool without having to create virtual environments.
 
 First time, you'd need to tap the `nmdp-bioinformatics` tap.
```

### Comparing `py-ard-1.0.0rc6/py_ard.egg-info/PKG-INFO` & `py-ard-1.0.0rc7/py_ard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.0.0rc6
+Version: 1.0.0rc7
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
         
@@ -42,14 +42,16 @@
         `py-ard` works with Python 3.8 and higher.
         
         ### Install from PyPi
         
         ```shell
         pip install py-ard
         ```
+        Note: With `py-ard` version *1.0.0* and higher, the redux API has changed. If your use requires the older API, please install with `pip install py-ard==0.9.2`
+        
         
         ### Install With Homebrew
         
         On macOS, `py-ard` can be installed using Homebrew package manager.
         This is very handy for using the command line versions of the tool without having to create virtual environments.
         
         First time, you'd need to tap the `nmdp-bioinformatics` tap.
```

### Comparing `py-ard-1.0.0rc6/pyard/CWD2.csv` & `py-ard-1.0.0rc7/pyard/CWD2.csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/__init__.py` & `py-ard-1.0.0rc7/pyard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from .blender import blender as dr_blender
 from .broad_splits import find_splits as find_broad_splits
 from .constants import DEFAULT_CACHE_SIZE
 from .misc import get_imgt_db_versions as db_versions
 
 __author__ = """NMDP Bioinformatics"""
-__version__ = "1.0.0rc6"
+__version__ = "1.0.0rc7"
 
 
 def init(
     imgt_version: str = "Latest",
     data_dir: str = None,
     load_mac: bool = True,
     cache_size: int = DEFAULT_CACHE_SIZE,
```

### Comparing `py-ard-1.0.0rc6/pyard/ard.py` & `py-ard-1.0.0rc7/pyard/ard.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/blender.py` & `py-ard-1.0.0rc7/pyard/blender.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/broad_splits.py` & `py-ard-1.0.0rc7/pyard/broad_splits.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/constants.py` & `py-ard-1.0.0rc7/pyard/constants.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/data_repository.py` & `py-ard-1.0.0rc7/pyard/data_repository.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/db.py` & `py-ard-1.0.0rc7/pyard/db.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/drbx.py` & `py-ard-1.0.0rc7/pyard/drbx.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/exceptions.py` & `py-ard-1.0.0rc7/pyard/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/load.py` & `py-ard-1.0.0rc7/pyard/load.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/mappings.py` & `py-ard-1.0.0rc7/pyard/mappings.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/misc.py` & `py-ard-1.0.0rc7/pyard/misc.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/pyard/smart_sort.py` & `py-ard-1.0.0rc7/pyard/smart_sort.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/scripts/pyard` & `py-ard-1.0.0rc7/scripts/pyard`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/scripts/pyard-import` & `py-ard-1.0.0rc7/scripts/pyard-import`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/scripts/pyard-reduce-csv` & `py-ard-1.0.0rc7/scripts/pyard-reduce-csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/scripts/pyard-status` & `py-ard-1.0.0rc7/scripts/pyard-status`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc6/setup.cfg` & `py-ard-1.0.0rc7/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0rc6
+current_version = 1.0.0rc7
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `py-ard-1.0.0rc6/setup.py` & `py-ard-1.0.0rc7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="py-ard",
-    version="1.0.0rc6",
+    version="1.0.0rc7",
     description="ARD reduction for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="CIBMTR",
     author_email="cibmtr-pypi@nmdp.org",
     url="https://github.com/nmdp-bioinformatics/py-ard",
     packages=[
```

