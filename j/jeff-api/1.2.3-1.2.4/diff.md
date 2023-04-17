# Comparing `tmp/jeff_api-1.2.3.tar.gz` & `tmp/jeff_api-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.2.3.tar", last modified: Mon Apr 17 16:58:16 2023, max compression
+gzip compressed data, was "jeff_api-1.2.4.tar", last modified: Mon Apr 17 17:19:01 2023, max compression
```

## Comparing `jeff_api-1.2.3.tar` & `jeff_api-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 16:58:16.528834 jeff_api-1.2.3/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.3/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 16:58:16.528834 jeff_api-1.2.3/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.3/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 16:57:25.000000 jeff_api-1.2.3/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 16:58:16.530834 jeff_api-1.2.3/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 16:58:16.492833 jeff_api-1.2.3/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 16:58:16.524834 jeff_api-1.2.3/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.3/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     7745 2023-04-17 00:58:34.000000 jeff_api-1.2.3/src/jeff_api/bridge.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1778 2023-04-17 16:28:35.000000 jeff_api-1.2.3/src/jeff_api/extension.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.3/src/jeff_api/message.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.3/src/jeff_api/tools.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 16:58:16.528834 jeff_api-1.2.3/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 16:58:16.000000 jeff_api-1.2.3/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 16:58:16.000000 jeff_api-1.2.3/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 16:58:16.000000 jeff_api-1.2.3/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 16:58:16.000000 jeff_api-1.2.3/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.294085 jeff_api-1.2.4/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.4/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:19:01.294085 jeff_api-1.2.4/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.4/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 17:18:23.000000 jeff_api-1.2.4/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 17:19:01.296085 jeff_api-1.2.4/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.238083 jeff_api-1.2.4/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.290085 jeff_api-1.2.4/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.4/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     7745 2023-04-17 00:58:34.000000 jeff_api-1.2.4/src/jeff_api/bridge.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1767 2023-04-17 17:15:10.000000 jeff_api-1.2.4/src/jeff_api/extension.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.4/src/jeff_api/message.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.4/src/jeff_api/tools.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:19:01.292086 jeff_api-1.2.4/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 17:19:01.000000 jeff_api-1.2.4/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.2.3/LICENSE` & `jeff_api-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.3/PKG-INFO` & `jeff_api-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.2.3/src/jeff_api/bridge.py` & `jeff_api-1.2.4/src/jeff_api/bridge.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.3/src/jeff_api/extension.py` & `jeff_api-1.2.4/src/jeff_api/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     if self.__verbose:
       print('Parsed arguments.')
     self.bridge = Bridge(jeff_host, self.__jeff_port, extension_host, self.__extension_port)
     self.__initialized = True
 
   def handle_shutdown(self) -> None:
     "TBD"
-    del self.bridge
+    pass
 
   def handle_message(self, message: Message) -> None:
     "TBD"
     pass
 
   def run(self) -> None:
     "TBD"
```

### Comparing `jeff_api-1.2.3/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.2.4/src/jeff_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.2.3
+Version: 1.2.4
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

