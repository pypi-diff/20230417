# Comparing `tmp/LibCode-1.1.0.tar.gz` & `tmp/LibCode-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibCode-1.1.0.tar", last modified: Tue Apr 11 20:59:20 2023, max compression
+gzip compressed data, was "LibCode-1.2.0.tar", last modified: Mon Apr 17 05:28:05 2023, max compression
```

## Comparing `LibCode-1.1.0.tar` & `LibCode-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-11 20:59:20.835778 LibCode-1.1.0/
--rw-r--r--   0 axelsanchez   (501) staff       (20)     1070 2023-04-04 05:26:09.000000 LibCode-1.1.0/LICENSE
-drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-11 20:59:20.835041 LibCode-1.1.0/LibCode.egg-info/
--rw-r--r--   0 axelsanchez   (501) staff       (20)     1245 2023-04-11 20:59:20.000000 LibCode-1.1.0/LibCode.egg-info/PKG-INFO
--rw-r--r--   0 axelsanchez   (501) staff       (20)      198 2023-04-11 20:59:20.000000 LibCode-1.1.0/LibCode.egg-info/SOURCES.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)        1 2023-04-11 20:59:20.000000 LibCode-1.1.0/LibCode.egg-info/dependency_links.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)        7 2023-04-11 20:59:20.000000 LibCode-1.1.0/LibCode.egg-info/requires.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)        6 2023-04-11 20:59:20.000000 LibCode-1.1.0/LibCode.egg-info/top_level.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)     1245 2023-04-11 20:59:20.835627 LibCode-1.1.0/PKG-INFO
--rw-r--r--   0 axelsanchez   (501) staff       (20)      782 2023-04-11 03:39:01.000000 LibCode-1.1.0/README.md
-drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-11 20:59:20.835164 LibCode-1.1.0/myLib/
--rw-r--r--   0 axelsanchez   (501) staff       (20)      241 2023-04-11 03:18:19.000000 LibCode-1.1.0/myLib/__init__.py
--rw-r--r--   0 axelsanchez   (501) staff       (20)       38 2023-04-11 20:59:20.835828 LibCode-1.1.0/setup.cfg
--rw-r--r--   0 axelsanchez   (501) staff       (20)      718 2023-04-11 20:59:14.000000 LibCode-1.1.0/setup.py
+drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:28:05.141228 LibCode-1.2.0/
+-rw-r--r--   0 axelsanchez   (501) staff       (20)     1070 2023-04-04 05:26:09.000000 LibCode-1.2.0/LICENSE
+drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:28:05.140390 LibCode-1.2.0/LibCode.egg-info/
+-rw-r--r--   0 axelsanchez   (501) staff       (20)    23223 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/PKG-INFO
+-rw-r--r--   0 axelsanchez   (501) staff       (20)      198 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/SOURCES.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)        1 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/dependency_links.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)        7 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/requires.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)        6 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/top_level.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)    23223 2023-04-17 05:28:05.141062 LibCode-1.2.0/PKG-INFO
+-rw-r--r--   0 axelsanchez   (501) staff       (20)    22760 2023-04-17 05:24:23.000000 LibCode-1.2.0/README.md
+drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:28:05.140539 LibCode-1.2.0/myLib/
+-rw-r--r--   0 axelsanchez   (501) staff       (20)      241 2023-04-11 03:18:19.000000 LibCode-1.2.0/myLib/__init__.py
+-rw-r--r--   0 axelsanchez   (501) staff       (20)       38 2023-04-17 05:28:05.141291 LibCode-1.2.0/setup.cfg
+-rw-r--r--   0 axelsanchez   (501) staff       (20)      718 2023-04-17 05:27:03.000000 LibCode-1.2.0/setup.py
```

### Comparing `LibCode-1.1.0/LICENSE` & `LibCode-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LibCode-1.1.0/setup.py` & `LibCode-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="LibCode",
-    version="1.1.0",
+    version="1.2.0",
     description="A data structures and algorithms library implemented with Python and tested with Pytest!",
     author="Axel Sanchez and  Mariia Podgaietska",
     packages=[
         "myLib",
     ],
     install_requires=[
         "pytest",
```

