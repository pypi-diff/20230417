# Comparing `tmp/sora_device_client-1.1.0.tar.gz` & `tmp/sora_device_client-1.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sora_device_client-1.1.0.tar", max compression
+gzip compressed data, was "sora_device_client-1.1.0a0.tar", max compression
```

## Comparing `sora_device_client-1.1.0.tar` & `sora_device_client-1.1.0a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     7288 2023-04-17 03:11:48.693472 sora_device_client-1.1.0/README.md
--rw-r--r--   0        0        0     1348 2023-04-17 03:17:27.507297 sora_device_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    20745 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/app/v1beta/service_pb2.py
--rw-r--r--   0        0        0    51578 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/app/v1beta/service_pb2_grpc.py
--rw-r--r--   0        0        0     4193 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/app/v1beta/types_pb2.py
--rw-r--r--   0        0        0      159 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/app/v1beta/types_pb2_grpc.py
--rw-r--r--   0        0        0     4134 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/device/v1beta/service_pb2.py
--rw-r--r--   0        0        0    10112 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/device/v1beta/service_pb2_grpc.py
--rw-r--r--   0        0        0     4480 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/v1beta/common_pb2.py
--rw-r--r--   0        0        0      159 2023-03-30 03:26:12.420385 sora_device_client-1.1.0/sora/v1beta/common_pb2_grpc.py
--rw-r--r--   0        0        0      384 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/__init__.py
--rw-r--r--   0        0        0     3491 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/auth0/__init__.py
--rw-r--r--   0        0        0      959 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/auth0/info.py
--rw-r--r--   0        0        0     1481 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/cli/__init__.py
--rw-r--r--   0        0        0     2520 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/cli/login.py
--rw-r--r--   0        0        0      385 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/cli/logout.py
--rw-r--r--   0        0        0      891 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/cli/paths.py
--rw-r--r--   0        0        0     2254 2023-04-17 03:11:48.693472 sora_device_client-1.1.0/sora_device_client/cli/start.py
--rw-r--r--   0        0        0    14769 2023-04-17 03:11:48.693472 sora_device_client-1.1.0/sora_device_client/client/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/config/__init__.py
--rw-r--r--   0        0        0     2093 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/config/device.py
--rw-r--r--   0        0        0      781 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/config/server.py
--rw-r--r--   0        0        0     2378 2023-04-11 04:00:37.651591 sora_device_client-1.1.0/sora_device_client/config_example.toml
--rw-r--r--   0        0        0     1609 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/drivers/__init__.py
--rw-r--r--   0        0        0      336 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/exceptions.py
--rw-r--r--   0        0        0     1332 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/formats/__init__.py
--rw-r--r--   0        0        0     2492 2023-04-10 23:29:44.863244 sora_device_client-1.1.0/sora_device_client/formats/sbp.py
--rw-r--r--   0        0        0      585 2023-04-17 03:11:48.693472 sora_device_client-1.1.0/sora_device_client/location.py
--rw-r--r--   0        0        0     8247 1970-01-01 00:00:00.000000 sora_device_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7288 2023-04-17 03:11:48.693472 sora_device_client-1.1.0a0/README.md
+-rw-r--r--   0        0        0     1350 2023-04-17 03:12:24.453971 sora_device_client-1.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0    20745 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/app/v1beta/service_pb2.py
+-rw-r--r--   0        0        0    51578 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/app/v1beta/service_pb2_grpc.py
+-rw-r--r--   0        0        0     4193 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/app/v1beta/types_pb2.py
+-rw-r--r--   0        0        0      159 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/app/v1beta/types_pb2_grpc.py
+-rw-r--r--   0        0        0     4134 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/device/v1beta/service_pb2.py
+-rw-r--r--   0        0        0    10112 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/device/v1beta/service_pb2_grpc.py
+-rw-r--r--   0        0        0     4480 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/v1beta/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-03-30 03:26:12.420385 sora_device_client-1.1.0a0/sora/v1beta/common_pb2_grpc.py
+-rw-r--r--   0        0        0      384 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/__init__.py
+-rw-r--r--   0        0        0     3491 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/auth0/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/auth0/info.py
+-rw-r--r--   0        0        0     1481 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/cli/__init__.py
+-rw-r--r--   0        0        0     2520 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/cli/login.py
+-rw-r--r--   0        0        0      385 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/cli/logout.py
+-rw-r--r--   0        0        0      891 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/cli/paths.py
+-rw-r--r--   0        0        0     2254 2023-04-17 03:11:48.693472 sora_device_client-1.1.0a0/sora_device_client/cli/start.py
+-rw-r--r--   0        0        0    14769 2023-04-17 03:11:48.693472 sora_device_client-1.1.0a0/sora_device_client/client/__init__.py
+-rw-r--r--   0        0        0     1470 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/config/__init__.py
+-rw-r--r--   0        0        0     2093 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/config/device.py
+-rw-r--r--   0        0        0      781 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/config/server.py
+-rw-r--r--   0        0        0     2378 2023-04-11 04:00:37.651591 sora_device_client-1.1.0a0/sora_device_client/config_example.toml
+-rw-r--r--   0        0        0     1609 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/drivers/__init__.py
+-rw-r--r--   0        0        0      336 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/exceptions.py
+-rw-r--r--   0        0        0     1332 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/formats/__init__.py
+-rw-r--r--   0        0        0     2492 2023-04-10 23:29:44.863244 sora_device_client-1.1.0a0/sora_device_client/formats/sbp.py
+-rw-r--r--   0        0        0      585 2023-04-17 03:11:48.693472 sora_device_client-1.1.0a0/sora_device_client/location.py
+-rw-r--r--   0        0        0     8249 1970-01-01 00:00:00.000000 sora_device_client-1.1.0a0/PKG-INFO
```

### Comparing `sora_device_client-1.1.0/README.md` & `sora_device_client-1.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/pyproject.toml` & `sora_device_client-1.1.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sora-device-client"
-version = "1.1.0"
+version = "1.1.0a0"
 description = "A client to stream device location data to a sever for the SORA api"
 authors = ["Swift Navigation <dev@swift-nav.com>"]
 readme = "README.md"
 packages = [{ include = "sora" }, { include = "sora_device_client" }]
 # poetry excludes stuff in .gitignore, so we need to make sure it gets picked up
 include = ["sora/**/*.py"]
 license = "MIT"
