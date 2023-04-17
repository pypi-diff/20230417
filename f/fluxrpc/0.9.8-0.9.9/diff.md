# Comparing `tmp/fluxrpc-0.9.8.tar.gz` & `tmp/fluxrpc-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxrpc-0.9.8.tar", max compression
+gzip compressed data, was "fluxrpc-0.9.9.tar", max compression
```

## Comparing `fluxrpc-0.9.8.tar` & `fluxrpc-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1089 2023-01-06 18:25:02.187887 fluxrpc-0.9.8/LICENSE
--rw-r--r--   0        0        0      113 2023-01-06 18:25:01.799405 fluxrpc-0.9.8/fluxrpc/__init__.py
--rw-r--r--   0        0        0     2455 2023-03-13 02:22:33.113243 fluxrpc-0.9.8/fluxrpc/auth/__init__.py
--rw-r--r--   0        0        0     7233 2023-02-12 23:08:04.165303 fluxrpc-0.9.8/fluxrpc/client.py
--rw-r--r--   0        0        0    12091 2023-02-12 23:08:45.569214 fluxrpc-0.9.8/fluxrpc/dispatch/__init__.py
--rw-r--r--   0        0        0     1649 2023-01-06 18:25:02.035298 fluxrpc-0.9.8/fluxrpc/exc.py
--rw-r--r--   0        0        0       51 2023-01-27 06:42:57.218099 fluxrpc-0.9.8/fluxrpc/log.py
--rw-r--r--   0        0        0    11745 2023-01-27 06:39:48.275005 fluxrpc-0.9.8/fluxrpc/protocols/__init__.py
--rw-r--r--   0        0        0    26364 2023-02-12 23:08:45.628987 fluxrpc-0.9.8/fluxrpc/protocols/jsonrpc.py
--rw-r--r--   0        0        0    15270 2023-02-12 23:08:45.633432 fluxrpc-0.9.8/fluxrpc/protocols/msgpackrpc.py
--rw-r--r--   0        0        0     4621 2023-02-12 23:08:45.617516 fluxrpc-0.9.8/fluxrpc/server/__init__.py
--rw-r--r--   0        0        0     1109 2023-01-06 18:25:01.844338 fluxrpc-0.9.8/fluxrpc/server/gevent.py
--rw-r--r--   0        0        0     3506 2023-01-06 18:25:01.485079 fluxrpc-0.9.8/fluxrpc/transports/__init__.py
--rw-r--r--   0        0        0     2001 2023-01-06 18:25:01.427484 fluxrpc-0.9.8/fluxrpc/transports/callback.py
--rw-r--r--   0        0        0     2388 2023-01-06 18:25:01.474261 fluxrpc-0.9.8/fluxrpc/transports/cgi.py
--rw-r--r--   0        0        0     1516 2023-01-06 18:25:01.514996 fluxrpc-0.9.8/fluxrpc/transports/http.py
--rw-r--r--   0        0        0     4851 2023-01-06 18:25:01.512484 fluxrpc-0.9.8/fluxrpc/transports/rabbitmq.py
--rw-r--r--   0        0        0    23310 2023-02-14 00:37:17.797263 fluxrpc-0.9.8/fluxrpc/transports/socket/client.py
--rw-r--r--   0        0        0     3762 2023-02-12 23:08:04.226266 fluxrpc-0.9.8/fluxrpc/transports/socket/messages.py
--rw-r--r--   0        0        0    23519 2023-03-18 19:42:10.122478 fluxrpc-0.9.8/fluxrpc/transports/socket/server.py
--rw-r--r--   0        0        0      199 2023-01-06 22:04:17.290124 fluxrpc-0.9.8/fluxrpc/transports/socket/symbols.py
--rw-r--r--   0        0        0     3197 2023-01-06 18:25:01.798353 fluxrpc-0.9.8/fluxrpc/transports/websocket.py
--rw-r--r--   0        0        0     1453 2023-01-06 18:25:01.514011 fluxrpc-0.9.8/fluxrpc/transports/websocketclient.py
--rw-r--r--   0        0        0     3402 2023-01-06 18:25:01.798785 fluxrpc-0.9.8/fluxrpc/transports/wsgi.py
--rw-r--r--   0        0        0     3466 2023-01-06 18:25:01.511109 fluxrpc-0.9.8/fluxrpc/transports/zmq.py
--rw-r--r--   0        0        0     1397 2023-03-18 19:42:58.882070 fluxrpc-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 fluxrpc-0.9.8/setup.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 fluxrpc-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-01-06 18:25:02.187887 fluxrpc-0.9.9/LICENSE
+-rw-r--r--   0        0        0      113 2023-01-06 18:25:01.799405 fluxrpc-0.9.9/fluxrpc/__init__.py
+-rw-r--r--   0        0        0     2455 2023-03-13 02:22:33.113243 fluxrpc-0.9.9/fluxrpc/auth/__init__.py
+-rw-r--r--   0        0        0     7233 2023-02-12 23:08:04.165303 fluxrpc-0.9.9/fluxrpc/client.py
+-rw-r--r--   0        0        0    12091 2023-02-12 23:08:45.569214 fluxrpc-0.9.9/fluxrpc/dispatch/__init__.py
+-rw-r--r--   0        0        0     1649 2023-01-06 18:25:02.035298 fluxrpc-0.9.9/fluxrpc/exc.py
+-rw-r--r--   0        0        0       51 2023-01-27 06:42:57.218099 fluxrpc-0.9.9/fluxrpc/log.py
+-rw-r--r--   0        0        0    11745 2023-01-27 06:39:48.275005 fluxrpc-0.9.9/fluxrpc/protocols/__init__.py
+-rw-r--r--   0        0        0    26364 2023-02-12 23:08:45.628987 fluxrpc-0.9.9/fluxrpc/protocols/jsonrpc.py
+-rw-r--r--   0        0        0    15270 2023-02-12 23:08:45.633432 fluxrpc-0.9.9/fluxrpc/protocols/msgpackrpc.py
+-rw-r--r--   0        0        0     4621 2023-02-12 23:08:45.617516 fluxrpc-0.9.9/fluxrpc/server/__init__.py
+-rw-r--r--   0        0        0     1109 2023-01-06 18:25:01.844338 fluxrpc-0.9.9/fluxrpc/server/gevent.py
+-rw-r--r--   0        0        0     3506 2023-01-06 18:25:01.485079 fluxrpc-0.9.9/fluxrpc/transports/__init__.py
+-rw-r--r--   0        0        0     2001 2023-01-06 18:25:01.427484 fluxrpc-0.9.9/fluxrpc/transports/callback.py
+-rw-r--r--   0        0        0     2388 2023-01-06 18:25:01.474261 fluxrpc-0.9.9/fluxrpc/transports/cgi.py
+-rw-r--r--   0        0        0     1516 2023-01-06 18:25:01.514996 fluxrpc-0.9.9/fluxrpc/transports/http.py
+-rw-r--r--   0        0        0     4851 2023-01-06 18:25:01.512484 fluxrpc-0.9.9/fluxrpc/transports/rabbitmq.py
+-rw-r--r--   0        0        0    23561 2023-03-24 19:12:20.667663 fluxrpc-0.9.9/fluxrpc/transports/socket/client.py
+-rw-r--r--   0        0        0     3762 2023-02-12 23:08:04.226266 fluxrpc-0.9.9/fluxrpc/transports/socket/messages.py
+-rw-r--r--   0        0        0    23519 2023-03-18 19:42:10.122478 fluxrpc-0.9.9/fluxrpc/transports/socket/server.py
+-rw-r--r--   0        0        0      199 2023-01-06 22:04:17.290124 fluxrpc-0.9.9/fluxrpc/transports/socket/symbols.py
+-rw-r--r--   0        0        0     3197 2023-01-06 18:25:01.798353 fluxrpc-0.9.9/fluxrpc/transports/websocket.py
+-rw-r--r--   0        0        0     1453 2023-01-06 18:25:01.514011 fluxrpc-0.9.9/fluxrpc/transports/websocketclient.py
+-rw-r--r--   0        0        0     3402 2023-01-06 18:25:01.798785 fluxrpc-0.9.9/fluxrpc/transports/wsgi.py
+-rw-r--r--   0        0        0     3466 2023-01-06 18:25:01.511109 fluxrpc-0.9.9/fluxrpc/transports/zmq.py
+-rw-r--r--   0        0        0     1398 2023-03-24 19:12:46.188309 fluxrpc-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 fluxrpc-0.9.9/setup.py
+-rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 fluxrpc-0.9.9/PKG-INFO
```

### Comparing `fluxrpc-0.9.8/LICENSE` & `fluxrpc-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/auth/__init__.py` & `fluxrpc-0.9.9/fluxrpc/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/client.py` & `fluxrpc-0.9.9/fluxrpc/client.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/dispatch/__init__.py` & `fluxrpc-0.9.9/fluxrpc/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/exc.py` & `fluxrpc-0.9.9/fluxrpc/exc.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/protocols/__init__.py` & `fluxrpc-0.9.9/fluxrpc/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/protocols/jsonrpc.py` & `fluxrpc-0.9.9/fluxrpc/protocols/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/protocols/msgpackrpc.py` & `fluxrpc-0.9.9/fluxrpc/protocols/msgpackrpc.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/server/__init__.py` & `fluxrpc-0.9.9/fluxrpc/server/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/server/gevent.py` & `fluxrpc-0.9.9/fluxrpc/server/gevent.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/__init__.py` & `fluxrpc-0.9.9/fluxrpc/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/callback.py` & `fluxrpc-0.9.9/fluxrpc/transports/callback.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/cgi.py` & `fluxrpc-0.9.9/fluxrpc/transports/cgi.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/http.py` & `fluxrpc-0.9.9/fluxrpc/transports/http.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/rabbitmq.py` & `fluxrpc-0.9.9/fluxrpc/transports/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/socket/client.py` & `fluxrpc-0.9.9/fluxrpc/transports/socket/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         await self.challenge_complete_event.wait()
         self.challenge_complete_event.clear()
 
         self.channels += 1
 
         if self.auth_required and not self.auth_provider:
             self.auth_error = "Auth required and no auth provider set"
