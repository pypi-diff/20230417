# Comparing `tmp/paddypy-0.0.7.tar.gz` & `tmp/paddypy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.0.7.tar", last modified: Mon Apr 17 10:36:30 2023, max compression
+gzip compressed data, was "paddypy-0.0.8.tar", last modified: Mon Apr 17 10:48:43 2023, max compression
```

## Comparing `paddypy-0.0.7.tar` & `paddypy-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:36:30.689571 paddypy-0.0.7/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-04-17 10:36:30.689072 paddypy-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 10:36:30.677072 paddypy-0.0.7/paddypy/
--rw-rw-rw-   0        0        0       53 2023-04-17 10:31:46.000000 paddypy-0.0.7/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2022-10-19 07:57:58.000000 paddypy-0.0.7/paddypy/access.py
--rw-rw-rw-   0        0        0     2851 2023-04-17 10:31:34.000000 paddypy-0.0.7/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:36:30.688072 paddypy-0.0.7/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 10:36:30.000000 paddypy-0.0.7/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 10:36:30.689571 paddypy-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1449 2023-04-17 10:36:10.000000 paddypy-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:43.899375 paddypy-0.0.8/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-04-17 10:48:43.898875 paddypy-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:43.887375 paddypy-0.0.8/paddypy/
+-rw-rw-rw-   0        0        0       53 2023-04-17 10:31:46.000000 paddypy-0.0.8/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2022-10-19 07:57:58.000000 paddypy-0.0.8/paddypy/access.py
+-rw-rw-rw-   0        0        0     2905 2023-04-17 10:47:40.000000 paddypy-0.0.8/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:48:43.897875 paddypy-0.0.8/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 10:48:43.000000 paddypy-0.0.8/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:48:43.899875 paddypy-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1449 2023-04-17 10:48:23.000000 paddypy-0.0.8/setup.py
```

### Comparing `paddypy-0.0.7/LICENSE` & `paddypy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.7/PKG-INFO` & `paddypy-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.0.7/README.md` & `paddypy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.7/paddypy/access.py` & `paddypy-0.0.8/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.0.7/paddypy/log.py` & `paddypy-0.0.8/paddypy/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from functools import wraps
 import time
 import logging
 import datetime
 import access
 
 class CloudLogger():
-    def __init__(self, app_logger_name, logger_level=int(access.getValue(key="loggging-level", deactivate_kv_access=False))):
+    def __init__(self, app_logger_name, module_name, logger_level=int(access.getValue(key="loggging-level", deactivate_kv_access=False))):
         self.LOGGER_LEVEL = logger_level
-        self.logger = self._get_logger(module_name=app_logger_name)
+        self.logger = self._get_logger(app_logger_name=app_logger_name, module_name=module_name)
 
         
-    def _get_logger(self, module_name):
+    def _get_logger(self, app_logger_name, module_name):
         FMT = "[{levelname:^9}] {name}: {message}"
         FORMATS = {
             logging.DEBUG: FMT,
             logging.INFO: "\33[36m{fmt}\33[0m".format(fmt=FMT),
             logging.WARNING: "\33[33m{fmt}\33[0m".format(fmt=FMT),
             logging.ERROR: "\33[31m{fmt}\33[0m".format(fmt=FMT),
             logging.CRITICAL: "\33[1m\33[31m{fmt}\33[0m".format(fmt=FMT)
@@ -34,15 +34,15 @@
         handler = logging.StreamHandler()
         handler.setFormatter(CustomFormatter())
         logging.basicConfig(
             level=self.LOGGER_LEVEL,
             handlers=[handler]
         )
 
-        logger = logging.getLogger(self.app_logger_name).getChild(module_name)
+        logger = logging.getLogger(app_logger_name).getChild(module_name)
         return logger
 
 
     def timeit(self, func):
         @wraps(func)
         def timeit_wrapper(*args, **kwargs):
             start_time = time.perf_counter()
```

### Comparing `paddypy-0.0.7/paddypy.egg-info/PKG-INFO` & `paddypy-0.0.8/paddypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.0.7/setup.py` & `paddypy-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

