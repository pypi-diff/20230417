# Comparing `tmp/Mongeasy-0.1.0.tar.gz` & `tmp/Mongeasy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mongeasy-0.1.0.tar", last modified: Mon Apr 17 11:03:39 2023, max compression
+gzip compressed data, was "Mongeasy-0.1.1.tar", last modified: Mon Apr 17 11:09:43 2023, max compression
```

## Comparing `Mongeasy-0.1.0.tar` & `Mongeasy-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:03:39.530413 Mongeasy-0.1.0/
--rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-17 11:03:39.512887 Mongeasy-0.1.0/Mongeasy.egg-info/
--rw-rw-rw-   0        0        0     6906 2023-04-17 11:03:39.000000 Mongeasy-0.1.0/Mongeasy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-04-17 11:03:39.000000 Mongeasy-0.1.0/Mongeasy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:03:39.000000 Mongeasy-0.1.0/Mongeasy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 11:03:39.000000 Mongeasy-0.1.0/Mongeasy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 11:03:39.000000 Mongeasy-0.1.0/Mongeasy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6906 2023-04-17 11:03:39.529406 Mongeasy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6179 2023-04-17 10:49:55.000000 Mongeasy-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 11:03:39.525894 Mongeasy-0.1.0/mongeasy/
--rw-rw-rw-   0        0        0     2035 2023-04-17 07:56:47.000000 Mongeasy-0.1.0/mongeasy/__init__.py
--rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.0/mongeasy/base_dict.py
--rw-rw-rw-   0        0        0    11100 2023-04-17 09:38:01.000000 Mongeasy-0.1.0/mongeasy/document.py
--rw-rw-rw-   0        0        0     2919 2023-04-17 08:03:57.000000 Mongeasy-0.1.0/mongeasy/dynamics.py
--rw-rw-rw-   0        0        0     1851 2023-03-09 08:28:25.000000 Mongeasy-0.1.0/mongeasy/exceptions.py
--rw-rw-rw-   0        0        0       20 2023-04-17 07:50:37.000000 Mongeasy-0.1.0/mongeasy/mongeasy.py
--rw-rw-rw-   0        0        0     4963 2023-04-17 10:49:05.000000 Mongeasy-0.1.0/mongeasy/resultlist.py
--rw-rw-rw-   0        0        0     1865 2023-04-17 08:02:18.000000 Mongeasy-0.1.0/mongeasy/utils.py
--rw-rw-rw-   0        0        0       42 2023-04-17 11:03:39.530413 Mongeasy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-04-17 10:57:00.000000 Mongeasy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:03:39.527400 Mongeasy-0.1.0/tests/
--rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     9850 2023-04-17 09:38:19.000000 Mongeasy-0.1.0/tests/test_mongeasy.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:43.141632 Mongeasy-0.1.1/
+-rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:43.126119 Mongeasy-0.1.1/Mongeasy.egg-info/
+-rw-rw-rw-   0        0        0     6906 2023-04-17 11:09:43.000000 Mongeasy-0.1.1/Mongeasy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      411 2023-04-17 11:09:43.000000 Mongeasy-0.1.1/Mongeasy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:09:43.000000 Mongeasy-0.1.1/Mongeasy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 11:09:43.000000 Mongeasy-0.1.1/Mongeasy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 11:09:43.000000 Mongeasy-0.1.1/Mongeasy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6906 2023-04-17 11:09:43.140632 Mongeasy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6179 2023-04-17 10:49:55.000000 Mongeasy-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:43.137632 Mongeasy-0.1.1/mongeasy/
+-rw-rw-rw-   0        0        0     2035 2023-04-17 11:08:48.000000 Mongeasy-0.1.1/mongeasy/__init__.py
+-rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.1/mongeasy/base_dict.py
+-rw-rw-rw-   0        0        0    11100 2023-04-17 09:38:01.000000 Mongeasy-0.1.1/mongeasy/document.py
+-rw-rw-rw-   0        0        0     2919 2023-04-17 08:03:57.000000 Mongeasy-0.1.1/mongeasy/dynamics.py
+-rw-rw-rw-   0        0        0     1851 2023-03-09 08:28:25.000000 Mongeasy-0.1.1/mongeasy/exceptions.py
+-rw-rw-rw-   0        0        0       20 2023-04-17 07:50:37.000000 Mongeasy-0.1.1/mongeasy/mongeasy.py
+-rw-rw-rw-   0        0        0     4963 2023-04-17 10:49:05.000000 Mongeasy-0.1.1/mongeasy/resultlist.py
+-rw-rw-rw-   0        0        0     1865 2023-04-17 08:02:18.000000 Mongeasy-0.1.1/mongeasy/utils.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:09:43.141632 Mongeasy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-17 11:08:41.000000 Mongeasy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:09:43.139633 Mongeasy-0.1.1/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     9850 2023-04-17 09:38:19.000000 Mongeasy-0.1.1/tests/test_mongeasy.py
```

### Comparing `Mongeasy-0.1.0/LICENSE` & `Mongeasy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/Mongeasy.egg-info/PKG-INFO` & `Mongeasy-0.1.1/Mongeasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `Mongeasy-0.1.0/PKG-INFO` & `Mongeasy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `Mongeasy-0.1.0/README.md` & `Mongeasy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/mongeasy/__init__.py` & `Mongeasy-0.1.1/mongeasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Mongeasy."""
 
 __author__ = """Joakim Wassberg"""
 __email__ = 'joakim.wassberg@arthead.se'
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import os
 import configparser
 import pymongo
 from mongeasy.exceptions import MongEasyDBConnectionError
 from mongeasy.dynamics import create_document_class
```

### Comparing `Mongeasy-0.1.0/mongeasy/base_dict.py` & `Mongeasy-0.1.1/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/mongeasy/document.py` & `Mongeasy-0.1.1/mongeasy/document.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/mongeasy/dynamics.py` & `Mongeasy-0.1.1/mongeasy/dynamics.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/mongeasy/exceptions.py` & `Mongeasy-0.1.1/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/mongeasy/resultlist.py` & `Mongeasy-0.1.1/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/mongeasy/utils.py` & `Mongeasy-0.1.1/mongeasy/utils.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.0/setup.py` & `Mongeasy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="Mongeasy",
-    version="0.1.0",
+    version="0.1.1",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `Mongeasy-0.1.0/tests/test_mongeasy.py` & `Mongeasy-0.1.1/tests/test_mongeasy.py`

 * *Files identical despite different names*

