# Comparing `tmp/flow_py_sdk_legacy-0.0.0.tar.gz` & `tmp/flow_py_sdk_legacy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_py_sdk_legacy-0.0.0.tar", max compression
+gzip compressed data, was "flow_py_sdk_legacy-1.0.0.tar", max compression
```

## Comparing `flow_py_sdk_legacy-0.0.0.tar` & `flow_py_sdk_legacy-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1075 2023-04-13 22:52:14.204474 flow_py_sdk_legacy-0.0.0/LICENSE
--rw-r--r--   0        0        0      957 2023-04-13 23:01:10.695886 flow_py_sdk_legacy-0.0.0/README.md
--rw-r--r--   0        0        0      505 2023-04-16 22:47:30.449664 flow_py_sdk_legacy-0.0.0/flow_py_sdk/__init__.py
--rw-r--r--   0        0        0     6482 2023-04-13 22:52:14.209351 flow_py_sdk_legacy-0.0.0/flow_py_sdk/account_key.py
--rw-r--r--   0        0        0     2001 2023-04-13 22:52:14.209540 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/__init__.py
--rw-r--r--   0        0        0     2116 2023-04-16 22:47:41.167252 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/address.py
--rw-r--r--   0        0        0     2160 2023-04-13 22:52:14.209797 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/composite.py
--rw-r--r--   0        0        0     1495 2023-04-13 22:52:14.209916 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/constants.py
--rw-r--r--   0        0        0     1507 2023-04-13 23:28:50.616608 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/decode.py
--rw-r--r--   0        0        0     1600 2023-04-13 23:29:22.066486 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/encode.py
--rw-r--r--   0        0        0     1125 2023-04-16 22:50:50.234068 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/kind.py
--rw-r--r--   0        0        0    10018 2023-04-14 20:28:59.437367 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/kinds.py
--rw-r--r--   0        0        0     7019 2023-04-13 22:52:14.210554 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/simple_kinds.py
--rw-r--r--   0        0        0    16642 2023-04-13 22:52:14.210721 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/types.py
--rw-r--r--   0        0        0     1131 2023-04-16 22:51:47.929400 flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/value.py
--rw-r--r--   0        0        0       43 2023-04-13 22:52:14.211112 flow_py_sdk_legacy-0.0.0/flow_py_sdk/client/__init__.py
--rw-r--r--   0        0        0    18652 2023-04-14 20:55:59.387493 flow_py_sdk_legacy-0.0.0/flow_py_sdk/client/client.py
--rw-r--r--   0        0        0     9839 2023-04-13 22:52:14.211514 flow_py_sdk_legacy-0.0.0/flow_py_sdk/client/entities.py
--rw-r--r--   0        0        0      689 2023-04-13 22:52:14.211629 flow_py_sdk_legacy-0.0.0/flow_py_sdk/exceptions.py
--rw-r--r--   0        0        0       37 2023-04-13 22:52:14.211793 flow_py_sdk_legacy-0.0.0/flow_py_sdk/frlp/__init__.py
--rw-r--r--   0        0        0      108 2023-04-13 22:52:14.211927 flow_py_sdk_legacy-0.0.0/flow_py_sdk/frlp/utils.py
--rw-r--r--   0        0        0        0 2023-04-14 20:40:09.975603 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 20:40:09.975664 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/__init__.py
--rw-r--r--   0        0        0    32783 2023-04-14 20:54:03.992745 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/access/__init__.py
--rw-r--r--   0        0        0    14122 2023-04-13 22:52:14.212407 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/access.py
--rw-r--r--   0        0        0     4255 2023-04-14 20:40:09.977190 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/entities/__init__.py
--rw-r--r--   0        0        0     4000 2023-04-13 22:52:14.212544 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/entities.py
--rw-r--r--   0        0        0     9399 2023-04-14 20:40:09.978036 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/execution/__init__.py
--rw-r--r--   0        0        0     4702 2023-04-13 22:52:14.212680 flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/execution.py
--rw-r--r--   0        0        0     1384 2023-04-13 22:52:14.212809 flow_py_sdk_legacy-0.0.0/flow_py_sdk/script.py
--rw-r--r--   0        0        0      361 2023-04-13 22:52:14.213000 flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/__init__.py
--rw-r--r--   0        0        0      804 2023-04-13 22:52:14.213153 flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/hash_algo.py
--rw-r--r--   0        0        0     1393 2023-04-13 22:52:14.213268 flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/in_memory_signer.py
--rw-r--r--   0        0        0     1060 2023-04-13 22:52:14.213376 flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/in_memory_verifier.py
--rw-r--r--   0        0        0     1015 2023-04-13 22:52:14.213492 flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/sign_algo.py
--rw-r--r--   0        0        0     2042 2023-04-13 22:52:14.213649 flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/signer.py
--rw-r--r--   0        0        0     1803 2023-04-13 22:52:14.213821 flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/verifier.py
--rw-r--r--   0        0        0     4164 2023-04-14 20:59:34.926612 flow_py_sdk_legacy-0.0.0/flow_py_sdk/templates.py
--rw-r--r--   0        0        0     8118 2023-04-14 20:54:59.172850 flow_py_sdk_legacy-0.0.0/flow_py_sdk/tx.py
--rw-r--r--   0        0        0       77 2023-04-13 22:52:14.214295 flow_py_sdk_legacy-0.0.0/flow_py_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1526 2023-04-13 22:52:14.214433 flow_py_sdk_legacy-0.0.0/flow_py_sdk/utils/verify_user_signature.py
--rw-r--r--   0        0        0      942 2023-04-16 23:15:52.275328 flow_py_sdk_legacy-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/LICENSE
+-rw-r--r--   0        0        0      970 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/README.md
+-rw-r--r--   0        0        0      505 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/__init__.py
+-rw-r--r--   0        0        0     6482 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/account_key.py
+-rw-r--r--   0        0        0     2001 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/__init__.py
+-rw-r--r--   0        0        0     2116 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/address.py
+-rw-r--r--   0        0        0     2160 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/composite.py
+-rw-r--r--   0        0        0     1495 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/constants.py
+-rw-r--r--   0        0        0     1507 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/decode.py
+-rw-r--r--   0        0        0     1600 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/encode.py
+-rw-r--r--   0        0        0     1125 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/kind.py
+-rw-r--r--   0        0        0    10018 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/kinds.py
+-rw-r--r--   0        0        0     7019 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/simple_kinds.py
+-rw-r--r--   0        0        0    16642 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/types.py
+-rw-r--r--   0        0        0     1131 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/value.py
+-rw-r--r--   0        0        0       43 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/client/__init__.py
+-rw-r--r--   0        0        0    18652 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/client/client.py
+-rw-r--r--   0        0        0     9839 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/client/entities.py
+-rw-r--r--   0        0        0      689 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/exceptions.py
+-rw-r--r--   0        0        0       37 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/frlp/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/frlp/utils.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/__init__.py
+-rw-r--r--   0        0        0    32783 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/access/__init__.py
+-rw-r--r--   0        0        0    14122 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/access.py
+-rw-r--r--   0        0        0     4255 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/entities/__init__.py
+-rw-r--r--   0        0        0     4000 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/entities.py
+-rw-r--r--   0        0        0     9399 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/execution/__init__.py
+-rw-r--r--   0        0        0     4702 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/execution.py
+-rw-r--r--   0        0        0     1384 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/script.py
+-rw-r--r--   0        0        0      361 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/__init__.py
+-rw-r--r--   0        0        0      804 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/hash_algo.py
+-rw-r--r--   0        0        0     1393 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/in_memory_signer.py
+-rw-r--r--   0        0        0     1060 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/in_memory_verifier.py
+-rw-r--r--   0        0        0     1015 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/sign_algo.py
+-rw-r--r--   0        0        0     2042 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/signer.py
+-rw-r--r--   0        0        0     1803 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/verifier.py
+-rw-r--r--   0        0        0     4164 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/templates.py
+-rw-r--r--   0        0        0     8118 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/tx.py
+-rw-r--r--   0        0        0       77 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1526 2023-04-16 23:21:33.419227 flow_py_sdk_legacy-1.0.0/flow_py_sdk/utils/verify_user_signature.py
+-rw-r--r--   0        0        0      943 2023-04-16 23:22:17.663993 flow_py_sdk_legacy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.0.0/setup.py
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 flow_py_sdk_legacy-1.0.0/PKG-INFO
```

### Comparing `flow_py_sdk_legacy-0.0.0/LICENSE` & `flow_py_sdk_legacy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/README.md` & `flow_py_sdk_legacy-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 The Flow Python SDK provides a set of packages for Python developers to build applications that interact with the Flow network.
 
