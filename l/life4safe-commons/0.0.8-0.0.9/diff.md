# Comparing `tmp/life4safe-commons-0.0.8.tar.gz` & `tmp/life4safe-commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life4safe-commons-0.0.8.tar", last modified: Fri Feb 10 13:39:41 2023, max compression
+gzip compressed data, was "life4safe-commons-0.0.9.tar", last modified: Fri Feb 10 14:00:16 2023, max compression
```

## Comparing `life4safe-commons-0.0.8.tar` & `life4safe-commons-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-02-10 13:39:41.186348 life4safe-commons-0.0.8/
--rwxrwxrwx   0 israel    (1000) israel    (1000)       38 2023-02-09 13:05:28.000000 life4safe-commons-0.0.8/LICENSE.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)      952 2023-02-10 13:39:41.186348 life4safe-commons-0.0.8/PKG-INFO
--rwxrwxrwx   0 israel    (1000) israel    (1000)      391 2023-02-09 13:05:28.000000 life4safe-commons-0.0.8/README.md
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-02-10 13:39:41.186348 life4safe-commons-0.0.8/life4safe_commons.egg-info/
--rw-rw-r--   0 israel    (1000) israel    (1000)      952 2023-02-10 13:39:41.000000 life4safe-commons-0.0.8/life4safe_commons.egg-info/PKG-INFO
--rw-rw-r--   0 israel    (1000) israel    (1000)      470 2023-02-10 13:39:41.000000 life4safe-commons-0.0.8/life4safe_commons.egg-info/SOURCES.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-02-10 13:39:41.000000 life4safe-commons-0.0.8/life4safe_commons.egg-info/dependency_links.txt
--rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-02-10 13:39:41.000000 life4safe-commons-0.0.8/life4safe_commons.egg-info/top_level.txt
-drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-02-10 13:39:41.186348 life4safe-commons-0.0.8/live4safe_commons/
--rwxrwxrwx   0 israel    (1000) israel    (1000)      287 2023-02-09 13:05:28.000000 life4safe-commons-0.0.8/live4safe_commons/__init__.py
--rwxrwxrwx   0 israel    (1000) israel    (1000)     4924 2023-02-10 13:22:17.000000 life4safe-commons-0.0.8/live4safe_commons/cloud_storage.py
--rwxrwxrwx   0 israel    (1000) israel    (1000)     5761 2023-02-09 13:05:28.000000 life4safe-commons-0.0.8/live4safe_commons/connection.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      895 2023-02-10 13:35:13.000000 life4safe-commons-0.0.8/live4safe_commons/controller.py
--rwxrwxrwx   0 israel    (1000) israel    (1000)      200 2023-02-09 13:05:28.000000 life4safe-commons-0.0.8/live4safe_commons/liveness_status_enum.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      363 2023-02-10 13:20:09.000000 life4safe-commons-0.0.8/live4safe_commons/logger_app.py
--rwxrwxrwx   0 israel    (1000) israel    (1000)     8030 2023-02-09 13:05:28.000000 life4safe-commons-0.0.8/live4safe_commons/misc.py
--rw-rw-r--   0 israel    (1000) israel    (1000)      784 2023-02-10 13:36:10.000000 life4safe-commons-0.0.8/live4safe_commons/server_instance.py
--rwxrwxrwx   0 israel    (1000) israel    (1000)      106 2023-02-10 13:39:41.186348 life4safe-commons-0.0.8/setup.cfg
--rwxrwxrwx   0 israel    (1000) israel    (1000)     1085 2023-02-10 13:37:26.000000 life4safe-commons-0.0.8/setup.py
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-02-10 14:00:16.327038 life4safe-commons-0.0.9/
+-rwxrwxrwx   0 israel    (1000) israel    (1000)       38 2023-02-09 13:05:28.000000 life4safe-commons-0.0.9/LICENSE.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)      952 2023-02-10 14:00:16.327038 life4safe-commons-0.0.9/PKG-INFO
+-rwxrwxrwx   0 israel    (1000) israel    (1000)      391 2023-02-09 13:05:28.000000 life4safe-commons-0.0.9/README.md
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-02-10 14:00:16.327038 life4safe-commons-0.0.9/life4safe_commons.egg-info/
+-rw-rw-r--   0 israel    (1000) israel    (1000)      952 2023-02-10 14:00:16.000000 life4safe-commons-0.0.9/life4safe_commons.egg-info/PKG-INFO
+-rw-rw-r--   0 israel    (1000) israel    (1000)      470 2023-02-10 14:00:16.000000 life4safe-commons-0.0.9/life4safe_commons.egg-info/SOURCES.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)        1 2023-02-10 14:00:16.000000 life4safe-commons-0.0.9/life4safe_commons.egg-info/dependency_links.txt
+-rw-rw-r--   0 israel    (1000) israel    (1000)       18 2023-02-10 14:00:16.000000 life4safe-commons-0.0.9/life4safe_commons.egg-info/top_level.txt
+drwxrwxr-x   0 israel    (1000) israel    (1000)        0 2023-02-10 14:00:16.327038 life4safe-commons-0.0.9/live4safe_commons/
+-rwxrwxrwx   0 israel    (1000) israel    (1000)      287 2023-02-09 13:05:28.000000 life4safe-commons-0.0.9/live4safe_commons/__init__.py
+-rwxrwxrwx   0 israel    (1000) israel    (1000)     4924 2023-02-10 13:22:17.000000 life4safe-commons-0.0.9/live4safe_commons/cloud_storage.py
+-rwxrwxrwx   0 israel    (1000) israel    (1000)     5761 2023-02-09 13:05:28.000000 life4safe-commons-0.0.9/live4safe_commons/connection.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      913 2023-02-10 13:58:36.000000 life4safe-commons-0.0.9/live4safe_commons/controller.py
+-rwxrwxrwx   0 israel    (1000) israel    (1000)      200 2023-02-09 13:05:28.000000 life4safe-commons-0.0.9/live4safe_commons/liveness_status_enum.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      363 2023-02-10 13:20:09.000000 life4safe-commons-0.0.9/live4safe_commons/logger_app.py
+-rwxrwxrwx   0 israel    (1000) israel    (1000)     8030 2023-02-09 13:05:28.000000 life4safe-commons-0.0.9/live4safe_commons/misc.py
+-rw-rw-r--   0 israel    (1000) israel    (1000)      784 2023-02-10 13:36:10.000000 life4safe-commons-0.0.9/live4safe_commons/server_instance.py
+-rwxrwxrwx   0 israel    (1000) israel    (1000)      106 2023-02-10 14:00:16.331038 life4safe-commons-0.0.9/setup.cfg
+-rwxrwxrwx   0 israel    (1000) israel    (1000)     1085 2023-02-10 13:58:58.000000 life4safe-commons-0.0.9/setup.py
```

### Comparing `life4safe-commons-0.0.8/PKG-INFO` & `life4safe-commons-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: life4safe-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common functions to liveliness algorithms
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Project-URL: Download, https://dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
```

### Comparing `life4safe-commons-0.0.8/life4safe_commons.egg-info/PKG-INFO` & `life4safe-commons-0.0.9/life4safe_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: life4safe-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common functions to liveliness algorithms
 Home-page: https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Author: TIT CS
 Author-email: contato@titcs.com.br
 License: MIT
 Project-URL: Código fonte, https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
 Project-URL: Download, https://dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common
