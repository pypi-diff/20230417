# Comparing `tmp/bodo_platform_utils-0.0.7.tar.gz` & `tmp/bodo_platform_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodo_platform_utils-0.0.7.tar", last modified: Wed Apr 12 19:38:18 2023, max compression
+gzip compressed data, was "bodo_platform_utils-0.0.8.tar", last modified: Mon Apr 17 17:38:03 2023, max compression
```

## Comparing `bodo_platform_utils-0.0.7.tar` & `bodo_platform_utils-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/bodo_platform_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/bodo_platform_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/bodo_platform_utils/utils_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 19:38:18.000000 bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-12 19:38:18.529388 bodo_platform_utils-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-12 19:36:58.000000 bodo_platform_utils-0.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/bodo_platform_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/bodo_platform_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/bodosqlwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/bodo_platform_utils/utils_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 17:38:03.000000 bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-17 17:38:03.881700 bodo_platform_utils-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-17 17:36:28.000000 bodo_platform_utils-0.0.8/versioneer.py
```

### Comparing `bodo_platform_utils-0.0.7/LICENSE` & `bodo_platform_utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.7/PKG-INFO` & `bodo_platform_utils-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodo_platform_utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.0.7/bodo_platform_utils/catalog.py` & `bodo_platform_utils-0.0.8/bodo_platform_utils/catalog.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # where it’ll be called every time the SQL cell is executed.
 # To reduce this cost, we set up a simple in-memory TTL cache on this function.
 @cached(
     cache=TTLCache(
         maxsize=256,
         ttl=3600,
     ),
-    key=lambda name, _parallel: hashkey(name, _parallel),
+    key=lambda name=None, _parallel=True: hashkey(name, _parallel),
 )
 def get_data(name=None, _parallel=True):
     """
      :param name: Name of the Catalog
      :param _parallel: Defaults to True
     :return: JSON object containing the Catalog data
     """
```

### Comparing `bodo_platform_utils-0.0.7/bodo_platform_utils/config.py` & `bodo_platform_utils-0.0.8/bodo_platform_utils/config.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.7/bodo_platform_utils/secrets.py` & `bodo_platform_utils-0.0.8/bodo_platform_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.7/bodo_platform_utils.egg-info/PKG-INFO` & `bodo_platform_utils-0.0.8/bodo_platform_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodo-platform-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: This is package contains utility functions to retrieve data from Cloud Providers for platform
 Home-page: https://github.com/Bodo-inc/bodo-platform-utils
 Author: Bodo Inc
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodo_platform_utils-0.0.7/setup.py` & `bodo_platform_utils-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `bodo_platform_utils-0.0.7/versioneer.py` & `bodo_platform_utils-0.0.8/versioneer.py`

 * *Files identical despite different names*

