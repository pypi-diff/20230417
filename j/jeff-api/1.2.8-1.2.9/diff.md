# Comparing `tmp/jeff_api-1.2.8.tar.gz` & `tmp/jeff_api-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.2.8.tar", last modified: Mon Apr 17 17:55:51 2023, max compression
+gzip compressed data, was "jeff_api-1.2.9.tar", last modified: Mon Apr 17 17:59:25 2023, max compression
```

## Comparing `jeff_api-1.2.8.tar` & `jeff_api-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:55:51.514620 jeff_api-1.2.8/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.8/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:55:51.512621 jeff_api-1.2.8/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.8/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 17:55:21.000000 jeff_api-1.2.8/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 17:55:51.514620 jeff_api-1.2.8/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:55:51.500620 jeff_api-1.2.8/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:55:51.508620 jeff_api-1.2.8/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.8/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     7871 2023-04-17 17:48:15.000000 jeff_api-1.2.8/src/jeff_api/bridge.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1900 2023-04-17 17:55:11.000000 jeff_api-1.2.8/src/jeff_api/extension.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.8/src/jeff_api/message.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.8/src/jeff_api/tools.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:55:51.512621 jeff_api-1.2.8/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:55:51.000000 jeff_api-1.2.8/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 17:55:51.000000 jeff_api-1.2.8/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 17:55:51.000000 jeff_api-1.2.8/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 17:55:51.000000 jeff_api-1.2.8/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:59:25.511910 jeff_api-1.2.9/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.9/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:59:25.505910 jeff_api-1.2.9/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.9/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 17:58:54.000000 jeff_api-1.2.9/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 17:59:25.511910 jeff_api-1.2.9/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:59:25.367909 jeff_api-1.2.9/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:59:25.499910 jeff_api-1.2.9/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.9/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     7871 2023-04-17 17:48:15.000000 jeff_api-1.2.9/src/jeff_api/bridge.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1920 2023-04-17 17:58:32.000000 jeff_api-1.2.9/src/jeff_api/extension.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.9/src/jeff_api/message.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.9/src/jeff_api/tools.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:59:25.505910 jeff_api-1.2.9/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:59:25.000000 jeff_api-1.2.9/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 17:59:25.000000 jeff_api-1.2.9/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 17:59:25.000000 jeff_api-1.2.9/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 17:59:25.000000 jeff_api-1.2.9/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.2.8/LICENSE` & `jeff_api-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.8/PKG-INFO` & `jeff_api-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.2.8/src/jeff_api/bridge.py` & `jeff_api-1.2.9/src/jeff_api/bridge.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.8/src/jeff_api/extension.py` & `jeff_api-1.2.9/src/jeff_api/extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     if self.__verbose:
       print('Parsed arguments.')
     self.bridge = Bridge(jeff_host, self.__jeff_port, extension_host, self.__extension_port)
     self.__initialized = True
 
   def handle_shutdown(self, *args) -> None:
     "TBD"
+    del self.bridge
     sys.exit(0)
 
   def handle_message(self, message: Message) -> None:
     "TBD"
     pass
 
   def run(self) -> None:
```

### Comparing `jeff_api-1.2.8/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.2.9/src/jeff_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

