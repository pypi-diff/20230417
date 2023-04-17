# Comparing `tmp/headscale_api-0.1.3.tar.gz` & `tmp/headscale_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headscale_api-0.1.3.tar", max compression
+gzip compressed data, was "headscale_api-0.1.4.tar", max compression
```

## Comparing `headscale_api-0.1.3.tar` & `headscale_api-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-04-14 01:20:03.795404 headscale_api-0.1.3/LICENSE
--rw-r--r--   0        0        0       68 2023-04-14 01:20:03.795404 headscale_api-0.1.3/README.md
--rw-r--r--   0        0        0      537 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/__init__.py
--rw-r--r--   0        0        0      428 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/config.py
--rw-r--r--   0        0        0     9775 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/endpoints.py
--rw-r--r--   0        0        0     7084 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/headscale.py
--rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/py.typed
--rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/__init__.py
--rw-r--r--   0        0        0     3967 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/config.py
--rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/google/__init__.py
--rw-r--r--   0        0        0    15302 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/google/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/headscale/__init__.py
--rw-r--r--   0        0        0    48177 2023-04-14 01:20:03.795404 headscale_api-0.1.3/headscale_api/schema/headscale/v1/__init__.py
--rw-r--r--   0        0        0     1684 2023-04-14 01:20:03.795404 headscale_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-17 12:42:47.464949 headscale_api-0.1.4/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-17 12:42:47.464949 headscale_api-0.1.4/README.md
+-rw-r--r--   0        0        0      537 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/config.py
+-rw-r--r--   0        0        0     9775 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/endpoints.py
+-rw-r--r--   0        0        0     7084 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/headscale.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/py.typed
+-rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/__init__.py
+-rw-r--r--   0        0        0     3967 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/config.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/google/__init__.py
+-rw-r--r--   0        0        0    15302 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/headscale/__init__.py
+-rw-r--r--   0        0        0    48177 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/headscale/v1/__init__.py
+-rw-r--r--   0        0        0     1887 2023-04-17 12:42:47.464949 headscale_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.4/PKG-INFO
```

### Comparing `headscale_api-0.1.3/LICENSE` & `headscale_api-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.3/headscale_api/__init__.py` & `headscale_api-0.1.4/headscale_api/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.3/headscale_api/endpoints.py` & `headscale_api-0.1.4/headscale_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.3/headscale_api/headscale.py` & `headscale_api-0.1.4/headscale_api/headscale.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.3/headscale_api/schema/config.py` & `headscale_api-0.1.4/headscale_api/schema/config.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.3/headscale_api/schema/google/api/__init__.py` & `headscale_api-0.1.4/headscale_api/schema/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.3/headscale_api/schema/headscale/v1/__init__.py` & `headscale_api-0.1.4/headscale_api/schema/headscale/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.3/pyproject.toml` & `headscale_api-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "headscale-api"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python Headscale API and configuration abstraction."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -40,14 +40,18 @@
 pyyaml = "^6.0"
 pytest-cov = "^4.0.0"
 pylint-pytest = "^1.1.2"
 
 [tool.poetry.group.gen.dependencies]
 datamodel-code-generator = "^0.17.2"
 
+[tool.poetry.group.dev.dependencies]
+# Add direct dependency only for development.
+betterproto = {git = "https://github.com/danielgtaylor/python-betterproto.git", rev = "master", extras = ["compiler"]}
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 skip_glob = ["headscale_api/schema"]
```

### Comparing `headscale_api-0.1.3/PKG-INFO` & `headscale_api-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headscale-api
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Headscale API and configuration abstraction.
 Home-page: https://github.com/MarekPikula/python-headscale-api
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
```

