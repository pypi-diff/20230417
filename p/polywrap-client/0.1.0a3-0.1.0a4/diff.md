# Comparing `tmp/polywrap_client-0.1.0a3.tar.gz` & `tmp/polywrap_client-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client-0.1.0a3.tar", max compression
+gzip compressed data, was "polywrap_client-0.1.0a4.tar", max compression
```

## Comparing `polywrap_client-0.1.0a3.tar` & `polywrap_client-0.1.0a4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        4 2023-02-23 14:37:25.309311 polywrap_client-0.1.0a3/README.md
--rw-r--r--   0        0        0       22 2023-02-23 14:37:25.309311 polywrap_client-0.1.0a3/polywrap_client/__init__.py
--rw-r--r--   0        0        0     5313 2023-02-23 14:37:25.309311 polywrap_client-0.1.0a3/polywrap_client/client.py
--rw-r--r--   0        0        0     1283 2023-02-23 14:44:47.817084 polywrap_client-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a3/setup.py
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0        4 2023-02-24 13:52:49.839099 polywrap_client-0.1.0a4/README.md
+-rw-r--r--   0        0        0       22 2023-02-24 13:52:49.843099 polywrap_client-0.1.0a4/polywrap_client/__init__.py
+-rw-r--r--   0        0        0     5313 2023-02-24 13:52:49.843099 polywrap_client-0.1.0a4/polywrap_client/client.py
+-rw-r--r--   0        0        0     1283 2023-02-24 14:00:34.812101 polywrap_client-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a4/setup.py
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a4/PKG-INFO
```

### Comparing `polywrap_client-0.1.0a3/polywrap_client/client.py` & `polywrap_client-0.1.0a4/polywrap_client/client.py`

 * *Files identical despite different names*

### Comparing `polywrap_client-0.1.0a3/pyproject.toml` & `polywrap_client-0.1.0a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-client"
-version = "0.1.0a3"
+version = "0.1.0a4"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 wasmtime = "^1.0.1"
 unsync = "^1.4.0"
-polywrap-core = "0.1.0a3"
-polywrap-msgpack = "0.1.0a3"
-polywrap-manifest = "0.1.0a3"
-polywrap-result = "0.1.0a3"
-polywrap-uri-resolvers = "0.1.0a3"
+polywrap-core = "0.1.0a4"
+polywrap-msgpack = "0.1.0a4"
+polywrap-manifest = "0.1.0a4"
+polywrap-result = "0.1.0a4"
+polywrap-uri-resolvers = "0.1.0a4"
 result = "^0.8.0"
 pysha3 = "^1.0.2"
 pycryptodome = "^3.14.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
```

### Comparing `polywrap_client-0.1.0a3/setup.py` & `polywrap_client-0.1.0a4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 packages = \
 ['polywrap_client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['polywrap-core==0.1.0a3',
- 'polywrap-manifest==0.1.0a3',
- 'polywrap-msgpack==0.1.0a3',
- 'polywrap-result==0.1.0a3',
- 'polywrap-uri-resolvers==0.1.0a3',
+['polywrap-core==0.1.0a4',
+ 'polywrap-manifest==0.1.0a4',
+ 'polywrap-msgpack==0.1.0a4',
+ 'polywrap-result==0.1.0a4',
+ 'polywrap-uri-resolvers==0.1.0a4',
  'pycryptodome>=3.14.1,<4.0.0',
  'pysha3>=1.0.2,<2.0.0',
  'result>=0.8.0,<0.9.0',
  'unsync>=1.4.0,<2.0.0',
  'wasmtime>=1.0.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'polywrap-client',
-    'version': '0.1.0a3',
+    'version': '0.1.0a4',
     'description': '',
     'long_description': 'TODO',
     'author': 'Cesar',
     'author_email': 'cesar@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `polywrap_client-0.1.0a3/PKG-INFO` & `polywrap_client-0.1.0a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: polywrap-client
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: 
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (==0.1.0a3)
-Requires-Dist: polywrap-manifest (==0.1.0a3)
-Requires-Dist: polywrap-msgpack (==0.1.0a3)
-Requires-Dist: polywrap-result (==0.1.0a3)
-Requires-Dist: polywrap-uri-resolvers (==0.1.0a3)
+Requires-Dist: polywrap-core (==0.1.0a4)
+Requires-Dist: polywrap-manifest (==0.1.0a4)
+Requires-Dist: polywrap-msgpack (==0.1.0a4)
+Requires-Dist: polywrap-result (==0.1.0a4)
+Requires-Dist: polywrap-uri-resolvers (==0.1.0a4)
 Requires-Dist: pycryptodome (>=3.14.1,<4.0.0)
 Requires-Dist: pysha3 (>=1.0.2,<2.0.0)
 Requires-Dist: result (>=0.8.0,<0.9.0)
 Requires-Dist: unsync (>=1.4.0,<2.0.0)
 Requires-Dist: wasmtime (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
```

