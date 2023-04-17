# Comparing `tmp/rext-0.1.8.tar.gz` & `tmp/rext-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rext-0.1.8.tar", last modified: Wed Jun  8 05:22:10 2022, max compression
+gzip compressed data, was "rext-0.1.9.tar", last modified: Mon Jul  4 06:08:06 2022, max compression
```

## Comparing `rext-0.1.8.tar` & `rext-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nsk        (501) staff       (20)        0 2022-06-08 05:22:10.874803 rext-0.1.8/
--rw-r--r--   0 nsk        (501) staff       (20)       53 2022-06-08 02:22:50.000000 rext-0.1.8/.gitignore
-drwxr-xr-x   0 nsk        (501) staff       (20)        0 2022-06-08 05:22:10.872467 rext-0.1.8/.vscode/
--rw-r--r--   0 nsk        (501) staff       (20)      414 2021-09-28 08:45:50.000000 rext-0.1.8/.vscode/settings.json
--rw-r--r--   0 nsk        (501) staff       (20)     1067 2021-12-02 13:41:44.000000 rext-0.1.8/LICENSE
--rw-r--r--   0 nsk        (501) staff       (20)      910 2022-06-08 05:22:10.874441 rext-0.1.8/PKG-INFO
--rw-r--r--   0 nsk        (501) staff       (20)      286 2022-06-08 02:25:56.000000 rext-0.1.8/README.md
-drwxr-xr-x   0 nsk        (501) staff       (20)        0 2022-06-08 05:22:10.873996 rext-0.1.8/rext.egg-info/
--rw-r--r--   0 nsk        (501) staff       (20)      910 2022-06-08 05:22:10.000000 rext-0.1.8/rext.egg-info/PKG-INFO
--rw-r--r--   0 nsk        (501) staff       (20)      206 2022-06-08 05:22:10.000000 rext-0.1.8/rext.egg-info/SOURCES.txt
--rw-r--r--   0 nsk        (501) staff       (20)        1 2022-06-08 05:22:10.000000 rext-0.1.8/rext.egg-info/dependency_links.txt
--rw-r--r--   0 nsk        (501) staff       (20)       15 2022-06-08 05:22:10.000000 rext-0.1.8/rext.egg-info/requires.txt
--rw-r--r--   0 nsk        (501) staff       (20)        5 2022-06-08 05:22:10.000000 rext-0.1.8/rext.egg-info/top_level.txt
--rw-r--r--   0 nsk        (501) staff       (20)     5615 2022-06-08 05:17:50.000000 rext-0.1.8/rext.py
--rw-r--r--   0 nsk        (501) staff       (20)       38 2022-06-08 05:22:10.874879 rext-0.1.8/setup.cfg
--rw-r--r--   0 nsk        (501) staff       (20)     3740 2022-06-08 05:17:55.000000 rext-0.1.8/setup.py
+drwxr-xr-x   0 nsk        (501) staff       (20)        0 2022-07-04 06:08:06.898337 rext-0.1.9/
+-rw-r--r--   0 nsk        (501) staff       (20)       53 2022-06-08 02:22:50.000000 rext-0.1.9/.gitignore
+drwxr-xr-x   0 nsk        (501) staff       (20)        0 2022-07-04 06:08:06.893428 rext-0.1.9/.vscode/
+-rw-r--r--   0 nsk        (501) staff       (20)      414 2021-09-28 08:45:50.000000 rext-0.1.9/.vscode/settings.json
+-rw-r--r--   0 nsk        (501) staff       (20)     1067 2021-12-02 13:41:44.000000 rext-0.1.9/LICENSE
+-rw-r--r--   0 nsk        (501) staff       (20)      910 2022-07-04 06:08:06.898157 rext-0.1.9/PKG-INFO
+-rw-r--r--   0 nsk        (501) staff       (20)      286 2022-06-08 02:25:56.000000 rext-0.1.9/README.md
+drwxr-xr-x   0 nsk        (501) staff       (20)        0 2022-07-04 06:08:06.897937 rext-0.1.9/rext.egg-info/
+-rw-r--r--   0 nsk        (501) staff       (20)      910 2022-07-04 06:08:06.000000 rext-0.1.9/rext.egg-info/PKG-INFO
+-rw-r--r--   0 nsk        (501) staff       (20)      206 2022-07-04 06:08:06.000000 rext-0.1.9/rext.egg-info/SOURCES.txt
+-rw-r--r--   0 nsk        (501) staff       (20)        1 2022-07-04 06:08:06.000000 rext-0.1.9/rext.egg-info/dependency_links.txt
+-rw-r--r--   0 nsk        (501) staff       (20)       15 2022-07-04 06:08:06.000000 rext-0.1.9/rext.egg-info/requires.txt
+-rw-r--r--   0 nsk        (501) staff       (20)        5 2022-07-04 06:08:06.000000 rext-0.1.9/rext.egg-info/top_level.txt
+-rw-r--r--   0 nsk        (501) staff       (20)     5909 2022-07-04 06:04:28.000000 rext-0.1.9/rext.py
+-rw-r--r--   0 nsk        (501) staff       (20)       38 2022-07-04 06:08:06.898386 rext-0.1.9/setup.cfg
+-rw-r--r--   0 nsk        (501) staff       (20)     3740 2022-07-04 06:04:22.000000 rext-0.1.9/setup.py
```

### Comparing `rext-0.1.8/LICENSE` & `rext-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rext-0.1.8/PKG-INFO` & `rext-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rext
-Version: 0.1.8
+Version: 0.1.9
 Summary: A toolbox by Rex
 Home-page: https://github.com/FallingHeart/rext
 Author: rex nathan
 Author-email: ceo@bamo.tech
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rext-0.1.8/rext.egg-info/PKG-INFO` & `rext-0.1.9/rext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rext
-Version: 0.1.8
+Version: 0.1.9
 Summary: A toolbox by Rex
 Home-page: https://github.com/FallingHeart/rext
 Author: rex nathan
 Author-email: ceo@bamo.tech
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rext-0.1.8/rext.py` & `rext-0.1.9/rext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 import pymongo
 import pandas as pd
 import os
 import csv
 import json
 import pytz
@@ -164,14 +164,24 @@
         for i, item in enumerate(list):
             if key == "":
                 temp_map[i] = item
             else:
                 temp_map[item[key]] = item
         return temp_map
 
+    def tranlate_header(data, col_dict):
+        result_data = []
+        for row in data:
+            temp = {}
+            for key in row.keys():
+                if key != "":
+                    temp[col_dict[key]] = row[key]
+            result_data.append(temp)
+        return result_data
+
 
 class mdict():
 
     def to_list(map):
         temp_list = []
         for i in map:
             temp_list.append(map[i])
```

### Comparing `rext-0.1.8/setup.py` & `rext-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'rext'
 DESCRIPTION = 'A toolbox by Rex'
 URL = 'https://github.com/FallingHeart/rext'
 EMAIL = 'ceo@bamo.tech'
 AUTHOR = 'rex nathan'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pymongo', 'pandas',
 ]
 
 # What packages are optional?
```

