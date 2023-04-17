# Comparing `tmp/django-germanium-2.3.8.tar.gz` & `tmp/django-germanium-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-germanium-2.3.8.tar", last modified: Fri Feb 10 15:25:43 2023, max compression
+gzip compressed data, was "django-germanium-2.3.9.tar", last modified: Sun Feb 12 15:09:29 2023, max compression
```

## Comparing `django-germanium-2.3.8.tar` & `django-germanium-2.3.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-10 15:25:43.539577 django-germanium-2.3.8/
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1110 2020-01-25 18:58:55.000000 django-germanium-2.3.8/LICENSE
--rw-rw-r--   0 lubos     (1000) lubos     (1000)      523 2023-02-10 15:25:43.539577 django-germanium-2.3.8/PKG-INFO
--rw-rw-r--   0 lubos     (1000) lubos     (1000)    20406 2023-01-25 12:20:55.000000 django-germanium-2.3.8/README.md
-drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-10 15:25:43.535576 django-germanium-2.3.8/django_germanium.egg-info/
--rw-r--r--   0 lubos     (1000) lubos     (1000)      523 2023-02-10 15:25:43.000000 django-germanium-2.3.8/django_germanium.egg-info/PKG-INFO
--rw-r--r--   0 lubos     (1000) lubos     (1000)      889 2023-02-10 15:25:43.000000 django-germanium-2.3.8/django_germanium.egg-info/SOURCES.txt
--rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2023-02-10 15:25:43.000000 django-germanium-2.3.8/django_germanium.egg-info/dependency_links.txt
--rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2020-01-25 18:58:55.000000 django-germanium-2.3.8/django_germanium.egg-info/not-zip-safe
--rw-r--r--   0 lubos     (1000) lubos     (1000)       82 2023-02-10 15:25:43.000000 django-germanium-2.3.8/django_germanium.egg-info/requires.txt
--rw-r--r--   0 lubos     (1000) lubos     (1000)       10 2023-02-10 15:25:43.000000 django-germanium-2.3.8/django_germanium.egg-info/top_level.txt
-drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-10 15:25:43.535576 django-germanium-2.3.8/germanium/
--rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2020-01-25 18:58:55.000000 django-germanium-2.3.8/germanium/__init__.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1433 2020-05-04 21:16:47.000000 django-germanium-2.3.8/germanium/config.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     5131 2020-03-25 18:41:10.000000 django-germanium-2.3.8/germanium/crawler.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)    10921 2022-12-21 13:07:31.000000 django-germanium-2.3.8/germanium/decorators.py
-drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-10 15:25:43.539577 django-germanium-2.3.8/germanium/django/
--rw-rw-r--   0 lubos     (1000) lubos     (1000)        0 2021-05-02 12:02:34.000000 django-germanium-2.3.8/germanium/django/__init__.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)      802 2021-05-05 16:04:20.000000 django-germanium-2.3.8/germanium/django/runner.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     2156 2022-05-09 09:05:16.000000 django-germanium-2.3.8/germanium/django/utils.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      877 2020-01-25 18:58:55.000000 django-germanium-2.3.8/germanium/patch.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)      127 2022-01-07 14:45:48.000000 django-germanium-2.3.8/germanium/signals.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     6565 2022-01-07 14:45:48.000000 django-germanium-2.3.8/germanium/storage.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     3151 2020-04-09 13:07:54.000000 django-germanium-2.3.8/germanium/sugar.py
-drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-10 15:25:43.539577 django-germanium-2.3.8/germanium/test_cases/
--rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2020-01-25 18:58:55.000000 django-germanium-2.3.8/germanium/test_cases/__init__.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      581 2020-01-25 18:58:55.000000 django-germanium-2.3.8/germanium/test_cases/auth.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     4170 2023-01-25 12:20:55.000000 django-germanium-2.3.8/germanium/test_cases/client.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     1406 2022-03-16 08:38:44.000000 django-germanium-2.3.8/germanium/test_cases/default.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)     1333 2020-01-25 18:58:55.000000 django-germanium-2.3.8/germanium/test_cases/migrations.py
--rw-r--r--   0 lubos     (1000) lubos     (1000)      628 2020-01-25 18:58:55.000000 django-germanium-2.3.8/germanium/test_cases/models.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     5695 2021-12-15 12:39:11.000000 django-germanium-2.3.8/germanium/test_cases/rest.py
-drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-10 15:25:43.539577 django-germanium-2.3.8/germanium/tools/
--rw-r--r--   0 lubos     (1000) lubos     (1000)      108 2020-01-25 18:58:55.000000 django-germanium-2.3.8/germanium/tools/__init__.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     4022 2021-11-19 19:03:00.000000 django-germanium-2.3.8/germanium/tools/django.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     4704 2023-02-10 15:25:16.000000 django-germanium-2.3.8/germanium/tools/http.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     3289 2023-01-25 12:20:55.000000 django-germanium-2.3.8/germanium/tools/models.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     1663 2023-02-10 15:25:16.000000 django-germanium-2.3.8/germanium/tools/rest.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)     1319 2021-10-20 13:43:21.000000 django-germanium-2.3.8/germanium/tools/trivials.py
--rw-rw-r--   0 lubos     (1000) lubos     (1000)       38 2023-02-10 15:25:43.539577 django-germanium-2.3.8/setup.cfg
--rw-rw-r--   0 lubos     (1000) lubos     (1000)      782 2023-02-10 15:25:24.000000 django-germanium-2.3.8/setup.py
+drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-12 15:09:29.916050 django-germanium-2.3.9/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1110 2020-01-25 18:58:55.000000 django-germanium-2.3.9/LICENSE
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)      548 2023-02-12 15:09:29.916050 django-germanium-2.3.9/PKG-INFO
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)    20406 2023-01-25 12:20:55.000000 django-germanium-2.3.9/README.md
+drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-12 15:09:29.912050 django-germanium-2.3.9/django_germanium.egg-info/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      548 2023-02-12 15:09:29.000000 django-germanium-2.3.9/django_germanium.egg-info/PKG-INFO
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      889 2023-02-12 15:09:29.000000 django-germanium-2.3.9/django_germanium.egg-info/SOURCES.txt
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2023-02-12 15:09:29.000000 django-germanium-2.3.9/django_germanium.egg-info/dependency_links.txt
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        1 2020-01-25 18:58:55.000000 django-germanium-2.3.9/django_germanium.egg-info/not-zip-safe
+-rw-r--r--   0 lubos     (1000) lubos     (1000)       77 2023-02-12 15:09:29.000000 django-germanium-2.3.9/django_germanium.egg-info/requires.txt
+-rw-r--r--   0 lubos     (1000) lubos     (1000)       10 2023-02-12 15:09:29.000000 django-germanium-2.3.9/django_germanium.egg-info/top_level.txt
+drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-12 15:09:29.916050 django-germanium-2.3.9/germanium/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2020-01-25 18:58:55.000000 django-germanium-2.3.9/germanium/__init__.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1433 2020-05-04 21:16:47.000000 django-germanium-2.3.9/germanium/config.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     5131 2020-03-25 18:41:10.000000 django-germanium-2.3.9/germanium/crawler.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)    11045 2023-02-12 15:09:06.000000 django-germanium-2.3.9/germanium/decorators.py
+drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-12 15:09:29.916050 django-germanium-2.3.9/germanium/django/
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)        0 2021-05-02 12:02:34.000000 django-germanium-2.3.9/germanium/django/__init__.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)      802 2021-05-05 16:04:20.000000 django-germanium-2.3.9/germanium/django/runner.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     2156 2022-05-09 09:05:16.000000 django-germanium-2.3.9/germanium/django/utils.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      877 2020-01-25 18:58:55.000000 django-germanium-2.3.9/germanium/patch.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)      127 2022-01-07 14:45:48.000000 django-germanium-2.3.9/germanium/signals.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     6565 2022-01-07 14:45:48.000000 django-germanium-2.3.9/germanium/storage.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     3151 2020-04-09 13:07:54.000000 django-germanium-2.3.9/germanium/sugar.py
+drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-12 15:09:29.916050 django-germanium-2.3.9/germanium/test_cases/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)        0 2020-01-25 18:58:55.000000 django-germanium-2.3.9/germanium/test_cases/__init__.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      581 2020-01-25 18:58:55.000000 django-germanium-2.3.9/germanium/test_cases/auth.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     4170 2023-01-25 12:20:55.000000 django-germanium-2.3.9/germanium/test_cases/client.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     1406 2022-03-16 08:38:44.000000 django-germanium-2.3.9/germanium/test_cases/default.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)     1333 2020-01-25 18:58:55.000000 django-germanium-2.3.9/germanium/test_cases/migrations.py
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      628 2020-01-25 18:58:55.000000 django-germanium-2.3.9/germanium/test_cases/models.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     5695 2021-12-15 12:39:11.000000 django-germanium-2.3.9/germanium/test_cases/rest.py
+drwxrwxr-x   0 lubos     (1000) lubos     (1000)        0 2023-02-12 15:09:29.916050 django-germanium-2.3.9/germanium/tools/
+-rw-r--r--   0 lubos     (1000) lubos     (1000)      108 2020-01-25 18:58:55.000000 django-germanium-2.3.9/germanium/tools/__init__.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     4022 2021-11-19 19:03:00.000000 django-germanium-2.3.9/germanium/tools/django.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     4704 2023-02-10 15:25:16.000000 django-germanium-2.3.9/germanium/tools/http.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     3289 2023-01-25 12:20:55.000000 django-germanium-2.3.9/germanium/tools/models.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     1663 2023-02-10 15:25:16.000000 django-germanium-2.3.9/germanium/tools/rest.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)     1319 2021-10-20 13:43:21.000000 django-germanium-2.3.9/germanium/tools/trivials.py
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)       38 2023-02-12 15:09:29.916050 django-germanium-2.3.9/setup.cfg
+-rw-rw-r--   0 lubos     (1000) lubos     (1000)      787 2023-02-12 15:09:12.000000 django-germanium-2.3.9/setup.py
```

### Comparing `django-germanium-2.3.8/LICENSE` & `django-germanium-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/README.md` & `django-germanium-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/django_germanium.egg-info/SOURCES.txt` & `django-germanium-2.3.9/django_germanium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/config.py` & `django-germanium-2.3.9/germanium/config.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/crawler.py` & `django-germanium-2.3.9/germanium/crawler.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/decorators.py` & `django-germanium-2.3.9/germanium/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import types
 
 from collections.abc import Iterable
 from functools import wraps
 
 from inspect import isclass, isfunction, ismethod, getfullargspec, signature
 
