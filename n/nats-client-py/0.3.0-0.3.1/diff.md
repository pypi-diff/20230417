# Comparing `tmp/nats-client-py-0.3.0.tar.gz` & `tmp/nats-client-py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats-client-py-0.3.0.tar", last modified: Sun Apr 16 15:32:41 2023, max compression
+gzip compressed data, was "nats-client-py-0.3.1.tar", last modified: Mon Apr 17 15:34:25 2023, max compression
```

## Comparing `nats-client-py-0.3.0.tar` & `nats-client-py-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:32:41.603184 nats-client-py-0.3.0/
--rw-rw-rw-   0        0        0       61 2023-04-16 15:32:41.602223 nats-client-py-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4673 2023-04-16 15:26:53.000000 nats-client-py-0.3.0/client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:32:41.602223 nats-client-py-0.3.0/nats_client_py.egg-info/
--rw-rw-rw-   0        0        0       61 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:32:41.603184 nats-client-py-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      208 2023-04-16 15:31:57.000000 nats-client-py-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:34:25.491655 nats-client-py-0.3.1/
+-rw-rw-rw-   0        0        0       61 2023-04-17 15:34:25.480617 nats-client-py-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4864 2023-04-17 15:34:10.000000 nats-client-py-0.3.1/client.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:34:25.479648 nats-client-py-0.3.1/nats_client_py.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-04-17 15:34:25.000000 nats-client-py-0.3.1/nats_client_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-04-17 15:34:25.000000 nats-client-py-0.3.1/nats_client_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:34:25.000000 nats-client-py-0.3.1/nats_client_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 15:34:25.000000 nats-client-py-0.3.1/nats_client_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:34:25.491655 nats-client-py-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      208 2023-04-17 15:31:13.000000 nats-client-py-0.3.1/setup.py
```

### Comparing `nats-client-py-0.3.0/client.py` & `nats-client-py-0.3.1/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,30 +56,35 @@
     async def closed_cb(self):
         print('Connection to NATS is closed.')
         self.is_done.set_result(True)
 
     def emit(self):
         ctx = self
 
-        async def emit_handle(topic, payload):
+        async def emit_handle(topic, payload, timeout=10000):
             try:
                 ctx.server_is_live()
                 m = await ctx.nc.request(
                     subject=topic,
-                    payload=encode_json(payload=payload)
+                    payload=encode_json(payload=payload),
+                    timeout=timeout
                 )
                 response = decode_json(m.data)
                 if not response['ok']:
                     raise Exception(response['message'])
                 return response
             except Exception as e:
                 raise e
 
         return emit_handle
 
+    async def call(self, topic, payload, timeout=10000):
+        res = await self.emit()(topic, payload, timeout)
+        return res
+
     def server_is_live(self):
         if not self.nc.is_connected:
             self.closed_cb()
 
     async def create_service(self, version, name, workers=1, actions: typing.List[ActionSchema] = []):
         self.server_is_live()
```

