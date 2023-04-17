# Comparing `tmp/grpc_auth_service-0.0.8.tar.gz` & `tmp/grpc_auth_service-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_auth_service-0.0.8.tar", last modified: Sun Jan  8 14:16:51 2023, max compression
+gzip compressed data, was "grpc_auth_service-0.0.9.tar", last modified: Sun Jan  8 18:27:04 2023, max compression
```

## Comparing `grpc_auth_service-0.0.8.tar` & `grpc_auth_service-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 14:16:51.247464 grpc_auth_service-0.0.8/
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     1069 2023-01-07 22:49:29.000000 grpc_auth_service-0.0.8/LICENSE
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       44 2023-01-07 23:35:39.000000 grpc_auth_service-0.0.8/MANIFEST.in
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      446 2023-01-08 14:16:51.247464 grpc_auth_service-0.0.8/PKG-INFO
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       50 2023-01-07 22:52:46.000000 grpc_auth_service-0.0.8/README.md
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     1479 2023-01-08 00:08:36.000000 grpc_auth_service-0.0.8/pyproject.toml
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      548 2023-01-08 14:16:51.247464 grpc_auth_service-0.0.8/setup.cfg
-drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 14:16:51.243463 grpc_auth_service-0.0.8/src/
-drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 14:16:51.247464 grpc_auth_service-0.0.8/src/grpc_auth_service/
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-07 22:47:07.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/__init__.py
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     2687 2023-01-08 14:14:03.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/auth_service_pb2.py
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     2656 2023-01-08 14:15:30.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/auth_service_pb2.pyi
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     7068 2023-01-08 14:14:49.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/auth_service_pb2_grpc.py
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       10 2023-01-07 23:58:24.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/py.typed
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     3118 2023-01-08 14:14:03.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/user_service_pb2.py
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     3061 2023-01-08 14:15:30.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/user_service_pb2.pyi
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     7333 2023-01-08 14:14:52.000000 grpc_auth_service-0.0.8/src/grpc_auth_service/user_service_pb2_grpc.py
-drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 14:16:51.247464 grpc_auth_service-0.0.8/src/grpc_auth_service.egg-info/
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      446 2023-01-08 14:16:51.000000 grpc_auth_service-0.0.8/src/grpc_auth_service.egg-info/PKG-INFO
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      563 2023-01-08 14:16:51.000000 grpc_auth_service-0.0.8/src/grpc_auth_service.egg-info/SOURCES.txt
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)        1 2023-01-08 14:16:51.000000 grpc_auth_service-0.0.8/src/grpc_auth_service.egg-info/dependency_links.txt
--rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       18 2023-01-08 14:16:51.000000 grpc_auth_service-0.0.8/src/grpc_auth_service.egg-info/top_level.txt
+drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 18:27:04.591486 grpc_auth_service-0.0.9/
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     1069 2023-01-07 22:49:29.000000 grpc_auth_service-0.0.9/LICENSE
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       44 2023-01-07 23:35:39.000000 grpc_auth_service-0.0.9/MANIFEST.in
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      446 2023-01-08 18:27:04.591486 grpc_auth_service-0.0.9/PKG-INFO
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       50 2023-01-07 22:52:46.000000 grpc_auth_service-0.0.9/README.md
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     1479 2023-01-08 00:08:36.000000 grpc_auth_service-0.0.9/pyproject.toml
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      548 2023-01-08 18:27:04.591486 grpc_auth_service-0.0.9/setup.cfg
+drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 18:27:04.591486 grpc_auth_service-0.0.9/src/
+drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 18:27:04.591486 grpc_auth_service-0.0.9/src/grpc_auth_service/
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-07 22:47:07.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/__init__.py
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     3067 2023-01-08 18:26:17.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/auth_service_pb2.py
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     2974 2023-01-08 18:26:17.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/auth_service_pb2.pyi
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     8652 2023-01-08 18:26:51.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/auth_service_pb2_grpc.py
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       10 2023-01-07 23:58:24.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/py.typed
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     3118 2023-01-08 18:26:17.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/user_service_pb2.py
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     3061 2023-01-08 18:26:28.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/user_service_pb2.pyi
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)     7333 2023-01-08 18:26:31.000000 grpc_auth_service-0.0.9/src/grpc_auth_service/user_service_pb2_grpc.py
+drwxrwxr-x   0 mnestulei  (1000) mnestulei  (1000)        0 2023-01-08 18:27:04.591486 grpc_auth_service-0.0.9/src/grpc_auth_service.egg-info/
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      446 2023-01-08 18:27:04.000000 grpc_auth_service-0.0.9/src/grpc_auth_service.egg-info/PKG-INFO
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)      563 2023-01-08 18:27:04.000000 grpc_auth_service-0.0.9/src/grpc_auth_service.egg-info/SOURCES.txt
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)        1 2023-01-08 18:27:04.000000 grpc_auth_service-0.0.9/src/grpc_auth_service.egg-info/dependency_links.txt
+-rw-rw-r--   0 mnestulei  (1000) mnestulei  (1000)       18 2023-01-08 18:27:04.000000 grpc_auth_service-0.0.9/src/grpc_auth_service.egg-info/top_level.txt
```

### Comparing `grpc_auth_service-0.0.8/LICENSE` & `grpc_auth_service-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc_auth_service-0.0.8/pyproject.toml` & `grpc_auth_service-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `grpc_auth_service-0.0.8/setup.cfg` & `grpc_auth_service-0.0.9/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = grpc_auth_service
-version = 0.0.8
+version = 0.0.9
 author = Async Boat
 author_email = nestulej@gmail.com
 description = A grpc autogenerated code for Auth microservice of online cinema
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `grpc_auth_service-0.0.8/src/grpc_auth_service/auth_service_pb2.py` & `grpc_auth_service-0.0.9/src/grpc_auth_service/auth_service_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x12\x61uth_service.proto"/\n\x0cLoginRequest\x12\r\n\x05login\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t"d\n\rLoginResponse\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\t\x12\x12\n\ntoken_type\x18\x04 \x01(\t",\n\x13RefreshTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t"k\n\x14RefreshTokenResponse\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\t\x12\x12\n\ntoken_type\x18\x04 \x01(\t"%\n\rLogoutRequest\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t"\x10\n\x0eLogoutResponse")\n\x11\x43heckTokenRequest\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t"%\n\x12\x43heckTokenResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x32\xcd\x01\n\x04\x41uth\x12&\n\x05Login\x12\r.LoginRequest\x1a\x0e.LoginResponse\x12;\n\x0cRefreshToken\x12\x14.RefreshTokenRequest\x1a\x15.RefreshTokenResponse\x12)\n\x06Logout\x12\x0e.LogoutRequest\x1a\x0f.LogoutResponse\x12\x35\n\nCheckToken\x12\x12.CheckTokenRequest\x1a\x13.CheckTokenResponseb\x06proto3'
+    b'\n\x12\x61uth_service.proto"/\n\x0cLoginRequest\x12\r\n\x05login\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t"d\n\rLoginResponse\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\t\x12\x12\n\ntoken_type\x18\x04 \x01(\t",\n\x13RefreshTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t"k\n\x14RefreshTokenResponse\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\t\x12\x12\n\ntoken_type\x18\x04 \x01(\t"%\n\rLogoutRequest\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t"\x10\n\x0eLogoutResponse"*\n\x12LogoutOtherRequest\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t"\x15\n\x13LogoutOtherResponse")\n\x11\x43heckTokenRequest\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t"%\n\x12\x43heckTokenResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x32\x87\x02\n\x04\x41uth\x12&\n\x05Login\x12\r.LoginRequest\x1a\x0e.LoginResponse\x12;\n\x0cRefreshToken\x12\x14.RefreshTokenRequest\x1a\x15.RefreshTokenResponse\x12)\n\x06Logout\x12\x0e.LogoutRequest\x1a\x0f.LogoutResponse\x12\x38\n\x0bLogoutOther\x12\x13.LogoutOtherRequest\x1a\x14.LogoutOtherResponse\x12\x35\n\nCheckToken\x12\x12.CheckTokenRequest\x1a\x13.CheckTokenResponseb\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "auth_service_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS is False:
 
     DESCRIPTOR._options = None
@@ -28,14 +28,18 @@
     _REFRESHTOKENREQUEST._serialized_end = 217
     _REFRESHTOKENRESPONSE._serialized_start = 219
     _REFRESHTOKENRESPONSE._serialized_end = 326
     _LOGOUTREQUEST._serialized_start = 328
     _LOGOUTREQUEST._serialized_end = 365
     _LOGOUTRESPONSE._serialized_start = 367
     _LOGOUTRESPONSE._serialized_end = 383
-    _CHECKTOKENREQUEST._serialized_start = 385
-    _CHECKTOKENREQUEST._serialized_end = 426
-    _CHECKTOKENRESPONSE._serialized_start = 428
-    _CHECKTOKENRESPONSE._serialized_end = 465
-    _AUTH._serialized_start = 468
-    _AUTH._serialized_end = 673
+    _LOGOUTOTHERREQUEST._serialized_start = 385
+    _LOGOUTOTHERREQUEST._serialized_end = 427
+    _LOGOUTOTHERRESPONSE._serialized_start = 429
+    _LOGOUTOTHERRESPONSE._serialized_end = 450
+    _CHECKTOKENREQUEST._serialized_start = 452
+    _CHECKTOKENREQUEST._serialized_end = 493
+    _CHECKTOKENRESPONSE._serialized_start = 495
+    _CHECKTOKENRESPONSE._serialized_end = 532
+    _AUTH._serialized_start = 535
+    _AUTH._serialized_end = 798
 # @@protoc_insertion_point(module_scope)
```

### Comparing `grpc_auth_service-0.0.8/src/grpc_auth_service/auth_service_pb2.pyi` & `grpc_auth_service-0.0.9/src/grpc_auth_service/auth_service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import ClassVar as _ClassVar, Optional as _Optional
-
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class CheckTokenRequest(_message.Message):
     __slots__ = ["access_token"]
     ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
     access_token: str
@@ -39,14 +38,24 @@
         self,
         access_token: _Optional[str] = ...,
         refresh_token: _Optional[str] = ...,
         expires_in: _Optional[str] = ...,
         token_type: _Optional[str] = ...,
     ) -> None: ...
 
