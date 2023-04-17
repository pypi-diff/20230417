# Comparing `tmp/serverless-sdk-0.4.0.tar.gz` & `tmp/serverless-sdk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-klpnetyx/serverless-sdk-0.4.0.tar", last modified: Fri Apr 14 13:30:06 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-0e7qlg8t/serverless-sdk-0.4.1.tar", last modified: Mon Apr 17 18:17:38 2023, max compression
```

## Comparing `serverless-sdk-0.4.0.tar` & `serverless-sdk-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/warning_captured_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/warning_captured_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.0/PKG-INFO` & `serverless-sdk-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.0/README.md` & `serverless-sdk-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/pyproject.toml` & `serverless-sdk-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
     "setuptools>=65.6.3",
     "wheel>=0.38.4",
 ]
 
 [project]
 name = "serverless-sdk"
-version = "0.4.0"
+version = "0.4.1"
 description = "Serverless SDK for Python"
 readme = "README.md"
 authors = [{ name = "serverlessinc" }]
 requires-python = ">=3.7"
 dependencies = [
     "backports.cached-property", # included in Python >=3.8
     "blinker>=1.5",
```

### Comparing `serverless-sdk-0.4.0/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.1/serverless_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.0/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.1/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/__init__.py` & `serverless-sdk-0.4.1/sls_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 class ServerlessSdk:
     name: Final[str] = __name__
     version: Final[str] = __version__
     _event_emitter: EventEmitter
 
     trace_spans: TraceSpans
-    instrumentation: Final = ...
+    instrumentation: Final = SimpleNamespace()
 
     org_id: Optional[str] = None
     _settings: ServerlessSdkSettings
     _custom_tags: Tags
     _is_initialized: bool
     _is_debug_mode: bool
     _is_dev_mode: bool
@@ -89,20 +89,22 @@
         self._report_error = report_error
         self._report_warning = report_warning
         self._report_notice = report_notice
         self._maximum_body_byte_length = 1024 * 127  # 127 KB
 
     def _initialize(
         self,
+        *args,
         org_id: Optional[str] = None,
         disable_captured_events_stdout: Optional[bool] = False,
         disable_python_log_monitoring: Optional[bool] = False,
         disable_request_response_monitoring: Optional[bool] = False,
         disable_http_monitoring: Optional[bool] = False,
         disable_flask_monitoring: Optional[bool] = False,
+        **kwargs,
     ):
         if self._is_initialized:
             return
         self.org_id = environ.get(SLS_ORG_ID, default=org_id)
         self._is_debug_mode = bool(environ.get("SLS_SDK_DEBUG"))
         self._is_dev_mode = bool(environ.get("SLS_DEV_MODE_ORG_ID"))
         self._settings = ServerlessSdkSettings(
@@ -122,14 +124,17 @@
             install_http()
 
         if not self._settings.disable_flask_monitoring:
             from .lib.instrumentation.flask import install as install_flask
 
             install_flask()
 
+        if hasattr(self, "_initialize_extension"):
+            self._initialize_extension(*args, **kwargs)
+
         self._is_initialized = True
 
     def _create_trace_span(
         self,
         name: str,
         input: Optional[str] = None,
         output: Optional[str] = None,
```

### Comparing `serverless-sdk-0.4.0/sls_sdk/exceptions.py` & `serverless-sdk-0.4.1/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.1/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/emitter.py` & `serverless-sdk-0.4.1/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/error.py` & `serverless-sdk-0.4.1/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.1/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/http.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 import time
 import importlib
+import contextvars
 from urllib.parse import urlparse
 from urllib.parse import parse_qs
 from ..error import report as report_error
 import sls_sdk
 
 SDK = sls_sdk.serverlessSdk
+_IGNORE_FOLLOWING_REQUEST = contextvars.ContextVar("ignore", default=False)
+
+
+def ignore_following_request():
+    _IGNORE_FOLLOWING_REQUEST.set(True)
+
+
+def reset_ignore_following_request():
+    _IGNORE_FOLLOWING_REQUEST.set(False)
+
+
+_HTTP_SPAN = contextvars.ContextVar("http-span", default=None)
 
 
 class BaseInstrumenter:
     def __init__(self, target_module):
         self._is_installed = False
         self._target_module = target_module
 
@@ -163,105 +176,113 @@
 
 
 class NativeHTTPInstrumenter(BaseInstrumenter):
     def __init__(self):
         super().__init__("http")
         self._original_request = None
         self._original_getresponse = None
-        self._trace_span = None
 
     def _instrumented_request(self):
         def _func(_self, method, url, body=None, headers={}, *, encode_chunked=False):
+            _self._sls_ignore = _IGNORE_FOLLOWING_REQUEST.get()
+            reset_ignore_following_request()
+
+            if _self._sls_ignore:
+                return self._original_request(
+                    _self, method, url, body, headers, encode_chunked=encode_chunked
+                )
             start_time = time.perf_counter_ns()
 
             SDK._debug_log("HTTP request")
             protocol = (
                 "https" if _self.__class__.__name__ == "HTTPSConnection" else "http"
             )
 
-            self._trace_span = SDK._create_trace_span(
+            trace_span = SDK._create_trace_span(
                 f"python.{protocol}.request",
                 start_time=start_time,
             )
+            _HTTP_SPAN.set(trace_span)
 
             try:
                 parsed_path = urlparse(url)
                 query = parse_qs(parsed_path.query)
-                self._trace_span.tags.update(
+                trace_span.tags.update(
                     {
                         "method": method,
                         "protocol": "HTTP/1.1",
                         "host": f"{_self.host}:{_self.port}",
                         "path": parsed_path.path,
                         "request_header_names": [h for h in headers.keys()],
                         "query_parameter_names": [q for q in query.keys()],
                     },
                     prefix="http",
                 )
-                self._capture_request_body(body)
+                self._capture_request_body(trace_span, body)
 
                 self._original_request(
                     _self, method, url, body, headers, encode_chunked=encode_chunked
                 )
             except Exception as ex:
-                self._trace_span.tags["http.error_code"] = ex.__class__.__name__
-                if self._trace_span.end_time is None:
-                    self._trace_span.close()
-                self._trace_span = None
+                trace_span = _HTTP_SPAN.get()
+                trace_span.tags["http.error_code"] = ex.__class__.__name__
+                if trace_span.end_time is None:
+                    trace_span.close()
                 raise
 
         return _func
 
-    def _capture_request_body(self, body):
+    def _capture_request_body(self, trace_span, body):
         if not body:
             return
         if not self.should_monitor_request_response:
             return
         if len(body) > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
                 "INPUT_BODY_TOO_LARGE",
-                self._trace_span,
+                trace_span,
             )
             return
         try:
-            self._trace_span.input = body.decode("utf-8")
+            trace_span.input = body.decode("utf-8")
         except Exception:
             pass
 
     def _instrumented_getresponse(self):
         def _func(_self, *args, **kwargs):
-            if not self._trace_span:
+            trace_span = _HTTP_SPAN.get()
+            if _self._sls_ignore or not trace_span:
                 return self._original_getresponse(_self, *args, **kwargs)
 
             try:
                 response = self._original_getresponse(_self, *args, **kwargs)
-                self._trace_span.tags["http.status_code"] = response.status
-                self._capture_response_body(response)
+                trace_span.tags["http.status_code"] = response.status
+                self._capture_response_body(trace_span, response)
                 return response
             finally:
-                if self._trace_span.end_time is None:
-                    self._trace_span.close()
+                if trace_span.end_time is None:
+                    trace_span.close()
 
         return _func
 
-    def _capture_response_body(self, response):
+    def _capture_response_body(self, trace_span, response):
         if not self.should_monitor_request_response:
             return
         if response.length > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
                 "OUTPUT_BODY_TOO_LARGE",
-                self._trace_span,
+                trace_span,
             )
             return
         try:
             response_body = response.peek()
             if response_body:
-                self._trace_span.output = response_body.decode("utf-8")
+                trace_span.output = response_body.decode("utf-8")
         except Exception as ex:
             report_error(ex)
 
     def _install(self):
         self._original_request = self._module.client.HTTPConnection.request
         self._original_getresponse = self._module.client.HTTPConnection.getresponse
         self._module.client.HTTPConnection.request = self._instrumented_request()
```

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/name.py` & `serverless-sdk-0.4.1/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.1/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.1/sls_sdk/lib/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,16 @@
 
         with self._lock:
             if name not in self:
                 super().__setitem__(name, value)
                 return
 
             current: ValidTags = self[name]
-
-            if isinstance(current, list):
-                if value != current:
-                    return
+            if value == current:
+                return
 
         raise DuplicateTraceSpanName(f"Cannot set tag: Tag {name} is already set")
 
     def set(self, key: str, value: ValidTags):
         try:
             self._set(key, value)
         except Exception as ex:
```

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.1/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.1/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.1/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.0/tests/test_sdk.py` & `serverless-sdk-0.4.1/tests/test_sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,7 +210,28 @@
     assert sdk._settings.disable_captured_events_stdout
     assert sdk._settings.disable_python_log_monitoring
     assert sdk._settings.disable_request_response_monitoring
     assert sdk._is_dev_mode
     assert sdk._is_debug_mode
 
     sdk._settings = _settings
+
+
+def test_initialize_extension(sdk: ServerlessSdk):
+    # given
+    sdk._initialize_extension = MagicMock()
+
+    # when
+    sdk._is_initialized = False
+    sdk._initialize(
+        "foo",
+        org_id="test",
+        disable_captured_events_stdout=True,
+        disable_python_log_monitoring=True,
+        disable_request_response_monitoring=True,
+        disable_http_monitoring=True,
+        disable_flask_monitoring=True,
+        bar="baz",
+    )
+
+    # then
+    sdk._initialize_extension.assert_called_once_with("foo", bar="baz")
```

### Comparing `serverless-sdk-0.4.0/tests/test_thread_safety.py` & `serverless-sdk-0.4.1/tests/test_thread_safety.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from __future__ import annotations
 from time import sleep
 import concurrent.futures
 import asyncio
 import random
 import pytest
+from pytest_httpserver import HTTPServer
+from werkzeug.wrappers import Request, Response
+
+SMALL_REQUEST_PAYLOAD = b"a"
+SMALL_RESPONSE_PAYLOAD = b"r"
 
 
 def print_spans(root, length=100):
     # normalize start and end times within [0, length]
     offset = root.start_time
     for span in root.spans:
         span.end_time -= offset
@@ -279,7 +284,60 @@
     with concurrent.futures.ThreadPoolExecutor(max_workers=parallelism) as executor:
         futures = [executor.submit(_set_tag_and_sleep, i) for i in range(parallelism)]
         for future in concurrent.futures.as_completed(futures):
             assert future.exception() is None
 
     # then
     assert len(sdk._custom_tags) == parallelism * scale
+
+
+@pytest.mark.parametrize(
+    "request_body,response_body",
+    [
+        (SMALL_REQUEST_PAYLOAD, SMALL_RESPONSE_PAYLOAD),
+    ],
+)
+def test_instrument_requests_multithreaded(
+    instrumented_sdk, httpserver: HTTPServer, request_body, response_body
+):
+    # given
+    def handler(request: Request):
+        return Response(response_body)
+
+    httpserver.expect_request("/foo/bar").respond_with_handler(handler)
+
+    root = instrumented_sdk._create_trace_span("rootspan")
+    parallelism = 5
+
+    # when
+    import requests
+
+    def _run():
+        requests.get(
+            httpserver.url_for("/foo/bar?baz=qux"),
+            headers={"User-Agent": "foo"},
+            data=request_body,
+        )
+
+    with concurrent.futures.ThreadPoolExecutor(max_workers=parallelism) as executor:
+        futures = [executor.submit(_run) for _i in range(parallelism)]
+        for future in concurrent.futures.as_completed(futures):
+            assert future.exception() is None
+
+    # then
+    assert len(root.spans) == parallelism + 1
+    for span in root.spans[1:]:
+        assert span.name == "python.http.request"
+        assert (
+            span.tags.items()
+            >= dict(
+                {
+                    "http.method": "GET",
+                    "http.protocol": "HTTP/1.1",
+                    "http.host": f"127.0.0.1:{httpserver.port}",
+                    "http.path": "/foo/bar",
+                    "http.query_parameter_names": ["baz"],
+                    "http.status_code": 200,
+                }
+            ).items()
+        )
+        assert "User-Agent" in span.tags["http.request_header_names"]
```

