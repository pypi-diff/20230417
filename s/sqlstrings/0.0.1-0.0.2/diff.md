# Comparing `tmp/sqlstrings-0.0.1.tar.gz` & `tmp/sqlstrings-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlstrings-0.0.1.tar", last modified: Mon Apr 17 07:58:53 2023, max compression
+gzip compressed data, was "sqlstrings-0.0.2.tar", last modified: Mon Apr 17 10:03:25 2023, max compression
```

## Comparing `sqlstrings-0.0.1.tar` & `sqlstrings-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 07:58:53.764298 sqlstrings-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:54:03.000000 sqlstrings-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      719 2023-04-17 07:58:53.764298 sqlstrings-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       97 2023-03-28 08:29:53.000000 sqlstrings-0.0.1/README.md
--rw-rw-rw-   0        0        0      576 2023-04-17 07:51:40.000000 sqlstrings-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 07:58:53.764298 sqlstrings-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-04-17 07:39:59.000000 sqlstrings-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 07:58:53.753858 sqlstrings-0.0.1/sqlstrings.egg-info/
--rw-rw-rw-   0        0        0      719 2023-04-17 07:58:53.000000 sqlstrings-0.0.1/sqlstrings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-17 07:58:53.000000 sqlstrings-0.0.1/sqlstrings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 07:58:53.000000 sqlstrings-0.0.1/sqlstrings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 07:58:53.000000 sqlstrings-0.0.1/sqlstrings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 07:58:53.762300 sqlstrings-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-03-31 15:43:40.000000 sqlstrings-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.1/tests/test_csv_handling.py
--rw-rw-rw-   0        0        0      162 2023-03-31 16:28:49.000000 sqlstrings-0.0.1/tests/test_main.py
--rw-rw-rw-   0        0        0     2472 2023-04-13 13:01:08.000000 sqlstrings-0.0.1/tests/test_postgre.py
--rw-rw-rw-   0        0        0     1984 2023-04-12 16:19:18.000000 sqlstrings-0.0.1/tests/test_transact.py
--rw-rw-rw-   0        0        0     1632 2023-04-12 16:19:28.000000 sqlstrings-0.0.1/tests/test_value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:03:25.547645 sqlstrings-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:54:03.000000 sqlstrings-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      856 2023-04-17 10:03:25.545642 sqlstrings-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-17 10:00:50.000000 sqlstrings-0.0.2/README.md
+-rw-rw-rw-   0        0        0      576 2023-04-17 10:00:31.000000 sqlstrings-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:03:25.547645 sqlstrings-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-04-17 10:02:48.000000 sqlstrings-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:03:25.531682 sqlstrings-0.0.2/sqlstrings.egg-info/
+-rw-rw-rw-   0        0        0      856 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 10:03:25.544654 sqlstrings-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:43:40.000000 sqlstrings-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.2/tests/test_csv_handling.py
+-rw-rw-rw-   0        0        0      162 2023-03-31 16:28:49.000000 sqlstrings-0.0.2/tests/test_main.py
+-rw-rw-rw-   0        0        0     2472 2023-04-13 13:01:08.000000 sqlstrings-0.0.2/tests/test_postgre.py
+-rw-rw-rw-   0        0        0     1984 2023-04-12 16:19:18.000000 sqlstrings-0.0.2/tests/test_transact.py
+-rw-rw-rw-   0        0        0     1632 2023-04-12 16:19:28.000000 sqlstrings-0.0.2/tests/test_value_handling.py
```

### Comparing `sqlstrings-0.0.1/LICENSE` & `sqlstrings-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.1/pyproject.toml` & `sqlstrings-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlstrings"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ali Kellaway", email="ali.kellaway139@gmail.com" },
 ]
 description = "Package generates SQL query strings in multiple dialects."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sqlstrings-0.0.1/setup.py` & `sqlstrings-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sqlstrings',
-    version='0.1.0',
+    version='0.0.2',
     description='A Python library for generating strings in different SQL dialects.',
     url='https://github.com/alikellaway/sqlstrings',
     author='Ali Kellaway',
     author_email='ali.kellaway139@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `sqlstrings-0.0.1/tests/test_postgre.py` & `sqlstrings-0.0.2/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.1/tests/test_transact.py` & `sqlstrings-0.0.2/tests/test_transact.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.1/tests/test_value_handling.py` & `sqlstrings-0.0.2/tests/test_value_handling.py`

 * *Files identical despite different names*

