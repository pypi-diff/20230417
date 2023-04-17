# Comparing `tmp/bitmap2-0.1.1.tar.gz` & `tmp/bitmap2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmap2-0.1.1.tar", last modified: Fri Nov  4 02:21:39 2022, max compression
+gzip compressed data, was "bitmap2-0.2.0.tar", last modified: Mon Apr 17 20:19:19 2023, max compression
```

## Comparing `bitmap2-0.1.1.tar` & `bitmap2-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 02:21:39.101546 bitmap2-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 02:21:39.101546 bitmap2-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 02:21:39.101546 bitmap2-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-11-04 02:21:31.000000 bitmap2-0.1.1/.github/workflows/pypi-upload.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-11-04 02:21:31.000000 bitmap2-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-11-04 02:21:31.000000 bitmap2-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-11-04 02:21:31.000000 bitmap2-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-04 02:21:31.000000 bitmap2-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-11-04 02:21:39.101546 bitmap2-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-11-04 02:21:31.000000 bitmap2-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 02:21:39.101546 bitmap2-0.1.1/bitmap2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-11-04 02:21:39.000000 bitmap2-0.1.1/bitmap2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-11-04 02:21:39.000000 bitmap2-0.1.1/bitmap2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 02:21:39.000000 bitmap2-0.1.1/bitmap2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-04 02:21:39.000000 bitmap2-0.1.1/bitmap2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 02:21:39.101546 bitmap2-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1130 2022-11-04 02:21:31.000000 bitmap2-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 02:21:39.101546 bitmap2-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-04 02:21:31.000000 bitmap2-0.1.1/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5347 2022-11-04 02:21:31.000000 bitmap2-0.1.1/src/bitmap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 02:21:39.101546 bitmap2-0.1.1/test/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3088 2022-11-04 02:21:31.000000 bitmap2-0.1.1/test/test_bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-17 20:19:14.000000 bitmap2-0.2.0/.github/workflows/pypi-upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-17 20:19:14.000000 bitmap2-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-17 20:19:14.000000 bitmap2-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-17 20:19:14.000000 bitmap2-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-17 20:19:14.000000 bitmap2-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-17 20:19:19.954870 bitmap2-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-17 20:19:14.000000 bitmap2-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/bitmap2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 20:19:19.000000 bitmap2-0.2.0/bitmap2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:19:19.954870 bitmap2-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-04-17 20:19:14.000000 bitmap2-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 20:19:14.000000 bitmap2-0.2.0/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6425 2023-04-17 20:19:14.000000 bitmap2-0.2.0/src/bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:19:19.954870 bitmap2-0.2.0/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-04-17 20:19:14.000000 bitmap2-0.2.0/test/test_bitmap.py
```

### Comparing `bitmap2-0.1.1/.github/workflows/pypi-upload.yml` & `bitmap2-0.2.0/.github/workflows/pypi-upload.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.1.1/.github/workflows/test.yml` & `bitmap2-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.1.1/.gitignore` & `bitmap2-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bitmap2-0.1.1/LICENSE.md` & `bitmap2-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.1.1/PKG-INFO` & `bitmap2-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.1.1
+Version: 0.2.0
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.1.1/README.md` & `bitmap2-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.1.1/bitmap2.egg-info/PKG-INFO` & `bitmap2-0.2.0/bitmap2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.1.1
+Version: 0.2.0
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.1.1/setup.py` & `bitmap2-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `bitmap2-0.1.1/test/test_bitmap.py` & `bitmap2-0.2.0/test/test_bitmap.py`

 * *Files identical despite different names*

