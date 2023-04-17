# Comparing `tmp/doji_core-0.1.2.tar.gz` & `tmp/doji_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doji_core-0.1.2.tar", max compression
+gzip compressed data, was "doji_core-0.1.3.tar", max compression
```

## Comparing `doji_core-0.1.2.tar` & `doji_core-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.2/LICENSE
--rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.2/doji/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.2/doji/core/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.2/doji/core/api/classes/__init__.py
--rw-r--r--   0        0        0     6102 2023-04-16 12:39:02.353036 doji_core-0.1.2/doji/core/api/classes/api.py
--rw-r--r--   0        0        0     4137 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/api/classes/response.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/api/mixins/__init__.py
--rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/api/mixins/api_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/asset/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/asset/classes/__init__.py
--rw-r--r--   0        0        0     3050 2023-04-16 14:02:21.510452 doji_core-0.1.2/doji/core/asset/classes/asset.py
--rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.2/doji/core/asset/classes/asset_instances.py
--rw-r--r--   0        0        0     4519 2023-04-16 14:09:13.680598 doji_core-0.1.2/doji/core/asset/classes/asset_pair.py
--rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.2/doji/core/asset/classes/asset_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/asset/mixins/__init__.py
--rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.2/doji/core/asset/mixins/asset_pairs_mixin.py
--rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.2/doji/core/asset/mixins/assets_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/__init__.py
--rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency.py
--rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency_instances.py
--rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency_pair.py
--rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/classes/currency_pair_instances.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/currency/mixins/__init__.py
--rw-r--r--   0        0        0    14713 2023-04-16 15:41:11.805369 doji_core-0.1.2/doji/core/currency/mixins/currencies_mixin.py
--rw-r--r--   0        0        0    10188 2023-04-16 15:47:25.691429 doji_core-0.1.2/doji/core/currency/mixins/currency_pairs_mixin.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/exchange/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/exchange/classes/__init__.py
--rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.2/doji/core/exchange/classes/currency_exchange.py
--rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.2/doji/core/exchange/classes/exchange.py
--rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.2/doji/core/py.typed
--rw-r--r--   0        0        0     2071 2023-04-16 16:30:03.427132 doji_core-0.1.2/doji/core/types/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.2/doji/core/utils/classes/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-16 14:01:48.390107 doji_core-0.1.2/doji/core/utils/classes/instance.py
--rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.2/doji/core/utils/classes/instances.py
--rw-r--r--   0        0        0      544 2023-04-16 16:30:21.175045 doji_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 doji_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-16 10:49:32.941115 doji_core-0.1.3/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-16 10:49:32.941115 doji_core-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.3/doji/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.3/doji/core/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.941115 doji_core-0.1.3/doji/core/api/classes/__init__.py
+-rw-r--r--   0        0        0     6129 2023-04-16 17:22:15.958372 doji_core-0.1.3/doji/core/api/classes/api.py
+-rw-r--r--   0        0        0     4143 2023-04-16 17:21:26.338411 doji_core-0.1.3/doji/core/api/classes/api_response.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/api/mixins/__init__.py
+-rw-r--r--   0        0        0     3303 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/api/mixins/api_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/asset/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/asset/classes/__init__.py
+-rw-r--r--   0        0        0     3050 2023-04-16 14:02:21.510452 doji_core-0.1.3/doji/core/asset/classes/asset.py
+-rw-r--r--   0        0        0     2603 2023-04-16 15:07:54.310882 doji_core-0.1.3/doji/core/asset/classes/asset_instances.py
+-rw-r--r--   0        0        0     4519 2023-04-16 14:09:13.680598 doji_core-0.1.3/doji/core/asset/classes/asset_pair.py
+-rw-r--r--   0        0        0     2641 2023-04-16 15:37:29.236623 doji_core-0.1.3/doji/core/asset/classes/asset_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/asset/mixins/__init__.py
+-rw-r--r--   0        0        0     6993 2023-04-16 15:19:48.797600 doji_core-0.1.3/doji/core/asset/mixins/asset_pairs_mixin.py
+-rw-r--r--   0        0        0     9416 2023-04-16 15:23:35.086566 doji_core-0.1.3/doji/core/asset/mixins/assets_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency.py
+-rw-r--r--   0        0        0     1348 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency_instances.py
+-rw-r--r--   0        0        0     1303 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency_pair.py
+-rw-r--r--   0        0        0     1388 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/classes/currency_pair_instances.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/currency/mixins/__init__.py
+-rw-r--r--   0        0        0    14781 2023-04-16 17:29:04.462159 doji_core-0.1.3/doji/core/currency/mixins/currencies_mixin.py
+-rw-r--r--   0        0        0    10226 2023-04-16 17:29:13.146156 doji_core-0.1.3/doji/core/currency/mixins/currency_pairs_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/exchange/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/exchange/classes/__init__.py
+-rw-r--r--   0        0        0     1586 2023-04-16 14:51:14.088258 doji_core-0.1.3/doji/core/exchange/classes/currency_exchange.py
+-rw-r--r--   0        0        0     4870 2023-04-16 14:51:38.852483 doji_core-0.1.3/doji/core/exchange/classes/exchange.py
+-rw-r--r--   0        0        0        0 2023-04-16 16:03:32.948981 doji_core-0.1.3/doji/core/py.typed
+-rw-r--r--   0        0        0     2690 2023-04-16 17:22:43.934352 doji_core-0.1.3/doji/core/types/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 10:49:32.945115 doji_core-0.1.3/doji/core/utils/classes/__init__.py
+-rw-r--r--   0        0        0     1470 2023-04-16 14:01:48.390107 doji_core-0.1.3/doji/core/utils/classes/instance.py
+-rw-r--r--   0        0        0     9168 2023-04-16 15:40:46.253260 doji_core-0.1.3/doji/core/utils/classes/instances.py
+-rw-r--r--   0        0        0      544 2023-04-16 17:36:31.926052 doji_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 doji_core-0.1.3/PKG-INFO
```

### Comparing `doji_core-0.1.2/LICENSE` & `doji_core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/api/classes/api.py` & `doji_core-0.1.3/doji/core/api/classes/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from json.decoder import JSONDecodeError
 from typing import Any
 
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ PROJECT IMPORTS
 # └─────────────────────────────────────────────────────────────────────────────────────
 
