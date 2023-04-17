# Comparing `tmp/redis-metric-helper-0.2.3.tar.gz` & `tmp/redis-metric-helper-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.2.3.tar", last modified: Mon Apr 17 10:27:29 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.2.4.tar", last modified: Mon Apr 17 10:31:03 2023, max compression
```

## Comparing `redis-metric-helper-0.2.3.tar` & `redis-metric-helper-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:27:29.138297 redis-metric-helper-0.2.3/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2.3/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-17 10:27:29.134297 redis-metric-helper-0.2.3/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2.3/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:27:29.134297 redis-metric-helper-0.2.3/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-17 10:26:25.000000 redis-metric-helper-0.2.3/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7037 2023-04-17 10:25:07.000000 redis-metric-helper-0.2.3/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-14 11:03:12.000000 redis-metric-helper-0.2.3/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1170 2023-04-14 14:07:38.000000 redis-metric-helper-0.2.3/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2.3/metric_helper/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-04-12 14:09:16.000000 redis-metric-helper-0.2.3/metric_helper/registry.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:27:29.134297 redis-metric-helper-0.2.3/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-17 10:27:29.000000 redis-metric-helper-0.2.3/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-04-17 10:27:29.000000 redis-metric-helper-0.2.3/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-17 10:27:29.000000 redis-metric-helper-0.2.3/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-17 10:27:29.000000 redis-metric-helper-0.2.3/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-17 10:27:29.000000 redis-metric-helper-0.2.3/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-17 10:27:29.138297 redis-metric-helper-0.2.3/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2.3/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2.4/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2.4/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-17 10:30:25.000000 redis-metric-helper-0.2.4/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7055 2023-04-17 10:30:18.000000 redis-metric-helper-0.2.4/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-14 11:03:12.000000 redis-metric-helper-0.2.4/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1170 2023-04-14 14:07:38.000000 redis-metric-helper-0.2.4/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2.4/metric_helper/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-04-12 14:09:16.000000 redis-metric-helper-0.2.4/metric_helper/registry.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2.4/setup.py
```

### Comparing `redis-metric-helper-0.2.3/LICENSE` & `redis-metric-helper-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.3/PKG-INFO` & `redis-metric-helper-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2.3
+Version: 0.2.4
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2.3/metric_helper/base.py` & `redis-metric-helper-0.2.4/metric_helper/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,14 +179,15 @@
         if pipeline:
             ts = pipeline.ts()
 
         start = start.timestamp() * 1000
         end = end.timestamp() * 1000
         bucket_msecs = bucket_secs * 1000
 
+        data = []
         start = int(start)
         end = int(end)
         bucket_msecs = int(bucket_msecs)
         try:
             data = self.ts.range(
                 key=self.key,
                 from_time=start,
```

### Comparing `redis-metric-helper-0.2.3/metric_helper/connections.py` & `redis-metric-helper-0.2.4/metric_helper/connections.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.3/metric_helper/registry.py` & `redis-metric-helper-0.2.4/metric_helper/registry.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.3/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.2.4/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2.3
+Version: 0.2.4
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2.3/setup.py` & `redis-metric-helper-0.2.4/setup.py`

 * *Files identical despite different names*

