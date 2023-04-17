# Comparing `tmp/dxsp-1.2.3.tar.gz` & `tmp/dxsp-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.2.3.tar", max compression
+gzip compressed data, was "dxsp-1.2.4.tar", max compression
```

## Comparing `dxsp-1.2.3.tar` & `dxsp-1.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-17 08:33:25.022310 dxsp-1.2.3/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-17 08:33:25.022310 dxsp-1.2.3/README.md
--rw-r--r--   0        0        0      136 2023-04-17 08:33:25.682304 dxsp-1.2.3/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-17 08:33:25.022310 dxsp-1.2.3/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-17 08:33:25.022310 dxsp-1.2.3/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    27341 2023-04-17 08:33:25.022310 dxsp-1.2.3/dxsp/main.py
--rw-r--r--   0        0        0      944 2023-04-17 08:33:25.682304 dxsp-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     4054 1970-01-01 00:00:00.000000 dxsp-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 10:20:19.490166 dxsp-1.2.4/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-17 10:20:19.490166 dxsp-1.2.4/README.md
+-rw-r--r--   0        0        0      136 2023-04-17 10:20:20.110157 dxsp-1.2.4/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-17 10:20:19.490166 dxsp-1.2.4/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-17 10:20:19.490166 dxsp-1.2.4/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    27961 2023-04-17 10:20:19.490166 dxsp-1.2.4/dxsp/main.py
+-rw-r--r--   0        0        0      960 2023-04-17 10:20:20.110157 dxsp-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 dxsp-1.2.4/PKG-INFO
```

### Comparing `dxsp-1.2.3/LICENSE` & `dxsp-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.3/README.md` & `dxsp-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.3/dxsp/assets/blockchains.py` & `dxsp-1.2.4/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.3/dxsp/main.py` & `dxsp-1.2.4/dxsp/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os, json, requests, asyncio, logging
 
 from dotenv import load_dotenv
 
 from web3 import Web3
 from pycoingecko import CoinGeckoAPI
 