```

### Comparing `life4safe-commons-0.0.8/live4safe_commons/cloud_storage.py` & `life4safe-commons-0.0.9/live4safe_commons/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `life4safe-commons-0.0.8/live4safe_commons/connection.py` & `life4safe-commons-0.0.9/live4safe_commons/connection.py`

 * *Files identical despite different names*

### Comparing `life4safe-commons-0.0.8/live4safe_commons/controller.py` & `life4safe-commons-0.0.9/live4safe_commons/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from flask import Flask, Response, request
 from flask_restx import Api, Resource
 import prometheus_client
 from prometheus_client.core import CollectorRegistry
 from prometheus_client import Summary, Counter, Histogram, Gauge
-from server_instance import server
+from live4safe_commons.server_instance import server
 
 app, api = server.app , server.api
 
 _INF = float("inf")
 
 graphs = {}
 graphs['c'] = Counter('python_request_operations_total', 'The total number of processed requests')
```

### Comparing `life4safe-commons-0.0.8/live4safe_commons/misc.py` & `life4safe-commons-0.0.9/live4safe_commons/misc.py`

 * *Files identical despite different names*

### Comparing `life4safe-commons-0.0.8/live4safe_commons/server_instance.py` & `life4safe-commons-0.0.9/live4safe_commons/server_instance.py`

 * *Files identical despite different names*

### Comparing `life4safe-commons-0.0.8/setup.py` & `life4safe-commons-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='life4safe-commons',
-    version='0.0.8',
+    version='0.0.9',
     author='TIT CS',
     author_email='contato@titcs.com.br',
     packages=['live4safe_commons'],
     description='Common functions to liveliness algorithms',
     long_description='Common functions to liveliness algorithms',
     url='https://TITBrasil@dev.azure.com/TITBrasil/TITCS%20-%20Live4Safe/_git/Live4Safe_Common',
     project_urls={
```

