# Comparing `tmp/web3client-1.1.4.tar.gz` & `tmp/web3client-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3client-1.1.4.tar", last modified: Mon Apr 17 14:57:00 2023, max compression
+gzip compressed data, was "web3client-1.1.5.tar", last modified: Mon Apr 17 16:01:33 2023, max compression
```

## Comparing `web3client-1.1.4.tar` & `web3client-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.4/LICENSE
--rw-r--r--   0        0        0     2757 2023-04-17 14:56:39.469040 web3client-1.1.4/README.md
--rw-r--r--   0        0        0     1983 2023-04-17 14:56:39.489153 web3client-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.4/src/.DS_Store
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.4/src/web3client/.DS_Store
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.4/src/web3client/__init__.py
--rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.4/src/web3client/abi/erc20.json
--rw-r--r--   0        0        0    24299 2023-04-17 14:56:39.481994 web3client-1.1.4/src/web3client/base_client.py
--rw-r--r--   0        0        0     3320 2023-04-05 16:33:33.363845 web3client-1.1.4/src/web3client/erc20_client.py
--rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.4/src/web3client/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.4/src/web3client/helpers/__init__.py
--rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.4/src/web3client/helpers/debug.py
--rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.4/src/web3client/helpers/general.py
--rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.4/src/web3client/helpers/websockets.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.4/src/web3factory/__init__.py
--rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.4/src/web3factory/erc20_tokens.py
--rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.4/src/web3factory/factory.py
--rw-r--r--   0        0        0     2770 2023-04-17 14:56:39.482576 web3client-1.1.4/src/web3factory/networks.py
--rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.4/src/web3factory/types.py
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.4/tests/.DS_Store
--rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.4/tests/ape/.DS_Store
--rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.4/tests/ape/.build/SafeMath.json
--rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.4/tests/ape/.build/Token.json
--rw-r--r--   0        0        0    20923 2023-04-16 07:19:49.635286 web3client-1.1.4/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.4/tests/ape/contracts/token/SafeMath.sol
--rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.4/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.4/tests/ape/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.4/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.4/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.4/tests/web3client/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.4/tests/web3client/fixtures.py
--rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.4/tests/web3client/test_networks.py
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 web3client-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2757 2023-04-17 14:56:39.469040 web3client-1.1.5/README.md
+-rw-r--r--   0        0        0     1983 2023-04-17 16:01:24.258722 web3client-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.5/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.5/src/web3client/.DS_Store
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.5/src/web3client/__init__.py
+-rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.5/src/web3client/abi/erc20.json
+-rw-r--r--   0        0        0    24453 2023-04-17 15:41:44.355806 web3client-1.1.5/src/web3client/base_client.py
+-rw-r--r--   0        0        0     3320 2023-04-05 16:33:33.363845 web3client-1.1.5/src/web3client/erc20_client.py
+-rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.5/src/web3client/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.5/src/web3client/helpers/__init__.py
+-rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.5/src/web3client/helpers/debug.py
+-rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.5/src/web3client/helpers/general.py
+-rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.5/src/web3client/helpers/websockets.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.5/src/web3factory/__init__.py
+-rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.5/src/web3factory/erc20_tokens.py
+-rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.5/src/web3factory/factory.py
+-rw-r--r--   0        0        0     2770 2023-04-17 14:56:39.482576 web3client-1.1.5/src/web3factory/networks.py
+-rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.5/src/web3factory/types.py
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.5/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.5/tests/ape/.DS_Store
+-rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.5/tests/ape/.build/SafeMath.json
+-rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.5/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0    20923 2023-04-17 16:01:26.777617 web3client-1.1.5/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.5/tests/ape/contracts/token/SafeMath.sol
+-rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.5/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.5/tests/ape/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.5/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.5/tests/web3client/__init__.py
+-rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.5/tests/web3client/fixtures.py
+-rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.5/tests/web3client/test_networks.py
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 web3client-1.1.5/PKG-INFO
```

### Comparing `web3client-1.1.4/LICENSE` & `web3client-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/README.md` & `web3client-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/pyproject.toml` & `web3client-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3client"
-version = "1.1.4"
+version = "1.1.5"
 description = "Batteries-included client to interact with blockchains and smart contracts"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3client-1.1.4/src/.DS_Store` & `web3client-1.1.5/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3client/.DS_Store` & `web3client-1.1.5/src/web3client/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3client/abi/erc20.json` & `web3client-1.1.5/src/web3client/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3client/base_client.py` & `web3client-1.1.5/src/web3client/base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import json
 from typing import Any, Awaitable, Callable, List, Tuple, Union, cast
 
 from eth_account import Account
 from eth_account.datastructures import SignedMessage, SignedTransaction
 from eth_account.messages import encode_defunct
