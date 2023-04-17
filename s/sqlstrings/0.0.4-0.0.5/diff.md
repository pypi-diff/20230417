# Comparing `tmp/sqlstrings-0.0.4.tar.gz` & `tmp/sqlstrings-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlstrings-0.0.4.tar", last modified: Mon Apr 17 10:44:02 2023, max compression
+gzip compressed data, was "sqlstrings-0.0.5.tar", last modified: Mon Apr 17 11:05:16 2023, max compression
```

## Comparing `sqlstrings-0.0.4.tar` & `sqlstrings-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:44:02.966784 sqlstrings-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-17 07:54:03.000000 sqlstrings-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      909 2023-04-17 10:44:02.965786 sqlstrings-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-17 10:16:44.000000 sqlstrings-0.0.4/README.md
--rw-rw-rw-   0        0        0      576 2023-04-17 10:33:15.000000 sqlstrings-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-17 10:44:02.967784 sqlstrings-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      832 2023-04-17 10:36:08.000000 sqlstrings-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:44:02.947785 sqlstrings-0.0.4/sqlstrings.egg-info/
--rw-rw-rw-   0        0        0      909 2023-04-17 10:44:02.000000 sqlstrings-0.0.4/sqlstrings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-17 10:44:02.000000 sqlstrings-0.0.4/sqlstrings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:44:02.000000 sqlstrings-0.0.4/sqlstrings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-17 10:44:02.000000 sqlstrings-0.0.4/sqlstrings.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 10:44:02.963787 sqlstrings-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-03-31 15:43:40.000000 sqlstrings-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.4/tests/test_csv_handling.py
--rw-rw-rw-   0        0        0      162 2023-03-31 16:28:49.000000 sqlstrings-0.0.4/tests/test_main.py
--rw-rw-rw-   0        0        0     2472 2023-04-13 13:01:08.000000 sqlstrings-0.0.4/tests/test_postgre.py
--rw-rw-rw-   0        0        0     1984 2023-04-12 16:19:18.000000 sqlstrings-0.0.4/tests/test_transact.py
--rw-rw-rw-   0        0        0     1632 2023-04-12 16:19:28.000000 sqlstrings-0.0.4/tests/test_value_handling.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:05:16.134525 sqlstrings-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 07:54:03.000000 sqlstrings-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1010 2023-04-17 11:05:16.133527 sqlstrings-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-04-17 10:54:33.000000 sqlstrings-0.0.5/README.md
+-rw-rw-rw-   0        0        0      576 2023-04-17 10:55:09.000000 sqlstrings-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:05:16.135529 sqlstrings-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-04-17 11:04:22.000000 sqlstrings-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:05:16.106526 sqlstrings-0.0.5/sqlstrings.egg-info/
+-rw-rw-rw-   0        0        0     1010 2023-04-17 11:05:16.000000 sqlstrings-0.0.5/sqlstrings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-04-17 11:05:16.000000 sqlstrings-0.0.5/sqlstrings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:05:16.000000 sqlstrings-0.0.5/sqlstrings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-04-17 11:05:16.000000 sqlstrings-0.0.5/sqlstrings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 11:05:16.131526 sqlstrings-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-31 15:43:40.000000 sqlstrings-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-31 16:34:51.000000 sqlstrings-0.0.5/tests/test_csv_handling.py
+-rw-rw-rw-   0        0        0      162 2023-03-31 16:28:49.000000 sqlstrings-0.0.5/tests/test_main.py
+-rw-rw-rw-   0        0        0     2472 2023-04-13 13:01:08.000000 sqlstrings-0.0.5/tests/test_postgre.py
+-rw-rw-rw-   0        0        0     1984 2023-04-12 16:19:18.000000 sqlstrings-0.0.5/tests/test_transact.py
+-rw-rw-rw-   0        0        0     1632 2023-04-12 16:19:28.000000 sqlstrings-0.0.5/tests/test_value_handling.py
```

### Comparing `sqlstrings-0.0.4/LICENSE` & `sqlstrings-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.4/PKG-INFO` & `sqlstrings-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: Ali Kellaway <ali.kellaway139@gmail.com>
 Project-URL: Homepage, https://github.com/alikellaway/sqlstrings
 Keywords: sql database python library strings generate
 Classifier: Programming Language :: Python :: 3
@@ -13,9 +13,15 @@
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlstrings
 This package contains functions allowing a user to generate SQL query strings in multiple dialects. It is also able to take in csv files and convert them into statements for easy upload of csv files into databases.
 
+# Installation
+Run the following to install:
+'''python
+pip install sqlstrings
+'''
 
+# Contribute
 Repo: https://github.com/alikellaway/sqlstrings.git
```

### Comparing `sqlstrings-0.0.4/pyproject.toml` & `sqlstrings-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlstrings"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ali Kellaway", email="ali.kellaway139@gmail.com" },
 ]
 description = "Package generates SQL query strings in multiple dialects."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `sqlstrings-0.0.4/setup.py` & `sqlstrings-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup
 
 setup(
     name='sqlstrings',
-    version='0.0.4',
+    version='0.0.5',
     description='A Python library for generating strings in different SQL dialects.',
     package_dir={'sqlstrings':'src'},
     py_modules=['csv_handling', 'postgre', 'transact', 'value_handling'],
     url='https://github.com/alikellaway/sqlstrings',
     author='Ali Kellaway',
     author_email='ali.kellaway139@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',  # TODO Research licenses.
+        'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='sql database python library strings generate',
-    install_requires=[],
     python_requires='>=3.8, <4',
 )
```

### Comparing `sqlstrings-0.0.4/sqlstrings.egg-info/PKG-INFO` & `sqlstrings-0.0.5/sqlstrings.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlstrings
-Version: 0.0.4
+Version: 0.0.5
 Summary: Package generates SQL query strings in multiple dialects.
 Home-page: https://github.com/alikellaway/sqlstrings
 Author: Ali Kellaway
 Author-email: Ali Kellaway <ali.kellaway139@gmail.com>
 Project-URL: Homepage, https://github.com/alikellaway/sqlstrings
 Keywords: sql database python library strings generate
 Classifier: Programming Language :: Python :: 3
@@ -13,9 +13,15 @@
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sqlstrings
 This package contains functions allowing a user to generate SQL query strings in multiple dialects. It is also able to take in csv files and convert them into statements for easy upload of csv files into databases.
 
+# Installation
+Run the following to install:
+'''python
+pip install sqlstrings
+'''
 
+# Contribute
 Repo: https://github.com/alikellaway/sqlstrings.git
```

### Comparing `sqlstrings-0.0.4/tests/test_postgre.py` & `sqlstrings-0.0.5/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.4/tests/test_transact.py` & `sqlstrings-0.0.5/tests/test_transact.py`

 * *Files identical despite different names*

### Comparing `sqlstrings-0.0.4/tests/test_value_handling.py` & `sqlstrings-0.0.5/tests/test_value_handling.py`

 * *Files identical despite different names*

