# Comparing `tmp/safe-eth-py-5.1.0.tar.gz` & `tmp/safe-eth-py-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-eth-py-5.1.0.tar", last modified: Wed Mar  8 17:13:33 2023, max compression
+gzip compressed data, was "safe-eth-py-5.2.0.tar", last modified: Mon Apr 17 11:23:21 2023, max compression
```

## Comparing `safe-eth-py-5.1.0.tar` & `safe-eth-py-5.2.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.362936 safe-eth-py-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-08 17:13:33.362936 safe-eth-py-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.322935 safe-eth-py-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.326935 safe-eth-py-5.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.eth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/gnosis.safe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.326935 safe-eth-py-5.1.0/gnosis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.326935 safe-eth-py-5.1.0/gnosis/eth/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.330936 safe-eth-py-5.1.0/gnosis/eth/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.338935 safe-eth-py-5.1.0/gnosis/eth/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.342936 safe-eth-py-5.1.0/gnosis/eth/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.342936 safe-eth-py-5.1.0/gnosis/eth/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/django/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.342936 safe-eth-py-5.1.0/gnosis/eth/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81674 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/ethereum_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.342936 safe-eth-py-5.1.0/gnosis/eth/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.346936 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/makerdao.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.346936 safe-eth-py-5.1.0/gnosis/eth/oracles/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)    32311 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.346936 safe-eth-py-5.1.0/gnosis/eth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.350936 safe-eth-py-5.1.0/gnosis/eth/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.350936 safe-eth-py-5.1.0/gnosis/eth/tests/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.350936 safe-eth-py-5.1.0/gnosis/eth/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)   753187 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    92731 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)   169556 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.354936 safe-eth-py-5.1.0/gnosis/eth/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    71326 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/eth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.354936 safe-eth-py-5.1.0/gnosis/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/protocol/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.354936 safe-eth-py-5.1.0/gnosis/protocol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.358936 safe-eth-py-5.1.0/gnosis/safe/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.358936 safe-eth-py-5.1.0/gnosis/safe/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/api/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    42010 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.358936 safe-eth-py-5.1.0/gnosis/safe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.358936 safe-eth-py-5.1.0/gnosis/safe/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.358936 safe-eth-py-5.1.0/gnosis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/gnosis/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:33.362936 safe-eth-py-5.1.0/safe_eth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-08 17:13:33.000000 safe-eth-py-5.1.0/safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-03-08 17:13:33.000000 safe-eth-py-5.1.0/safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 17:13:33.000000 safe-eth-py-5.1.0/safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-08 17:13:33.000000 safe-eth-py-5.1.0/safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-08 17:13:33.000000 safe-eth-py-5.1.0/safe_eth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-08 17:13:33.362936 safe-eth-py-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-08 17:13:15.000000 safe-eth-py-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.665265 safe-eth-py-5.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.665265 safe-eth-py-5.2.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.665265 safe-eth-py-5.2.0/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.665265 safe-eth-py-5.2.0/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.669265 safe-eth-py-5.2.0/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.677264 safe-eth-py-5.2.0/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.677264 safe-eth-py-5.2.0/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.677264 safe-eth-py-5.2.0/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.677264 safe-eth-py-5.2.0/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81858 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.677264 safe-eth-py-5.2.0/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.681264 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/makerdao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.681264 safe-eth-py-5.2.0/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32311 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.681264 safe-eth-py-5.2.0/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.681264 safe-eth-py-5.2.0/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.681264 safe-eth-py-5.2.0/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.685264 safe-eth-py-5.2.0/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   753187 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92731 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169556 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.685264 safe-eth-py-5.2.0/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71326 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.685264 safe-eth-py-5.2.0/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.685264 safe-eth-py-5.2.0/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23606 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42010 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32576 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:23:21.689264 safe-eth-py-5.2.0/safe_eth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-04-17 11:23:21.000000 safe-eth-py-5.2.0/safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-17 11:23:21.000000 safe-eth-py-5.2.0/safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:23:21.000000 safe-eth-py-5.2.0/safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 11:23:21.000000 safe-eth-py-5.2.0/safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 11:23:21.000000 safe-eth-py-5.2.0/safe_eth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-17 11:23:21.693264 safe-eth-py-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 11:23:07.000000 safe-eth-py-5.2.0/setup.py
```

### Comparing `safe-eth-py-5.1.0/LICENSE` & `safe-eth-py-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/PKG-INFO` & `safe-eth-py-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.1.0
+Version: 5.2.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.1.0/README.rst` & `safe-eth-py-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/Makefile` & `safe-eth-py-5.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/make.bat` & `safe-eth-py-5.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/conf.py` & `safe-eth-py-5.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/gnosis.eth.clients.rst` & `safe-eth-py-5.2.0/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/gnosis.eth.django.rst` & `safe-eth-py-5.2.0/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/gnosis.eth.oracles.abis.rst` & `safe-eth-py-5.2.0/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/gnosis.eth.rst` & `safe-eth-py-5.2.0/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/gnosis.safe.rst` & `safe-eth-py-5.2.0/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/index.rst` & `safe-eth-py-5.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/docs/source/quickstart.rst` & `safe-eth-py-5.2.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/__init__.py` & `safe-eth-py-5.2.0/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/clients/__init__.py` & `safe-eth-py-5.2.0/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/clients/blockscout_client.py` & `safe-eth-py-5.2.0/gnosis/eth/clients/blockscout_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         EthereumNetwork.EVMOS_TESTNET: "https://evm.evmos.dev",
         EthereumNetwork.RABBIT_ANALOG_TESTNET_CHAIN: "https://rabbit.analogscan.com",
         EthereumNetwork.KCC_MAINNET: "https://scan.kcc.io/",
         EthereumNetwork.KCC_TESTNET: "https://scan-testnet.kcc.network/",
         EthereumNetwork.ARBITRUM_ONE: "https://explorer.arbitrum.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://nova-explorer.arbitrum.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://goerli-rollup-explorer.arbitrum.io",
