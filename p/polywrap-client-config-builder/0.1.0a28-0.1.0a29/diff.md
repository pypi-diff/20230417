# Comparing `tmp/polywrap_client_config_builder-0.1.0a28.tar.gz` & `tmp/polywrap_client_config_builder-0.1.0a29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client_config_builder-0.1.0a28.tar", max compression
+gzip compressed data, was "polywrap_client_config_builder-0.1.0a29.tar", max compression
```

## Comparing `polywrap_client_config_builder-0.1.0a28.tar` & `polywrap_client_config_builder-0.1.0a29.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1400 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/README.md
--rw-r--r--   0        0        0      117 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/__init__.py
--rw-r--r--   0        0        0      309 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/__init__.py
--rw-r--r--   0        0        0     1046 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/base_configure.py
--rw-r--r--   0        0        0     1997 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/env_configure.py
--rw-r--r--   0        0        0     1793 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/interface_configure.py
--rw-r--r--   0        0        0     1626 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/package_configure.py
--rw-r--r--   0        0        0     1510 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/redirect_configure.py
--rw-r--r--   0        0        0      884 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/resolver_configure.py
--rw-r--r--   0        0        0     1605 2023-04-13 19:13:28.770947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/wrapper_configure.py
--rw-r--r--   0        0        0     2885 2023-04-13 19:13:28.774947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/polywrap_client_config_builder.py
--rw-r--r--   0        0        0        0 2023-04-13 19:13:28.774947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/py.typed
--rw-r--r--   0        0        0      164 2023-04-13 19:13:28.774947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/types/__init__.py
--rw-r--r--   0        0        0      542 2023-04-13 19:13:28.774947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/types/build_options.py
--rw-r--r--   0        0        0     1077 2023-04-13 19:13:28.774947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/types/builder_config.py
--rw-r--r--   0        0        0     6793 2023-04-13 19:13:28.774947 polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/types/client_config_builder.py
--rw-r--r--   0        0        0      991 2023-04-13 19:21:28.611240 polywrap_client_config_builder-0.1.0a28/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0a28/PKG-INFO
+-rw-r--r--   0        0        0     1400 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/README.md
+-rw-r--r--   0        0        0      117 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/__init__.py
+-rw-r--r--   0        0        0      309 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/__init__.py
+-rw-r--r--   0        0        0     1046 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/base_configure.py
+-rw-r--r--   0        0        0     1997 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/env_configure.py
+-rw-r--r--   0        0        0     1793 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/interface_configure.py
+-rw-r--r--   0        0        0     1626 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/package_configure.py
+-rw-r--r--   0        0        0     1510 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/redirect_configure.py
+-rw-r--r--   0        0        0      884 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/resolver_configure.py
+-rw-r--r--   0        0        0     1605 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/wrapper_configure.py
+-rw-r--r--   0        0        0     2885 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/polywrap_client_config_builder.py
+-rw-r--r--   0        0        0        0 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/py.typed
+-rw-r--r--   0        0        0      164 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/build_options.py
+-rw-r--r--   0        0        0     1077 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/builder_config.py
+-rw-r--r--   0        0        0     6793 2023-04-17 14:51:11.080563 polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/client_config_builder.py
+-rw-r--r--   0        0        0      991 2023-04-17 14:59:36.146234 polywrap_client_config_builder-0.1.0a29/pyproject.toml
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 polywrap_client_config_builder-0.1.0a29/PKG-INFO
```

### Comparing `polywrap_client_config_builder-0.1.0a28/README.md` & `polywrap_client_config_builder-0.1.0a29/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/base_configure.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/base_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/env_configure.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/env_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/interface_configure.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/interface_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/package_configure.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/package_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/redirect_configure.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/redirect_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/resolver_configure.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/resolver_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/configures/wrapper_configure.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/configures/wrapper_configure.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/polywrap_client_config_builder.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/polywrap_client_config_builder.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/types/build_options.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/build_options.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/types/builder_config.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/builder_config.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/polywrap_client_config_builder/types/client_config_builder.py` & `polywrap_client_config_builder-0.1.0a29/polywrap_client_config_builder/types/client_config_builder.py`

 * *Files identical despite different names*

### Comparing `polywrap_client_config_builder-0.1.0a28/pyproject.toml` & `polywrap_client_config_builder-0.1.0a29/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-client-config-builder"
-version = "0.1.0a28"
+version = "0.1.0a29"
 description = ""
 authors = ["Media <media@polywrap.io>", "Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-uri-resolvers = "^0.1.0a28"
-polywrap-core = "^0.1.0a28"
+polywrap-uri-resolvers = "^0.1.0a29"
+polywrap-core = "^0.1.0a29"
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
```

### Comparing `polywrap_client_config_builder-0.1.0a28/PKG-INFO` & `polywrap_client_config_builder-0.1.0a29/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: polywrap-client-config-builder
-Version: 0.1.0a28
+Version: 0.1.0a29
 Summary: 
 Author: Media
 Author-email: media@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (>=0.1.0a28,<0.2.0)
-Requires-Dist: polywrap-uri-resolvers (>=0.1.0a28,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0a29,<0.2.0)
+Requires-Dist: polywrap-uri-resolvers (>=0.1.0a29,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-client-config-builder
 
 A utility class for building the PolywrapClient config. 
 
 Supports building configs using method chaining or imperatively.
```

