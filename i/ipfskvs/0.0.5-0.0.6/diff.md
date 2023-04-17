# Comparing `tmp/ipfskvs-0.0.5.tar.gz` & `tmp/ipfskvs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.0.5.tar", last modified: Mon Apr 17 16:10:30 2023, max compression
+gzip compressed data, was "ipfskvs-0.0.6.tar", last modified: Mon Apr 17 16:26:21 2023, max compression
```

## Comparing `ipfskvs-0.0.5.tar` & `ipfskvs-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:10:30.417597 ipfskvs-0.0.5/
--rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.5/LICENSE
--rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 16:10:30.417480 ipfskvs-0.0.5/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)     1392 2023-04-17 15:48:04.000000 ipfskvs-0.0.5/README.md
--rw-r--r--   0 nate       (501) staff       (20)      634 2023-04-17 15:48:20.000000 ipfskvs-0.0.5/pyproject.toml
--rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 16:10:30.417627 ipfskvs-0.0.5/setup.cfg
--rw-r--r--   0 nate       (501) staff       (20)      871 2023-04-17 16:09:46.000000 ipfskvs-0.0.5/setup.py
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:10:30.416284 ipfskvs-0.0.5/src/
-drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:10:30.417337 ipfskvs-0.0.5/src/ipfskvs.egg-info/
--rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/PKG-INFO
--rw-r--r--   0 nate       (501) staff       (20)      215 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/SOURCES.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/dependency_links.txt
--rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/requires.txt
--rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 16:10:30.000000 ipfskvs-0.0.5/src/ipfskvs.egg-info/top_level.txt
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:26:21.266709 ipfskvs-0.0.6/
+-rw-r--r--   0 nate       (501) staff       (20)     1211 2023-04-12 01:55:42.000000 ipfskvs-0.0.6/LICENSE
+-rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 16:26:21.266588 ipfskvs-0.0.6/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)     1392 2023-04-17 15:48:04.000000 ipfskvs-0.0.6/README.md
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:26:21.265083 ipfskvs-0.0.6/ipfskvs/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2023-04-17 16:26:21.266447 ipfskvs-0.0.6/ipfskvs/ipfskvs.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)     3282 2023-04-17 16:26:21.000000 ipfskvs-0.0.6/ipfskvs/ipfskvs.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)      235 2023-04-17 16:26:21.000000 ipfskvs-0.0.6/ipfskvs/ipfskvs.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 16:26:21.000000 ipfskvs-0.0.6/ipfskvs/ipfskvs.egg-info/dependency_links.txt
+-rw-r--r--   0 nate       (501) staff       (20)       50 2023-04-17 16:26:21.000000 ipfskvs-0.0.6/ipfskvs/ipfskvs.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2023-04-17 16:26:21.000000 ipfskvs-0.0.6/ipfskvs/ipfskvs.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)      638 2023-04-17 16:19:20.000000 ipfskvs-0.0.6/pyproject.toml
+-rw-r--r--   0 nate       (501) staff       (20)       38 2023-04-17 16:26:21.266747 ipfskvs-0.0.6/setup.cfg
+-rw-r--r--   0 nate       (501) staff       (20)      879 2023-04-17 16:23:20.000000 ipfskvs-0.0.6/setup.py
```

### Comparing `ipfskvs-0.0.5/LICENSE` & `ipfskvs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.0.5/PKG-INFO` & `ipfskvs-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.5
+Version: 0.0.6
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

### Comparing `ipfskvs-0.0.5/README.md` & `ipfskvs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.0.5/pyproject.toml` & `ipfskvs-0.0.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.coverage.paths]
-source = ["src", "*/site-packages"]
+source = ["ipfskvs", "*/site-packages"]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "ipfskvs"
-version = "0.0.5"
+version = "0.0.6"
 description = "IPFS python client"
 urls = {'Bug Tracker' = 'https://github.com/nanoswap/ipfskvs/issues'}
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: The Unlicense (Unlicense)'
 ]
 authors = [{'name' = 'Nathaniel Schultz', 'email' = 'nate@nanoswap.finance'}]
```

### Comparing `ipfskvs-0.0.5/setup.py` & `ipfskvs-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     """Convert README.md to a string."""
     with open(filename, "r", encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="ipfskvs",
-    version="0.0.5",
+    version="0.0.6",
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
-    package_dir={'': "src"},
-    packages=find_packages("src"),
+    package_dir={'': "ipfskvs"},
+    packages=find_packages("ipfskvs"),
     python_requires=">=3.11"
 )
```

### Comparing `ipfskvs-0.0.5/src/ipfskvs.egg-info/PKG-INFO` & `ipfskvs-0.0.6/ipfskvs/ipfskvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.0.5
+Version: 0.0.6
 Summary: IPFS python client
 Home-page: https://github.com/nanoswap/ipfskvs
 Author: Nathaniel Schultz
 Author-email: Nathaniel Schultz <nate@nanoswap.finance>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
```