-[![PyPI](https://img.shields.io/pypi/v/flow-py-sdk.svg)](https://pypi.org/project/flow-py-sdk/)
-[![codecov](https://codecov.io/gh/janezpodhostnik/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)
+[![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/)
+[![codecov](https://codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)
 
 
 See the [guide](https://janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)!
 
 
 Note: This SDK is also fully compatible with the Flow Emulator and can be used for local development.
 
 ## Installing
 
 To start using the SDK, install Python 3.7 or higher and install package:
 
 ```sh
-pip install flow-py-sdk
+pip install flow-py-sdk-legacy
 ```
 
 or if using poetry:
 
 ```sh
-poetry add flow-py-sdk
+poetry add flow-py-sdk-legacy
 ```
 
 ## Contributors
 
-<a href="https://github.com/janezpodhostnik/flow-py-sdk/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=janezpodhostnik/flow-py-sdk" />
+<a href="https://github.com/justinnout/flow-py-sdk/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=justinnout/flow-py-sdk" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 The Flow Python SDK provides a set of packages for Python developers to build
 applications that interact with the Flow network. [![PyPI](https://
-img.shields.io/pypi/v/flow-py-sdk.svg)](https://pypi.org/project/flow-py-sdk/)
-[![codecov](https://codecov.io/gh/janezpodhostnik/flow-py-sdk/branch/master/
-graph/badge.svg)](https://codecov.io/gh/codecov/example-go) See the [guide]
-(https://janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)! Note: This
-SDK is also fully compatible with the Flow Emulator and can be used for local
-development. ## Installing To start using the SDK, install Python 3.7 or higher
-and install package: ```sh pip install flow-py-sdk ``` or if using poetry:
-```sh poetry add flow-py-sdk ``` ## Contributors [https://contrib.rocks/
-image?repo=janezpodhostnik/flow-py-sdk] Made with [contrib.rocks](https://
-contrib.rocks).
+img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/project/flow-
+py-sdk-legacy/) [![codecov](https://codecov.io/gh/justinnout/flow-py-sdk/
+branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go) See
+the [guide](https://janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)!
+Note: This SDK is also fully compatible with the Flow Emulator and can be used
+for local development. ## Installing To start using the SDK, install Python 3.7
+or higher and install package: ```sh pip install flow-py-sdk-legacy ``` or if
+using poetry: ```sh poetry add flow-py-sdk-legacy ``` ## Contributors [https://
+contrib.rocks/image?repo=justinnout/flow-py-sdk] Made with [contrib.rocks]
+(https://contrib.rocks).
```

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/account_key.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/account_key.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/__init__.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/address.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/address.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/composite.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/composite.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/constants.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/constants.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/decode.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/decode.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/encode.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/encode.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/kind.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/kind.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/kinds.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/kinds.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/simple_kinds.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/simple_kinds.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/types.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/types.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/cadence/value.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/cadence/value.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/client/client.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/client/client.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/client/entities.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/client/entities.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/exceptions.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/access/__init__.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/access/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/access.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/access.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/entities/__init__.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/entities.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/entities.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/execution/__init__.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/proto/flow/execution.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/proto/flow/execution.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/script.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/script.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/hash_algo.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/hash_algo.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/in_memory_signer.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/in_memory_signer.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/in_memory_verifier.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/in_memory_verifier.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/sign_algo.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/sign_algo.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/signer.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/signer.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/signer/verifier.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/signer/verifier.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/templates.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/templates.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/tx.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/tx.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/flow_py_sdk/utils/verify_user_signature.py` & `flow_py_sdk_legacy-1.0.0/flow_py_sdk/utils/verify_user_signature.py`

 * *Files identical despite different names*

### Comparing `flow_py_sdk_legacy-0.0.0/pyproject.toml` & `flow_py_sdk_legacy-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow-py-sdk-legacy"
-version = "0.0.0"
+version = "1.0.0"
 description = "A python SDK for the flow blockchain"
 authors = ["Janez Podhostnik <janez.podhostnik@gmail.com>", "justin.kc.herrera@gmail.com"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/justinnout/flow-py-sdk"
 packages = [
     { include = "flow_py_sdk" },
@@ -25,15 +25,15 @@
 pytest = "^7.2"
 mkdocs = "^1.4"
 mkdocs-material = "^9.0"
 mkdocstrings = "^0.20"
 coverage = "^7.1"
 
 [tool.poetry-dynamic-versioning]
-enable = true
+enable = false
 vcs = "git"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `flow_py_sdk_legacy-0.0.0/PKG-INFO` & `flow_py_sdk_legacy-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow-py-sdk-legacy
-Version: 0.0.0
+Version: 1.0.0
 Summary: A python SDK for the flow blockchain
 Home-page: https://github.com/justinnout/flow-py-sdk
 License: MIT
 Author: Janez Podhostnik
 Author-email: janez.podhostnik@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,37 +20,37 @@
 Requires-Dist: grpclib (>=0.4,<0.5)
 Requires-Dist: rlp (>=3.0,<4.0)
 Project-URL: Repository, https://github.com/justinnout/flow-py-sdk
 Description-Content-Type: text/markdown
 
 The Flow Python SDK provides a set of packages for Python developers to build applications that interact with the Flow network.
 
-[![PyPI](https://img.shields.io/pypi/v/flow-py-sdk.svg)](https://pypi.org/project/flow-py-sdk/)
-[![codecov](https://codecov.io/gh/janezpodhostnik/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)
+[![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)](https://pypi.org/project/flow-py-sdk-legacy/)
+[![codecov](https://codecov.io/gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/codecov/example-go)
 
 
 See the [guide](https://janezpodhostnik.github.io/flow-py-sdk/python_SDK_guide/)!
 
 
 Note: This SDK is also fully compatible with the Flow Emulator and can be used for local development.
 
 ## Installing
 
 To start using the SDK, install Python 3.7 or higher and install package:
 
 ```sh
-pip install flow-py-sdk
+pip install flow-py-sdk-legacy
 ```
 
 or if using poetry:
 
 ```sh
-poetry add flow-py-sdk
+poetry add flow-py-sdk-legacy
 ```
 
 ## Contributors
 
-<a href="https://github.com/janezpodhostnik/flow-py-sdk/graphs/contributors">
-  <img src="https://contrib.rocks/image?repo=janezpodhostnik/flow-py-sdk" />
+<a href="https://github.com/justinnout/flow-py-sdk/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=justinnout/flow-py-sdk" />
 </a>
 
 Made with [contrib.rocks](https://contrib.rocks).
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: flow-py-sdk-legacy Version: 0.0.0 Summary: A python
+Metadata-Version: 2.1 Name: flow-py-sdk-legacy Version: 1.0.0 Summary: A python
 SDK for the flow blockchain Home-page: https://github.com/justinnout/flow-py-
 sdk License: MIT Author: Janez Podhostnik Author-email:
 janez.podhostnik@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: betterproto[compiler] (==v2.0.0-
 beta5) Requires-Dist: ecdsa (>=v0.18,<0.19) Requires-Dist: grpcio-tools
 (>=1.51,<2.0) Requires-Dist: grpclib (>=0.4,<0.5) Requires-Dist: rlp
 (>=3.0,<4.0) Project-URL: Repository, https://github.com/justinnout/flow-py-sdk
 Description-Content-Type: text/markdown The Flow Python SDK provides a set of
 packages for Python developers to build applications that interact with the
-Flow network. [![PyPI](https://img.shields.io/pypi/v/flow-py-sdk.svg)](https://
-pypi.org/project/flow-py-sdk/) [![codecov](https://codecov.io/gh/
-janezpodhostnik/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/
+Flow network. [![PyPI](https://img.shields.io/pypi/v/flow-py-sdk-legacy.svg)]
+(https://pypi.org/project/flow-py-sdk-legacy/) [![codecov](https://codecov.io/
+gh/justinnout/flow-py-sdk/branch/master/graph/badge.svg)](https://codecov.io/
 gh/codecov/example-go) See the [guide](https://janezpodhostnik.github.io/flow-
 py-sdk/python_SDK_guide/)! Note: This SDK is also fully compatible with the
 Flow Emulator and can be used for local development. ## Installing To start
 using the SDK, install Python 3.7 or higher and install package: ```sh pip
-install flow-py-sdk ``` or if using poetry: ```sh poetry add flow-py-sdk ``` ##
-Contributors [https://contrib.rocks/image?repo=janezpodhostnik/flow-py-sdk]
-Made with [contrib.rocks](https://contrib.rocks).
+install flow-py-sdk-legacy ``` or if using poetry: ```sh poetry add flow-py-
+sdk-legacy ``` ## Contributors [https://contrib.rocks/image?repo=justinnout/
+flow-py-sdk] Made with [contrib.rocks](https://contrib.rocks).
```

