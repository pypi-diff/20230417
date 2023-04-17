# Comparing `tmp/ocean-lib-2.2.2.tar.gz` & `tmp/ocean-lib-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean-lib-2.2.2.tar", last modified: Fri Apr  7 11:53:17 2023, max compression
+gzip compressed data, was "ocean-lib-2.2.3.tar", last modified: Mon Apr 17 08:56:24 2023, max compression
```

## Comparing `ocean-lib-2.2.2.tar` & `ocean-lib-2.2.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.804018 ocean-lib-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-07 11:53:17.804018 ocean-lib-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.788018 ocean-lib-2.2.2/ocean_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.792018 ocean-lib-2.2.2/ocean_lib/agreements/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/agreements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/agreements/consumable.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/agreements/service_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.792018 ocean-lib-2.2.2/ocean_lib/aquarius/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/aquarius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/aquarius/aquarius.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.792018 ocean-lib-2.2.2/ocean_lib/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/assets/asset_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/assets/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/assets/ddo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.796018 ocean-lib-2.2.2/ocean_lib/data_provider/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/data_provider/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/data_provider/data_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/data_provider/data_service_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/data_provider/fileinfo_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/example_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.796018 ocean-lib-2.2.2/ocean_lib/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/http_requests/requests_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.796018 ocean-lib-2.2.2/ocean_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/compute_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/data_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/data_nft_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/datatoken1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/datatoken2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/datatoken_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.796018 ocean-lib-2.2.2/ocean_lib/models/df/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/df/df_rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/df/df_strategy_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/dispenser.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/erc721_token_factory_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/factory_router.py
--rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/fixed_rate_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.800018 ocean-lib-2.2.2/ocean_lib/models/ve/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/ve/smart_wallet_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/ve/ve_allocate.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/ve/ve_delegation.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/ve/ve_delegation_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/ve/ve_fee_distributor.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/ve/ve_fee_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/models/ve/ve_ocean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.800018 ocean-lib-2.2.2/ocean_lib/ocean/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/ocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/ocean/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/ocean/mint_fake_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/ocean/ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    28559 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/ocean/ocean_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/ocean/ocean_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/ocean/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.800018 ocean-lib-2.2.2/ocean_lib/services/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/services/consumer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/services/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.800018 ocean-lib-2.2.2/ocean_lib/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/structures/abi_tuples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/structures/algorithm_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/structures/file_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.804018 ocean-lib-2.2.2/ocean_lib/web3_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/web3_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/web3_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/web3_internal/contract_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/web3_internal/contract_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/ocean_lib/web3_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:53:17.792018 ocean-lib-2.2.2/ocean_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-07 11:53:17.000000 ocean-lib-2.2.2/ocean_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-07 11:53:17.000000 ocean-lib-2.2.2/ocean_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:53:17.000000 ocean-lib-2.2.2/ocean_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:53:17.000000 ocean-lib-2.2.2/ocean_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-07 11:53:17.000000 ocean-lib-2.2.2/ocean_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 11:53:17.000000 ocean-lib-2.2.2/ocean_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-07 11:53:17.804018 ocean-lib-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-07 11:53:06.000000 ocean-lib-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.446375 ocean-lib-2.2.3/ocean_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/agreements/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/agreements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/agreements/consumable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/agreements/service_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/aquarius/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/aquarius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/aquarius/aquarius.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/asset_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/assets/ddo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/data_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/data_service_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/data_provider/fileinfo_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/example_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/http_requests/requests_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/compute_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/data_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/data_nft_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/datatoken1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/datatoken2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/datatoken_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib/models/df/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/df/df_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/df/df_strategy_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/dispenser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/erc721_token_factory_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/factory_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16713 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/fixed_rate_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/models/ve/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/smart_wallet_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_allocate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_delegation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_delegation_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_fee_distributor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_fee_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/models/ve/ve_ocean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/ocean/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/mint_fake_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28533 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/ocean_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/ocean_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/ocean/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/services/consumer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/structures/abi_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/structures/algorithm_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/structures/file_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/ocean_lib/web3_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/contract_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/contract_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/ocean_lib/web3_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:56:24.450375 ocean-lib-2.2.3/ocean_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 08:56:24.000000 ocean-lib-2.2.3/ocean_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-17 08:56:24.454375 ocean-lib-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-17 08:56:12.000000 ocean-lib-2.2.3/setup.py
```

### Comparing `ocean-lib-2.2.2/LICENSE` & `ocean-lib-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/PKG-INFO` & `ocean-lib-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-lib
-Version: 2.2.2
+Version: 2.2.3
 Summary: 🐳 Ocean protocol library.
 Home-page: https://github.com/oceanprotocol/ocean.py
 Author: ocean-core-team
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Keywords: ocean-lib
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ocean-lib-2.2.2/README.md` & `ocean-lib-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/agreements/consumable.py` & `ocean-lib-2.2.3/ocean_lib/agreements/consumable.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/aquarius/aquarius.py` & `ocean-lib-2.2.3/ocean_lib/aquarius/aquarius.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/assets/asset_downloader.py` & `ocean-lib-2.2.3/ocean_lib/assets/asset_downloader.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/assets/credentials.py` & `ocean-lib-2.2.3/ocean_lib/assets/credentials.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/assets/ddo.py` & `ocean-lib-2.2.3/ocean_lib/assets/ddo.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/data_provider/base.py` & `ocean-lib-2.2.3/ocean_lib/data_provider/base.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/data_provider/data_encryptor.py` & `ocean-lib-2.2.3/ocean_lib/data_provider/data_encryptor.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/data_provider/data_service_provider.py` & `ocean-lib-2.2.3/ocean_lib/data_provider/data_service_provider.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/data_provider/fileinfo_provider.py` & `ocean-lib-2.2.3/ocean_lib/data_provider/fileinfo_provider.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/example_config.py` & `ocean-lib-2.2.3/ocean_lib/example_config.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/exceptions.py` & `ocean-lib-2.2.3/ocean_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/http_requests/requests_session.py` & `ocean-lib-2.2.3/ocean_lib/http_requests/requests_session.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/compute_input.py` & `ocean-lib-2.2.3/ocean_lib/models/compute_input.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/data_nft.py` & `ocean-lib-2.2.3/ocean_lib/models/data_nft.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/data_nft_factory.py` & `ocean-lib-2.2.3/ocean_lib/models/data_nft_factory.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/datatoken1.py` & `ocean-lib-2.2.3/ocean_lib/models/datatoken1.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/datatoken2.py` & `ocean-lib-2.2.3/ocean_lib/models/datatoken2.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/datatoken_base.py` & `ocean-lib-2.2.3/ocean_lib/models/datatoken_base.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/dispenser.py` & `ocean-lib-2.2.3/ocean_lib/models/dispenser.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/models/fixed_rate_exchange.py` & `ocean-lib-2.2.3/ocean_lib/models/fixed_rate_exchange.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/ocean/crypto.py` & `ocean-lib-2.2.3/ocean_lib/ocean/crypto.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/ocean/mint_fake_ocean.py` & `ocean-lib-2.2.3/ocean_lib/ocean/mint_fake_ocean.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/ocean/ocean.py` & `ocean-lib-2.2.3/ocean_lib/ocean/ocean.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/ocean/ocean_assets.py` & `ocean-lib-2.2.3/ocean_lib/ocean/ocean_assets.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     TokenFeeInfo,
 )
 from ocean_lib.models.dispenser import DispenserArguments
 from ocean_lib.models.fixed_rate_exchange import ExchangeArguments
 from ocean_lib.ocean.util import (
     create_checksum,
     get_address_of_type,
+    get_args_object,
     get_from_address,
     to_wei,
 )
 from ocean_lib.services.service import Service
 from ocean_lib.structures.algorithm_metadata import AlgorithmMetadata
 from ocean_lib.structures.file_objects import (
     ArweaveFile,
@@ -49,14 +50,36 @@
 )
 from ocean_lib.web3_internal.constants import ZERO_ADDRESS
 from ocean_lib.web3_internal.utils import check_network
 
 logger = logging.getLogger("ocean")
 
 
