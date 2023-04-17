# Comparing `tmp/dxsp-1.2.1.tar.gz` & `tmp/dxsp-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.2.1.tar", max compression
+gzip compressed data, was "dxsp-1.2.2.tar", max compression
```

## Comparing `dxsp-1.2.1.tar` & `dxsp-1.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-16 15:29:03.606209 dxsp-1.2.1/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-16 15:29:03.606209 dxsp-1.2.1/README.md
--rw-r--r--   0        0        0      136 2023-04-16 15:29:04.250208 dxsp-1.2.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-16 15:29:03.606209 dxsp-1.2.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-16 15:29:03.606209 dxsp-1.2.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    26947 2023-04-16 15:29:03.606209 dxsp-1.2.1/dxsp/main.py
--rw-r--r--   0        0        0      929 2023-04-16 15:29:04.250208 dxsp-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 dxsp-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 08:17:22.790547 dxsp-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-17 08:17:22.790547 dxsp-1.2.2/README.md
+-rw-r--r--   0        0        0      136 2023-04-17 08:17:23.486556 dxsp-1.2.2/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-17 08:17:22.790547 dxsp-1.2.2/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-17 08:17:22.790547 dxsp-1.2.2/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    27036 2023-04-17 08:17:22.790547 dxsp-1.2.2/dxsp/main.py
+-rw-r--r--   0        0        0      929 2023-04-17 08:17:23.482556 dxsp-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 dxsp-1.2.2/PKG-INFO
```

### Comparing `dxsp-1.2.1/LICENSE` & `dxsp-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.1/README.md` & `dxsp-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.1/dxsp/assets/blockchains.py` & `dxsp-1.2.2/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.1/dxsp/main.py` & `dxsp-1.2.2/dxsp/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-import os
-import json
-import requests
-import asyncio
+from dxsp import __version__
+from dxsp.assets.blockchains import blockchains
 
-import logging
+import os, json, requests, asyncio, logging
 
 from dotenv import load_dotenv
 
 from web3 import Web3
 from datetime import datetime
 from pycoingecko import CoinGeckoAPI
 
-from dxsp.assets.blockchains import blockchains
-
 from ping3 import ping
 
 class DexSwap:
 
 
     def __init__(self,
                  chain_id: int = 1, 
@@ -30,15 +26,15 @@
                  dex_exchange: str = None,
                  dex_router: str = None,
                  base_trading_symbol: str = None,
                  amount_trading_option: int = 1,
                  ):
 
         self.logger =  logging.getLogger(__name__)
-        self.logger.debug(f"DXSP Logger:  {self.logger} on {__name__}")
+        self.logger.debug(f"DXSP Logger:  {self.logger} on {__name__} version: {__version__}")
         self.logger.info(f"Initializing DexSwap object for {wallet_address} on {chain_id}")
 
         self.chain_id = int(chain_id)
         self.logger.debug(f"self.chain_id {self.chain_id}")
         if self.chain_id  is None:
             self.logger.warning("self.chain_id not setup")
             return
@@ -119,25 +115,24 @@
 
         self.gecko_api = CoinGeckoAPI() # llama_api = f"https://api.llama.fi/" maybe as backup to be reviewed
         assetplatform = self.gecko_api.get_asset_platforms()
         output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
         self.gecko_platform = output_dict[0]['id']
         self.logger.debug(f"self.gecko_platform {self.gecko_platform}")
 
-        # global gasPrice
-        # global gasLimit
+        # self.gasPrice = gasPrice
+        # self.gasLimit = gasLimit
 
     async def _get(self, url, params=None, headers=None):
         headers = { "User-Agent": "Mozilla/5.0" }
-        #self.logger.debug(f"_get url {url}")
+        self.logger.debug(f"_get url {url}")
         response = requests.get(url,params =params,headers=headers)
         #self.logger.debug(f"response _get {response}")
         return response.json()
 
-
     async def get_quote(self, symbol):
         self.logger.debug(f"get_quote {symbol}")
         asset_in_address = await self.search_contract(symbol)
         self.logger.debug(f"asset_in_address {asset_in_address}")
         asset_out_symbol = self.base_trading_symbol
         asset_out_address = await self.search_contract(asset_out_symbol)
         self.logger.debug(f"asset_out_address {asset_out_address}")
