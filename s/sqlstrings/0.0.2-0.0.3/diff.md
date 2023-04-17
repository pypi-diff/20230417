# Comparing `tmp/sqlstrings-0.0.2.tar.gz` & `tmp/sqlstrings-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlstrings-0.0.2.tar", last modified: Mon Apr 17 10:03:25 2023, max compression
+gzip compressed data, was "sqlstrings-0.0.3.tar", last modified: Mon Apr 17 10:18:36 2023, max compression
```

## Comparing `sqlstrings-0.0.2.tar` & `sqlstrings-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:03:25.547645 sqlstrings-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:54:03.000000 sqlstrings-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      856 2023-04-17 10:03:25.545642 sqlstrings-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-17 10:00:50.000000 sqlstrings-0.0.2/README.md
--rw-rw-rw-   0        0        0      576 2023-04-17 10:00:31.000000 sqlstrings-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 10:03:25.547645 sqlstrings-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-04-17 10:02:48.000000 sqlstrings-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:03:25.531682 sqlstrings-0.0.2/sqlstrings.egg-info/
--rw-rw-rw-   0        0        0      856 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 10:03:25.000000 sqlstrings-0.0.2/sqlstrings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 10:03:25.544654 sqlstrings-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2023-03-31 15:43:40.000000 sqlstrings-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.2/tests/test_csv_handling.py
--rw-rw-rw-   0        0        0      162 2023-03-31 16:28:49.000000 sqlstrings-0.0.2/tests/test_main.py
--rw-rw-rw-   0        0        0     2472 2023-04-13 13:01:08.000000 sqlstrings-0.0.2/tests/test_postgre.py
--rw-rw-rw-   0        0        0     1984 2023-04-12 16:19:18.000000 sqlstrings-0.0.2/tests/test_transact.py
--rw-rw-rw-   0        0        0     1632 2023-04-12 16:19:28.000000 sqlstrings-0.0.2/tests/test_value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:18:36.675582 sqlstrings-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:54:03.000000 sqlstrings-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      909 2023-04-17 10:18:36.674581 sqlstrings-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-17 10:16:44.000000 sqlstrings-0.0.3/README.md
+-rw-rw-rw-   0        0        0      576 2023-04-17 10:17:22.000000 sqlstrings-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:18:36.676581 sqlstrings-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-04-17 10:17:16.000000 sqlstrings-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:18:36.628588 sqlstrings-0.0.3/sqlstrings/
+-rw-rw-rw-   0        0        0       75 2023-04-17 07:19:06.000000 sqlstrings-0.0.3/sqlstrings/__init__.py
+-rw-rw-rw-   0        0        0     3533 2023-04-14 09:26:10.000000 sqlstrings-0.0.3/sqlstrings/csv_handling.py
+-rw-rw-rw-   0        0        0     4543 2023-04-13 13:01:44.000000 sqlstrings-0.0.3/sqlstrings/postgre.py
+-rw-rw-rw-   0        0        0     4190 2023-03-31 16:29:50.000000 sqlstrings-0.0.3/sqlstrings/transact.py
+-rw-rw-rw-   0        0        0     2068 2023-04-14 09:05:58.000000 sqlstrings-0.0.3/sqlstrings/value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:18:36.655579 sqlstrings-0.0.3/sqlstrings.egg-info/
+-rw-rw-rw-   0        0        0      909 2023-04-17 10:18:36.000000 sqlstrings-0.0.3/sqlstrings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-17 10:18:36.000000 sqlstrings-0.0.3/sqlstrings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:18:36.000000 sqlstrings-0.0.3/sqlstrings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-17 10:18:36.000000 sqlstrings-0.0.3/sqlstrings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 10:18:36.671581 sqlstrings-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:43:40.000000 sqlstrings-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.3/tests/test_csv_handling.py
+-rw-rw-rw-   0        0        0      162 2023-03-31 16:28:49.000000 sqlstrings-0.0.3/tests/test_main.py
+-rw-rw-rw-   0        0        0     2472 2023-04-13 13:01:08.000000 sqlstrings-0.0.3/tests/test_postgre.py
+-rw-rw-rw-   0        0        0     1984 2023-04-12 16:19:18.000000 sqlstrings-0.0.3/tests/test_transact.py
+-rw-rw-rw-   0        0        0     1632 2023-04-12 16:19:28.000000 sqlstrings-0.0.3/tests/test_value_handling.py
```

### Comparing `sqlstrings-0.0.2/LICENSE` & `sqlstrings-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.2/PKG-INFO` & `sqlstrings-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: Ali Kellaway <ali.kellaway139@gmail.com>
 Project-URL: Homepage, https://github.com/alikellaway/sqlstrings
 Keywords: sql database python library strings generate
 Classifier: Programming Language :: Python :: 3
@@ -14,7 +14,8 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlstrings
 This package contains functions allowing a user to generate SQL query strings in multiple dialects. It is also able to take in csv files and convert them into statements for easy upload of csv files into databases.
 
 
+Repo: https://github.com/alikellaway/sqlstrings.git
```

### Comparing `sqlstrings-0.0.2/pyproject.toml` & `sqlstrings-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlstrings"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ali Kellaway", email="ali.kellaway139@gmail.com" },
 ]
 description = "Package generates SQL query strings in multiple dialects."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sqlstrings-0.0.2/setup.py` & `sqlstrings-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sqlstrings',
-    version='0.0.2',
+    version='0.0.3',
     description='A Python library for generating strings in different SQL dialects.',
     url='https://github.com/alikellaway/sqlstrings',
     author='Ali Kellaway',
     author_email='ali.kellaway139@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `sqlstrings-0.0.2/sqlstrings.egg-info/PKG-INFO` & `sqlstrings-0.0.3/sqlstrings.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: Ali Kellaway <ali.kellaway139@gmail.com>
 Project-URL: Homepage, https://github.com/alikellaway/sqlstrings
 Keywords: sql database python library strings generate
 Classifier: Programming Language :: Python :: 3
@@ -14,7 +14,8 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlstrings
 This package contains functions allowing a user to generate SQL query strings in multiple dialects. It is also able to take in csv files and convert them into statements for easy upload of csv files into databases.
 
 
+Repo: https://github.com/alikellaway/sqlstrings.git
```

### Comparing `sqlstrings-0.0.2/tests/test_postgre.py` & `sqlstrings-0.0.3/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.2/tests/test_transact.py` & `sqlstrings-0.0.3/tests/test_transact.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.2/tests/test_value_handling.py` & `sqlstrings-0.0.3/tests/test_value_handling.py`

 * *Files identical despite different names*