+class AssetArguments:
+    def __init__(
+        self,
+        wait_for_aqua: bool = True,
+        dt_template_index: Optional[int] = 1,
+        pricing_schema_args: Optional[
+            Union[DispenserArguments, ExchangeArguments]
+        ] = None,
+        metadata: Optional[dict] = None,
+        with_compute: Optional[bool] = False,
+        compute_values: Optional[dict] = None,
+        credentials: Optional[dict] = None,
+    ):
+        self.wait_for_aqua = wait_for_aqua
+        self.dt_template_index = dt_template_index
+        self.pricing_schema_args = pricing_schema_args
+        self.metadata = metadata
+        self.with_compute = with_compute
+        self.compute_values = compute_values
+        self.credentials = credentials if credentials else {"allow": [], "deny": []}
+
+
 class OceanAssets:
     """Ocean asset class for V4."""
 
     @enforce_types
     def __init__(self, config_dict, data_provider: Type[DataServiceProvider]) -> None:
         """Initialises OceanAssets object."""
         network_name = config_dict["NETWORK_NAME"]
@@ -169,155 +192,118 @@
         self,
         name: str,
         url: str,
         tx_dict: dict,
         image: str = "oceanprotocol/algo_dockers",
         tag: str = "python-branin",
         checksum: str = "sha256:8221d20c1c16491d7d56b9657ea09082c0ee4a8ab1a6621fa720da58b09580e4",
