# Comparing `tmp/xbridge_cli-0.3.0.tar.gz` & `tmp/xbridge_cli-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xbridge_cli-0.3.0.tar", max compression
+gzip compressed data, was "xbridge_cli-1.0.0b0.tar", max compression
```

## Comparing `xbridge_cli-0.3.0.tar` & `xbridge_cli-1.0.0b0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1076 2022-06-02 18:55:19.569628 xbridge_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0      941 2023-04-12 21:26:10.799452 xbridge_cli-0.3.0/README.md
--rw-r--r--   0        0        0     1350 2023-04-17 21:02:02.743330 xbridge_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-12 21:26:10.827320 xbridge_cli-0.3.0/xbridge_cli/__init__.py
--rw-r--r--   0        0        0      642 2023-04-12 21:26:10.829434 xbridge_cli-0.3.0/xbridge_cli/bridge/__init__.py
--rw-r--r--   0        0        0    18431 2023-04-17 20:46:34.649920 xbridge_cli-0.3.0/xbridge_cli/bridge/build.py
--rw-r--r--   0        0        0     6260 2023-04-17 20:43:50.122911 xbridge_cli-0.3.0/xbridge_cli/bridge/create_account.py
--rw-r--r--   0        0        0     6477 2023-04-12 21:26:10.832975 xbridge_cli-0.3.0/xbridge_cli/bridge/register.py
--rw-r--r--   0        0        0     8049 2023-04-17 20:43:50.124018 xbridge_cli-0.3.0/xbridge_cli/bridge/transfer.py
--rw-r--r--   0        0        0      500 2023-04-12 21:26:10.834687 xbridge_cli-0.3.0/xbridge_cli/exceptions.py
--rw-r--r--   0        0        0      680 2023-04-17 20:41:09.822418 xbridge_cli-0.3.0/xbridge_cli/main.py
--rw-r--r--   0        0        0       20 2023-04-12 21:26:10.837291 xbridge_cli-0.3.0/xbridge_cli/misc/__init__.py
--rw-r--r--   0        0        0     6174 2023-04-12 21:26:10.838312 xbridge_cli-0.3.0/xbridge_cli/misc/explorer.html
--rw-r--r--   0        0        0      406 2023-04-12 21:26:10.839082 xbridge_cli-0.3.0/xbridge_cli/misc/explorer.py
--rw-r--r--   0        0        0     2094 2023-04-17 20:41:09.824441 xbridge_cli-0.3.0/xbridge_cli/misc/fund.py
--rw-r--r--   0        0        0     1700 2023-04-12 21:26:10.841233 xbridge_cli-0.3.0/xbridge_cli/misc/trust.py
--rw-r--r--   0        0        0     1109 2023-04-12 21:26:10.841776 xbridge_cli-0.3.0/xbridge_cli/server/__init__.py
--rw-r--r--   0        0        0      614 2023-04-12 21:26:10.842765 xbridge_cli-0.3.0/xbridge_cli/server/config/__init__.py
--rw-r--r--   0        0        0    18276 2023-04-17 20:43:50.125098 xbridge_cli-0.3.0/xbridge_cli/server/config/config.py
--rw-r--r--   0        0        0     2253 2023-04-12 21:26:10.845523 xbridge_cli-0.3.0/xbridge_cli/server/config/ports.py
--rw-r--r--   0        0        0     1360 2023-04-12 21:26:10.847508 xbridge_cli-0.3.0/xbridge_cli/server/config/templates/bootstrap.jinja
--rw-r--r--   0        0        0     1806 2023-04-12 21:26:10.848692 xbridge_cli-0.3.0/xbridge_cli/server/config/templates/rippled.jinja
--rw-r--r--   0        0        0     1518 2023-04-12 21:26:10.849839 xbridge_cli-0.3.0/xbridge_cli/server/config/templates/witness.jinja
--rw-r--r--   0        0        0     1403 2023-04-12 21:26:10.851113 xbridge_cli-0.3.0/xbridge_cli/server/list.py
--rw-r--r--   0        0        0      721 2023-04-12 21:26:10.851992 xbridge_cli-0.3.0/xbridge_cli/server/print.py
--rw-r--r--   0        0        0     2338 2023-04-12 21:26:10.852613 xbridge_cli-0.3.0/xbridge_cli/server/request.py
--rw-r--r--   0        0        0     2156 2023-04-12 21:26:10.853921 xbridge_cli-0.3.0/xbridge_cli/server/restart.py
--rw-r--r--   0        0        0    12440 2023-04-17 20:46:34.651131 xbridge_cli-0.3.0/xbridge_cli/server/start.py
--rw-r--r--   0        0        0     2834 2023-04-12 21:26:10.855973 xbridge_cli-0.3.0/xbridge_cli/server/stop.py
--rw-r--r--   0        0        0     1341 2023-04-12 21:26:10.856994 xbridge_cli-0.3.0/xbridge_cli/utils/__init__.py
--rw-r--r--   0        0        0     4741 2023-04-12 21:26:10.857889 xbridge_cli-0.3.0/xbridge_cli/utils/attestations.py
--rw-r--r--   0        0        0      539 2023-04-12 21:26:10.858776 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/__init__.py
--rw-r--r--   0        0        0     2399 2023-04-12 21:26:10.859431 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/bridge_config.py
--rw-r--r--   0        0        0     1189 2023-04-12 21:26:10.860319 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/chain_config.py
--rw-r--r--   0        0        0     5813 2023-04-12 21:26:10.861145 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_file.py
--rw-r--r--   0        0        0      543 2023-04-12 21:26:10.862021 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_item.py
--rw-r--r--   0        0        0      702 2023-04-12 21:26:10.862611 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/server_config.py
--rw-r--r--   0        0        0      840 2023-04-12 21:26:10.864534 xbridge_cli-0.3.0/xbridge_cli/utils/config_file/witness_config.py
--rw-r--r--   0        0        0     6603 2023-04-12 21:26:10.865568 xbridge_cli-0.3.0/xbridge_cli/utils/config_utils.py
--rw-r--r--   0        0        0      665 2023-04-12 21:26:10.867038 xbridge_cli-0.3.0/xbridge_cli/utils/misc.py
--rw-r--r--   0        0        0     5073 2023-04-12 21:26:10.868191 xbridge_cli-0.3.0/xbridge_cli/utils/rippled_config.py
--rw-r--r--   0        0        0     2596 2023-04-12 21:26:10.869342 xbridge_cli-0.3.0/xbridge_cli/utils/transaction.py
--rw-r--r--   0        0        0     1075 2023-04-12 21:26:10.871219 xbridge_cli-0.3.0/xbridge_cli/utils/types.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 xbridge_cli-0.3.0/setup.py
--rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 xbridge_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-06-02 18:55:19.569628 xbridge_cli-1.0.0b0/LICENSE
+-rw-r--r--   0        0        0      941 2023-02-17 16:27:31.784221 xbridge_cli-1.0.0b0/README.md
+-rw-r--r--   0        0        0     1353 2023-02-17 16:27:32.088526 xbridge_cli-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-02-17 16:27:31.912010 xbridge_cli-1.0.0b0/xbridge_cli/__init__.py
+-rw-r--r--   0        0        0      642 2023-02-17 16:27:31.713474 xbridge_cli-1.0.0b0/xbridge_cli/bridge/__init__.py
+-rw-r--r--   0        0        0     5615 2023-02-17 16:27:31.913459 xbridge_cli-1.0.0b0/xbridge_cli/bridge/create_account.py
+-rw-r--r--   0        0        0     6475 2023-02-17 16:27:31.916485 xbridge_cli-1.0.0b0/xbridge_cli/bridge/register.py
+-rw-r--r--   0        0        0    15658 2023-02-17 16:27:31.919054 xbridge_cli-1.0.0b0/xbridge_cli/bridge/setup.py
+-rw-r--r--   0        0        0     7197 2023-02-17 16:27:31.920431 xbridge_cli-1.0.0b0/xbridge_cli/bridge/transfer.py
+-rw-r--r--   0        0        0      500 2023-02-17 16:27:31.923863 xbridge_cli-1.0.0b0/xbridge_cli/exceptions.py
+-rw-r--r--   0        0        0      680 2023-02-17 16:27:32.000058 xbridge_cli-1.0.0b0/xbridge_cli/main.py
+-rw-r--r--   0        0        0       20 2023-02-17 16:27:31.721004 xbridge_cli-1.0.0b0/xbridge_cli/misc/__init__.py
+-rw-r--r--   0        0        0     6174 2023-02-17 16:27:32.003166 xbridge_cli-1.0.0b0/xbridge_cli/misc/explorer.html
+-rw-r--r--   0        0        0      406 2023-02-17 16:27:31.723240 xbridge_cli-1.0.0b0/xbridge_cli/misc/explorer.py
+-rw-r--r--   0        0        0     1917 2023-02-17 16:27:31.927438 xbridge_cli-1.0.0b0/xbridge_cli/misc/fund.py
+-rw-r--r--   0        0        0     1700 2023-02-17 16:27:31.929799 xbridge_cli-1.0.0b0/xbridge_cli/misc/trust.py
+-rw-r--r--   0        0        0     1109 2023-02-17 16:27:31.725525 xbridge_cli-1.0.0b0/xbridge_cli/server/__init__.py
+-rw-r--r--   0        0        0      614 2023-02-17 16:27:31.726178 xbridge_cli-1.0.0b0/xbridge_cli/server/config/__init__.py
+-rw-r--r--   0        0        0    17498 2023-02-17 16:27:31.726821 xbridge_cli-1.0.0b0/xbridge_cli/server/config/config.py
+-rw-r--r--   0        0        0     2253 2023-02-17 16:27:31.727571 xbridge_cli-1.0.0b0/xbridge_cli/server/config/ports.py
+-rw-r--r--   0        0        0     1326 2023-02-17 16:27:31.728941 xbridge_cli-1.0.0b0/xbridge_cli/server/config/templates/bootstrap.jinja
+-rw-r--r--   0        0        0     1806 2023-02-17 16:27:31.729768 xbridge_cli-1.0.0b0/xbridge_cli/server/config/templates/rippled.jinja
+-rw-r--r--   0        0        0     1502 2023-02-17 16:27:31.730390 xbridge_cli-1.0.0b0/xbridge_cli/server/config/templates/witness.jinja
+-rw-r--r--   0        0        0     1403 2023-02-17 16:27:31.731163 xbridge_cli-1.0.0b0/xbridge_cli/server/list.py
+-rw-r--r--   0        0        0      721 2023-02-17 16:27:31.731835 xbridge_cli-1.0.0b0/xbridge_cli/server/print.py
+-rw-r--r--   0        0        0     2338 2023-02-17 16:27:31.931251 xbridge_cli-1.0.0b0/xbridge_cli/server/request.py
+-rw-r--r--   0        0        0     2156 2023-02-17 16:27:31.932637 xbridge_cli-1.0.0b0/xbridge_cli/server/restart.py
+-rw-r--r--   0        0        0    12243 2023-02-17 16:27:31.934025 xbridge_cli-1.0.0b0/xbridge_cli/server/start.py
+-rw-r--r--   0        0        0     2834 2023-02-17 16:27:31.935333 xbridge_cli-1.0.0b0/xbridge_cli/server/stop.py
+-rw-r--r--   0        0        0     1341 2023-02-17 16:27:32.004733 xbridge_cli-1.0.0b0/xbridge_cli/utils/__init__.py
+-rw-r--r--   0        0        0     4741 2023-02-17 16:27:31.938044 xbridge_cli-1.0.0b0/xbridge_cli/utils/attestations.py
+-rw-r--r--   0        0        0      539 2023-02-17 16:27:32.006981 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/__init__.py
+-rw-r--r--   0        0        0     2399 2023-02-17 16:27:31.740314 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/bridge_config.py
+-rw-r--r--   0        0        0     1189 2023-02-17 16:27:31.741050 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/chain_config.py
+-rw-r--r--   0        0        0     5813 2023-02-17 16:27:31.942548 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/config_file.py
+-rw-r--r--   0        0        0      543 2023-02-17 16:27:31.742581 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/config_item.py
+-rw-r--r--   0        0        0      702 2023-02-17 16:27:31.743164 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/server_config.py
+-rw-r--r--   0        0        0      840 2023-02-17 16:27:31.743918 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/witness_config.py
+-rw-r--r--   0        0        0     6603 2023-02-17 16:27:31.944258 xbridge_cli-1.0.0b0/xbridge_cli/utils/config_utils.py
+-rw-r--r--   0        0        0      157 2023-02-17 16:27:31.745900 xbridge_cli-1.0.0b0/xbridge_cli/utils/misc.py
+-rw-r--r--   0        0        0     5073 2023-02-17 16:27:31.746700 xbridge_cli-1.0.0b0/xbridge_cli/utils/rippled_config.py
+-rw-r--r--   0        0        0     2556 2023-02-17 16:27:31.747611 xbridge_cli-1.0.0b0/xbridge_cli/utils/transaction.py
+-rw-r--r--   0        0        0     1075 2023-02-17 16:27:31.748389 xbridge_cli-1.0.0b0/xbridge_cli/utils/types.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 xbridge_cli-1.0.0b0/setup.py
+-rw-r--r--   0        0        0     2009 1970-01-01 00:00:00.000000 xbridge_cli-1.0.0b0/PKG-INFO
```

### Comparing `xbridge_cli-0.3.0/LICENSE` & `xbridge_cli-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/README.md` & `xbridge_cli-1.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/pyproject.toml` & `xbridge_cli-1.0.0b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xbridge-cli"
-version = "0.3.0"
+version = "1.0.0b0"
 description = "A CLI that helps you set up an XRPL-XRPL bridge."
 readme = "README.md"
 repository = "https://github.com/xpring-eng/xbridge-cli"
 authors = ["Mayukha Vadari <mvadari@ripple.com>"]
 keywords = [
   "xrp",
   "xrpl",
@@ -26,23 +26,23 @@
 click = "^8.1.3"
 tabulate = ">=0.8.9,<0.10.0"
 httpx = ">=0.18.1,<0.24.0"
 websockets = "^10.3"
 Jinja2 = "^3.1.2"
 psutil = "^5.9.2"
 docker = "^6.0.0"
-xrpl-py = "1.9.0b1"
+xrpl-py = "1.8.0b1"
 pycryptodome = "^3.17"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^5.0.4"
-black = "^23.3"
+black = "^22.12"
 flake8-black = "^0.3.6"
 flake8-docstrings = "^1.5.0"
-mypy = "^1"
+mypy = "^0"
 isort = "^5.11.4"
 flake8-isort = "^6.0.0"
 flake8-annotations = "^2.5.0"
 flake8-absolute-import = "^1.0"
 darglint = "^1.5.8"
 types-tabulate = "^0.9.0"
 coverage = "^7.0.3"
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/__init__.py` & `xbridge_cli-1.0.0b0/xbridge_cli/bridge/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """CLI command for starting a bridge."""
 
 import click
 
-from xbridge_cli.bridge.build import setup_bridge
 from xbridge_cli.bridge.create_account import create_xchain_account
 from xbridge_cli.bridge.register import register_bridge
+from xbridge_cli.bridge.setup import setup_bridge
 from xbridge_cli.bridge.transfer import send_transfer
 
 
 @click.group()
 def bridge() -> None:
     """Subcommand for all commands dealing with the bridge itself."""
     pass
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/build.py` & `xbridge_cli-1.0.0b0/xbridge_cli/bridge/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,104 @@
 """CLI command for setting up a bridge."""
 
 import json
 import os
 from pprint import pformat
-from typing import List, Optional
+from typing import Any, Dict, List, Literal, Optional, TypedDict, Union, cast
 
 import click
 from xrpl import CryptoAlgorithm
 from xrpl.account import does_account_exist
 from xrpl.clients import JsonRpcClient
+from xrpl.core.binarycodec import encode
+from xrpl.core.keypairs import sign
 from xrpl.models import (
     XRP,
-    AccountInfo,
-    AccountLines,
-    AccountObjects,
-    AccountObjectType,
     AccountSet,
     AccountSetFlag,
+    Amount,
     Currency,
     IssuedCurrency,
-    Payment,
     ServerState,
     SignerEntry,
     SignerListSet,
     Transaction,
     TrustSet,
+    XChainAccountCreateCommit,
+    XChainAddAccountCreateAttestation,
     XChainBridge,
     XChainCreateBridge,
 )
+from xrpl.models.transactions.transaction import transaction_json_to_binary_codec_form
 from xrpl.wallet import Wallet
 
 from xbridge_cli.exceptions import XBridgeCLIException
 from xbridge_cli.utils import (
     BridgeData,
     CryptoAlgorithmChoice,
     add_bridge,
     check_bridge_exists,
     submit_tx,
 )
-from xbridge_cli.utils.misc import is_standalone_network
 
-_GENESIS_ACCOUNT = "rHb9CJAWyB4rj91VRWn96DkukG4bwdtyTh"
-_GENESIS_SEED = "snoPBrXtMeMyMHUVTgbuqAfg1SUTb"
-_GENESIS_WALLET = Wallet(_GENESIS_SEED, 0)
 
-LSF_DISABLE_MASTER = 0x00100000
+class _UnsignedAttestation(TypedDict):
+    xchain_bridge: XChainBridge
+    other_chain_source: str
+    amount: Amount
+    attestation_reward_account: str
+    was_locking_chain_send: Union[Literal[0], Literal[1]]
+    xchain_account_create_count: str
+    destination: str
+    signature_reward: Amount
+
+
+class _SignedAttestation(_UnsignedAttestation):
+    public_key: str
+    signature: str
+
+
+_ATTESTATION_ENCODE_ORDER = [
+    ("other_chain_source", 6),
+    ("amount", 2),
+    ("signature_reward", 4),
+    ("attestation_reward_account", 6),
+    ("was_locking_chain_send", 0),
+    ("xchain_account_create_count", 4),
+    ("destination", 4),
+]
+
+
+def _sign_attestation(
+    attestation: _UnsignedAttestation,
+    bridge: XChainBridge,
+    wallet: Wallet,
+) -> _SignedAttestation:
+    # TODO: use this instead once it's been implemented
+    # attestation_xrpl = transaction_json_to_binary_codec_form(attestation)
+    # encoded_obj = encode(attestation_xrpl)
+    bridge_dict: Dict[str, Any] = {"xchain_bridge": bridge.to_dict()}
+    encoded_obj = encode(transaction_json_to_binary_codec_form(bridge_dict))[4:]
+    for key, prefix in _ATTESTATION_ENCODE_ORDER:
+        value = attestation[key]  # type: ignore  # Hard to type
+        if key == "was_locking_chain_send":
+            encoded_obj += "0" + str(value)
+        else:
+            xrpl_attestation = transaction_json_to_binary_codec_form({key: value})
+            encoded_obj += encode(xrpl_attestation)[prefix:]
+    signature = sign(bytes.fromhex(encoded_obj), wallet.private_key)
+    signed_attestation: _SignedAttestation = cast(
+        _SignedAttestation,
+        {
+            **attestation,
+            "signature": signature,
+            "public_key": wallet.public_key,
+        },
+    )
+    return signed_attestation
 
 
 @click.command(name="build")
 @click.option(
     "--name",
     required=True,
     prompt=True,
@@ -59,68 +109,54 @@
     envvar="XCHAIN_CONFIG_DIR",
     required=True,
     prompt=True,
     type=click.Path(exists=True),
     help="The filepath to the bootstrap config file.",
 )
 @click.option(
-    "--signature-reward",
+    "--signature_reward",
     default="100",
     help="The reward for witnesses providing a signature.",
 )
 @click.option(
-    "--funding-seed",
+    "--funding_seed",
     help=(
         "The master key of an account on the locking chain that can fund accounts on "
         "the issuing chain. This is only needed for an XRP-XRP bridge."
     ),
 )
 @click.option(
-    "--funding-algorithm",
+    "--funding_algorithm",
     type=CryptoAlgorithmChoice,
     help="The algorithm used to generate the keypair from the funding seed.",
 )
 @click.option(
     "--close-ledgers/--no-close-ledgers",
     "close_ledgers",
     default=True,
     help=(
         "Whether to close ledgers manually (via `ledger_accept`) or wait for ledgers "
         "to close automatically. A standalone node requires ledgers to be closed; an "
         "external network does not support ledger closing."
     ),
 )
 @click.option(
-    "--fund-locking",
-    "fund_locking",
-    is_flag=True,
-    help="Whether to fund the locking chain accounts from the funding seed.",
-)
-@click.option(
     "-v",
     "--verbose",
     help="Whether or not to print more verbose information. Also supports `-vv`.",
     count=True,
 )
-@click.option(
-    "-s",
-    "--silent",
-    is_flag=True,
-    help="Whether or not to print no information. Cannot be used with -v.",
-)
 def setup_bridge(
     name: str,
     bootstrap: str,
     signature_reward: str,
     funding_seed: Optional[str] = None,
     funding_algorithm: Optional[str] = None,
     close_ledgers: bool = True,
-    fund_locking: bool = False,
     verbose: int = 0,
-    silent: bool = False,
 ) -> None:
     """
     Keep track of a bridge between a locking chain and issuing chain.
     \f
 
     Args:
         name: The name of the bridge (used for differentiation purposes).
@@ -130,52 +166,34 @@
             accounts on the issuing chain. This is only needed for an XRP-XRP bridge.
             If not provided, uses the genesis seed.
         funding_algorithm: The algorithm used to generate the keypair from the funding
             seed.
         close_ledgers: Whether to close ledgers manually (via `ledger_accept`) or wait
             for ledgers to close automatically. A standalone node requires ledgers to
             be closed; an external network does not support ledger closing.
-        fund_locking: Whether to fund the locking chain accounts from the funding seed.
         verbose: Whether or not to print more verbose information. Add more v's for
             more verbosity.
-        silent: Whether or not to print no information. Cannot be used with `-v`.
 
     Raises:
         XBridgeCLIException: If an account on the locking chain doesn't exist
             (namely, the witness reward or submit accounts or the door account).
     """  # noqa: D301
-    if silent and verbose > 0:
-        raise XBridgeCLIException("Cannot have verbose and silent flags.")
-    verbosity = 0 if silent else 1 + verbose
     # check name
     if check_bridge_exists(name):
         raise XBridgeCLIException(f"Bridge named {name} already exists.")
 
     if bootstrap == os.getenv("XCHAIN_CONFIG_DIR"):
         bootstrap = os.path.join(bootstrap, "bridge_bootstrap.json")
 
     with open(bootstrap) as f:
         bootstrap_config = json.load(f)
 
     bootstrap_locking = bootstrap_config["LockingChain"]
     bootstrap_issuing = bootstrap_config["IssuingChain"]
 
-    locking_endpoint = bootstrap_locking["Endpoint"]
-    locking_url = f"http://{locking_endpoint['Host']}:{locking_endpoint['JsonRPCPort']}"
-    locking_client = JsonRpcClient(locking_url)
-
-    issuing_endpoint = bootstrap_issuing["Endpoint"]
-    issuing_url = f"http://{issuing_endpoint['Host']}:{issuing_endpoint['JsonRPCPort']}"
-    issuing_client = JsonRpcClient(issuing_url)
-
-    if not is_standalone_network(locking_client) and close_ledgers:
-        raise XBridgeCLIException(
-            "Must use `--no-close-ledgers` on a non-standalone node."
-        )
-
     locking_door = bootstrap_locking["DoorAccount"]["Address"]
     locking_issue = bootstrap_locking["BridgeIssue"]
     issuing_door = bootstrap_issuing["DoorAccount"]["Address"]
     issuing_issue = bootstrap_issuing["BridgeIssue"]
 
     if locking_issue == {"currency": "XRP"}:
         locking_chain_issue: Currency = XRP()
@@ -191,91 +209,75 @@
         locking_chain_issue=locking_chain_issue,
         issuing_chain_door=issuing_door,
         issuing_chain_issue=issuing_chain_issue,
     )
 
     is_xrp_bridge = locking_chain_issue == XRP()
 
