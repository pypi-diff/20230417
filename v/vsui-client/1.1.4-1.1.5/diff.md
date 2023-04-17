# Comparing `tmp/vsui_client-1.1.4.tar.gz` & `tmp/vsui_client-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-1.1.4.tar", max compression
+gzip compressed data, was "vsui_client-1.1.5.tar", max compression
```

## Comparing `vsui_client-1.1.4.tar` & `vsui_client-1.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3880 2023-04-14 11:42:57.282794 vsui_client-1.1.4/README.md
--rw-r--r--   0        0        0      887 2023-04-17 09:29:17.396500 vsui_client-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      157 2023-04-13 14:15:11.923134 vsui_client-1.1.4/vsui_client/__init__.py
--rw-r--r--   0        0        0       92 2023-04-13 14:13:57.331155 vsui_client-1.1.4/vsui_client/_log.py
--rw-r--r--   0        0        0      946 2023-04-17 09:28:11.931488 vsui_client-1.1.4/vsui_client/_main.py
--rw-r--r--   0        0        0     5519 2023-04-17 09:29:01.652675 vsui_client-1.1.4/vsui_client/_oo_interface.py
--rw-r--r--   0        0        0     4060 2023-04-14 08:21:12.200729 vsui_client-1.1.4/vsui_client/_vsui_client.py
--rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 vsui_client-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3880 2023-04-14 11:42:57.282794 vsui_client-1.1.5/README.md
+-rw-r--r--   0        0        0      887 2023-04-17 09:59:13.493390 vsui_client-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-04-13 14:15:11.923134 vsui_client-1.1.5/vsui_client/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-13 14:13:57.331155 vsui_client-1.1.5/vsui_client/_log.py
+-rw-r--r--   0        0        0      982 2023-04-17 09:43:07.707763 vsui_client-1.1.5/vsui_client/_main.py
+-rw-r--r--   0        0        0     5519 2023-04-17 09:29:01.652675 vsui_client-1.1.5/vsui_client/_oo_interface.py
+-rw-r--r--   0        0        0     4060 2023-04-14 08:21:12.200729 vsui_client-1.1.5/vsui_client/_vsui_client.py
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 vsui_client-1.1.5/PKG-INFO
```

### Comparing `vsui_client-1.1.4/README.md` & `vsui_client-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.4/pyproject.toml` & `vsui_client-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vsui-client"
-version = "1.1.4"
+version = "1.1.5"
 description = "Client module for connecting to Volume Segmantics User Inteface"
 authors = ["Matthew Pimblott <matthew.pimblott@diamond.ac.uk>"]
 readme = "README.md"
 packages = [{include = "vsui_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `vsui_client-1.1.4/vsui_client/_main.py` & `vsui_client-1.1.5/vsui_client/_main.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 client = None
 
 def get_client() -> _oo_interface.VSUIClient:
     ''' return the current vsui client instance
     Returns:
         _oo_interface.VSUIClient: the client instance
     '''
+    global client
     if client is None:
         raise Exception('vsui client not initialized')
     return client
 
 def init_vsui(enabled: bool, task_id: str = None, logging_target: str = None) -> _oo_interface.VSUIClient:
     ''' initialize the vsui client
     Args:
         enabled (bool): whether vsui is enabled
         task_id (str): the id of the task
         logging_target (str): the key of the logging target
     Returns:
         _oo_interface.VSUIClient: the client instance
     '''
+    global client
     if enabled:
         client = _oo_interface.VSUIEnabled()
     else:
         client = _oo_interface.VSUIDisabled()
     # set task id and logging target
     client.set_task_id(task_id)
     client.set_logging_target(logging_target)
```

### Comparing `vsui_client-1.1.4/vsui_client/_oo_interface.py` & `vsui_client-1.1.5/vsui_client/_oo_interface.py`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.4/vsui_client/_vsui_client.py` & `vsui_client-1.1.5/vsui_client/_vsui_client.py`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.4/PKG-INFO` & `vsui_client-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsui-client
-Version: 1.1.4
+Version: 1.1.5
 Summary: Client module for connecting to Volume Segmantics User Inteface
 Author: Matthew Pimblott
 Author-email: matthew.pimblott@diamond.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

