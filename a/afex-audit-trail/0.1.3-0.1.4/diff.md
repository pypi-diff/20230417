# Comparing `tmp/afex-audit-trail-0.1.3.tar.gz` & `tmp/afex-audit-trail-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-audit-trail-0.1.3.tar", last modified: Sun Apr  9 17:24:37 2023, max compression
+gzip compressed data, was "afex-audit-trail-0.1.4.tar", last modified: Mon Apr 17 16:12:09 2023, max compression
```

## Comparing `afex-audit-trail-0.1.3.tar` & `afex-audit-trail-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 17:24:37.502998 afex-audit-trail-0.1.3/
--rw-rw-rw-   0        0        0     1061 2023-04-04 12:20:36.000000 afex-audit-trail-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6661 2023-04-09 17:24:37.502998 afex-audit-trail-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-09 17:24:37.461156 afex-audit-trail-0.1.3/afex_audit_trail.egg-info/
--rw-rw-rw-   0        0        0     6661 2023-04-09 17:24:37.000000 afex-audit-trail-0.1.3/afex_audit_trail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      681 2023-04-09 17:24:37.000000 afex-audit-trail-0.1.3/afex_audit_trail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 17:24:37.000000 afex-audit-trail-0.1.3/afex_audit_trail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-09 17:24:37.000000 afex-audit-trail-0.1.3/afex_audit_trail.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-09 17:24:37.000000 afex-audit-trail-0.1.3/afex_audit_trail.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 17:24:37.492412 afex-audit-trail-0.1.3/audit_trails/
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.3/audit_trails/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.3/audit_trails/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:24:37.492412 afex-audit-trail-0.1.3/audit_trails/api/
--rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.3/audit_trails/api/__init__.py
--rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.3/audit_trails/api/serializers.py
--rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.3/audit_trails/api/urls.py
--rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.1.3/audit_trails/api/views.py
--rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.3/audit_trails/apps.py
--rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.3/audit_trails/logger.py
--rw-rw-rw-   0        0        0     3164 2023-04-05 10:39:42.000000 afex-audit-trail-0.1.3/audit_trails/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:24:37.502998 afex-audit-trail-0.1.3/audit_trails/migrations/
--rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.3/audit_trails/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.3/audit_trails/migrations/__init__.py
--rw-rw-rw-   0        0        0     3438 2023-04-04 08:39:29.000000 afex-audit-trail-0.1.3/audit_trails/models.py
--rw-rw-rw-   0        0        0     1072 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.3/audit_trails/signals.py
--rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.3/audit_trails/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.3/audit_trails/urls.py
--rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.3/audit_trails/views.py
--rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      987 2023-04-09 17:24:37.508577 afex-audit-trail-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:12:09.907843 afex-audit-trail-0.1.4/
+-rw-rw-rw-   0        0        0     1061 2023-04-04 12:20:36.000000 afex-audit-trail-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       72 2023-04-04 13:06:30.000000 afex-audit-trail-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6661 2023-04-17 16:12:09.907843 afex-audit-trail-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-05 09:42:53.000000 afex-audit-trail-0.1.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 16:12:09.889683 afex-audit-trail-0.1.4/afex_audit_trail.egg-info/
+-rw-rw-rw-   0        0        0     6661 2023-04-17 16:12:09.000000 afex-audit-trail-0.1.4/afex_audit_trail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-04-17 16:12:09.000000 afex-audit-trail-0.1.4/afex_audit_trail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 16:12:09.000000 afex-audit-trail-0.1.4/afex_audit_trail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-17 16:12:09.000000 afex-audit-trail-0.1.4/afex_audit_trail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 16:12:09.000000 afex-audit-trail-0.1.4/afex_audit_trail.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 16:12:09.900843 afex-audit-trail-0.1.4/audit_trails/
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.4/audit_trails/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.4/audit_trails/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:12:09.904843 afex-audit-trail-0.1.4/audit_trails/api/
+-rw-rw-rw-   0        0        0        0 2023-04-03 15:08:20.000000 afex-audit-trail-0.1.4/audit_trails/api/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-04-06 12:53:03.000000 afex-audit-trail-0.1.4/audit_trails/api/serializers.py
+-rw-rw-rw-   0        0        0      860 2023-04-04 09:18:28.000000 afex-audit-trail-0.1.4/audit_trails/api/urls.py
+-rw-rw-rw-   0        0        0     3195 2023-04-09 17:23:20.000000 afex-audit-trail-0.1.4/audit_trails/api/views.py
+-rw-rw-rw-   0        0        0      160 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.4/audit_trails/apps.py
+-rw-rw-rw-   0        0        0     1353 2023-04-04 08:22:08.000000 afex-audit-trail-0.1.4/audit_trails/logger.py
+-rw-rw-rw-   0        0        0     3284 2023-04-17 16:12:00.000000 afex-audit-trail-0.1.4/audit_trails/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-17 16:12:09.906843 afex-audit-trail-0.1.4/audit_trails/migrations/
+-rw-rw-rw-   0        0        0     3055 2023-04-04 17:08:43.000000 afex-audit-trail-0.1.4/audit_trails/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.4/audit_trails/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3438 2023-04-04 08:39:29.000000 afex-audit-trail-0.1.4/audit_trails/models.py
+-rw-rw-rw-   0        0        0     1072 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.4/audit_trails/signals.py
+-rw-rw-rw-   0        0        0       63 2023-03-28 14:13:46.000000 afex-audit-trail-0.1.4/audit_trails/tests.py
+-rw-rw-rw-   0        0        0      821 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.4/audit_trails/urls.py
+-rw-rw-rw-   0        0        0     2235 2023-04-04 13:07:53.000000 afex-audit-trail-0.1.4/audit_trails/views.py
+-rw-rw-rw-   0        0        0      110 2023-04-04 11:53:51.000000 afex-audit-trail-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      987 2023-04-17 16:12:09.909842 afex-audit-trail-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-04-04 13:00:35.000000 afex-audit-trail-0.1.4/setup.py
```

### Comparing `afex-audit-trail-0.1.3/LICENSE` & `afex-audit-trail-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/PKG-INFO` & `afex-audit-trail-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.3/afex_audit_trail.egg-info/PKG-INFO` & `afex-audit-trail-0.1.4/afex_audit_trail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-audit-trail
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Django app to create server logs and users' notification.
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@afexnigeria.com
 License: MIT
 Description: # AFEX Audit Trail
