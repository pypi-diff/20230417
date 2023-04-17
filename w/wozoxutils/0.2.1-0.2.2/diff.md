# Comparing `tmp/wozoxutils-0.2.1.tar.gz` & `tmp/wozoxutils-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wozoxutils-0.2.1.tar", last modified: Mon Apr 17 12:52:43 2023, max compression
+gzip compressed data, was "wozoxutils-0.2.2.tar", last modified: Mon Apr 17 13:00:07 2023, max compression
```

## Comparing `wozoxutils-0.2.1.tar` & `wozoxutils-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:52:43.520092 wozoxutils-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 12:52:33.000000 wozoxutils-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-17 12:52:43.520092 wozoxutils-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-17 12:52:33.000000 wozoxutils-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:52:43.520092 wozoxutils-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 12:52:33.000000 wozoxutils-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:52:43.520092 wozoxutils-0.2.1/wozoxutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:52:33.000000 wozoxutils-0.2.1/wozoxutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 12:52:33.000000 wozoxutils-0.2.1/wozoxutils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-17 12:52:33.000000 wozoxutils-0.2.1/wozoxutils/hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:52:43.520092 wozoxutils-0.2.1/wozoxutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-17 12:52:43.000000 wozoxutils-0.2.1/wozoxutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-17 12:52:43.000000 wozoxutils-0.2.1/wozoxutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:52:43.000000 wozoxutils-0.2.1/wozoxutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 12:52:43.000000 wozoxutils-0.2.1/wozoxutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:00:07.070633 wozoxutils-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 12:59:55.000000 wozoxutils-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-17 13:00:07.070633 wozoxutils-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-17 12:59:55.000000 wozoxutils-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:00:07.070633 wozoxutils-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-17 12:59:55.000000 wozoxutils-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:00:07.070633 wozoxutils-0.2.2/wozoxutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 12:59:55.000000 wozoxutils-0.2.2/wozoxutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 12:59:55.000000 wozoxutils-0.2.2/wozoxutils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-17 12:59:55.000000 wozoxutils-0.2.2/wozoxutils/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:00:07.070633 wozoxutils-0.2.2/wozoxutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-17 13:00:07.000000 wozoxutils-0.2.2/wozoxutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-17 13:00:07.000000 wozoxutils-0.2.2/wozoxutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:00:07.000000 wozoxutils-0.2.2/wozoxutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 13:00:07.000000 wozoxutils-0.2.2/wozoxutils.egg-info/top_level.txt
```

### Comparing `wozoxutils-0.2.1/LICENSE` & `wozoxutils-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.1/PKG-INFO` & `wozoxutils-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wozoxutils
-Version: 0.2.1
+Version: 0.2.2
 Summary: general-purpose library for Python that contains various commonly used functional modules
 Home-page: https://github.com/wozox/wozoxutils-py
 Author: illiten
 Author-email: admin@leelib.com
 Keywords: wozox utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wozoxutils-0.2.1/setup.py` & `wozoxutils-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name="wozoxutils",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     install_requires=[],  # 添加依赖包
     author="illiten",
     author_email="admin@leelib.com",
     description="general-purpose library for Python that contains various commonly used functional modules",
     url="https://github.com/wozox/wozoxutils-py",
     long_description=long_description,
```

### Comparing `wozoxutils-0.2.1/wozoxutils/file.py` & `wozoxutils-0.2.2/wozoxutils/file.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.1/wozoxutils/hash.py` & `wozoxutils-0.2.2/wozoxutils/hash.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.1/wozoxutils.egg-info/PKG-INFO` & `wozoxutils-0.2.2/wozoxutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wozoxutils
-Version: 0.2.1
+Version: 0.2.2
 Summary: general-purpose library for Python that contains various commonly used functional modules
 Home-page: https://github.com/wozox/wozoxutils-py
 Author: illiten
 Author-email: admin@leelib.com
 Keywords: wozox utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