-            log.error(self.auth_error)
+            log.warning(self.auth_error)
             await self.disconnect()
             self._connecting = False
             return
 
         if self.auth_required:
             await self.authentication_event.wait()
             self.authentication_event.clear()
@@ -450,19 +450,26 @@
             reader=self.reader,
             writer=self.writer,
             ssl_context=context,
         )
 
     async def read_socket_loop(self):
         extra_messages = []
+        timeout = 15
         while self.reader and not self.reader.at_eof():
             try:
-                data = await self.reader.readuntil(self.separator)
+                coro = self.reader.readuntil(self.separator)
+                data = await asyncio.wait_for(coro, timeout=timeout)
+            except TimeoutError as e:
+                log.error(f"Timeout of {timeout}s exceeded for socket read, returning")
+                self._connected = False
+                self.encrypted = False
+                break
             except asyncio.IncompleteReadError as e:
-                log.debug("EOF reached, socket closed")
+                # log.debug("EOF reached, socket closed")
                 self._connected = False
                 self.encrypted = False
                 break
             except ssl.SSLError as e:
                 log.error(e)
                 self._connected = False
                 self.encrypted = False
@@ -489,67 +496,64 @@
                     last_data = extra_messages.pop(0)
                     data.append(last_data + b"<?!!?>")
 
                 data = b"".join(data)
             except Exception as e:
                 print("in read socket loop")
                 print(repr(e))
