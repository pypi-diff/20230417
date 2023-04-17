# Comparing `tmp/django-structlog-5.0.1.tar.gz` & `tmp/django-structlog-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-structlog-5.0.1.tar", last modified: Fri Mar 24 12:21:34 2023, max compression
+gzip compressed data, was "django-structlog-5.0.2.tar", last modified: Mon Apr 17 00:49:30 2023, max compression
```

## Comparing `django-structlog-5.0.1.tar` & `django-structlog-5.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:21:34.555151 django-structlog-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-24 12:21:24.000000 django-structlog-5.0.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-24 12:21:24.000000 django-structlog-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-03-24 12:21:34.555151 django-structlog-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22196 2023-03-24 12:21:24.000000 django-structlog-5.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:21:34.555151 django-structlog-5.0.1/django_structlog/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:21:34.555151 django-structlog-5.0.1/django_structlog/celery/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/celery/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/celery/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/celery/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/celery/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:21:34.555151 django-structlog-5.0.1/django_structlog/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/middlewares/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-24 12:21:24.000000 django-structlog-5.0.1/django_structlog/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:21:34.555151 django-structlog-5.0.1/django_structlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-03-24 12:21:34.000000 django-structlog-5.0.1/django_structlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-24 12:21:34.000000 django-structlog-5.0.1/django_structlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 12:21:34.000000 django-structlog-5.0.1/django_structlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-24 12:21:34.000000 django-structlog-5.0.1/django_structlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 12:21:34.000000 django-structlog-5.0.1/django_structlog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-24 12:21:24.000000 django-structlog-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-24 12:21:34.555151 django-structlog-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.238410 django-structlog-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-17 00:49:20.000000 django-structlog-5.0.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-17 00:49:20.000000 django-structlog-5.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-17 00:49:30.238410 django-structlog-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21911 2023-04-17 00:49:20.000000 django-structlog-5.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.234410 django-structlog-5.0.2/django_structlog/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.234410 django-structlog-5.0.2/django_structlog/celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/celery/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.238410 django-structlog-5.0.2/django_structlog/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/middlewares/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-17 00:49:20.000000 django-structlog-5.0.2/django_structlog/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 00:49:30.234410 django-structlog-5.0.2/django_structlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23035 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 00:49:30.000000 django-structlog-5.0.2/django_structlog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-17 00:49:20.000000 django-structlog-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 00:49:30.238410 django-structlog-5.0.2/setup.cfg
```

### Comparing `django-structlog-5.0.1/LICENSE.rst` & `django-structlog-5.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.1/PKG-INFO` & `django-structlog-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-structlog
-Version: 5.0.1
+Version: 5.0.2
 Summary: Structured Logging for Django
 Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/jrobichaud/django-structlog
 Project-URL: repository, https://github.com/jrobichaud/django-structlog
 Project-URL: documentation, https://django-structlog.readthedocs.io
 Classifier: Framework :: Django
@@ -372,19 +372,19 @@
 Upgrading to 5.0+
 ^^^^^^^^^^^^^^^^^
 
 Minimum requirements
 ~~~~~~~~~~~~~~~~~~~~
 - requires asgiref 3.6+
 
-Changes you may need to do
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+Change you may need to do
+~~~~~~~~~~~~~~~~~~~~~~~~~
 
-1. Make sure you use ``django_structlog.middlewares.RequestMiddleware``
------------------------------------------------------------------------
+Make sure you use ``django_structlog.middlewares.RequestMiddleware``
+--------------------------------------------------------------------
 
 If you used any of the experimental async or sync middlewares, you do not need to anymore.
 Make sure you use ``django_structlog.middlewares.RequestMiddleware`` instead of any of the other request middlewares commented below:
 
 .. code-block:: python
 
     MIDDLEWARE += [
@@ -393,21 +393,14 @@
         # "django_structlog.middlewares.requests.AsyncRequestMiddleware", # <- remove
         "django_structlog.middlewares.RequestMiddleware", # <- make sure you use this one
         "django_structlog.middlewares.CeleryMiddleware",
     ]
 
 They will be removed in another major version.
 
-2. ``django_structlog.signals.bind_extra_request_failed_metadata`` was removed
-------------------------------------------------------------------------------
-
-The signal ``bind_extra_request_failed_metadata`` was removed since it was never called.
-
-Remove your custom signal.
-
 
 .. _upgrade_4.0:
 
 Upgrading to 4.0+
 ^^^^^^^^^^^^^^^^^
 
 ``django-structlog`` drops support of django below 3.2.