@@ -163,101 +158,17 @@
                 return round(quote_readable,2)
             if self.protocol_type in ["uniswap_v2","uniswap_v3"]:
                 return
         except Exception as e:
             self.logger.debug(f"error get_quote {e}")
             return
 
-    async def get_abi(self,addr):
-        self.logger.debug(f"get_abi {addr}")
-        try:
-            params = {
-                "module": "contract",
-                "action": "getabi",
-                "address": addr,
-                "apikey": self.block_explorer_api }
-            headers = { "User-Agent": "Mozilla/5.0" }
-            resp = await self._get(url=self.block_explorer_url,params=params,headers=headers)
-            #self.logger.debug(f"resp {resp} status {resp['status']}")
-            if resp['status']=="1":
-                self.logger.debug(f"ABI found {resp}")
-                abi = resp["result"]
-                return abi
-            else:
-                self.logger.debug(f"No ABI identified Option B needed for contract {addr} on chain {self.chain_id}")
-        except Exception as e:
-            self.logger.debug(f"error get_abi {e}")
-            return
-
-    async def get_approve(self, asset_out_address: str, amount=None):
-        self.logger.debug(f"get_approve {asset_out_address}")
-        if self.protocol_type in ["1inch","1inch_limit"]:
-            approval_check_URL = f"{self.dex_url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
-            approval_response = await self._get(approval_check_URL)
-            approval_check = approval_response['allowance']
-            if (approval_check==0):
-                approval_URL = f"{self.dex_url}/approve/transaction?tokenAddress={asset_out_address}"
-                approval_response = await self._get(approval_URL)
-        elif self.protocol_type in ["uniswap_v2","uniswap_v3"]:
-            asset_out_abi= await self.get_abi(asset_out_address)
-            asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)           
-            approval_check = asset_out_contract.functions.allowance(self.w3.to_checksum_address(self.wallet_address), self.w3.to_checksum_address(self.router)).call()
-            if (approval_check==0):
-                approved_amount = (self.w3.to_wei(2**64-1,'ether'))
-                asset_out_abi = await fetch_abi_dex(asset_out_address)
-                asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
-                approval_TX = asset_out_contract.functions.approve(self.w3.to_checksum_address(self.router), approved_amount)
-                approval_txHash = await sign_transaction_dex(approval_TX)
-                approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
-
-    async def get_sign(self, tx):
-        self.logger.debug(f"get_sign {tx}")
-        try:
-            if self.protocol_type in ['uniswap_v2']:
-                tx_params = {
-                'from': self.wallet_address,
-                'gas': await self.get_gas(tx),
-                'gasPrice': await self.get_gasPrice(tx),
-                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
-                }
-                tx = tx.build_transaction(tx_params)
-            elif self.protocol_type in ['uniswap_v3']:
-                tx_params = {
-                'from': self.wallet_address,
-                'gas': await estimate_gas(tx),
-                'gasPrice': await self.get_gasPrice(tx),
-                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
-                }
-                tx = tx.build_transaction(tx_params)
-            elif self.protocol_type in ["1inch","1inch_limit"]:
-                tx = tx['tx']
-                tx['gas'] = await estimate_gas(tx)
-                tx['nonce'] = self.w3.eth.get_transaction_count(self.wallet_address)
-                tx['value'] = int(tx['value'])
-                tx['gasPrice'] = await self.get_gasPrice(tx)
-            signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
-            raw_tx = signed.rawTransaction
-            return self.w3.eth.send_raw_transaction(raw_tx)
-        except Exception as e:
-            self.logger.debug(f"error get_sign {e}")
-            return
-
-    async def get_gas(self, tx):
-        self.logger.debug(f"get_gas {tx}")
-        gasestimate= self.web3.eth.estimate_gas(tx) * 1.25
-        return int(self.w3.to_wei(gasestimate,'wei'))
-
-    async def get_gasPrice(self, tx):
-        self.logger.debug(f"get_gasPrice {tx}")
-        gasprice= self.w3.eth.generate_gas_price()
-        return self.w3.to_wei(gasPrice,'gwei')
-
     async def execute_order(self,direction,symbol,stoploss=10000,takeprofit=10000,quantity=1,amount_trading_option=1,order_type='swap'):
         self.logger.debug(f"execute_order {direction} {symbol} {order_type}")
