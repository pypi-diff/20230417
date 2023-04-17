# Comparing `tmp/dxsp-1.2.2.tar.gz` & `tmp/dxsp-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.2.2.tar", max compression
+gzip compressed data, was "dxsp-1.2.3.tar", max compression
```

## Comparing `dxsp-1.2.2.tar` & `dxsp-1.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-17 08:17:22.790547 dxsp-1.2.2/LICENSE
--rw-r--r--   0        0        0     3225 2023-04-17 08:17:22.790547 dxsp-1.2.2/README.md
--rw-r--r--   0        0        0      136 2023-04-17 08:17:23.486556 dxsp-1.2.2/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-17 08:17:22.790547 dxsp-1.2.2/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8675 2023-04-17 08:17:22.790547 dxsp-1.2.2/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    27036 2023-04-17 08:17:22.790547 dxsp-1.2.2/dxsp/main.py
--rw-r--r--   0        0        0      929 2023-04-17 08:17:23.482556 dxsp-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 dxsp-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-17 08:33:25.022310 dxsp-1.2.3/LICENSE
+-rw-r--r--   0        0        0     3225 2023-04-17 08:33:25.022310 dxsp-1.2.3/README.md
+-rw-r--r--   0        0        0      136 2023-04-17 08:33:25.682304 dxsp-1.2.3/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-17 08:33:25.022310 dxsp-1.2.3/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8675 2023-04-17 08:33:25.022310 dxsp-1.2.3/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    27341 2023-04-17 08:33:25.022310 dxsp-1.2.3/dxsp/main.py
+-rw-r--r--   0        0        0      944 2023-04-17 08:33:25.682304 dxsp-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4054 1970-01-01 00:00:00.000000 dxsp-1.2.3/PKG-INFO
```

### Comparing `dxsp-1.2.2/LICENSE` & `dxsp-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.2/README.md` & `dxsp-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.2/dxsp/assets/blockchains.py` & `dxsp-1.2.3/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.2.2/dxsp/main.py` & `dxsp-1.2.3/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from dxsp.assets.blockchains import blockchains
 
 import os, json, requests, asyncio, logging
 
 from dotenv import load_dotenv
 
 from web3 import Web3
-from datetime import datetime
 from pycoingecko import CoinGeckoAPI
 
 from ping3 import ping
 
 class DexSwap:
 
 
@@ -267,17 +266,19 @@
             if swap_TX:
                 self.logger.debug(f"swap_TX {swap_TX}")
                 signed_TX = await self.get_sign(swap_TX)
                 txHash = str(self.w3.to_hex(signed_TX))
                 txResult = await self.get_block_explorer_status(txHash)
                 txHashDetail= self.w3.wait_for_transaction_receipt(txHash, timeout=120, poll_latency=0.1)
                 if(txResult == "1"):
+                    blockNumber = txHashDetail['blockNumber']
+                    transaction_block = self.w3.eth.get_block(blockNumber)
                     order={}
                     d['id'] = '15222'
-                    d['datetime'] = datetime.now()
+                    d['timestamp'] = transaction_block['timestamp']
                     d['gasUsed'] = txHashDetail['gasUsed']
                     d['id'] = '15222'
                     d['amount'] = 'host name'
                     d['price'] = '15222'
                     return txHash
         except Exception as e:
             self.logger.debug(f"error get_swap {e}")
@@ -474,14 +475,21 @@
                 self.logger.debug(f"No ABI identified Option B needed for contract {addr} on chain {self.chain_id}")
         except Exception as e:
             self.logger.debug(f"error get_abi {e}")
             return
 
 #####USERS
 
+    async def get_wallet_auth():
+        try:
+            return
+        except Exception as e:
+            self.logger.error(msg=f"get_wallet_auth error: {e}")
+            return
+
     async def get_token_balance(self, token):
         self.logger.debug(f"get_token_balance {token}")
         try:
             token_address = await self.search_contract(token)
             token_abi =  await self.get_abi(token_address)
             token_contract = self.w3.eth.contract(address=token_address, abi=token_abi)
             token_balance = token_contract.functions.balanceOf(self.wallet_address).call()
```

### Comparing `dxsp-1.2.2/pyproject.toml` & `dxsp-1.2.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.2.2"
+version = "1.2.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 asyncio = "*"
 python-dotenv = "*"
 web3 = ">=6.*"
 pycoingecko = "*"
 ping3 = "*"
+dynaconf = "*"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dxsp-1.2.2/PKG-INFO` & `dxsp-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.2.2
+Version: 1.2.3
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
+Requires-Dist: dynaconf
 Requires-Dist: ping3
 Requires-Dist: pycoingecko
 Requires-Dist: python-dotenv
 Requires-Dist: web3 (>=6)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
```

