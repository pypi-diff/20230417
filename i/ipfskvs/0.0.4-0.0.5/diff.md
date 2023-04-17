# Comparing `tmp/ipfskvs-0.0.4.tar.gz` & `tmp/ipfskvs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.0.4.tar", last modified: Mon Apr 17 15:43:23 2023, max compression
+gzip compressed data, was "ipfskvs-0.0.5.tar", last modified: Mon Apr 17 16:10:30 2023, max compression
```

## Comparing `ipfskvs-0.0.4.tar` & `ipfskvs-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 15:43:23.898825 ipfskvs-0.0.4/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.4/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     3281 2023-04-17 15:43:23.898708 ipfskvs-0.0.4/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1391 2023-04-17 15:40:23.000000 ipfskvs-0.0.4/README.md
--rw-r--r--   0 nate       (501) staff       (20)      634 2023-04-17 15:42:55.000000 ipfskvs-0.0.4/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 15:43:23.898854 ipfskvs-0.0.4/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      817 2023-04-17 15:42:48.000000 ipfskvs-0.0.4/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 15:43:23.897632 ipfskvs-0.0.4/src/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 15:43:23.898574 ipfskvs-0.0.4/src/ipfskvs.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     3281 2023-04-17 15:43:23.000000 ipfskvs-0.0.4/src/ipfskvs.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      215 2023-04-17 15:43:23.000000 ipfskvs-0.0.4/src/ipfskvs.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 15:43:23.000000 ipfskvs-0.0.4/src/ipfskvs.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 15:43:23.000000 ipfskvs-0.0.4/src/ipfskvs.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 15:43:23.000000 ipfskvs-0.0.4/src/ipfskvs.egg-info/top_level.txt
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:10:30.417597 ipfskvs-0.0.5/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.5/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 16:10:30.417480 ipfskvs-0.0.5/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     1392 2023-04-17 15:48:04.000000 ipfskvs-0.0.5/README.md
+-rw-r--r--   0 nate       (501) staff       (20)      634 2023-04-17 15:48:20.000000 ipfskvs-0.0.5/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 16:10:30.417627 ipfskvs-0.0.5/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      871 2023-04-17 16:09:46.000000 ipfskvs-0.0.5/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:10:30.416284 ipfskvs-0.0.5/src/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:10:30.417337 ipfskvs-0.0.5/src/ipfskvs.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      215 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/top_level.txt
```

### Comparing `ipfskvs-0.0.4/LICENSE` & `ipfskvs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.0.4/PKG-INFO` & `ipfskvs-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.4
+Version: 0.0.5
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
@@ -35,15 +35,15 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipfs (interplanetary filesystem) kvs (key value store)
 
-Documentation: https://ipfskvs.readthedocs.io/
+Documentation: https://ipfs-kvs.readthedocs.io/
 
 ## Build docs
 `mkdocs serve`
 
 ## Run tests
 To only run tests: `pytest`  
 To run all checks: `nox`
```

### Comparing `ipfskvs-0.0.4/README.md` & `ipfskvs-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ipfs (interplanetary filesystem) kvs (key value store)
 
-Documentation: https://ipfskvs.readthedocs.io/
+Documentation: https://ipfs-kvs.readthedocs.io/
 
 ## Build docs
 `mkdocs serve`
 
 ## Run tests
 To only run tests: `pytest`  
 To run all checks: `nox`
```

### Comparing `ipfskvs-0.0.4/pyproject.toml` & `ipfskvs-0.0.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 source = ["src", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "ipfskvs"
-version = "0.0.4"
+version = "0.0.5"
 description = "IPFS python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/ipfskvs/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
```

### Comparing `ipfskvs-0.0.4/setup.py` & `ipfskvs-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from setuptools import setup, find_packages
+"""Setup."""
+from setuptools import find_packages, setup
 
 
 def load_long_description(filename: str) -> str:
+    """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="ipfskvs",
-    version="0.0.4",
+    version="0.0.5",
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="IPFS Key Value Store",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/ipfskvs",
     project_urls={
```

### Comparing `ipfskvs-0.0.4/src/ipfskvs.egg-info/PKG-INFO` & `ipfskvs-0.0.5/src/ipfskvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.4
+Version: 0.0.5
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
@@ -35,15 +35,15 @@
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipfs (interplanetary filesystem) kvs (key value store)
 
-Documentation: https://ipfskvs.readthedocs.io/
+Documentation: https://ipfs-kvs.readthedocs.io/
 
 ## Build docs
 `mkdocs serve`
 
 ## Run tests
 To only run tests: `pytest`  
 To run all checks: `nox`
```

