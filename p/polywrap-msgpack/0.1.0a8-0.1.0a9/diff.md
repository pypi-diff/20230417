# Comparing `tmp/polywrap_msgpack-0.1.0a8.tar.gz` & `tmp/polywrap_msgpack-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_msgpack-0.1.0a8.tar", max compression
+gzip compressed data, was "polywrap_msgpack-0.1.0a9.tar", max compression
```

## Comparing `polywrap_msgpack-0.1.0a8.tar` & `polywrap_msgpack-0.1.0a9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2022-10-16 06:28:28.670104 polywrap_msgpack-0.1.0a8/README.md
--rw-r--r--   0        0        0     3467 2023-03-02 19:36:47.836502 polywrap_msgpack-0.1.0a8/polywrap_msgpack/__init__.py
--rw-r--r--   0        0        0      643 2023-03-02 19:01:29.239002 polywrap_msgpack-0.1.0a8/polywrap_msgpack/generic_map.py
--rw-r--r--   0        0        0     1004 2023-03-02 20:06:41.226722 polywrap_msgpack-0.1.0a8/pyproject.toml
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0a8/setup.py
--rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0a8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-16 06:28:28.670104 polywrap_msgpack-0.1.0a9/README.md
+-rw-r--r--   0        0        0     3467 2023-03-02 19:36:47.836502 polywrap_msgpack-0.1.0a9/polywrap_msgpack/__init__.py
+-rw-r--r--   0        0        0      643 2023-03-02 19:01:29.239002 polywrap_msgpack-0.1.0a9/polywrap_msgpack/generic_map.py
+-rw-r--r--   0        0        0     1004 2023-03-02 20:08:58.642060 polywrap_msgpack-0.1.0a9/pyproject.toml
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0a9/setup.py
+-rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0a9/PKG-INFO
```

### Comparing `polywrap_msgpack-0.1.0a8/polywrap_msgpack/__init__.py` & `polywrap_msgpack-0.1.0a9/polywrap_msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0a8/polywrap_msgpack/generic_map.py` & `polywrap_msgpack-0.1.0a9/polywrap_msgpack/generic_map.py`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0a8/pyproject.toml` & `polywrap_msgpack-0.1.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-msgpack"
-version = "0.1.0a8"
+version = "0.1.0a9"
 description = "WRAP msgpack encoding"
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 msgpack = "^1.0.4"
```

### Comparing `polywrap_msgpack-0.1.0a8/setup.py` & `polywrap_msgpack-0.1.0a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['msgpack>=1.0.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'polywrap-msgpack',
-    'version': '0.1.0a8',
+    'version': '0.1.0a9',
     'description': 'WRAP msgpack encoding',
     'long_description': '',
     'author': 'Cesar',
     'author_email': 'cesar@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