-    # get min create account amount values
-    if is_xrp_bridge:
-        server_state1 = locking_client.request(ServerState())
-        min_create1 = server_state1.result["state"]["validated_ledger"]["reserve_base"]
-        server_state2 = issuing_client.request(ServerState())
-        min_create2 = server_state2.result["state"]["validated_ledger"]["reserve_base"]
-    else:
-        min_create1 = None
-        min_create2 = None
-    min_create1_rippled = str(min_create1) if min_create1 is not None else None
-    min_create2_rippled = str(min_create2) if min_create2 is not None else None
-
     if funding_seed is None:
-        if is_xrp_bridge and funding_seed is None:
+        if bridge_obj.issuing_chain_issue == XRP() and funding_seed is None:
             if close_ledgers:
                 funding_seed = "snoPBrXtMeMyMHUVTgbuqAfg1SUTb"
             else:
                 raise XBridgeCLIException(
                     "Must include `funding_seed` for external XRP-XRP bridge."
                 )
-    funding_wallet_algo = (
-        CryptoAlgorithm(funding_algorithm) if funding_algorithm else None
-    )
-    funding_wallet = (
-        Wallet(funding_seed, 0, algorithm=funding_wallet_algo) if funding_seed else None
-    )
+
+    locking_endpoint = bootstrap_locking["Endpoint"]
+    locking_url = f"http://{locking_endpoint['IP']}:{locking_endpoint['JsonRPCPort']}"
+    locking_client = JsonRpcClient(locking_url)
+
+    issuing_endpoint = bootstrap_issuing["Endpoint"]
+    issuing_url = f"http://{issuing_endpoint['IP']}:{issuing_endpoint['JsonRPCPort']}"
+    issuing_client = JsonRpcClient(issuing_url)
 
     accounts_locking_check = set(
         [locking_door]
         + bootstrap_locking["WitnessRewardAccounts"]
         + bootstrap_locking["WitnessSubmitAccounts"]
     )
     accounts_issuing_check = set(
         bootstrap_issuing["WitnessRewardAccounts"]
         + bootstrap_issuing["WitnessSubmitAccounts"]
     )
 