```

### Comparing `sora_device_client-1.1.0/sora/app/v1beta/service_pb2.py` & `sora_device_client-1.1.0a0/sora/app/v1beta/service_pb2.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora/app/v1beta/service_pb2_grpc.py` & `sora_device_client-1.1.0a0/sora/app/v1beta/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora/app/v1beta/types_pb2.py` & `sora_device_client-1.1.0a0/sora/app/v1beta/types_pb2.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora/device/v1beta/service_pb2.py` & `sora_device_client-1.1.0a0/sora/device/v1beta/service_pb2.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora/device/v1beta/service_pb2_grpc.py` & `sora_device_client-1.1.0a0/sora/device/v1beta/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora/v1beta/common_pb2.py` & `sora_device_client-1.1.0a0/sora/v1beta/common_pb2.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/auth0/__init__.py` & `sora_device_client-1.1.0a0/sora_device_client/auth0/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/auth0/info.py` & `sora_device_client-1.1.0a0/sora_device_client/auth0/info.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/cli/__init__.py` & `sora_device_client-1.1.0a0/sora_device_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/cli/login.py` & `sora_device_client-1.1.0a0/sora_device_client/cli/login.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/cli/paths.py` & `sora_device_client-1.1.0a0/sora_device_client/cli/paths.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/cli/start.py` & `sora_device_client-1.1.0a0/sora_device_client/cli/start.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/client/__init__.py` & `sora_device_client-1.1.0a0/sora_device_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/config/__init__.py` & `sora_device_client-1.1.0a0/sora_device_client/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/config/device.py` & `sora_device_client-1.1.0a0/sora_device_client/config/device.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/config/server.py` & `sora_device_client-1.1.0a0/sora_device_client/config/server.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/config_example.toml` & `sora_device_client-1.1.0a0/sora_device_client/config_example.toml`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/drivers/__init__.py` & `sora_device_client-1.1.0a0/sora_device_client/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/formats/__init__.py` & `sora_device_client-1.1.0a0/sora_device_client/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/formats/sbp.py` & `sora_device_client-1.1.0a0/sora_device_client/formats/sbp.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/sora_device_client/location.py` & `sora_device_client-1.1.0a0/sora_device_client/location.py`

 * *Files identical despite different names*

### Comparing `sora_device_client-1.1.0/PKG-INFO` & `sora_device_client-1.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sora-device-client
-Version: 1.1.0
+Version: 1.1.0a0
 Summary: A client to stream device location data to a sever for the SORA api
 License: MIT
 Author: Swift Navigation
 Author-email: dev@swift-nav.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

