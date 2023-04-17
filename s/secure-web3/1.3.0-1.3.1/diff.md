# Comparing `tmp/secure_web3-1.3.0.tar.gz` & `tmp/secure_web3-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure_web3-1.3.0.tar", last modified: Mon Apr 17 20:51:37 2023, max compression
+gzip compressed data, was "secure_web3-1.3.1.tar", last modified: Mon Apr 17 21:17:55 2023, max compression
```

## Comparing `secure_web3-1.3.0.tar` & `secure_web3-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.420738 secure_web3-1.3.0/
--rw-r--r--   0 anon      (1000) anon      (1000)     1080 2023-02-21 22:28:09.000000 secure_web3-1.3.0/LICENSE.txt
--rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 20:51:37.420738 secure_web3-1.3.0/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)     2761 2023-04-03 00:13:38.000000 secure_web3-1.3.0/README.md
--rw-r--r--   0 anon      (1000) anon      (1000)      666 2023-04-17 20:51:25.000000 secure_web3-1.3.0/pyproject.toml
--rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-17 20:51:37.420738 secure_web3-1.3.0/setup.cfg
--rw-r--r--   0 anon      (1000) anon      (1000)      554 2023-04-17 20:51:25.000000 secure_web3-1.3.0/setup.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.404738 secure_web3-1.3.0/src/
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.408738 secure_web3-1.3.0/src/secure_web3/
--rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-03-08 04:05:51.000000 secure_web3-1.3.0/src/secure_web3/__init__.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.412738 secure_web3-1.3.0/src/secure_web3/data/
--rw-r--r--   0 anon      (1000) anon      (1000)      717 2023-02-21 22:41:47.000000 secure_web3-1.3.0/src/secure_web3/data/networks.json
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.412738 secure_web3-1.3.0/src/secure_web3/keys/
--rw-r--r--   0 anon      (1000) anon      (1000)      162 2023-01-26 23:28:56.000000 secure_web3-1.3.0/src/secure_web3/keys/default_wallet.json
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.416738 secure_web3-1.3.0/src/secure_web3/lib/
--rw-r--r--   0 anon      (1000) anon      (1000)     6187 2023-01-22 21:32:35.000000 secure_web3-1.3.0/src/secure_web3/lib/abi_lib.py
--rw-r--r--   0 anon      (1000) anon      (1000)      660 2023-03-08 05:44:20.000000 secure_web3-1.3.0/src/secure_web3/lib/inputs.py
--rw-r--r--   0 anon      (1000) anon      (1000)      257 2023-02-21 22:39:53.000000 secure_web3-1.3.0/src/secure_web3/lib/load_networks.py
--rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-01-22 21:27:26.000000 secure_web3-1.3.0/src/secure_web3/lib/style.py
--rw-r--r--   0 anon      (1000) anon      (1000)      580 2023-01-26 23:29:39.000000 secure_web3-1.3.0/src/secure_web3/lib/w3_validation.py
--rw-r--r--   0 anon      (1000) anon      (1000)     8025 2023-03-14 01:49:35.000000 secure_web3-1.3.0/src/secure_web3/lib/wallet_manager.py
--rw-r--r--   0 anon      (1000) anon      (1000)     6418 2023-04-17 20:51:08.000000 secure_web3-1.3.0/src/secure_web3/sw3.py
--rw-r--r--   0 anon      (1000) anon      (1000)    16577 2023-03-12 03:08:22.000000 secure_web3-1.3.0/src/secure_web3/sw3_wallet.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.412738 secure_web3-1.3.0/src/secure_web3.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)      598 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       50 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       12 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.632790 secure_web3-1.3.1/
+-rw-r--r--   0 anon      (1000) anon      (1000)     1080 2023-02-21 22:28:09.000000 secure_web3-1.3.1/LICENSE.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 21:17:55.632790 secure_web3-1.3.1/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)     2761 2023-04-03 00:13:38.000000 secure_web3-1.3.1/README.md
+-rw-r--r--   0 anon      (1000) anon      (1000)      666 2023-04-17 21:17:39.000000 secure_web3-1.3.1/pyproject.toml
+-rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-17 21:17:55.632790 secure_web3-1.3.1/setup.cfg
+-rw-r--r--   0 anon      (1000) anon      (1000)      554 2023-04-17 21:17:39.000000 secure_web3-1.3.1/setup.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.624790 secure_web3-1.3.1/src/
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.624790 secure_web3-1.3.1/src/secure_web3/
+-rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-03-08 04:05:51.000000 secure_web3-1.3.1/src/secure_web3/__init__.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3/data/
+-rw-r--r--   0 anon      (1000) anon      (1000)      717 2023-02-21 22:41:47.000000 secure_web3-1.3.1/src/secure_web3/data/networks.json
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3/keys/
+-rw-r--r--   0 anon      (1000) anon      (1000)      162 2023-01-26 23:28:56.000000 secure_web3-1.3.1/src/secure_web3/keys/default_wallet.json
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3/lib/
+-rw-r--r--   0 anon      (1000) anon      (1000)     6187 2023-01-22 21:32:35.000000 secure_web3-1.3.1/src/secure_web3/lib/abi_lib.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      660 2023-03-08 05:44:20.000000 secure_web3-1.3.1/src/secure_web3/lib/inputs.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      257 2023-02-21 22:39:53.000000 secure_web3-1.3.1/src/secure_web3/lib/load_networks.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-01-22 21:27:26.000000 secure_web3-1.3.1/src/secure_web3/lib/style.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      580 2023-01-26 23:29:39.000000 secure_web3-1.3.1/src/secure_web3/lib/w3_validation.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     8025 2023-03-14 01:49:35.000000 secure_web3-1.3.1/src/secure_web3/lib/wallet_manager.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     6418 2023-04-17 20:51:08.000000 secure_web3-1.3.1/src/secure_web3/sw3.py
+-rw-r--r--   0 anon      (1000) anon      (1000)    16528 2023-04-17 21:16:45.000000 secure_web3-1.3.1/src/secure_web3/sw3_wallet.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)      598 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       50 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       12 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/top_level.txt
```

### Comparing `secure_web3-1.3.0/LICENSE.txt` & `secure_web3-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/PKG-INFO` & `secure_web3-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_web3
-Version: 1.3.0
+Version: 1.3.1
 Summary: Secure wallet and development enviroment
 Home-page: https://github.com/darkerego/secure_web3
 Author: darkerego
 Author-email: Darkergo <chevisyoung@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/darkerego/secure_web3
 Project-URL: Bug Tracker, https://github.com/darkerego/secure_web3/issues
