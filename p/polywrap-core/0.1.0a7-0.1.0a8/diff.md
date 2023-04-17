# Comparing `tmp/polywrap_core-0.1.0a7.tar.gz` & `tmp/polywrap_core-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_core-0.1.0a7.tar", max compression
+gzip compressed data, was "polywrap_core-0.1.0a8.tar", max compression
```

## Comparing `polywrap_core-0.1.0a7.tar` & `polywrap_core-0.1.0a8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       98 2023-02-22 15:57:14.692017 polywrap_core-0.1.0a7/polywrap_core/__init__.py
--rw-r--r--   0        0        0       38 2023-02-22 15:57:14.692337 polywrap_core-0.1.0a7/polywrap_core/algorithms/__init__.py
--rw-r--r--   0        0        0     2392 2023-02-22 15:57:14.692494 polywrap_core-0.1.0a7/polywrap_core/algorithms/build_clean_uri_history.py
--rw-r--r--   0        0        0      360 2023-02-22 15:57:14.692622 polywrap_core-0.1.0a7/polywrap_core/types/__init__.py
--rw-r--r--   0        0        0     1542 2023-02-24 15:43:21.891062 polywrap_core-0.1.0a7/polywrap_core/types/client.py
--rw-r--r--   0        0        0       51 2023-02-22 15:57:14.693626 polywrap_core-0.1.0a7/polywrap_core/types/env.py
--rw-r--r--   0        0        0      231 2023-02-22 15:57:14.693388 polywrap_core-0.1.0a7/polywrap_core/types/file_reader.py
--rw-r--r--   0        0        0     1799 2023-02-24 15:43:21.891664 polywrap_core-0.1.0a7/polywrap_core/types/invoke.py
--rw-r--r--   0        0        0     3475 2023-02-22 15:57:14.693549 polywrap_core-0.1.0a7/polywrap_core/types/uri.py
--rw-r--r--   0        0        0      208 2023-02-24 15:43:21.891172 polywrap_core-0.1.0a7/polywrap_core/types/uri_package_wrapper.py
--rw-r--r--   0        0        0      913 2023-02-22 15:57:14.693710 polywrap_core-0.1.0a7/polywrap_core/types/uri_resolution_context.py
--rw-r--r--   0        0        0      479 2023-02-22 15:57:14.694476 polywrap_core-0.1.0a7/polywrap_core/types/uri_resolution_step.py
--rw-r--r--   0        0        0     1086 2023-02-24 15:43:21.891479 polywrap_core-0.1.0a7/polywrap_core/types/uri_resolver.py
--rw-r--r--   0        0        0      446 2023-02-22 15:57:14.694185 polywrap_core-0.1.0a7/polywrap_core/types/uri_resolver_handler.py
--rw-r--r--   0        0        0      240 2023-02-22 15:57:14.694258 polywrap_core-0.1.0a7/polywrap_core/types/wasm_package.py
--rw-r--r--   0        0        0      485 2023-02-24 15:43:21.891784 polywrap_core-0.1.0a7/polywrap_core/types/wrap_package.py
--rw-r--r--   0        0        0      900 2023-02-24 15:43:21.892094 polywrap_core-0.1.0a7/polywrap_core/types/wrapper.py
--rw-r--r--   0        0        0       38 2023-02-22 15:57:14.694627 polywrap_core-0.1.0a7/polywrap_core/uri_resolution/__init__.py
--rw-r--r--   0        0        0     1675 2022-12-09 10:57:58.160601 polywrap_core-0.1.0a7/polywrap_core/uri_resolution/uri_resolution_context.py
--rw-r--r--   0        0        0      122 2022-12-10 08:39:18.501105 polywrap_core-0.1.0a7/polywrap_core/utils/__init__.py
--rw-r--r--   0        0        0      254 2023-02-22 15:57:14.694748 polywrap_core-0.1.0a7/polywrap_core/utils/get_env_from_uri_history.py
--rw-r--r--   0        0        0      246 2022-12-09 10:18:25.573666 polywrap_core-0.1.0a7/polywrap_core/utils/init_wrapper.py
--rw-r--r--   0        0        0      125 2022-10-16 06:28:28.766955 polywrap_core-0.1.0a7/polywrap_core/utils/instance_of.py
--rw-r--r--   0        0        0      438 2022-10-16 06:28:28.767147 polywrap_core-0.1.0a7/polywrap_core/utils/maybe_async.py
--rw-r--r--   0        0        0     1064 2023-03-02 20:01:18.751492 polywrap_core-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 polywrap_core-0.1.0a7/setup.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 polywrap_core-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0       98 2023-02-22 15:57:14.692017 polywrap_core-0.1.0a8/polywrap_core/__init__.py
+-rw-r--r--   0        0        0       38 2023-02-22 15:57:14.692337 polywrap_core-0.1.0a8/polywrap_core/algorithms/__init__.py
+-rw-r--r--   0        0        0     2392 2023-02-22 15:57:14.692494 polywrap_core-0.1.0a8/polywrap_core/algorithms/build_clean_uri_history.py
+-rw-r--r--   0        0        0      360 2023-02-22 15:57:14.692622 polywrap_core-0.1.0a8/polywrap_core/types/__init__.py
+-rw-r--r--   0        0        0     1542 2023-02-24 15:43:21.891062 polywrap_core-0.1.0a8/polywrap_core/types/client.py
+-rw-r--r--   0        0        0       51 2023-02-22 15:57:14.693626 polywrap_core-0.1.0a8/polywrap_core/types/env.py
+-rw-r--r--   0        0        0      231 2023-02-22 15:57:14.693388 polywrap_core-0.1.0a8/polywrap_core/types/file_reader.py
+-rw-r--r--   0        0        0     1799 2023-02-24 15:43:21.891664 polywrap_core-0.1.0a8/polywrap_core/types/invoke.py
+-rw-r--r--   0        0        0     3475 2023-02-22 15:57:14.693549 polywrap_core-0.1.0a8/polywrap_core/types/uri.py
+-rw-r--r--   0        0        0      208 2023-02-24 15:43:21.891172 polywrap_core-0.1.0a8/polywrap_core/types/uri_package_wrapper.py
+-rw-r--r--   0        0        0      913 2023-02-22 15:57:14.693710 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolution_context.py
+-rw-r--r--   0        0        0      479 2023-02-22 15:57:14.694476 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolution_step.py
+-rw-r--r--   0        0        0     1086 2023-02-24 15:43:21.891479 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolver.py
+-rw-r--r--   0        0        0      446 2023-02-22 15:57:14.694185 polywrap_core-0.1.0a8/polywrap_core/types/uri_resolver_handler.py
+-rw-r--r--   0        0        0      240 2023-02-22 15:57:14.694258 polywrap_core-0.1.0a8/polywrap_core/types/wasm_package.py
+-rw-r--r--   0        0        0      485 2023-02-24 15:43:21.891784 polywrap_core-0.1.0a8/polywrap_core/types/wrap_package.py
+-rw-r--r--   0        0        0      900 2023-02-24 15:43:21.892094 polywrap_core-0.1.0a8/polywrap_core/types/wrapper.py
+-rw-r--r--   0        0        0       38 2023-02-22 15:57:14.694627 polywrap_core-0.1.0a8/polywrap_core/uri_resolution/__init__.py
+-rw-r--r--   0        0        0     1675 2022-12-09 10:57:58.160601 polywrap_core-0.1.0a8/polywrap_core/uri_resolution/uri_resolution_context.py
+-rw-r--r--   0        0        0      122 2022-12-10 08:39:18.501105 polywrap_core-0.1.0a8/polywrap_core/utils/__init__.py
+-rw-r--r--   0        0        0      254 2023-02-22 15:57:14.694748 polywrap_core-0.1.0a8/polywrap_core/utils/get_env_from_uri_history.py
+-rw-r--r--   0        0        0      246 2022-12-09 10:18:25.573666 polywrap_core-0.1.0a8/polywrap_core/utils/init_wrapper.py
+-rw-r--r--   0        0        0      125 2022-10-16 06:28:28.766955 polywrap_core-0.1.0a8/polywrap_core/utils/instance_of.py
+-rw-r--r--   0        0        0      438 2022-10-16 06:28:28.767147 polywrap_core-0.1.0a8/polywrap_core/utils/maybe_async.py
+-rw-r--r--   0        0        0     1064 2023-03-02 20:07:34.919806 polywrap_core-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 polywrap_core-0.1.0a8/setup.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 polywrap_core-0.1.0a8/PKG-INFO
```

### Comparing `polywrap_core-0.1.0a7/polywrap_core/algorithms/build_clean_uri_history.py` & `polywrap_core-0.1.0a8/polywrap_core/algorithms/build_clean_uri_history.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/polywrap_core/types/client.py` & `polywrap_core-0.1.0a8/polywrap_core/types/client.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/polywrap_core/types/invoke.py` & `polywrap_core-0.1.0a8/polywrap_core/types/invoke.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/polywrap_core/types/uri.py` & `polywrap_core-0.1.0a8/polywrap_core/types/uri.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/polywrap_core/types/uri_resolution_context.py` & `polywrap_core-0.1.0a8/polywrap_core/types/uri_resolution_context.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/polywrap_core/types/uri_resolver.py` & `polywrap_core-0.1.0a8/polywrap_core/types/uri_resolver.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/polywrap_core/types/wrapper.py` & `polywrap_core-0.1.0a8/polywrap_core/types/wrapper.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/polywrap_core/uri_resolution/uri_resolution_context.py` & `polywrap_core-0.1.0a8/polywrap_core/uri_resolution/uri_resolution_context.py`

 * *Files identical despite different names*

### Comparing `polywrap_core-0.1.0a7/pyproject.toml` & `polywrap_core-0.1.0a8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-core"
-version = "0.1.0a7"
+version = "0.1.0a8"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 gql = "3.4.0"
 graphql-core = "^3.2.1"
```

### Comparing `polywrap_core-0.1.0a7/setup.py` & `polywrap_core-0.1.0a8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'graphql-core>=3.2.1,<4.0.0',
  'polywrap-manifest==0.1.0a7',
  'polywrap-result==0.1.0a7',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'polywrap-core',
-    'version': '0.1.0a7',
+    'version': '0.1.0a8',
     'description': '',
     'long_description': 'None',
     'author': 'Cesar',
     'author_email': 'cesar@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

