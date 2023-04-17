# Comparing `tmp/testdontdownloadthis-1.0.1.tar.gz` & `tmp/testdontdownloadthis-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdontdownloadthis-1.0.1.tar", last modified: Mon Apr 17 14:08:49 2023, max compression
+gzip compressed data, was "testdontdownloadthis-1.0.2.tar", last modified: Mon Apr 17 14:13:30 2023, max compression
```

## Comparing `testdontdownloadthis-1.0.1.tar` & `testdontdownloadthis-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:08:49.812921 testdontdownloadthis-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-17 14:08:49.812921 testdontdownloadthis-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 14:08:49.812921 testdontdownloadthis-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-17 14:08:48.000000 testdontdownloadthis-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:08:49.812921 testdontdownloadthis-1.0.1/testdontdownloadthis/
--rw-r--r--   0 root         (0) root         (0)    69206 2023-04-17 14:08:49.000000 testdontdownloadthis-1.0.1/testdontdownloadthis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:08:49.812921 testdontdownloadthis-1.0.1/testdontdownloadthis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      308 2023-04-17 14:08:49.000000 testdontdownloadthis-1.0.1/testdontdownloadthis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-04-17 14:08:49.000000 testdontdownloadthis-1.0.1/testdontdownloadthis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:08:49.000000 testdontdownloadthis-1.0.1/testdontdownloadthis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 14:08:49.000000 testdontdownloadthis-1.0.1/testdontdownloadthis.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:13:30.965331 testdontdownloadthis-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-17 14:13:30.965331 testdontdownloadthis-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 14:13:30.965331 testdontdownloadthis-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-17 14:13:29.000000 testdontdownloadthis-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:13:30.961331 testdontdownloadthis-1.0.2/testdontdownloadthis/
+-rw-r--r--   0 root         (0) root         (0)    69206 2023-04-17 14:13:30.000000 testdontdownloadthis-1.0.2/testdontdownloadthis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:13:30.965331 testdontdownloadthis-1.0.2/testdontdownloadthis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-17 14:13:30.000000 testdontdownloadthis-1.0.2/testdontdownloadthis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-04-17 14:13:30.000000 testdontdownloadthis-1.0.2/testdontdownloadthis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:13:30.000000 testdontdownloadthis-1.0.2/testdontdownloadthis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 14:13:30.000000 testdontdownloadthis-1.0.2/testdontdownloadthis.egg-info/top_level.txt
```

### Comparing `testdontdownloadthis-1.0.1/setup.py` & `testdontdownloadthis-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = "e"
 LONG_DESCRIPTION = "e"
 
 # Setting up
 setup(
     name="testdontdownloadthis",
     version=VERSION,
```

### Comparing `testdontdownloadthis-1.0.1/testdontdownloadthis/__init__.py` & `testdontdownloadthis-1.0.2/testdontdownloadthis/__init__.py`

 * *Files identical despite different names*

