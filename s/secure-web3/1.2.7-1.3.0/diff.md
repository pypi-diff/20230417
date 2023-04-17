# Comparing `tmp/secure_web3-1.2.7.tar.gz` & `tmp/secure_web3-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure_web3-1.2.7.tar", last modified: Sun Apr  2 22:58:25 2023, max compression
+gzip compressed data, was "secure_web3-1.3.0.tar", last modified: Mon Apr 17 20:51:37 2023, max compression
```

## Comparing `secure_web3-1.2.7.tar` & `secure_web3-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-02 22:58:25.948085 secure_web3-1.2.7/
--rw-r--r--   0 anon      (1000) anon      (1000)     1080 2023-02-21 22:28:09.000000 secure_web3-1.2.7/LICENSE.txt
--rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-02 22:58:25.948085 secure_web3-1.2.7/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)     2761 2023-04-02 22:58:14.000000 secure_web3-1.2.7/README.md
--rw-r--r--   0 anon      (1000) anon      (1000)      666 2023-04-02 22:58:14.000000 secure_web3-1.2.7/pyproject.toml
--rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-02 22:58:25.948085 secure_web3-1.2.7/setup.cfg
--rw-r--r--   0 anon      (1000) anon      (1000)      566 2023-04-02 22:58:14.000000 secure_web3-1.2.7/setup.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-02 22:58:25.936085 secure_web3-1.2.7/src/
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-02 22:58:25.940085 secure_web3-1.2.7/src/secure_web3/
--rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-03-08 04:05:51.000000 secure_web3-1.2.7/src/secure_web3/__init__.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-02 22:58:25.944085 secure_web3-1.2.7/src/secure_web3/data/
--rw-r--r--   0 anon      (1000) anon      (1000)      717 2023-02-21 22:41:47.000000 secure_web3-1.2.7/src/secure_web3/data/networks.json
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-02 22:58:25.944085 secure_web3-1.2.7/src/secure_web3/keys/
--rw-r--r--   0 anon      (1000) anon      (1000)      162 2023-01-26 23:28:56.000000 secure_web3-1.2.7/src/secure_web3/keys/default_wallet.json
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-02 22:58:25.948085 secure_web3-1.2.7/src/secure_web3/lib/
--rw-r--r--   0 anon      (1000) anon      (1000)     6187 2023-01-22 21:32:35.000000 secure_web3-1.2.7/src/secure_web3/lib/abi_lib.py
--rw-r--r--   0 anon      (1000) anon      (1000)      660 2023-03-08 05:44:20.000000 secure_web3-1.2.7/src/secure_web3/lib/inputs.py
--rw-r--r--   0 anon      (1000) anon      (1000)      257 2023-02-21 22:39:53.000000 secure_web3-1.2.7/src/secure_web3/lib/load_networks.py
--rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-01-22 21:27:26.000000 secure_web3-1.2.7/src/secure_web3/lib/style.py
--rw-r--r--   0 anon      (1000) anon      (1000)      580 2023-01-26 23:29:39.000000 secure_web3-1.2.7/src/secure_web3/lib/w3_validation.py
--rw-r--r--   0 anon      (1000) anon      (1000)     8025 2023-03-14 01:49:35.000000 secure_web3-1.2.7/src/secure_web3/lib/wallet_manager.py
--rw-r--r--   0 anon      (1000) anon      (1000)     6208 2023-04-02 22:53:56.000000 secure_web3-1.2.7/src/secure_web3/sw3.py
--rw-r--r--   0 anon      (1000) anon      (1000)    16577 2023-03-12 03:08:22.000000 secure_web3-1.2.7/src/secure_web3/sw3_wallet.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-02 22:58:25.944085 secure_web3-1.2.7/src/secure_web3.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-02 22:58:25.000000 secure_web3-1.2.7/src/secure_web3.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)      598 2023-04-02 22:58:25.000000 secure_web3-1.2.7/src/secure_web3.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-02 22:58:25.000000 secure_web3-1.2.7/src/secure_web3.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       59 2023-04-02 22:58:25.000000 secure_web3-1.2.7/src/secure_web3.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       12 2023-04-02 22:58:25.000000 secure_web3-1.2.7/src/secure_web3.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.420738 secure_web3-1.3.0/
+-rw-r--r--   0 anon      (1000) anon      (1000)     1080 2023-02-21 22:28:09.000000 secure_web3-1.3.0/LICENSE.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 20:51:37.420738 secure_web3-1.3.0/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)     2761 2023-04-03 00:13:38.000000 secure_web3-1.3.0/README.md
+-rw-r--r--   0 anon      (1000) anon      (1000)      666 2023-04-17 20:51:25.000000 secure_web3-1.3.0/pyproject.toml
+-rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-17 20:51:37.420738 secure_web3-1.3.0/setup.cfg
+-rw-r--r--   0 anon      (1000) anon      (1000)      554 2023-04-17 20:51:25.000000 secure_web3-1.3.0/setup.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.404738 secure_web3-1.3.0/src/
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.408738 secure_web3-1.3.0/src/secure_web3/
+-rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-03-08 04:05:51.000000 secure_web3-1.3.0/src/secure_web3/__init__.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.412738 secure_web3-1.3.0/src/secure_web3/data/
+-rw-r--r--   0 anon      (1000) anon      (1000)      717 2023-02-21 22:41:47.000000 secure_web3-1.3.0/src/secure_web3/data/networks.json
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.412738 secure_web3-1.3.0/src/secure_web3/keys/
+-rw-r--r--   0 anon      (1000) anon      (1000)      162 2023-01-26 23:28:56.000000 secure_web3-1.3.0/src/secure_web3/keys/default_wallet.json
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.416738 secure_web3-1.3.0/src/secure_web3/lib/
+-rw-r--r--   0 anon      (1000) anon      (1000)     6187 2023-01-22 21:32:35.000000 secure_web3-1.3.0/src/secure_web3/lib/abi_lib.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      660 2023-03-08 05:44:20.000000 secure_web3-1.3.0/src/secure_web3/lib/inputs.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      257 2023-02-21 22:39:53.000000 secure_web3-1.3.0/src/secure_web3/lib/load_networks.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-01-22 21:27:26.000000 secure_web3-1.3.0/src/secure_web3/lib/style.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      580 2023-01-26 23:29:39.000000 secure_web3-1.3.0/src/secure_web3/lib/w3_validation.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     8025 2023-03-14 01:49:35.000000 secure_web3-1.3.0/src/secure_web3/lib/wallet_manager.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     6418 2023-04-17 20:51:08.000000 secure_web3-1.3.0/src/secure_web3/sw3.py
+-rw-r--r--   0 anon      (1000) anon      (1000)    16577 2023-03-12 03:08:22.000000 secure_web3-1.3.0/src/secure_web3/sw3_wallet.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 20:51:37.412738 secure_web3-1.3.0/src/secure_web3.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)      598 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       50 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       12 2023-04-17 20:51:37.000000 secure_web3-1.3.0/src/secure_web3.egg-info/top_level.txt
```

### Comparing `secure_web3-1.2.7/LICENSE.txt` & `secure_web3-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/PKG-INFO` & `secure_web3-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_web3
-Version: 1.2.7
+Version: 1.3.0
 Summary: Secure wallet and development enviroment
 Home-page: https://github.com/darkerego/secure_web3
 Author: darkerego
 Author-email: Darkergo <chevisyoung@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/darkerego/secure_web3
 Project-URL: Bug Tracker, https://github.com/darkerego/secure_web3/issues
