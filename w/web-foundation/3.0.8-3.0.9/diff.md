# Comparing `tmp/web_foundation-3.0.8.tar.gz` & `tmp/web_foundation-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_foundation-3.0.8.tar", max compression
+gzip compressed data, was "web_foundation-3.0.9.tar", max compression
```

## Comparing `web_foundation-3.0.8.tar` & `web_foundation-3.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.475807 web_foundation-3.0.8/README.md
--rw-r--r--   0        0        0     1317 2023-03-09 12:31:05.444703 web_foundation-3.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/__init__.py
--rw-r--r--   0        0        0     7203 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/app.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/cli.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/env/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/env/database/__init__.py
--rw-r--r--   0        0        0     5587 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/env/database/access.py
--rw-r--r--   0        0        0     4981 2023-03-09 11:47:34.889040 web_foundation-3.0.8/web/env/database/database.py
--rw-r--r--   0        0        0    10069 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/env/database/model_loader.py
--rw-r--r--   0        0        0     3082 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/env/database/models.py
--rw-r--r--   0        0        0     1757 2023-03-08 21:18:57.675850 web_foundation-3.0.8/web/env/database/utils.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/errors/__init__.py
--rw-r--r--   0        0        0     1186 2023-03-08 21:18:57.679850 web_foundation-3.0.8/web/errors/app.py
--rw-r--r--   0        0        0      299 2023-03-08 21:18:57.671850 web_foundation-3.0.8/web/errors/files.py
--rw-r--r--   0        0        0     6668 2023-03-08 21:18:57.667849 web_foundation-3.0.8/web/errors/http.py
--rw-r--r--   0        0        0       51 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/errors/metrics.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/messaging/__init__.py
--rw-r--r--   0        0        0     3415 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/messaging/channel.py
--rw-r--r--   0        0        0     3529 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/messaging/dispatcher.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/proc/__init__.py
--rw-r--r--   0        0        0     2775 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/proc/isolate.py
--rw-r--r--   0        0        0     1627 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/proc/manager.py
--rw-r--r--   0        0        0     7419 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/proc/scheduler.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/signal.py
--rw-r--r--   0        0        0     3373 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/kernel/transport.py
--rw-r--r--   0        0        0    26691 2023-03-09 12:11:49.906184 web_foundation-3.0.8/web/kernel/types.py
--rw-r--r--   0        0        0      779 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/sanic_test.py
--rw-r--r--   0        0        0      191 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/settings.py
--rw-r--r--   0        0        0     2120 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/test.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/__init__.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/grpc/__init__.py
--rw-r--r--   0        0        0      818 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/grpc/transport.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/rest/__init__.py
--rw-r--r--   0        0        0    14204 2023-03-09 12:31:05.440703 web_foundation-3.0.8/web/trend/rest/custom.py
--rw-r--r--   0        0        0     2031 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/rest/sse.py
--rw-r--r--   0        0        0     2325 2023-03-09 12:08:08.626588 web_foundation-3.0.8/web/trend/rest/transport.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/rest/utils/__init__.py
--rw-r--r--   0        0        0     8495 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/rest/utils/openapi.py
--rw-r--r--   0        0        0     2951 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/rest/utils/openapi_gen.py
--rw-r--r--   0        0        0     6766 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/rest/utils/openapi_spec.py
--rw-r--r--   0        0        0     1081 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/trend/rest/ws.py
--rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/utils/__init__.py
--rw-r--r--   0        0        0      979 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/utils/crypto.py
--rw-r--r--   0        0        0     2457 2023-03-09 10:50:45.173869 web_foundation-3.0.8/web/utils/helpers.py
--rw-r--r--   0        0        0     1284 2023-03-08 20:00:20.479807 web_foundation-3.0.8/web/utils/logger.py
--rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 web_foundation-3.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.475807 web_foundation-3.0.9/README.md
+-rw-r--r--   0        0        0     1317 2023-03-09 12:56:25.913514 web_foundation-3.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/__init__.py
+-rw-r--r--   0        0        0     7203 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/app.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/cli.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/env/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/env/database/__init__.py
+-rw-r--r--   0        0        0     5587 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/env/database/access.py
+-rw-r--r--   0        0        0     4981 2023-03-09 11:47:34.889040 web_foundation-3.0.9/web/env/database/database.py
+-rw-r--r--   0        0        0    10069 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/env/database/model_loader.py
+-rw-r--r--   0        0        0     3082 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/env/database/models.py
+-rw-r--r--   0        0        0     1757 2023-03-08 21:18:57.675850 web_foundation-3.0.9/web/env/database/utils.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/errors/__init__.py
+-rw-r--r--   0        0        0     1186 2023-03-08 21:18:57.679850 web_foundation-3.0.9/web/errors/app.py
+-rw-r--r--   0        0        0      299 2023-03-08 21:18:57.671850 web_foundation-3.0.9/web/errors/files.py
+-rw-r--r--   0        0        0     6668 2023-03-08 21:18:57.667849 web_foundation-3.0.9/web/errors/http.py
+-rw-r--r--   0        0        0       51 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/errors/metrics.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/messaging/__init__.py
+-rw-r--r--   0        0        0     3415 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/messaging/channel.py
+-rw-r--r--   0        0        0     3529 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/messaging/dispatcher.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/proc/__init__.py
+-rw-r--r--   0        0        0     2775 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/proc/isolate.py
+-rw-r--r--   0        0        0     1626 2023-03-09 12:39:26.916706 web_foundation-3.0.9/web/kernel/proc/manager.py
+-rw-r--r--   0        0        0     7419 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/proc/scheduler.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/signal.py
+-rw-r--r--   0        0        0     3373 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/kernel/transport.py
+-rw-r--r--   0        0        0    26784 2023-03-09 12:56:06.097062 web_foundation-3.0.9/web/kernel/types.py
+-rw-r--r--   0        0        0      779 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/sanic_test.py
+-rw-r--r--   0        0        0      191 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/settings.py
+-rw-r--r--   0        0        0     2120 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/test.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/grpc/__init__.py
+-rw-r--r--   0        0        0      818 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/grpc/transport.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/rest/__init__.py
+-rw-r--r--   0        0        0    14204 2023-03-09 12:31:05.440703 web_foundation-3.0.9/web/trend/rest/custom.py
+-rw-r--r--   0        0        0     2031 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/rest/sse.py
+-rw-r--r--   0        0        0     2325 2023-03-09 12:08:08.626588 web_foundation-3.0.9/web/trend/rest/transport.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/rest/utils/__init__.py
+-rw-r--r--   0        0        0     8495 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/rest/utils/openapi.py
+-rw-r--r--   0        0        0     2951 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/rest/utils/openapi_gen.py
+-rw-r--r--   0        0        0     6766 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/rest/utils/openapi_spec.py
+-rw-r--r--   0        0        0     1081 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/trend/rest/ws.py
+-rw-r--r--   0        0        0        0 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/utils/__init__.py
+-rw-r--r--   0        0        0      979 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/utils/crypto.py
+-rw-r--r--   0        0        0     2457 2023-03-09 10:50:45.173869 web_foundation-3.0.9/web/utils/helpers.py
+-rw-r--r--   0        0        0     1284 2023-03-08 20:00:20.479807 web_foundation-3.0.9/web/utils/logger.py
+-rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 web_foundation-3.0.9/PKG-INFO
```

### Comparing `web_foundation-3.0.8/pyproject.toml` & `web_foundation-3.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-foundation"
-version = "3.0.8"
+version = "3.0.9"
 description = "python web-server template"
 authors = ["yaroher <yaroher2442@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "web" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `web_foundation-3.0.8/web/app.py` & `web_foundation-3.0.9/web/app.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/env/database/access.py` & `web_foundation-3.0.9/web/env/database/access.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/env/database/database.py` & `web_foundation-3.0.9/web/env/database/database.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/env/database/model_loader.py` & `web_foundation-3.0.9/web/env/database/model_loader.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/env/database/models.py` & `web_foundation-3.0.9/web/env/database/models.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/env/database/utils.py` & `web_foundation-3.0.9/web/env/database/utils.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/errors/app.py` & `web_foundation-3.0.9/web/errors/app.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/errors/http.py` & `web_foundation-3.0.9/web/errors/http.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/kernel/messaging/channel.py` & `web_foundation-3.0.9/web/kernel/messaging/channel.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/kernel/messaging/dispatcher.py` & `web_foundation-3.0.9/web/kernel/messaging/dispatcher.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/kernel/proc/isolate.py` & `web_foundation-3.0.9/web/kernel/proc/isolate.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/kernel/proc/manager.py` & `web_foundation-3.0.9/web/kernel/proc/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     def add_isolate(self, isolate: Isolate, run: bool = False):
         self._add_isolate(isolate, run)
 
     def remove_isolate(self, name: str):
         self._isolates.pop(name)
 
     async def run(self):
-
         with self._manager as manager:
             ctx = multiprocessing.get_context("fork")
             for isolate in self._isolates.values():
                 isolate.fork(ctx)
 
     def stop(self):
         for i in self._isolates.values():
```

### Comparing `web_foundation-3.0.8/web/kernel/proc/scheduler.py` & `web_foundation-3.0.9/web/kernel/proc/scheduler.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/kernel/transport.py` & `web_foundation-3.0.9/web/kernel/transport.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/kernel/types.py` & `web_foundation-3.0.9/web/kernel/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,14 +635,15 @@
 
     def __init__(self, services: List[GenService]):
         EnvAble.__init__(self)
         self.services = services
         for service in self.services:
             service.transport = self
         self.rt_writers = {}
+        self._plugins_store = None
         self.plugins_dir = None
 
     def get_service(self, typed: Type[GenService]) -> GenService | None:
         for service in self.services:
             if isinstance(service, typed):
                 return service
 
@@ -683,14 +684,16 @@
         raise NotImplementedError
 
     async def run(self, sock: ISocket):
         raise NotImplementedError
 
     @property
     def plugins(self):
+        if not self._plugins_store:
+            return []
         return [container.plugin for container in self._plugins_store.local_store.values()]
 
 
 class Resource(AppNameAble, ConfAble, ChanAble, metaclass=ABCMeta):
     __communicator: GenCommunicator | None
 
     def __init__(self, communicator: GenCommunicator | None = None):
```

### Comparing `web_foundation-3.0.8/web/sanic_test.py` & `web_foundation-3.0.9/web/sanic_test.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/test.py` & `web_foundation-3.0.9/web/test.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/grpc/transport.py` & `web_foundation-3.0.9/web/trend/grpc/transport.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/rest/custom.py` & `web_foundation-3.0.9/web/trend/rest/custom.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/rest/sse.py` & `web_foundation-3.0.9/web/trend/rest/sse.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/rest/transport.py` & `web_foundation-3.0.9/web/trend/rest/transport.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/rest/utils/openapi.py` & `web_foundation-3.0.9/web/trend/rest/utils/openapi.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/rest/utils/openapi_gen.py` & `web_foundation-3.0.9/web/trend/rest/utils/openapi_gen.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/rest/utils/openapi_spec.py` & `web_foundation-3.0.9/web/trend/rest/utils/openapi_spec.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/trend/rest/ws.py` & `web_foundation-3.0.9/web/trend/rest/ws.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/utils/crypto.py` & `web_foundation-3.0.9/web/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/utils/helpers.py` & `web_foundation-3.0.9/web/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/web/utils/logger.py` & `web_foundation-3.0.9/web/utils/logger.py`

 * *Files identical despite different names*

### Comparing `web_foundation-3.0.8/PKG-INFO` & `web_foundation-3.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-foundation
-Version: 3.0.8
+Version: 3.0.9
 Summary: python web-server template
 Author: yaroher
 Author-email: yaroher2442@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

