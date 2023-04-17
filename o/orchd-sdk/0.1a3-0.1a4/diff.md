# Comparing `tmp/orchd-sdk-0.1a3.tar.gz` & `tmp/orchd-sdk-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchd-sdk-0.1a3.tar", last modified: Fri Apr 14 14:58:35 2023, max compression
+gzip compressed data, was "orchd-sdk-0.1a4.tar", last modified: Mon Apr 17 15:14:56 2023, max compression
```

## Comparing `orchd-sdk-0.1a3.tar` & `orchd-sdk-0.1a4.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.389757 orchd-sdk-0.1a3/
--rw-r--r--   0 mathias    (501) staff       (20)     1097 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/LICENSE.md
--rw-r--r--   0 mathias    (501) staff       (20)      704 2023-04-14 14:58:35.389617 orchd-sdk-0.1a3/PKG-INFO
--rw-r--r--   0 mathias    (501) staff       (20)     1256 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/README.md
--rw-r--r--   0 mathias    (501) staff       (20)       38 2023-04-14 14:58:35.389804 orchd-sdk-0.1a3/setup.cfg
--rw-r--r--   0 mathias    (501) staff       (20)     2587 2023-04-07 08:22:35.000000 orchd-sdk-0.1a3/setup.py
-drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.385676 orchd-sdk-0.1a3/src/
-drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.387824 orchd-sdk-0.1a3/src/orchd_sdk/
--rw-r--r--   0 mathias    (501) staff       (20)       10 2023-04-14 13:36:21.000000 orchd-sdk-0.1a3/src/orchd_sdk/VERSION
--rw-r--r--   0 mathias    (501) staff       (20)     1324 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/__init__.py
-drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.389430 orchd-sdk-0.1a3/src/orchd_sdk/api/
--rw-r--r--   0 mathias    (501) staff       (20)     2463 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/__init__.py
--rw-r--r--   0 mathias    (501) staff       (20)      575 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/events.py
--rw-r--r--   0 mathias    (501) staff       (20)     2264 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/reactions.py
--rw-r--r--   0 mathias    (501) staff       (20)     2298 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/sensors.py
--rw-r--r--   0 mathias    (501) staff       (20)     1012 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/sinks.py
--rw-r--r--   0 mathias    (501) staff       (20)    11267 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/cli.py
--rw-r--r--   0 mathias    (501) staff       (20)     1550 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/common.py
--rw-r--r--   0 mathias    (501) staff       (20)     2161 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/errors.py
--rw-r--r--   0 mathias    (501) staff       (20)      869 2022-01-22 13:12:41.000000 orchd-sdk-0.1a3/src/orchd_sdk/logger.ini
--rw-r--r--   0 mathias    (501) staff       (20)     1318 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/logging.py
--rw-r--r--   0 mathias    (501) staff       (20)    12001 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/models.py
--rw-r--r--   0 mathias    (501) staff       (20)    13919 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/project.py
--rw-r--r--   0 mathias    (501) staff       (20)     9526 2023-04-14 13:34:59.000000 orchd-sdk-0.1a3/src/orchd_sdk/reaction.py
--rw-r--r--   0 mathias    (501) staff       (20)     6912 2023-04-06 07:46:08.000000 orchd-sdk-0.1a3/src/orchd_sdk/sensor.py
--rw-r--r--   0 mathias    (501) staff       (20)     3436 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/sink.py
--rw-r--r--   0 mathias    (501) staff       (20)     2065 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/util.py
-drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.388805 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/
--rw-r--r--   0 mathias    (501) staff       (20)      704 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mathias    (501) staff       (20)      587 2022-01-28 15:55:21.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/SOURCES 2.txt
--rw-r--r--   0 mathias    (501) staff       (20)      783 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mathias    (501) staff       (20)        1 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mathias    (501) staff       (20)       49 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/entry_points.txt
--rw-r--r--   0 mathias    (501) staff       (20)      112 2022-01-28 15:55:21.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/requires 2.txt
--rw-r--r--   0 mathias    (501) staff       (20)      158 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/requires.txt
--rw-r--r--   0 mathias    (501) staff       (20)       10 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.720550 orchd-sdk-0.1a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/src/orchd_sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/src/orchd_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2264 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/api/sinks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2161 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/logger.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12001 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13919 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9526 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6912 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3436 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/sink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-17 15:14:12.000000 orchd-sdk-0.1a4/src/orchd_sdk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:14:56.724551 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-17 15:14:56.000000 orchd-sdk-0.1a4/src/orchd_sdk.egg-info/top_level.txt
```

### Comparing `orchd-sdk-0.1a3/LICENSE.md` & `orchd-sdk-0.1a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/PKG-INFO` & `orchd-sdk-0.1a4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: orchd-sdk
-Version: 0.1a3
+Version: 0.1a4
 Summary: SDK for Orchd Ecosystem Applications
 Home-page: http://orchd.io
 Author: Mathias Santos de Brito
 Author-email: mathias.brito@me.com
 License: UNKNOWN