+        EthereumNetwork.CROSSBELL: "https://scan.crossbell.io",
     }
 
     def __init__(self, network: EthereumNetwork):
         self.network = network
         self.base_url = self.NETWORK_WITH_URL.get(network)
         if self.base_url is None:
             raise BlockScoutConfigurationProblem(
```

### Comparing `safe-eth-py-5.1.0/gnosis/eth/clients/etherscan_client.py` & `safe-eth-py-5.2.0/gnosis/eth/clients/etherscan_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,48 +26,52 @@
         EthereumNetwork.MAINNET: "https://etherscan.io",
         EthereumNetwork.RINKEBY: "https://rinkeby.etherscan.io",
         EthereumNetwork.ROPSTEN: "https://ropsten.etherscan.io",
         EthereumNetwork.GOERLI: "https://goerli.etherscan.io",
         EthereumNetwork.KOVAN: "https://kovan.etherscan.io",
         EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: "https://bscscan.com",
         EthereumNetwork.POLYGON: "https://polygonscan.com",
+        EthereumNetwork.POLYGON_ZKEVM: "https://zkevm.polygonscan.com",
         EthereumNetwork.OPTIMISM: "https://optimistic.etherscan.io",
         EthereumNetwork.ARBITRUM_ONE: "https://arbiscan.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://nova.arbiscan.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://goerli.arbiscan.io",
         EthereumNetwork.AVALANCHE_C_CHAIN: "https://snowtrace.io",
         EthereumNetwork.MOONBEAM: "https://moonscan.io",
         EthereumNetwork.MOONRIVER: "https://moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://goerli.basescan.org",
+        EthereumNetwork.NEON_EVM_DEVNET: "https://neonscan.org",
     }
 
     NETWORK_WITH_API_URL = {
         EthereumNetwork.MAINNET: "https://api.etherscan.io",
         EthereumNetwork.RINKEBY: "https://api-rinkeby.etherscan.io",
         EthereumNetwork.ROPSTEN: "https://api-ropsten.etherscan.io",
         EthereumNetwork.GOERLI: "https://api-goerli.etherscan.io",
         EthereumNetwork.KOVAN: "https://api-kovan.etherscan.io",
         EthereumNetwork.BINANCE_SMART_CHAIN_MAINNET: "https://api.bscscan.com",
         EthereumNetwork.POLYGON: "https://api.polygonscan.com",
+        EthereumNetwork.POLYGON_ZKEVM: "https://api-zkevm.polygonscan.com",
         EthereumNetwork.OPTIMISM: "https://api-optimistic.etherscan.io",
         EthereumNetwork.ARBITRUM_ONE: "https://api.arbiscan.io",
         EthereumNetwork.ARBITRUM_NOVA: "https://api-nova.arbiscan.io",
         EthereumNetwork.ARBITRUM_GOERLI: "https://api-goerli.arbiscan.io",
         EthereumNetwork.AVALANCHE_C_CHAIN: "https://api.snowtrace.io",
         EthereumNetwork.MOONBEAM: "https://api-moonbeam.moonscan.io",
         EthereumNetwork.MOONRIVER: "https://api-moonriver.moonscan.io",
         EthereumNetwork.MOONBASE_ALPHA: "https://api-moonbase.moonscan.io",
         EthereumNetwork.CRONOS_MAINNET_BETA: "https://api.cronoscan.com",
         EthereumNetwork.CRONOS_TESTNET: "https://api-testnet.cronoscan.com",
         EthereumNetwork.CELO_MAINNET: "https://api.celoscan.io",
         EthereumNetwork.BASE_GOERLI_TESTNET: "https://api-goerli.basescan.org",
+        EthereumNetwork.NEON_EVM_DEVNET: "https://devnet-api.neonscan.org",
     }
     HTTP_HEADERS = {
         "User-Agent": "curl/7.77.0",
     }
 
     def __init__(self, network: EthereumNetwork, api_key: Optional[str] = None):
         self.network = network
