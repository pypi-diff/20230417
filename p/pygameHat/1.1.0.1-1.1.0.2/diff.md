# Comparing `tmp/pygameHat-1.1.0.1.tar.gz` & `tmp/pygameHat-1.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameHat-1.1.0.1.tar", last modified: Mon Apr 17 15:03:20 2023, max compression
+gzip compressed data, was "pygameHat-1.1.0.2.tar", last modified: Mon Apr 17 15:21:39 2023, max compression
```

## Comparing `pygameHat-1.1.0.1.tar` & `pygameHat-1.1.0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:03:20.515081 pygameHat-1.1.0.1/
--rw-rw-rw-   0        0        0      550 2023-04-17 15:03:20.512071 pygameHat-1.1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 15:03:20.504032 pygameHat-1.1.0.1/pygameHat.egg-info/
--rw-rw-rw-   0        0        0      550 2023-04-17 15:03:19.000000 pygameHat-1.1.0.1/pygameHat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-04-17 15:03:19.000000 pygameHat-1.1.0.1/pygameHat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:03:19.000000 pygameHat-1.1.0.1/pygameHat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-17 15:03:19.000000 pygameHat-1.1.0.1/pygameHat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:03:19.000000 pygameHat-1.1.0.1/pygameHat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:03:20.516089 pygameHat-1.1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      735 2023-04-17 15:02:03.000000 pygameHat-1.1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:21:39.081035 pygameHat-1.1.0.2/
+-rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      545 2023-04-17 15:21:39.081035 pygameHat-1.1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 15:21:38.991025 pygameHat-1.1.0.2/pygameHat/
+-rw-rw-rw-   0        0        0    41091 2023-04-17 15:21:05.000000 pygameHat-1.1.0.2/pygameHat/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.0.2/pygameHat/pygameHat.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:21:39.072017 pygameHat-1.1.0.2/pygameHat.egg-info/
+-rw-rw-rw-   0        0        0      545 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:21:39.087015 pygameHat-1.1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-17 15:20:14.000000 pygameHat-1.1.0.2/setup.py
```

### Comparing `pygameHat-1.1.0.1/PKG-INFO` & `pygameHat-1.1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.0.1
-Summary: pygame game-making engine
+Version: 1.1.0.2
+Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
-Keywords: python,pygame,game,engine,maker,tool
+Keywords: python,engine,pygame,game,maker
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pygameHat-1.1.0.1/pygameHat.egg-info/PKG-INFO` & `pygameHat-1.1.0.2/pygameHat.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.0.1
-Summary: pygame game-making engine
+Version: 1.1.0.2
+Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
-Keywords: python,pygame,game,engine,maker,tool
+Keywords: python,engine,pygame,game,maker
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

