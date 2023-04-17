# Comparing `tmp/jeff_api-1.2.5.tar.gz` & `tmp/jeff_api-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.2.5.tar", last modified: Mon Apr 17 17:31:38 2023, max compression
+gzip compressed data, was "jeff_api-1.2.6.tar", last modified: Mon Apr 17 17:48:58 2023, max compression
```

## Comparing `jeff_api-1.2.5.tar` & `jeff_api-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.642183 jeff_api-1.2.5/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.5/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:31:38.640183 jeff_api-1.2.5/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.5/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 17:30:51.000000 jeff_api-1.2.5/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 17:31:38.642183 jeff_api-1.2.5/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.610183 jeff_api-1.2.5/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.636183 jeff_api-1.2.5/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.5/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     7745 2023-04-17 00:58:34.000000 jeff_api-1.2.5/src/jeff_api/bridge.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1881 2023-04-17 17:30:36.000000 jeff_api-1.2.5/src/jeff_api/extension.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.5/src/jeff_api/message.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.5/src/jeff_api/tools.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:31:38.640183 jeff_api-1.2.5/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 17:31:38.000000 jeff_api-1.2.5/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:48:58.975407 jeff_api-1.2.6/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.2.6/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:48:58.973407 jeff_api-1.2.6/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      254 2023-04-16 22:22:30.000000 jeff_api-1.2.6/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-17 17:48:26.000000 jeff_api-1.2.6/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-17 17:48:58.975407 jeff_api-1.2.6/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:48:58.961407 jeff_api-1.2.6/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:48:58.967407 jeff_api-1.2.6/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       89 2023-04-17 00:43:22.000000 jeff_api-1.2.6/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     7871 2023-04-17 17:48:15.000000 jeff_api-1.2.6/src/jeff_api/bridge.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1881 2023-04-17 17:30:36.000000 jeff_api-1.2.6/src/jeff_api/extension.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      474 2023-04-16 22:31:38.000000 jeff_api-1.2.6/src/jeff_api/message.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      188 2023-04-16 23:00:37.000000 jeff_api-1.2.6/src/jeff_api/tools.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-17 17:48:58.973407 jeff_api-1.2.6/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)      765 2023-04-17 17:48:58.000000 jeff_api-1.2.6/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      296 2023-04-17 17:48:58.000000 jeff_api-1.2.6/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-17 17:48:58.000000 jeff_api-1.2.6/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-17 17:48:58.000000 jeff_api-1.2.6/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.2.5/LICENSE` & `jeff_api-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.5/PKG-INFO` & `jeff_api-1.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.2.5/src/jeff_api/bridge.py` & `jeff_api-1.2.6/src/jeff_api/bridge.py`

 * *Files 13% similar despite different names*

```diff
@@ -229,22 +229,28 @@
     j = decode_json(self._accept(encode_json(j), buffer_size))
     if "memory_values" not in j: return None
     return j["memory_values"]
 
   def listen(self, buffer_size: int = 8192) -> dict:
     "TBD"
     if self.__scenario_status == ScenarioStates.UNUSED:
-      return decode_json(self._waits_for(buffer_size))
+      j: Any = dict()
+      try:
+        j = decode_json(self._waits_for(buffer_size))
+      except Exception as e:
+        print(f'Got an error: {e}.')
+        return {}
+      return j
     elif self.__scenario_status == ScenarioStates.STARTED:
       j: Any = dict()
       try:
         j = decode_json(self.bridge._waits_for(buffer_size))
-      except UnicodeDecodeError:
-        print('Unicode decode error.')
-        return j
+      except Exception as e:
+        print(f'Got an error: {e}.')
+        return {}
       if "sfinish" in j:
         if j["sfinish"] is True:
           self.__scenario_status = ScenarioStates.UNUSED
       return j
 
   def wait(self, buffer_size: int = 8192) -> Optional[str]:
     "TBD"
```

### Comparing `jeff_api-1.2.5/src/jeff_api/extension.py` & `jeff_api-1.2.6/src/jeff_api/extension.py`

 * *Files identical despite different names*

### Comparing `jeff_api-1.2.5/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.2.6/src/jeff_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

