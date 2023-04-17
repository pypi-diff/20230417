# Comparing `tmp/planetmint_driver_python-0.17.0.tar.gz` & `tmp/planetmint_driver_python-0.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint_driver_python-0.17.0.tar", max compression
+gzip compressed data, was "planetmint_driver_python-0.18.2.tar", max compression
```

## Comparing `planetmint_driver_python-0.17.0.tar` & `planetmint_driver_python-0.18.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-01-31 15:39:55.122280 planetmint_driver_python-0.17.0/LICENSE
--rw-r--r--   0        0        0     7680 2023-01-31 15:39:55.122280 planetmint_driver_python-0.17.0/README.rst
--rw-r--r--   0        0        0      279 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/__init__.py
--rw-r--r--   0        0        0     4638 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/connection.py
--rw-r--r--   0        0        0      877 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/crypto.py
--rw-r--r--   0        0        0    18176 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/driver.py
--rw-r--r--   0        0        0     2108 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/exceptions.py
--rw-r--r--   0        0        0     2871 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/helper.py
--rw-r--r--   0        0        0    13616 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/offchain.py
--rw-r--r--   0        0        0     2253 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/pool.py
--rw-r--r--   0        0        0     3034 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/transport.py
--rw-r--r--   0        0        0     2828 2023-01-31 15:39:55.126280 planetmint_driver_python-0.17.0/planetmint_driver/utils.py
--rw-r--r--   0        0        0     1165 2023-01-31 15:39:55.130280 planetmint_driver_python-0.17.0/pyproject.toml
--rw-r--r--   0        0        0     8737 1970-01-01 00:00:00.000000 planetmint_driver_python-0.17.0/setup.py
--rw-r--r--   0        0        0     8546 1970-01-01 00:00:00.000000 planetmint_driver_python-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-17 14:28:10.371199 planetmint_driver_python-0.18.2/LICENSE
+-rw-r--r--   0        0        0     7659 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/README.rst
+-rw-r--r--   0        0        0      279 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/planetmint_driver/__init__.py
+-rw-r--r--   0        0        0     4638 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/planetmint_driver/connection.py
+-rw-r--r--   0        0        0      877 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/planetmint_driver/crypto.py
+-rw-r--r--   0        0        0    18148 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/planetmint_driver/driver.py
+-rw-r--r--   0        0        0     2108 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/planetmint_driver/exceptions.py
+-rw-r--r--   0        0        0    13818 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/planetmint_driver/offchain.py
+-rw-r--r--   0        0        0     2253 2023-04-17 14:28:10.375198 planetmint_driver_python-0.18.2/planetmint_driver/pool.py
+-rw-r--r--   0        0        0     3034 2023-04-17 14:28:10.379198 planetmint_driver_python-0.18.2/planetmint_driver/transport.py
+-rw-r--r--   0        0        0     2828 2023-04-17 14:28:10.379198 planetmint_driver_python-0.18.2/planetmint_driver/utils.py
+-rw-r--r--   0        0        0     1164 2023-04-17 14:28:10.379198 planetmint_driver_python-0.18.2/pyproject.toml
+-rw-r--r--   0        0        0     8525 1970-01-01 00:00:00.000000 planetmint_driver_python-0.18.2/PKG-INFO
```

### Comparing `planetmint_driver_python-0.17.0/LICENSE` & `planetmint_driver_python-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint_driver_python-0.17.0/README.rst` & `planetmint_driver_python-0.18.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 .. image:: https://img.shields.io/codecov/c/github/planetmint/planetmint-driver/master.svg
     :target: https://codecov.io/github/planetmint/planetmint-driver?branch=master
 
 
 Planetmint Python Driver
 ==========================
 
-* Free software: Apache Software License 2.0
+* Free software: AGPLv3
 * Check our `Documentation`_
 
 .. contents:: Table of Contents
 
 
 Features
 --------
