# Comparing `tmp/deetlist-1.0.tar.gz` & `tmp/deetlist-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deetlist-1.0.tar", last modified: Mon Mar  6 00:41:12 2023, max compression
+gzip compressed data, was "deetlist-1.2.tar", last modified: Mon Apr 17 15:45:16 2023, max compression
```

## Comparing `deetlist-1.0.tar` & `deetlist-1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 00:41:12.333311 deetlist-1.0/
--rw-rw-rw-   0        0        0      290 2023-03-06 00:41:12.331306 deetlist-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-03-06 00:41:03.000000 deetlist-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-06 00:41:12.329306 deetlist-1.0/deetlist.egg-info/
--rw-rw-rw-   0        0        0      290 2023-03-06 00:41:12.000000 deetlist-1.0/deetlist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-03-06 00:41:12.000000 deetlist-1.0/deetlist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 00:41:12.000000 deetlist-1.0/deetlist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      279 2023-03-06 00:41:12.000000 deetlist-1.0/deetlist.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 00:41:12.000000 deetlist-1.0/deetlist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-06 00:41:12.334309 deetlist-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-03-06 00:40:46.000000 deetlist-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:45:16.546502 deetlist-1.2/
+-rw-rw-rw-   0        0        0     1037 2023-04-17 15:45:16.543497 deetlist-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2023-04-09 17:25:37.000000 deetlist-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 15:45:16.541494 deetlist-1.2/deetlist.egg-info/
+-rw-rw-rw-   0        0        0     1037 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      279 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:45:16.000000 deetlist-1.2/deetlist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:45:16.546502 deetlist-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-04-17 15:45:15.000000 deetlist-1.2/setup.py
```

### Comparing `deetlist-1.0/setup.py` & `deetlist-1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name="deetlist",
-    version="1.0",
+    version="1.2",
     license="MIT License",
     author="Marcuth",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author_email="marcuth2006@gmail.com",
     keywords="dragoncity dcutils tools",
     description=f"Fetcher/scraper of https://deetlist.com/dragoncity/",
```

