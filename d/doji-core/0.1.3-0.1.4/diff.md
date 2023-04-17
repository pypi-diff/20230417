# Comparing `tmp/doji_core-0.1.3.tar.gz` & `tmp/doji_core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doji_core-0.1.3.tar", max compression
+gzip compressed data, was "doji_core-0.1.4.tar", max compression
```

## Comparing `doji_core-0.1.3.tar` & `doji_core-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.3/LICENSE
--rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.3/doji/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.3/doji/core/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.3/doji/core/api/classes/__init__.py
--rw-r--r--   0        0        0     6129 2023-04-16 17:22:15.958372 doji_core-0.1.3/doji/core/api/classes/api.py
--rw-r--r--   0        0        0     4143 2023-04-16 17:21:26.338411 doji_core-0.1.3/doji/core/api/classes/api_response.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/api/mixins/__init__.py
--rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/api/mixins/api_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/asset/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/asset/classes/__init__.py
--rw-r--r--   0        0        0     3050 2023-04-16 14:02:21.510452 doji_core-0.1.3/doji/core/asset/classes/asset.py
--rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.3/doji/core/asset/classes/asset_instances.py
--rw-r--r--   0        0        0     4519 2023-04-16 14:09:13.680598 doji_core-0.1.3/doji/core/asset/classes/asset_pair.py
--rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.3/doji/core/asset/classes/asset_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/asset/mixins/__init__.py
--rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.3/doji/core/asset/mixins/asset_pairs_mixin.py
--rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.3/doji/core/asset/mixins/assets_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency.py
--rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency_instances.py
--rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency_pair.py
--rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/mixins/__init__.py
--rw-r--r--   0        0        0    14781 2023-04-16 17:29:04.462159 doji_core-0.1.3/doji/core/currency/mixins/currencies_mixin.py
--rw-r--r--   0        0        0    10226 2023-04-16 17:29:13.146156 doji_core-0.1.3/doji/core/currency/mixins/currency_pairs_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/exchange/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/exchange/classes/__init__.py
--rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.3/doji/core/exchange/classes/currency_exchange.py
--rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.3/doji/core/exchange/classes/exchange.py
--rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.3/doji/core/py.typed
--rw-r--r--   0        0        0     2690 2023-04-16 17:22:43.934352 doji_core-0.1.3/doji/core/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/utils/classes/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-16 14:01:48.390107 doji_core-0.1.3/doji/core/utils/classes/instance.py
--rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.3/doji/core/utils/classes/instances.py
--rw-r--r--   0        0        0      544 2023-04-16 17:36:31.926052 doji_core-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 doji_core-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.4/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.4/doji/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.4/doji/core/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.4/doji/core/api/classes/__init__.py
+-rw-r--r--   0        0        0     6129 2023-04-16 17:22:15.958372 doji_core-0.1.4/doji/core/api/classes/api.py
+-rw-r--r--   0        0        0     6368 2023-04-17 14:24:09.341628 doji_core-0.1.4/doji/core/api/classes/api_response.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/api/mixins/__init__.py
+-rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/api/mixins/api_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/asset/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/asset/classes/__init__.py
+-rw-r--r--   0        0        0     2417 2023-04-17 13:37:12.266329 doji_core-0.1.4/doji/core/asset/classes/asset.py
+-rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.4/doji/core/asset/classes/asset_instances.py
+-rw-r--r--   0        0        0     3841 2023-04-17 13:37:32.636002 doji_core-0.1.4/doji/core/asset/classes/asset_pair.py
+-rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.4/doji/core/asset/classes/asset_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/asset/mixins/__init__.py
+-rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.4/doji/core/asset/mixins/asset_pairs_mixin.py
+-rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.4/doji/core/asset/mixins/assets_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/currency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/currency/classes/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/currency/classes/currency.py
+-rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/currency/classes/currency_instances.py
+-rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/currency/classes/currency_pair.py
+-rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/currency/classes/currency_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/currency/mixins/__init__.py
+-rw-r--r--   0        0        0    14781 2023-04-16 17:29:04.462159 doji_core-0.1.4/doji/core/currency/mixins/currencies_mixin.py
+-rw-r--r--   0        0        0    10226 2023-04-16 17:29:13.146156 doji_core-0.1.4/doji/core/currency/mixins/currency_pairs_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/exchange/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/exchange/classes/__init__.py
+-rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.4/doji/core/exchange/classes/currency_exchange.py
+-rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.4/doji/core/exchange/classes/exchange.py
+-rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.4/doji/core/py.typed
+-rw-r--r--   0        0        0     2719 2023-04-17 14:24:33.933160 doji_core-0.1.4/doji/core/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.4/doji/core/utils/classes/__init__.py
+-rw-r--r--   0        0        0     3985 2023-04-17 14:05:18.816166 doji_core-0.1.4/doji/core/utils/classes/instance.py
+-rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.4/doji/core/utils/classes/instances.py
+-rw-r--r--   0        0        0      565 2023-04-17 14:25:42.812090 doji_core-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      724 1970-01-01 00:00:00.000000 doji_core-0.1.4/PKG-INFO
```

### Comparing `doji_core-0.1.3/LICENSE` & `doji_core-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/api/classes/api.py` & `doji_core-0.1.4/doji/core/api/classes/api.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/api/mixins/api_mixin.py` & `doji_core-0.1.4/doji/core/api/mixins/api_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/asset/classes/asset.py` & `doji_core-0.1.4/doji/core/asset/classes/asset.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,24 +17,14 @@
     # │ CLASS ATTRIBUTES
     # └─────────────────────────────────────────────────────────────────────────────────
 
     # Declare type of code
     code: str
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
-    # │ __INIT__
-    # └─────────────────────────────────────────────────────────────────────────────────
-
-    def __init__(self, code: str):
-        """Init Method"""
-
-        # Set code
-        self.code = code
-
-    # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ __STR__
     # └─────────────────────────────────────────────────────────────────────────────────
 
     def __str__(self) -> str:
         """String Method"""
 
         # Return code