+Description: UNKNOWN
 Keywords: service resource orchestration edge cloud
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Distributed Computing
 Provides-Extra: test
 Provides-Extra: docs
-License-File: LICENSE.md
-
-UNKNOWN
-
```

### Comparing `orchd-sdk-0.1a3/README.md` & `orchd-sdk-0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/setup.py` & `orchd-sdk-0.1a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from setuptools import setup, find_packages
 
 name = 'orchd-sdk'
 version = open('src/orchd_sdk/VERSION').read().strip()
 author = "Mathias Santos de Brito"
 
 requirements = [
+    'click',
     'reactivex',
     'pydantic',
     'GitPython',
     'colorama'
 ]
 
 test_requirements = [
```

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/__init__.py` & `orchd-sdk-0.1a4/src/orchd_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/api/__init__.py` & `orchd-sdk-0.1a4/src/orchd_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/api/events.py` & `orchd-sdk-0.1a4/src/orchd_sdk/api/events.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/api/reactions.py` & `orchd-sdk-0.1a4/src/orchd_sdk/api/reactions.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/api/sensors.py` & `orchd-sdk-0.1a4/src/orchd_sdk/api/sensors.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/api/sinks.py` & `orchd-sdk-0.1a4/src/orchd_sdk/api/sinks.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/cli.py` & `orchd-sdk-0.1a4/src/orchd_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/common.py` & `orchd-sdk-0.1a4/src/orchd_sdk/common.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/errors.py` & `orchd-sdk-0.1a4/src/orchd_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/logger.ini` & `orchd-sdk-0.1a4/src/orchd_sdk/logger.ini`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/logging.py` & `orchd-sdk-0.1a4/src/orchd_sdk/logging.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/models.py` & `orchd-sdk-0.1a4/src/orchd_sdk/models.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/project.py` & `orchd-sdk-0.1a4/src/orchd_sdk/project.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/reaction.py` & `orchd-sdk-0.1a4/src/orchd_sdk/reaction.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/sensor.py` & `orchd-sdk-0.1a4/src/orchd_sdk/sensor.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/sink.py` & `orchd-sdk-0.1a4/src/orchd_sdk/sink.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk/util.py` & `orchd-sdk-0.1a4/src/orchd_sdk/util.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk.egg-info/PKG-INFO` & `orchd-sdk-0.1a4/src/orchd_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: orchd-sdk
-Version: 0.1a3
+Version: 0.1a4
 Summary: SDK for Orchd Ecosystem Applications
 Home-page: http://orchd.io
 Author: Mathias Santos de Brito
 Author-email: mathias.brito@me.com
 License: UNKNOWN
+Description: UNKNOWN
 Keywords: service resource orchestration edge cloud
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Distributed Computing
 Provides-Extra: test
 Provides-Extra: docs
-License-File: LICENSE.md
-
-UNKNOWN
-
```

### Comparing `orchd-sdk-0.1a3/src/orchd_sdk.egg-info/SOURCES 2.txt` & `orchd-sdk-0.1a4/src/orchd_sdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+LICENSE.md
 README.md
 setup.py
 src/orchd_sdk/VERSION
 src/orchd_sdk/__init__.py
 src/orchd_sdk/cli.py
 src/orchd_sdk/common.py
 src/orchd_sdk/errors.py
 src/orchd_sdk/logger.ini
 src/orchd_sdk/logging.py
 src/orchd_sdk/models.py
 src/orchd_sdk/project.py
 src/orchd_sdk/reaction.py
-src/orchd_sdk/reaction.schema.json
 src/orchd_sdk/sensor.py
 src/orchd_sdk/sink.py
 src/orchd_sdk/util.py
 src/orchd_sdk.egg-info/PKG-INFO
 src/orchd_sdk.egg-info/SOURCES.txt
 src/orchd_sdk.egg-info/dependency_links.txt
 src/orchd_sdk.egg-info/entry_points.txt
 src/orchd_sdk.egg-info/requires.txt
-src/orchd_sdk.egg-info/top_level.txt
+src/orchd_sdk.egg-info/top_level.txt
+src/orchd_sdk/api/__init__.py
+src/orchd_sdk/api/events.py
+src/orchd_sdk/api/reactions.py
+src/orchd_sdk/api/sensors.py
+src/orchd_sdk/api/sinks.py
```

