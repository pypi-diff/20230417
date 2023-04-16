# Comparing `tmp/sprocket_boxcars_py-0.1.15.tar.gz` & `tmp/sprocket_boxcars_py-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocket_boxcars_py-0.1.15.tar", max compression
+gzip compressed data, was "sprocket_boxcars_py-0.1.16.tar", max compression
```

## Comparing `sprocket_boxcars_py-0.1.15.tar` & `sprocket_boxcars_py-0.1.16.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1052 2023-04-16 06:44:03.383270 sprocket_boxcars_py-0.1.15/LICENSE
--rw-r--r--   0        0        0      721 2023-04-16 21:48:09.905238 sprocket_boxcars_py-0.1.15/README.md
--rw-r--r--   0        0        0      457 2023-04-16 21:54:45.371474 sprocket_boxcars_py-0.1.15/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-16 21:53:58.812169 sprocket_boxcars_py-0.1.15/src/sprocket_boxcars_py/sprocket_boxcars_py/__init__.py
--rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 sprocket_boxcars_py-0.1.15/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-04-16 06:44:03.383270 sprocket_boxcars_py-0.1.16/LICENSE
+-rw-r--r--   0        0        0      721 2023-04-16 21:48:09.905238 sprocket_boxcars_py-0.1.16/README.md
+-rw-r--r--   0        0        0      457 2023-04-16 22:00:16.754767 sprocket_boxcars_py-0.1.16/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-16 21:53:58.812169 sprocket_boxcars_py-0.1.16/src/sprocket_boxcars_py/sprocket_boxcars_py/__init__.py
+-rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 sprocket_boxcars_py-0.1.16/PKG-INFO
```

### Comparing `sprocket_boxcars_py-0.1.15/LICENSE` & `sprocket_boxcars_py-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocket_boxcars_py-0.1.15/README.md` & `sprocket_boxcars_py-0.1.16/README.md`

 * *Files identical despite different names*

### Comparing `sprocket_boxcars_py-0.1.15/PKG-INFO` & `sprocket_boxcars_py-0.1.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocket-boxcars-py
-Version: 0.1.15
+Version: 0.1.16
 Summary: Python bindings for the Rocket League replay parser boxcars.
 Home-page: https://github.com/SprocketBot/boxcars-py
 License: MIT
 Author: Jake Bailey
 Author-email: asaxplayinghorse@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

