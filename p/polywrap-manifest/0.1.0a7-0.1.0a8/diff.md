# Comparing `tmp/polywrap_manifest-0.1.0a7.tar.gz` & `tmp/polywrap_manifest-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_manifest-0.1.0a7.tar", max compression
+gzip compressed data, was "polywrap_manifest-0.1.0a8.tar", max compression
```

## Comparing `polywrap_manifest-0.1.0a7.tar` & `polywrap_manifest-0.1.0a8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-02-22 15:57:14.696500 polywrap_manifest-0.1.0a7/README.md
--rw-r--r--   0        0        0       51 2023-02-22 15:57:14.696015 polywrap_manifest-0.1.0a7/polywrap_manifest/__init__.py
--rw-r--r--   0        0        0     1690 2023-02-22 15:57:14.696334 polywrap_manifest-0.1.0a7/polywrap_manifest/deserialize.py
--rw-r--r--   0        0        0     1251 2023-02-22 15:57:14.696418 polywrap_manifest-0.1.0a7/polywrap_manifest/manifest.py
--rw-r--r--   0        0        0     6053 2023-02-22 15:57:14.696732 polywrap_manifest-0.1.0a7/polywrap_manifest/wrap_0_1.py
--rw-r--r--   0        0        0     1114 2023-03-02 20:00:48.195349 polywrap_manifest-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 polywrap_manifest-0.1.0a7/setup.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 polywrap_manifest-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-22 15:57:14.696500 polywrap_manifest-0.1.0a8/README.md
+-rw-r--r--   0        0        0       51 2023-02-22 15:57:14.696015 polywrap_manifest-0.1.0a8/polywrap_manifest/__init__.py
+-rw-r--r--   0        0        0     1690 2023-02-22 15:57:14.696334 polywrap_manifest-0.1.0a8/polywrap_manifest/deserialize.py
+-rw-r--r--   0        0        0     1251 2023-02-22 15:57:14.696418 polywrap_manifest-0.1.0a8/polywrap_manifest/manifest.py
+-rw-r--r--   0        0        0     6053 2023-02-22 15:57:14.696732 polywrap_manifest-0.1.0a8/polywrap_manifest/wrap_0_1.py
+-rw-r--r--   0        0        0     1114 2023-03-02 20:07:15.378985 polywrap_manifest-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 polywrap_manifest-0.1.0a8/setup.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 polywrap_manifest-0.1.0a8/PKG-INFO
```

### Comparing `polywrap_manifest-0.1.0a7/polywrap_manifest/deserialize.py` & `polywrap_manifest-0.1.0a8/polywrap_manifest/deserialize.py`

 * *Files identical despite different names*

### Comparing `polywrap_manifest-0.1.0a7/polywrap_manifest/manifest.py` & `polywrap_manifest-0.1.0a8/polywrap_manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `polywrap_manifest-0.1.0a7/polywrap_manifest/wrap_0_1.py` & `polywrap_manifest-0.1.0a8/polywrap_manifest/wrap_0_1.py`

 * *Files identical despite different names*

### Comparing `polywrap_manifest-0.1.0a7/pyproject.toml` & `polywrap_manifest-0.1.0a8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-manifest"
-version = "0.1.0a7"
+version = "0.1.0a8"
 description = "WRAP manifest"
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 polywrap-msgpack = "0.1.0a7"
```

### Comparing `polywrap_manifest-0.1.0a7/setup.py` & `polywrap_manifest-0.1.0a8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['polywrap-msgpack==0.1.0a7',
  'polywrap-result==0.1.0a7',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'polywrap-manifest',
-    'version': '0.1.0a7',
+    'version': '0.1.0a8',
     'description': 'WRAP manifest',
     'long_description': '',
     'author': 'Niraj',
     'author_email': 'niraj@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