-        wait_for_aqua: bool = True,
-        dt_template_index: Optional[int] = 1,
-        pricing_schema_args: Optional[
-            Union[DispenserArguments, ExchangeArguments]
-        ] = None,
+        *args,
+        **kwargs,
     ) -> tuple:
         """Create asset of type "algorithm", having UrlFiles, with good defaults"""
 
         if image == "oceanprotocol/algo_dockers" or tag == "python-branin":
             assert image == "oceanprotocol/algo_dockers" and tag == "python-branin"
 
-        metadata = self._default_metadata(name, tx_dict, "algorithm")
-        metadata["algorithm"] = {
-            "language": "python",
-            "format": "docker-image",
-            "version": "0.1",
-            "container": {
-                "entrypoint": "python $ALGO",
-                "image": image,
-                "tag": tag,
-                "checksum": checksum,
-            },
-        }
+        asset_args = get_args_object(args, kwargs, AssetArguments)
+
+        if not asset_args.metadata:
+            metadata = OceanAssets.default_metadata(name, tx_dict, "algorithm")
+
+            metadata["algorithm"] = {
+                "language": "python",
+                "format": "docker-image",
+                "version": "0.1",
+                "container": {
+                    "entrypoint": "python $ALGO",
+                    "image": image,
+                    "tag": tag,
+                    "checksum": checksum,
+                },
+            }
+
+            asset_args.metadata = metadata
 
         files = [UrlFile(url)]
 
-        return self.create_bundled(
-            metadata,
-            files,
-            tx_dict,
-            wait_for_aqua=wait_for_aqua,
-            dt_template_index=dt_template_index,
-            pricing_schema_args=pricing_schema_args,
-        )
+        return self.create_bundled(files, tx_dict, asset_args)
 
     @enforce_types
     def create_url_asset(
         self,
         name: str,
         url: str,
         tx_dict: dict,
-        wait_for_aqua: bool = True,
-        dt_template_index: Optional[int] = 1,
-        pricing_schema_args: Optional[
-            Union[DispenserArguments, ExchangeArguments]
-        ] = None,
+        *args,
+        **kwargs,
     ) -> tuple:
         """Create asset of type "data", having UrlFiles, with good defaults"""
-        metadata = self._default_metadata(name, tx_dict)
+        asset_args = get_args_object(args, kwargs, AssetArguments)
+        if not asset_args.metadata:
+            asset_args.metadata = OceanAssets.default_metadata(name, tx_dict)
+
         files = [UrlFile(url)]
 
-        return self.create_bundled(
-            metadata,
-            files,
-            tx_dict,
-            wait_for_aqua=wait_for_aqua,
-            dt_template_index=dt_template_index,
-            pricing_schema_args=pricing_schema_args,
-        )
+        return self.create_bundled(files, tx_dict, asset_args)
 
     @enforce_types
     def create_arweave_asset(
-        self,
-        name: str,
-        transaction_id: str,
-        tx_dict: dict,
-        wait_for_aqua: bool = True,
-        dt_template_index: Optional[int] = 1,
-        pricing_schema_args: Optional[
-            Union[DispenserArguments, ExchangeArguments]
-        ] = None,
+        self, name: str, transaction_id: str, tx_dict: dict, *args, **kwargs
     ) -> tuple:
         """Create asset of type "data", having UrlFiles, with good defaults"""