```

### Comparing `afex-audit-trail-0.1.3/afex_audit_trail.egg-info/SOURCES.txt` & `afex-audit-trail-0.1.4/afex_audit_trail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/api/serializers.py` & `afex-audit-trail-0.1.4/audit_trails/api/serializers.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/api/urls.py` & `afex-audit-trail-0.1.4/audit_trails/api/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/api/views.py` & `afex-audit-trail-0.1.4/audit_trails/api/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/logger.py` & `afex-audit-trail-0.1.4/audit_trails/logger.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/middleware.py` & `afex-audit-trail-0.1.4/audit_trails/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from utils.encryption import DataEncryption
 
 
 class ActivityLoggingMiddleware(MiddlewareMixin):
 
     def process_request(self, request):
         request.start_time = time.time()
+        self.activity_log = None
 
     def process_view(self, request, view_func, view_args, view_kwargs):
         host = request.META.get('REMOTE_HOST')
         ip_address = request.META.get('REMOTE_ADDR')
         remote_address = host if host else ip_address
         request_method = request.META.get('REQUEST_METHOD')
         request_body = str(request.body) if request_method in ('POST', 'PUT', 'PATCH',) else None
@@ -66,16 +67,18 @@
         # except:
         #     self.activity_log.response_body = response.data
         try:
             self.activity_log.response_body = str(response.data.get('message'))
         except AttributeError:
             pass
         exec_time = f'{int((time.time() - request.start_time) * 1000)}ms'
-        self.activity_log.response_code = response.status_code
-        self.activity_log.exec_time = exec_time
-        self.activity_log.save()
-        return response
+        if self.activity_log:
+            self.activity_log.response_code = response.status_code
+            self.activity_log.exec_time = exec_time
+            self.activity_log.save()
+            return response
 
     def process_exception(self, request, exception):
-        self.activity_log.error_message = str(exception.__class__.__name__)
-        self.activity_log.save()
+        if self.activity_log:
+            self.activity_log.error_message = str(exception.__class__.__name__)
+            self.activity_log.save()
```

### Comparing `afex-audit-trail-0.1.3/audit_trails/migrations/0001_initial.py` & `afex-audit-trail-0.1.4/audit_trails/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/models.py` & `afex-audit-trail-0.1.4/audit_trails/models.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/signals.py` & `afex-audit-trail-0.1.4/audit_trails/signals.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/urls.py` & `afex-audit-trail-0.1.4/audit_trails/urls.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/audit_trails/views.py` & `afex-audit-trail-0.1.4/audit_trails/views.py`

 * *Files identical despite different names*

### Comparing `afex-audit-trail-0.1.3/setup.cfg` & `afex-audit-trail-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6665 782d 6175 6469 742d 7472   = afex-audit-tr
 00000020: 6169 6c0d 0a76 6572 7369 6f6e 203d 2030  ail..version = 0
-00000030: 2e31 2e33 0d0a 6465 7363 7269 7074 696f  .1.3..descriptio
+00000030: 2e31 2e34 0d0a 6465 7363 7269 7074 696f  .1.4..descriptio
 00000040: 6e20 3d20 4120 446a 616e 676f 2061 7070  n = A Django app
 00000050: 2074 6f20 6372 6561 7465 2073 6572 7665   to create serve
 00000060: 7220 6c6f 6773 2061 6e64 2075 7365 7273  r logs and users
 00000070: 2720 6e6f 7469 6669 6361 7469 6f6e 2e0d  ' notification..
 00000080: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000090: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
 000000a0: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
```