```

### Comparing `django-structlog-5.0.1/README.rst` & `django-structlog-5.0.2/django_structlog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: django-structlog
+Version: 5.0.2
+Summary: Structured Logging for Django
+Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
+License: MIT
+Project-URL: homepage, https://github.com/jrobichaud/django-structlog
+Project-URL: repository, https://github.com/jrobichaud/django-structlog
+Project-URL: documentation, https://django-structlog.readthedocs.io
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: System :: Logging
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: celery
+License-File: LICENSE.rst
+
 .. inclusion-marker-introduction-begin
 
 django-structlog
 ================
 
 | |pypi| |wheels| |build-status| |docs| |coverage| |open_issues| |pull_requests|
 | |django| |python| |license| |black|
@@ -344,19 +372,19 @@
 Upgrading to 5.0+
 ^^^^^^^^^^^^^^^^^
 
 Minimum requirements
 ~~~~~~~~~~~~~~~~~~~~
 - requires asgiref 3.6+
 
-Changes you may need to do
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+Change you may need to do
+~~~~~~~~~~~~~~~~~~~~~~~~~
 
-1. Make sure you use ``django_structlog.middlewares.RequestMiddleware``
------------------------------------------------------------------------
+Make sure you use ``django_structlog.middlewares.RequestMiddleware``
+--------------------------------------------------------------------
 
 If you used any of the experimental async or sync middlewares, you do not need to anymore.
 Make sure you use ``django_structlog.middlewares.RequestMiddleware`` instead of any of the other request middlewares commented below:
 
 .. code-block:: python
 
     MIDDLEWARE += [
@@ -365,21 +393,14 @@
         # "django_structlog.middlewares.requests.AsyncRequestMiddleware", # <- remove
         "django_structlog.middlewares.RequestMiddleware", # <- make sure you use this one
         "django_structlog.middlewares.CeleryMiddleware",
     ]
 
 They will be removed in another major version.
 
-2. ``django_structlog.signals.bind_extra_request_failed_metadata`` was removed
-------------------------------------------------------------------------------
-
-The signal ``bind_extra_request_failed_metadata`` was removed since it was never called.
-
-Remove your custom signal.
-
 
 .. _upgrade_4.0:
 
 Upgrading to 4.0+
 ^^^^^^^^^^^^^^^^^
 
 ``django-structlog`` drops support of django below 3.2.
```

### Comparing `django-structlog-5.0.1/django_structlog/celery/middlewares.py` & `django-structlog-5.0.2/django_structlog/celery/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.1/django_structlog/celery/receivers.py` & `django-structlog-5.0.2/django_structlog/celery/receivers.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.1/django_structlog/celery/signals.py` & `django-structlog-5.0.2/django_structlog/celery/signals.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.1/django_structlog/celery/steps.py` & `django-structlog-5.0.2/django_structlog/celery/steps.py`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.1/django_structlog/middlewares/request.py` & `django-structlog-5.0.2/django_structlog/middlewares/request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import uuid
 
 import structlog
 from asgiref.sync import iscoroutinefunction, markcoroutinefunction
+from django.core.exceptions import PermissionDenied
+from django.http import Http404
 from django.utils.decorators import sync_and_async_middleware
 from asgiref import sync
 from django.utils.deprecation import warn_about_renamed_method
 
 from .. import signals
 
 logger = structlog.getLogger(__name__)
@@ -19,26 +21,29 @@
 
 
 class BaseRequestMiddleWare:
     def __init__(self, get_response):
         self.get_response = get_response
 
     def handle_response(self, request, response):
-        self.bind_user_id(request)
-        signals.bind_extra_request_finished_metadata.send(
-            sender=self.__class__,
-            request=request,
-            logger=logger,
-            response=response,
-        )
-        logger.info(
-            "request_finished",
-            code=response.status_code,
-            request=self.format_request(request),
-        )
+        if not hasattr(request, "_raised_exception"):
+            self.bind_user_id(request)
+            signals.bind_extra_request_finished_metadata.send(
+                sender=self.__class__,
+                request=request,
+                logger=logger,
+                response=response,
+            )
+            logger.info(
+                "request_finished",
+                code=response.status_code,
+                request=self.format_request(request),
+            )
+        else:
+            delattr(request, "_raised_exception")
         structlog.contextvars.clear_contextvars()
 
     def prepare(self, request):
         from ipware import get_client_ip
 
         request_id = get_request_header(
             request, "x-request-id", "HTTP_X_REQUEST_ID"
@@ -61,14 +66,35 @@
             user_agent=request.META.get("HTTP_USER_AGENT"),
         )
 
     @staticmethod
     def format_request(request):
         return "%s %s" % (request.method, request.get_full_path())
 
+    def process_exception(self, request, exception):
+        if isinstance(exception, (Http404, PermissionDenied)):
+            # We don't log an exception here, and we don't set that we handled
+            # an error as we want the standard `request_finished` log message
+            # to be emitted.
+            return
+
+        setattr(request, "_raised_exception", True)
+        self.bind_user_id(request)
+        signals.bind_extra_request_failed_metadata.send(
+            sender=self.__class__,
+            request=request,
+            logger=logger,
+            exception=exception,
+        )
+        logger.exception(
+            "request_failed",
+            code=500,
+            request=self.format_request(request),
+        )
+
     @staticmethod
     def bind_user_id(request):
         if hasattr(request, "user") and request.user is not None:
             user_id = None
             if hasattr(request.user, "pk"):
                 user_id = request.user.pk
                 if isinstance(user_id, uuid.UUID):
```