```

### Comparing `doji_core-0.1.3/doji/core/asset/classes/asset_instances.py` & `doji_core-0.1.4/doji/core/asset/classes/asset_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/asset/classes/asset_pair.py` & `doji_core-0.1.4/doji/core/asset/classes/asset_pair.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,25 +27,14 @@
     # └─────────────────────────────────────────────────────────────────────────────────
 
     # Declare type of base and quote
     base: T
     quote: T
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
-    # │ __INIT__
-    # └─────────────────────────────────────────────────────────────────────────────────
-
-    def __init__(self, base: T, quote: T):
-        """Init Method"""
-
-        # Set base and quote
-        self.base = base
-        self.quote = quote
-
-    # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ __STR__
     # └─────────────────────────────────────────────────────────────────────────────────
 
     def __str__(self) -> str:
         """String Method"""
 
         # Return symbol
```

### Comparing `doji_core-0.1.3/doji/core/asset/classes/asset_pair_instances.py` & `doji_core-0.1.4/doji/core/asset/classes/asset_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/asset/mixins/asset_pairs_mixin.py` & `doji_core-0.1.4/doji/core/asset/mixins/asset_pairs_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/asset/mixins/assets_mixin.py` & `doji_core-0.1.4/doji/core/asset/mixins/assets_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/currency/classes/currency.py` & `doji_core-0.1.4/doji/core/currency/classes/currency.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/currency/classes/currency_instances.py` & `doji_core-0.1.4/doji/core/currency/classes/currency_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/currency/classes/currency_pair.py` & `doji_core-0.1.4/doji/core/currency/classes/currency_pair.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/currency/classes/currency_pair_instances.py` & `doji_core-0.1.4/doji/core/currency/classes/currency_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/currency/mixins/currencies_mixin.py` & `doji_core-0.1.4/doji/core/currency/mixins/currencies_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/currency/mixins/currency_pairs_mixin.py` & `doji_core-0.1.4/doji/core/currency/mixins/currency_pairs_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/exchange/classes/currency_exchange.py` & `doji_core-0.1.4/doji/core/exchange/classes/currency_exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/exchange/classes/exchange.py` & `doji_core-0.1.4/doji/core/exchange/classes/exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/doji/core/types/__init__.py` & `doji_core-0.1.4/doji/core/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ GENERAL IMPORTS
 # └─────────────────────────────────────────────────────────────────────────────────────
 
-from typing import Any
+from typing import Any, Union
 
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ PROJECT IMPORTS
 # └─────────────────────────────────────────────────────────────────────────────────────
 
-from doji.core.api.classes.api_response import APIResponse  # noqa: F401
+from doji.core.api.classes.api_response import APIResponse as APIResponse  # noqa: F401
 
 
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ ARGS AND KWARGS
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 # Define a generic Args type
@@ -25,14 +25,14 @@
 # │ JSON
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 # Define a generic JSON value type
 JSONValue = str | int | float | bool | None
 
 # Define a generic JSON dict type
-JSONDict = dict[str, JSONValue | "JSON" | list["JSON"]]
+JSONDict = dict[str, Union[JSONValue, "JSON", list["JSON"]]]
 
-# Define a generic JSON array type
-JSONArray = list[JSONValue | "JSON" | JSONDict]
+# Define a generic JSON list type
+JSONList = list[Union[JSONValue, "JSON", JSONDict]]
 
 # Define a generic JSON type
-JSON = JSONValue | JSONDict | JSONArray
+JSON = JSONValue | JSONDict | JSONList
```

### Comparing `doji_core-0.1.3/doji/core/utils/classes/instances.py` & `doji_core-0.1.4/doji/core/utils/classes/instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.3/pyproject.toml` & `doji_core-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "doji-core"
-version = "0.1.3"
+version = "0.1.4"
 description = "A repository for Doji, a trade analytics suite written in Python."
 authors = ["Sean O'Leary <seamicole@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "doji"}]
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.4"
+pydantic = "^1.10.7"
 python = "^3.10"
 requests = "^2.28.2"
 types-requests = "^2.28.11.17"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
```

### Comparing `doji_core-0.1.3/PKG-INFO` & `doji_core-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: doji-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: A repository for Doji, a trade analytics suite written in Python.
 License: MIT
 Author: Sean O'Leary
 Author-email: seamicole@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: types-requests (>=2.28.11.17,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 # doji-core
 A repository for Doji, a trade analytics suite written in Python.
```

