# Comparing `tmp/surquest_fastapi_utils-0.2.0rc1.tar.gz` & `tmp/surquest_fastapi_utils-0.2.1.tar.gz`

## Comparing `surquest_fastapi_utils-0.2.0rc1.tar` & `surquest_fastapi_utils-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/package.base.dockerfile
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/.github/workflows/test.yml
--rw-r--r--   0        0        0    43478 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/assets/img/logs.png
--rw-r--r--   0        0        0    66316 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/assets/img/trace.png
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/base.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/info.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/message.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/metadata.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/responses.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/status.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/__init__.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/args.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/route.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/GCP.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/__init__.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/catcher.py
--rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/formatter.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/http_context.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/logging.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/middleware.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/tracer.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/test/pytest.ini
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/test/utils/test_catcher.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/package.base.dockerfile
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0    43478 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/assets/img/logs.png
+-rw-r--r--   0        0        0    66316 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/assets/img/trace.png
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/base.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/info.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/message.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/metadata.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/responses.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/status.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/__init__.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/args.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/route.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/GCP.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/__init__.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/catcher.py
+-rw-r--r--   0        0        0     6510 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/formatter.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/http_context.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/logging.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/middleware.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/tracer.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/test/pytest.ini
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/test/utils/test_catcher.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/README.md
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.1/PKG-INFO
```

### Comparing `surquest_fastapi_utils-0.2.0rc1/package.base.dockerfile` & `surquest_fastapi_utils-0.2.1/package.base.dockerfile`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/.github/workflows/release.yml` & `surquest_fastapi_utils-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/.github/workflows/test.yml` & `surquest_fastapi_utils-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/assets/img/logs.png` & `surquest_fastapi_utils-0.2.1/assets/img/logs.png`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/assets/img/trace.png` & `surquest_fastapi_utils-0.2.1/assets/img/trace.png`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/metadata.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/metadata.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/responses.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/schemas/responses/responses.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/args.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/args.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/route.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/route.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/catcher.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/catcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
     "Catcher",
     "catch_validation_exceptions",
     "catch_http_exceptions"
 ]
 
 
 async def catch_validation_exceptions(request: Request, exc):
-    return Catcher.catch_validation_error(request, exc)
+    return await Catcher.catch_validation_error(request, exc)
 
 
 async def catch_http_exceptions(request: Request, exc):
-    return Catcher.catch_http_exception(request, exc)
+    return await Catcher.catch_http_exception(request, exc)
 
 
 class Catcher:
 
     OUPS = "Oups, something went wrong"
 
     @classmethod
```

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/formatter.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,18 +103,23 @@
 
         # convert log record to dictionary compatible with GCP LogRecord format
         log = self.format_log_entry(record)
 
         # if log record is an error add @type attribute to comply with GCP Error Reporting format
         if record.levelno >= logging.ERROR:
 
+            tb = [] # empty traceback
+            if "ctx" in log and "traceback" in log["ctx"]:
+                # get traceback from log record if present
+                tb = log["ctx"]["traceback"]
+
             log["@type"] = self.GCP_LOG_TYPE
             log["message"] = self.format_stack_trace(
                 message=log["message"],
-                traceback=log["ctx"]["traceback"]
+                traceback=tb
             )
             log["serviceContext"] = self.get_service_context()
             log["context"] = {
                 "httpRequest": self.get_http_request_context(),
                 "reportLocation": self.get_report_location(record),
                 "user": self.get_user()
             }
```

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/http_context.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/http_context.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/logging.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/logging.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/middleware.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/middleware.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/tracer.py` & `surquest_fastapi_utils-0.2.1/surquest/fastapi/utils/GCP/tracer.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/test/utils/test_catcher.py` & `surquest_fastapi_utils-0.2.1/test/utils/test_catcher.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/.gitignore` & `surquest_fastapi_utils-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/LICENSE` & `surquest_fastapi_utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/README.md` & `surquest_fastapi_utils-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.2.0rc1/pyproject.toml` & `surquest_fastapi_utils-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "surquest-fastapi-utils"
-version = "0.2.0rc1"
+version = "0.2.1"
 description = "This project provides collection of utilities for FastAPI framework as: Catcher, Middleware, etc."
 authors = [
     {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
 ]
 readme = "README.md"
 dependencies = [
     "fastapi >= 0.81.0",
```

### Comparing `surquest_fastapi_utils-0.2.0rc1/PKG-INFO` & `surquest_fastapi_utils-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surquest-fastapi-utils
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: This project provides collection of utilities for FastAPI framework as: Catcher, Middleware, etc.
 Project-URL: Homepage, https://github.com/surquest/python-fastapi-utils
 Project-URL: Bug Tracker, https://github.com/surquest/python-fastapi-utils/issues
 Author-email: Michal Švarc <michal.svarc@surquest.com>
 License-File: LICENSE
 Requires-Dist: fastapi>=0.81.0
 Requires-Dist: google-cloud-logging>=3.1.0
```