-        metadata = self._default_metadata(name, tx_dict)
+        asset_args = get_args_object(args, kwargs, AssetArguments)
+        if not asset_args.metadata:
+            asset_args.metadata = OceanAssets.default_metadata(name, tx_dict)
+
         files = [ArweaveFile(transaction_id)]
 
-        return self.create_bundled(
-            metadata,
-            files,
-            tx_dict,
-            wait_for_aqua=wait_for_aqua,
-            dt_template_index=dt_template_index,
-            pricing_schema_args=pricing_schema_args,
-        )
+        return self.create_bundled(files, tx_dict, asset_args)
 
     @enforce_types
     def create_graphql_asset(
-        self,
-        name: str,
-        url: str,
-        query: str,
-        tx_dict: dict,
-        wait_for_aqua: bool = True,
-        dt_template_index: Optional[int] = 1,
-        pricing_schema_args: Optional[
-            Union[DispenserArguments, ExchangeArguments]
-        ] = None,
+        self, name: str, url: str, query: str, tx_dict: dict, *args, **kwargs
     ) -> tuple:
         """Create asset of type "data", having GraphqlQuery files, w good defaults"""
-        metadata = self._default_metadata(name, tx_dict)
+        asset_args = get_args_object(args, kwargs, AssetArguments)
+        if not asset_args.metadata:
+            asset_args.metadata = OceanAssets.default_metadata(name, tx_dict)
+
         files = [GraphqlQuery(url, query)]
 
-        return self.create_bundled(
-            metadata,
-            files,
-            tx_dict,
-            wait_for_aqua=wait_for_aqua,
-            dt_template_index=dt_template_index,
-            pricing_schema_args=pricing_schema_args,
-        )
+        return self.create_bundled(files, tx_dict, asset_args)
 
     @enforce_types
     def create_onchain_asset(
         self,
         name: str,
         contract_address: str,
         contract_abi: dict,
         tx_dict: dict,
         wait_for_aqua: bool = True,
         dt_template_index: Optional[int] = 1,
         pricing_schema_args: Optional[
             Union[DispenserArguments, ExchangeArguments]
         ] = None,
+        *args,
+        **kwargs,
     ) -> tuple:
         """Create asset of type "data", having SmartContractCall files, w defaults"""
         chain_id = self._chain_id
         onchain_data = SmartContractCall(contract_address, chain_id, contract_abi)
         files = [onchain_data]
-        metadata = self._default_metadata(name, tx_dict)
 
-        return self.create_bundled(
-            metadata,
-            files,
-            tx_dict,
-            wait_for_aqua=wait_for_aqua,
-            dt_template_index=dt_template_index,
-            pricing_schema_args=pricing_schema_args,
-        )
+        asset_args = get_args_object(args, kwargs, AssetArguments)
+        if not asset_args.metadata:
+            asset_args.metadata = OceanAssets.default_metadata(name, tx_dict)
+
+        return self.create_bundled(files, tx_dict, asset_args)
 
+    @classmethod
     @enforce_types
-    def _default_metadata(self, name: str, tx_dict: dict, type="dataset") -> dict:
+    def default_metadata(cls, name: str, tx_dict: dict, type="dataset") -> dict:
         address = get_from_address(tx_dict)
 
         date_created = datetime.now().isoformat()
         metadata = {
             "created": date_created,
             "updated": date_created,
             "description": name,
@@ -326,78 +312,78 @@
             "author": address[:7],
             "license": "CC0: PublicDomain",
         }
         return metadata
 
     @enforce_types
     def create_bundled(
-        self,
-        metadata: dict,
-        files: List[FilesType],
-        tx_dict: dict,
-        credentials: Optional[dict] = None,
-        wait_for_aqua: bool = True,
-        dt_template_index: Optional[int] = 1,
-        pricing_schema_args: Optional[
-            Union[DispenserArguments, ExchangeArguments]
-        ] = None,
+        self, files: List[FilesType], tx_dict: dict, asset_args: AssetArguments
     ):
         provider_uri = DataServiceProvider.get_url(self._config_dict)
 
-        self._assert_ddo_metadata(metadata)
-        name = metadata["name"]
+        self._assert_ddo_metadata(asset_args.metadata)
+        name = asset_args.metadata["name"]
         data_nft_args = DataNFTArguments(name, name)
 
