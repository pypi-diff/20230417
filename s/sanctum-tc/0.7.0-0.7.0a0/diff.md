# Comparing `tmp/sanctum_tc-0.7.0.tar.gz` & `tmp/sanctum_tc-0.7.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctum_tc-0.7.0.tar", max compression
+gzip compressed data, was "sanctum_tc-0.7.0a0.tar", max compression
```

## Comparing `sanctum_tc-0.7.0.tar` & `sanctum_tc-0.7.0a0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2022-02-18 23:50:37.218899 sanctum_tc-0.7.0/LICENSE
--rw-r--r--   0        0        0      453 2023-04-17 14:58:48.709389 sanctum_tc-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 14:56:36.673483 sanctum_tc-0.7.0/sanctum/__init__.py
--rw-r--r--   0        0        0     6747 2023-04-11 03:12:34.810765 sanctum_tc-0.7.0/sanctum/client.py
--rw-r--r--   0        0        0      517 2022-09-28 14:35:56.064447 sanctum_tc-0.7.0/sanctum/exceptions.py
--rw-r--r--   0        0        0      284 2022-02-25 04:15:29.285866 sanctum_tc-0.7.0/sanctum/utils.py
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 sanctum_tc-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-02-18 23:50:37.218899 sanctum_tc-0.7.0a0/LICENSE
+-rw-r--r--   0        0        0      455 2023-04-17 14:56:47.813419 sanctum_tc-0.7.0a0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 14:56:36.673483 sanctum_tc-0.7.0a0/sanctum/__init__.py
+-rw-r--r--   0        0        0     6747 2023-04-11 03:12:34.810765 sanctum_tc-0.7.0a0/sanctum/client.py
+-rw-r--r--   0        0        0      517 2022-09-28 14:35:56.064447 sanctum_tc-0.7.0a0/sanctum/exceptions.py
+-rw-r--r--   0        0        0      284 2022-02-25 04:15:29.285866 sanctum_tc-0.7.0a0/sanctum/utils.py
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 sanctum_tc-0.7.0a0/PKG-INFO
```

### Comparing `sanctum_tc-0.7.0/LICENSE` & `sanctum_tc-0.7.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanctum_tc-0.7.0/sanctum/client.py` & `sanctum_tc-0.7.0a0/sanctum/client.py`

 * *Files identical despite different names*

### Comparing `sanctum_tc-0.7.0/sanctum/exceptions.py` & `sanctum_tc-0.7.0a0/sanctum/exceptions.py`

 * *Files identical despite different names*

### Comparing `sanctum_tc-0.7.0/PKG-INFO` & `sanctum_tc-0.7.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctum-tc
-Version: 0.7.0
+Version: 0.7.0a0
 Summary: Library for interacting with the Sanctum API
 License: MIT
 Author: LightSage
 Author-email: lightsage01@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