+#import many_abis as ma
+
 from ping3 import ping
 
 class DexSwap:
 
 
     def __init__(self,
                  chain_id: int = 1, 
@@ -39,23 +41,24 @@
             return
         blockchain = blockchains[self.chain_id ]
         self.logger.debug(f"blockchain {blockchain}")
 
         self.wallet_address = wallet_address
         self.logger.debug(f"self.wallet_address {self.wallet_address}")
         self.private_key = private_key
-        self.block_explorer_api = block_explorer_api
 
+        self.block_explorer_api = block_explorer_api
+        if self.block_explorer_api is None:
+            self.logger.warning("self.block_explorer_api not setup")
         self.block_explorer_url = block_explorer_url
         self.logger.debug(f"self.block_explorer_url {self.block_explorer_url}")
         if self.block_explorer_url is None:
             self.block_explorer_url = blockchain["block_explorer_url"]
         if self.block_explorer_url is None:
             self.logger.warning("self.block_explorer_url not setup")
-            return
         self.logger.debug(f"self.block_explorer_url {self.block_explorer_url}")
 
         self.rpc = rpc
         if self.rpc is None:
             self.rpc = blockchain["rpc"]
         self.logger.debug(f"self.rpc {self.rpc}")
 
@@ -63,15 +66,15 @@
         self.logger.debug(f"self.latency {self.latency}")    
 
         self.w3 = w3
         if self.w3 is None:
             self.w3 = Web3(Web3.HTTPProvider(self.rpc))
             try:
                 self.w3.net.listening
-                logger.info(msg=f"connected to {w3}")
+                logger.info(msg=f"connected to {rpc} with w3 {w3}")
             except Exception as e:
                 logger.error(msg=f"connectivity failed using {rpc}")
                 return
         self.logger.debug(f"self.w3 {self.w3}")
         self.logger.info(msg=f"connected")
 
         self.protocol_type = protocol_type
@@ -262,39 +265,40 @@
 
             #UNISWAP V3
             if self.protocol_type ['uniswap_v3']:
                 return
             if swap_TX:
                 self.logger.debug(f"swap_TX {swap_TX}")
                 signed_TX = await self.get_sign(swap_TX)
-                txHash = str(self.w3.to_hex(signed_TX))
-                txResult = await self.get_block_explorer_status(txHash)
-                txHashDetail= self.w3.wait_for_transaction_receipt(txHash, timeout=120, poll_latency=0.1)
-                if(txResult == "1"):
-                    blockNumber = txHashDetail['blockNumber']
+                transaction_hash = str(self.w3.to_hex(signed_TX))
+                #transaction_results = await self.get_block_explorer_status(transaction_hash)
+                transaction_hash_details = self.w3.wait_for_transaction_receipt(transaction_hash, timeout=120, poll_latency=0.1)
+                if(transaction_hash_details['status'] == "1"):
+                    transaction_blockNumber = transaction_hash_details['blockNumber']
+                    transaction_receipt = self.w3.eth.get_transaction_receipt(transaction_hash)
                     transaction_block = self.w3.eth.get_block(blockNumber)
                     order={}
-                    d['id'] = '15222'
-                    d['timestamp'] = transaction_block['timestamp']
-                    d['gasUsed'] = txHashDetail['gasUsed']
-                    d['id'] = '15222'
-                    d['amount'] = 'host name'
-                    d['price'] = '15222'
-                    return txHash
+                    order['id'] = transaction_receipt['transactionHash']
+                    order['timestamp'] = transaction_block['timestamp']
+                    order['symbol'] = asset_out_symbol
+                    order['contract'] = asset_out_address
+                    order['amount'] = transaction_amount
+                    order['fee'] = transaction_receipt['gasUsed']
+                    order['price'] = 'na'
+                    return order
         except Exception as e:
             self.logger.debug(f"error get_swap {e}")
             return
 
     async def get_block_explorer_status(self,txHash):
         self.logger.debug(f"get_block_explorer_status {txHash}")
         checkTransactionSuccessURL = f"{self.block_explorer_url}?module=transaction&action=gettxreceiptstatus&txhash={txHash}&apikey={self.block_explorer_api}"
         checkTransactionRequest =  self.get(checkTransactionSuccessURL)
         return checkTransactionRequest['status']
 
-
 ####CONTRACT SEARCH
 
     # async def search_gecko_platform(self):
     #     self.logger.debug("search_gecko_platform")
     #     try:
     #         assetplatform = self.gecko_api.get_asset_platforms()
     #         output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
@@ -441,27 +445,28 @@
             signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
             raw_tx = signed.rawTransaction
             return self.w3.eth.send_raw_transaction(raw_tx)
         except Exception as e:
             self.logger.debug(f"error get_sign {e}")
             return
 
-
     async def get_gas(self, tx):
         self.logger.debug(f"get_gas {tx}")
         gasestimate= self.web3.eth.estimate_gas(tx) * 1.25
         return int(self.w3.to_wei(gasestimate,'wei'))
 
     async def get_gasPrice(self, tx):
         self.logger.debug(f"get_gasPrice {tx}")
         gasprice= self.w3.eth.generate_gas_price()
         return self.w3.to_wei(gasPrice,'gwei')
 
     async def get_abi(self,addr):
         self.logger.debug(f"get_abi {addr}")
+        if self.block_explorer_api is None:
+            self.logger.debug("No block_explorer_api")
         try:
             params = {
                 "module": "contract",
                 "action": "getabi",
                 "address": addr,
                 "apikey": self.block_explorer_api }
             headers = { "User-Agent": "Mozilla/5.0" }
@@ -469,18 +474,22 @@
             #self.logger.debug(f"resp {resp} status {resp['status']}")
             if resp['status']=="1":
                 self.logger.debug(f"ABI found {resp}")
                 abi = resp["result"]
                 return abi
             else:
                 self.logger.debug(f"No ABI identified Option B needed for contract {addr} on chain {self.chain_id}")
+                #manyABI options UNISWAP_V2_ROUTER  ?
+
         except Exception as e:
             self.logger.debug(f"error get_abi {e}")
             return
 
+
+
 #####USERS
 
     async def get_wallet_auth():
         try:
             return
         except Exception as e:
             self.logger.error(msg=f"get_wallet_auth error: {e}")
```

### Comparing `dxsp-1.2.3/pyproject.toml` & `dxsp-1.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.2.3"
+version = "1.2.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -16,14 +16,15 @@
 python = "^3.10"
 asyncio = "*"
 python-dotenv = "*"
 web3 = ">=6.*"
 pycoingecko = "*"
 ping3 = "*"
 dynaconf = "*"
+many-abis = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dxsp-1.2.3/PKG-INFO` & `dxsp-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.2.3
+Version: 1.2.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio
 Requires-Dist: dynaconf
+Requires-Dist: many-abis
 Requires-Dist: ping3
 Requires-Dist: pycoingecko
 Requires-Dist: python-dotenv
 Requires-Dist: web3 (>=6)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
```

