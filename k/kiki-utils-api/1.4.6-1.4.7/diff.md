# Comparing `tmp/kiki_utils_api-1.4.6.tar.gz` & `tmp/kiki_utils_api-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiki_utils_api-1.4.6.tar", last modified: Wed Mar 22 08:17:42 2023, max compression
+gzip compressed data, was "kiki_utils_api-1.4.7.tar", last modified: Mon Apr 17 10:09:29 2023, max compression
```

## Comparing `kiki_utils_api-1.4.6.tar` & `kiki_utils_api-1.4.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-03-22 08:17:42.888477 kiki_utils_api-1.4.6/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.6/LICENSE.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      266 2023-03-22 08:17:42.888477 kiki_utils_api-1.4.6/PKG-INFO
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.6/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-03-22 08:17:42.884477 kiki_utils_api-1.4.6/kiki_utils_api.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      266 2023-03-22 08:17:42.000000 kiki_utils_api-1.4.6/kiki_utils_api.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      657 2023-03-22 08:17:42.000000 kiki_utils_api-1.4.6/kiki_utils_api.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-03-22 08:17:42.000000 kiki_utils_api-1.4.6/kiki_utils_api.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       40 2023-03-22 08:17:42.000000 kiki_utils_api-1.4.6/kiki_utils_api.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       14 2023-03-22 08:17:42.000000 kiki_utils_api-1.4.6/kiki_utils_api.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-03-22 08:17:42.000000 kiki_utils_api-1.4.6/kiki_utils_api.egg-info/zip-safe
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-03-22 08:17:42.884477 kiki_utils_api-1.4.6/kikiutils_api/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.6/kikiutils_api/__init__.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-03-22 08:17:42.884477 kiki_utils_api-1.4.6/kikiutils_api/classes/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     4876 2023-03-22 08:16:04.000000 kiki_utils_api-1.4.6/kikiutils_api/classes/__init__.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      796 2023-01-06 04:19:49.000000 kiki_utils_api-1.4.6/kikiutils_api/classes/blacksheep.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      701 2023-01-06 04:15:46.000000 kiki_utils_api-1.4.6/kikiutils_api/classes/sanic.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     2601 2023-01-04 08:24:42.000000 kiki_utils_api-1.4.6/kikiutils_api/classes/transmission.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     3868 2023-03-22 08:15:02.000000 kiki_utils_api-1.4.6/kikiutils_api/classes/websocket.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-03-22 08:17:42.884477 kiki_utils_api-1.4.6/kikiutils_api/decorators/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.6/kikiutils_api/decorators/__init__.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1593 2023-01-06 05:46:57.000000 kiki_utils_api-1.4.6/kikiutils_api/decorators/blacksheep.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     3433 2023-01-06 05:44:11.000000 kiki_utils_api-1.4.6/kikiutils_api/decorators/sanic.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-03-22 08:17:42.888477 kiki_utils_api-1.4.6/kikiutils_api/utils/
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1634 2023-01-06 05:48:36.000000 kiki_utils_api-1.4.6/kikiutils_api/utils/__init__.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      989 2022-12-30 18:34:06.000000 kiki_utils_api-1.4.6/kikiutils_api/utils/blacksheep.py
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      569 2022-12-21 05:28:38.000000 kiki_utils_api-1.4.6/kikiutils_api/utils/sanic.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-03-22 08:17:42.888477 kiki_utils_api-1.4.6/setup.cfg
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      525 2023-03-22 08:17:05.000000 kiki_utils_api-1.4.6/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1066 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.7/LICENSE.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      266 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/PKG-INFO
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.7/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/kiki_utils_api.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      266 2023-04-17 10:09:29.000000 kiki_utils_api-1.4.7/kiki_utils_api.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      657 2023-04-17 10:09:29.000000 kiki_utils_api-1.4.7/kiki_utils_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-04-17 10:09:29.000000 kiki_utils_api-1.4.7/kiki_utils_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       40 2023-04-17 10:09:29.000000 kiki_utils_api-1.4.7/kiki_utils_api.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       14 2023-04-17 10:09:29.000000 kiki_utils_api-1.4.7/kiki_utils_api.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-04-17 10:09:29.000000 kiki_utils_api-1.4.7/kiki_utils_api.egg-info/zip-safe
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/kikiutils_api/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.7/kikiutils_api/__init__.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/kikiutils_api/classes/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     4876 2023-03-22 08:16:04.000000 kiki_utils_api-1.4.7/kikiutils_api/classes/__init__.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      796 2023-01-06 04:19:49.000000 kiki_utils_api-1.4.7/kikiutils_api/classes/blacksheep.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      701 2023-01-06 04:15:46.000000 kiki_utils_api-1.4.7/kikiutils_api/classes/sanic.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     2601 2023-01-04 08:24:42.000000 kiki_utils_api-1.4.7/kikiutils_api/classes/transmission.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4038 2023-04-17 10:05:37.000000 kiki_utils_api-1.4.7/kikiutils_api/classes/websocket.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/kikiutils_api/decorators/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2022-11-28 10:23:50.000000 kiki_utils_api-1.4.7/kikiutils_api/decorators/__init__.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1579 2023-04-17 10:08:39.000000 kiki_utils_api-1.4.7/kikiutils_api/decorators/blacksheep.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     3433 2023-01-06 05:44:11.000000 kiki_utils_api-1.4.7/kikiutils_api/decorators/sanic.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/kikiutils_api/utils/
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)     1634 2023-01-06 05:48:36.000000 kiki_utils_api-1.4.7/kikiutils_api/utils/__init__.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      989 2022-12-30 18:34:06.000000 kiki_utils_api-1.4.7/kikiutils_api/utils/blacksheep.py
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      569 2022-12-21 05:28:38.000000 kiki_utils_api-1.4.7/kikiutils_api/utils/sanic.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-04-17 10:09:29.200352 kiki_utils_api-1.4.7/setup.cfg
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      525 2023-04-17 10:09:17.000000 kiki_utils_api-1.4.7/setup.py
```

### Comparing `kiki_utils_api-1.4.6/LICENSE.txt` & `kiki_utils_api-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kiki_utils_api.egg-info/SOURCES.txt` & `kiki_utils_api-1.4.7/kiki_utils_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/classes/__init__.py` & `kiki_utils_api-1.4.7/kikiutils_api/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/classes/blacksheep.py` & `kiki_utils_api-1.4.7/kikiutils_api/classes/blacksheep.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/classes/sanic.py` & `kiki_utils_api-1.4.7/kikiutils_api/classes/sanic.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/classes/transmission.py` & `kiki_utils_api-1.4.7/kikiutils_api/classes/transmission.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/classes/websocket.py` & `kiki_utils_api-1.4.7/kikiutils_api/classes/websocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,38 +5,41 @@
 from typing import Callable, Coroutine, Optional
 from uuid import uuid1
 from websockets.legacy.client import Connect
 
 
 class WebsocketClient:
     _check_task: Task