-import responses
 from django.db import transaction
 from django.db.models import Model
 from django.db.models.fields import DateField, DateTimeField
 from django.utils.functional import cached_property
 
+try:
+    import responses
+
+    def reset_responses():
+        responses.reset()
+except ImportError:
+    def reset_responses():
+        pass
+
 
 def is_iterable(data):
     return isinstance(data, Iterable) and not isinstance(data, str)
 
 
 def refresh_model_object(obj):
     obj.refresh_from_db()
@@ -186,15 +194,15 @@
         else:
             if hasattr(self, 'set_up_data_consumer'):
                 self.tear_up_data_consumer()
             call(method, self, ((data,) if not is_iterable(data) else data), named_data)
     finally:
         if use_rollback:
             transaction.savepoint_rollback(sid)
-            responses.reset()
+            reset_responses()
             refresh_model_objects(
                 *(data.data.values() if isinstance(data, NamedTestData) else data)
             )
         if not is_data_consumer and hasattr(self, 'tear_down_data_consumer'):
             self.tear_down_data_consumer()
```

### Comparing `django-germanium-2.3.8/germanium/django/runner.py` & `django-germanium-2.3.9/germanium/django/runner.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/django/utils.py` & `django-germanium-2.3.9/germanium/django/utils.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/patch.py` & `django-germanium-2.3.9/germanium/patch.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/storage.py` & `django-germanium-2.3.9/germanium/storage.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/sugar.py` & `django-germanium-2.3.9/germanium/sugar.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/test_cases/auth.py` & `django-germanium-2.3.9/germanium/test_cases/auth.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/test_cases/client.py` & `django-germanium-2.3.9/germanium/test_cases/client.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/test_cases/default.py` & `django-germanium-2.3.9/germanium/test_cases/default.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/test_cases/migrations.py` & `django-germanium-2.3.9/germanium/test_cases/migrations.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/test_cases/models.py` & `django-germanium-2.3.9/germanium/test_cases/models.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/test_cases/rest.py` & `django-germanium-2.3.9/germanium/test_cases/rest.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/tools/django.py` & `django-germanium-2.3.9/germanium/tools/django.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/tools/http.py` & `django-germanium-2.3.9/germanium/tools/http.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/tools/models.py` & `django-germanium-2.3.9/germanium/tools/models.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/tools/rest.py` & `django-germanium-2.3.9/germanium/tools/rest.py`

 * *Files identical despite different names*

### Comparing `django-germanium-2.3.8/germanium/tools/trivials.py` & `django-germanium-2.3.9/germanium/tools/trivials.py`

 * *Files identical despite different names*