-from doji.core.api.classes.response import Response
+from doji.core.api.classes.api_response import APIResponse
 
 
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ API
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 
@@ -55,15 +55,15 @@
     # └─────────────────────────────────────────────────────────────────────────────────
 
     def get(
         self,
         *route: str,
         params: dict[str, Any] | None = None,
         base_url: str | None = None
-    ) -> Response:
+    ) -> APIResponse:
         """Makes a synchronous HTTP GET request"""
 
         # Initialize params
         params = params or {}
 
         # Construct URL
         url = self.construct_url(*route, base_url=base_url)
@@ -77,27 +77,27 @@
             json = response.json()
 
         # Handle JSONDecodeError
         except JSONDecodeError:
             # Set JSON data to None
             json = None
 
-        # Return response
-        return Response(response=response, json=json)
+        # Return API response
+        return APIResponse(response=response, json=json)
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ GET ASYNC
     # └─────────────────────────────────────────────────────────────────────────────────
 
     async def get_async(
         self,
         *route: str,
         params: dict[str, Any] | None = None,
         base_url: str | None = None
-    ) -> Response:
+    ) -> APIResponse:
         """Makes an asynchronous HTTP GET request"""
 
         # Initialize params
         params = params or {}
 
         # Construct URL
         url = self.construct_url(*route, base_url=base_url)
@@ -112,9 +112,9 @@
                     json = await response.json(content_type=None)
 
                 # Handle JSONDecodeError
                 except JSONDecodeError:
                     # Set JSON data to None
                     json = None
 
