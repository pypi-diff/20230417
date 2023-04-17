# Comparing `tmp/mymlcustomtools-0.0.6.tar.gz` & `tmp/mymlcustomtools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mymlcustomtools-0.0.6.tar", last modified: Mon Apr 17 15:23:50 2023, max compression
+gzip compressed data, was "dist\mymlcustomtools-0.0.7.tar", last modified: Mon Apr 17 18:53:12 2023, max compression
```

## Comparing `mymlcustomtools-0.0.6.tar` & `mymlcustomtools-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/
--rw-rw-rw-   0        0        0      321 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 15:23:50.440769 mymlcustomtools-0.0.6/mymlcustomtools/
--rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.6/mymlcustomtools/__init__.py
--rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.6/mymlcustomtools/imports.py
--rw-rw-rw-   0        0        0     2065 2023-04-17 15:23:44.000000 mymlcustomtools-0.0.6/mymlcustomtools/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/
--rw-rw-rw-   0        0        0      321 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-04-17 15:23:50.000000 mymlcustomtools-0.0.6/mymlcustomtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:23:50.456430 mymlcustomtools-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-04-17 15:23:49.000000 mymlcustomtools-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:53:12.074916 mymlcustomtools-0.0.7/
+-rw-rw-rw-   0        0        0      321 2023-04-17 18:53:12.073918 mymlcustomtools-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2023-04-17 14:36:20.000000 mymlcustomtools-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 18:53:12.053973 mymlcustomtools-0.0.7/mymlcustomtools/
+-rw-rw-rw-   0        0        0       60 2023-04-17 14:17:11.000000 mymlcustomtools-0.0.7/mymlcustomtools/__init__.py
+-rw-rw-rw-   0        0        0     3033 2023-04-17 14:34:13.000000 mymlcustomtools-0.0.7/mymlcustomtools/imports.py
+-rw-rw-rw-   0        0        0     2108 2023-04-17 18:51:09.000000 mymlcustomtools-0.0.7/mymlcustomtools/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:53:12.071924 mymlcustomtools-0.0.7/mymlcustomtools.egg-info/
+-rw-rw-rw-   0        0        0      321 2023-04-17 18:53:11.000000 mymlcustomtools-0.0.7/mymlcustomtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-17 18:53:11.000000 mymlcustomtools-0.0.7/mymlcustomtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:53:11.000000 mymlcustomtools-0.0.7/mymlcustomtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 14:47:42.000000 mymlcustomtools-0.0.7/mymlcustomtools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-04-17 18:53:11.000000 mymlcustomtools-0.0.7/mymlcustomtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 18:53:12.074916 mymlcustomtools-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-04-17 18:53:11.000000 mymlcustomtools-0.0.7/setup.py
```

### Comparing `mymlcustomtools-0.0.6/mymlcustomtools/imports.py` & `mymlcustomtools-0.0.7/mymlcustomtools/imports.py`

 * *Files identical despite different names*

### Comparing `mymlcustomtools-0.0.6/setup.py` & `mymlcustomtools-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
 	name = "mymlcustomtools",
-	version = "0.0.6",
+	version = "0.0.7",
 	description = """
 	A package with frequently and useful functions for machine learning
 	""",
 	author = "Gustavo Exel",
 	author_email = "gustavoexelgpe@gmail.com",
 	url = "https://pypi.org/project/mymlcustomtools/",
 	packages = ["mymlcustomtools"],
```

