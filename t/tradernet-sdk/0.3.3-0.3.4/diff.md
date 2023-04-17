# Comparing `tmp/tradernet_sdk-0.3.3.tar.gz` & `tmp/tradernet_sdk-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradernet_sdk-0.3.3.tar", max compression
+gzip compressed data, was "tradernet_sdk-0.3.4.tar", max compression
```

## Comparing `tradernet_sdk-0.3.3.tar` & `tradernet_sdk-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1131 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/LICENSE
--rw-r--r--   0        0        0     4024 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/README.md
--rw-r--r--   0        0        0      978 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/PublicApiClient.py
--rw-r--r--   0        0        0      583 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/__init__.py
--rw-r--r--   0        0        0    32929 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/client.py
--rw-r--r--   0        0        0    11656 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/core.py
--rw-r--r--   0        0        0     2231 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/netutils.py
--rw-r--r--   0        0        0     7877 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/string_utils.py
--rw-r--r--   0        0        0        0 2023-04-12 19:01:58.087196 tradernet_sdk-0.3.3/tradernet/symbols/__init__.py
--rw-r--r--   0        0        0     6329 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/base_market_symbol.py
--rw-r--r--   0        0        0     4151 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/base_option_symbol.py
--rw-r--r--   0        0        0     2836 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/das_option.py
--rw-r--r--   0        0        0      290 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/option_properties.py
--rw-r--r--   0        0        0     2132 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/tradernet_option.py
--rw-r--r--   0        0        0     2336 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/symbols/tradernet_symbol.py
--rw-r--r--   0        0        0     3052 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.3/tradernet/tradernet_wsapi.py
--rw-r--r--   0        0        0     6414 2023-04-12 18:30:40.754961 tradernet_sdk-0.3.3/tradernet/trading.py
--rw-r--r--   0        0        0     2858 2023-04-12 18:30:40.754961 tradernet_sdk-0.3.3/tradernet/ws_utils.py
--rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4024 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/README.md
+-rw-r--r--   0        0        0      978 2023-04-17 12:07:06.989999 tradernet_sdk-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1305 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/PublicApiClient.py
+-rw-r--r--   0        0        0      583 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/__init__.py
+-rw-r--r--   0        0        0    32929 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/client.py
+-rw-r--r--   0        0        0    11656 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/core.py
+-rw-r--r--   0        0        0     2231 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/netutils.py
+-rw-r--r--   0        0        0     7877 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/string_utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 12:12:02.327268 tradernet_sdk-0.3.4/tradernet/symbols/__init__.py
+-rw-r--r--   0        0        0     6329 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/base_market_symbol.py
+-rw-r--r--   0        0        0     4151 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/base_option_symbol.py
+-rw-r--r--   0        0        0     2836 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/das_option.py
+-rw-r--r--   0        0        0      290 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/option_properties.py
+-rw-r--r--   0        0        0     2132 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/tradernet_option.py
+-rw-r--r--   0        0        0     2336 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/symbols/tradernet_symbol.py
+-rw-r--r--   0        0        0     3052 2023-04-12 18:30:40.750961 tradernet_sdk-0.3.4/tradernet/tradernet_wsapi.py
+-rw-r--r--   0        0        0     6996 2023-04-14 16:56:52.678694 tradernet_sdk-0.3.4/tradernet/trading.py
+-rw-r--r--   0        0        0     2858 2023-04-12 18:30:40.754961 tradernet_sdk-0.3.4/tradernet/ws_utils.py
+-rw-r--r--   0        0        0     4906 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.4/PKG-INFO
```

### Comparing `tradernet_sdk-0.3.3/LICENSE` & `tradernet_sdk-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/README.md` & `tradernet_sdk-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/pyproject.toml` & `tradernet_sdk-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tradernet-sdk"
-version = "0.3.3"
+version = "0.3.4"
 description = "Public API for TraderNet"
 authors = ["Anton Kudelin <a.kudelin@freedomfinance.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://tradernet.com/tradernet-api/"
 packages = [
     {include = "tradernet"}
```

### Comparing `tradernet_sdk-0.3.3/tradernet/PublicApiClient.py` & `tradernet_sdk-0.3.4/tradernet/PublicApiClient.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/__init__.py` & `tradernet_sdk-0.3.4/tradernet/__init__.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/client.py` & `tradernet_sdk-0.3.4/tradernet/client.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/core.py` & `tradernet_sdk-0.3.4/tradernet/core.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/netutils.py` & `tradernet_sdk-0.3.4/tradernet/netutils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/string_utils.py` & `tradernet_sdk-0.3.4/tradernet/string_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/symbols/base_market_symbol.py` & `tradernet_sdk-0.3.4/tradernet/symbols/base_market_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/symbols/base_option_symbol.py` & `tradernet_sdk-0.3.4/tradernet/symbols/base_option_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/symbols/das_option.py` & `tradernet_sdk-0.3.4/tradernet/symbols/das_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/symbols/tradernet_option.py` & `tradernet_sdk-0.3.4/tradernet/symbols/tradernet_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/symbols/tradernet_symbol.py` & `tradernet_sdk-0.3.4/tradernet/symbols/tradernet_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/tradernet_wsapi.py` & `tradernet_sdk-0.3.4/tradernet/tradernet_wsapi.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/tradernet/trading.py` & `tradernet_sdk-0.3.4/tradernet/trading.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,37 @@
         params = {
             'instr_name': symbol,
             'stop_loss_percent': percent,
             'stoploss_trailing_percent': percent
         }
         return self.authorized_request(cmd, params, version=2)
 
+    def take_profit(self, symbol: str, price: float) -> dict[str, Any]:
+        """
+        Placing a new take profit order on a certain open position.
+
+        Parameters
+        ----------
+        symbol : str
+            TraderNet symbol.
+        price : float
+            Take profit price.
+
+        Returns
+        -------
+        dict[str, Any]
+            Order information.
+        """
+        cmd = 'putStopLoss'
+        params = {
+            'instr_name': symbol,
+            'take_profit': price
+        }
+        return self.authorized_request(cmd, params, version=2)
+
     def cancel(self, order_id: int) -> dict[str, Any]:
         """
         Cancelling an order.
 
         Parameters
         ----------
         order_id : int
@@ -213,15 +236,15 @@
         Returns
         -------
         result : dict
             A dictionary of orders.
 
         Notes
         -----
-        https://tradernet.ru/tradernet-api/orders-get-history
+        https://tradernet.ru/tradernet-api/get-orders-history
         """
         cmd = 'getOrdersHistory'
         params = {
             'from': start.strftime('%Y-%m-%dT%H:%M:%S'),
             'till': end.strftime('%Y-%m-%dT%H:%M:%S')
         }
         if not self._session_id:
```

### Comparing `tradernet_sdk-0.3.3/tradernet/ws_utils.py` & `tradernet_sdk-0.3.4/tradernet/ws_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.3/PKG-INFO` & `tradernet_sdk-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradernet-sdk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Public API for TraderNet
 Home-page: https://tradernet.com/tradernet-api/
 License: MIT
 Author: Anton Kudelin
 Author-email: a.kudelin@freedomfinance.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