```

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/connection.py` & `planetmint_driver_python-0.18.2/planetmint_driver/connection.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/crypto.py` & `planetmint_driver_python-0.18.2/planetmint_driver/crypto.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/driver.py` & `planetmint_driver_python-0.18.2/planetmint_driver/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
             method="POST",
             path=self.path,
             json=transaction,
             params={"mode": "commit"},
             headers=headers,
         )
 
-    def retrieve(self, txid, headers=None):
+    def retrieve(self, txid):
         """Retrieves the transaction with the given id.
 
         Args:
             txid (str): Id of the transaction to retrieve.
             headers (dict): Optional headers to pass to the request.
 
         Returns:
@@ -460,15 +460,15 @@
             method="GET",
             path=self.path,
             params={"transaction_id": txid},
             headers=headers,
         )
         return block_list if block_list else None
 
-    def retrieve(self, block_height, headers=None):
+    def retrieve(self, block_height):
         """Retrieves the block with the given ``block_height``.
 
         Args:
             block_height (str): height of the block to retrieve.
             headers (dict): Optional headers to pass to the request.
 
         Returns:
```

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/exceptions.py` & `planetmint_driver_python-0.18.2/planetmint_driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/offchain.py` & `planetmint_driver_python-0.18.2/planetmint_driver/offchain.py`

 * *Files 5% similar despite different names*

```diff
@@ -283,16 +283,21 @@
     if not isinstance(inputs, (list, tuple)):
         inputs = (inputs,)
     if not isinstance(recipients, (list, tuple)):
         recipients = [([recipients], 1)]
 
     # NOTE: Needed for the time being. See
     # https://github.com/planetmint/planetmint/issues/797
