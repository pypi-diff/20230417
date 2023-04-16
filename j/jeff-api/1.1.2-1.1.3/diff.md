# Comparing `tmp/jeff_api-1.1.2.tar.gz` & `tmp/jeff_api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.1.2.tar", last modified: Sun Apr 16 23:02:49 2023, max compression
+gzip compressed data, was "jeff_api-1.1.3.tar", last modified: Sun Apr 16 23:05:14 2023, max compression
```

## Comparing `jeff_api-1.1.2.tar` & `jeff_api-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:02:49.497427 jeff_api-1.1.2/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.1.2/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-16 23:02:49.497427 jeff_api-1.1.2/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.1.2/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 23:02:18.000000 jeff_api-1.1.2/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 23:02:49.497427 jeff_api-1.1.2/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:02:49.485426 jeff_api-1.1.2/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:02:49.493426 jeff_api-1.1.2/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)      120 2023-04-16 22:46:34.000000 jeff_api-1.1.2/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     3635 2023-04-16 23:01:35.000000 jeff_api-1.1.2/src/jeff_api/bridge.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1760 2023-04-16 22:42:49.000000 jeff_api-1.1.2/src/jeff_api/extension.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.1.2/src/jeff_api/message.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     3671 2023-04-16 23:02:10.000000 jeff_api-1.1.2/src/jeff_api/scenario.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.1.2/src/jeff_api/tools.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:02:49.495427 jeff_api-1.1.2/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-16 23:02:49.000000 jeff_api-1.1.2/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      321 2023-04-16 23:02:49.000000 jeff_api-1.1.2/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 23:02:49.000000 jeff_api-1.1.2/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 23:02:49.000000 jeff_api-1.1.2/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:05:14.828948 jeff_api-1.1.3/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.1.3/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-16 23:05:14.828948 jeff_api-1.1.3/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.1.3/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 23:04:45.000000 jeff_api-1.1.3/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 23:05:14.828948 jeff_api-1.1.3/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:05:14.816947 jeff_api-1.1.3/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:05:14.824948 jeff_api-1.1.3/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      120 2023-04-16 22:46:34.000000 jeff_api-1.1.3/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     3635 2023-04-16 23:01:35.000000 jeff_api-1.1.3/src/jeff_api/bridge.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1759 2023-04-16 23:04:37.000000 jeff_api-1.1.3/src/jeff_api/extension.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.1.3/src/jeff_api/message.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     3671 2023-04-16 23:02:10.000000 jeff_api-1.1.3/src/jeff_api/scenario.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.1.3/src/jeff_api/tools.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 23:05:14.826948 jeff_api-1.1.3/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-16 23:05:14.000000 jeff_api-1.1.3/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      321 2023-04-16 23:05:14.000000 jeff_api-1.1.3/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 23:05:14.000000 jeff_api-1.1.3/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 23:05:14.000000 jeff_api-1.1.3/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.1.2/LICENSE` & `jeff_api-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.1.2/PKG-INFO` & `jeff_api-1.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.1.2/src/jeff_api/bridge.py` & `jeff_api-1.1.3/src/jeff_api/bridge.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.1.2/src/jeff_api/extension.py` & `jeff_api-1.1.3/src/jeff_api/extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   "The extension isn't started properly."
   pass
 
 
 class Extension:
   "TBD"
 
-  def __init__(self, ext_description: str, auto_on: bool = False):
+  def __init__(self, ext_description: str, auto_on: bool = True):
     "TBD"
     self.args_parser = argparse.ArgumentParser(description=ext_description)
     self.args_parser.add_argument("extension_port", type=int, help="extension's server port")
     self.args_parser.add_argument("jeff_port", type=int, help="Jeff port")
     self.args_parser.add_argument("-v", "--verbose", action="store_true", help="verbose output")
     self.__initialized: bool = False
     if auto_on: self.turn_on(None, None)
```

### Comparing `jeff_api-1.1.2/src/jeff_api/scenario.py` & `jeff_api-1.1.3/src/jeff_api/scenario.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.1.2/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.1.3/src/jeff_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