@@ -75,15 +75,15 @@
 See main.py for example use.
 </p>
 
 ### Installation 
 <p>
 To install with pip:
 </p>
-pip3 install secure-web3==1.2.7
+pip3 install secure-web3==1.2.8
 
 <p>
 You can also install from source by cloning this repo, installing the dependencies in requirements.txt, 
 and running `setup.py build`  and then `setup.py install`.
 </p>
 
 ### Configuration
```

### Comparing `secure_web3-1.2.7/README.md` & `secure_web3-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 See main.py for example use.
 </p>
 
 ### Installation 
 <p>
 To install with pip:
 </p>
-pip3 install secure-web3==1.2.7
+pip3 install secure-web3==1.2.8
 
 <p>
 You can also install from source by cloning this repo, installing the dependencies in requirements.txt, 
 and running `setup.py build`  and then `setup.py install`.
 </p>
 
 ### Configuration
```

### Comparing `secure_web3-1.2.7/pyproject.toml` & `secure_web3-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "secure_web3"
-version = "1.2.7"
+version = "1.3.0"
 authors = [
   { name="Darkergo", email="chevisyoung@gmail.com" },
 ]
 description = "Secure wallet and development enviroment"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_web3-1.2.7/setup.py` & `secure_web3-1.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='secure_web3',
-    version='1.2.7',
+    version='1.3.0',
     packages=['secure_web3'],