-    funding_txs: List[Transaction] = []
-
     # check locking chain for accounts that should already exist
     for account in accounts_locking_check:
         if not does_account_exist(account, locking_client):
-            if is_xrp_bridge and fund_locking:
-                assert funding_wallet is not None  # for type reasons
-                funding_txs.append(
-                    Payment(
-                        account=funding_wallet.classic_address,
-                        destination=account,
-                        amount=str(min_create1 * 2),
-                    )
-                )
-            else:
-                raise XBridgeCLIException(
-                    f"Account {account} does not exist on the locking chain."
-                )
-    if len(funding_txs) > 0:
-        assert funding_wallet is not None  # for type reasons
-        submit_tx(funding_txs, locking_client, funding_wallet, verbose, close_ledgers)
-
+            raise XBridgeCLIException(
+                f"Account {account} does not exist on the locking chain."
+            )
     # make sure issuing door account exists
     if not does_account_exist(issuing_door, issuing_client):
         raise XBridgeCLIException(
             f"Issuing chain door {issuing_door} does not exist on the locking chain."
         )
-    if not is_xrp_bridge:
+    if bridge_obj.issuing_chain_issue != XRP():
         # if a bridge is an XRP bridge, then the accounts need to be created via the
         # bridge (the bridge that doesn't exist yet)
         # so we only check if accounts already exist on the issuing chain for IOU
         # bridges
         for account in accounts_issuing_check:
             if not does_account_exist(account, issuing_client):
                 raise XBridgeCLIException(
                     f"Account {account} does not exist on the issuing chain."
                 )
 
+    # get min create account amount values
+    if is_xrp_bridge:
+        server_state1 = locking_client.request(ServerState())
+        min_create1 = server_state1.result["state"]["validated_ledger"]["reserve_base"]
+        server_state2 = issuing_client.request(ServerState())
+        min_create2 = server_state2.result["state"]["validated_ledger"]["reserve_base"]
+    else:
+        min_create1 = None
+        min_create2 = None
+
     # set up signer entries for multisign on the door accounts
-    signer_entries: List[SignerEntry] = []
+    signer_entries = []
     for witness_entry in bootstrap_config["Witnesses"]["SignerList"]:
         signer_entries.append(
             SignerEntry(
                 account=witness_entry["Account"], signer_weight=witness_entry["Weight"]
             )
         )
 
@@ -288,234 +290,165 @@
     issuing_door_seed_algo = bootstrap_issuing["DoorAccount"]["KeyType"]
     issuing_door_wallet = Wallet(
         issuing_door_seed, 0, algorithm=CryptoAlgorithm(issuing_door_seed_algo)
     )
 
     ###################################################################################
     # set up locking chain
-    locking_txs: List[Transaction] = []
+    transactions: List[Transaction] = []
 
     # create the trustline (if IOU)