-        if order_type == 'swap'
+        if order_type == 'swap':
             self.logger.debug(f"execute_order {order_type}")
             try:
                 asset_out_symbol = self.base_trading_symbol if direction=="BUY" else symbol
                 asset_in_symbol = symbol if direction=="BUY" else self.base_trading_symbol
                 asset_out_contract = await self.get_token_contract(asset_out_symbol)
                 asset_out_decimals = asset_out_contract.functions.decimals().call()
                 asset_out_balance = await self.get_token_balance(asset_out_symbol)
@@ -268,18 +179,18 @@
           
                 swap = self.get_swap(asset_out_symbol,asset_in_symbol,asset_out_amount)
 
             except Exception as e:
                 self.logger.debug(f"error execute_order {e}")
                 return
 
-        if order_type == 'market'
+        if order_type == 'market':
             self.logger.debug(f"execute_order {order_type}")
             return
-        if order_type == 'limit'
+        if order_type == 'limit':
             self.logger.debug(f"execute_order {order_type}")
             return
 
     async def get_swap(self, 
             asset_out_symbol: str, 
             asset_in_symbol: str,
             amount: int, 
@@ -375,14 +286,16 @@
     async def get_block_explorer_status(self,txHash):
         self.logger.debug(f"get_block_explorer_status {txHash}")
         checkTransactionSuccessURL = f"{self.block_explorer_url}?module=transaction&action=gettxreceiptstatus&txhash={txHash}&apikey={self.block_explorer_api}"
         checkTransactionRequest =  self.get(checkTransactionSuccessURL)
         return checkTransactionRequest['status']
 
 
+####CONTRACT SEARCH
+
     # async def search_gecko_platform(self):
     #     self.logger.debug("search_gecko_platform")
     #     try:
     #         assetplatform = self.gecko_api.get_asset_platforms()
     #         output_dict = [x for x in assetplatform if x['chain_identifier'] == int(self.chain_id)]
     #         self.logger.debug(f"search_gecko_platform search {output_dict}")
     #         return output_dict[0]['id']
@@ -472,14 +385,103 @@
             token_address = await self.search_contract(token)
             token_abi = await self.get_abi(token_address)
             return self.w3.eth.contract(address=token_address, abi=token_abi)
         except Exception as e:
             self.logger.error(f"error  get_token_contract {e}")
             return
 
+
+####UTILS
+    async def get_approve(self, asset_out_address: str, amount=None):
+        self.logger.debug(f"get_approve {asset_out_address}")
+        if self.protocol_type in ["1inch","1inch_limit"]:
+            approval_check_URL = f"{self.dex_url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
+            approval_response = await self._get(approval_check_URL)
+            approval_check = approval_response['allowance']
+            if (approval_check==0):
+                approval_URL = f"{self.dex_url}/approve/transaction?tokenAddress={asset_out_address}"
+                approval_response = await self._get(approval_URL)
+        elif self.protocol_type in ["uniswap_v2","uniswap_v3"]:
+            asset_out_abi= await self.get_abi(asset_out_address)
+            asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)           
+            approval_check = asset_out_contract.functions.allowance(self.w3.to_checksum_address(self.wallet_address), self.w3.to_checksum_address(self.router)).call()
+            if (approval_check==0):
+                approved_amount = (self.w3.to_wei(2**64-1,'ether'))
+                asset_out_abi = await fetch_abi_dex(asset_out_address)
+                asset_out_contract = self.w3.eth.contract(address=asset_out_address, abi=asset_out_abi)
+                approval_TX = asset_out_contract.functions.approve(self.w3.to_checksum_address(self.router), approved_amount)
+                approval_txHash = await sign_transaction_dex(approval_TX)
+                approval_txHash_complete = self.w3.eth.wait_for_transaction_receipt(approval_txHash, timeout=120, poll_latency=0.1)
+
+    async def get_sign(self, tx):
+        self.logger.debug(f"get_sign {tx}")
+        try:
+            if self.protocol_type in ['uniswap_v2']:
+                tx_params = {
+                'from': self.wallet_address,
+                'gas': await self.get_gas(tx),
+                'gasPrice': await self.get_gasPrice(tx),
+                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
+                }
+                tx = tx.build_transaction(tx_params)
+            elif self.protocol_type in ['uniswap_v3']:
+                tx_params = {
+                'from': self.wallet_address,
+                'gas': await estimate_gas(tx),
+                'gasPrice': await self.get_gasPrice(tx),
+                'nonce': self.w3.eth.get_transaction_count(self.wallet_address),
+                }
+                tx = tx.build_transaction(tx_params)
+            elif self.protocol_type in ["1inch","1inch_limit"]:
+                tx = tx['tx']
+                tx['gas'] = await estimate_gas(tx)
+                tx['nonce'] = self.w3.eth.get_transaction_count(self.wallet_address)
+                tx['value'] = int(tx['value'])
+                tx['gasPrice'] = await self.get_gasPrice(tx)
+            signed = self.w3.eth.account.sign_transaction(tx, self.private_key)
+            raw_tx = signed.rawTransaction
+            return self.w3.eth.send_raw_transaction(raw_tx)
+        except Exception as e:
+            self.logger.debug(f"error get_sign {e}")
+            return
+
+
+    async def get_gas(self, tx):
+        self.logger.debug(f"get_gas {tx}")
+        gasestimate= self.web3.eth.estimate_gas(tx) * 1.25
+        return int(self.w3.to_wei(gasestimate,'wei'))
+
+    async def get_gasPrice(self, tx):
+        self.logger.debug(f"get_gasPrice {tx}")
+        gasprice= self.w3.eth.generate_gas_price()
+        return self.w3.to_wei(gasPrice,'gwei')
+
+    async def get_abi(self,addr):
+        self.logger.debug(f"get_abi {addr}")
+        try:
+            params = {
+                "module": "contract",
+                "action": "getabi",
+                "address": addr,
+                "apikey": self.block_explorer_api }
+            headers = { "User-Agent": "Mozilla/5.0" }
+            resp = await self._get(url=self.block_explorer_url,params=params,headers=headers)
+            #self.logger.debug(f"resp {resp} status {resp['status']}")
+            if resp['status']=="1":
+                self.logger.debug(f"ABI found {resp}")
+                abi = resp["result"]
+                return abi
+            else:
+                self.logger.debug(f"No ABI identified Option B needed for contract {addr} on chain {self.chain_id}")
+        except Exception as e:
+            self.logger.debug(f"error get_abi {e}")
+            return
+
+#####USERS
+
     async def get_token_balance(self, token):
         self.logger.debug(f"get_token_balance {token}")
         try:
             token_address = await self.search_contract(token)
             token_abi =  await self.get_abi(token_address)
             token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
             token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
