# Comparing `tmp/dittoffi-0.0.2.tar.gz` & `tmp/dittoffi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dittoffi-0.0.2.tar", last modified: Fri Apr 14 15:33:34 2023, max compression
+gzip compressed data, was "dittoffi-0.0.3.tar", last modified: Mon Apr 17 09:24:11 2023, max compression
```

## Comparing `dittoffi-0.0.2.tar` & `dittoffi-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:33:34.020220 dittoffi-0.0.2/
--rw-r--r--   0 ronan     (1000) ronan     (1000)     1815 2023-04-14 13:25:48.000000 dittoffi-0.0.2/LICENSE.md
--rw-r--r--   0 ronan     (1000) ronan     (1000)       46 2023-04-13 15:26:57.000000 dittoffi-0.0.2/MANIFEST.in
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2926 2023-04-14 15:33:34.020220 dittoffi-0.0.2/PKG-INFO
--rw-r--r--   0 ronan     (1000) ronan     (1000)      576 2023-04-14 13:25:48.000000 dittoffi-0.0.2/README.md
--rw-r--r--   0 ronan     (1000) ronan     (1000)      537 2023-04-14 15:33:02.000000 dittoffi-0.0.2/pyproject.toml
--rw-r--r--   0 ronan     (1000) ronan     (1000)       38 2023-04-14 15:33:34.020220 dittoffi-0.0.2/setup.cfg
--rw-r--r--   0 ronan     (1000) ronan     (1000)      189 2023-04-13 15:26:57.000000 dittoffi-0.0.2/setup.py
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:33:34.020220 dittoffi-0.0.2/src/
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:33:34.020220 dittoffi-0.0.2/src/_dittoffi/
--rw-r--r--   0 ronan     (1000) ronan     (1000)      265 2023-04-14 13:25:48.000000 dittoffi-0.0.2/src/_dittoffi/__init__.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)     3610 2023-04-14 13:25:48.000000 dittoffi-0.0.2/src/_dittoffi/_ffi_build.py
--rw-r--r--   0 ronan     (1000) ronan     (1000)    60190 2023-04-14 13:25:48.000000 dittoffi-0.0.2/src/_dittoffi/dittoffi.cffi
--rw-r--r--   0 ronan     (1000) ronan     (1000)   112301 2023-04-13 06:27:45.000000 dittoffi-0.0.2/src/_dittoffi/dittoffi.h
-drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-14 15:33:34.020220 dittoffi-0.0.2/src/dittoffi.egg-info/
--rw-r--r--   0 ronan     (1000) ronan     (1000)     2926 2023-04-14 15:33:33.000000 dittoffi-0.0.2/src/dittoffi.egg-info/PKG-INFO
--rw-r--r--   0 ronan     (1000) ronan     (1000)      307 2023-04-14 15:33:34.000000 dittoffi-0.0.2/src/dittoffi.egg-info/SOURCES.txt
--rw-r--r--   0 ronan     (1000) ronan     (1000)        1 2023-04-14 15:33:33.000000 dittoffi-0.0.2/src/dittoffi.egg-info/dependency_links.txt
--rw-r--r--   0 ronan     (1000) ronan     (1000)       15 2023-04-14 15:33:33.000000 dittoffi-0.0.2/src/dittoffi.egg-info/top_level.txt
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:24:11.704702 dittoffi-0.0.3/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     1815 2023-04-14 13:25:48.000000 dittoffi-0.0.3/LICENSE.md
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       46 2023-04-13 15:26:57.000000 dittoffi-0.0.3/MANIFEST.in
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2926 2023-04-17 09:24:11.704702 dittoffi-0.0.3/PKG-INFO
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      576 2023-04-14 13:25:48.000000 dittoffi-0.0.3/README.md
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      537 2023-04-17 09:21:53.000000 dittoffi-0.0.3/pyproject.toml
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       38 2023-04-17 09:24:11.704702 dittoffi-0.0.3/setup.cfg
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      189 2023-04-17 09:02:19.000000 dittoffi-0.0.3/setup.py
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:24:11.704702 dittoffi-0.0.3/src/
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:24:11.704702 dittoffi-0.0.3/src/_dittoffi/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      265 2023-04-14 13:25:48.000000 dittoffi-0.0.3/src/_dittoffi/__init__.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     4223 2023-04-17 08:25:34.000000 dittoffi-0.0.3/src/_dittoffi/_ffi_build.py
+-rw-r--r--   0 ronan     (1000) ronan     (1000)    60190 2023-04-14 13:25:48.000000 dittoffi-0.0.3/src/_dittoffi/dittoffi.cffi
+-rw-r--r--   0 ronan     (1000) ronan     (1000)   112301 2023-04-13 06:27:45.000000 dittoffi-0.0.3/src/_dittoffi/dittoffi.h
+drwxr-xr-x   0 ronan     (1000) ronan     (1000)        0 2023-04-17 09:24:11.704702 dittoffi-0.0.3/src/dittoffi.egg-info/
+-rw-r--r--   0 ronan     (1000) ronan     (1000)     2926 2023-04-17 09:24:11.000000 dittoffi-0.0.3/src/dittoffi.egg-info/PKG-INFO
+-rw-r--r--   0 ronan     (1000) ronan     (1000)      342 2023-04-17 09:24:11.000000 dittoffi-0.0.3/src/dittoffi.egg-info/SOURCES.txt
+-rw-r--r--   0 ronan     (1000) ronan     (1000)        1 2023-04-17 09:24:11.000000 dittoffi-0.0.3/src/dittoffi.egg-info/dependency_links.txt
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       13 2023-04-17 09:24:11.000000 dittoffi-0.0.3/src/dittoffi.egg-info/requires.txt
+-rw-r--r--   0 ronan     (1000) ronan     (1000)       15 2023-04-17 09:24:11.000000 dittoffi-0.0.3/src/dittoffi.egg-info/top_level.txt
```

### Comparing `dittoffi-0.0.2/LICENSE.md` & `dittoffi-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dittoffi-0.0.2/PKG-INFO` & `dittoffi-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dittoffi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ditto FFI bindings for Python.
 Author-email: Ditto Engineering Team <engineering@ditto.live>
 License: Ditto Binary License
         
         Copyright © 2021 DittoLive Incorporated. All rights reserved.
         
         NOTICE: All information contained herein is, and remains the property of