-    if not is_xrp_bridge:
+    if bridge_obj.locking_chain_issue != XRP():
         assert isinstance(bridge_obj.locking_chain_issue, IssuedCurrency)
-
-        # check if the trustline already exists
-        account_lines = locking_client.request(AccountLines(locking_door)).result[
-            "lines"
-        ]
-        filtered_lines = [
-            line
-            for line in account_lines
-            if line["account"] == bridge_obj.locking_chain_issue.issuer
-            and line["currency"] == bridge_obj.locking_chain_issue.currency
-        ]
-        # TODO: perhaps add a check to make sure the trustline is large enough
-        if len(filtered_lines) == 0:  # no trustline set yet
-            locking_txs.append(
-                TrustSet(
-                    account=locking_door,
-                    limit_amount=bridge_obj.locking_chain_issue.to_amount("1000000000"),
-                )
+        transactions.append(
+            TrustSet(
+                account=locking_door,
+                limit_amount=bridge_obj.locking_chain_issue.to_amount("1000000000"),
             )
+        )
 
     # create the bridge
-
-    # check if the bridge already exists
-    locking_bridge_exists = False
-    locking_door_objs = locking_client.request(
-        AccountObjects(account=locking_door, type=AccountObjectType.BRIDGE)
-    ).result["account_objects"]
-    if len(locking_door_objs) > 0:
-        assert (
-            len(locking_door_objs) == 1
-        ), "Cannot have multiple bridges on one account"
-        if XChainBridge.from_xrpl(locking_door_objs[0]["XChainBridge"]) == bridge_obj:
-            locking_bridge_exists = True
-        else:
-            raise XBridgeCLIException(
-                f"Locking chain door account {locking_door} already has a bridge."
-            )
-
-    # build if not
-    if not locking_bridge_exists:
-        locking_txs.append(
-            XChainCreateBridge(
-                account=locking_door,
-                xchain_bridge=bridge_obj,
-                signature_reward=signature_reward,
-                min_account_create_amount=min_create2_rippled,
-            )
+    min_create2_rippled = str(min_create2) if min_create2 is not None else None
+    transactions.append(
+        XChainCreateBridge(
+            account=locking_door,
+            xchain_bridge=bridge_obj,
+            signature_reward=signature_reward,
+            min_account_create_amount=min_create2_rippled,
         )
+    )
 
     # set up multisign on the door account
-
-    # check if multisign exists
-    locking_signer_list_exists = False
-    locking_account_info = locking_client.request(
-        AccountInfo(account=locking_door, signer_lists=True)
-    ).result["account_data"]
-    locking_signer_list = locking_account_info["signer_lists"]
-    if len(locking_signer_list) > 0:
-        assert len(locking_signer_list) == 1
-        locking_signer_entries = locking_signer_list[0]["SignerEntries"]
-        if all(
-            SignerEntry.from_xrpl(entry) in signer_entries
-            for entry in locking_signer_entries
-        ):
-            if len(locking_signer_entries) == len(signer_entries):
-                locking_signer_list_exists = True
-
-    # set up if not
-    if not locking_signer_list_exists:
-        locking_txs.append(
-            SignerListSet(
-                account=locking_door,
-                signer_quorum=max(1, len(signer_entries) - 1),
-                signer_entries=signer_entries,
-            )
+    transactions.append(
+        SignerListSet(
+            account=locking_door,
+            signer_quorum=max(1, len(signer_entries) - 1),
+            signer_entries=signer_entries,
         )
+    )
 
     # disable the master key
-    if not locking_account_info["Flags"] & LSF_DISABLE_MASTER:
-        locking_txs.append(
-            AccountSet(account=locking_door, set_flag=AccountSetFlag.ASF_DISABLE_MASTER)
-        )
+    transactions.append(
+        AccountSet(account=locking_door, set_flag=AccountSetFlag.ASF_DISABLE_MASTER)
+    )
 
     # submit transactions
     submit_tx(
-        locking_txs,
+        transactions,
         locking_client,
         locking_door_wallet,
-        verbosity,
+        verbose,
         close_ledgers,
     )
 
     ###################################################################################
     # set up issuing chain
 
-    if is_xrp_bridge:
-        # we need to create the witness reward + submission accounts
+    # create the bridge
+    min_create1_rippled = str(min_create1) if min_create2 is not None else None
+    create_tx2 = XChainCreateBridge(
+        account=issuing_door,
+        xchain_bridge=bridge_obj,
+        signature_reward=signature_reward,
+        min_account_create_amount=min_create1_rippled,
+    )
+    submit_tx(create_tx2, issuing_client, issuing_door_wallet, verbose, close_ledgers)
+
+    if bridge_obj.issuing_chain_issue == XRP():
+        # we need to create the witness reward + submission accounts via the bridge
+
+        # helper function for submitting the attestations
+        def _submit_attestation(
+            attestation: _SignedAttestation,
+        ) -> None:
+            attestation_tx = XChainAddAccountCreateAttestation.from_dict(
+                {
+                    **attestation,
+                    "account": issuing_door,
+                    "attestation_signer_account": issuing_door,
+                }
+            )
+            submit_tx(
+                attestation_tx,
+                issuing_client,
+                issuing_door_wallet,
+                verbose,
+                close_ledgers,
+            )
 
         assert funding_seed is not None  # for typing purposes - checked earlier
         funding_wallet_algo = (
             CryptoAlgorithm(funding_algorithm) if funding_algorithm else None
         )
         funding_wallet = Wallet(funding_seed, 0, algorithm=funding_wallet_algo)
 
-        # TODO: add param to customize amount
         amount = str(min_create2 * 2)  # submit accounts need spare funds
-        total_amount = 0
+        count = 1
 
         # create the accounts
         acct_txs: List[Transaction] = []
-        # send the funds for the accounts on the issuing chain from the genesis account
+        # commit the funds for the account
         for account in accounts_issuing_check:
-            if not does_account_exist(account, issuing_client):
-                acct_txs.append(
-                    Payment(
-                        account=_GENESIS_ACCOUNT,
-                        destination=account,
-                        amount=amount,
-                    )
+            acct_txs.append(
+                XChainAccountCreateCommit(
+                    account=funding_wallet.classic_address,
+                    xchain_bridge=bridge_obj,
+                    signature_reward=signature_reward,
+                    destination=account,
+                    amount=amount,
                 )
-                total_amount += int(amount)
-        submit_tx(acct_txs, issuing_client, _GENESIS_WALLET, verbosity, close_ledgers)
-
-        # set up the attestations for the commit
-        if total_amount > 0:
-            door_payment = Payment(
-                account=funding_wallet.classic_address,
-                destination=locking_door,
-                amount=str(total_amount),
             )
-            submit_tx(
-                door_payment, locking_client, funding_wallet, verbosity, close_ledgers
-            )
-
-    issuing_txs: List[Transaction] = []
-
-    # create the bridge
+        submit_tx(acct_txs, locking_client, funding_wallet, verbose, close_ledgers)
 
-    # check if the bridge already exists
-    issuing_bridge_exists = False
-    issuing_door_objs = issuing_client.request(
-        AccountObjects(account=issuing_door, type=AccountObjectType.BRIDGE)
-    ).result["account_objects"]
-    if len(issuing_door_objs) > 0:
-        assert (
-            len(issuing_door_objs) == 1
-        ), "Cannot have multiple bridges on one account"
-        if XChainBridge.from_xrpl(issuing_door_objs[0]["XChainBridge"]) == bridge_obj:
-            issuing_bridge_exists = True
-        else:
-            raise XBridgeCLIException(
-                f"Issuing chain door account {issuing_door} already has a bridge."
-            )
-
-    # build if not
-    if not issuing_bridge_exists:
-        issuing_txs.append(
-            XChainCreateBridge(
-                account=issuing_door,
+        # set up the attestations for the commit
+        for account in accounts_issuing_check:
+            init_attestation = _UnsignedAttestation(
                 xchain_bridge=bridge_obj,
+                other_chain_source=funding_wallet.classic_address,
+                amount=amount,
+                attestation_reward_account=issuing_door,
+                destination=account,
                 signature_reward=signature_reward,
-                min_account_create_amount=min_create1_rippled,
+                was_locking_chain_send=1,
+                xchain_account_create_count=str(count),
             )
-        )
+            signed_attestation = _sign_attestation(
+                init_attestation, bridge_obj, issuing_door_wallet
+            )
+            _submit_attestation(signed_attestation)
+            count += 1
 
     # set up multisign on the door account
-
-    # check if multisign exists
-    issuing_signer_list_exists = False
-    issuing_account_info = issuing_client.request(
-        AccountInfo(account=issuing_door, signer_lists=True)
-    ).result["account_data"]
-    issuing_signer_list = issuing_account_info["signer_lists"]
-    if len(issuing_signer_list) > 0:
-        assert len(issuing_signer_list) == 1
-        issuing_signer_entries = issuing_signer_list[0]["SignerEntries"]
-        if all(
-            SignerEntry.from_xrpl(entry) in signer_entries
-            for entry in issuing_signer_entries
-        ):
-            if len(issuing_signer_entries) == len(signer_entries):
-                issuing_signer_list_exists = True
-
-    # set up if not
-    if not issuing_signer_list_exists:
-        issuing_txs.append(
-            SignerListSet(
-                account=issuing_door,
-                signer_quorum=max(1, len(signer_entries) - 1),
-                signer_entries=signer_entries,
-            )
-        )
+    signer_tx2 = SignerListSet(
+        account=issuing_door,
+        signer_quorum=max(1, len(signer_entries) - 1),
+        signer_entries=signer_entries,
+    )
 
     # disable the master key
-    if not issuing_account_info["Flags"] & LSF_DISABLE_MASTER:
-        issuing_txs.append(
-            AccountSet(account=issuing_door, set_flag=AccountSetFlag.ASF_DISABLE_MASTER)
-        )
+    disable_master_tx2 = AccountSet(
+        account=issuing_door, set_flag=AccountSetFlag.ASF_DISABLE_MASTER
+    )
 
     # submit transactions
     submit_tx(
-        issuing_txs,
+        [signer_tx2, disable_master_tx2],
         issuing_client,
         issuing_door_wallet,
-        verbosity,
+        verbose,
         close_ledgers,
     )
 
     # add bridge to CLI config
     bridge_data: BridgeData = {
         "name": name,
         "chains": (locking_url, issuing_url),
         "quorum": max(1, len(signer_entries) - 1),
         "door_accounts": (locking_door, issuing_door),
         "xchain_currencies": (locking_issue, issuing_issue),
         "signature_reward": signature_reward,
         "create_account_amounts": (str(min_create2), str(min_create1)),
     }
 
-    if verbosity > 1:
+    if verbose:
         click.echo(pformat(bridge_data))
     add_bridge(bridge_data)
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/create_account.py` & `xbridge_cli-1.0.0b0/xbridge_cli/bridge/create_account.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 from xbridge_cli.exceptions import XBridgeCLIException
 from xbridge_cli.utils import (
     CryptoAlgorithmChoice,
     get_config,
     submit_tx,
     wait_for_attestations,
 )
-from xbridge_cli.utils.misc import is_standalone_network
 
 
 @click.command(name="create-account")
 @click.option(
-    "--from-locking/--from-issuing",
+    "--from_locking/--from_issuing",
     "from_locking",
     required=True,
     prompt=True,
     help=(
         "Whether funding from the locking chain or the issuing chain. "
         "Defaults to the locking chain."
     ),
@@ -79,30 +78,23 @@
 )
 @click.option(
     "-v",
     "--verbose",
     help="Whether or not to print more verbose information. Also supports `-vv`.",
     count=True,
 )
-@click.option(
-    "-s",
-    "--silent",
-    is_flag=True,
-    help="Whether or not to print no information. Cannot be used with -v.",
-)
 def create_xchain_account(
     from_locking: bool,
     bridge: str,
     from_seed: str,
     to_account: str,
     algorithm: Optional[str] = None,
     amount: Optional[int] = None,
     close_ledgers: bool = True,
     verbose: int = 0,
-    silent: bool = False,
 ) -> None:
     """
     Create an account on the opposite chain via a cross-chain transfer.
     \f
 
     Args:
         from_locking: Whether funding from the locking chain or the issuing chain.
@@ -114,39 +106,30 @@
         amount: The amount with which to fund the account. Must be greater than the
             account reserve. Defaults to the account reserve.
         close_ledgers: Whether to close ledgers manually (via `ledger_accept`) or wait
             for ledgers to close automatically. A standalone node requires ledgers to
             be closed; an external network does not support ledger closing.
         verbose: Whether or not to print more verbose information. Add more v's for
             more verbosity.
-        silent: Whether or not to print no information. Cannot be used with `-v`.
 
     Raises:
         XBridgeCLIException: Min create account isn't set or amount is less than the
             minimum account reserve, or timeout on attestations.
         AttestationTimeoutException: If there is a timeout when waiting for
             attestations.
     """  # noqa: D301
-    if silent and verbose > 0:
-        raise XBridgeCLIException("Cannot have verbose and silent flags.")
-    verbosity = 0 if silent else 1 + verbose
     bridge_config = get_config().get_bridge(bridge)
     locking_client, issuing_client = bridge_config.get_clients()
     if from_locking:
         from_client = locking_client
         to_client = issuing_client
     else:
         from_client = issuing_client
         to_client = locking_client
 
-    if not is_standalone_network(locking_client) and close_ledgers:
-        raise XBridgeCLIException(
-            "Must use `--no-close-ledgers` on a non-standalone node."
-        )
-
     min_create_account_amount = bridge_config.create_account_amounts[
         0 if from_locking else 1
     ]
     if min_create_account_amount is None:
         raise XBridgeCLIException(
             "Cannot create a cross-chain account if the create account amount "
             "is not set."
@@ -170,30 +153,30 @@
     fund_tx = XChainAccountCreateCommit(
         account=from_wallet.classic_address,
         xchain_bridge=bridge_config.get_bridge(),
         signature_reward=bridge_config.signature_reward,
         destination=to_account,
         amount=create_amount,
     )
-    submit_tx(fund_tx, from_client, from_wallet, verbosity, close_ledgers)
+    submit_tx(fund_tx, from_client, from_wallet, verbose, close_ledgers)
 
     # wait for attestations
-    if verbosity > 0:
+    if verbose > 0:
         click.secho(
             f"Waiting for attestations from the witness servers on {to_client.url}...",
             fg="blue",
         )
 
     wait_for_attestations(
         False,
         bridge_config,
         to_client,
         from_wallet,
         to_account,
         create_amount,
         None,
         close_ledgers,
-        verbosity,
+        verbose,
     )
 
-    if verbosity > 1:
+    if verbose > 0:
         click.echo(pformat(to_client.request(AccountInfo(account=to_account)).result))
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/register.py` & `xbridge_cli-1.0.0b0/xbridge_cli/bridge/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         del signers["SignerListID"]
         del signers["Flags"]
     return signers1 == signers2
 
 
 def _get_bootstrap_chain_and_door(chain_json: Dict[str, Any]) -> Tuple[str, str]:
     endpoint = chain_json["Endpoint"]
-    chain = f"http://{endpoint['Host']}:{endpoint['JsonRPCPort']}"
+    chain = f"http://{endpoint['IP']}:{endpoint['JsonRPCPort']}"
     door = chain_json["DoorAccount"]["Address"]
     return chain, door
 
 
 @click.command(name="register")
 @click.option(
     "--name",
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/bridge/transfer.py` & `xbridge_cli-1.0.0b0/xbridge_cli/bridge/transfer.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,31 @@
     IssuedCurrency,
     Response,
     Transaction,
     Tx,
     XChainCommit,
     XChainCreateClaimID,
 )
-from xrpl.utils import xrp_to_drops
 from xrpl.wallet import Wallet
 
 from xbridge_cli.exceptions import XBridgeCLIException
 from xbridge_cli.utils import get_config, submit_tx, wait_for_attestations
-from xbridge_cli.utils.misc import is_standalone_network
+
+_ATTESTATION_TIME_LIMIT = 10  # in seconds
+_WAIT_STEP_LENGTH = 0.05
 
 
 def _submit_tx(
     tx: Transaction,
     client: JsonRpcClient,
     wallet: Wallet,
-    verbosity: int,
+    verbose: int,
     close_ledgers: bool,
 ) -> Response:
-    result = submit_tx(tx, client, wallet, verbosity, close_ledgers)[0]
+    result = submit_tx(tx, client, wallet, verbose, close_ledgers)[0]
     tx_result = (
         result.result.get("error")
         or result.result.get("engine_result")
         or result.result["meta"]["TransactionResult"]
     )
     if tx_result != "tesSUCCESS":
         raise XBridgeCLIException(
@@ -53,29 +54,25 @@
     "--bridge",
     required=True,
     prompt=True,
     type=str,
     help="The bridge to transfer across.",
 )
 @click.option(
-    "--from-locking/--from-issuing",
+    "--from_locking/--from_issuing",
     "from_locking",
     required=True,
     prompt=True,
     help=(
         "Whether funding from the locking chain or the issuing chain. "
         "Defaults to the locking chain."
     ),
 )
 @click.option(
-    "--amount",
-    required=True,
-    prompt=True,
-    type=float,
-    help="The amount to transfer.",
+    "--amount", required=True, prompt=True, type=str, help="The amount to transfer."
 )
 @click.option(
     "--from",
     "from_account",
     required=True,
     prompt=True,
     type=str,
@@ -102,99 +99,79 @@
 @click.option(
     "-v",
     "--verbose",
     count=True,
     help="Whether or not to print more verbose information. Supports `-vv`.",
 )
 @click.option(
-    "-s",
-    "--silent",
-    is_flag=True,
-    help="Whether or not to print no information. Cannot be used with -v.",
-)
-@click.option(
     "--tutorial",
     is_flag=True,
     help="Turn this flag on if you want to slow down and really understand each step.",
 )
 def send_transfer(
     bridge: str,
     from_locking: bool,
-    amount: int | float,
+    amount: str,
     from_account: str,
     to_account: str,
     close_ledgers: bool = True,
     verbose: int = 0,
-    silent: bool = False,
     tutorial: bool = False,
 ) -> None:
     """
     Set up a bridge between a locking chain and issuing chain.
     \f
 
     Args:
         bridge: The bridge to transfer across.
         from_locking: Whether funding from the locking chain or the issuing chain.
             Defaults to the locking chain.
-        amount: The amount to transfer (in XRP).
+        amount: The amount to transfer.
         from_account: The seed of the account to transfer from.
         to_account: The seed of the account to transfer to.
         close_ledgers: Whether to close ledgers manually (via `ledger_accept`) or wait
             for ledgers to close automatically. A standalone node requires ledgers to
             be closed; an external network does not support ledger closing.
         verbose: Whether or not to print more verbose information. Supports `-vv`.
-        silent: Whether or not to print no information. Cannot be used with `-v`.
         tutorial: Whether to slow down and explain each step.
 
     Raises:
         XBridgeCLIException: If there is an error with a transaction somewhere along
             the way.
         AttestationTimeoutException: If there is a timeout when waiting for
             attestations.
     """  # noqa: D301
-    if silent and verbose > 0:
-        raise XBridgeCLIException("Cannot have verbose and silent flags.")
-    if silent and tutorial:
-        raise XBridgeCLIException("Cannot have tutorial and silent flags.")
-
-    verbosity = 0 if silent else 1 + verbose
-    print_level = max(verbosity, 2 if tutorial else 0)
+    print_level = max(verbose, 2 if tutorial else 0)
     bridge_config = get_config().get_bridge(bridge)
     bridge_obj = bridge_config.get_bridge()
     locking_client, issuing_client = bridge_config.get_clients()
     if from_locking:
         src_client = locking_client
         dst_client = issuing_client
         from_issue = bridge_obj.locking_chain_issue
     else:
         src_client = issuing_client
         dst_client = locking_client
         from_issue = bridge_obj.issuing_chain_issue
 
-    if not is_standalone_network(locking_client) and close_ledgers:
-        raise XBridgeCLIException(
-            "Must use `--no-close-ledgers` on a non-standalone node."
-        )
-
     if isinstance(from_issue, IssuedCurrency):
         original_issue: Currency = from_issue
     else:
         original_issue = XRP()
-        amount = int(xrp_to_drops(amount))
 
     try:
         from_wallet = Wallet(from_account, 0)
-    except ValueError as error:
-        raise XBridgeCLIException(f"Invalid `from` seed: {from_account}") from error
+    except ValueError:
+        raise XBridgeCLIException(f"Invalid `from` seed: {from_account}")
     try:
         to_wallet = Wallet(to_account, 0)
-    except ValueError as error:
-        raise XBridgeCLIException(f"Invalid `to` seed: {to_account}") from error
+    except ValueError:
+        raise XBridgeCLIException(f"Invalid `to` seed: {to_account}")
 
-    transfer_amount = original_issue.to_amount(amount)  # type: ignore
+    transfer_amount = original_issue.to_amount(amount)
 
     # XChainSeqNumCreate
     if tutorial:
         click.pause(
             info=click.style(
                 "\nCreating a cross-chain claim ID on the destination chain...",
                 fg="blue",
@@ -259,9 +236,9 @@
         bridge_config,
         dst_client,
         from_wallet,
         to_wallet.classic_address,
         transfer_amount,
         xchain_claim_id,
         close_ledgers,
-        verbosity,
+        verbose,
     )
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/main.py` & `xbridge_cli-1.0.0b0/xbridge_cli/main.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/misc/explorer.html` & `xbridge_cli-1.0.0b0/xbridge_cli/misc/explorer.html`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/misc/fund.py` & `xbridge_cli-1.0.0b0/xbridge_cli/misc/fund.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,44 +9,42 @@
 from xrpl.wallet import Wallet
 
 from xbridge_cli.exceptions import XBridgeCLIException
 from xbridge_cli.utils import get_config, submit_tx
 
 
 @click.command(name="fund")
-@click.argument("chain", required=True, type=str)
+@click.argument(
+    "chain",
+    required=True,
+    type=str,
+)
 @click.argument(
     "accounts",
     required=True,
     type=str,
     nargs=-1,
 )
 @click.option(
-    "--amount", type=int, default=1000, help="The amount to fund each account (in XRP)."
-)
-@click.option(
     "-v",
     "--verbose",
     is_flag=True,
     help="Whether or not to print more verbose information.",
 )
-def fund_account(
-    chain: str, accounts: List[str], amount: int = 1000, verbose: bool = False
-) -> None:
+def fund_account(chain: str, accounts: List[str], verbose: bool = False) -> None:
     """
     Of the form `xbridge-cli fund CHAIN ACCOUNT1 [ACCOUNT2 ...].
 
     Fund an account from the genesis account. Only works on a normal standalone rippled
     node.
     \f
 
     Args:
         chain: The chain to fund an account on.
         accounts: The account(s) to fund.
-        amount: The amount to fund each account (in XRP).
         verbose: Whether or not to print more verbose information.
 
     Raises:
         XBridgeCLIException: If the chain is the issuing chain.
     """  # noqa: D301
     if chain == "issuing_chain":
         raise XBridgeCLIException(
@@ -59,14 +57,14 @@
     wallet = Wallet("snoPBrXtMeMyMHUVTgbuqAfg1SUTb", 0)
     payments: List[Transaction] = []
     for account in accounts:
         payments.append(
             Payment(
                 account=wallet.classic_address,
                 destination=account,
-                amount=xrp_to_drops(amount),
+                amount=xrp_to_drops(1000),
             )
         )
     submit_tx(payments, client, wallet)
     if verbose:
         for account in accounts:
             click.echo(pformat(client.request(AccountInfo(account=account)).result))
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/misc/trust.py` & `xbridge_cli-1.0.0b0/xbridge_cli/misc/trust.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/__init__.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/__init__.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/config.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/config/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,16 +106,15 @@
     )
 
     return locking_ports.ws_public_port, issuing_ports.ws_public_port
 
 
 @click.command(name="witness")
 @click.option(
-    "--config-dir",
-    "config_dir",
+    "--config_dir",
     required=True,
     prompt=True,
     help="The folder in which to store config files.",
 )
 @click.option(
     "--name",
     default="witness",
@@ -124,99 +123,89 @@
 @click.option(
     "--docker",
     "is_docker",
     is_flag=True,
     help="Whether the config files are for a docker setup.",
 )
 @click.option(
-    "--locking-port",
+    "--locking_port",
     "locking_chain_port",
     required=True,
     prompt=True,
     type=int,
     help="The port used by the locking chain.",
 )
 @click.option(
-    "--issuing-port",
+    "--issuing_port",
     "issuing_chain_port",
     required=True,
     prompt=True,
     type=int,
     help="The port used by the issuing chain.",
 )
 @click.option(
-    "--witness-port",
-    "witness_port",
+    "--witness_port",
     required=True,
     prompt=True,
     type=int,
     help="The port that will be used by the witness server.",
 )
 @click.option(
-    "--src-door",
-    "src_door",
+    "--src_door",
     required=True,
     prompt=True,
     help="The door account on the source chain.",
 )
 @click.option(
-    "--src-currency",
-    "src_currency",
+    "--src_currency",
     default="XRP",
     help=(
         "The currency on the source chain. Defaults to XRP. An issued currency is of "
         "the form `{{currency}}.{{issue}}`"
     ),
 )
 @click.option(
-    "--dst-door",
-    "dst_door",
+    "--dst_door",
     default="rHb9CJAWyB4rj91VRWn96DkukG4bwdtyTh",
     help="The door account on the destination chain. Defaults to the genesis account.",
 )
 @click.option(
-    "--dst-currency",
-    "dst_currency",
+    "--dst_currency",
     default="XRP",
     help=(
         "The currency on the destination chain. Defaults to XRP. An issued currency "
         "is of the form `{{currency}}.{{issue}}`"
     ),
 )
 @click.option(
-    "--locking-reward-seed",
-    "locking_reward_seed",
+    "--locking_reward_seed",
     required=True,
     prompt=True,
     help="The seed for the reward account for the witness on the locking chain.",
 )
 @click.option(
-    "--locking-reward-account",
-    "locking_reward_account",
+    "--locking_reward_account",
     required=True,
     prompt=True,
     help="The reward account for the witness on the locking chain.",
 )
 @click.option(
-    "--signing-seed",
-    "signing_seed",
+    "--signing_seed",
     required=True,
     prompt=True,
     help="The seed to use for signing attestations.",
 )
 @click.option(
-    "--issuing-reward-seed",
-    "issuing_reward_seed",
+    "--issuing_reward_seed",
     required=True,
     prompt=True,
     help="The seed for the reward account for the witness on the issuing chain.",
 )
 @click.option(
-    "--issuing-reward-account",
-    "issuing_reward_account",
+    "--issuing_reward_account",
     required=True,
     prompt=True,
     help="The reward account for the witness on the issuing chain.",
 )
 @click.option(
     "-v",
     "--verbose",
@@ -326,66 +315,64 @@
     "--directory",
     "config_dir",
     required=True,
     prompt=True,
     help="The folder in which to store the bridge bootstrap file.",
 )
 @click.option(
-    "--locking-seed",
+    "--locking_seed",
     "locking_seed",
     required=True,
     prompt=True,
     help="The seed of the locking chain door account.",
 )
 @click.option(
-    "--locking-algorithm",
-    "locking_algorithm",
+    "--locking_algorithm",
     type=CryptoAlgorithmChoice,
     help="The algorithm used to generate the keypair from the locking door's seed.",
 )
 @click.option(
-    "--locking-currency",
+    "--locking_currency",
     "locking_currency",
     default="XRP",
     help=(
         "The bridge's locking chain currency. Defaults to XRP. An issued currency is "
         "of the form `{{currency}}.{{issue}}`."
     ),
 )
 @click.option(
-    "--issuing-seed",
+    "--issuing_seed",
     "issuing_seed",
     default="snoPBrXtMeMyMHUVTgbuqAfg1SUTb",
     help="The seed of the issuing chain door account. Defaults to the genesis account.",
 )
 @click.option(
-    "--issuing-algorithm",
-    "issuing_algorithm",
+    "--issuing_algorithm",
     type=CryptoAlgorithmChoice,
     help="The algorithm used to generate the keypair from the issuing door's seed.",
 )
 @click.option(
-    "--issuing-currency",
+    "--issuing_currency",
     "issuing_currency",
     default="XRP",
     help=(
         "The bridge's issuing chain currency. Defaults to XRP. An issued currency is "
         "of the form `{{currency}}.{{issue}}`."
     ),
 )
 @click.option(
-    "--reward-account",
+    "--reward_account",
     "reward_accounts",
     required=True,
     prompt=True,
     multiple=True,
     help="The seed of the witness reward account.",
 )
 @click.option(
-    "--signing-account",
+    "--signing_account",
     "signing_accounts",
     required=True,
     prompt=True,
     multiple=True,
     help="The account the witness uses to sign attestations.",
 )
 @click.option(
@@ -422,22 +409,18 @@
             door seed.
         issuing_currency: The currency on the issuing chain.
         reward_accounts: The witness reward accounts (which need to be created).
         signing_accounts: The accounts the witness uses to sign attestations.
         verbose: Whether or not to print more verbose information.
     """  # noqa: D301
     locking_wallet_algo = (
-        CryptoAlgorithm(locking_algorithm)
-        if locking_algorithm
-        else CryptoAlgorithm.ED25519
+        CryptoAlgorithm(locking_algorithm) if locking_algorithm else None
     )
     issuing_wallet_algo = (
-        CryptoAlgorithm(issuing_algorithm)
-        if issuing_algorithm
-        else CryptoAlgorithm.ED25519
+        CryptoAlgorithm(issuing_algorithm) if issuing_algorithm else None
     )
     locking_door = Wallet(locking_seed, 0, algorithm=locking_wallet_algo)
     issuing_door = Wallet(issuing_seed, 0, algorithm=issuing_wallet_algo)
 
     assert (locking_currency == "XRP" and issuing_currency == "XRP") or (
         locking_currency != "XRP" and issuing_currency != "XRP"
     )
@@ -447,22 +430,20 @@
         assert issuing_issue["issuer"] == issuing_door.classic_address
 
     template_data = {
         "is_linux": platform == "linux" or platform == "linux2",
         "locking_node_port": 5005,
         "locking_door_account": locking_door.classic_address,
         "locking_door_seed": locking_door.seed,
-        "locking_door_algo": locking_wallet_algo.value,
         "locking_issue": repr(locking_issue).replace("'", '"'),
         "locking_reward_accounts": reward_accounts,
         "locking_submit_accounts": reward_accounts,
         "issuing_node_port": 5006,
         "issuing_door_account": issuing_door.classic_address,
         "issuing_door_seed": issuing_door.seed,
-        "issuing_door_algo": issuing_wallet_algo.value,
         "issuing_issue": repr(issuing_issue).replace("'", '"'),
         "issuing_reward_accounts": reward_accounts,
         "issuing_submit_accounts": reward_accounts,
         "signing_accounts": signing_accounts,
     }
     if verbose:
         click.echo(pformat(template_data))
@@ -472,25 +453,23 @@
         template_data,
         os.path.join(config_dir, "bridge_bootstrap.json"),
     )
 
 
 @click.command(name="all")
 @click.option(
-    "--config-dir",
-    "config_dir",
+    "--config_dir",
     envvar="XCHAIN_CONFIG_DIR",
     required=True,
     prompt=True,
     type=click.Path(),
     help="The folder in which to store config files.",
 )
 @click.option(
-    "--num-witnesses",
-    "num_witnesses",
+    "--num_witnesses",
     default=5,
     type=int,
     help="The number of witness configs to generate. Defaults to 5.",
 )
 @click.option(
     "--currency",
     default="XRP",
@@ -530,29 +509,27 @@
         currency: The currency that is being transferred across the bridge.
         is_docker: Whether the config files are for a docker setup.
         verbose: Whether or not to print more verbose information.
     """
     # TODO: add support for external networks
     abs_config_dir = os.path.abspath(config_dir)
 
-    locking_port, issuing_port = _generate_rippled_configs(abs_config_dir, is_docker)
-    locking_door = Wallet.create(crypto_algorithm=CryptoAlgorithm.SECP256K1)
+    mc_port, sc_port = _generate_rippled_configs(abs_config_dir, is_docker)
+    src_door = Wallet.create(CryptoAlgorithm.SECP256K1)
 
-    if currency == "XRP":
-        locking_currency = "XRP"
-        issuing_currency = "XRP"
-        issuing_door = Wallet(_GENESIS_SEED, 0, algorithm=CryptoAlgorithm.SECP256K1)
-        issuing_algorithm = "secp256k1"
-    else:
+    if currency != "XRP":
         assert currency.count(".") == 1
         currency_code, _issuer = currency.split(".")
-        locking_currency = currency
-        issuing_door = Wallet.create()
-        issuing_algorithm = "ed25519"
-        issuing_currency = f"{currency_code}.{issuing_door.classic_address}"
+        src_currency = currency
+        dst_door = Wallet.create()
+        dst_currency = f"{currency_code}.{dst_door.classic_address}"
+    else:
+        src_currency = "XRP"
+        dst_currency = "XRP"
+        dst_door = Wallet(_GENESIS_SEED, 0, algorithm=CryptoAlgorithm.SECP256K1)
 
     reward_accounts = []
     signing_accounts = []
     for i in range(num_witnesses):
         original_wallet = Wallet.create(crypto_algorithm=CryptoAlgorithm.SECP256K1)
         witness_reward_wallet = Wallet(
             original_wallet.seed, 0, algorithm=CryptoAlgorithm.ED25519
@@ -561,34 +538,32 @@
         wallet = Wallet.create(CryptoAlgorithm.SECP256K1)
         signing_wallet = Wallet(wallet.seed, 0, algorithm=CryptoAlgorithm.ED25519)
         signing_accounts.append(signing_wallet.classic_address)
         ctx.invoke(
             generate_witness_config,
             config_dir=abs_config_dir,
             name=f"witness{i}",
-            locking_chain_port=locking_port,
-            issuing_chain_port=issuing_port,
+            locking_chain_port=mc_port,
+            issuing_chain_port=sc_port,
             witness_port=6010 + i,
             signing_seed=signing_wallet.seed,
-            src_door=locking_door.classic_address,
-            src_currency=locking_currency,
-            dst_door=issuing_door.classic_address,
-            dst_currency=issuing_currency,
+            src_door=src_door.classic_address,
+            src_currency=src_currency,
+            dst_door=dst_door.classic_address,
+            dst_currency=dst_currency,
             locking_reward_seed=witness_reward_wallet.seed,
             locking_reward_account=witness_reward_wallet.classic_address,
             issuing_reward_seed=witness_reward_wallet.seed,
             issuing_reward_account=witness_reward_wallet.classic_address,
             is_docker=is_docker,
         )
     ctx.invoke(
         generate_bootstrap,
         config_dir=abs_config_dir,
-        locking_seed=locking_door.seed,
-        locking_algorithm="secp256k1",
-        locking_currency=locking_currency,
-        issuing_seed=issuing_door.seed,
-        issuing_algorithm=issuing_algorithm,
-        issuing_currency=issuing_currency,
+        locking_seed=src_door.seed,
+        locking_currency=src_currency,
+        issuing_seed=dst_door.seed,
+        issuing_currency=dst_currency,
         verbose=verbose,
         reward_accounts=reward_accounts,
         signing_accounts=signing_accounts,
     )
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/ports.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/config/ports.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/templates/bootstrap.jinja` & `xbridge_cli-1.0.0b0/xbridge_cli/server/config/templates/bootstrap.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 {
   "LockingChain": {
     "Endpoint": {
-      "Host": "0.0.0.0",
+      "IP": "0.0.0.0",
       "JsonRPCPort": {{ locking_node_port }}
     },
     "DoorAccount": {
       "Address": "{{ locking_door_account }}",
       "Seed": "{{ locking_door_seed }}",
-      "KeyType": "{{ locking_door_algo }}"
+      "KeyType": "secp256k1"
     },
     "BridgeIssue": {{ locking_issue }},
     "WitnessRewardAccounts": [
       "{{ locking_reward_accounts | join("\",\n      \"") }}"
     ],
     "WitnessSubmitAccounts": [
       "{{ locking_submit_accounts | join("\",\n      \"") }}"
     ]
   },
   "IssuingChain": {
     "Endpoint": {
       {% if is_linux %}
-      "Host": "0.0.0.0",
+      "IP": "0.0.0.0",
       {% else %}
-      "Host": "0.0.0.0",
+      "IP": "0.0.0.0",
       {% endif %}
       "JsonRPCPort": {{ issuing_node_port }}
     },
     "DoorAccount": {
       "Address": "{{ issuing_door_account }}",
       "Seed": "{{ issuing_door_seed }}",
-      "KeyType": "{{ issuing_door_algo }}"
+      "KeyType": "secp256k1"
     },
     "BridgeIssue": {{ issuing_issue }},
     "WitnessRewardAccounts": [
       "{{ issuing_reward_accounts | join("\",\n      \"") }}"
     ],
     "WitnessSubmitAccounts": [
       "{{ issuing_submit_accounts | join("\",\n      \"") }}"
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/templates/rippled.jinja` & `xbridge_cli-1.0.0b0/xbridge_cli/server/config/templates/rippled.jinja`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/config/templates/witness.jinja` & `xbridge_cli-1.0.0b0/xbridge_cli/server/config/templates/witness.jinja`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 {
   "LockingChain": {
     "Endpoint": {
       {% if is_docker %}
-      "Host": "192.168.176.2",
+      "IP": "192.168.176.2",
       {% else %}
-      "Host": "127.0.0.1",
+      "IP": "127.0.0.1",
       {% endif %}
       "Port": {{ locking_chain_port }}
     },
     "TxnSubmit": {
       "ShouldSubmit": true,
       "SigningKeySeed": "{{ locking_reward_seed }}",
       "SigningKeyType": "ed25519",
       "SubmittingAccount": "{{ locking_reward_account }}"
     },
     "RewardAccount": "{{ locking_reward_account }}"
   },
   "IssuingChain": {
     "Endpoint": {
       {% if is_docker %}
-      "Host": "192.168.176.3",
+      "IP": "192.168.176.3",
       {% elif is_linux %}
-      "Host": "127.0.0.2",
+      "IP": "127.0.0.2",
       {% else %}
-      "Host": "127.0.0.1",
+      "IP": "127.0.0.1",
       {% endif %}
       "Port": {{ issuing_chain_port }}
     },
     "TxnSubmit": {
       "ShouldSubmit": true,
       "SigningKeySeed": "{{ issuing_reward_seed }}",
       "SigningKeyType": "ed25519",
       "SubmittingAccount": "{{ issuing_reward_account }}"
     },
     "RewardAccount": "{{ issuing_reward_account }}"
   },
   "RPCEndpoint": {
     {% if is_docker %}
-    "Host": "0.0.0.0",
+    "IP": "0.0.0.0",
     {% elif is_linux %}
-    "Host": "127.0.0.3",
+    "IP": "127.0.0.3",
     {% else %}
-    "Host": "127.0.0.1",
+    "IP": "127.0.0.1",
     {% endif %}
     "Port": {{ witness_port }}
   },
   "LogFile": "{{ log_file }}",
   "LogLevel": "Trace",
   "DBDir": "{{ db_dir }}",
   "SigningKeySeed": "{{ seed }}",
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/list.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/list.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/print.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/print.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/request.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/request.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/restart.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/restart.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/start.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import subprocess
 import time
 from typing import List, Tuple
 
 import click
 import docker
 import httpx
-import psutil
 
 from xbridge_cli.exceptions import XBridgeCLIException
 from xbridge_cli.utils import (
     ChainData,
     RippledConfig,
     WitnessData,
     add_chain,
@@ -33,32 +32,29 @@
         "docker-setup",
         "docker-compose.yml",
     )
 )
 
 _DOCKER_COMPOSE = ["docker", "compose", "-f", _DOCKER_COMPOSE_FILE]
 
-_START_UP_TIME = 30  # seconds
+_START_UP_TIME = 10  # seconds
 _WAIT_INCREMENT = 0.5  # seconds
 
 
 def _wait_for_process(
-    subprocess_process: subprocess.Popen[bytes],
+    process: subprocess.Popen[bytes],
     name: str,
     http_ip: str,
     http_port: int,
     output_file: str,
     is_docker: bool = False,
 ) -> None:
     http_url = f"http://{http_ip}:{http_port}"
     time_waited = 0.0
-    process = psutil.Process(pid=subprocess_process.pid)
     while time_waited < _START_UP_TIME:
-        if process.status() == psutil.STATUS_ZOMBIE:
-            break
         try:
             request = {"method": "server_info"}
             httpx.post(http_url, json=request)
             if is_docker:
                 docker_client = docker.from_env()
                 container = docker_client.containers.get(name)
                 assert container.status == "running"
@@ -191,57 +187,55 @@
         # add chain to config file
         add_chain(chain_data)
     else:
         # check if server actually started up correctly
         _wait_for_process(
             process,
             name,
-            config_json["RPCEndpoint"]["Host"],
+            config_json["RPCEndpoint"]["IP"],
             config_json["RPCEndpoint"]["Port"],
             output_file,
             exe == "docker",
         )
         witness_data: WitnessData = {
             "name": name,
             "type": "witness",
             "exe": exe,
             "config": config,
             "pid": process.pid,
-            "http_ip": config_json["RPCEndpoint"]["Host"],
+            "http_ip": config_json["RPCEndpoint"]["IP"],
             "http_port": config_json["RPCEndpoint"]["Port"],
         }
         # add witness to config file
         add_witness(witness_data)
 
     if verbose:
         click.echo(f"started {server_type} at `{exe}` with config `{config}`")
         click.echo(f"PID: {process.pid}")
 
 
 @click.command(name="start-all")
 @click.option(
-    "--config-dir",
-    "config_dir",
+    "--config_dir",
     envvar="XCHAIN_CONFIG_DIR",
     required=True,
     prompt=True,
     type=click.Path(exists=True),
-    help="The folder in which config files are stored.",
+    help="The folder in which config files are storeds.",
 )
 @click.option(
-    "--rippled-exe",
-    "rippled_exe",
+    "--rippled_exe",
     envvar="RIPPLED_EXE",
     required=True,
     prompt=True,
     type=str,  # TODO: should be Union[Literal["docker"], click.Path(exists=True)]
     help="The filepath to the rippled executable.",
 )
 @click.option(
-    "--witnessd-exe",
+    "--witnessd_exe",
     envvar="WITNESSD_EXE",
     required=True,
     prompt=True,
     type=str,  # TODO: should be Union[Literal["docker"], click.Path(exists=True)]
     help="The filepath to the witnessd executable.",
 )
 @click.option("--docker", is_flag=True, help="Use executables from Docker.")
@@ -359,27 +353,27 @@
                 with open(config) as f:
                     config_json = json.load(f)
 
                 # check if server actually started up correctly
                 _wait_for_process(
                     process,
                     name,
-                    config_json["RPCEndpoint"]["Host"],
+                    config_json["RPCEndpoint"]["IP"],
                     config_json["RPCEndpoint"]["Port"],
                     output_file,
                     witnessd_exe == "docker",
                 )
 
                 witness_data: WitnessData = {
                     "name": name,
                     "type": "witness",
                     "exe": "docker",
                     "config": config,
                     "pid": process.pid,
-                    "http_ip": config_json["RPCEndpoint"]["Host"],
+                    "http_ip": config_json["RPCEndpoint"]["IP"],
                     "http_port": config_json["RPCEndpoint"]["Port"],
                 }
                 # add witness to config file
                 add_witness(witness_data)
         else:
             for name, config in witnesses:
                 ctx.invoke(
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/server/stop.py` & `xbridge_cli-1.0.0b0/xbridge_cli/server/stop.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/__init__.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/attestations.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/attestations.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/__init__.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/__init__.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/bridge_config.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/bridge_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/chain_config.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/chain_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_file.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/config_file.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/config_item.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/config_item.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/server_config.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/server_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_file/witness_config.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_file/witness_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/config_utils.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/rippled_config.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/rippled_config.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/transaction.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,14 @@
             automatically.
 
     Returns:
         The response from rippled.
     """
     if isinstance(txs, Transaction):
         txs = [txs]
-    if len(txs) == 0:
-        return []
     if verbose > 0:
         tx_types = ", ".join([tx.transaction_type.value for tx in txs])
         click.secho(f"Submitting {tx_types} tx to {client.url}...", fg="blue")
         if verbose > 1:
             for tx in txs:
                 click.echo(pformat(tx.to_xrpl()))
```

### Comparing `xbridge_cli-0.3.0/xbridge_cli/utils/types.py` & `xbridge_cli-1.0.0b0/xbridge_cli/utils/types.py`

 * *Files identical despite different names*

### Comparing `xbridge_cli-0.3.0/setup.py` & `xbridge_cli-1.0.0b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,22 @@
  'click>=8.1.3,<9.0.0',
  'docker>=6.0.0,<7.0.0',
  'httpx>=0.18.1,<0.24.0',
  'psutil>=5.9.2,<6.0.0',
  'pycryptodome>=3.17,<4.0',
  'tabulate>=0.8.9,<0.10.0',
  'websockets>=10.3,<11.0',
- 'xrpl-py==1.9.0b1']
+ 'xrpl-py==1.8.0b1']
 
 entry_points = \
 {'console_scripts': ['xbridge-cli = xbridge_cli.main:main']}
 
 setup_kwargs = {
     'name': 'xbridge-cli',
-    'version': '0.3.0',
+    'version': '1.0.0b0',
     'description': 'A CLI that helps you set up an XRPL-XRPL bridge.',
     'long_description': "# xbridge-cli\n\n## Install\n\n```bash\npip install xbridge-cli\n```\n\nNOTE: if you're looking at the repo before it's published, this won't work. Instead, you'll do this:\n\n```bash\ngit clone https://github.com/xpring-eng/xbridge-cli.git\ncd xbridge-cli\n# install poetry\ncurl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -\npoetry install\npoetry shell\n```\n\nInstall rippled and the xbridge witness.\n\nrippled: https://xrpl.org/install-rippled.html\n\nwitness: https://github.com/seelabs/xbridge_witness\n\n## Get started\n\n```bash\nexport XCHAIN_CONFIG_DIR={filepath where you want your config files stored}\nexport RIPPLED_EXE={rippled exe filepath}\nexport WITNESSD_EXE={witnessd exe filepath}\n./scripts/tutorial.sh\n```\n\nTo stop the servers:\n\n```bash\nxbridge-cli server stop --all\n```\n\n## Use Commands\n\n```bash\nxbridge-cli --help\n```\n\nEach subcommand also has a `--help` flag, to tell you what fields you'll need.\n",
     'author': 'Mayukha Vadari',
     'author_email': 'mvadari@ripple.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xpring-eng/xbridge-cli',
```

### Comparing `xbridge_cli-0.3.0/PKG-INFO` & `xbridge_cli-1.0.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xbridge-cli
-Version: 0.3.0
+Version: 1.0.0b0
 Summary: A CLI that helps you set up an XRPL-XRPL bridge.
 Home-page: https://github.com/xpring-eng/xbridge-cli
 License: MIT
 Keywords: xrp,xrpl,cryptocurrency
 Author: Mayukha Vadari
 Author-email: mvadari@ripple.com
 Requires-Python: >=3.7.1,<4.0.0
@@ -18,15 +18,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: httpx (>=0.18.1,<0.24.0)
 Requires-Dist: psutil (>=5.9.2,<6.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: tabulate (>=0.8.9,<0.10.0)
 Requires-Dist: websockets (>=10.3,<11.0)
-Requires-Dist: xrpl-py (==1.9.0b1)
+Requires-Dist: xrpl-py (==1.8.0b1)
 Project-URL: Repository, https://github.com/xpring-eng/xbridge-cli
 Description-Content-Type: text/markdown
 
 # xbridge-cli
 
 ## Install
```

