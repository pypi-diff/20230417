# Comparing `tmp/vsui_client-1.1.3.tar.gz` & `tmp/vsui_client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-1.1.3.tar", max compression
+gzip compressed data, was "vsui_client-1.1.4.tar", max compression
```

## Comparing `vsui_client-1.1.3.tar` & `vsui_client-1.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3880 2023-04-14 11:42:57.282794 vsui_client-1.1.3/README.md
--rw-r--r--   0        0        0      887 2023-04-17 08:50:35.764632 vsui_client-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      157 2023-04-13 14:15:11.923134 vsui_client-1.1.3/vsui_client/__init__.py
--rw-r--r--   0        0        0       92 2023-04-13 14:13:57.331155 vsui_client-1.1.3/vsui_client/_log.py
--rw-r--r--   0        0        0      917 2023-04-13 13:50:27.784220 vsui_client-1.1.3/vsui_client/_main.py
--rw-r--r--   0        0        0     5522 2023-04-14 10:52:31.733087 vsui_client-1.1.3/vsui_client/_oo_interface.py
--rw-r--r--   0        0        0     4060 2023-04-14 08:21:12.200729 vsui_client-1.1.3/vsui_client/_vsui_client.py
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 vsui_client-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3880 2023-04-14 11:42:57.282794 vsui_client-1.1.4/README.md
+-rw-r--r--   0        0        0      887 2023-04-17 09:29:17.396500 vsui_client-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-04-13 14:15:11.923134 vsui_client-1.1.4/vsui_client/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-13 14:13:57.331155 vsui_client-1.1.4/vsui_client/_log.py
+-rw-r--r--   0        0        0      946 2023-04-17 09:28:11.931488 vsui_client-1.1.4/vsui_client/_main.py
+-rw-r--r--   0        0        0     5519 2023-04-17 09:29:01.652675 vsui_client-1.1.4/vsui_client/_oo_interface.py
+-rw-r--r--   0        0        0     4060 2023-04-14 08:21:12.200729 vsui_client-1.1.4/vsui_client/_vsui_client.py
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 vsui_client-1.1.4/PKG-INFO
```

### Comparing `vsui_client-1.1.3/README.md` & `vsui_client-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.3/pyproject.toml` & `vsui_client-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vsui-client"
-version = "1.1.3"
+version = "1.1.4"
 description = "Client module for connecting to Volume Segmantics User Inteface"
 authors = ["Matthew Pimblott <matthew.pimblott@diamond.ac.uk>"]
 readme = "README.md"
 packages = [{include = "vsui_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `vsui_client-1.1.3/vsui_client/_main.py` & `vsui_client-1.1.4/vsui_client/_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,10 +20,11 @@
     Returns:
         _oo_interface.VSUIClient: the client instance
     '''
     if enabled:
         client = _oo_interface.VSUIEnabled()
     else:
         client = _oo_interface.VSUIDisabled()
-        client.set_task_id(task_id)
-        client.set_logging_target(logging_target)
+    # set task id and logging target
+    client.set_task_id(task_id)
+    client.set_logging_target(logging_target)
     return client
```

### Comparing `vsui_client-1.1.3/vsui_client/_oo_interface.py` & `vsui_client-1.1.4/vsui_client/_oo_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             format=format,
             figsize=figsize,
             cmap=cmap
         )
     
     def get_handler(self) -> logging.Handler:
         ''' Provides access to the logging handler singleton.'''
-        if self.get_handler is None:
+        if self._handler is None:
             self._handler = _vsui_client.RequestHandler()
         return self._handler
 
 class VSUIDisabled():
     ''' OO interface for vsui client, when vsui is disabled '''
     def connect(self, host : str = 'localhost', port : str = '8000') -> None:
         ''' do nothing - not in UI mode '''
```

### Comparing `vsui_client-1.1.3/vsui_client/_vsui_client.py` & `vsui_client-1.1.4/vsui_client/_vsui_client.py`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.3/PKG-INFO` & `vsui_client-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsui-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: Client module for connecting to Volume Segmantics User Inteface
 Author: Matthew Pimblott
 Author-email: matthew.pimblott@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

