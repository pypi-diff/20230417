# Comparing `tmp/flow_py_sdk_legacy-1.0.2.tar.gz` & `tmp/flow_py_sdk_legacy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_py_sdk_legacy-1.0.2.tar", max compression
+gzip compressed data, was "flow_py_sdk_legacy-1.1.0.tar", max compression
```

## Comparing `flow_py_sdk_legacy-1.0.2.tar` & `flow_py_sdk_legacy-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,41 @@
--rw-r--r--   0        0        0     1075 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/LICENSE
--rw-r--r--   0        0        0      970 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/README.md
--rw-r--r--   0        0        0      505 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/__init__.py
--rw-r--r--   0        0        0     6482 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/account_key.py
--rw-r--r--   0        0        0     2001 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/__init__.py
--rw-r--r--   0        0        0     2116 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/address.py
--rw-r--r--   0        0        0     2160 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/composite.py
--rw-r--r--   0        0        0     1495 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/constants.py
--rw-r--r--   0        0        0     1507 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/decode.py
--rw-r--r--   0        0        0     1600 2023-04-16 23:35:37.961074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/encode.py
--rw-r--r--   0        0        0     1125 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/kind.py
--rw-r--r--   0        0        0    10018 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/kinds.py
--rw-r--r--   0        0        0     7019 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/simple_kinds.py
--rw-r--r--   0        0        0    16642 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/types.py
--rw-r--r--   0        0        0     1131 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/value.py
--rw-r--r--   0        0        0       43 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/client/__init__.py
--rw-r--r--   0        0        0    18652 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/client/client.py
--rw-r--r--   0        0        0     9839 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/client/entities.py
--rw-r--r--   0        0        0      689 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/exceptions.py
--rw-r--r--   0        0        0       37 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/frlp/__init__.py
--rw-r--r--   0        0        0      108 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/frlp/utils.py
--rw-r--r--   0        0        0        0 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/__init__.py
--rw-r--r--   0        0        0    32783 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/access/__init__.py
--rw-r--r--   0        0        0    14122 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/access.py
--rw-r--r--   0        0        0     4255 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/entities/__init__.py
--rw-r--r--   0        0        0     4000 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/entities.py
--rw-r--r--   0        0        0     9399 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/execution/__init__.py
--rw-r--r--   0        0        0     4702 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/execution.py
--rw-r--r--   0        0        0     1384 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/script.py
--rw-r--r--   0        0        0      361 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/__init__.py
--rw-r--r--   0        0        0      804 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/hash_algo.py
--rw-r--r--   0        0        0     1393 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/in_memory_signer.py
--rw-r--r--   0        0        0     1060 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/in_memory_verifier.py
--rw-r--r--   0        0        0     1015 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/sign_algo.py
--rw-r--r--   0        0        0     2042 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/signer.py
--rw-r--r--   0        0        0     1803 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/verifier.py
--rw-r--r--   0        0        0     4164 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/templates.py
--rw-r--r--   0        0        0     8118 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/tx.py
--rw-r--r--   0        0        0       77 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1526 2023-04-16 23:35:37.965074 flow_py_sdk_legacy-1.0.2/flow_py_sdk/utils/verify_user_signature.py
--rw-r--r--   0        0        0      943 2023-04-16 23:36:34.085194 flow_py_sdk_legacy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.0.2/setup.py
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-17 00:14:32.700247 flow_py_sdk_legacy-1.1.0/LICENSE
+-rw-r--r--   0        0        0      970 2023-04-17 00:14:32.700247 flow_py_sdk_legacy-1.1.0/README.md
+-rw-r--r--   0        0        0      505 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/__init__.py
+-rw-r--r--   0        0        0     6482 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/account_key.py
+-rw-r--r--   0        0        0     2001 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/__init__.py
+-rw-r--r--   0        0        0     2116 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/address.py
+-rw-r--r--   0        0        0     2160 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/composite.py
+-rw-r--r--   0        0        0     1495 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/constants.py
+-rw-r--r--   0        0        0     1507 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/decode.py
+-rw-r--r--   0        0        0     1600 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/encode.py
+-rw-r--r--   0        0        0     1125 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/kind.py
+-rw-r--r--   0        0        0    10018 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/kinds.py
+-rw-r--r--   0        0        0     7019 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/simple_kinds.py
+-rw-r--r--   0        0        0    16642 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/types.py
+-rw-r--r--   0        0        0     1131 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/value.py
+-rw-r--r--   0        0        0       43 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/client/__init__.py
+-rw-r--r--   0        0        0    18652 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/client/client.py
+-rw-r--r--   0        0        0     9839 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/client/entities.py
+-rw-r--r--   0        0        0      689 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/exceptions.py
+-rw-r--r--   0        0        0       37 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/frlp/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/frlp/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/flow/__init__.py
+-rw-r--r--   0        0        0    14122 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/flow/access.py
+-rw-r--r--   0        0        0     4000 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/flow/entities.py
+-rw-r--r--   0        0        0     4702 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/flow/execution.py
+-rw-r--r--   0        0        0     1384 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/script.py
+-rw-r--r--   0        0        0      361 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/__init__.py
+-rw-r--r--   0        0        0      804 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/hash_algo.py
+-rw-r--r--   0        0        0     1393 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/in_memory_signer.py
+-rw-r--r--   0        0        0     1060 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/in_memory_verifier.py
+-rw-r--r--   0        0        0     1015 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/sign_algo.py
+-rw-r--r--   0        0        0     2042 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/signer.py
+-rw-r--r--   0        0        0     1803 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/verifier.py
+-rw-r--r--   0        0        0     4164 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/templates.py
+-rw-r--r--   0        0        0     8118 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/tx.py
+-rw-r--r--   0        0        0       77 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1549 2023-04-17 00:14:32.704247 flow_py_sdk_legacy-1.1.0/flow_py_sdk/utils/verify_user_signature.py
+-rw-r--r--   0        0        0      945 2023-04-17 00:15:18.704142 flow_py_sdk_legacy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2065 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.1.0/setup.py
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.1.0/PKG-INFO
```

### Comparing `flow_py_sdk_legacy-1.0.2/LICENSE` & `flow_py_sdk_legacy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/README.md` & `flow_py_sdk_legacy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/account_key.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/account_key.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/__init__.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/address.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/address.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/composite.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/composite.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/constants.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/constants.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/decode.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/decode.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/encode.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/encode.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/kind.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/kind.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/kinds.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/kinds.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/simple_kinds.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/simple_kinds.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/types.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/types.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/cadence/value.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/cadence/value.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/client/client.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from grpclib.encoding.base import CodecBase, StatusDetailsCodecBase
 from grpclib.metadata import Deadline
 
 from flow_py_sdk import cadence
 from flow_py_sdk.cadence import Value, cadence_object_hook, encode_arguments
 from flow_py_sdk.client import entities
 from flow_py_sdk.proto.flow.access import (
-    AccessApiStub,
+    AccessAPIStub,
     PingResponse,
 )
 from flow_py_sdk.script import Script
 from flow_py_sdk.tx import Tx, TransactionStatus
 
 log = logging.getLogger(__name__)
 
 