+    _emit_raise_exception: bool
     _listen_task: Task
     code: str
     loop: AbstractEventLoop = None
 
     def __init__(
         self,
         aes: AesCrypt,
         name: str,
         url: str,
         check_interval: int = 3,
-        headers: dict = {}
+        headers: dict = {},
+        emit_raise_exception: bool = False
     ):
         self.aes = aes
         self.check_interval = check_interval
         self.code = random_str()
         self.connect_kwargs = {
             'extra_headers': {
                 'extra-info': aes.encrypt(headers)
             },
             'ping_interval': None,
             'uri': url
         }
 
         self.disconnecting = False
+        self._emit_raise_exception = emit_raise_exception
         self.event_handlers: dict[str, Callable[..., Coroutine]] = {}
         self.name = name
         self.waiting_events: dict[str, dict[str, Future]] = {}
 
     async def _check(self):
         try:
             await sleep(self.check_interval)
@@ -78,23 +81,25 @@
         self.disconnecting = True
         self._check_task.cancel()
         self._listen_task.cancel()
         await self.ws.close()
         self.disconnecting = False
 
     async def emit(self, event: str, *args, **kwargs):
-        await self.ws.send(self.aes.encrypt([event, args, kwargs]))
+        if self._emit_raise_exception:
+            await self.ws.send(self.aes.encrypt([event, args, kwargs]))
+        else:
+            try:
+                await self.ws.send(self.aes.encrypt([event, args, kwargs]))
+            except:
+                return False
 
-    async def emit_and_wait_event(
-        self,
-        event: str,
-        wait_event: str,
-        *args,
-        **kwargs
-    ):
+        return True
+
+    async def emit_and_wait_event(self, event: str, wait_event: str, *args, **kwargs):
         uuid = uuid1().hex
         kwargs['__wait_event_uuid'] = uuid
 
         if wait_event in self.waiting_events:
             self.waiting_events[wait_event][uuid] = Future()
         else:
             self.waiting_events[wait_event] = {uuid: Future()}
@@ -102,19 +107,16 @@
         await self.emit(event, *args, **kwargs)
         return await self.waiting_events[wait_event][uuid]
 
     def on(self, event: str):
         """Register event handler."""
 
         def decorator(view_func):
-            @wraps(view_func)
-            async def wrapped_view(*args, **kwargs):
-                await view_func(*args, **kwargs)
-            self.event_handlers[event] = wrapped_view
-            return wrapped_view
+            self.event_handlers[event] = view_func
+            return view_func
         return decorator
 
     async def wait_connect_success(self):
         """Wait for connect success."""
 
         while not self.disconnecting:
             try:
```

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/decorators/blacksheep.py` & `kiki_utils_api-1.4.7/kikiutils_api/decorators/blacksheep.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 from kikiutils.aes import AesCrypt
 
 from ..classes.transmission import DataTransmission
 from ..utils import data_transmission_exec, get_func_annotation_index
 from ..utils.blacksheep import get_file, get_rq, get_ws
 
 
-def data_transmission_api(
-    *secret_classes: DataTransmission,
-    parse_json: bool = True,
-    kwarg_name: str = 'data'
-):
+def data_transmission_api(*secret_classes: DataTransmission, parse_json: bool = True, kwarg_name: str = 'data'):
     def decorator(view_func):
         rq_index = get_func_annotation_index(view_func, Request)
 
         @wraps(view_func)
         async def wrapped_view(*args):
             if (hash_file := await get_file(args[rq_index], 'hash_file')) is None:
                 return not_found()
```

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/decorators/sanic.py` & `kiki_utils_api-1.4.7/kikiutils_api/decorators/sanic.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/utils/__init__.py` & `kiki_utils_api-1.4.7/kikiutils_api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/utils/blacksheep.py` & `kiki_utils_api-1.4.7/kikiutils_api/utils/blacksheep.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/kikiutils_api/utils/sanic.py` & `kiki_utils_api-1.4.7/kikiutils_api/utils/sanic.py`

 * *Files identical despite different names*

### Comparing `kiki_utils_api-1.4.6/setup.py` & `kiki_utils_api-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     name='kiki_utils_api',
     classifiers=[
         'License :: Freely Distributable'
     ],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=True,
-    version='1.4.6',
+    version='1.4.7',
     description='Utils functions with api data process.',
     author='kiki-kanri',
     author_email='a470666@gmail.com',
     keywords=['Utils'],
     install_requires=[
         'aiohttp[speedups]',
         'kiki-utils',
```