```

### Comparing `dittoffi-0.0.2/README.md` & `dittoffi-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dittoffi-0.0.2/src/_dittoffi/_ffi_build.py` & `dittoffi-0.0.3/src/_dittoffi/_ffi_build.py`

 * *Files 13% similar despite different names*

```diff
@@ -100,16 +100,32 @@
     # Windows :
     # C:\Windows\System32
     # PWD
     path = os.environ.get("PWD")
     if path is not None and dir_contains_file(path, lib_name):
         return path
 
+    # Download dittoffi
+    platform_name = platform.system()
+    platform_proc_type  = platform.uname()[4]
+    is_arm = "arm" in platform_proc_type
+
+    if platform_name == "Linux" and is_arm:
+        target = "arm-unknown-linux-gnueabihf"
+    elif platform_name == "Linux" and not is_arm:
+        target = "x86_64-unknown-linux-gnu"
+    elif platform_name == "Darwin" and is_arm:
+        target = "aarch64-apple-darwin"
+    elif platform_name == "Darwin" and not is_arm: #x86
+        target = "x86_64-apple-darwin"
+    else:
+        raise SystemError(f"The platform {platform_name} on {platform_proc_type} is not supported yet!")
+
     #TODO : match target architecture
-    await download_libdittoffi(path, LIB_VERSION, "x86_64-unknown-linux-gnu", lib_name)
+    await download_libdittoffi(path, LIB_VERSION, target, lib_name)
     return path
 
 async def prepare_compilation():
     with read_header_file("dittoffi.cffi") as content:
         ffi.cdef(content)
 
     with read_header_file("dittoffi.h") as content:
```

### Comparing `dittoffi-0.0.2/src/_dittoffi/dittoffi.cffi` & `dittoffi-0.0.3/src/_dittoffi/dittoffi.cffi`

 * *Files identical despite different names*

### Comparing `dittoffi-0.0.2/src/_dittoffi/dittoffi.h` & `dittoffi-0.0.3/src/_dittoffi/dittoffi.h`

 * *Files identical despite different names*

### Comparing `dittoffi-0.0.2/src/dittoffi.egg-info/PKG-INFO` & `dittoffi-0.0.3/src/dittoffi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dittoffi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Ditto FFI bindings for Python.
 Author-email: Ditto Engineering Team <engineering@ditto.live>
 License: Ditto Binary License
         
         Copyright © 2021 DittoLive Incorporated. All rights reserved.
         
         NOTICE: All information contained herein is, and remains the property of
```