-        if dt_template_index == 2:
+        if asset_args.dt_template_index == 2:
             datatoken_args = DatatokenArguments(
                 f"{name}: DT1", files=files, template_index=2, cap=to_wei(100)
             )
         else:
             datatoken_args = DatatokenArguments(f"{name}: DT1", files=files)
 
-        if not pricing_schema_args:
+        if not asset_args.pricing_schema_args:
             data_nft, datatoken = self.data_nft_factory.create_with_erc20(
                 data_nft_args, datatoken_args, tx_dict
             )
 
-        if isinstance(pricing_schema_args, DispenserArguments):
+        if isinstance(asset_args.pricing_schema_args, DispenserArguments):
             data_nft, datatoken = self.data_nft_factory.create_with_erc20_and_dispenser(
-                data_nft_args, datatoken_args, pricing_schema_args, tx_dict
+                data_nft_args, datatoken_args, asset_args.pricing_schema_args, tx_dict
             )
 
-        if isinstance(pricing_schema_args, ExchangeArguments):
+        if isinstance(asset_args.pricing_schema_args, ExchangeArguments):
             (
                 data_nft,
                 datatoken,
                 _,
             ) = self.data_nft_factory.create_with_erc20_and_fixed_rate(
-                data_nft_args, datatoken_args, pricing_schema_args, tx_dict
+                data_nft_args, datatoken_args, asset_args.pricing_schema_args, tx_dict
             )
 
         ddo = DDO()
         # Generate the did, add it to the ddo.
         ddo.did = data_nft.calculate_did()
         # Check if it's already registered first!
         if self._aquarius.ddo_exists(ddo.did):
             raise AquariusError(
                 f"Asset id {ddo.did} is already registered to another asset."
             )
 
         ddo.chain_id = self._chain_id
-        ddo.metadata = metadata
-        ddo.credentials = credentials if credentials else {"allow": [], "deny": []}
+        ddo.metadata = asset_args.metadata
+        ddo.credentials = asset_args.credentials
         ddo.nft_address = data_nft.address
 
         access_service = datatoken.build_access_service(
             service_id="0",
             service_endpoint=provider_uri,
             files=files,
         )
         ddo.add_service(access_service)
 
+        if asset_args.with_compute or asset_args.compute_values:
+            ddo.create_compute_service(
+                "1",
+                provider_uri,
+                datatoken.address,
+                files,
+                asset_args.compute_values,
+            )
+
         # Validation by Aquarius
         _, proof = self.validate(ddo)
         proof = (
             proof["publicKey"],
             proof["v"],
             proof["r"][0],
             proof["s"][0],
@@ -415,15 +401,15 @@
             document,
             ddo_hash,
             [proof],
             tx_dict,
         )
 
         # Fetch the ddo on chain