+                self._connected = False
+                self.encrypted = False
                 break
 
             message = data.rstrip(self.separator)
 
             all_messages = [message, *extra_messages]
             extra_messages = []
 
             for message in all_messages:
                 # ToDo: catch
                 try:
                     message = SerializedMessage(message).deserialize()
                 except Exception as e:
                     print("can't deserialize in for")
                     print(repr(e))
+                    continue
                 log.debug(f"Received : {type(message).__name__}")
 
                 if self.encrypted:
                     message = message.decrypt(self.aeskey)
 
-                if isinstance(message, PtyMessage):
-                    our_socket = self.writer.get_extra_info("sockname")
-                    await self.on_pty_data_callback(our_socket, message.data)
-                    continue
-
-                if isinstance(message, RpcReplyMessage):
-                    await self.messages.put(message)
-                    continue
-
-                if isinstance(message, (ChallengeMessage, AuthReplyMessage)):
-                    await self.authentication_message_handler(message)
-                    continue
-
-                if isinstance(message, ProxyResponseMessage):
-                    asyncio.create_task(self.forwarding_message_handler(message))
-                    continue
-
-                if isinstance(message, (RsaPublicKeyMessage, TestMessage)):
-                    await self.encryption_message_handler(message)
-                    continue
-
-                # This is our test message as we're not encrypted yet
-                # it could be part of the handler above but more clear here
-                if isinstance(message, EncryptedMessage):
-                    await self.encryption_message_handler(message)
-                    continue
-
-                if isinstance(message, PtyClosedMessage):
-                    our_socket = self.writer.get_extra_info("sockname")
-                    await self.on_pty_closed_callback(our_socket)
-                    continue
+                match message:
+                    case PtyMessage():
+                        our_socket = self.writer.get_extra_info("sockname")
+                        await self.on_pty_data_callback(our_socket, message.data)
+
+                    case RpcReplyMessage():
+                        await self.messages.put(message)
+
+                    case ChallengeMessage(), AuthReplyMessage():
+                        await self.authentication_message_handler(message)
+
+                    case ProxyResponseMessage():
+                        asyncio.create_task(self.forwarding_message_handler(message))
+
+                    case RsaPublicKeyMessage(), TestMessage():
+                        await self.encryption_message_handler(message)
+
+                    # This is our test message as we're not encrypted yet
+                    # it could be part of the handler above but more clear here
+                    case EncryptedMessage():
+                        await self.encryption_message_handler(message)
+
+                    case PtyClosedMessage():
+                        our_socket = self.writer.get_extra_info("sockname")
+                        await self.on_pty_closed_callback(our_socket)
 
