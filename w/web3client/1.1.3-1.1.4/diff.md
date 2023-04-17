# Comparing `tmp/web3client-1.1.3.tar.gz` & `tmp/web3client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3client-1.1.3.tar", last modified: Mon Apr 10 16:34:41 2023, max compression
+gzip compressed data, was "web3client-1.1.4.tar", last modified: Mon Apr 17 14:57:00 2023, max compression
```

## Comparing `web3client-1.1.3.tar` & `web3client-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.3/LICENSE
--rw-r--r--   0        0        0     2647 2023-04-05 14:07:40.813589 web3client-1.1.3/README.md
--rw-r--r--   0        0        0     1983 2023-04-10 16:33:25.656644 web3client-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.3/src/.DS_Store
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.3/src/web3client/.DS_Store
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.3/src/web3client/__init__.py
--rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.3/src/web3client/abi/erc20.json
--rw-r--r--   0        0        0    24177 2023-04-10 16:32:21.324544 web3client-1.1.3/src/web3client/base_client.py
--rw-r--r--   0        0        0     3320 2023-04-05 16:33:33.363845 web3client-1.1.3/src/web3client/erc20_client.py
--rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.3/src/web3client/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.3/src/web3client/helpers/__init__.py
--rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.3/src/web3client/helpers/debug.py
--rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.3/src/web3client/helpers/general.py
--rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.3/src/web3client/helpers/websockets.py
--rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.3/src/web3factory/__init__.py
--rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.3/src/web3factory/erc20_tokens.py
--rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.3/src/web3factory/factory.py
--rw-r--r--   0        0        0     2605 2023-04-05 13:58:18.268462 web3client-1.1.3/src/web3factory/networks.py
--rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.3/src/web3factory/types.py
--rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.3/tests/.DS_Store
--rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.3/tests/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.3/tests/ape/.DS_Store
--rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.3/tests/ape/.build/SafeMath.json
--rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.3/tests/ape/.build/Token.json
--rw-r--r--   0        0        0    20923 2023-04-10 16:33:31.235366 web3client-1.1.3/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.3/tests/ape/contracts/token/SafeMath.sol
--rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.3/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.3/tests/ape/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.3/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.3/tests/web3client/__init__.py
--rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.3/tests/web3client/fixtures.py
--rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.3/tests/web3client/test_networks.py
--rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 web3client-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-13 15:30:24.076003 web3client-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2757 2023-04-17 14:56:39.469040 web3client-1.1.4/README.md
+-rw-r--r--   0        0        0     1983 2023-04-17 14:56:39.489153 web3client-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.879656 web3client-1.1.4/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:28.884980 web3client-1.1.4/src/web3client/.DS_Store
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.603558 web3client-1.1.4/src/web3client/__init__.py
+-rw-r--r--   0        0        0    11117 2022-10-18 14:47:37.604295 web3client-1.1.4/src/web3client/abi/erc20.json
+-rw-r--r--   0        0        0    24299 2023-04-17 14:56:39.481994 web3client-1.1.4/src/web3client/base_client.py
+-rw-r--r--   0        0        0     3320 2023-04-05 16:33:33.363845 web3client-1.1.4/src/web3client/erc20_client.py
+-rw-r--r--   0        0        0      342 2022-10-19 17:40:52.208885 web3client-1.1.4/src/web3client/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.604873 web3client-1.1.4/src/web3client/helpers/__init__.py
+-rw-r--r--   0        0        0     1732 2023-02-13 20:06:35.817499 web3client-1.1.4/src/web3client/helpers/debug.py
+-rw-r--r--   0        0        0     2438 2022-10-18 14:47:37.605628 web3client-1.1.4/src/web3client/helpers/general.py
+-rw-r--r--   0        0        0     1909 2023-04-10 15:26:30.878490 web3client-1.1.4/src/web3client/helpers/websockets.py
+-rw-r--r--   0        0        0        0 2022-10-18 14:47:37.601242 web3client-1.1.4/src/web3factory/__init__.py
+-rw-r--r--   0        0        0     2190 2023-04-05 13:58:18.268337 web3client-1.1.4/src/web3factory/erc20_tokens.py
+-rw-r--r--   0        0        0     1431 2023-02-13 20:30:39.832108 web3client-1.1.4/src/web3factory/factory.py
+-rw-r--r--   0        0        0     2770 2023-04-17 14:56:39.482576 web3client-1.1.4/src/web3factory/networks.py
+-rw-r--r--   0        0        0      621 2023-02-13 19:47:49.818983 web3client-1.1.4/src/web3factory/types.py
+-rw-r--r--   0        0        0     6148 2023-03-13 02:23:33.878800 web3client-1.1.4/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:23.399090 web3client-1.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     6148 2023-04-05 16:39:49.642961 web3client-1.1.4/tests/ape/.DS_Store
+-rw-r--r--   0        0        0      779 2023-04-06 10:47:11.288879 web3client-1.1.4/tests/ape/.build/SafeMath.json
+-rw-r--r--   0        0        0    14895 2023-04-06 10:47:11.290250 web3client-1.1.4/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0    20923 2023-04-16 07:19:49.635286 web3client-1.1.4/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0      600 2023-02-23 10:18:28.269673 web3client-1.1.4/tests/ape/contracts/token/SafeMath.sol
+-rw-r--r--   0        0        0     4082 2023-02-23 10:18:28.283242 web3client-1.1.4/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0     3529 2023-04-05 16:42:52.576613 web3client-1.1.4/tests/ape/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-05 15:27:07.832128 web3client-1.1.4/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-05 14:37:05.616337 web3client-1.1.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-02-23 10:04:38.139397 web3client-1.1.4/tests/web3client/__init__.py
+-rw-r--r--   0        0        0     1300 2023-04-06 11:08:05.647477 web3client-1.1.4/tests/web3client/fixtures.py
+-rw-r--r--   0        0        0     1417 2023-02-13 20:04:46.649348 web3client-1.1.4/tests/web3client/test_networks.py
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 web3client-1.1.4/PKG-INFO
```

### Comparing `web3client-1.1.3/LICENSE` & `web3client-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/README.md` & `web3client-1.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Batteries-included client to interact with blockchains and smart contracts; used by [`web3cli`](https://github.com/coccoinomane/web3cli) and [crabada.py](https://github.com/coccoinomane/crabada.py).
 
 # Features
 
 - Easily create a client to interact with EVM-compatible chains
-- Perform ERC20 operations, using the token name (e.g. USDC) instead of address.
 - Interact with the most popular chains: Ethereum, Binance, Avalanche, Arbitrum One, zkSync Era, and more to come!
+- Subscribe to pending transactions in the mempool and new blocks.
 - Save gas by setting an upper limit on the base fee.
 - Need more flexibility? Use directly the underlying web3.py client.
+- Perform ERC20 operations, using the token name (e.g. USDC) instead of address.
+
 
 # Install
 
 ```bash
 pip3 install -U web3client
 ```
 
 # Examples
 
-Get the latest block on both Ethereum, BNB Chain and Avalanche:
+Get the latest block on supported blockchains:
 
 ```python
 from web3factory.factory import make_client
 
-eth_block = make_client("eth").get_latest_block()
-bnb_block = make_client("bnb").get_latest_block()
-avax_block = make_client("avax").get_latest_block()
-arb_block = make_client("arb").get_latest_block()
-era_block = make_client("era").get_latest_block()
+eth_block = make_client("eth").get_latest_block() # Ethereum
+bnb_block = make_client("bnb").get_latest_block() # BNB chain
+avax_block = make_client("avax").get_latest_block() # Avalanche
+arb_block = make_client("arb").get_latest_block() # Arbitrum
+era_block = make_client("era").get_latest_block() # zkSync Era
 ```
 
 Get the ETH and USDC balances of the Ethereum foundation:
 
 ```python
 from web3factory.factory import make_client, make_erc20_client
```

### Comparing `web3client-1.1.3/pyproject.toml` & `web3client-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3client"
-version = "1.1.3"
+version = "1.1.4"
 description = "Batteries-included client to interact with blockchains and smart contracts"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3client-1.1.3/src/.DS_Store` & `web3client-1.1.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3client/.DS_Store` & `web3client-1.1.4/src/web3client/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3client/abi/erc20.json` & `web3client-1.1.4/src/web3client/abi/erc20.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3client/base_client.py` & `web3client-1.1.4/src/web3client/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,18 +432,19 @@
     async def async_subscribe(
         self,
         on_notification: Callable[[Any], Awaitable[None]],
         on_subscribe: Callable[[Any], None] = None,
         once: bool = False,
         subscription_type: str = "newPendingTransactions",
     ) -> None:
-        """Look for new pending transactions, blocks or events and, when one is found,
+        """Look for new pending transactions, blocks or events; when one is found,
         call the 'on_notification' callback concurrently.
 
-        For more details, see subscribe().
+        Call this function with asyncio.run(client.async_subscribe(callback)), where the
+        callback must be an async function.  For more details, see subscribe().
         """
         # Raise if not a websocket uri
         rpc_url = self.node_uri
         if not rpc_url.startswith("ws") and not rpc_url.endswith(".ipc"):
             raise ValueError("Websocket RPC needed to subscribe to node notifications")
 
         async def process_notification(
```

### Comparing `web3client-1.1.3/src/web3client/erc20_client.py` & `web3client-1.1.4/src/web3client/erc20_client.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3client/helpers/debug.py` & `web3client-1.1.4/src/web3client/helpers/debug.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3client/helpers/general.py` & `web3client-1.1.4/src/web3client/helpers/general.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3client/helpers/websockets.py` & `web3client-1.1.4/src/web3client/helpers/websockets.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3factory/erc20_tokens.py` & `web3client-1.1.4/src/web3factory/erc20_tokens.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3factory/factory.py` & `web3client-1.1.4/src/web3factory/factory.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/src/web3factory/networks.py` & `web3client-1.1.4/src/web3factory/networks.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,22 @@
     {
         "name": "era",
         "tx_type": 2,
         "chain_id": 324,
         "rpcs": ["https://mainnet.era.zksync.io"],
         "coin": "ETH",
     },
+    # Kava EVM
+    {
+        "name": "kava",
+        "tx_type": 1,
+        "chain_id": 2222,
+        "rpcs": ["https://evm.kava.io"],
+        "coin": "KAVA",
+    },
 ]
 
 
 def get_network_config(name: str) -> NetworkConfig:
     """
     Return the configuration for the network with the given
     name; raises an exception if not found
```

### Comparing `web3client-1.1.3/src/web3factory/types.py` & `web3client-1.1.4/src/web3factory/types.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/.DS_Store` & `web3client-1.1.4/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/ape/.DS_Store` & `web3client-1.1.4/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/ape/.build/SafeMath.json` & `web3client-1.1.4/tests/ape/.build/SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/ape/.build/Token.json` & `web3client-1.1.4/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/ape/.build/__local__.json` & `web3client-1.1.4/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/ape/contracts/token/SafeMath.sol` & `web3client-1.1.4/tests/ape/contracts/token/SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/ape/contracts/token/Token.sol` & `web3client-1.1.4/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/ape/fixtures.py` & `web3client-1.1.4/tests/ape/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/web3client/fixtures.py` & `web3client-1.1.4/tests/web3client/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/tests/web3client/test_networks.py` & `web3client-1.1.4/tests/web3client/test_networks.py`

 * *Files identical despite different names*

### Comparing `web3client-1.1.3/PKG-INFO` & `web3client-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 Metadata-Version: 2.1
 Name: web3client
-Version: 1.1.3
+Version: 1.1.4
 Summary: Batteries-included client to interact with blockchains and smart contracts
 License: MIT
 Keywords: web3,blockchain,ethereum,evm
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3client
 Project-URL: repository, https://github.com/coccoinomane/web3client
 Description-Content-Type: text/markdown
 
 Batteries-included client to interact with blockchains and smart contracts; used by [`web3cli`](https://github.com/coccoinomane/web3cli) and [crabada.py](https://github.com/coccoinomane/crabada.py).
 
 # Features
 
 - Easily create a client to interact with EVM-compatible chains
-- Perform ERC20 operations, using the token name (e.g. USDC) instead of address.
 - Interact with the most popular chains: Ethereum, Binance, Avalanche, Arbitrum One, zkSync Era, and more to come!
+- Subscribe to pending transactions in the mempool and new blocks.
 - Save gas by setting an upper limit on the base fee.
 - Need more flexibility? Use directly the underlying web3.py client.
+- Perform ERC20 operations, using the token name (e.g. USDC) instead of address.
+
 
 # Install
 
 ```bash
 pip3 install -U web3client
 ```
 
 # Examples
 
-Get the latest block on both Ethereum, BNB Chain and Avalanche:
+Get the latest block on supported blockchains:
 
 ```python
 from web3factory.factory import make_client
 
-eth_block = make_client("eth").get_latest_block()
-bnb_block = make_client("bnb").get_latest_block()
-avax_block = make_client("avax").get_latest_block()
-arb_block = make_client("arb").get_latest_block()
-era_block = make_client("era").get_latest_block()
+eth_block = make_client("eth").get_latest_block() # Ethereum
+bnb_block = make_client("bnb").get_latest_block() # BNB chain
+avax_block = make_client("avax").get_latest_block() # Avalanche
+arb_block = make_client("arb").get_latest_block() # Arbitrum
+era_block = make_client("era").get_latest_block() # zkSync Era
 ```
 
 Get the ETH and USDC balances of the Ethereum foundation:
 
 ```python
 from web3factory.factory import make_client, make_erc20_client
```