```

### Comparing `safe-eth-py-5.1.0/gnosis/eth/clients/sourcify.py` & `safe-eth-py-5.2.0/gnosis/eth/clients/sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/constants.py` & `safe-eth-py-5.2.0/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/CPKFactory.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/DelegateConstructorProxy.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/ERC1155.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/ERC20.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/ERC20TestToken.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/ERC721.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/MultiSend.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/PayingProxy.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/Proxy_V1_0_0.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/Proxy_V1_1_1.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/Proxy_V1_3_0.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/__init__.py` & `safe-eth-py-5.2.0/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/kyber_network_proxy.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_exchange.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_factory.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_v2_factory.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_v2_pair.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/contracts/uniswap_v2_router.json` & `safe-eth-py-5.2.0/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/admin.py` & `safe-eth-py-5.2.0/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/forms.py` & `safe-eth-py-5.2.0/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/models.py` & `safe-eth-py-5.2.0/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/serializers.py` & `safe-eth-py-5.2.0/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/tests/models.py` & `safe-eth-py-5.2.0/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/tests/test_forms.py` & `safe-eth-py-5.2.0/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/tests/test_models.py` & `safe-eth-py-5.2.0/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/django/tests/test_serializers.py` & `safe-eth-py-5.2.0/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/eip712/__init__.py` & `safe-eth-py-5.2.0/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/ethereum_client.py` & `safe-eth-py-5.2.0/gnosis/eth/ethereum_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1403,18 +1403,19 @@
         """
         :return: RPC version information
         """
         return self.w3.clientVersion
 
     def get_network(self) -> EthereumNetwork:
         """
-        Get network name based on the chainId
+        Get network name based on the chainId. This method is not cached as the method for getting the
+        `chainId` already is.
 
         :return: EthereumNetwork based on the chainId. If network is not
-            on our list, `EthereumNetwork.UNKOWN` is returned
+            on our list, `EthereumNetwork.UNKNOWN` is returned
         """
         return EthereumNetwork(self.get_chain_id())
 
     @cache
     def is_eip1559_supported(self) -> EthereumNetwork:
         """
         :return: `True` if EIP1559 is supported by the node, `False` otherwise
@@ -1529,14 +1530,15 @@
             if data:
                 tx: TxParams = {
                     "from": deployer_account.address,
                     "data": data,
                     "gasPrice": self.w3.eth.gas_price,
                     "value": Wei(0),
                     "to": contract_address if contract_address else "",
+                    "chainId": self.get_chain_id(),
                 }
                 tx["gas"] = self.w3.eth.estimate_gas(tx)
                 tx_hash = self.send_unsigned_transaction(
                     tx, private_key=deployer_account.key
                 )
                 if check_receipt:
                     tx_receipt = self.get_transaction_receipt(
@@ -1938,14 +1940,15 @@
 
         tx: TxParams = {
             "from": account.address,
             "to": to,
             "value": value,
             "gas": gas or Wei(self.estimate_gas(to, account.address, value)),
             "gasPrice": Wei(gas_price),
+            "chainId": self.get_chain_id(),
         }
 
         if nonce is not None:
             tx["nonce"] = Nonce(nonce)
 
         return self.send_unsigned_transaction(
             tx, private_key=private_key, retry=retry, block_identifier=block_identifier
```

### Comparing `safe-eth-py-5.1.0/gnosis/eth/ethereum_network.py` & `safe-eth-py-5.2.0/gnosis/eth/ethereum_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,14 +264,15 @@
     BITTORRENT_CHAIN_TESTNET = 1028
     CONFLUX_ESPACE = 1030
     PROXY_NETWORK_TESTNET = 1031
     BRONOS_TESTNET = 1038
     BRONOS_MAINNET = 1039
     METIS_ANDROMEDA_MAINNET = 1088
     MOAC_MAINNET = 1099
+    POLYGON_ZKEVM = 1101
     WEMIX3_0_MAINNET = 1111
     WEMIX3_0_TESTNET = 1112
     CORE_BLOCKCHAIN_MAINNET = 1116
     DEFICHAIN_EVM_NETWORK_MAINNET = 1130
     DEFICHAIN_EVM_NETWORK_TESTNET = 1131
     MATHCHAIN = 1139
     MATHCHAIN_TESTNET = 1140
```

### Comparing `safe-eth-py-5.1.0/gnosis/eth/exceptions.py` & `safe-eth-py-5.2.0/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/multicall.py` & `safe-eth-py-5.2.0/gnosis/eth/multicall.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         EthereumNetwork.MUMBAI: "0xed386Fe855C1EFf2f843B910923Dd8846E45C5A4",
         EthereumNetwork.OPTIMISM: "0x2DC0E2aa608532Da689e89e237dF582B783E552C",
         EthereumNetwork.RINKEBY: "0x5BA1e12693Dc8F9c48aAD8770482f4739bEeD696",
         EthereumNetwork.ROPSTEN: "0x5BA1e12693Dc8F9c48aAD8770482f4739bEeD696",
         EthereumNetwork.GNOSIS: "0x08612d3C4A5Dfe2FaaFaFe6a4ff712C2dC675bF7",
         EthereumNetwork.KCC_MAINNET: "0x7C1C85C39d3D6b6ecB811dfe949B9C23f6E818B0",
         EthereumNetwork.KCC_TESTNET: "0x665683D9bd41C09cF38c3956c926D9924F1ADa97",
+        EthereumNetwork.POLYGON_ZKEVM: "0xcA11bde05977b3631167028862bE2a173976CA11",
     }
 
     def __init__(
         self,
         ethereum_client: EthereumClient,
         multicall_contract_address: Optional[ChecksumAddress] = None,
     ):
```

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/__init__.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/aave_abis.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/balancer_abis.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/cream_abis.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/curve_abis.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/makerdao.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/makerdao.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/mooniswap_abis.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/uniswap_v3.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/yearn_abis.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/abis/zerion_abis.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/cowswap.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/kyber.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/oracles.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/superfluid.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/sushiswap.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/uniswap_v3.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/oracles/utils.py` & `safe-eth-py-5.2.0/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/clients/mocks.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/clients/test_blockscout_client.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/clients/test_etherscan_client.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/clients/test_sourcify.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/eip712/test_eip712.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/ethereum_test_case.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_internal_txs.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_log_receipts.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_trace_block.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_trace_filter.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_cowswap.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,32 +54,24 @@
             usdc_token_mainnet_address, dai_token_mainnet_address
         )
         self.assertAlmostEqual(price, 1.0, delta=0.5)
 
         with mock.patch.object(
             Session, "post", side_effect=IOError("Connection Error")
         ):
-            with self.assertRaisesMessage(
-                CannotGetPriceFromOracle,
-                f"Cannot get price from CowSwap "
-                f"{{}} "
-                f"for token-1={usdc_token_mainnet_address} to token-2={dai_token_mainnet_address}",
-            ):
+            with self.assertRaises(CannotGetPriceFromOracle):
                 cowswap_oracle.get_price(
                     usdc_token_mainnet_address, dai_token_mainnet_address
                 )
 
         random_token = Account.create().address
         with self.assertRaisesMessage(
             CannotGetPriceFromOracle,
             f"Cannot get decimals for token={random_token}",
         ):
             cowswap_oracle.get_price(random_token)
 
         with mock.patch(
             "gnosis.eth.oracles.cowswap.get_decimals", autospec=True, return_value=18
         ):
-            with self.assertRaisesMessage(
-                CannotGetPriceFromOracle,
-                f"Cannot get price from CowSwap {{'errorType': 'UnsupportedToken', 'description': 'Token {random_token.lower()} is unsupported: Could not find on chain source of the token with at least {{MIN_AMOUNT}} balance.'}} for token-1={random_token} to token-2={weth_token_mainnet_address}",
-            ):
+            with self.assertRaises(CannotGetPriceFromOracle):
                 cowswap_oracle.get_price(random_token)
```

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_kyber.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_superfluid.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_sushiswap.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/test_ethereum_client.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/test_multicall.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/test_oracles.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/test_utils.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/tests/utils.py` & `safe-eth-py-5.2.0/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/eth/utils.py` & `safe-eth-py-5.2.0/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/protocol/gnosis_protocol_api.py` & `safe-eth-py-5.2.0/gnosis/protocol/gnosis_protocol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,21 @@
         self.http_session = requests.Session()
 
     @cached_property
     def weth_address(self) -> ChecksumAddress:
         """
         :return: Wrapped ether checksummed address
         """
-        if self.network == EthereumNetwork.MAINNET:
-            return ChecksumAddress("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2")
-        elif self.network == EthereumNetwork.RINKEBY:
-            return ChecksumAddress("0xc778417E063141139Fce010982780140Aa0cD5Ab")
-        else:  # XDAI
-            return ChecksumAddress("0x6A023CCd1ff6F2045C3309768eAd9E68F978f6e1")
+        if self.network == EthereumNetwork.GNOSIS:  # WXDAI
+            return ChecksumAddress("0xe91D153E0b41518A2Ce8Dd3D7944Fa863463a97d")
+        if self.network == EthereumNetwork.GOERLI:  # Goerli WETH9
+            return ChecksumAddress("0xB4FBF271143F4FBf7B91A5ded31805e42b2208d6")
+
+        # Mainnet WETH9
+        return ChecksumAddress("0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2")
 
     def get_quote(
         self, order: Order, from_address: ChecksumAddress
     ) -> Union[Dict[str, Any], ErrorResponse]:
         url = self.base_url + "quote"
         data_json = {
             "sellToken": order.sellToken.lower(),
@@ -125,17 +126,18 @@
             order.buyAmount and order.sellAmount
         ), "Order buyAmount and sellAmount cannot be empty"
 
         url = self.base_url + "orders/"
         from_address = Account.from_key(private_key).address
         if not order.feeAmount:
             fee_amount = self.get_fee(order, from_address)
-            if "errorType" in fee_amount:  # ErrorResponse
+            if isinstance(fee_amount, int):
+                order.feeAmount = fee_amount
+            elif "errorType" in fee_amount:  # ErrorResponse
                 return fee_amount
-            order.feeAmount = fee_amount
 
         signable_hash = eip712_encode_hash(
             order.get_eip712_structured_data(
                 self.network.value, self.settlement_contract_address
             )
         )
         message = encode_defunct(primitive=signable_hash)
```

### Comparing `safe-eth-py-5.1.0/gnosis/protocol/order.py` & `safe-eth-py-5.2.0/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `safe-eth-py-5.2.0/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,10 +149,12 @@
         order_id = self.goerli_gnosis_protocol_api.place_order(
             order, Account().create().key
         )
 
         if type(order_id) is dict:
             if order_id["errorType"] == "NoLiquidity":
                 pytest.xfail("NoLiquidity Error")
+            elif order_id["errorType"] == "InsufficientBalance":
+                pytest.xfail("InsufficientBalance")
 
         self.assertEqual(order_id[:2], "0x")
         self.assertEqual(len(order_id), 114)
```

### Comparing `safe-eth-py-5.1.0/gnosis/safe/__init__.py` & `safe-eth-py-5.2.0/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/addresses.py` & `safe-eth-py-5.2.0/gnosis/safe/addresses.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         ("0x6851D6fDFAfD08c0295C392436245E5bc78B0185", 6876086, "1.2.0"),
         ("0x34CfAC646f301356fAa8B21e94227e3583Fe3F5F", 6876642, "1.1.1"),
     ],
     EthereumNetwork.POLYGON: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 14306478, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 14306478, "1.3.0"),
     ],
+    EthereumNetwork.POLYGON_ZKEVM: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 79000, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 79000, "1.3.0"),
+    ],
     EthereumNetwork.MUMBAI: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 13736914, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 13736914, "1.3.0"),
     ],
     EthereumNetwork.ARBITRUM_ONE: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 1146, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1140, "1.3.0"),
@@ -252,14 +256,42 @@
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 42293309, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 42293315, "1.3.0"),
     ],
     EthereumNetwork.BASE_GOERLI_TESTNET: [
         ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 938848, "1.3.0+L2"),
         ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 939064, "1.3.0"),
     ],
+    EthereumNetwork.KAVA_EVM: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 2116303, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 2116307, "1.3.0"),
+    ],
+    EthereumNetwork.CROSSBELL: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 28314790, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 28314796, "1.3.0"),
+    ],
+    EthereumNetwork.IOTEX_NETWORK_MAINNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 22172521, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 22172524, "1.3.0"),
+    ],
+    EthereumNetwork.VELAS_EVM_MAINNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 27572492, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 27572642, "1.3.0"),
+    ],
+    EthereumNetwork.VELAS_EVM_TESTNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 27572492, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 27572642, "1.3.0"),
+    ],
+    EthereumNetwork.WEMIX3_0_MAINNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 12651754, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 12651757, "1.3.0"),
+    ],
+    EthereumNetwork.WEMIX3_0_TESTNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 20834033, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 20834039, "1.3.0"),
+    ],
 }
 
 PROXY_FACTORIES: Dict[EthereumNetwork, List[Tuple[str, int]]] = {
     EthereumNetwork.MAINNET: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 12504126),  # v1.3.0
         ("0x76E2cFc1F5Fa8F6a5b3fC4c8F4788F0116861F9B", 9084508),  # v1.1.1
         ("0x50e55Af101C777bA7A1d560a774A82eF002ced9F", 8915731),  # v1.1.0
@@ -298,14 +330,17 @@
     ],
     EthereumNetwork.POLYGON: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 14306478),  # v1.3.0
     ],
     EthereumNetwork.MUMBAI: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 13736914),  # v1.3.0
     ],
+    EthereumNetwork.POLYGON_ZKEVM: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 79000),  # v1.3.0
+    ],
     EthereumNetwork.ARBITRUM_ONE: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 1140),  # v1.3.0
     ],
     EthereumNetwork.ARBITRUM_NOVA: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 419),  # v1.3.0
     ],
     EthereumNetwork.ARBITRUM_RINKEBY: [
@@ -439,8 +474,29 @@
     ],
     EthereumNetwork.XDC_APOTHEM_NETWORK: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 42293264),  # v1.3.0
     ],
     EthereumNetwork.BASE_GOERLI_TESTNET: [
         ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 938848),  # v1.3.0
     ],
+    EthereumNetwork.KAVA_EVM: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 2116356),  # v1.3.0
+    ],
+    EthereumNetwork.CROSSBELL: [
+        ("0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2", 28314747),  # v1.3.0
+    ],
+    EthereumNetwork.IOTEX_NETWORK_MAINNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 22172504),  # v1.3.0
+    ],
+    EthereumNetwork.VELAS_EVM_MAINNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 27571962),  # v1.3.0
+    ],
+    EthereumNetwork.VELAS_EVM_TESTNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 27571962),  # v1.3.0
+    ],
+    EthereumNetwork.WEMIX3_0_MAINNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 12651730),  # v1.3.0
+    ],
+    EthereumNetwork.WEMIX3_0_TESTNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 20833988),  # v1.3.0
+    ],
 }
```

### Comparing `safe-eth-py-5.1.0/gnosis/safe/api/base_api.py` & `safe-eth-py-5.2.0/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/api/relay_service_api.py` & `safe-eth-py-5.2.0/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/api/transaction_service_api.py` & `safe-eth-py-5.2.0/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/exceptions.py` & `safe-eth-py-5.2.0/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/multi_send.py` & `safe-eth-py-5.2.0/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/proxy_factory.py` & `safe-eth-py-5.2.0/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/safe.py` & `safe-eth-py-5.2.0/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/safe_create2_tx.py` & `safe-eth-py-5.2.0/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/safe_creation_tx.py` & `safe-eth-py-5.2.0/gnosis/safe/safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/safe_signature.py` & `safe-eth-py-5.2.0/gnosis/safe/safe_signature.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,16 @@
             try:
                 return (
                     safe_contract.functions.approvedHashes(
                         self.owner, self.safe_tx_hash
                     ).call(block_identifier=block_identifier)
                     == 1
                 )
-            except BadFunctionCallOutput as e:  # Error using `pending` block identifier
+            except (ValueError, BadFunctionCallOutput, DecodingError) as e:
+                # Error using `pending` block identifier
                 exception = e
         raise exception  # This should never happen
 
 
 class SafeSignatureEthSign(SafeSignature):
     @property
     def owner(self):
```

### Comparing `safe-eth-py-5.1.0/gnosis/safe/safe_tx.py` & `safe-eth-py-5.2.0/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/serializers.py` & `safe-eth-py-5.2.0/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/signatures.py` & `safe-eth-py-5.2.0/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/api/test_transaction_service_api.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/safe_test_case.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_multi_send.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_proxy_factory.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_safe.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_create2_tx.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_creation_tx.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_signature.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_safe_tx.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_serializers.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/test_signatures.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/gnosis/safe/tests/utils.py` & `safe-eth-py-5.2.0/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/safe_eth_py.egg-info/PKG-INFO` & `safe-eth-py-5.2.0/safe_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.1.0
+Version: 5.2.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.1.0/safe_eth_py.egg-info/SOURCES.txt` & `safe-eth-py-5.2.0/safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.1.0/setup.cfg` & `safe-eth-py-5.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = safe-eth-py
-version = 5.1.0
+version = 5.2.0
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