### Comparing `django-structlog-5.0.1/django_structlog/signals.py` & `django-structlog-5.0.2/django_structlog/signals.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,7 +27,23 @@
 >>> import structlog
 >>>
 >>> @receiver(signals.bind_extra_request_finished_metadata)
 ... def bind_user_email(request, logger, response, **kwargs):
 ...     structlog.contextvars.bind_contextvars(user_email=getattr(request.user, 'email', ''))
 
 """
+
+bind_extra_request_failed_metadata = django.dispatch.Signal()
+""" Signal to add extra ``structlog`` bindings from ``django``'s failed request and exception.
+
+:param logger: the logger to bind more metadata or override existing bound metadata
+:param exception: the exception resulting of the request
+
+>>> from django.dispatch import receiver
+>>> from django_structlog import signals
+>>> import structlog
+>>>
+>>> @receiver(signals.bind_extra_request_failed_metadata)
+... def bind_user_email(request, logger, exception, **kwargs):
+...     structlog.contextvars.bind_contextvars(user_email=getattr(request.user, 'email', ''))
+
+"""
```

### Comparing `django-structlog-5.0.1/django_structlog.egg-info/PKG-INFO` & `django-structlog-5.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: django-structlog
-Version: 5.0.1
-Summary: Structured Logging for Django
-Author-email: Jules Robichaud-Gagnon <j.robichaudg+pypi@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/jrobichaud/django-structlog
-Project-URL: repository, https://github.com/jrobichaud/django-structlog
-Project-URL: documentation, https://django-structlog.readthedocs.io
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: System :: Logging
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: celery
-License-File: LICENSE.rst
-
 .. inclusion-marker-introduction-begin
 
 django-structlog
 ================
 
 | |pypi| |wheels| |build-status| |docs| |coverage| |open_issues| |pull_requests|
 | |django| |python| |license| |black|
@@ -372,19 +344,19 @@
 Upgrading to 5.0+
 ^^^^^^^^^^^^^^^^^
 
 Minimum requirements
 ~~~~~~~~~~~~~~~~~~~~
 - requires asgiref 3.6+
 
-Changes you may need to do
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+Change you may need to do
+~~~~~~~~~~~~~~~~~~~~~~~~~
 
-1. Make sure you use ``django_structlog.middlewares.RequestMiddleware``
------------------------------------------------------------------------
+Make sure you use ``django_structlog.middlewares.RequestMiddleware``
+--------------------------------------------------------------------
 
 If you used any of the experimental async or sync middlewares, you do not need to anymore.
 Make sure you use ``django_structlog.middlewares.RequestMiddleware`` instead of any of the other request middlewares commented below:
 
 .. code-block:: python
 
     MIDDLEWARE += [
@@ -393,21 +365,14 @@
         # "django_structlog.middlewares.requests.AsyncRequestMiddleware", # <- remove
         "django_structlog.middlewares.RequestMiddleware", # <- make sure you use this one
         "django_structlog.middlewares.CeleryMiddleware",
     ]
 
 They will be removed in another major version.
 
-2. ``django_structlog.signals.bind_extra_request_failed_metadata`` was removed
-------------------------------------------------------------------------------
-
-The signal ``bind_extra_request_failed_metadata`` was removed since it was never called.
-
-Remove your custom signal.
-
 
 .. _upgrade_4.0:
 
 Upgrading to 4.0+
 ^^^^^^^^^^^^^^^^^
 
 ``django-structlog`` drops support of django below 3.2.
```

### Comparing `django-structlog-5.0.1/django_structlog.egg-info/SOURCES.txt` & `django-structlog-5.0.2/django_structlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-structlog-5.0.1/pyproject.toml` & `django-structlog-5.0.2/pyproject.toml`

 * *Files identical despite different names*