-        # Return response
-        return Response(response=response, json=json)
+        # Return API response
+        return APIResponse(response=response, json=json)
```

### Comparing `doji_core-0.1.2/doji/core/api/classes/response.py` & `doji_core-0.1.3/doji/core/api/classes/api_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 if TYPE_CHECKING:
     from doji.core.types import JSON
 
 
 # ┌─────────────────────────────────────────────────────────────────────────────────────
-# │ RESPONSE
+# │ API RESPONSE
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 
-class Response:
-    """A utility class that represents HTTP responses"""
+class APIResponse:
+    """A utility class that represents API responses"""
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ CLASS ATTRIBUTES
     # └─────────────────────────────────────────────────────────────────────────────────
 
     # Declare type of _object
     _object: requests.Response | aiohttp.ClientResponse
```

### Comparing `doji_core-0.1.2/doji/core/api/mixins/api_mixin.py` & `doji_core-0.1.3/doji/core/api/mixins/api_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/asset/classes/asset.py` & `doji_core-0.1.3/doji/core/asset/classes/asset.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/asset/classes/asset_instances.py` & `doji_core-0.1.3/doji/core/asset/classes/asset_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/asset/classes/asset_pair.py` & `doji_core-0.1.3/doji/core/asset/classes/asset_pair.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/asset/classes/asset_pair_instances.py` & `doji_core-0.1.3/doji/core/asset/classes/asset_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/asset/mixins/asset_pairs_mixin.py` & `doji_core-0.1.3/doji/core/asset/mixins/asset_pairs_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/asset/mixins/assets_mixin.py` & `doji_core-0.1.3/doji/core/asset/mixins/assets_mixin.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/currency/classes/currency.py` & `doji_core-0.1.3/doji/core/currency/classes/currency.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/currency/classes/currency_instances.py` & `doji_core-0.1.3/doji/core/currency/classes/currency_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/currency/classes/currency_pair.py` & `doji_core-0.1.3/doji/core/currency/classes/currency_pair.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/currency/classes/currency_pair_instances.py` & `doji_core-0.1.3/doji/core/currency/classes/currency_pair_instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/currency/mixins/currencies_mixin.py` & `doji_core-0.1.3/doji/core/currency/mixins/currencies_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,51 +140,53 @@
         return await self.assets_async
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ FETCH ASSETS
     # └─────────────────────────────────────────────────────────────────────────────────
 
     def fetch_assets(self) -> CurrencyInstances:
-        """Fetches a collection of Currency instances by API synchronously"""
+        """Fetches a collection of Currency instances from an API synchronously"""
 
         # Initialize assets
         assets = CurrencyInstances()
 
         # Iterate over currency pairs
         for currency_pair in self.fetch_currency_pairs():
             # Iterate over base and quote currencies
             for currency in (currency_pair.base, currency_pair.quote):
                 # Add currency to assets
                 assets.add(currency)
 
         # Iterate over currencies
-        for currency in self.fetch_currencies_by_api():
+        for currency in self.fetch_currencies_from_api():
             # Add currency to assets
             assets.update_or_add(currency)
 
         # Cache assets
         self._assets = assets
 
         # Return assets
         return assets
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ FETCH ASSETS ASYNC
     # └─────────────────────────────────────────────────────────────────────────────────
 
     async def fetch_assets_async(self) -> CurrencyInstances:
-        """Fetches a collection of Currency instances by API asynchronously"""
+        """Fetches a collection of Currency instances from an API asynchronously"""
 
         # Initialize assets
         assets = CurrencyInstances()
 
         # Define list currencies helper
         async def list_currencies() -> list[Currency]:
             # Return list of currencies
-            return [currency async for currency in self.fetch_currencies_by_api_async()]
+            return [
+                currency async for currency in self.fetch_currencies_from_api_async()
+            ]
 
         # Await currencies and currency pairs
         currencies, currency_pairs = await asyncio.gather(
             list_currencies(), self.fetch_currency_pairs_async()
         )
 
         # Iterate over currency pairs
