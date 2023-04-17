# Comparing `tmp/pygameHat-1.0.8.tar.gz` & `tmp/pygameHat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameHat-1.0.8.tar", last modified: Sun Apr 16 16:46:00 2023, max compression
+gzip compressed data, was "pygameHat-1.1.0.tar", last modified: Sun Apr 16 20:29:52 2023, max compression
```

## Comparing `pygameHat-1.0.8.tar` & `pygameHat-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:46:00.219011 pygameHat-1.0.8/
--rw-rw-rw-   0        0        0      549 2023-04-16 16:46:00.214986 pygameHat-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 16:46:00.206002 pygameHat-1.0.8/pygameHat.egg-info/
--rw-rw-rw-   0        0        0      549 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 16:46:00.219011 pygameHat-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-04-16 16:39:34.000000 pygameHat-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 20:29:52.685909 pygameHat-1.1.0/
+-rw-rw-rw-   0        0        0      548 2023-04-16 20:29:52.682948 pygameHat-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 20:29:52.674910 pygameHat-1.1.0/pygameHat.egg-info/
+-rw-rw-rw-   0        0        0      548 2023-04-16 20:29:52.000000 pygameHat-1.1.0/pygameHat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-04-16 20:29:52.000000 pygameHat-1.1.0/pygameHat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 20:29:52.000000 pygameHat-1.1.0/pygameHat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 20:29:52.000000 pygameHat-1.1.0/pygameHat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 20:29:52.000000 pygameHat-1.1.0/pygameHat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 20:29:52.685909 pygameHat-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-04-16 20:16:05.000000 pygameHat-1.1.0/setup.py
```

### Comparing `pygameHat-1.0.8/PKG-INFO` & `pygameHat-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.0.8
+Version: 1.1.0
 Summary: pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,pygame,game,engine,maker,tool
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pygameHat-1.0.8/pygameHat.egg-info/PKG-INFO` & `pygameHat-1.1.0/pygameHat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.0.8
+Version: 1.1.0
 Summary: pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,pygame,game,engine,maker,tool
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pygameHat-1.0.8/setup.py` & `pygameHat-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.8'
+VERSION = '1.1.0'
 DESCRIPTION = 'pygame game-making engine'
 
 # Setting up
 setup(
     name="pygameHat",
     version=VERSION,
     author="Wojciech Błajda",
     #author_email="<mail@neuralnine.com>",
     description=DESCRIPTION,
-    install_requires=['pygame'],
+    install_requires=['pygame', 'pyinstaller'],
     keywords=['python', 'pygame', 'game', 'engine', 'maker', 'tool'],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