-                else:
-                    log.error(f"Unknown message: {message}")
+                    case _:
+                        log.error(f"Unknown message: {message}")
 
         log.debug("Finished read socket loop")
 
     async def send_pty_message(self, data):
         msg = PtyMessage(data)
         if self.encrypted:
             msg = msg.encrypt(self.aeskey)
@@ -658,14 +662,15 @@
         sockname = "Not connected"
         if self.writer:
             sockname = self.writer.get_extra_info("sockname")
         log.info(
             f"Disconnect called for socket: {sockname}. Total channels before: {self.channels}"
         )
         self.channels -= 1
+        # this is dodgey, -1 is True
         if self.channels:
             return
 
         self._disconnecting = True
 
         self.reset_state()
```

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/socket/messages.py` & `fluxrpc-0.9.9/fluxrpc/transports/socket/messages.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/socket/server.py` & `fluxrpc-0.9.9/fluxrpc/transports/socket/server.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/websocket.py` & `fluxrpc-0.9.9/fluxrpc/transports/websocket.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/websocketclient.py` & `fluxrpc-0.9.9/fluxrpc/transports/websocketclient.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/wsgi.py` & `fluxrpc-0.9.9/fluxrpc/transports/wsgi.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/fluxrpc/transports/zmq.py` & `fluxrpc-0.9.9/fluxrpc/transports/zmq.py`

 * *Files identical despite different names*

### Comparing `fluxrpc-0.9.8/pyproject.toml` & `fluxrpc-0.9.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "fluxrpc"
-version = "0.9.8"
+version = "0.9.9"
 description = "\"A sercure RPC provider for Flux\""
 authors = ["David White <dr.white.nz@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 six = "^1.16.0"
 pymongo = "^4.3.2"
 gevent = {version="^21.1.2", optional = true}
 gevent-websocket = {version="^0.10.1", optional = true}
 msgpack = {version="^1.0.2", optional = true}
 pika = {version="^1.2.0", optional = true}
 pyzmq = {version="^22.0.3", optional = true}
```

### Comparing `fluxrpc-0.9.8/setup.py` & `fluxrpc-0.9.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,24 +26,24 @@
             'python-bitcoinlib>=0.11.2,<0.12.0'],
  'websocket': ['gevent-websocket>=0.10.1,<0.11.0'],
  'wsgi': ['werkzeug>=2.2.2,<3.0.0'],
  'zmq': ['pyzmq>=22.0.3,<23.0.0']}
 
 setup_kwargs = {
     'name': 'fluxrpc',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': '"A sercure RPC provider for Flux"',
     'long_description': 'None',
     'author': 'David White',
     'author_email': 'dr.white.nz@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `fluxrpc-0.9.8/PKG-INFO` & `fluxrpc-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: fluxrpc
-Version: 0.9.8
+Version: 0.9.9
 Summary: "A sercure RPC provider for Flux"
 License: MIT
 Author: David White
 Author-email: dr.white.nz@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gevent
 Provides-Extra: httpclient
 Provides-Extra: jsonext
 Provides-Extra: msgpack
 Provides-Extra: rabbitmq
```