@@ -222,41 +224,41 @@
     async def fetch_currencies_async(self) -> CurrencyInstances:
         """Fetches a collection of Currency instances asynchronously"""
 
         # Fetch and return assets
         return await self.fetch_assets_async()
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
-    # │ FETCH CURRENCIES BY API
+    # │ FETCH CURRENCIES FROM API
     # └─────────────────────────────────────────────────────────────────────────────────
 
-    def fetch_currencies_by_api(self) -> Generator[Currency, None, None]:
-        """Fetches a collection of Currency instances by API synchronously"""
+    def fetch_currencies_from_api(self) -> Generator[Currency, None, None]:
+        """Fetches a collection of Currency instances from an API synchronously"""
 
         # Initialize currencies
         currencies: list[Currency] = []
 
         # Iterate over currencies
         for currency in currencies:
             # Yield currency
             yield currency
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
-    # │ FETCH CURRENCIES BY API ASYNC
+    # │ FETCH CURRENCIES FROM API ASYNC
     # └─────────────────────────────────────────────────────────────────────────────────
 
-    async def fetch_currencies_by_api_async(self) -> AsyncGenerator[Currency, None]:
-        """Fetches a collection of Currency instances by API asynchronously"""
+    async def fetch_currencies_from_api_async(self) -> AsyncGenerator[Currency, None]:
+        """Fetches a collection of Currency instances from an API asynchronously"""
 
         # Get class name
         class_name = self.__class__.__name__
 
         # Log a warning
         logging.warning(
-            f"{class_name}.fetch_currencies_by_api_async not implemented; "
-            f"using {class_name}.fetch_currencies_by_api.\n"
+            f"{class_name}.fetch_currencies_from_api_async not implemented; "
+            f"using {class_name}.fetch_currencies_from_api.\n"
         )
 
         # Iterate over currencies
-        for currency in self.fetch_currencies_by_api():
+        for currency in self.fetch_currencies_from_api():
             # Yield currency
             yield currency
```

### Comparing `doji_core-0.1.2/doji/core/currency/mixins/currency_pairs_mixin.py` & `doji_core-0.1.3/doji/core/currency/mixins/currency_pairs_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,42 +56,42 @@
         return await self.asset_pairs_async
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ FETCH ASSET PAIRS
     # └─────────────────────────────────────────────────────────────────────────────────
 
     def fetch_asset_pairs(self) -> CurrencyPairInstances:
-        """Fetches a collection of CurrencyPair instances by API synchronously"""
+        """Fetches a collection of CurrencyPair instances from an API synchronously"""
 
         # Initialize asset pairs
         asset_pairs = CurrencyPairInstances()
 
         # Iterate over currency pairs
-        for currency_pair in self.fetch_currency_pairs_by_api():
+        for currency_pair in self.fetch_currency_pairs_from_api():
             # Add currency pairs to asset pairs
             asset_pairs.add(currency_pair)
 
         # Cache asset pairs
         self._asset_pairs = asset_pairs
 
         # Return asset pairs
         return asset_pairs
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
     # │ FETCH ASSET PAIRS ASYNC
     # └─────────────────────────────────────────────────────────────────────────────────
 
     async def fetch_asset_pairs_async(self) -> CurrencyPairInstances:
-        """Fetches a collection of CurrencyPair instances by API asynchronously"""
+        """Fetches a collection of CurrencyPair instances from an API asynchronously"""
 
         # Initialize asset pairs
         asset_pairs = CurrencyPairInstances()
 
         # Iterate over currency pairs
-        async for currency_pair in self.fetch_currency_pairs_by_api_async():
+        async for currency_pair in self.fetch_currency_pairs_from_api_async():
             # Add currency pairs to asset pairs
             asset_pairs.add(currency_pair)
 
         # Cache asset pairs
         self._asset_pairs = asset_pairs
 
         # Return asset pairs
