# Comparing `tmp/slink_api-0.1.6.tar.gz` & `tmp/slink_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slink_api-0.1.6.tar", max compression
+gzip compressed data, was "slink_api-0.1.7.tar", max compression
```

## Comparing `slink_api-0.1.6.tar` & `slink_api-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3679 2023-04-13 06:52:25.996761 slink_api-0.1.6/README.md
--rw-r--r--   0        0        0      640 2023-04-13 06:52:42.953208 slink_api-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-13 06:52:25.996761 slink_api-0.1.6/slink/__init__.py
--rw-r--r--   0        0        0     2159 2023-04-13 06:52:25.996761 slink_api-0.1.6/slink/api.py
--rw-r--r--   0        0        0     4043 2023-04-13 06:52:25.996761 slink_api-0.1.6/slink/decorators.py
--rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 slink_api-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3679 2023-04-17 10:20:57.534362 slink_api-0.1.7/README.md
+-rw-r--r--   0        0        0      640 2023-04-17 10:21:11.975267 slink_api-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-17 10:20:57.534362 slink_api-0.1.7/slink/__init__.py
+-rw-r--r--   0        0        0     2263 2023-04-17 10:20:57.534362 slink_api-0.1.7/slink/api.py
+-rw-r--r--   0        0        0     4227 2023-04-17 10:20:57.534362 slink_api-0.1.7/slink/decorators.py
+-rw-r--r--   0        0        0     4381 1970-01-01 00:00:00.000000 slink_api-0.1.7/PKG-INFO
```

### Comparing `slink_api-0.1.6/README.md` & `slink_api-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `slink_api-0.1.6/pyproject.toml` & `slink_api-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slink-api"
-version = "v0.1.6"
+version = "v0.1.7"
 description = "Simple and expressive REST clients without the fuss"
 authors = ["James Lloyd <james.allan.lloyd@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/james-allan-lloyd/slink"
 packages = [{include = "slink"}]
 
 [tool.poetry.dependencies]
```

### Comparing `slink_api-0.1.6/slink/api.py` & `slink_api-0.1.7/slink/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import functools
-from typing import Any, Dict, List, Optional, Protocol, Generator, Tuple
+from typing import Dict, List, Optional, Protocol, Generator, Tuple, Union
 from urllib.parse import urljoin, urlparse
 import requests
 import inspect
 
 
 class Api:
     def __init__(self, base_url="", session: Optional[requests.Session] = None) -> None:
@@ -45,25 +44,34 @@
 
 class Body:
     pass
 
 
 class DecoratorParser:
     def __init__(self, kwargs) -> None:
-        self.queryParams = {k: v.alias if len(v.alias) else k for k, v in kwargs.items() if type(v) == Query}
+        self.queryParams = {
+            k: v.alias if len(v.alias) else k
+            for k, v in kwargs.items()
+            if type(v) == Query
+        }
         self.bodyParams = [k for k, v in kwargs.items() if type(v) == Body]
 
     def parse(self, args, kwargs) -> Tuple[Dict[str, str], List[str]]:
         if len(args):
             raise Exception("Must use keyword arguments in api calls")
 
         params = {
             self.queryParams[k]: v for k, v in kwargs.items() if k in self.queryParams
         }
         body = [v for k, v in kwargs.items() if k in self.bodyParams]
 
         return params, body
 
 
+PagerGeneratorType = Generator[
+    Union[Tuple[str, dict], Tuple[str, None]], requests.Response, None
+]
+
+
 class Pager(Protocol):
-    def pages(self, url: str) -> Generator[Tuple[str, dict], requests.Response, None]:  # type: ignore
+    def pages(self, url: str) -> PagerGeneratorType:  # type: ignore
         pass
```

### Comparing `slink_api-0.1.6/slink/decorators.py` & `slink_api-0.1.7/slink/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,21 +97,23 @@
         def call_get(self: Api, *args, **kwargs):
             params, body = decoratorParser.parse(args, kwargs)
             url = self.construct_url(url_template, kwargs)
             page_generator = pager_actual.pages(url)
             response = None
             try:
                 while True:
-                    url, page_params = (
-                        page_generator.send(response)
-                        if response
-                        else next(page_generator)
-                    )
-                    params.update(page_params)
-                    response = self.session.get(url, params=params)
+                    page_params = None
+                    if response is not None:
+                        url, page_params = page_generator.send(response)
+                    elif next_result := next(page_generator):
+                        assert next_result
+                        url, page_params = next_result
+                    if page_params is not None:
+                        page_params = {**params, **page_params}
+                    response = self.session.get(url, params=page_params)
                     assert response
                     self._response = response
                     self.check_response()
                     for value in get_impl(self, *args, **kwargs):
                         yield value
             except StopIteration:
                 pass
```

### Comparing `slink_api-0.1.6/PKG-INFO` & `slink_api-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slink-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple and expressive REST clients without the fuss
 Home-page: https://github.com/james-allan-lloyd/slink
 Author: James Lloyd
 Author-email: james.allan.lloyd@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

