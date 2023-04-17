# Comparing `tmp/ethereal-0.1.2.tar.gz` & `tmp/ethereal-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethereal-0.1.2.tar", max compression
+gzip compressed data, was "ethereal-0.1.3.tar", max compression
```

## Comparing `ethereal-0.1.2.tar` & `ethereal-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.2/LICENSE
--rw-r--r--   0        0        0     1572 2023-04-17 07:26:20.322824 ethereal-0.1.2/README.md
--rw-r--r--   0        0        0     1308 2023-04-16 07:11:11.928618 ethereal-0.1.2/ethereal/__init__.py
--rw-r--r--   0        0        0     1402 2023-04-14 14:08:02.175740 ethereal-0.1.2/ethereal/app.py
--rw-r--r--   0        0        0      288 2023-04-14 18:53:08.549415 ethereal-0.1.2/ethereal/base.py
--rw-r--r--   0        0        0     6978 2023-04-16 06:36:31.316428 ethereal-0.1.2/ethereal/cache.py
--rw-r--r--   0        0        0      971 2023-04-14 18:52:21.303480 ethereal-0.1.2/ethereal/containers.py
--rw-r--r--   0        0        0     8806 2023-04-17 07:14:39.659777 ethereal-0.1.2/ethereal/contracts.py
--rw-r--r--   0        0        0     4652 2023-04-14 18:47:51.186401 ethereal-0.1.2/ethereal/etherscan.py
--rw-r--r--   0        0        0     3175 2023-04-14 14:31:35.858070 ethereal-0.1.2/ethereal/facade.py
--rw-r--r--   0        0        0     1439 2023-04-14 18:59:17.941096 ethereal-0.1.2/ethereal/networks.py
--rw-r--r--   0        0        0      586 2023-04-17 18:10:06.564404 ethereal-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2350 2023-04-17 18:10:17.874991 ethereal-0.1.2/setup.py
--rw-r--r--   0        0        0     2167 2023-04-17 18:10:17.875191 ethereal-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1573 2023-04-17 18:13:33.206391 ethereal-0.1.3/README.md
+-rw-r--r--   0        0        0     1308 2023-04-16 07:11:11.928618 ethereal-0.1.3/ethereal/__init__.py
+-rw-r--r--   0        0        0     1402 2023-04-14 14:08:02.175740 ethereal-0.1.3/ethereal/app.py
+-rw-r--r--   0        0        0      288 2023-04-14 18:53:08.549415 ethereal-0.1.3/ethereal/base.py
+-rw-r--r--   0        0        0     6978 2023-04-16 06:36:31.316428 ethereal-0.1.3/ethereal/cache.py
+-rw-r--r--   0        0        0      971 2023-04-14 18:52:21.303480 ethereal-0.1.3/ethereal/containers.py
+-rw-r--r--   0        0        0     8806 2023-04-17 07:14:39.659777 ethereal-0.1.3/ethereal/contracts.py
+-rw-r--r--   0        0        0     4652 2023-04-14 18:47:51.186401 ethereal-0.1.3/ethereal/etherscan.py
+-rw-r--r--   0        0        0     3175 2023-04-14 14:31:35.858070 ethereal-0.1.3/ethereal/facade.py
+-rw-r--r--   0        0        0     1439 2023-04-14 18:59:17.941096 ethereal-0.1.3/ethereal/networks.py
+-rw-r--r--   0        0        0      586 2023-04-17 18:13:46.291533 ethereal-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2351 2023-04-17 18:13:47.726799 ethereal-0.1.3/setup.py
+-rw-r--r--   0        0        0     2168 2023-04-17 18:13:47.726999 ethereal-0.1.3/PKG-INFO
```

### Comparing `ethereal-0.1.2/LICENSE` & `ethereal-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/README.md` & `ethereal-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Ethereal cat](./docs/images/ethereal_cat.png)
+![Ethereal logo](./docs/images/ethereal_cat.png)
 
 ## Ethereal
 
 [![docs](https://readthedocs.org/projects/ethereal/badge/?version=latest)](https://ethereal.readthedocs.io/en/latest/?badge=latest)
 
 Ethereal is a lightweight wrapper around the [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) class that simplifies
 working with Ethereum smart contracts.
```

### Comparing `ethereal-0.1.2/ethereal/__init__.py` & `ethereal-0.1.3/ethereal/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/ethereal/app.py` & `ethereal-0.1.3/ethereal/app.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/ethereal/cache.py` & `ethereal-0.1.3/ethereal/cache.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/ethereal/containers.py` & `ethereal-0.1.3/ethereal/containers.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/ethereal/contracts.py` & `ethereal-0.1.3/ethereal/contracts.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/ethereal/etherscan.py` & `ethereal-0.1.3/ethereal/etherscan.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/ethereal/facade.py` & `ethereal-0.1.3/ethereal/facade.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/ethereal/networks.py` & `ethereal-0.1.3/ethereal/networks.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.2/pyproject.toml` & `ethereal-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ethereal"
-version = "0.1.2"
+version = "0.1.3"
 description = "Ergonomic python tooling for web3"
 authors = ["Alex Euler <0xalexeuler@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ethereal-0.1.2/setup.py` & `ethereal-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'click>=8.1.3,<9.0.0',
  'dependency-injector>=4.41.0,<5.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'web3>=6.1.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'ethereal',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Ergonomic python tooling for web3',
-    'long_description': '![Ethereal cat](./docs/images/ethereal_cat.png)\n\n## Ethereal\n\n[![docs](https://readthedocs.org/projects/ethereal/badge/?version=latest)](https://ethereal.readthedocs.io/en/latest/?badge=latest)\n\nEthereal is a lightweight wrapper around the [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) class that simplifies\nworking with Ethereum smart contracts.\n\nTo use it, simply create a regular [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) instance and write `w3 = Ethereal(w3)`.\nThen, you can use w3 as usual, but with additional methods\naccessible under the `e` property.\n\nFor example, you can call `w3.e.get_abi("0x...")` or\n`w3.e.list_events("0x...", "Mint", "2023-01-01", "2023-02-14")`.\n\nFor more available methods, please refer to the :class:`ethereal.facade.EtherealFacade` class.\n\n### Example\n\n```python\n\n        from web3.auto import w3\n        from ethereal import Ethereal\n        from ethereal import load_provider_from_uri\n\n        # If WEB3_PROVIDER_URI env is not set, uncomment the lines below\n        # w3 = Web3(load_provider_from_uri("https://alchemy.com/..."))\n\n        w3 = Ethereal(w3)\n\n        ADDRESS = "0xB0B195aEFA3650A6908f15CdaC7D92F8a5791B0B"\n        print(w3.e.list_events(ADDRESS))\n        # Lists event signatures for the contract at ADDRESS\n\n        events = w3.e.get_events(ADDRESS, "Transfer", "2023-01-01", "2023-02-14")\n        # Gets all Transfer events for the contract at ADDRESS between 2023-01-01 and 2023-02-14\n        print(events[:10])\n```\n\n### Install\n\n```\npip install ethereal\n```\n',
+    'long_description': '![Ethereal logo](./docs/images/ethereal_cat.png)\n\n## Ethereal\n\n[![docs](https://readthedocs.org/projects/ethereal/badge/?version=latest)](https://ethereal.readthedocs.io/en/latest/?badge=latest)\n\nEthereal is a lightweight wrapper around the [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) class that simplifies\nworking with Ethereum smart contracts.\n\nTo use it, simply create a regular [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) instance and write `w3 = Ethereal(w3)`.\nThen, you can use w3 as usual, but with additional methods\naccessible under the `e` property.\n\nFor example, you can call `w3.e.get_abi("0x...")` or\n`w3.e.list_events("0x...", "Mint", "2023-01-01", "2023-02-14")`.\n\nFor more available methods, please refer to the :class:`ethereal.facade.EtherealFacade` class.\n\n### Example\n\n```python\n\n        from web3.auto import w3\n        from ethereal import Ethereal\n        from ethereal import load_provider_from_uri\n\n        # If WEB3_PROVIDER_URI env is not set, uncomment the lines below\n        # w3 = Web3(load_provider_from_uri("https://alchemy.com/..."))\n\n        w3 = Ethereal(w3)\n\n        ADDRESS = "0xB0B195aEFA3650A6908f15CdaC7D92F8a5791B0B"\n        print(w3.e.list_events(ADDRESS))\n        # Lists event signatures for the contract at ADDRESS\n\n        events = w3.e.get_events(ADDRESS, "Transfer", "2023-01-01", "2023-02-14")\n        # Gets all Transfer events for the contract at ADDRESS between 2023-01-01 and 2023-02-14\n        print(events[:10])\n```\n\n### Install\n\n```\npip install ethereal\n```\n',
     'author': 'Alex Euler',
     'author_email': '0xalexeuler@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `ethereal-0.1.2/PKG-INFO` & `ethereal-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereal
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ergonomic python tooling for web3
 License: MIT
 Author: Alex Euler
 Author-email: 0xalexeuler@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dependency-injector (>=4.41.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: web3 (>=6.1.0,<7.0.0)
 Description-Content-Type: text/markdown
 
-![Ethereal cat](./docs/images/ethereal_cat.png)
+![Ethereal logo](./docs/images/ethereal_cat.png)
 
 ## Ethereal
 
 [![docs](https://readthedocs.org/projects/ethereal/badge/?version=latest)](https://ethereal.readthedocs.io/en/latest/?badge=latest)
 
 Ethereal is a lightweight wrapper around the [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) class that simplifies
 working with Ethereum smart contracts.
```

