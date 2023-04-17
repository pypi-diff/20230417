# Comparing `tmp/vsui_client-1.1.2.tar.gz` & `tmp/vsui_client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsui_client-1.1.2.tar", max compression
+gzip compressed data, was "vsui_client-1.1.3.tar", max compression
```

## Comparing `vsui_client-1.1.2.tar` & `vsui_client-1.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1308 2023-04-11 12:01:56.729566 vsui_client-1.1.2/README.md
--rw-r--r--   0        0        0      887 2023-04-13 13:47:24.971386 vsui_client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      249 2023-04-13 13:43:11.106253 vsui_client-1.1.2/vsui_client/__init__.py
--rw-r--r--   0        0        0      917 2023-04-13 13:50:27.784220 vsui_client-1.1.2/vsui_client/_main.py
--rw-r--r--   0        0        0     3975 2023-04-13 13:50:00.720258 vsui_client-1.1.2/vsui_client/_oo_interface.py
--rw-r--r--   0        0        0     3939 2023-04-13 13:45:59.194231 vsui_client-1.1.2/vsui_client/_vsui_client.py
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 vsui_client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3880 2023-04-14 11:42:57.282794 vsui_client-1.1.3/README.md
+-rw-r--r--   0        0        0      887 2023-04-17 08:50:35.764632 vsui_client-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-04-13 14:15:11.923134 vsui_client-1.1.3/vsui_client/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-13 14:13:57.331155 vsui_client-1.1.3/vsui_client/_log.py
+-rw-r--r--   0        0        0      917 2023-04-13 13:50:27.784220 vsui_client-1.1.3/vsui_client/_main.py
+-rw-r--r--   0        0        0     5522 2023-04-14 10:52:31.733087 vsui_client-1.1.3/vsui_client/_oo_interface.py
+-rw-r--r--   0        0        0     4060 2023-04-14 08:21:12.200729 vsui_client-1.1.3/vsui_client/_vsui_client.py
+-rw-r--r--   0        0        0     4447 1970-01-01 00:00:00.000000 vsui_client-1.1.3/PKG-INFO
```

### Comparing `vsui_client-1.1.2/pyproject.toml` & `vsui_client-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vsui-client"
-version = "1.1.2"
+version = "1.1.3"
 description = "Client module for connecting to Volume Segmantics User Inteface"
 authors = ["Matthew Pimblott <matthew.pimblott@diamond.ac.uk>"]
 readme = "README.md"
 packages = [{include = "vsui_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `vsui_client-1.1.2/vsui_client/_main.py` & `vsui_client-1.1.3/vsui_client/_main.py`

 * *Files identical despite different names*

### Comparing `vsui_client-1.1.2/vsui_client/_vsui_client.py` & `vsui_client-1.1.3/vsui_client/_vsui_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 import logging
 from matplotlib import pyplot as plt
 import io
 import sys
 import base64
 import time
 
-from vsui_client import _vsui_logger
+from vsui_client._log import _vsui_logger
 
 sio = socketio.Client()
 task_id = None
 # target log for where intercepted logs should be forwarded to
 logging_target = None
 timeout_count = 0
 
 # https://stackoverflow.com/a/51981833
 def vsui_process() -> Callable:
     ''' Decorator for functions that should be run as a vsui task 
         This decorator will catch any exceptions and send a message to the server
         returns the decorator
     '''
-    def decorator(func) -> Callable:
+    def decorator(func) -> Any:
         def wrapper(*args, **kwargs):
             _vsui_logger.info(f'running {func.__name__} as vsui process')
             r = None
             try:
                 r = func(*args, **kwargs)
             except (SystemExit, Exception) as e:
                 _vsui_logger.exception(f'exception caught: {e}')
                 safe_emit('exception', {'task_id' : task_id, 'exception' : str(e)})
                 r = disconnect()
-                time.sleep(1)
-                sys.exit(1)
+                # print to the standart error stream
+                print(f'process {func.__name__} failed, exception: {e}', file=sys.stderr)
+                raise SystemExit(1)
             finally:
                 _vsui_logger.info(f'finished running {func.__name__} as vsui process')
                 return r
         return wrapper
     return decorator
 
 def safe_emit(event, data):
```