-class AccessAPI(AccessApiStub):
+class AccessAPI(AccessAPIStub):
     def __init__(
         self,
         channel: "Channel",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata=None,
```

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/client/entities.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/client/entities.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/exceptions.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/access.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/flow/access.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/entities/__init__.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/flow/entities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,117 +1,114 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: flow/entities/account.proto, flow/entities/block.proto, flow/entities/block_header.proto, flow/entities/block_seal.proto, flow/entities/collection.proto, flow/entities/event.proto, flow/entities/transaction.proto
+# sources: flow/entities/account.proto, flow/entities/block_header.proto, flow/entities/collection.proto, flow/entities/block_seal.proto, flow/entities/block.proto, flow/entities/event.proto, flow/entities/transaction.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 from datetime import datetime
-from typing import (
-    Dict,
-    List,
-)
+from typing import Dict, List
 
 import betterproto
 
 
 class TransactionStatus(betterproto.Enum):
     UNKNOWN = 0
     PENDING = 1
     FINALIZED = 2
     EXECUTED = 3
     SEALED = 4
     EXPIRED = 5
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class Account(betterproto.Message):
     address: bytes = betterproto.bytes_field(1)
     balance: int = betterproto.uint64_field(2)
     code: bytes = betterproto.bytes_field(3)
     keys: List["AccountKey"] = betterproto.message_field(4)
     contracts: Dict[str, bytes] = betterproto.map_field(
         5, betterproto.TYPE_STRING, betterproto.TYPE_BYTES
     )
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class AccountKey(betterproto.Message):
     index: int = betterproto.uint32_field(1)
     public_key: bytes = betterproto.bytes_field(2)
     sign_algo: int = betterproto.uint32_field(3)
     hash_algo: int = betterproto.uint32_field(4)
     weight: int = betterproto.uint32_field(5)
     sequence_number: int = betterproto.uint32_field(6)
     revoked: bool = betterproto.bool_field(7)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class BlockHeader(betterproto.Message):
     id: bytes = betterproto.bytes_field(1)
     parent_id: bytes = betterproto.bytes_field(2)
     height: int = betterproto.uint64_field(3)
     timestamp: datetime = betterproto.message_field(4)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class Collection(betterproto.Message):
     id: bytes = betterproto.bytes_field(1)
     transaction_ids: List[bytes] = betterproto.bytes_field(2)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class CollectionGuarantee(betterproto.Message):
     collection_id: bytes = betterproto.bytes_field(1)
     signatures: List[bytes] = betterproto.bytes_field(2)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class BlockSeal(betterproto.Message):
     block_id: bytes = betterproto.bytes_field(1)
     execution_receipt_id: bytes = betterproto.bytes_field(2)
     execution_receipt_signatures: List[bytes] = betterproto.bytes_field(3)
     result_approval_signatures: List[bytes] = betterproto.bytes_field(4)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class Block(betterproto.Message):
     id: bytes = betterproto.bytes_field(1)
     parent_id: bytes = betterproto.bytes_field(2)
     height: int = betterproto.uint64_field(3)
     timestamp: datetime = betterproto.message_field(4)
     collection_guarantees: List["CollectionGuarantee"] = betterproto.message_field(5)
     block_seals: List["BlockSeal"] = betterproto.message_field(6)
     signatures: List[bytes] = betterproto.bytes_field(7)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class Event(betterproto.Message):
     type: str = betterproto.string_field(1)
     transaction_id: bytes = betterproto.bytes_field(2)
     transaction_index: int = betterproto.uint32_field(3)
     event_index: int = betterproto.uint32_field(4)
     payload: bytes = betterproto.bytes_field(5)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class Transaction(betterproto.Message):
     script: bytes = betterproto.bytes_field(1)
     arguments: List[bytes] = betterproto.bytes_field(2)
     reference_block_id: bytes = betterproto.bytes_field(3)
     gas_limit: int = betterproto.uint64_field(4)
     proposal_key: "TransactionProposalKey" = betterproto.message_field(5)
     payer: bytes = betterproto.bytes_field(6)
     authorizers: List[bytes] = betterproto.bytes_field(7)
     payload_signatures: List["TransactionSignature"] = betterproto.message_field(8)
     envelope_signatures: List["TransactionSignature"] = betterproto.message_field(9)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class TransactionProposalKey(betterproto.Message):
     address: bytes = betterproto.bytes_field(1)
     key_id: int = betterproto.uint32_field(2)
     sequence_number: int = betterproto.uint64_field(3)
 
 
-@dataclass(eq=False, repr=False)
+@dataclass
 class TransactionSignature(betterproto.Message):
     address: bytes = betterproto.bytes_field(1)
     key_id: int = betterproto.uint32_field(2)
     signature: bytes = betterproto.bytes_field(3)
```

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/proto/flow/execution.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/proto/flow/execution.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/script.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/script.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/hash_algo.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/hash_algo.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/in_memory_signer.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/in_memory_signer.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/in_memory_verifier.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/in_memory_verifier.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/sign_algo.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/sign_algo.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/signer.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/signer.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/signer/verifier.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/signer/verifier.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/templates.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/templates.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/tx.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/tx.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-1.0.2/flow_py_sdk/utils/verify_user_signature.py` & `flow_py_sdk_legacy-1.1.0/flow_py_sdk/utils/verify_user_signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import dataclass
 
 from flow_py_sdk import cadence
 from flow_py_sdk.exceptions import PySDKError
 from flow_py_sdk.templates import TransactionTemplates
 from flow_py_sdk.client import AccessAPI
 from flow_py_sdk.script import Script
-
+from typing import List
 
 @dataclass
 class CompositeSignature(object):
     addr: str
     keyId: int
     signature: str
 
 
 async def verify_user_signature(
-    *, client: AccessAPI, message: bytes, composite_signatures: list[CompositeSignature]
+    *, client: AccessAPI, message: bytes, composite_signatures: List[CompositeSignature]
 ) -> bool:
     # if there is no signature return False
     if len(composite_signatures) == 0:
         return False
 
     # it does not make sense for the signatures to be from different addresses
     if any(x.addr != composite_signatures[0].addr for x in composite_signatures):
```

### Comparing `flow_py_sdk_legacy-1.0.2/pyproject.toml` & `flow_py_sdk_legacy-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "flow-py-sdk-legacy"
-version = "1.0.2"
+version = "1.1.0"
 description = "A python SDK for the flow blockchain"
 authors = ["Janez Podhostnik <janez.podhostnik@gmail.com>", "justin.kc.herrera@gmail.com"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/justinnout/flow-py-sdk"
 packages = [
     { include = "flow_py_sdk" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 betterproto = {extras = ["compiler"], version = "v2.0.0-beta5"}
 grpcio-tools = "^1.51"
 ecdsa = "^v0.15"
-rlp = "^3.0"
+rlp = "^1.2.0"
 grpclib = "^0.4"
 
 [tool.poetry.dev-dependencies]
 coloredlogs = "^15.0"
 toml = "^0.10"
 black = "^23.1"
 pytest = "^7.2"
```

### Comparing `flow_py_sdk_legacy-1.0.2/setup.py` & `flow_py_sdk_legacy-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,36 +4,33 @@
 packages = \
 ['flow_py_sdk',
  'flow_py_sdk.cadence',
  'flow_py_sdk.client',
  'flow_py_sdk.frlp',
  'flow_py_sdk.proto',
  'flow_py_sdk.proto.flow',
- 'flow_py_sdk.proto.flow.access',
- 'flow_py_sdk.proto.flow.entities',
- 'flow_py_sdk.proto.flow.execution',
  'flow_py_sdk.signer',
  'flow_py_sdk.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['betterproto[compiler]==v2.0.0-beta5',
  'ecdsa>=v0.15,<0.16',
  'grpcio-tools>=1.51,<2.0',
  'grpclib>=0.4,<0.5',
- 'rlp>=3.0,<4.0']
+ 'rlp>=1.2.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['examples = examples.main:run']}
 
 setup_kwargs = {
     'name': 'flow-py-sdk-legacy',
-    'version': '1.0.2',
+    'version': '1.1.0',
     'description': 'A python SDK for the flow blockchain',
     'long_description': 'The Flow Python SDK provides a set of packages for Python developers to build applications that interact with the Flow network.\n\n[![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/)\n[![codecov](https://codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)\n\n\nSee the [guide](https://janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)!\n\n\nNote: This SDK is also fully compatible with the Flow Emulator and can be used for local development.\n\n## Installing\n\nTo start using the SDK, install Python 3.7 or higher and install package:\n\n```sh\npip install flow-py-sdk-legacy\n```\n\nor if using poetry:\n\n```sh\npoetry add flow-py-sdk-legacy\n```\n\n## Contributors\n\n<a href="https://github.com/justinnout/flow-py-sdk/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=justinnout/flow-py-sdk" />\n</a>\n\nMade with [contrib.rocks](https://contrib.rocks).',
     'author': 'Janez Podhostnik',
     'author_email': 'janez.podhostnik@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/justinnout/flow-py-sdk',
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['flow_py_sdk', 'flow_py_sdk.cadence', 'flow_py_sdk.client',
 'flow_py_sdk.frlp', 'flow_py_sdk.proto', 'flow_py_sdk.proto.flow',
-'flow_py_sdk.proto.flow.access', 'flow_py_sdk.proto.flow.entities',
-'flow_py_sdk.proto.flow.execution', 'flow_py_sdk.signer', 'flow_py_sdk.utils']
-package_data = \ {'': ['*']} install_requires = \ ['betterproto
-[compiler]==v2.0.0-beta5', 'ecdsa>=v0.15,<0.16', 'grpcio-tools>=1.51,<2.0',
-'grpclib>=0.4,<0.5', 'rlp>=3.0,<4.0'] entry_points = \ {'console_scripts':
-['examples = examples.main:run']} setup_kwargs = { 'name': 'flow-py-sdk-
-legacy', 'version': '1.0.2', 'description': 'A python SDK for the flow
-blockchain', 'long_description': 'The Flow Python SDK provides a set of
-packages for Python developers to build applications that interact with the
-Flow network.\n\n[![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-
-legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/)\n[![codecov](https:/
-/codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://
-codecov.io/gh/codecov/example-go)\n\n\nSee the [guide](https://
-janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)!\n\n\nNote: This SDK
-is also fully compatible with the Flow Emulator and can be used for local
-development.\n\n## Installing\n\nTo start using the SDK, install Python 3.7 or
-higher and install package:\n\n```sh\npip install flow-py-sdk-legacy\n```\n\nor
-if using poetry:\n\n```sh\npoetry add flow-py-sdk-legacy\n```\n\n##
-Contributors\n\n\n_[https://contrib.rocks/image?repo=justinnout/flow-py-
-sdk]\n\n\nMade with [contrib.rocks](https://contrib.rocks).', 'author': 'Janez
-Podhostnik', 'author_email': 'janez.podhostnik@gmail.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/justinnout/flow-
-py-sdk', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+'flow_py_sdk.signer', 'flow_py_sdk.utils'] package_data = \ {'': ['*']}
+install_requires = \ ['betterproto[compiler]==v2.0.0-beta5',
+'ecdsa>=v0.15,<0.16', 'grpcio-tools>=1.51,<2.0', 'grpclib>=0.4,<0.5',
+'rlp>=1.2.0,<2.0.0'] entry_points = \ {'console_scripts': ['examples =
+examples.main:run']} setup_kwargs = { 'name': 'flow-py-sdk-legacy', 'version':
+'1.1.0', 'description': 'A python SDK for the flow blockchain',
+'long_description': 'The Flow Python SDK provides a set of packages for Python
+developers to build applications that interact with the Flow network.\n\n[!
+[PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/
+project/flow-py-sdk-legacy/)\n[![codecov](https://codecov.io/gh/justinnout/
+flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/
+example-go)\n\n\nSee the [guide](https://janezpodhostnik.github.io/flow-py-sdk/
+python_SDK_guide/)!\n\n\nNote: This SDK is also fully compatible with the Flow
+Emulator and can be used for local development.\n\n## Installing\n\nTo start
+using the SDK, install Python 3.7 or higher and install package:\n\n```sh\npip
+install flow-py-sdk-legacy\n```\n\nor if using poetry:\n\n```sh\npoetry add
+flow-py-sdk-legacy\n```\n\n## Contributors\n\n\n_[https://contrib.rocks/
+image?repo=justinnout/flow-py-sdk]\n\n\nMade with [contrib.rocks](https://
+contrib.rocks).', 'author': 'Janez Podhostnik', 'author_email':
+'janez.podhostnik@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
+'url': 'https://github.com/justinnout/flow-py-sdk', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
+(**setup_kwargs)
```

### Comparing `flow_py_sdk_legacy-1.0.2/PKG-INFO` & `flow_py_sdk_legacy-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow-py-sdk-legacy
-Version: 1.0.2
+Version: 1.1.0
 Summary: A python SDK for the flow blockchain
 Home-page: https://github.com/justinnout/flow-py-sdk
 License: MIT
 Author: Janez Podhostnik
 Author-email: janez.podhostnik@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: betterproto[compiler] (==v2.0.0-beta5)
 Requires-Dist: ecdsa (>=v0.15,<0.16)
 Requires-Dist: grpcio-tools (>=1.51,<2.0)
 Requires-Dist: grpclib (>=0.4,<0.5)
-Requires-Dist: rlp (>=3.0,<4.0)
+Requires-Dist: rlp (>=1.2.0,<2.0.0)
 Project-URL: Repository, https://github.com/justinnout/flow-py-sdk
 Description-Content-Type: text/markdown
 
 The Flow Python SDK provides a set of packages for Python developers to build applications that interact with the Flow network.
 
 [![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/)
 [![codecov](https://codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: flow-py-sdk-legacy Version: 1.0.2 Summary: A python
+Metadata-Version: 2.1 Name: flow-py-sdk-legacy Version: 1.1.0 Summary: A python
 SDK for the flow blockchain Home-page: https://github.com/justinnout/flow-py-
 sdk License: MIT Author: Janez Podhostnik Author-email:
 janez.podhostnik@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: betterproto[compiler] (==v2.0.0-
 beta5) Requires-Dist: ecdsa (>=v0.15,<0.16) Requires-Dist: grpcio-tools
 (>=1.51,<2.0) Requires-Dist: grpclib (>=0.4,<0.5) Requires-Dist: rlp
-(>=3.0,<4.0) Project-URL: Repository, https://github.com/justinnout/flow-py-sdk
-Description-Content-Type: text/markdown The Flow Python SDK provides a set of
-packages for Python developers to build applications that interact with the
-Flow network. [![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)]
-(https://pypi.org/project/flow-py-sdk-legacy/) [![codecov](https://codecov.io/
-gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/
-gh/codecov/example-go) See the [guide](https://janezpodhostnik.github.io/flow-
-py-sdk/python_SDK_guide/)! Note: This SDK is also fully compatible with the
-Flow Emulator and can be used for local development. ## Installing To start
-using the SDK, install Python 3.7 or higher and install package: ```sh pip
-install flow-py-sdk-legacy ``` or if using poetry: ```sh poetry add flow-py-
-sdk-legacy ``` ## Contributors [https://contrib.rocks/image?repo=justinnout/
-flow-py-sdk] Made with [contrib.rocks](https://contrib.rocks).
+(>=1.2.0,<2.0.0) Project-URL: Repository, https://github.com/justinnout/flow-
+py-sdk Description-Content-Type: text/markdown The Flow Python SDK provides a
+set of packages for Python developers to build applications that interact with
+the Flow network. [![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-
+legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/) [![codecov](https://
+codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://
+codecov.io/gh/codecov/example-go) See the [guide](https://
+janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)! Note: This SDK is
+also fully compatible with the Flow Emulator and can be used for local
+development. ## Installing To start using the SDK, install Python 3.7 or higher
+and install package: ```sh pip install flow-py-sdk-legacy ``` or if using
+poetry: ```sh poetry add flow-py-sdk-legacy ``` ## Contributors [https://
+contrib.rocks/image?repo=justinnout/flow-py-sdk] Made with [contrib.rocks]
+(https://contrib.rocks).
```

