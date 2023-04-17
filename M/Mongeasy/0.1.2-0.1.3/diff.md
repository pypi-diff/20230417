# Comparing `tmp/Mongeasy-0.1.2.tar.gz` & `tmp/Mongeasy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mongeasy-0.1.2.tar", last modified: Mon Apr 17 11:14:33 2023, max compression
+gzip compressed data, was "Mongeasy-0.1.3.tar", last modified: Mon Apr 17 11:51:01 2023, max compression
```

## Comparing `Mongeasy-0.1.2.tar` & `Mongeasy-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 11:14:33.009930 Mongeasy-0.1.2/
--rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-17 11:14:32.999417 Mongeasy-0.1.2/Mongeasy.egg-info/
--rw-rw-rw-   0        0        0     6982 2023-04-17 11:14:32.000000 Mongeasy-0.1.2/Mongeasy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-04-17 11:14:32.000000 Mongeasy-0.1.2/Mongeasy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 11:14:32.000000 Mongeasy-0.1.2/Mongeasy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 11:14:32.000000 Mongeasy-0.1.2/Mongeasy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 11:14:32.000000 Mongeasy-0.1.2/Mongeasy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-17 11:14:32.000000 Mongeasy-0.1.2/Mongeasy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6982 2023-04-17 11:14:33.010928 Mongeasy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6179 2023-04-17 10:49:55.000000 Mongeasy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 11:14:33.007930 Mongeasy-0.1.2/mongeasy/
--rw-rw-rw-   0        0        0     2035 2023-04-17 11:13:47.000000 Mongeasy-0.1.2/mongeasy/__init__.py
--rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.2/mongeasy/base_dict.py
--rw-rw-rw-   0        0        0    11100 2023-04-17 09:38:01.000000 Mongeasy-0.1.2/mongeasy/document.py
--rw-rw-rw-   0        0        0     2919 2023-04-17 08:03:57.000000 Mongeasy-0.1.2/mongeasy/dynamics.py
--rw-rw-rw-   0        0        0     1851 2023-03-09 08:28:25.000000 Mongeasy-0.1.2/mongeasy/exceptions.py
--rw-rw-rw-   0        0        0       20 2023-04-17 07:50:37.000000 Mongeasy-0.1.2/mongeasy/mongeasy.py
--rw-rw-rw-   0        0        0     4963 2023-04-17 10:49:05.000000 Mongeasy-0.1.2/mongeasy/resultlist.py
--rw-rw-rw-   0        0        0     1865 2023-04-17 08:02:18.000000 Mongeasy-0.1.2/mongeasy/utils.py
--rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2023-04-17 11:14:33.010928 Mongeasy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1076 2023-04-17 11:13:41.000000 Mongeasy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 11:14:33.009930 Mongeasy-0.1.2/tests/
--rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     9850 2023-04-17 09:38:19.000000 Mongeasy-0.1.2/tests/test_mongeasy.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:51:01.217608 Mongeasy-0.1.3/
+-rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-17 11:51:01.195967 Mongeasy-0.1.3/Mongeasy.egg-info/
+-rw-rw-rw-   0        0        0     6982 2023-04-17 11:51:01.000000 Mongeasy-0.1.3/Mongeasy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-04-17 11:51:01.000000 Mongeasy-0.1.3/Mongeasy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:51:01.000000 Mongeasy-0.1.3/Mongeasy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 11:51:01.000000 Mongeasy-0.1.3/Mongeasy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 11:51:01.000000 Mongeasy-0.1.3/Mongeasy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-17 11:51:01.000000 Mongeasy-0.1.3/Mongeasy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6982 2023-04-17 11:51:01.217608 Mongeasy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6179 2023-04-17 10:49:55.000000 Mongeasy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 11:51:01.214607 Mongeasy-0.1.3/mongeasy/
+-rw-rw-rw-   0        0        0     2035 2023-04-17 11:50:44.000000 Mongeasy-0.1.3/mongeasy/__init__.py
+-rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.3/mongeasy/base_dict.py
+-rw-rw-rw-   0        0        0    11378 2023-04-17 11:50:23.000000 Mongeasy-0.1.3/mongeasy/document.py
+-rw-rw-rw-   0        0        0     2919 2023-04-17 08:03:57.000000 Mongeasy-0.1.3/mongeasy/dynamics.py
+-rw-rw-rw-   0        0        0     1851 2023-03-09 08:28:25.000000 Mongeasy-0.1.3/mongeasy/exceptions.py
+-rw-rw-rw-   0        0        0       20 2023-04-17 07:50:37.000000 Mongeasy-0.1.3/mongeasy/mongeasy.py
+-rw-rw-rw-   0        0        0     4963 2023-04-17 10:49:05.000000 Mongeasy-0.1.3/mongeasy/resultlist.py
+-rw-rw-rw-   0        0        0     1865 2023-04-17 08:02:18.000000 Mongeasy-0.1.3/mongeasy/utils.py
+-rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1057 2023-04-17 11:51:01.219120 Mongeasy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2023-04-17 11:50:33.000000 Mongeasy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:51:01.216608 Mongeasy-0.1.3/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     9850 2023-04-17 09:38:19.000000 Mongeasy-0.1.3/tests/test_mongeasy.py
```

### Comparing `Mongeasy-0.1.2/LICENSE` & `Mongeasy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.2/Mongeasy.egg-info/PKG-INFO` & `Mongeasy-0.1.3/Mongeasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Mongeasy-0.1.2/PKG-INFO` & `Mongeasy-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mongeasy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Mongeasy-0.1.2/README.md` & `Mongeasy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.2/mongeasy/__init__.py` & `Mongeasy-0.1.3/mongeasy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Mongeasy."""
 
 __author__ = """Joakim Wassberg"""
 __email__ = 'joakim.wassberg@arthead.se'
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 import os
 import configparser
 import pymongo
 from mongeasy.exceptions import MongEasyDBConnectionError
 from mongeasy.dynamics import create_document_class
```

### Comparing `Mongeasy-0.1.2/mongeasy/base_dict.py` & `Mongeasy-0.1.3/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.2/mongeasy/document.py` & `Mongeasy-0.1.3/mongeasy/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,23 @@
         """
         Returns all documents in the collection
         :return: ResultList
         """
         return ResultList(cls(item) for item in cls.collection.find({}))
 
     @classmethod
+    def all_iter(cls) -> dict:
+        """
+        Retrieve all documents from the collection as an iterator
+        :yields: dict representation of next document
+        """
+        for item in cls.collection.find({}):
+            yield cls(**item).to_dict()
+
+    @classmethod
     def delete(cls, *args, **kwargs) -> None:
         """
         Delete the document that matches the keywords
 
         :param args: positional arguments
         :param kwargs: keyword arguments or dict to match
         :return: None