+class LogoutOtherRequest(_message.Message):
+    __slots__ = ["access_token"]
+    ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    access_token: str
+    def __init__(self, access_token: _Optional[str] = ...) -> None: ...
+
+class LogoutOtherResponse(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
 class LogoutRequest(_message.Message):
     __slots__ = ["access_token"]
     ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
     access_token: str
     def __init__(self, access_token: _Optional[str] = ...) -> None: ...
 
 class LogoutResponse(_message.Message):
```

### Comparing `grpc_auth_service-0.0.8/src/grpc_auth_service/auth_service_pb2_grpc.py` & `grpc_auth_service-0.0.9/src/grpc_auth_service/auth_service_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,19 @@
             response_deserializer=auth__service__pb2.RefreshTokenResponse.FromString,
         )
         self.Logout = channel.unary_unary(
             "/Auth/Logout",
             request_serializer=auth__service__pb2.LogoutRequest.SerializeToString,
             response_deserializer=auth__service__pb2.LogoutResponse.FromString,
         )
+        self.LogoutOther = channel.unary_unary(
+            "/Auth/LogoutOther",
+            request_serializer=auth__service__pb2.LogoutOtherRequest.SerializeToString,
+            response_deserializer=auth__service__pb2.LogoutOtherResponse.FromString,
+        )
         self.CheckToken = channel.unary_unary(
             "/Auth/CheckToken",
             request_serializer=auth__service__pb2.CheckTokenRequest.SerializeToString,
             response_deserializer=auth__service__pb2.CheckTokenResponse.FromString,
         )
 
 
