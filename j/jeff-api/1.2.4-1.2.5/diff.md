# Comparing `tmp/jeff_api-1.2.4.tar.gz` & `tmp/jeff_api-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.2.4.tar", last modified: Mon Apr 17 17:19:01 2023, max compression
+gzip compressed data, was "jeff_api-1.2.5.tar", last modified: Mon Apr 17 17:31:38 2023, max compression
```

## Comparing `jeff_api-1.2.4.tar` & `jeff_api-1.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.294085 jeff_api-1.2.4/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.4/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:19:01.294085 jeff_api-1.2.4/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.4/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 17:18:23.000000 jeff_api-1.2.4/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 17:19:01.296085 jeff_api-1.2.4/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.238083 jeff_api-1.2.4/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.290085 jeff_api-1.2.4/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.4/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     7745 2023-04-17 00:58:34.000000 jeff_api-1.2.4/src/jeff_api/bridge.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1767 2023-04-17 17:15:10.000000 jeff_api-1.2.4/src/jeff_api/extension.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.4/src/jeff_api/message.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.4/src/jeff_api/tools.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.292086 jeff_api-1.2.4/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.642183 jeff_api-1.2.5/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.5/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:31:38.640183 jeff_api-1.2.5/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.5/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 17:30:51.000000 jeff_api-1.2.5/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 17:31:38.642183 jeff_api-1.2.5/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.610183 jeff_api-1.2.5/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.636183 jeff_api-1.2.5/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.5/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     7745 2023-04-17 00:58:34.000000 jeff_api-1.2.5/src/jeff_api/bridge.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1881 2023-04-17 17:30:36.000000 jeff_api-1.2.5/src/jeff_api/extension.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.5/src/jeff_api/message.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.5/src/jeff_api/tools.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.640183 jeff_api-1.2.5/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.2.4/LICENSE` & `jeff_api-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.4/PKG-INFO` & `jeff_api-1.2.5/src/jeff_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jeff_api
-Version: 1.2.4
+Name: jeff-api
+Version: 1.2.5
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.2.4/src/jeff_api/bridge.py` & `jeff_api-1.2.5/src/jeff_api/bridge.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.4/src/jeff_api/extension.py` & `jeff_api-1.2.5/src/jeff_api/extension.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, sys
+import argparse, signal
 from typing import Optional
 from .bridge import Bridge
 from .message import Message
 
 
 class ExtensionNotStartedException(Exception):
   "The extension isn't started properly."
@@ -15,14 +15,16 @@
   def __init__(self, ext_description: str, auto_on: bool = True):
     "TBD"
     self.args_parser = argparse.ArgumentParser(description=ext_description)
     self.args_parser.add_argument("extension_port", type=int, help="extension's server port")
     self.args_parser.add_argument("jeff_port", type=int, help="Jeff port")
     self.args_parser.add_argument("-v", "--verbose", action="store_true", help="verbose output")
     self.__initialized: bool = False
+    signal.signal(signal.SIGINT, self.handle_shutdown)
+    signal.signal(signal.SIGTERM, self.handle_shutdown)
     if auto_on: self.turn_on('localhost', None)
 
   def turn_on(self, jeff_host: Optional[str] = None, extension_host: Optional[str] = None):
     "TBD"
     args = self.args_parser.parse_args()
     self.__extension_port: int = args.extension_port
     self.__jeff_port: int = args.jeff_port
```

### Comparing `jeff_api-1.2.4/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jeff-api
-Version: 1.2.4
+Name: jeff_api
+Version: 1.2.5
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

