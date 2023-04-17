# Comparing `tmp/paddypy-0.0.8.tar.gz` & `tmp/paddypy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.0.8.tar", last modified: Mon Apr 17 10:48:43 2023, max compression
+gzip compressed data, was "paddypy-0.0.9.tar", last modified: Mon Apr 17 11:00:01 2023, max compression
```

## Comparing `paddypy-0.0.8.tar` & `paddypy-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:48:43.899375 paddypy-0.0.8/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-04-17 10:48:43.898875 paddypy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:48:43.887375 paddypy-0.0.8/paddypy/
--rw-rw-rw-   0        0        0       53 2023-04-17 10:31:46.000000 paddypy-0.0.8/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2022-10-19 07:57:58.000000 paddypy-0.0.8/paddypy/access.py
--rw-rw-rw-   0        0        0     2905 2023-04-17 10:47:40.000000 paddypy-0.0.8/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:48:43.897875 paddypy-0.0.8/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:48:43.899875 paddypy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1449 2023-04-17 10:48:23.000000 paddypy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:00:01.333416 paddypy-0.0.9/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-04-17 11:00:01.332916 paddypy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 11:00:01.321414 paddypy-0.0.9/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 10:59:11.000000 paddypy-0.0.9/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2022-10-19 07:57:58.000000 paddypy-0.0.9/paddypy/access.py
+-rw-rw-rw-   0        0        0     2912 2023-04-17 10:59:27.000000 paddypy-0.0.9/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:00:01.331915 paddypy-0.0.9/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 11:00:01.000000 paddypy-0.0.9/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:00:01.333416 paddypy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1449 2023-04-17 10:59:57.000000 paddypy-0.0.9/setup.py
```

### Comparing `paddypy-0.0.8/LICENSE` & `paddypy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.8/PKG-INFO` & `paddypy-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.0.8/README.md` & `paddypy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.8/paddypy/access.py` & `paddypy-0.0.9/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.8/paddypy/log.py` & `paddypy-0.0.9/paddypy/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from functools import wraps
 import time
 import logging
 import datetime
-import access
+from . import access
 
 class CloudLogger():
     def __init__(self, app_logger_name, module_name, logger_level=int(access.getValue(key="loggging-level", deactivate_kv_access=False))):
         self.LOGGER_LEVEL = logger_level
         self.logger = self._get_logger(app_logger_name=app_logger_name, module_name=module_name)
```

### Comparing `paddypy-0.0.8/paddypy.egg-info/PKG-INFO` & `paddypy-0.0.9/paddypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.0.8/setup.py` & `paddypy-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

