# Comparing `tmp/combadge-0.1.0rc3.tar.gz` & `tmp/combadge-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combadge-0.1.0rc3.tar", max compression
+gzip compressed data, was "combadge-0.1.0rc4.tar", max compression
```

## Comparing `combadge-0.1.0rc3.tar` & `combadge-0.1.0rc4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11350 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/LICENSE
--rw-r--r--   0        0        0     2682 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/README.md
--rw-r--r--   0        0        0        0 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/__init__.py
--rw-r--r--   0        0        0     1259 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/backend.py
--rw-r--r--   0        0        0     3377 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/binder.py
--rw-r--r--   0        0        0     3016 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/markers/__init__.py
--rw-r--r--   0        0        0     2568 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/markers/method.py
--rw-r--r--   0        0        0      902 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/markers/parameter.py
--rw-r--r--   0        0        0     1907 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/request.py
--rw-r--r--   0        0        0     6814 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/response.py
--rw-r--r--   0        0        0     1830 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/service.py
--rw-r--r--   0        0        0     2372 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/signature.py
--rw-r--r--   0        0        0      343 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/typevars.py
--rw-r--r--   0        0        0      203 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/core/warnings.py
--rw-r--r--   0        0        0        0 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/py.typed
--rw-r--r--   0        0        0       50 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/support/__init__.py
--rw-r--r--   0        0        0       40 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/support/http/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/support/http/abc.py
--rw-r--r--   0        0        0      807 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/support/http/aliases.py
--rw-r--r--   0        0        0      264 2023-04-14 15:10:04.262491 combadge-0.1.0rc3/combadge/support/http/headers.py
--rw-r--r--   0        0        0     7338 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/http/markers.py
--rw-r--r--   0        0        0      398 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/http/request.py
--rw-r--r--   0        0        0      124 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/httpx/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/httpx/backends/__init__.py
--rw-r--r--   0        0        0     3337 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/httpx/backends/async_.py
--rw-r--r--   0        0        0     1542 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/httpx/backends/base.py
--rw-r--r--   0        0        0     3232 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/httpx/backends/sync.py
--rw-r--r--   0        0        0        0 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/shared/__init__.py
--rw-r--r--   0        0        0      348 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/shared/async_.py
--rw-r--r--   0        0        0      308 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/shared/contextlib.py
--rw-r--r--   0        0        0      338 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/shared/sync.py
--rw-r--r--   0        0        0       39 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/soap/__init__.py
--rw-r--r--   0        0        0      256 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/soap/abc.py
--rw-r--r--   0        0        0     2198 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/soap/markers.py
--rw-r--r--   0        0        0      212 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/soap/request.py
--rw-r--r--   0        0        0      741 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/soap/response.py
--rw-r--r--   0        0        0      131 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/zeep/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/zeep/backends/__init__.py
--rw-r--r--   0        0        0     3475 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/zeep/backends/async_.py
--rw-r--r--   0        0        0     3059 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/zeep/backends/base.py
--rw-r--r--   0        0        0     3334 2023-04-14 15:10:04.266491 combadge-0.1.0rc3/combadge/support/zeep/backends/sync.py
--rw-r--r--   0        0        0     3397 2023-04-14 15:10:18.926789 combadge-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 combadge-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/LICENSE
+-rw-r--r--   0        0        0     2682 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/__init__.py
+-rw-r--r--   0        0        0     1259 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/backend.py
+-rw-r--r--   0        0        0     3377 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/binder.py
+-rw-r--r--   0        0        0     3016 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/markers/__init__.py
+-rw-r--r--   0        0        0     2568 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/markers/method.py
+-rw-r--r--   0        0        0      902 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/markers/parameter.py
+-rw-r--r--   0        0        0     1907 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/request.py
+-rw-r--r--   0        0        0     6814 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/response.py
+-rw-r--r--   0        0        0     1830 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/service.py
+-rw-r--r--   0        0        0     2372 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/signature.py
+-rw-r--r--   0        0        0      343 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/typevars.py
+-rw-r--r--   0        0        0      203 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/core/warnings.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/py.typed
+-rw-r--r--   0        0        0       50 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/http/__init__.py
+-rw-r--r--   0        0        0     1470 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/http/abc.py
+-rw-r--r--   0        0        0      807 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/http/aliases.py
+-rw-r--r--   0        0        0      264 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/http/headers.py
+-rw-r--r--   0        0        0     7338 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/http/markers.py
+-rw-r--r--   0        0        0      398 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/http/request.py
+-rw-r--r--   0        0        0      124 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/httpx/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/httpx/backends/__init__.py
+-rw-r--r--   0        0        0     3374 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/httpx/backends/async_.py
+-rw-r--r--   0        0        0     1542 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/httpx/backends/base.py
+-rw-r--r--   0        0        0     3232 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/httpx/backends/sync.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/shared/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/shared/async_.py
+-rw-r--r--   0        0        0      308 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/shared/contextlib.py
+-rw-r--r--   0        0        0      338 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/shared/sync.py
+-rw-r--r--   0        0        0       39 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/soap/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/soap/abc.py
+-rw-r--r--   0        0        0     2198 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/soap/markers.py
+-rw-r--r--   0        0        0      212 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/soap/request.py
+-rw-r--r--   0        0        0      741 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/soap/response.py
+-rw-r--r--   0        0        0      131 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/zeep/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/zeep/backends/__init__.py
+-rw-r--r--   0        0        0     3475 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/zeep/backends/async_.py
+-rw-r--r--   0        0        0     3059 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/zeep/backends/base.py
+-rw-r--r--   0        0        0     3334 2023-04-17 10:41:42.095448 combadge-0.1.0rc4/combadge/support/zeep/backends/sync.py
+-rw-r--r--   0        0        0     3397 2023-04-17 10:41:56.675319 combadge-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 combadge-0.1.0rc4/PKG-INFO
```

### Comparing `combadge-0.1.0rc3/LICENSE` & `combadge-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/README.md` & `combadge-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/backend.py` & `combadge-0.1.0rc4/combadge/core/backend.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/binder.py` & `combadge-0.1.0rc4/combadge/core/binder.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/interfaces.py` & `combadge-0.1.0rc4/combadge/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/markers/method.py` & `combadge-0.1.0rc4/combadge/core/markers/method.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/markers/parameter.py` & `combadge-0.1.0rc4/combadge/core/markers/parameter.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/request.py` & `combadge-0.1.0rc4/combadge/core/request.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/response.py` & `combadge-0.1.0rc4/combadge/core/response.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/service.py` & `combadge-0.1.0rc4/combadge/core/service.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/core/signature.py` & `combadge-0.1.0rc4/combadge/core/signature.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/http/abc.py` & `combadge-0.1.0rc4/combadge/support/http/abc.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/http/aliases.py` & `combadge-0.1.0rc4/combadge/support/http/aliases.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/http/markers.py` & `combadge-0.1.0rc4/combadge/support/http/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/httpx/backends/async_.py` & `combadge-0.1.0rc4/combadge/support/httpx/backends/async_.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         """
         response: Response = await self._client.request(
             request.method,
             request.path,
             json=request.json_,
             data=request.form_data,
             params=request.query_params,
+            headers=request.headers,
         )
         if self._raise_for_status:
             response.raise_for_status()
         return self._parse_response(response, response_type)
 
     @classmethod
     def bind_method(cls, signature: Signature) -> CallServiceMethod[HttpxBackend]:  # noqa: D102
```

### Comparing `combadge-0.1.0rc3/combadge/support/httpx/backends/base.py` & `combadge-0.1.0rc4/combadge/support/httpx/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/httpx/backends/sync.py` & `combadge-0.1.0rc4/combadge/support/httpx/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/soap/markers.py` & `combadge-0.1.0rc4/combadge/support/soap/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/soap/response.py` & `combadge-0.1.0rc4/combadge/support/soap/response.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/zeep/backends/async_.py` & `combadge-0.1.0rc4/combadge/support/zeep/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/zeep/backends/base.py` & `combadge-0.1.0rc4/combadge/support/zeep/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/combadge/support/zeep/backends/sync.py` & `combadge-0.1.0rc4/combadge/support/zeep/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc3/pyproject.toml` & `combadge-0.1.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 description = "Generic API client based on Pydantic"
 keywords = ["api", "api-client", "pydantic"]
 license = "Apache-2.0"
 name = "combadge"
 readme = "README.md"
 repository = "https://github.com/kpn/combadge"
-version = "0.1.0rc3"
+version = "0.1.0rc4"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `combadge-0.1.0rc3/PKG-INFO` & `combadge-0.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combadge
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Generic API client based on Pydantic
 Home-page: https://github.com/kpn/combadge
 License: Apache-2.0
 Keywords: api,api-client,pydantic
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.1,<4.0.0
```