@@ -101,35 +103,41 @@
         if middlewares:
             self.set_middlewares(middlewares)
 
     ####################
     # Setters
     ####################
 
-    def set_provider(self, node_uri: str) -> None:
+    def set_provider(self, node_uri: str) -> BaseClient:
         self.node_uri: str = node_uri
         self.w3 = self.get_provider(node_uri)
+        return self
 
-    def set_account(self, private_key: str) -> None:
+    def set_account(self, private_key: str) -> BaseClient:
         self.private_key: str = private_key
         self.account: LocalAccount = Account.from_key(private_key)
         self.user_address: Address = self.account.address
+        return self
 
-    def set_contract(self, contract_address: Address, abi: dict[str, Any]) -> None:
+    def set_contract(
+        self, contract_address: Address, abi: dict[str, Any]
+    ) -> BaseClient:
         self.contract_address: Address = cast(
             Address, Web3.to_checksum_address(contract_address)
         )
         self.abi: dict[str, Any] = abi
         self.contract = self.getContract(contract_address, self.w3, abi=abi)
         self.functions = self.contract.functions
+        return self
 
-    def set_middlewares(self, middlewares: List[Middleware]) -> None:
+    def set_middlewares(self, middlewares: List[Middleware]) -> BaseClient:
         self.middlewares: List[Middleware] = middlewares
         for i, m in enumerate(middlewares):
             self.w3.middleware_onion.inject(m, layer=i)
+        return self
 
     ####################
     # Build Tx
     ####################
 
     def build_base_tx(
         self,
```

### Comparing `web3client-1.1.4/src/web3client/erc20_client.py` & `web3client-1.1.5/src/web3client/erc20_client.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3client/helpers/debug.py` & `web3client-1.1.5/src/web3client/helpers/debug.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3client/helpers/general.py` & `web3client-1.1.5/src/web3client/helpers/general.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3client/helpers/websockets.py` & `web3client-1.1.5/src/web3client/helpers/websockets.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3factory/erc20_tokens.py` & `web3client-1.1.5/src/web3factory/erc20_tokens.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3factory/factory.py` & `web3client-1.1.5/src/web3factory/factory.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3factory/networks.py` & `web3client-1.1.5/src/web3factory/networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/src/web3factory/types.py` & `web3client-1.1.5/src/web3factory/types.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/.DS_Store` & `web3client-1.1.5/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/ape/.DS_Store` & `web3client-1.1.5/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/ape/.build/SafeMath.json` & `web3client-1.1.5/tests/ape/.build/SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/ape/.build/Token.json` & `web3client-1.1.5/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/ape/.build/__local__.json` & `web3client-1.1.5/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/ape/contracts/token/SafeMath.sol` & `web3client-1.1.5/tests/ape/contracts/token/SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/ape/contracts/token/Token.sol` & `web3client-1.1.5/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/ape/fixtures.py` & `web3client-1.1.5/tests/ape/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/web3client/fixtures.py` & `web3client-1.1.5/tests/web3client/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/tests/web3client/test_networks.py` & `web3client-1.1.5/tests/web3client/test_networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.4/PKG-INFO` & `web3client-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3client
-Version: 1.1.4
+Version: 1.1.5
 Summary: Batteries-included client to interact with blockchains and smart contracts
 License: MIT
 Keywords: web3,blockchain,ethereum,evm
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3client
 Project-URL: repository, https://github.com/coccoinomane/web3client
```

