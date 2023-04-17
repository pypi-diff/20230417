# Comparing `tmp/hasher_cnml-0.0.1.tar.gz` & `tmp/hasher_cnml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hasher_cnml-0.0.1.tar", last modified: Mon Apr 17 12:10:41 2023, max compression
+gzip compressed data, was "hasher_cnml-0.0.2.tar", last modified: Mon Apr 17 13:00:11 2023, max compression
```

## Comparing `hasher_cnml-0.0.1.tar` & `hasher_cnml-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:10:41.752115 hasher_cnml-0.0.1/
--rw-rw-rw-   0        0        0     1069 2023-04-17 11:57:46.000000 hasher_cnml-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      737 2023-04-17 12:10:41.751115 hasher_cnml-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-17 12:06:41.000000 hasher_cnml-0.0.1/README.md
--rw-rw-rw-   0        0        0      602 2023-04-17 12:08:41.000000 hasher_cnml-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 12:10:41.752115 hasher_cnml-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 12:10:41.723027 hasher_cnml-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 12:10:41.732120 hasher_cnml-0.0.1/src/hasher/
--rw-rw-rw-   0        0        0        0 2023-04-17 10:24:34.000000 hasher_cnml-0.0.1/src/hasher/__init__.py
--rw-rw-rw-   0        0        0     2090 2023-04-17 11:48:41.000000 hasher_cnml-0.0.1/src/hasher/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:10:41.749558 hasher_cnml-0.0.1/src/hasher_cnml.egg-info/
--rw-rw-rw-   0        0        0      737 2023-04-17 12:10:41.000000 hasher_cnml-0.0.1/src/hasher_cnml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-17 12:10:41.000000 hasher_cnml-0.0.1/src/hasher_cnml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:10:41.000000 hasher_cnml-0.0.1/src/hasher_cnml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 12:10:41.000000 hasher_cnml-0.0.1/src/hasher_cnml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:00:11.613614 hasher_cnml-0.0.2/
+-rw-rw-rw-   0        0        0     1069 2023-04-17 11:57:46.000000 hasher_cnml-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1307 2023-04-17 13:00:11.612617 hasher_cnml-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-04-17 12:57:00.000000 hasher_cnml-0.0.2/README.md
+-rw-rw-rw-   0        0        0      602 2023-04-17 12:43:57.000000 hasher_cnml-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:00:11.613614 hasher_cnml-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 13:00:11.583824 hasher_cnml-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:00:11.594093 hasher_cnml-0.0.2/src/hasher/
+-rw-rw-rw-   0        0        0        0 2023-04-17 10:24:34.000000 hasher_cnml-0.0.2/src/hasher/__init__.py
+-rw-rw-rw-   0        0        0     2090 2023-04-17 12:40:38.000000 hasher_cnml-0.0.2/src/hasher/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:00:11.610613 hasher_cnml-0.0.2/src/hasher_cnml.egg-info/
+-rw-rw-rw-   0        0        0     1307 2023-04-17 13:00:11.000000 hasher_cnml-0.0.2/src/hasher_cnml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-17 13:00:11.000000 hasher_cnml-0.0.2/src/hasher_cnml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:00:11.000000 hasher_cnml-0.0.2/src/hasher_cnml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 13:00:11.000000 hasher_cnml-0.0.2/src/hasher_cnml.egg-info/top_level.txt
```

### Comparing `hasher_cnml-0.0.1/LICENSE` & `hasher_cnml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hasher_cnml-0.0.1/pyproject.toml` & `hasher_cnml-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hasher_cnml"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Michael Chen", email="mail@cnml.de" },
 ]
 description = "Command line interface to the hashlib library."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `hasher_cnml-0.0.1/src/hasher/__main__.py` & `hasher_cnml-0.0.2/src/hasher/__main__.py`

 * *Files identical despite different names*

