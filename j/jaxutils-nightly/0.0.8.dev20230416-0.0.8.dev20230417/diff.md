# Comparing `tmp/jaxutils-nightly-0.0.8.dev20230416.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20230417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230416.tar", last modified: Sun Apr 16 00:06:36 2023, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20230417.tar", last modified: Mon Apr 17 00:06:44 2023, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20230416.tar` & `jaxutils-nightly-0.0.8.dev20230417.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-16 00:06:36.071148 jaxutils-nightly-0.0.8.dev20230416/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-16 00:06:36.071148 jaxutils-nightly-0.0.8.dev20230416/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2894 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-16 00:06:36.071148 jaxutils-nightly-0.0.8.dev20230416/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-04-16 00:06:36.071148 jaxutils-nightly-0.0.8.dev20230416/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-16 00:06:36.067149 jaxutils-nightly-0.0.8.dev20230416/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-16 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-04-16 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-16 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-04-16 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-16 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230416/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-04-16 00:06:36.071148 jaxutils-nightly-0.0.8.dev20230416/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-04-16 00:06:29.000000 jaxutils-nightly-0.0.8.dev20230416/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 00:06:44.324731 jaxutils-nightly-0.0.8.dev20230417/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-17 00:06:44.324731 jaxutils-nightly-0.0.8.dev20230417/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2894 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 00:06:44.324731 jaxutils-nightly-0.0.8.dev20230417/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2023-04-17 00:06:44.324731 jaxutils-nightly-0.0.8.dev20230417/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-17 00:06:44.324731 jaxutils-nightly-0.0.8.dev20230417/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4448 2023-04-17 00:06:44.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2023-04-17 00:06:44.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-17 00:06:44.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-04-17 00:06:44.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2023-04-17 00:06:44.000000 jaxutils-nightly-0.0.8.dev20230417/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2023-04-17 00:06:44.324731 jaxutils-nightly-0.0.8.dev20230417/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2023-04-17 00:06:36.000000 jaxutils-nightly-0.0.8.dev20230417/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20230416/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230416
+Version: 0.0.8.dev20230417
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230416/README.md` & `jaxutils-nightly-0.0.8.dev20230417/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20230417/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20230417/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20230417/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20230417/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20230417/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20230417/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20230417/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20230416
+Version: 0.0.8.dev20230417
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20230416/setup.py` & `jaxutils-nightly-0.0.8.dev20230417/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20230416/versioneer.py` & `jaxutils-nightly-0.0.8.dev20230417/versioneer.py`

 * *Files identical despite different names*