@@ -53,14 +58,20 @@
 
     def Logout(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def LogoutOther(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
     def CheckToken(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
 
@@ -77,14 +88,19 @@
             response_serializer=auth__service__pb2.RefreshTokenResponse.SerializeToString,
         ),
         "Logout": grpc.unary_unary_rpc_method_handler(
             servicer.Logout,
             request_deserializer=auth__service__pb2.LogoutRequest.FromString,
             response_serializer=auth__service__pb2.LogoutResponse.SerializeToString,
         ),
+        "LogoutOther": grpc.unary_unary_rpc_method_handler(
+            servicer.LogoutOther,
+            request_deserializer=auth__service__pb2.LogoutOtherRequest.FromString,
+            response_serializer=auth__service__pb2.LogoutOtherResponse.SerializeToString,
+        ),
         "CheckToken": grpc.unary_unary_rpc_method_handler(
             servicer.CheckToken,
             request_deserializer=auth__service__pb2.CheckTokenRequest.FromString,
             response_serializer=auth__service__pb2.CheckTokenResponse.SerializeToString,
         ),
     }
     generic_handler = grpc.method_handlers_generic_handler("Auth", rpc_method_handlers)
@@ -175,14 +191,43 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def LogoutOther(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/Auth/LogoutOther",
+            auth__service__pb2.LogoutOtherRequest.SerializeToString,
+            auth__service__pb2.LogoutOtherResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
 
     @staticmethod
     def CheckToken(
         request,
         target,
```

### Comparing `grpc_auth_service-0.0.8/src/grpc_auth_service/user_service_pb2.py` & `grpc_auth_service-0.0.9/src/grpc_auth_service/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `grpc_auth_service-0.0.8/src/grpc_auth_service/user_service_pb2.pyi` & `grpc_auth_service-0.0.9/src/grpc_auth_service/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpc_auth_service-0.0.8/src/grpc_auth_service/user_service_pb2_grpc.py` & `grpc_auth_service-0.0.9/src/grpc_auth_service/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `grpc_auth_service-0.0.8/src/grpc_auth_service.egg-info/SOURCES.txt` & `grpc_auth_service-0.0.9/src/grpc_auth_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