@@ -520,15 +522,14 @@
             # asset_position_contract = ex.eth.contract(address=asset_out_address, abi=asset_out_abi)
             # open_positions = asset_position_contract.functions.getOpenPositions(walletaddress).call()
             return
         except Exception as e:
             logger.error(msg=f"get_account_position error: {e}")
             return 0
 
-
     # async def fetch_account_dex(addr):
     #     url = block_explorer_url
     #     query = {'module':'account',
     #             'action':'tokenbalance',
     #             'contractaddress':addr,
     #             'address':walletaddress,
     #             'tag':'latest',
@@ -536,15 +537,14 @@
     #     r = requests.get(url, params=query)
     #     try:
     #         d = json.loads(r.text)
     #     except:
     #         return None
     #     return int(d['result']) / self.zeroes
 
-
 #     async def fetch_gecko_asset_price(token):
 #     try:
 #         asset_in_address = ex.to_checksum_address(await search_contract(token))
 #         fetch_tokeninfo = gecko_api.get_coin_info_from_contract_address_by_id(id=f'{coin_platform}',contract_address=asset_in_address)
 #         return fetch_tokeninfo['market_data']['current_price']['usd']
 #     except Exception:
 #         return
```

### Comparing `dxsp-1.2.1/pyproject.toml` & `dxsp-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.2.1"
+version = "1.2.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.2.1/PKG-INFO` & `dxsp-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.2.1
+Version: 1.2.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

