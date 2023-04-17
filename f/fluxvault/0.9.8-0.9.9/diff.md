# Comparing `tmp/fluxvault-0.9.8.tar.gz` & `tmp/fluxvault-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxvault-0.9.8.tar", max compression
+gzip compressed data, was "fluxvault-0.9.9.tar", max compression
```

## Comparing `fluxvault-0.9.8.tar` & `fluxvault-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1138 2023-01-06 18:29:06.059430 fluxvault-0.9.8/LICENSE
--rw-r--r--   0        0        0      187 2023-03-20 04:37:59.728292 fluxvault-0.9.8/fluxvault/__init__.py
--rw-r--r--   0        0        0     2863 2023-03-13 23:44:52.505465 fluxvault-0.9.8/fluxvault/app_init.py
--rw-r--r--   0        0        0    28158 2023-03-23 22:46:40.349567 fluxvault-0.9.8/fluxvault/cli.py
--rw-r--r--   0        0        0      300 2023-03-15 22:12:23.253389 fluxvault-0.9.8/fluxvault/constants.py
--rw-r--r--   0        0        0      230 2023-01-27 06:48:21.728108 fluxvault-0.9.8/fluxvault/extensions.py
--rw-r--r--   0        0        0    25043 2023-03-23 22:46:30.931436 fluxvault-0.9.8/fluxvault/fluxagent.py
--rw-r--r--   0        0        0    13190 2023-03-19 23:26:56.719254 fluxvault-0.9.8/fluxvault/fluxapp.py
--rw-r--r--   0        0        0    39678 2023-03-24 18:32:16.502187 fluxvault-0.9.8/fluxvault/fluxkeeper.py
--rw-r--r--   0        0        0     5014 2023-01-23 01:26:19.495189 fluxvault-0.9.8/fluxvault/fluxkeeper_gui.py
--rw-r--r--   0        0        0    25520 2023-03-24 23:18:50.981385 fluxvault-0.9.8/fluxvault/fs.py
--rw-r--r--   0        0        0     7317 2023-03-20 20:35:17.232411 fluxvault-0.9.8/fluxvault/helpers.py
--rw-r--r--   0        0        0     1495 2023-02-13 23:50:31.889530 fluxvault-0.9.8/fluxvault/log.py
--rw-r--r--   0        0        0     8305 2023-03-14 18:31:10.375164 fluxvault-0.9.8/fluxvault/registrar.py
--rw-r--r--   0        0        0     1013 2023-03-26 01:35:56.564095 fluxvault-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 fluxvault-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1138 2023-01-06 18:29:06.059430 fluxvault-0.9.9/LICENSE
+-rw-r--r--   0        0        0      187 2023-03-20 04:37:59.728292 fluxvault-0.9.9/fluxvault/__init__.py
+-rw-r--r--   0        0        0     2863 2023-03-13 23:44:52.505465 fluxvault-0.9.9/fluxvault/app_init.py
+-rw-r--r--   0        0        0    28158 2023-03-23 22:46:40.349567 fluxvault-0.9.9/fluxvault/cli.py
+-rw-r--r--   0        0        0      300 2023-03-15 22:12:23.253389 fluxvault-0.9.9/fluxvault/constants.py
+-rw-r--r--   0        0        0      230 2023-01-27 06:48:21.728108 fluxvault-0.9.9/fluxvault/extensions.py
+-rw-r--r--   0        0        0    25043 2023-03-23 22:46:30.931436 fluxvault-0.9.9/fluxvault/fluxagent.py
+-rw-r--r--   0        0        0    13190 2023-03-19 23:26:56.719254 fluxvault-0.9.9/fluxvault/fluxapp.py
+-rw-r--r--   0        0        0    39678 2023-03-24 18:32:16.502187 fluxvault-0.9.9/fluxvault/fluxkeeper.py
+-rw-r--r--   0        0        0     5098 2023-03-26 01:44:45.030082 fluxvault-0.9.9/fluxvault/fluxkeeper_gui.py
+-rw-r--r--   0        0        0    25520 2023-03-24 23:18:50.981385 fluxvault-0.9.9/fluxvault/fs.py
+-rw-r--r--   0        0        0     7317 2023-03-20 20:35:17.232411 fluxvault-0.9.9/fluxvault/helpers.py
+-rw-r--r--   0        0        0     1495 2023-02-13 23:50:31.889530 fluxvault-0.9.9/fluxvault/log.py
+-rw-r--r--   0        0        0     8305 2023-03-14 18:31:10.375164 fluxvault-0.9.9/fluxvault/registrar.py
+-rw-r--r--   0        0        0     1013 2023-03-26 01:45:16.739207 fluxvault-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1167 1970-01-01 00:00:00.000000 fluxvault-0.9.9/PKG-INFO
```

### Comparing `fluxvault-0.9.8/LICENSE` & `fluxvault-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/app_init.py` & `fluxvault-0.9.9/fluxvault/app_init.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/cli.py` & `fluxvault-0.9.9/fluxvault/cli.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/fluxagent.py` & `fluxvault-0.9.9/fluxvault/fluxagent.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/fluxapp.py` & `fluxvault-0.9.9/fluxvault/fluxapp.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/fluxkeeper.py` & `fluxvault-0.9.9/fluxvault/fluxkeeper.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/fluxkeeper_gui.py` & `fluxvault-0.9.9/fluxvault/fluxkeeper_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 
 
 @dataclass
 class FluxKeeperGui:
     address: str
     port: int
     keeper: FluxKeeper
-    root_dir: Path = Path(".")
-    app: web.Application = web.Application()
-    sio: socketio.AsyncServer = socketio.AsyncServer(cors_allowed_origins="*")
+    root_dir: Path = field(default_factory=Path)
+    app: web.Application = field(default_factory=web.Application)
+    sio: socketio.AsyncServer = field(
+        default_factory=lambda: socketio.AsyncServer(cors_allowed_origins="*")
+    )
     namespace: str = "/pty"
 
     @staticmethod
     async def index(request):
         print("received request")
         """Serve the client-side application."""
         with open("index.html") as f:
```

### Comparing `fluxvault-0.9.8/fluxvault/fs.py` & `fluxvault-0.9.9/fluxvault/fs.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/helpers.py` & `fluxvault-0.9.9/fluxvault/helpers.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/log.py` & `fluxvault-0.9.9/fluxvault/log.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/fluxvault/registrar.py` & `fluxvault-0.9.9/fluxvault/registrar.py`

 * *Files identical despite different names*

### Comparing `fluxvault-0.9.8/pyproject.toml` & `fluxvault-0.9.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluxvault"
-version = "0.9.8"
+version = "0.9.9"
 description = "A system to load secrets into Flux applications"
 authors = ["David White <dr.white.nz@gmail.com>", "Tom Moulton <tom@moulton.us>"]
 license = "MIT"
 repository = "https://github.com/RunOnFlux/FluxVault.git"
 homepage = "https://runonflux.io"
 
 [tool.poetry.dependencies]
```

### Comparing `fluxvault-0.9.8/PKG-INFO` & `fluxvault-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxvault
-Version: 0.9.8
+Version: 0.9.9
 Summary: A system to load secrets into Flux applications
 Home-page: https://runonflux.io
 License: MIT
 Author: David White
 Author-email: dr.white.nz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

