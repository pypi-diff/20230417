# Comparing `tmp/polywrap_plugin-0.1.0a6.tar.gz` & `tmp/polywrap_plugin-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_plugin-0.1.0a6.tar", max compression
+gzip compressed data, was "polywrap_plugin-0.1.0a7.tar", max compression
```

## Comparing `polywrap_plugin-0.1.0a6.tar` & `polywrap_plugin-0.1.0a7.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-03-02 19:49:55.541791 polywrap_plugin-0.1.0a6/README.md
--rw-r--r--   0        0        0       68 2023-03-02 19:49:55.541791 polywrap_plugin-0.1.0a6/polywrap_plugin/__init__.py
--rw-r--r--   0        0        0     1287 2023-03-02 19:49:55.541791 polywrap_plugin-0.1.0a6/polywrap_plugin/module.py
--rw-r--r--   0        0        0      851 2023-03-02 19:49:55.541791 polywrap_plugin-0.1.0a6/polywrap_plugin/package.py
--rw-r--r--   0        0        0     1577 2023-03-02 19:49:55.541791 polywrap_plugin-0.1.0a6/polywrap_plugin/wrapper.py
--rw-r--r--   0        0        0     1061 2023-03-02 19:52:30.350335 polywrap_plugin-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-22 15:57:14.698952 polywrap_plugin-0.1.0a7/README.md
+-rw-r--r--   0        0        0       68 2023-02-22 15:57:14.698831 polywrap_plugin-0.1.0a7/polywrap_plugin/__init__.py
+-rw-r--r--   0        0        0     1287 2023-03-02 12:38:55.321099 polywrap_plugin-0.1.0a7/polywrap_plugin/module.py
+-rw-r--r--   0        0        0      851 2023-03-02 12:38:52.589154 polywrap_plugin-0.1.0a7/polywrap_plugin/package.py
+-rw-r--r--   0        0        0     1577 2023-03-02 17:12:07.060382 polywrap_plugin-0.1.0a7/polywrap_plugin/wrapper.py
+-rw-r--r--   0        0        0     1061 2023-03-02 20:02:49.412858 polywrap_plugin-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0a7/setup.py
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0a7/PKG-INFO
```

### Comparing `polywrap_plugin-0.1.0a6/polywrap_plugin/module.py` & `polywrap_plugin-0.1.0a7/polywrap_plugin/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0a6/polywrap_plugin/package.py` & `polywrap_plugin-0.1.0a7/polywrap_plugin/package.py`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0a6/polywrap_plugin/wrapper.py` & `polywrap_plugin-0.1.0a7/polywrap_plugin/wrapper.py`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0a6/pyproject.toml` & `polywrap_plugin-0.1.0a7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-plugin"
-version = "0.1.0a6"
+version = "0.1.0a7"
 description = "Plugin package"
 authors = ["Cesar <cesar@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap_core = "0.1.0a6"
-polywrap_manifest = "0.1.0a4"
-polywrap_result = "0.1.0a4"
-polywrap_msgpack = "0.1.0a4"
+polywrap_core = "0.1.0a7"
+polywrap_manifest = "0.1.0a7"
+polywrap_result = "0.1.0a7"
+polywrap_msgpack = "0.1.0a7"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
```

### Comparing `polywrap_plugin-0.1.0a6/PKG-INFO` & `polywrap_plugin-0.1.0a7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: polywrap-plugin
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Plugin package
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap_core (==0.1.0a6)
-Requires-Dist: polywrap_manifest (==0.1.0a4)
-Requires-Dist: polywrap_msgpack (==0.1.0a4)
-Requires-Dist: polywrap_result (==0.1.0a4)
+Requires-Dist: polywrap_core (==0.1.0a7)
+Requires-Dist: polywrap_manifest (==0.1.0a7)
+Requires-Dist: polywrap_msgpack (==0.1.0a7)
+Requires-Dist: polywrap_result (==0.1.0a7)
 Description-Content-Type: text/markdown
```