```

### Comparing `secure_web3-1.3.0/README.md` & `secure_web3-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/pyproject.toml` & `secure_web3-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "secure_web3"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Darkergo", email="chevisyoung@gmail.com" },
 ]
 description = "Secure wallet and development enviroment"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_web3-1.3.0/src/secure_web3/data/networks.json` & `secure_web3-1.3.1/src/secure_web3/data/networks.json`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/src/secure_web3/lib/abi_lib.py` & `secure_web3-1.3.1/src/secure_web3/lib/abi_lib.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/src/secure_web3/lib/inputs.py` & `secure_web3-1.3.1/src/secure_web3/lib/inputs.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/src/secure_web3/lib/style.py` & `secure_web3-1.3.1/src/secure_web3/lib/style.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/src/secure_web3/lib/w3_validation.py` & `secure_web3-1.3.1/src/secure_web3/lib/w3_validation.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/src/secure_web3/lib/wallet_manager.py` & `secure_web3-1.3.1/src/secure_web3/lib/wallet_manager.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/src/secure_web3/sw3.py` & `secure_web3-1.3.1/src/secure_web3/sw3.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.0/src/secure_web3/sw3_wallet.py` & `secure_web3-1.3.1/src/secure_web3/sw3_wallet.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 import requests
 import web3
 from eth_typing import HexStr
 from web3.contract import Contract
 from web3.exceptions import TransactionNotFound
 from web3.middleware import geth_poa_middleware
 from web3.types import RPCResponse
-
+from eth_utils import to_checksum_address
 import secure_web3.lib.style
+from eth_utils import to_checksum_address, to_wei
+
 from secure_web3.lib.w3_validation import validate_addr, valid_token
 from secure_web3.lib.wallet_manager import WalletManager
 from secure_web3.sw3 import SecureWeb3
 
 
 class EtherShellWallet:
     def __init__(self, sw3: SecureWeb3):
@@ -111,18 +113,20 @@
 
     def _token(self, token_address: str) -> Contract:
         """
         Create and return a Contract object with the ERC/BEP/20 abi
         :param token_address: contract address string
         :return: Contract object
         """
+
+
         if self.sw3.w3.eth.chain_id == 56:
-            token = self.sw3.w3.eth.contract(self.sw3.w3.toChecksumAddress(token_address), abi=lib.abi_lib.BEP_ABI)
+            token = self.sw3.w3.eth.contract(to_checksum_address(token_address), abi=lib.abi_lib.BEP_ABI)
         else:
-            token = self.sw3.w3.eth.contract(self.sw3.w3.toChecksumAddress(token_address), abi=lib.abi_lib.EIP20_ABI)
+            token = self.sw3.w3.eth.contract(to_checksum_address(token_address), abi=lib.abi_lib.EIP20_ABI)
         return token
 
     def eth_balance(self, raw: bool = False) -> (int, float):
         """
 
         :param raw: if true return raw integer
         :return:
@@ -130,25 +134,25 @@
         self._balance = sw3.w3.eth.getBalance(sw3.account.address)
         if raw:
             return self._balance
         return self._balance / (10 ** 18)
 
     def token_convert(self, token_address: str, qty: int) -> float:
         for token in self.sw3.tokens:
-            if self.sw3.w3.toChecksumAddress(token_address) == self.sw3.w3.toChecksumAddress(token.get("address")):
+            if to_checksum_address(token_address) == to_checksum_address(token.get("address")):
                 dec = token.get('decimals')
                 return int(qty / (10 ** dec))
 
     def token_balance(self, token_address: str, raw: bool = False) -> (int, float):
         token = self._token(token_address)
         token_balance = token.functions.balanceOf(self.sw3.account.address).call()
         if raw:
             return token_balance
         for tok in self.sw3.tokens:
-            if self.sw3.w3.toChecksumAddress(tok.get('address')) == self.sw3.w3.toChecksumAddress(token_address):
+            if to_checksum_address(tok.get('address')) == to_checksum_address(token_address):
                 dec = int(tok.get('decimals'))
                 return token_balance / (10 ** dec)
 
     def poll_receipt(self, tx_hash: hex):
         poll = 0
         while True:
             if poll > 100:
@@ -163,23 +167,23 @@
             else:
                 receipt = receipt.__dict__
                 return receipt
         self.sw3.printer.error('Timed out, transaction may be underpriced!')
 
     def send_erc20_token(self, raw_amount: int, destination: str, token_address: str, legacy: bool = False,
                          private: bool = False) -> HexStr:
-        token = self.sw3.w3.eth.contract(self.sw3.w3.toChecksumAddress(token_address), abi=lib.abi_lib.EIP20_ABI)
+        token = self.sw3.w3.eth.contract(to_checksum_address(token_address), abi=lib.abi_lib.EIP20_ABI)
         mpfpg, mfpg = self.query_gas_api()
         if self.sw3.w3.eth.chain_id in [0, 1, 5, 137]:
             tx = {
                 'maxPriorityFeePerGas': self.sw3.w3.toWei(mpfpg, 'gwei'),
                 'maxFeePerGas': self.sw3.w3.toWei(mfpg, 'gwei'),
-                "to": self.sw3.w3.toChecksumAddress(destination),
+                "to": to_checksum_address(destination),
                 "value": "0x0",
-                "data": token.encodeABI('transfer', args=(self.sw3.w3.toChecksumAddress(destination), raw_amount)),
+                "data": token.encodeABI('transfer', args=(to_checksum_address(destination), raw_amount)),
                 "nonce": self.sw3.w3.eth.get_transaction_count(self.sw3.account.address),
                 "chainId": self.sw3.w3.eth.chain_id
             }
             if legacy:
                 tx.pop('maxFeePerGas')
                 tx.pop('maxPriorityFeePerGas')
                 tx.pop('type')
@@ -190,40 +194,40 @@
             return self.broadcast_raw_tx(tx, private)
 
     def send_eth(self, raw_amount: int, destination: str, legacy: bool = False, private: bool = False) -> HexStr:
         mpfpg, mfpg = self.query_gas_api()
 
         tx = {
             'nonce': self.sw3.w3.eth.get_transaction_count(self.sw3.account.address),
-            'to': self.sw3.w3.toChecksumAddress(destination),
+            'to': to_checksum_address(destination),
             'value': raw_amount,
-            'maxFeePerGas': self.sw3.w3.toWei(mfpg, 'gwei'),
-            'maxPriorityFeePerGas': self.sw3.w3.toWei(mpfpg, 'gwei'),
+            'maxFeePerGas': to_wei(mfpg, 'gwei'),
+            'maxPriorityFeePerGas': to_wei(mpfpg, 'gwei'),
             'type': 2,
             'chainId': hex(self.sw3.w3.eth.chain_id)
         }
         if legacy:
             tx.pop('maxFeePerGas')
             tx.pop('maxPriorityFeePerGas')
             tx.pop('type')
-            tx.update({'gasPrice': self.sw3.w3.toWei(int(self.sw3.w3.eth.gas_price * 1.1), 'gwei')})
+            tx.update({'gasPrice': to_wei(int(self.sw3.w3.eth.gas_price * 1.1), 'gwei')})
         gas = self.sw3.w3.eth.estimate_gas(tx)
         tx.update({'gas': gas})
         return self.broadcast_raw_tx(tx, private)
 
     def import_token(self, token_address: str) -> bool:
         if not validate_addr(token_address):
             return False
         if not valid_token(self._token(token_address)):
             return False
         token = self._token(token_address)
         decimals = token.functions.decimals().call()
         symbol = token.functions.symbol().call()
         balance = token.functions.balanceOf(self.sw3.account.address).call()
-        token_dict = {'address': self.sw3.w3.toChecksumAddress(token_address),
+        token_dict = {'address': to_checksum_address(token_address),
                       'network': self.sw3.w3.eth.chain_id,
                       'decimals': decimals,
                       'symbol': symbol,
                       'balance': balance}
         self.sw3.tokens.append(token_dict)
         self.sw3.wallet.wallet.update_wallet('tokens', self.sw3.tokens)
         return True
```

### Comparing `secure_web3-1.3.0/src/secure_web3.egg-info/PKG-INFO` & `secure_web3-1.3.1/src/secure_web3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-web3
-Version: 1.3.0
+Version: 1.3.1
 Summary: Secure wallet and development enviroment
 Home-page: https://github.com/darkerego/secure_web3
 Author: darkerego
 Author-email: Darkergo <chevisyoung@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/darkerego/secure_web3
 Project-URL: Bug Tracker, https://github.com/darkerego/secure_web3/issues
```

### Comparing `secure_web3-1.3.0/src/secure_web3.egg-info/SOURCES.txt` & `secure_web3-1.3.1/src/secure_web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

