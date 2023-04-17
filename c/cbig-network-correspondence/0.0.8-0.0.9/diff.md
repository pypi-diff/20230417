# Comparing `tmp/cbig_network_correspondence-0.0.8.tar.gz` & `tmp/cbig_network_correspondence-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbig_network_correspondence-0.0.8.tar", max compression
+gzip compressed data, was "cbig_network_correspondence-0.0.9.tar", max compression
```

## Comparing `cbig_network_correspondence-0.0.8.tar` & `cbig_network_correspondence-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3180 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/README.md
--rw-r--r--   0        0        0     2376 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      490 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/__init__.py
--rw-r--r--   0        0        0    14137 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/compute_overlap_with_atlases.py
--rw-r--r--   0        0        0     3143 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/grab_data_info.py
--rw-r--r--   0        0        0      429 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/load_example.py
--rw-r--r--   0        0        0        0 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/py.typed
--rw-r--r--   0        0        0     5430 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/visualize_overlap_lib.py
--rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3180 2023-04-17 09:43:18.799261 cbig_network_correspondence-0.0.9/README.md
+-rw-r--r--   0        0        0     2376 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/__init__.py
+-rw-r--r--   0        0        0    14137 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/compute_overlap_with_atlases.py
+-rw-r--r--   0        0        0     3143 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/grab_data_info.py
+-rw-r--r--   0        0        0      429 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/load_example.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/py.typed
+-rw-r--r--   0        0        0     5430 2023-04-17 09:43:18.803261 cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/visualize_overlap_lib.py
+-rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.9/PKG-INFO
```

### Comparing `cbig_network_correspondence-0.0.8/README.md` & `cbig_network_correspondence-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.8/pyproject.toml` & `cbig_network_correspondence-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbig_network_correspondence"
-version = "0.0.8"
+version = "0.0.9"
 description = "A toolbox for exploring network correspondence across atlases"
 authors = [
     "Ruby Kong <roo.cone@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/compute_overlap_with_atlases.py` & `cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/compute_overlap_with_atlases.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/grab_data_info.py` & `cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/grab_data_info.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/visualize_overlap_lib.py` & `cbig_network_correspondence-0.0.9/src/cbig_network_correspondence/visualize_overlap_lib.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.8/PKG-INFO` & `cbig_network_correspondence-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbig-network-correspondence
-Version: 0.0.8
+Version: 0.0.9
 Summary: A toolbox for exploring network correspondence across atlases
 Home-page: https://rubykong.github.io/cbig_network_correspondence
 License: MIT
 Author: Ruby Kong
 Author-email: roo.cone@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
```

