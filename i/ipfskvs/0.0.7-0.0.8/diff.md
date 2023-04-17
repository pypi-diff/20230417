# Comparing `tmp/ipfskvs-0.0.7.tar.gz` & `tmp/ipfskvs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.0.7.tar", last modified: Mon Apr 17 18:46:42 2023, max compression
+gzip compressed data, was "ipfskvs-0.0.8.tar", last modified: Mon Apr 17 19:17:36 2023, max compression
```

## Comparing `ipfskvs-0.0.7.tar` & `ipfskvs-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 18:46:42.357810 ipfskvs-0.0.7/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.7/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 18:46:42.357705 ipfskvs-0.0.7/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1392 2023-04-17 15:48:04.000000 ipfskvs-0.0.7/README.md
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 18:46:42.356650 ipfskvs-0.0.7/ipfskvs/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 18:46:42.357576 ipfskvs-0.0.7/ipfskvs/ipfskvs.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 18:46:42.000000 ipfskvs-0.0.7/ipfskvs/ipfskvs.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      235 2023-04-17 18:46:42.000000 ipfskvs-0.0.7/ipfskvs/ipfskvs.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 18:46:42.000000 ipfskvs-0.0.7/ipfskvs/ipfskvs.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 18:46:42.000000 ipfskvs-0.0.7/ipfskvs/ipfskvs.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 18:46:42.000000 ipfskvs-0.0.7/ipfskvs/ipfskvs.egg-info/top_level.txt
--rw-r--r--   0 nate       (501) staff       (20)      638 2023-04-17 18:43:16.000000 ipfskvs-0.0.7/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 18:46:42.357839 ipfskvs-0.0.7/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      879 2023-04-17 18:43:18.000000 ipfskvs-0.0.7/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 19:17:36.076885 ipfskvs-0.0.8/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.8/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 19:17:36.076781 ipfskvs-0.0.8/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     1392 2023-04-17 15:48:04.000000 ipfskvs-0.0.8/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 19:17:36.076650 ipfskvs-0.0.8/ipfskvs.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      195 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 19:17:36.000000 ipfskvs-0.0.8/ipfskvs.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      638 2023-04-17 19:16:25.000000 ipfskvs-0.0.8/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 19:17:36.076913 ipfskvs-0.0.8/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      886 2023-04-17 19:16:21.000000 ipfskvs-0.0.8/setup.py
```

### Comparing `ipfskvs-0.0.7/LICENSE` & `ipfskvs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.0.7/PKG-INFO` & `ipfskvs-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.7
+Version: 0.0.8
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `ipfskvs-0.0.7/README.md` & `ipfskvs-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.0.7/ipfskvs/ipfskvs.egg-info/PKG-INFO` & `ipfskvs-0.0.8/ipfskvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.7
+Version: 0.0.8
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `ipfskvs-0.0.7/pyproject.toml` & `ipfskvs-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 source = ["ipfskvs", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "ipfskvs"
-version = "0.0.7"
+version = "0.0.8"
 description = "IPFS python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/ipfskvs/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
```

### Comparing `ipfskvs-0.0.7/setup.py` & `ipfskvs-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="ipfskvs",
-    version="0.0.7",
+    version="0.0.8",
     author="Nathaniel Schultz",
     author_email="nate@nanoswap.finance",
     description="IPFS Key Value Store",
     long_description=load_long_description("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/nanoswap/ipfskvs",
     project_urls={
         "Bug Tracker": "https://github.com/nanoswap/ipfskvs/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: The Unlicense (Unlicense)"
 
     ],
-    package_dir={'': "ipfskvs"},
+    package_dir={'ipfskvs': "ipfskvs"},
     packages=find_packages("ipfskvs"),
     python_requires=">=3.11"
 )
```

