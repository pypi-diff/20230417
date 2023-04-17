# Comparing `tmp/bittrade_luno_websocket-0.1.1.tar.gz` & `tmp/bittrade_luno_websocket-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittrade_luno_websocket-0.1.1.tar", max compression
+gzip compressed data, was "bittrade_luno_websocket-0.1.2.tar", max compression
```

## Comparing `bittrade_luno_websocket-0.1.1.tar` & `bittrade_luno_websocket-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566521 bittrade_luno_websocket-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566632 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/__init__.py
--rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566732 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/channels/__init__.py
--rw-r--r--   0        0        0    12996 2023-03-23 09:09:52.264805 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/channels/orderbook.py
--rw-r--r--   0        0        0        0 2023-03-11 21:05:54.544362 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/__init__.py
--rw-r--r--   0        0        0     1374 2023-03-11 21:05:54.545267 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/authenticate.py
--rw-r--r--   0        0        0     3525 2023-03-13 09:43:24.335646 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/generic.py
--rw-r--r--   0        0        0     2401 2023-03-13 09:43:24.335922 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/http.py
--rw-r--r--   0        0        0      720 2023-03-13 09:43:24.336282 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/public.py
--rw-r--r--   0        0        0      102 2023-03-13 09:43:24.336634 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/__init__.py
--rw-r--r--   0        0        0      219 2023-03-23 09:08:33.508837 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/endpoints.py
--rw-r--r--   0        0        0      690 2023-03-11 21:05:54.548298 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/enhanced_websocket.py
--rw-r--r--   0        0        0      203 2023-03-13 09:43:24.337178 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/orderbook.py
--rw-r--r--   0        0        0      398 2023-03-13 09:43:24.337444 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/request.py
--rw-r--r--   0        0        0      847 2023-03-13 09:43:24.337668 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/response_message.py
--rw-r--r--   0        0        0        0 2023-03-13 09:43:24.337809 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/rest/__init__.py
--rw-r--r--   0        0        0     1100 2023-03-23 09:08:33.509055 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/rest/get_order.py
--rw-r--r--   0        0        0      312 2023-03-13 09:43:24.339575 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/rest/post_limit_order.py
--rw-r--r--   0        0        0      376 2023-03-23 09:08:33.509254 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/rest/post_market_order.py
--rw-r--r--   0        0        0      580 2023-03-23 09:08:33.509444 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/rest/get_book.py
--rw-r--r--   0        0        0      621 2023-03-23 09:08:33.509626 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/rest/get_order.py
--rw-r--r--   0        0        0     1041 2023-03-23 09:08:33.509783 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/rest/post_market_order.py
--rw-r--r--   0        0        0      367 2023-03-13 09:43:24.340924 bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/signing/__init__.py
--rw-r--r--   0        0        0     1070 2023-03-23 09:09:58.095802 bittrade_luno_websocket-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.1/setup.py
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566521 bittrade_luno_websocket-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566632 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-23 05:51:40.566732 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/__init__.py
+-rw-r--r--   0        0        0    12996 2023-03-23 09:09:52.264805 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/orderbook.py
+-rw-r--r--   0        0        0     1838 2023-04-16 10:55:15.725467 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/user_stream.py
+-rw-r--r--   0        0        0        0 2023-03-11 21:05:54.544362 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/__init__.py
+-rw-r--r--   0        0        0     1374 2023-03-11 21:05:54.545267 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/authenticate.py
+-rw-r--r--   0        0        0     3525 2023-03-13 09:43:24.335646 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/generic.py
+-rw-r--r--   0        0        0     2401 2023-03-13 09:43:24.335922 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/http.py
+-rw-r--r--   0        0        0      720 2023-03-13 09:43:24.336282 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/public.py
+-rw-r--r--   0        0        0      102 2023-03-13 09:43:24.336634 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/__init__.py
+-rw-r--r--   0        0        0      300 2023-04-16 20:07:19.291721 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/endpoints.py
+-rw-r--r--   0        0        0      690 2023-03-11 21:05:54.548298 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/enhanced_websocket.py
+-rw-r--r--   0        0        0      203 2023-03-13 09:43:24.337178 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/orderbook.py
+-rw-r--r--   0        0        0      398 2023-03-13 09:43:24.337444 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/request.py
+-rw-r--r--   0        0        0      847 2023-03-13 09:43:24.337668 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/response_message.py
+-rw-r--r--   0        0        0        0 2023-03-13 09:43:24.337809 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/__init__.py
+-rw-r--r--   0        0        0      470 2023-04-16 20:12:18.269435 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/balance.py
+-rw-r--r--   0        0        0     1100 2023-03-23 09:08:33.509055 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/get_order.py
+-rw-r--r--   0        0        0     1236 2023-04-16 20:00:08.620775 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/order.py
+-rw-r--r--   0        0        0     1034 2023-04-17 04:25:05.453554 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/balance.py
+-rw-r--r--   0        0        0      580 2023-03-23 09:08:33.509444 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_book.py
+-rw-r--r--   0        0        0      621 2023-03-23 09:08:33.509626 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_order.py
+-rw-r--r--   0        0        0     1876 2023-04-17 04:24:16.695673 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/order.py
+-rw-r--r--   0        0        0      367 2023-03-13 09:43:24.340924 bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/signing/__init__.py
+-rw-r--r--   0        0        0     1070 2023-04-17 04:46:18.032120 bittrade_luno_websocket-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.2/setup.py
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 bittrade_luno_websocket-0.1.2/PKG-INFO
```

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/channels/orderbook.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/channels/orderbook.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/authenticate.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/authenticate.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/generic.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/generic.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/http.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/http.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/connection/public.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/connection/public.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/enhanced_websocket.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/response_message.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/response_message.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/models/rest/get_order.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/models/rest/get_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/rest/get_book.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_book.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/rest/get_order.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/get_order.py`

 * *Files identical despite different names*