@@ -114,43 +114,43 @@
     async def fetch_currency_pairs_async(self) -> CurrencyPairInstances:
         """Fetches a collection of CurrencyPair instances asynchronously"""
 
         # Fetch and return asset pairs
         return await self.fetch_asset_pairs_async()
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
-    # │ FETCH CURRENCY PAIRS BY API
+    # │ FETCH CURRENCY PAIRS FROM API
     # └─────────────────────────────────────────────────────────────────────────────────
 
-    def fetch_currency_pairs_by_api(self) -> Generator[CurrencyPair, None, None]:
-        """Fetches a collection of CurrencyPair instances by API synchronously"""
+    def fetch_currency_pairs_from_api(self) -> Generator[CurrencyPair, None, None]:
+        """Fetches a collection of CurrencyPair instances from an API synchronously"""
 
         # Initialize currency pairs
         currency_pairs: list[CurrencyPair] = []
 
         # Iterate over currency pairs
         for currency_pair in currency_pairs:
             # Yield currency pair
             yield currency_pair
 
     # ┌─────────────────────────────────────────────────────────────────────────────────
-    # │ FETCH CURRENCY PAIRS BY API ASYNC
+    # │ FETCH CURRENCY PAIRS FROM API ASYNC
     # └─────────────────────────────────────────────────────────────────────────────────
 
-    async def fetch_currency_pairs_by_api_async(
+    async def fetch_currency_pairs_from_api_async(
         self,
     ) -> AsyncGenerator[CurrencyPair, None]:
-        """Fetches a collection of CurrencyPair instances by API asynchronously"""
+        """Fetches a collection of CurrencyPair instances from an API asynchronously"""
 
         # Get class name
         class_name = self.__class__.__name__
 
         # Log a warning
         logging.warning(
-            f"{class_name}.fetch_currency_pairs_by_api_async not implemented; "
-            f"using {class_name}.fetch_currency_pairs_by_api.\n"
+            f"{class_name}.fetch_currency_pairs_from_api_async not implemented; "
+            f"using {class_name}.fetch_currency_pairs_from_api.\n"
         )
 
         # Iterate over currency pairs
-        for currency_pair in self.fetch_currency_pairs_by_api():
+        for currency_pair in self.fetch_currency_pairs_from_api():
             # Yield currency pair
             yield currency_pair
```

### Comparing `doji_core-0.1.2/doji/core/exchange/classes/currency_exchange.py` & `doji_core-0.1.3/doji/core/exchange/classes/currency_exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/exchange/classes/exchange.py` & `doji_core-0.1.3/doji/core/exchange/classes/exchange.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/types/__init__.py` & `doji_core-0.1.3/doji/core/types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ GENERAL IMPORTS
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 from typing import Any
 
+# ┌─────────────────────────────────────────────────────────────────────────────────────
+# │ PROJECT IMPORTS
+# └─────────────────────────────────────────────────────────────────────────────────────
+
+from doji.core.api.classes.api_response import APIResponse  # noqa: F401
+
 
 # ┌─────────────────────────────────────────────────────────────────────────────────────
 # │ ARGS AND KWARGS
 # └─────────────────────────────────────────────────────────────────────────────────────
 
 # Define a generic Args type
 Args = tuple[Any, ...]
```

### Comparing `doji_core-0.1.2/doji/core/utils/classes/instance.py` & `doji_core-0.1.3/doji/core/utils/classes/instance.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/doji/core/utils/classes/instances.py` & `doji_core-0.1.3/doji/core/utils/classes/instances.py`

 * *Files identical despite different names*

### Comparing `doji_core-0.1.2/pyproject.toml` & `doji_core-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "doji-core"
-version = "0.1.2"
+version = "0.1.3"
 description = "A repository for Doji, a trade analytics suite written in Python."
 authors = ["Sean O'Leary <seamicole@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "doji"}]
 
 [tool.poetry.dependencies]
```

### Comparing `doji_core-0.1.2/PKG-INFO` & `doji_core-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doji-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: A repository for Doji, a trade analytics suite written in Python.
 License: MIT
 Author: Sean O'Leary
 Author-email: seamicole@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