-    install_requires=['web3', 'pycryptodome', 'python-dotenv', 'eth-utils', 'colored', 'pycrypto'],
+    install_requires=['web3', 'pycryptodome', 'python-dotenv', 'eth-utils', 'colored'],
     package_dir={"": "src"},
     include_package_data=True,
     data_files=[('', ['src/secure_web3/keys/default_wallet.json', 'src/secure_web3/data/networks.json'])],
     url='https://github.com/darkerego/secure_web3',
     license='MIT',
     author='darkerego',
     author_email='chevisyoung@gmail.com',
```

### Comparing `secure_web3-1.2.7/src/secure_web3/data/networks.json` & `secure_web3-1.3.0/src/secure_web3/data/networks.json`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/src/secure_web3/lib/abi_lib.py` & `secure_web3-1.3.0/src/secure_web3/lib/abi_lib.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/src/secure_web3/lib/inputs.py` & `secure_web3-1.3.0/src/secure_web3/lib/inputs.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/src/secure_web3/lib/style.py` & `secure_web3-1.3.0/src/secure_web3/lib/style.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/src/secure_web3/lib/w3_validation.py` & `secure_web3-1.3.0/src/secure_web3/lib/w3_validation.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/src/secure_web3/lib/wallet_manager.py` & `secure_web3-1.3.0/src/secure_web3/lib/wallet_manager.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/src/secure_web3/sw3.py` & `secure_web3-1.3.0/src/secure_web3/sw3.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,25 @@
 import dotenv
 import web3
 from eth_typing import HexStr
 from web3.middleware import geth_poa_middleware
 import secure_web3.lib.abi_lib
 import secure_web3.lib.style
 from secure_web3.lib.wallet_manager import WalletManager
-from lib import load_networks
+from secure_web3.lib import load_networks
+
 
 
 class Web3RpcNotConfigured(Exception):
     pass
 
+class WalletFileNotFound(Exception):
+    pass
+
+
 
 class SecureWeb3:
     def __init__(self, wallet_file: str = None, network: str = 'ethereum',
                  use_flashbots: bool = False):
         # dotenv.load_dotenv()
         self.endpoint = None
         self.use_flashbots = use_flashbots
@@ -110,35 +115,35 @@
     def w3(self) -> web3.Web3:
         """
         Access web3
         :return:
         """
         return self._w3
 
-
-
-
-
-
     def switch_network(self, network_name: str, poa: bool = False) -> None:
         """
         Switch network of w3 connections
         :param network_name:
         :param poa: load point of authority middleware for networks like polygon
         """
         endpoint = os.environ.get(f'infura_{network_name}_endpoint')
         if not endpoint:
             self.printer.error('Could not find network, is it configured?')
             return
+        self.endpoint = endpoint
         w3 = web3.Web3(web3.HTTPProvider(endpoint))
         if network_name == 'polygon':
             poa = True
         if poa:
             w3.middleware_onion.inject(geth_poa_middleware)
-        if w3.isConnected():
+        if hasattr(w3, 'isConnected'):
+            is_conn = w3.isConnected()
+        else:
+            is_conn = w3.is_connected
+        if is_conn:
             self.printer.good(f'Successfully switched to {network_name}')
         else:
             self.printer.error(f'Web3 could not connect to endpoint at {endpoint}')
 
 
 if __name__ == '__main__':
     networks = load_networks.load_networks()
```

### Comparing `secure_web3-1.2.7/src/secure_web3/sw3_wallet.py` & `secure_web3-1.3.0/src/secure_web3/sw3_wallet.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.2.7/src/secure_web3.egg-info/PKG-INFO` & `secure_web3-1.3.0/src/secure_web3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-web3
-Version: 1.2.7
+Version: 1.3.0
 Summary: Secure wallet and development enviroment
 Home-page: https://github.com/darkerego/secure_web3
 Author: darkerego
 Author-email: Darkergo <chevisyoung@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/darkerego/secure_web3
 Project-URL: Bug Tracker, https://github.com/darkerego/secure_web3/issues
@@ -75,15 +75,15 @@
 See main.py for example use.
 </p>
 
 ### Installation 
 <p>
 To install with pip:
 </p>
-pip3 install secure-web3==1.2.7
+pip3 install secure-web3==1.2.8
 
 <p>
 You can also install from source by cloning this repo, installing the dependencies in requirements.txt, 
 and running `setup.py build`  and then `setup.py install`.
 </p>
 
 ### Configuration
```

### Comparing `secure_web3-1.2.7/src/secure_web3.egg-info/SOURCES.txt` & `secure_web3-1.3.0/src/secure_web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