### Comparing `bittrade_luno_websocket-0.1.1/bittrade_luno_websocket/rest/post_market_order.py` & `bittrade_luno_websocket-0.1.2/bittrade_luno_websocket/rest/order.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,60 @@
 import dataclasses
-from typing import Callable
+from typing import Any, Callable
 import reactivex
 import requests
-from bittrade_luno_websocket.models.rest.post_market_order import MarketOrderRequest, MarketOrderResponse
+from bittrade_luno_websocket.models.rest.order import (
+    OrderRequest,
+    MarketOrderRequest,
+    OrderResponse,
+)
 from bittrade_luno_websocket.connection.http import prepare_request, send_request
 from bittrade_luno_websocket.models import RequestMessage
 from bittrade_luno_websocket.models import endpoints
 from bittrade_luno_websocket.rest.get_order import get_order_http, GetOrderRequest
 from reactivex import operators, compose
 
 
-def post_market_order_http(request: MarketOrderRequest, add_token: Callable) -> reactivex.Observable[MarketOrderResponse]:
+def create_order_http_factory(
+    add_token: Callable,
+) -> Callable[[OrderRequest], reactivex.Observable[Any]]:
+    def create_order_http(request: OrderRequest) -> reactivex.Observable[OrderResponse]:
+        params = request.to_dict()
+        return send_request(
+            add_token(
+                prepare_request(
+                    RequestMessage(
+                        method="POST",
+                        endpoint=endpoints.Endpoints.POST_MARKET_ORDER
+                        if request.type == "market"
+                        else endpoints.Endpoints.POST_LIMIT_ORDER,
+                        params=params,
+                    )
+                )
+            )
+        )
+
+    return create_order_http
+
+
+def post_market_order_http(
+    request: MarketOrderRequest, add_token: Callable
+) -> reactivex.Observable[OrderResponse]:
     return send_request(
         add_token(
-            prepare_request(RequestMessage(
-            method="POST",
-            endpoint=endpoints.Endpoints.POST_MARKET_ORDER,
-            params=dataclasses.asdict(request),
+            prepare_request(
+                RequestMessage(
+                    method="POST",
+                    endpoint=endpoints.Endpoints.POST_MARKET_ORDER,
+                    params=dataclasses.asdict(request),
+                )
+            )
         )
-    )))
+    )
+
 
 def load_order_details(add_token: Callable):
     return compose(
-        operators.flat_map(lambda x: get_order_http(GetOrderRequest(id=x["order_id"]), add_token)),
+        operators.flat_map(
+            lambda x: get_order_http(GetOrderRequest(id=x["order_id"]), add_token)
+        ),
     )
```

### Comparing `bittrade_luno_websocket-0.1.1/pyproject.toml` & `bittrade_luno_websocket-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bittrade-luno-websocket"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Matt <matt@techspace.asia>"]
 readme = "README.md"
 packages = [{ include = "bittrade_luno_websocket" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `bittrade_luno_websocket-0.1.1/setup.py` & `bittrade_luno_websocket-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'reactivex>=4.0.4,<5.0.0',
  'requests>=2.28.2,<3.0.0',
  'returns>=0.19.0,<0.20.0',
  'websocket-client>=1.5.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'bittrade-luno-websocket',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '',
     'author': 'Matt',
     'author_email': 'matt@techspace.asia',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bittrade_luno_websocket-0.1.1/PKG-INFO` & `bittrade_luno_websocket-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittrade-luno-websocket
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Matt
 Author-email: matt@techspace.asia
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ccxt (>=2.7.91,<3.0.0)
```

