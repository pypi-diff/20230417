# Comparing `tmp/polywrap_wasm-0.1.0a6.tar.gz` & `tmp/polywrap_wasm-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_wasm-0.1.0a6.tar", max compression
+gzip compressed data, was "polywrap_wasm-0.1.0a7.tar", max compression
```

## Comparing `polywrap_wasm-0.1.0a6.tar` & `polywrap_wasm-0.1.0a7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0        4 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/README.md
--rw-r--r--   0        0        0      228 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/__init__.py
--rw-r--r--   0        0        0     1880 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/buffer.py
--rw-r--r--   0        0        0       64 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/constants.py
--rw-r--r--   0        0        0      381 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/errors.py
--rw-r--r--   0        0        0    31434 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/example-wasm-files/wrap.wasm
--rw-r--r--   0        0        0      859 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/exports.py
--rw-r--r--   0        0        0    16304 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/imports.py
--rw-r--r--   0        0        0      994 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/inmemory_file_reader.py
--rw-r--r--   0        0        0       21 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/types/__init__.py
--rw-r--r--   0        0        0     1009 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/types/state.py
--rw-r--r--   0        0        0     2648 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/wasm_package.py
--rw-r--r--   0        0        0     3276 2023-03-02 19:49:55.545791 polywrap_wasm-0.1.0a6/polywrap_wasm/wasm_wrapper.py
--rw-r--r--   0        0        0     1133 2023-03-02 19:52:06.748172 polywrap_wasm-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0        4 2022-10-16 06:28:28.645779 polywrap_wasm-0.1.0a7/README.md
+-rw-r--r--   0        0        0      228 2022-10-17 13:37:13.496919 polywrap_wasm-0.1.0a7/polywrap_wasm/__init__.py
+-rw-r--r--   0        0        0     1880 2023-02-24 14:26:10.918069 polywrap_wasm-0.1.0a7/polywrap_wasm/buffer.py
+-rw-r--r--   0        0        0       64 2023-02-22 15:57:14.720682 polywrap_wasm-0.1.0a7/polywrap_wasm/constants.py
+-rw-r--r--   0        0        0      381 2022-10-16 06:28:28.649783 polywrap_wasm-0.1.0a7/polywrap_wasm/errors.py
+-rw-r--r--   0        0        0    31434 2022-10-16 06:28:28.650532 polywrap_wasm-0.1.0a7/polywrap_wasm/example-wasm-files/wrap.wasm
+-rw-r--r--   0        0        0      859 2022-10-27 11:21:02.039549 polywrap_wasm-0.1.0a7/polywrap_wasm/exports.py
+-rw-r--r--   0        0        0    16304 2023-03-02 18:40:25.696994 polywrap_wasm-0.1.0a7/polywrap_wasm/imports.py
+-rw-r--r--   0        0        0      994 2023-02-22 15:57:14.720770 polywrap_wasm-0.1.0a7/polywrap_wasm/inmemory_file_reader.py
+-rw-r--r--   0        0        0       21 2022-10-16 06:28:28.652225 polywrap_wasm-0.1.0a7/polywrap_wasm/types/__init__.py
+-rw-r--r--   0        0        0     1009 2023-02-22 15:57:14.720871 polywrap_wasm-0.1.0a7/polywrap_wasm/types/state.py
+-rw-r--r--   0        0        0     2648 2023-02-22 15:57:14.721422 polywrap_wasm-0.1.0a7/polywrap_wasm/wasm_package.py
+-rw-r--r--   0        0        0     3276 2023-02-22 15:57:14.721526 polywrap_wasm-0.1.0a7/polywrap_wasm/wasm_wrapper.py
+-rw-r--r--   0        0        0     1133 2023-03-02 20:02:08.941294 polywrap_wasm-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0a7/setup.py
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0a7/PKG-INFO
```

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/buffer.py` & `polywrap_wasm-0.1.0a7/polywrap_wasm/buffer.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/example-wasm-files/wrap.wasm` & `polywrap_wasm-0.1.0a7/polywrap_wasm/example-wasm-files/wrap.wasm`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/exports.py` & `polywrap_wasm-0.1.0a7/polywrap_wasm/exports.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/imports.py` & `polywrap_wasm-0.1.0a7/polywrap_wasm/imports.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/inmemory_file_reader.py` & `polywrap_wasm-0.1.0a7/polywrap_wasm/inmemory_file_reader.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/types/state.py` & `polywrap_wasm-0.1.0a7/polywrap_wasm/types/state.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/wasm_package.py` & `polywrap_wasm-0.1.0a7/polywrap_wasm/wasm_package.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/polywrap_wasm/wasm_wrapper.py` & `polywrap_wasm-0.1.0a7/polywrap_wasm/wasm_wrapper.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0a6/pyproject.toml` & `polywrap_wasm-0.1.0a7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-wasm"
-version = "0.1.0a6"
+version = "0.1.0a7"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 wasmtime = "^1.0.1"
-polywrap-core = "0.1.0a6"
-polywrap-manifest = "0.1.0a4"
-polywrap-msgpack = "0.1.0a4"
-polywrap-result = "0.1.0a4"
+polywrap-core = "0.1.0a7"
+polywrap-manifest = "0.1.0a7"
+polywrap-msgpack = "0.1.0a7"
+polywrap-result = "0.1.0a7"
 unsync = "^1.4.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
```

### Comparing `polywrap_wasm-0.1.0a6/PKG-INFO` & `polywrap_wasm-0.1.0a7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: polywrap-wasm
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: 
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (==0.1.0a6)
-Requires-Dist: polywrap-manifest (==0.1.0a4)
-Requires-Dist: polywrap-msgpack (==0.1.0a4)
-Requires-Dist: polywrap-result (==0.1.0a4)
+Requires-Dist: polywrap-core (==0.1.0a7)
+Requires-Dist: polywrap-manifest (==0.1.0a7)
+Requires-Dist: polywrap-msgpack (==0.1.0a7)
+Requires-Dist: polywrap-result (==0.1.0a7)
 Requires-Dist: unsync (>=1.4.0,<2.0.0)
 Requires-Dist: wasmtime (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 TODO
```