```

### Comparing `Mongeasy-0.1.2/mongeasy/dynamics.py` & `Mongeasy-0.1.3/mongeasy/dynamics.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.2/mongeasy/exceptions.py` & `Mongeasy-0.1.3/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.2/mongeasy/resultlist.py` & `Mongeasy-0.1.3/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.2/mongeasy/utils.py` & `Mongeasy-0.1.3/mongeasy/utils.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.2/setup.cfg` & `Mongeasy-0.1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6e 6765 6173 790d 0a76 6572   = mongeasy..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e32 0d0a 6175  sion = 0.1.2..au
+00000020: 7369 6f6e 203d 2030 2e31 2e33 0d0a 6175  sion = 0.1.3..au
 00000030: 7468 6f72 203d 204a 6f61 6b69 6d20 5761  thor = Joakim Wa
 00000040: 7373 6265 7267 0d0a 6175 7468 6f72 5f65  ssberg..author_e
 00000050: 6d61 696c 203d 206a 6f61 6b69 6d2e 7761  mail = joakim.wa
 00000060: 7373 6265 7267 4061 7274 6865 6164 2e73  ssberg@arthead.s
 00000070: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
 00000080: 2045 6173 7920 746f 2075 7365 2077 7261   Easy to use wra
 00000090: 7070 6572 2061 726f 756e 6420 7079 6d6f  pper around pymo
```

### Comparing `Mongeasy-0.1.2/setup.py` & `Mongeasy-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="Mongeasy",
-    version="0.1.2",
+    version="0.1.3",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `Mongeasy-0.1.2/tests/test_mongeasy.py` & `Mongeasy-0.1.3/tests/test_mongeasy.py`

 * *Files identical despite different names*