-    if isinstance(recipients, tuple):
-        recipients = [(list(recipients), 1)]
+    elif isinstance(recipients, tuple):
+        if len(recipients) == 1:  # format (pubkey)
+            recipients = [([recipients[0]], 1)]
+        elif len(recipients) == 2:  # format (pubkey, amount)
+            recipients = [recipients]
+    elif isinstance(recipients, list):
+        recipients = recipients
 
     fulfillments = [
         Input(
             _fulfillment_from_details(input_["fulfillment"]),
             input_["owners_before"],
             fulfills=TransactionLink(
                 txid=input_["fulfills"]["transaction_id"],
@@ -307,32 +312,32 @@
         recipients,
         asset_ids=assets,
         metadata=metadata,
     )
     return transaction.to_dict()
 
 
-def prepare_compose_transaction(*, inputs: list, assets: list, recipients, metadata=None):
+def prepare_compose_transaction(*, inputs: list, assets: list, recipients):
     if not isinstance(inputs, (list, tuple)):
         inputs = (inputs,)
     if not isinstance(assets, (list, tuple)):
         assets = [assets]
 
     compose_tx = Compose.generate(inputs, recipients, assets)
     return compose_tx.to_dict()
 
 
-def prepare_decompose_transaction(*, inputs: list, assets: list, recipients: list, metadata=None):
+def prepare_decompose_transaction(*, inputs: list, assets: list, recipients: list):
     if not isinstance(inputs, (list, tuple)):
         inputs = (inputs,)
     if not isinstance(assets, (list, tuple)):
         assets = [assets]
 
-    compose_tx = Decompose.generate(inputs, recipients, assets)
-    return compose_tx
+    decompose_tx = Decompose.generate(inputs, recipients, assets)
+    return decompose_tx
 
 
 def fulfill_transaction(transaction, *, private_keys):
     """Fulfills the given transaction.
 
     Args:
         transaction (dict): The transaction to be fulfilled.
```

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/pool.py` & `planetmint_driver_python-0.18.2/planetmint_driver/pool.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/transport.py` & `planetmint_driver_python-0.18.2/planetmint_driver/transport.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver_python-0.17.0/planetmint_driver/utils.py` & `planetmint_driver_python-0.18.2/planetmint_driver/utils.py`

 * *Files identical despite different names*

### Comparing `planetmint_driver_python-0.17.0/pyproject.toml` & `planetmint_driver_python-0.18.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "planetmint-driver-python"
-version = "0.17.0"
+version = "0.18.2"
 description = "Python driver for Planetmint"
 authors = ["Your Name <you@example.com>"]
 license = "AGPLv3-or-later"
 readme = "README.rst"
 packages = [{include = "planetmint_driver"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-planetmint-transactions = "^0.6.0"
+planetmint-transactions = "^0.8.0"
 python-rapidjson = "^1.9"
 python-rapidjson-schema = "^0.1.1"
 pysha3 = "^1.0.2"
 requests = "^2.28.2"
 planetmint-ipld = "^0.0.3"
 sphinx-press-theme = "0.8.0"
 wheel = "^0.38.1"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
+black = "^23.1.0"
 coverage = "^7.1.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-env = "^0.8.1"
 pytest-sugar = "^0.9.6"
 pytest-xdist = "^3.1.0"
 responses = "^0.22.0"
```

### Comparing `planetmint_driver_python-0.17.0/setup.py` & `planetmint_driver_python-0.18.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,212 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: planetmint-driver-python
+Version: 0.18.2
+Summary: Python driver for Planetmint
+License: AGPLv3-or-later
+Author: Your Name
+Author-email: you@example.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: planetmint-ipld (>=0.0.3,<0.0.4)
+Requires-Dist: planetmint-transactions (>=0.8.0,<0.9.0)
+Requires-Dist: pysha3 (>=1.0.2,<2.0.0)
+Requires-Dist: python-rapidjson (>=1.9,<2.0)
+Requires-Dist: python-rapidjson-schema (>=0.1.1,<0.2.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: sphinx-press-theme (==0.8.0)
+Requires-Dist: wheel (>=0.38.1,<0.39.0)
+Description-Content-Type: text/x-rst
+
+
+.. Copyright Planetmint GmbH and Planetmint contributors
+   SPDX-License-Identifier: (Apache-2.0 AND CC-BY-4.0)
+   Code is Apache-2.0 and docs are CC-BY-4.0
+
+.. image:: https://badges.gitter.im/planetmint/planetmint-driver.svg
+   :alt: Join the chat at https://gitter.im/planetmint/planetmint-driver
+   :target: https://gitter.im/planetmint/planetmint-driver?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+
+
+.. image:: https://badge.fury.io/py/planetmint-driver.svg
+    :target: https://badge.fury.io/py/planetmint-driver
+
+.. image:: https://app.travis-ci.com/planetmint/planetmint-driver.svg?branch=main
+    :target: https://app.travis-ci.com/planetmint/planetmint-driver
+
+.. image:: https://img.shields.io/codecov/c/github/planetmint/planetmint-driver/master.svg
+    :target: https://codecov.io/github/planetmint/planetmint-driver?branch=master
+
+
+Planetmint Python Driver
+==========================
+
+* Free software: AGPLv3
+* Check our `Documentation`_
+
+.. contents:: Table of Contents
+
+
+Features
+--------
+
+* Support for preparing, fulfilling, and sending transactions to a Planetmint
+  node.
+* Retrieval of transactions by id.
+
+Install
+----------
+
+The instructions below were tested on Ubuntu 16.04 LTS. They should also work on other Linux distributions and on macOS. The driver might work on Windows as well, but we do not guarantee it. We recommend to set up (e.g. via Docker on Windows) an Ubuntu VM there.
+
+We recommend you use a virtual environment to install and update to the latest stable version using `pip` (or `pip3`):
+
+.. code-block:: text
+
+    pip install -U planetmint-driver
+
+That will install the latest *stable* Planetmint Python Driver. If you want to install an Alpha, Beta or RC version of the Python Driver, use something like:
+
+.. code-block:: text
+
+    pip install -U planetmint_driver==0.11.1
+
+The above command will install version 0.11.1. You can find a list of all versions in `the release history page on PyPI <https://pypi.org/project/planetmint-driver/#history>`_.
+
+More information on how to install the driver can be found in the `Quickstart`_
+
+Planetmint Documentation
+------------------------------------
+* `Planetmint Server Quickstart`_
+* `The Hitchhiker's Guide to Planetmint`_
+* `HTTP API Reference`_
+* `All Planetmint Documentation`_
+
+Usage
+----------
+Example: Create a divisible asset for Alice who issues 10 token to Bob so that he can use her Game Boy.
+Afterwards Bob spends 3 of these tokens.
+
+If you want to send a transaction you need to `Determine the Planetmint Root URL`_.
+
+.. code-block:: python
+
+    # import Planetmint and create an object
+    from planetmint_driver import Planetmint
+    bdb_root_url = 'https://example.com:9984'
+    bdb = Planetmint(bdb_root_url)
+
+    # generate a keypair
+    from planetmint_driver.crypto import generate_keypair
+    alice, bob = generate_keypair(), generate_keypair()
+
+    # create a digital asset for Alice
+    game_boy_token = {
+        'data': {
+            'token_for': {
+                'game_boy': {
+                    'serial_number': 'LR35902'
+                }
+            },
+            'description': 'Time share token. Each token equals one hour of usage.',
+        },
+    }
+
+    # prepare the transaction with the digital asset and issue 10 tokens for Bob
+    prepared_token_tx = bdb.transactions.prepare(
+        operation='CREATE',
+        signers=alice.public_key,
+        recipients=[([bob.public_key], 10)],
+        asset=game_boy_token)
+
+    # fulfill and send the transaction
+    fulfilled_token_tx = bdb.transactions.fulfill(
+        prepared_token_tx,
+        private_keys=alice.private_key)
+    bdb.transactions.send_commit(fulfilled_token_tx)
+
+    # Use the tokens
+    # create the output and inout for the transaction
+    transfer_asset = {'id': fulfilled_token_tx['id']}
+    output_index = 0
+    output = fulfilled_token_tx['outputs'][output_index]
+    transfer_input = {'fulfillment': output['condition']['details'],
+                      'fulfills': {'output_index': output_index,
+                                   'transaction_id': transfer_asset['id']},
+                      'owners_before': output['public_keys']}
+
+    # prepare the transaction and use 3 tokens
+    prepared_transfer_tx = bdb.transactions.prepare(
+        operation='TRANSFER',
+        asset=transfer_asset,
+        inputs=transfer_input,
+        recipients=[([alice.public_key], 3), ([bob.public_key], 7)])
+
+    # fulfill and send the transaction
+    fulfilled_transfer_tx = bdb.transactions.fulfill(
+        prepared_transfer_tx,
+        private_keys=bob.private_key)
+    sent_transfer_tx = bdb.transactions.send_commit(fulfilled_transfer_tx)
+
+Compatibility Matrix
+--------------------
+
++-----------------------+---------------------------+
+| **Planetmint Server** | **Planetmint Driver**     |
++=======================+===========================+
+| ``>= 2.0.0b7``        | ``0.6.2``                 |
++-----------------------+---------------------------+
+| ``>= 2.0.0b7``        | ``0.6.1``                 |
++-----------------------+---------------------------+
+| ``>= 2.0.0b7``        | ``0.6.0``                 |
++-----------------------+---------------------------+
+| ``>= 2.0.0b5``        | ``0.5.3``                 |
++-----------------------+---------------------------+
+| ``>= 2.0.0b5``        | ``0.5.2``                 |
++-----------------------+---------------------------+
+| ``>= 2.0.0b5``        | ``0.5.1``                 |
++-----------------------+---------------------------+
+| ``>= 2.0.0b1``        | ``0.5.0``                 |
++-----------------------+---------------------------+
+| ``>= 2.0.0a3``        | ``0.5.0a4``               |
++-----------------------+---------------------------+
+| ``>= 2.0.0a2``        | ``0.5.0a2``               |
++-----------------------+---------------------------+
+| ``>= 2.0.0a1``        | ``0.5.0a1``               |
++-----------------------+---------------------------+
+| ``>= 1.0.0``          | ``0.4.x``                 |
++-----------------------+---------------------------+
+| ``== 1.0.0rc1``       | ``0.3.x``                 |
++-----------------------+---------------------------+
+| ``>= 0.9.1``          | ``0.2.x``                 |
++-----------------------+---------------------------+
+| ``>= 0.8.2``          | ``>= 0.1.3``              |
++-----------------------+---------------------------+
+
+`Although we do our best to keep the master branches in sync, there may be
+occasional delays.`
+
+License
+--------
+* `licenses`_ - open source & open content
+
+Credits
+-------
+
+This package was initially created using Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Many Planetmint developers have contributed since then.
+
+.. _Documentation: https://docs.planetmint.com/projects/py-driver/
+.. _pypi history: https://pypi.org/project/planetmint-driver/#history
+.. _Quickstart: https://docs.planetmint.com/projects/py-driver/en/latest/quickstart.html
+.. _Planetmint Server Quickstart: https://docs.planetmint.com/projects/server/en/latest/quickstart.html
+.. _The Hitchhiker's Guide to Planetmint: https://www.planetmint.com/developers/guide/
+.. _HTTP API Reference: https://docs.planetmint.com/projects/server/en/latest/http-client-server-api.html
+.. _All Planetmint Documentation: https://docs.planetmint.com/
+.. _Determine the Planetmint Root URL: https://docs.planetmint.com/projects/py-driver/en/latest/connect.html
+.. _licenses: https://github.com/planetmint/planetmint-driver/blob/master/LICENSES.md
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
-packages = \
-['planetmint_driver']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['planetmint-ipld>=0.0.3,<0.0.4',
- 'planetmint-transactions>=0.6.0,<0.7.0',
- 'pysha3>=1.0.2,<2.0.0',
- 'python-rapidjson-schema>=0.1.1,<0.2.0',
- 'python-rapidjson>=1.9,<2.0',
- 'requests>=2.28.2,<3.0.0',
- 'sphinx-press-theme==0.8.0',
- 'wheel>=0.38.1,<0.39.0']
-
-setup_kwargs = {
-    'name': 'planetmint-driver-python',
-    'version': '0.17.0',
-    'description': 'Python driver for Planetmint',
-    'long_description': "\n.. Copyright Planetmint GmbH and Planetmint contributors\n   SPDX-License-Identifier: (Apache-2.0 AND CC-BY-4.0)\n   Code is Apache-2.0 and docs are CC-BY-4.0\n\n.. image:: https://badges.gitter.im/planetmint/planetmint-driver.svg\n   :alt: Join the chat at https://gitter.im/planetmint/planetmint-driver\n   :target: https://gitter.im/planetmint/planetmint-driver?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge\n\n\n.. image:: https://badge.fury.io/py/planetmint-driver.svg\n    :target: https://badge.fury.io/py/planetmint-driver\n\n.. image:: https://app.travis-ci.com/planetmint/planetmint-driver.svg?branch=main\n    :target: https://app.travis-ci.com/planetmint/planetmint-driver\n\n.. image:: https://img.shields.io/codecov/c/github/planetmint/planetmint-driver/master.svg\n    :target: https://codecov.io/github/planetmint/planetmint-driver?branch=master\n\n\nPlanetmint Python Driver\n==========================\n\n* Free software: Apache Software License 2.0\n* Check our `Documentation`_\n\n.. contents:: Table of Contents\n\n\nFeatures\n--------\n\n* Support for preparing, fulfilling, and sending transactions to a Planetmint\n  node.\n* Retrieval of transactions by id.\n\nInstall\n----------\n\nThe instructions below were tested on Ubuntu 16.04 LTS. They should also work on other Linux distributions and on macOS. The driver might work on Windows as well, but we do not guarantee it. We recommend to set up (e.g. via Docker on Windows) an Ubuntu VM there.\n\nWe recommend you use a virtual environment to install and update to the latest stable version using `pip` (or `pip3`):\n\n.. code-block:: text\n\n    pip install -U planetmint-driver\n\nThat will install the latest *stable* Planetmint Python Driver. If you want to install an Alpha, Beta or RC version of the Python Driver, use something like:\n\n.. code-block:: text\n\n    pip install -U planetmint_driver==0.11.1\n\nThe above command will install version 0.11.1. You can find a list of all versions in `the release history page on PyPI <https://pypi.org/project/planetmint-driver/#history>`_.\n\nMore information on how to install the driver can be found in the `Quickstart`_\n\nPlanetmint Documentation\n------------------------------------\n* `Planetmint Server Quickstart`_\n* `The Hitchhiker's Guide to Planetmint`_\n* `HTTP API Reference`_\n* `All Planetmint Documentation`_\n\nUsage\n----------\nExample: Create a divisible asset for Alice who issues 10 token to Bob so that he can use her Game Boy.\nAfterwards Bob spends 3 of these tokens.\n\nIf you want to send a transaction you need to `Determine the Planetmint Root URL`_.\n\n.. code-block:: python\n\n    # import Planetmint and create an object\n    from planetmint_driver import Planetmint\n    bdb_root_url = 'https://example.com:9984'\n    bdb = Planetmint(bdb_root_url)\n\n    # generate a keypair\n    from planetmint_driver.crypto import generate_keypair\n    alice, bob = generate_keypair(), generate_keypair()\n\n    # create a digital asset for Alice\n    game_boy_token = {\n        'data': {\n            'token_for': {\n                'game_boy': {\n                    'serial_number': 'LR35902'\n                }\n            },\n            'description': 'Time share token. Each token equals one hour of usage.',\n        },\n    }\n\n    # prepare the transaction with the digital asset and issue 10 tokens for Bob\n    prepared_token_tx = bdb.transactions.prepare(\n        operation='CREATE',\n        signers=alice.public_key,\n        recipients=[([bob.public_key], 10)],\n        asset=game_boy_token)\n\n    # fulfill and send the transaction\n    fulfilled_token_tx = bdb.transactions.fulfill(\n        prepared_token_tx,\n        private_keys=alice.private_key)\n    bdb.transactions.send_commit(fulfilled_token_tx)\n\n    # Use the tokens\n    # create the output and inout for the transaction\n    transfer_asset = {'id': fulfilled_token_tx['id']}\n    output_index = 0\n    output = fulfilled_token_tx['outputs'][output_index]\n    transfer_input = {'fulfillment': output['condition']['details'],\n                      'fulfills': {'output_index': output_index,\n                                   'transaction_id': transfer_asset['id']},\n                      'owners_before': output['public_keys']}\n\n    # prepare the transaction and use 3 tokens\n    prepared_transfer_tx = bdb.transactions.prepare(\n        operation='TRANSFER',\n        asset=transfer_asset,\n        inputs=transfer_input,\n        recipients=[([alice.public_key], 3), ([bob.public_key], 7)])\n\n    # fulfill and send the transaction\n    fulfilled_transfer_tx = bdb.transactions.fulfill(\n        prepared_transfer_tx,\n        private_keys=bob.private_key)\n    sent_transfer_tx = bdb.transactions.send_commit(fulfilled_transfer_tx)\n\nCompatibility Matrix\n--------------------\n\n+-----------------------+---------------------------+\n| **Planetmint Server** | **Planetmint Driver**     |\n+=======================+===========================+\n| ``>= 2.0.0b7``        | ``0.6.2``                 |\n+-----------------------+---------------------------+\n| ``>= 2.0.0b7``        | ``0.6.1``                 |\n+-----------------------+---------------------------+\n| ``>= 2.0.0b7``        | ``0.6.0``                 |\n+-----------------------+---------------------------+\n| ``>= 2.0.0b5``        | ``0.5.3``                 |\n+-----------------------+---------------------------+\n| ``>= 2.0.0b5``        | ``0.5.2``                 |\n+-----------------------+---------------------------+\n| ``>= 2.0.0b5``        | ``0.5.1``                 |\n+-----------------------+---------------------------+\n| ``>= 2.0.0b1``        | ``0.5.0``                 |\n+-----------------------+---------------------------+\n| ``>= 2.0.0a3``        | ``0.5.0a4``               |\n+-----------------------+---------------------------+\n| ``>= 2.0.0a2``        | ``0.5.0a2``               |\n+-----------------------+---------------------------+\n| ``>= 2.0.0a1``        | ``0.5.0a1``               |\n+-----------------------+---------------------------+\n| ``>= 1.0.0``          | ``0.4.x``                 |\n+-----------------------+---------------------------+\n| ``== 1.0.0rc1``       | ``0.3.x``                 |\n+-----------------------+---------------------------+\n| ``>= 0.9.1``          | ``0.2.x``                 |\n+-----------------------+---------------------------+\n| ``>= 0.8.2``          | ``>= 0.1.3``              |\n+-----------------------+---------------------------+\n\n`Although we do our best to keep the master branches in sync, there may be\noccasional delays.`\n\nLicense\n--------\n* `licenses`_ - open source & open content\n\nCredits\n-------\n\nThis package was initially created using Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template. Many Planetmint developers have contributed since then.\n\n.. _Documentation: https://docs.planetmint.com/projects/py-driver/\n.. _pypi history: https://pypi.org/project/planetmint-driver/#history\n.. _Quickstart: https://docs.planetmint.com/projects/py-driver/en/latest/quickstart.html\n.. _Planetmint Server Quickstart: https://docs.planetmint.com/projects/server/en/latest/quickstart.html\n.. _The Hitchhiker's Guide to Planetmint: https://www.planetmint.com/developers/guide/\n.. _HTTP API Reference: https://docs.planetmint.com/projects/server/en/latest/http-client-server-api.html\n.. _All Planetmint Documentation: https://docs.planetmint.com/\n.. _Determine the Planetmint Root URL: https://docs.planetmint.com/projects/py-driver/en/latest/connect.html\n.. _licenses: https://github.com/planetmint/planetmint-driver/blob/master/LICENSES.md\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage\n",
-    'author': 'Your Name',
-    'author_email': 'you@example.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