-        if wait_for_aqua:
+        if asset_args.wait_for_aqua:
             ddo = self._aquarius.wait_for_ddo(ddo.did)
 
         return (data_nft, datatoken, ddo)
 
     # Don't enforce types due to error:
     # TypeError: Subscripted generics cannot be used with class and instance checks
     def create(
```

### Comparing `ocean-lib-2.2.2/ocean_lib/ocean/ocean_compute.py` & `ocean-lib-2.2.3/ocean_lib/ocean/ocean_compute.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/ocean/util.py` & `ocean-lib-2.2.3/ocean_lib/ocean/util.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/services/consumer_parameters.py` & `ocean-lib-2.2.3/ocean_lib/services/consumer_parameters.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/services/service.py` & `ocean-lib-2.2.3/ocean_lib/services/service.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/structures/abi_tuples.py` & `ocean-lib-2.2.3/ocean_lib/structures/abi_tuples.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/structures/algorithm_metadata.py` & `ocean-lib-2.2.3/ocean_lib/structures/algorithm_metadata.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/structures/file_objects.py` & `ocean-lib-2.2.3/ocean_lib/structures/file_objects.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/web3_internal/contract_base.py` & `ocean-lib-2.2.3/ocean_lib/web3_internal/contract_base.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/web3_internal/contract_utils.py` & `ocean-lib-2.2.3/ocean_lib/web3_internal/contract_utils.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib/web3_internal/utils.py` & `ocean-lib-2.2.3/ocean_lib/web3_internal/utils.py`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib.egg-info/PKG-INFO` & `ocean-lib-2.2.3/ocean_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocean-lib
-Version: 2.2.2
+Version: 2.2.3
 Summary: 🐳 Ocean protocol library.
 Home-page: https://github.com/oceanprotocol/ocean.py
 Author: ocean-core-team
 Author-email: devops@oceanprotocol.com
 License: Apache Software License 2.0
 Keywords: ocean-lib
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ocean-lib-2.2.2/ocean_lib.egg-info/SOURCES.txt` & `ocean-lib-2.2.3/ocean_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocean-lib-2.2.2/ocean_lib.egg-info/requires.txt` & `ocean-lib-2.2.3/ocean_lib.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 ocean-contracts==1.1.12
 coloredlogs==15.0.1
 requests>=2.21.0
 pytz
 enforce-typing==1.0.0.post1
 eciespy==0.3.11
 eth-brownie==1.19.3
-cryptography==39.0.1
+cryptography==40.0.2
 yarl==1.8.1
 bitarray<3,>=2.6.0
 
 [dev]
 bumpversion==0.6.0
 pkginfo==1.9.6
 twine==4.0.2
 watchdog==3.0.0
 isort==5.12.0
 flake8==6.0.0
 black
-pre-commit==3.2.1
+pre-commit==3.2.2
 licenseheaders==0.8.8
 codacy-coverage==1.3.11
-coverage==7.2.2
+coverage==7.2.3
 mccabe==0.7.0
 pytest==6.2.5
 pytest-watch==4.2.0
 pytest-env==0.6.2
 matplotlib
 mkcodes==0.1.1
-pytest-sugar==0.9.6
+pytest-sugar==0.9.7
 
 [test]
 codacy-coverage==1.3.11
-coverage==7.2.2
+coverage==7.2.3
 mccabe==0.7.0
 pytest==6.2.5
 pytest-watch==4.2.0
 pytest-env==0.6.2
 matplotlib
 mkcodes==0.1.1
-pytest-sugar==0.9.6
+pytest-sugar==0.9.7
```

### Comparing `ocean-lib-2.2.2/setup.py` & `ocean-lib-2.2.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,46 +21,46 @@
     "ocean-contracts==1.1.12",
     "coloredlogs==15.0.1",
     "requests>=2.21.0",
     "pytz",  # used minimally and unlikely to change, common dependency
     "enforce-typing==1.0.0.post1",
     "eciespy==0.3.11",
     "eth-brownie==1.19.3",
-    "cryptography==39.0.1",
+    "cryptography==40.0.2",
     "yarl==1.8.1",
     "bitarray>=2.6.0,<3",
     # brownie requires web3.py, eth-abi, requests, and more,
     # so those will be installed too.
     # See https://github.com/ethereum/web3.py/blob/master/setup.py
 ]
 # Required to run setup.py:
 setup_requirements = ["pytest-runner"]
 
 test_requirements = [
     "codacy-coverage==1.3.11",
-    "coverage==7.2.2",
+    "coverage==7.2.3",
     "mccabe==0.7.0",
     "pytest==6.2.5",
     "pytest-watch==4.2.0",
     "pytest-env==0.6.2",
     "matplotlib",  # just used in a readme test and unlikely to change, common dependency
     "mkcodes==0.1.1",
-    "pytest-sugar==0.9.6",
+    "pytest-sugar==0.9.7",
 ]
 
 # Possibly required by developers of ocean-lib:
 dev_requirements = [
     "bumpversion==0.6.0",
     "pkginfo==1.9.6",
     "twine==4.0.2",
     "watchdog==3.0.0",
     "isort==5.12.0",
     "flake8==6.0.0",
     "black",  # need to keep this up to date to brownie
-    "pre-commit==3.2.1",
+    "pre-commit==3.2.2",
     "licenseheaders==0.8.8",
 ]
 
 packages = find_namespace_packages(include=["ocean_lib*"], exclude=["*test*"])
 
 setup(
     author="ocean-core-team",
@@ -87,11 +87,11 @@
     packages=packages,
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/oceanprotocol/ocean.py",
     # fmt: off
     # bumpversion.sh needs single-quotes
-    version='2.2.2',
+    version='2.2.3',
     # fmt: on
     zip_safe=False,
 )
```

