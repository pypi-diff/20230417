# Comparing `tmp/pipcryptliberyV2-1.0.0.tar.gz` & `tmp/pipcryptliberyV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptliberyV2-1.0.0.tar", last modified: Fri Apr 14 21:24:41 2023, max compression
+gzip compressed data, was "pipcryptliberyV2-1.1.0.tar", last modified: Mon Apr 17 17:17:10 2023, max compression
```

## Comparing `pipcryptliberyV2-1.0.0.tar` & `pipcryptliberyV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:24:41.364829 pipcryptliberyV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-14 21:24:41.364829 pipcryptliberyV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:24:41.364829 pipcryptliberyV2-1.0.0/pipcryptliberyV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 21:24:40.000000 pipcryptliberyV2-1.0.0/pipcryptliberyV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:24:41.364829 pipcryptliberyV2-1.0.0/pipcryptliberyV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-14 21:24:41.000000 pipcryptliberyV2-1.0.0/pipcryptliberyV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-14 21:24:41.000000 pipcryptliberyV2-1.0.0/pipcryptliberyV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 21:24:41.000000 pipcryptliberyV2-1.0.0/pipcryptliberyV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-14 21:24:41.000000 pipcryptliberyV2-1.0.0/pipcryptliberyV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 21:24:41.364829 pipcryptliberyV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      537 2023-04-14 21:24:40.000000 pipcryptliberyV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:17:10.502797 pipcryptliberyV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-17 17:17:10.502797 pipcryptliberyV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:17:10.502797 pipcryptliberyV2-1.1.0/pipcryptliberyV2/
+-rw-r--r--   0 root         (0) root         (0)    72559 2023-04-17 17:17:10.000000 pipcryptliberyV2-1.1.0/pipcryptliberyV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 17:17:10.502797 pipcryptliberyV2-1.1.0/pipcryptliberyV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-17 17:17:10.000000 pipcryptliberyV2-1.1.0/pipcryptliberyV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-17 17:17:10.000000 pipcryptliberyV2-1.1.0/pipcryptliberyV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 17:17:10.000000 pipcryptliberyV2-1.1.0/pipcryptliberyV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-17 17:17:10.000000 pipcryptliberyV2-1.1.0/pipcryptliberyV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 17:17:10.502797 pipcryptliberyV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-17 17:17:09.000000 pipcryptliberyV2-1.1.0/setup.py
```

### Comparing `pipcryptliberyV2-1.0.0/setup.py` & `pipcryptliberyV2-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '1.1.0'
+DESCRIPTION = "Crypting Package"
+LONG_DESCRIPTION = "Crypting Package"
 
 # Setting up
 setup(
     name="pipcryptliberyV2",
     version=VERSION,
     author="NHJonas",
     author_email="nick.faltermeier@gmx.de",
```

