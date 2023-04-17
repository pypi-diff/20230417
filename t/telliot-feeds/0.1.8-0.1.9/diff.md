# Comparing `tmp/telliot_feeds-0.1.8.tar.gz` & `tmp/telliot_feeds-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telliot_feeds-0.1.8.tar", last modified: Tue Mar 21 16:59:35 2023, max compression
+gzip compressed data, was "telliot_feeds-0.1.9.tar", last modified: Tue Apr  4 14:40:34 2023, max compression
```

## Comparing `telliot_feeds-0.1.8.tar` & `telliot_feeds-0.1.9.tar`

### file list

```diff
@@ -1,436 +1,455 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.241417 telliot_feeds-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)      814 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.github/ISSUE_TEMPLATE/support-for-new-query-type.md
--rw-r--r--   0 runner    (1001) docker     (116)     1493 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)      716 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1194 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.github/workflows/py39.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1309 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      715 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (116)      719 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.github/workflows/typing.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2477 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1101 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       86 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)     2159 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1274 2023-03-21 16:59:35.241417 telliot_feeds-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      380 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       62 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.193417 telliot_feeds-0.1.8/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/contracts/SampleReporterContract/
--rw-r--r--   0 runner    (1001) docker     (116)     3056 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/SampleReporterContract/SampleFlexReporter.sol
--rw-r--r--   0 runner    (1001) docker     (116)     2168 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/SampleReporterContract/SampleXReporter.sol
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/contracts/TellorFlex/
--rw-r--r--   0 runner    (1001) docker     (116)    28700 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorFlex/Autopay.sol
--rw-r--r--   0 runner    (1001) docker     (116)      994 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorFlex/QueryDataStorage.sol
--rw-r--r--   0 runner    (1001) docker     (116)    22342 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorFlex/TellorFlex.sol
--rw-r--r--   0 runner    (1001) docker     (116)    27210 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorFlex/TellorFlex360.sol
--rw-r--r--   0 runner    (1001) docker     (116)    17249 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorFlex/TellorPlayground.sol
--rw-r--r--   0 runner    (1001) docker     (116)     9363 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorFlex/UsingTellor.sol
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/contracts/TellorFlex/testing/
--rw-r--r--   0 runner    (1001) docker     (116)      317 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorFlex/testing/StakingToken.sol
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/contracts/TellorX/
--rw-r--r--   0 runner    (1001) docker     (116)      253 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorX/TellorXMasterMock.sol
--rw-r--r--   0 runner    (1001) docker     (116)     1264 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/TellorX/TellorXOracleMock.sol
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/contracts/integrations/
--rw-r--r--   0 runner    (1001) docker     (116)     4044 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/integrations/DIVAProtocolMock.sol
--rw-r--r--   0 runner    (1001) docker     (116)     4156 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/integrations/DIVATellorOracleMock.sol
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.201417 telliot_feeds-0.1.8/contracts/integrations/interfaces/
--rw-r--r--   0 runner    (1001) docker     (116)     2246 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/contracts/integrations/interfaces/IDIVADiamond.sol
--rw-r--r--   0 runner    (1001) docker     (116)      139 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (116)     1594 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/add-chain.md
--rw-r--r--   0 runner    (1001) docker     (116)     3949 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/add-spot-price.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (116)     1722 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/assets/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (116)   160315 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/assets/tellor_swoosh.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/docs/code/
--rw-r--r--   0 runner    (1001) docker     (116)       77 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/code/datafeed.md
--rw-r--r--   0 runner    (1001) docker     (116)      101 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/code/dtypes.md
--rw-r--r--   0 runner    (1001) docker     (116)      138 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/code/query-base-classes.md
--rw-r--r--   0 runner    (1001) docker     (116)       90 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/code/query-catalog.md
--rw-r--r--   0 runner    (1001) docker     (116)      105 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/code/query-types.md
--rw-r--r--   0 runner    (1001) docker     (116)     1692 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (116)      347 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/documentation.md
--rw-r--r--   0 runner    (1001) docker     (116)     7327 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (116)      475 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (116)     4371 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/new-query.md
--rw-r--r--   0 runner    (1001) docker     (116)     1682 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/new-release.md
--rw-r--r--   0 runner    (1001) docker     (116)    11205 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      503 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/examples/spot_price_query_example.py
--rw-r--r--   0 runner    (1001) docker     (116)      562 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/examples/text_query_example.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/interfaces/
--rw-r--r--   0 runner    (1001) docker     (116)      446 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/interfaces/IERC20.sol
--rw-r--r--   0 runner    (1001) docker     (116)     8566 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/interfaces/ITellor.sol
--rw-r--r--   0 runner    (1001) docker     (116)     2042 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      219 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      160 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2075 2023-03-21 16:59:35.241417 telliot_feeds-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.197417 telliot_feeds-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/src/telliot_feeds/
--rw-r--r--   0 runner    (1001) docker     (116)       22 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/src/telliot_feeds/cli/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.209417 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      524 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/account.py
--rw-r--r--   0 runner    (1001) docker     (116)     1904 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/catalog.py
--rw-r--r--   0 runner    (1001) docker     (116)      460 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (116)      216 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/integrations.py
--rw-r--r--   0 runner    (1001) docker     (116)     4332 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (116)    15499 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (116)     2415 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/settle.py
--rw-r--r--   0 runner    (1001) docker     (116)     2072 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/tip.py
--rw-r--r--   0 runner    (1001) docker     (116)     1264 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     9445 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      189 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)      633 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/datafeed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2723 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/datasource.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.209417 telliot_feeds-0.1.8/src/telliot_feeds/dtypes/
--rw-r--r--   0 runner    (1001) docker     (116)      224 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      455 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/dtypes/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (116)     1654 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/dtypes/float_type.py
--rw-r--r--   0 runner    (1001) docker     (116)     1646 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/dtypes/value_type.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.213417 telliot_feeds-0.1.8/src/telliot_feeds/feeds/
--rw-r--r--   0 runner    (1001) docker     (116)     7491 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/aave_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      935 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/albt_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      395 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/ampl_usd_vwap_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/avax_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      841 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/badger_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/bch_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      848 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/bct_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1103 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/btc_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/comp_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/crv_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1106 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/dai_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      422 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/daily_volatility_manual_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      383 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/diva_manual_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/doge_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/dot_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      964 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_btc_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      877 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_jpy_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1438 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_usd_30day_volatility.py
--rw-r--r--   0 runner    (1001) docker     (116)     1103 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      817 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/eul_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      765 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/eur_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      624 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/evm_call_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/fil_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      682 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/gas_price_oracle_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/gno_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      684 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/idle_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/link_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/ltc_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1262 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/matic_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      949 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/mimicry_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1245 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/mkr_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      565 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/numeric_api_response_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      389 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/numeric_api_response_manual_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      518 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/olympus.py
--rw-r--r--   0 runner    (1001) docker     (116)      381 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/pls_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      842 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/rai_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      522 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/reth_btc_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      685 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/reth_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      679 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/ric_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/shib_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      634 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/snapshot_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      429 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/spot_price_manual_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      526 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/steth_btc_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      690 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/steth_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      302 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/string_query_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1262 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/sushi_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      737 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/tellor_rng_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      343 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/tellor_rng_manual_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      733 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/trb_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      761 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/twap_manual_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/uni_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/usdc_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      829 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/usdt_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      287 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/uspce_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      518 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/vesq.py
--rw-r--r--   0 runner    (1001) docker     (116)      830 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/xdai_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      823 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/feeds/yfi_usd_feed.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.213417 telliot_feeds-0.1.8/src/telliot_feeds/flashbots/
--rw-r--r--   0 runner    (1001) docker     (116)     1138 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/flashbots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10375 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/flashbots/flashbots.py
--rw-r--r--   0 runner    (1001) docker     (116)     1360 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/flashbots/middleware.py
--rw-r--r--   0 runner    (1001) docker     (116)     2316 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/flashbots/provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     1340 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/flashbots/types.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.213417 telliot_feeds-0.1.8/src/telliot_feeds/integrations/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.217417 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/
--rw-r--r--   0 runner    (1001) docker     (116)      261 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22120 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/abi.py
--rw-r--r--   0 runner    (1001) docker     (116)     1119 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     6337 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/contract.py
--rw-r--r--   0 runner    (1001) docker     (116)     2370 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     4140 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/generate_price_history_csv.py
--rw-r--r--   0 runner    (1001) docker     (116)     3179 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/pool.py
--rw-r--r--   0 runner    (1001) docker     (116)    14754 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/report.py
--rw-r--r--   0 runner    (1001) docker     (116)     3016 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/sources.py
--rw-r--r--   0 runner    (1001) docker     (116)     3288 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.217417 telliot_feeds-0.1.8/src/telliot_feeds/pricing/
--rw-r--r--   0 runner    (1001) docker     (116)       57 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/pricing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2316 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/pricing/price_service.py
--rw-r--r--   0 runner    (1001) docker     (116)     1067 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/pricing/price_source.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.217417 telliot_feeds-0.1.8/src/telliot_feeds/queries/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2990 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/abi_query.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.217417 telliot_feeds-0.1.8/src/telliot_feeds/queries/ampleforth/
--rw-r--r--   0 runner    (1001) docker     (116)       45 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/ampleforth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      824 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/ampleforth/ampl_usd_vwap.py
--rw-r--r--   0 runner    (1001) docker     (116)      665 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/ampleforth/uspce.py
--rw-r--r--   0 runner    (1001) docker     (116)     3842 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/catalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1451 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/daily_volatility.py
--rw-r--r--   0 runner    (1001) docker     (116)     3011 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/diva_protocol.py
--rw-r--r--   0 runner    (1001) docker     (116)     1148 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/evm_call.py
--rw-r--r--   0 runner    (1001) docker     (116)      330 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/export_query_catalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1294 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/gas_price_oracle.py
--rw-r--r--   0 runner    (1001) docker     (116)      712 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/json_query.py
--rw-r--r--   0 runner    (1001) docker     (116)     1454 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/legacy_query.py
--rw-r--r--   0 runner    (1001) docker     (116)     1501 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/mimicry.py
--rw-r--r--   0 runner    (1001) docker     (116)     1206 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/numeric_api_response_query.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.217417 telliot_feeds-0.1.8/src/telliot_feeds/queries/price/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2559 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/price/spot_price.py
--rw-r--r--   0 runner    (1001) docker     (116)     1982 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/price/twap.py
--rw-r--r--   0 runner    (1001) docker     (116)     3241 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/query.py
--rw-r--r--   0 runner    (1001) docker     (116)     8577 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/query_catalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     1231 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (116)      693 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/string_query.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.221417 telliot_feeds-0.1.8/src/telliot_feeds/queries/tellor/
--rw-r--r--   0 runner    (1001) docker     (116)      928 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/tellor/autopay_addresses.py
--rw-r--r--   0 runner    (1001) docker     (116)      901 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/tellor/tellor_oracle_address.py
--rw-r--r--   0 runner    (1001) docker     (116)      842 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/tellor_rng.py
--rw-r--r--   0 runner    (1001) docker     (116)     1003 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/queries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.221417 telliot_feeds-0.1.8/src/telliot_feeds/reporters/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10970 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/custom_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     8570 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/flashbot.py
--rw-r--r--   0 runner    (1001) docker     (116)    21659 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/interval.py
--rw-r--r--   0 runner    (1001) docker     (116)    22355 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/reporter_autopay_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.221417 telliot_feeds-0.1.8/src/telliot_feeds/reporters/rewards/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/rewards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1351 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/rewards/time_based_rewards.py
--rw-r--r--   0 runner    (1001) docker     (116)     2766 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/rng_interval.py
--rw-r--r--   0 runner    (1001) docker     (116)    12564 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tellor_360.py
--rw-r--r--   0 runner    (1001) docker     (116)    13652 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tellor_flex.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.221417 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/
--rw-r--r--   0 runner    (1001) docker     (116)     2049 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.221417 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1966 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/assemble_call.py
--rw-r--r--   0 runner    (1001) docker     (116)     1343 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (116)     6700 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/funded_feeds.py
--rw-r--r--   0 runner    (1001) docker     (116)    10088 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/funded_feeds_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1165 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/one_time_tips.py
--rw-r--r--   0 runner    (1001) docker     (116)     3019 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/tip_listener_filter.py
--rw-r--r--   0 runner    (1001) docker     (116)     1433 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.221417 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/multicall_functions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/multicall_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4265 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/multicall_functions/call_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     7621 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/multicall_functions/multicall_autopay.py
--rw-r--r--   0 runner    (1001) docker     (116)     2623 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/suggest_datafeed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2843 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/tip_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.221417 telliot_feeds-0.1.8/src/telliot_feeds/sources/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.225417 telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7461 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/ampl_usd_vwap.py
--rw-r--r--   0 runner    (1001) docker     (116)     6792 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (116)     1048 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/symbols.py
--rw-r--r--   0 runner    (1001) docker     (116)     8126 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/blockhash_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2819 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/etherscan_gas.py
--rw-r--r--   0 runner    (1001) docker     (116)     3336 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/evm_call.py
--rw-r--r--   0 runner    (1001) docker     (116)     4099 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/gas_price_oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.225417 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1966 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/daily_volatility_manual_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     2583 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/diva_manual_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1953 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/numeric_api_manual_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (116)     2029 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/spot_price_input_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1196 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/string_query_manual_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     2488 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/tellor_rng_manual_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1935 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/twap_manual_input_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1933 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/uspce.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.225417 telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8761 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/collection_stat.py
--rw-r--r--   0 runner    (1001) docker     (116)     4006 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/tami.py
--rw-r--r--   0 runner    (1001) docker     (116)      634 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/types.py
--rw-r--r--   0 runner    (1001) docker     (116)     1876 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2773 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/numeric_api_response.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.225417 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.225417 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/currency/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/currency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2280 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/currency/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (116)     2347 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/currency/openexchangerate.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.225417 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2987 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/coingecko_daily.py
--rw-r--r--   0 runner    (1001) docker     (116)     5105 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/cryptowatch.py
--rw-r--r--   0 runner    (1001) docker     (116)     2244 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/cryptowatch_ohlc.py
--rw-r--r--   0 runner    (1001) docker     (116)     6511 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/kraken.py
--rw-r--r--   0 runner    (1001) docker     (116)     2528 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/kraken_ohlc.py
--rw-r--r--   0 runner    (1001) docker     (116)     4686 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/poloniex.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.229417 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2190 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/binance.py
--rw-r--r--   0 runner    (1001) docker     (116)     2130 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (116)     2188 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/bitflyer.py
--rw-r--r--   0 runner    (1001) docker     (116)     2423 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/bittrex.py
--rw-r--r--   0 runner    (1001) docker     (116)     1985 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (116)     3440 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/coingecko.py
--rw-r--r--   0 runner    (1001) docker     (116)     2940 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/coinmarketcap.py
--rw-r--r--   0 runner    (1001) docker     (116)     2409 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/gemini.py
--rw-r--r--   0 runner    (1001) docker     (116)     2464 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/kraken.py
--rw-r--r--   0 runner    (1001) docker     (116)     2618 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/nomics.py
--rw-r--r--   0 runner    (1001) docker     (116)     2292 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/pancakeswap.py
--rw-r--r--   0 runner    (1001) docker     (116)     3197 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/pulsechain_subgraph.py
--rw-r--r--   0 runner    (1001) docker     (116)     3787 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/uniswapV3.py
--rw-r--r--   0 runner    (1001) docker     (116)     3201 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/sources/price_aggregator.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.229417 telliot_feeds-0.1.8/src/telliot_feeds/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12402 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/abi.py
--rw-r--r--   0 runner    (1001) docker     (116)     5605 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/cfg.py
--rw-r--r--   0 runner    (1001) docker     (116)     6559 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/contract.py
--rw-r--r--   0 runner    (1001) docker     (116)     4018 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/decode.py
--rw-r--r--   0 runner    (1001) docker     (116)       77 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/home.py
--rw-r--r--   0 runner    (1001) docker     (116)     2192 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/input_timeout.py
--rw-r--r--   0 runner    (1001) docker     (116)     1669 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (116)     7903 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/reporter_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      528 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/src/telliot_feeds/utils/stdev_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.205417 telliot_feeds-0.1.8/src/telliot_feeds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1274 2023-03-21 16:59:35.000000 telliot_feeds-0.1.8/src/telliot_feeds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    15266 2023-03-21 16:59:35.000000 telliot_feeds-0.1.8/src/telliot_feeds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-21 16:59:35.000000 telliot_feeds-0.1.8/src/telliot_feeds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       56 2023-03-21 16:59:35.000000 telliot_feeds-0.1.8/src/telliot_feeds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      860 2023-03-21 16:59:35.000000 telliot_feeds-0.1.8/src/telliot_feeds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-03-21 16:59:35.000000 telliot_feeds-0.1.8/src/telliot_feeds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.229417 telliot_feeds-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.229417 telliot_feeds-0.1.8/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (116)     7708 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     1817 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/cli/test_diva_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     2066 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/cli/test_query_cmd.py
--rw-r--r--   0 runner    (1001) docker     (116)      500 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/cli/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     9085 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.233417 telliot_feeds-0.1.8/tests/feeds/
--rw-r--r--   0 runner    (1001) docker     (116)       35 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      361 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_active_feeds.py
--rw-r--r--   0 runner    (1001) docker     (116)      229 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_ampl_usd_vwap_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2657 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_bct_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      993 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_btc_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2659 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_diva_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      826 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_eth_btc_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      614 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_eth_jpy_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      758 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_eth_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      265 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_eth_usd_volatility_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      311 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_eur_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      603 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_gas_price_oracle_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2658 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_idle_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      952 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_manual_snapshot_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2659 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_matic_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1360 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_mimicry_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2657 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_mkr_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     1198 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_pop_spot_price_feeds.py
--rw-r--r--   0 runner    (1001) docker     (116)      692 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_reth_btc_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      692 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_reth_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2657 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_ric_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      699 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_steth_btc_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      699 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_steth_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2659 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_sushi_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      595 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_trb_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2658 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_usdc_usd_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      205 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/feeds/test_uspce_feed.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.197417 telliot_feeds-0.1.8/tests/integrations/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.233417 telliot_feeds-0.1.8/tests/integrations/diva_protocol/
--rw-r--r--   0 runner    (1001) docker     (116)     1427 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_construct_datafeed.py
--rw-r--r--   0 runner    (1001) docker     (116)     4598 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_diva_contracts.py
--rw-r--r--   0 runner    (1001) docker     (116)     6947 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_e2e_create_report_settle_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     1496 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_get_pools.py
--rw-r--r--   0 runner    (1001) docker     (116)     4345 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_report.py
--rw-r--r--   0 runner    (1001) docker     (116)     1607 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/integrations/diva_protocol/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.237417 telliot_feeds-0.1.8/tests/queries/
--rw-r--r--   0 runner    (1001) docker     (116)      946 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_abi_query.py
--rw-r--r--   0 runner    (1001) docker     (116)      331 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_json_query.py
--rw-r--r--   0 runner    (1001) docker     (116)      914 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_ampl_usd_vwap.py
--rw-r--r--   0 runner    (1001) docker     (116)      645 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_base.py
--rw-r--r--   0 runner    (1001) docker     (116)      686 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_catalog.py
--rw-r--r--   0 runner    (1001) docker     (116)     2677 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_daily_volatility.py
--rw-r--r--   0 runner    (1001) docker     (116)     3298 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_diva_protocol.py
--rw-r--r--   0 runner    (1001) docker     (116)     3455 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_evm_call.py
--rw-r--r--   0 runner    (1001) docker     (116)     2045 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_gas_price_oracle.py
--rw-r--r--   0 runner    (1001) docker     (116)     1445 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_legacy_query.py
--rw-r--r--   0 runner    (1001) docker     (116)     2323 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_mimicry.py
--rw-r--r--   0 runner    (1001) docker     (116)     3114 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_numeric_api_response.py
--rw-r--r--   0 runner    (1001) docker     (116)     2824 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (116)     2816 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_spot_price.py
--rw-r--r--   0 runner    (1001) docker     (116)      547 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_string_query.py
--rw-r--r--   0 runner    (1001) docker     (116)     1157 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_support.py
--rw-r--r--   0 runner    (1001) docker     (116)     3584 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_tellor_addresses.py
--rw-r--r--   0 runner    (1001) docker     (116)     1812 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_tellor_rng.py
--rw-r--r--   0 runner    (1001) docker     (116)     2092 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_twap.py
--rw-r--r--   0 runner    (1001) docker     (116)      871 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/queries/test_query_uspce.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.237417 telliot_feeds-0.1.8/tests/reporters/
--rw-r--r--   0 runner    (1001) docker     (116)       35 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9481 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_360_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     4832 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_autopay_multicalls.py
--rw-r--r--   0 runner    (1001) docker     (116)     5206 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_custom_360_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     3284 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_evm_call.py
--rw-r--r--   0 runner    (1001) docker     (116)      959 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_flashbot_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     5153 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_flex_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     7411 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_interval_reporter.py
--rw-r--r--   0 runner    (1001) docker     (116)     7355 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/reporters/test_rng_reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.237417 telliot_feeds-0.1.8/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.237417 telliot_feeds-0.1.8/tests/sources/manual/
--rw-r--r--   0 runner    (1001) docker     (116)      702 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/manual/test_diva_manual_entry_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     2749 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/manual/test_rng_manual_input_source.py
--rw-r--r--   0 runner    (1001) docker     (116)      980 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/manual/test_spot_price_manual_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1043 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/manual/test_string_query_manual_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1377 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/manual/test_twap_manual_source.py
--rw-r--r--   0 runner    (1001) docker     (116)      565 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/manual/test_uspce_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     2665 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_ampl_usd_vwap_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1130 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_curr_exchange_sources.py
--rw-r--r--   0 runner    (1001) docker     (116)     1652 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_etherscan_gas.py
--rw-r--r--   0 runner    (1001) docker     (116)     2399 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_evm_call_source.py
--rw-r--r--   0 runner    (1001) docker     (116)      550 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_gas_price_oracle_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     5639 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_historical_price_sources.py
--rw-r--r--   0 runner    (1001) docker     (116)      587 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_mimicry_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     1397 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_source_numeric_api_response.py
--rw-r--r--   0 runner    (1001) docker     (116)    14180 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_spot_price_sources.py
--rw-r--r--   0 runner    (1001) docker     (116)     5145 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_tami_calcuation.py
--rw-r--r--   0 runner    (1001) docker     (116)     3218 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/sources/test_tellor_rng_source.py
--rw-r--r--   0 runner    (1001) docker     (116)     8749 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_autopay.py
--rw-r--r--   0 runner    (1001) docker     (116)     2152 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_bct_usd.py
--rw-r--r--   0 runner    (1001) docker     (116)     2152 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_dai_usd.py
--rw-r--r--   0 runner    (1001) docker     (116)      430 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_data_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)      572 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (116)      701 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (116)     2547 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_numeric_api_response_feed.py
--rw-r--r--   0 runner    (1001) docker     (116)     2597 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_olympus.py
--rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_price_service.py
--rw-r--r--   0 runner    (1001) docker     (116)     2230 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_value_type.py
--rw-r--r--   0 runner    (1001) docker     (116)     2649 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/test_vesq.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.241417 telliot_feeds-0.1.8/tests/tips/
--rw-r--r--   0 runner    (1001) docker     (116)     4192 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/tips/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)     3478 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/tips/test_feed_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (116)     2656 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/tips/test_multicall_autopay.py
--rw-r--r--   0 runner    (1001) docker     (116)      834 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/tips/test_multicall_support.py
--rw-r--r--   0 runner    (1001) docker     (116)     2623 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/tips/test_one_time_tips.py
--rw-r--r--   0 runner    (1001) docker     (116)     8596 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/tips/test_selected_queryid.py
--rw-r--r--   0 runner    (1001) docker     (116)     5091 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/tips/test_tips_available_after_submission.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:35.241417 telliot_feeds-0.1.8/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5294 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/utils/test_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1124 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/utils/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (116)     1014 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/utils/test_input_timeout.py
--rw-r--r--   0 runner    (1001) docker     (116)     3665 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/utils/test_reporter_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      310 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tests/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1012 2023-03-21 16:59:26.000000 telliot_feeds-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.670380 telliot_feeds-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.578377 telliot_feeds-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.578377 telliot_feeds-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.github/ISSUE_TEMPLATE/support-for-new-query-type.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.582377 telliot_feeds-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.github/workflows/py39.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.github/workflows/typing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-04 14:40:34.670380 telliot_feeds-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.562377 telliot_feeds-0.1.9/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.582377 telliot_feeds-0.1.9/contracts/SampleReporterContract/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/SampleReporterContract/SampleFlexReporter.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/SampleReporterContract/SampleXReporter.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.582377 telliot_feeds-0.1.9/contracts/TellorFlex/
+-rw-r--r--   0 runner    (1001) docker     (123)    28700 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorFlex/Autopay.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorFlex/QueryDataStorage.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    22342 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorFlex/TellorFlex.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    27210 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorFlex/TellorFlex360.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorFlex/TellorPlayground.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorFlex/UsingTellor.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.582377 telliot_feeds-0.1.9/contracts/TellorFlex/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorFlex/testing/StakingToken.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.582377 telliot_feeds-0.1.9/contracts/TellorX/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorX/TellorXMasterMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/TellorX/TellorXOracleMock.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.582377 telliot_feeds-0.1.9/contracts/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/integrations/DIVAProtocolMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/integrations/DIVATellorOracleMock.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.582377 telliot_feeds-0.1.9/contracts/integrations/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/contracts/integrations/interfaces/IDIVADiamond.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.586377 telliot_feeds-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/add-chain.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/add-spot-price.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.586377 telliot_feeds-0.1.9/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/assets/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160315 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/assets/tellor_swoosh.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.590378 telliot_feeds-0.1.9/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/code/datafeed.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/code/dtypes.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/code/query-base-classes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/code/query-catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/code/query-types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/new-query.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/new-release.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.590378 telliot_feeds-0.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/examples/spot_price_query_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/examples/text_query_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.590378 telliot_feeds-0.1.9/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/interfaces/IERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/interfaces/ITellor.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-04 14:40:34.674380 telliot_feeds-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.566377 telliot_feeds-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.590378 telliot_feeds-0.1.9/src/telliot_feeds/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.594378 telliot_feeds-0.1.9/src/telliot_feeds/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.594378 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/settle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/tip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/datafeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/datasource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.594378 telliot_feeds-0.1.9/src/telliot_feeds/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/dtypes/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/dtypes/float_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/dtypes/value_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.610378 telliot_feeds-0.1.9/src/telliot_feeds/feeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/aave_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/albt_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/ampl_usd_vwap_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/avax_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/badger_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/bch_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/bct_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/btc_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/comp_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/crv_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/dai_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/daily_volatility_manual_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/diva_manual_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/doge_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/dot_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_btc_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_jpy_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_usd_30day_volatility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/eul_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/eur_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/evm_call_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/fil_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/gas_price_oracle_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/gno_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/idle_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/link_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/ltc_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/matic_usd_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.610378 telliot_feeds-0.1.9/src/telliot_feeds/feeds/mimicry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/mimicry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/mimicry/collection_stat_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/mimicry/macro_market_mashup_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/mimicry/nft_index_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/mkr_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/numeric_api_response_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/numeric_api_response_manual_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/olympus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/op_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/pls_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/rai_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/reth_btc_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/reth_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/ric_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/shib_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/snapshot_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/spot_price_manual_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/steth_btc_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/steth_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/string_query_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/sushi_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/tellor_rng_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/tellor_rng_manual_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/trb_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/twap_manual_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/uni_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/usdc_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/usdt_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/uspce_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/vesq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/wsteth_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/xdai_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/feeds/yfi_usd_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.614378 telliot_feeds-0.1.9/src/telliot_feeds/flashbots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/flashbots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/flashbots/flashbots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/flashbots/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/flashbots/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/flashbots/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.614378 telliot_feeds-0.1.9/src/telliot_feeds/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.618378 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22120 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/generate_price_history_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.622379 telliot_feeds-0.1.9/src/telliot_feeds/pricing/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/pricing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/pricing/price_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/pricing/price_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.622379 telliot_feeds-0.1.9/src/telliot_feeds/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/abi_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.626379 telliot_feeds-0.1.9/src/telliot_feeds/queries/ampleforth/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/ampleforth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/ampleforth/ampl_usd_vwap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/ampleforth/uspce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/daily_volatility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/diva_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/evm_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/export_query_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/gas_price_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/legacy_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.626379 telliot_feeds-0.1.9/src/telliot_feeds/queries/mimicry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/mimicry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/mimicry/collection_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/mimicry/macro_market_mash_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/mimicry/nft_market_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/numeric_api_response_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.626379 telliot_feeds-0.1.9/src/telliot_feeds/queries/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/price/spot_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/price/twap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/query_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/string_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.626379 telliot_feeds-0.1.9/src/telliot_feeds/queries/tellor/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/tellor/autopay_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/tellor/tellor_oracle_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/tellor_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/queries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.630379 telliot_feeds-0.1.9/src/telliot_feeds/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/custom_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/flashbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21659 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/reporter_autopay_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.630379 telliot_feeds-0.1.9/src/telliot_feeds/reporters/rewards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/rewards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/rewards/time_based_rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/rng_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tellor_360.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tellor_flex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.630379 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.630379 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/assemble_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/funded_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/funded_feeds_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/one_time_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/tip_listener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.630379 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/multicall_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/multicall_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/multicall_functions/call_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/multicall_functions/multicall_autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/suggest_datafeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/tip_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.634379 telliot_feeds-0.1.9/src/telliot_feeds/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.634379 telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/ampl_usd_vwap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/bitfinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/blockhash_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/etherscan_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/evm_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/gas_price_oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.638379 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/daily_volatility_manual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/diva_manual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/numeric_api_manual_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/spot_price_input_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/string_query_manual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/tellor_rng_manual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/twap_manual_input_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/uspce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.638379 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/collection_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/mashup_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/nft_market_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/tami.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/numeric_api_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.638379 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.638379 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/currency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/currency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/currency/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/currency/openexchangerate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.642379 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/coingecko_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/cryptowatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/cryptowatch_ohlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/kraken_ohlc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/poloniex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.646379 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/bitfinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/bitflyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/bittrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/coingecko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/coinmarketcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/coinpaprika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/curvefi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/nomics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/pancakeswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/pulsechain_subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/uniswapV3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/price_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/sources/wsteth_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.646379 telliot_feeds-0.1.9/src/telliot_feeds/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/input_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/reporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/src/telliot_feeds/utils/stdev_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.590378 telliot_feeds-0.1.9/src/telliot_feeds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-04 14:40:34.000000 telliot_feeds-0.1.9/src/telliot_feeds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-04-04 14:40:34.000000 telliot_feeds-0.1.9/src/telliot_feeds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:40:34.000000 telliot_feeds-0.1.9/src/telliot_feeds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 14:40:34.000000 telliot_feeds-0.1.9/src/telliot_feeds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-04 14:40:34.000000 telliot_feeds-0.1.9/src/telliot_feeds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 14:40:34.000000 telliot_feeds-0.1.9/src/telliot_feeds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.650380 telliot_feeds-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.650380 telliot_feeds-0.1.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/cli/test_diva_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/cli/test_query_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/cli/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.658380 telliot_feeds-0.1.9/tests/feeds/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_active_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_ampl_usd_vwap_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_bct_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_btc_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_diva_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_eth_btc_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_eth_jpy_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_eth_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_eth_usd_volatility_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_eur_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_gas_price_oracle_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_idle_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_manual_snapshot_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_matic_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_mimicry_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_mkr_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_op_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_pop_spot_price_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_reth_btc_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_reth_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_ric_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_steth_btc_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_steth_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_sushi_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_trb_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_usdc_usd_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_uspce_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/feeds/test_wsteth_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.574377 telliot_feeds-0.1.9/tests/integrations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.658380 telliot_feeds-0.1.9/tests/integrations/diva_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_construct_datafeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_diva_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_e2e_create_report_settle_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/integrations/diva_protocol/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.662380 telliot_feeds-0.1.9/tests/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_abi_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_ampl_usd_vwap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_daily_volatility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_diva_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_evm_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_gas_price_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_legacy_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_mimicry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_mimicry_mashup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_mimicry_nft_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_numeric_api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_spot_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_string_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_tellor_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_tellor_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_twap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/queries/test_query_uspce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.666380 telliot_feeds-0.1.9/tests/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_360_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_autopay_multicalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_custom_360_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_evm_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_flashbot_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_flex_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_interval_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/reporters/test_rng_reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.666380 telliot_feeds-0.1.9/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.670380 telliot_feeds-0.1.9/tests/sources/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/manual/test_diva_manual_entry_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/manual/test_rng_manual_input_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/manual/test_spot_price_manual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/manual/test_string_query_manual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/manual/test_twap_manual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/manual/test_uspce_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_ampl_usd_vwap_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_curr_exchange_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_etherscan_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_evm_call_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_gas_price_oracle_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_historical_price_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_mimicry_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_source_numeric_api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14959 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_spot_price_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_tami_calcuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/sources/test_tellor_rng_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_bct_usd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_dai_usd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_numeric_api_response_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_olympus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_price_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_value_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/test_vesq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.670380 telliot_feeds-0.1.9/tests/tips/
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/tips/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/tips/test_feed_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/tips/test_multicall_autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/tips/test_multicall_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/tips/test_one_time_tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/tips/test_selected_queryid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/tips/test_tips_available_after_submission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:34.670380 telliot_feeds-0.1.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/utils/test_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/utils/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/utils/test_input_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/utils/test_reporter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tests/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-04 14:40:23.000000 telliot_feeds-0.1.9/tox.ini
```

### Comparing `telliot_feeds-0.1.8/.github/ISSUE_TEMPLATE/support-for-new-query-type.md` & `telliot_feeds-0.1.9/.github/ISSUE_TEMPLATE/support-for-new-query-type.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/.github/pull_request_template.md` & `telliot_feeds-0.1.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/.github/workflows/docs.yml` & `telliot_feeds-0.1.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/.github/workflows/py39.yml` & `telliot_feeds-0.1.9/.github/workflows/py39.yml`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/.github/workflows/release.yml` & `telliot_feeds-0.1.9/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 on:
   release:
     types: [published, released]
 
 jobs:
   build-n-publish:
     name: Publish telliot-feeds
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
 
     steps:
     - uses: actions/checkout@master
     - name: Set up Python 3.9
       uses: actions/setup-python@v1
       with:
         python-version: 3.9
@@ -41,8 +41,8 @@
         password: ${{ secrets.TELLIOT_FEEDS_TEST_PYPI_API_TOKEN }}
         repository_url: https://test.pypi.org/legacy/
 
     - name: Publish telliot-feeds to PyPI
       if: "!github.event.release.prerelease"
       uses: pypa/gh-action-pypi-publish@master
       with:
-        password: ${{ secrets.TELLIOT_FEEDS_PYPI_API_TOKEN }}
+        password: ${{ secrets.TELLIOT_FEEDS_PYPI_API_TOKEN }}
```

### Comparing `telliot_feeds-0.1.8/.github/workflows/style.yml` & `telliot_feeds-0.1.9/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/.github/workflows/typing.yml` & `telliot_feeds-0.1.9/.github/workflows/typing.yml`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/.gitignore` & `telliot_feeds-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/.pre-commit-config.yaml` & `telliot_feeds-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/LICENSE` & `telliot_feeds-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/PKG-INFO` & `telliot_feeds-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot_feeds
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for interacting with Tellor Protocol smart contracts.
 Home-page: https://github.com/tellor-io/telliot-feeds
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,ethereum,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_feeds-0.1.8/contracts/SampleReporterContract/SampleFlexReporter.sol` & `telliot_feeds-0.1.9/contracts/SampleReporterContract/SampleFlexReporter.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/SampleReporterContract/SampleXReporter.sol` & `telliot_feeds-0.1.9/contracts/SampleReporterContract/SampleXReporter.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/TellorFlex/Autopay.sol` & `telliot_feeds-0.1.9/contracts/TellorFlex/Autopay.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/TellorFlex/QueryDataStorage.sol` & `telliot_feeds-0.1.9/contracts/TellorFlex/QueryDataStorage.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/TellorFlex/TellorFlex.sol` & `telliot_feeds-0.1.9/contracts/TellorFlex/TellorFlex.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/TellorFlex/TellorFlex360.sol` & `telliot_feeds-0.1.9/contracts/TellorFlex/TellorFlex360.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/TellorFlex/TellorPlayground.sol` & `telliot_feeds-0.1.9/contracts/TellorFlex/TellorPlayground.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/TellorFlex/UsingTellor.sol` & `telliot_feeds-0.1.9/contracts/TellorFlex/UsingTellor.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/TellorX/TellorXOracleMock.sol` & `telliot_feeds-0.1.9/contracts/TellorX/TellorXOracleMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/integrations/DIVAProtocolMock.sol` & `telliot_feeds-0.1.9/contracts/integrations/DIVAProtocolMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/integrations/DIVATellorOracleMock.sol` & `telliot_feeds-0.1.9/contracts/integrations/DIVATellorOracleMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/contracts/integrations/interfaces/IDIVADiamond.sol` & `telliot_feeds-0.1.9/contracts/integrations/interfaces/IDIVADiamond.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/add-chain.md` & `telliot_feeds-0.1.9/docs/add-chain.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/add-spot-price.md` & `telliot_feeds-0.1.9/docs/add-spot-price.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/assets/favicon-32x32.png` & `telliot_feeds-0.1.9/docs/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/assets/tellor_swoosh.png` & `telliot_feeds-0.1.9/docs/assets/tellor_swoosh.png`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/contributing.md` & `telliot_feeds-0.1.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/getting-started.md` & `telliot_feeds-0.1.9/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/new-query.md` & `telliot_feeds-0.1.9/docs/new-query.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/new-release.md` & `telliot_feeds-0.1.9/docs/new-release.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/docs/usage.md` & `telliot_feeds-0.1.9/docs/usage.md`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/examples/text_query_example.py` & `telliot_feeds-0.1.9/examples/text_query_example.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/interfaces/ITellor.sol` & `telliot_feeds-0.1.9/interfaces/ITellor.sol`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/mkdocs.yml` & `telliot_feeds-0.1.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/setup.cfg` & `telliot_feeds-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 	python-dateutil==2.8.1
 	python-dotenv==0.21.0
 	PyYAML==6.0
 	requests==2.28.1
 	rlp==2.0.1
 	simple-term-menu==1.5.2
 	six==1.16.0
-	telliot-core==0.2.3
+	telliot-core==0.2.4
 	toolz==0.12.0
 	typing_extensions==4.4.0
 	urllib3==1.26.12
 	varint==1.0.2
 	web3==5.28.0
 	websockets==9.1
 	yarl==1.8.1
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/account.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/catalog.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/catalog.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/query.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/report.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/settle.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/settle.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/commands/tip.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/commands/tip.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/main.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/main.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/cli/utils.py` & `telliot_feeds-0.1.9/src/telliot_feeds/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,18 @@
         # get param type if type isn't optional
         try:
             param_dtype = get_args(type_hints[query_param])[0]  # parse out Optional type
         except IndexError:
             param_dtype = type_hints[query_param]
 
         val = input(f"Enter value for QueryParameter {query_param}: ")
+        try:
+            val = eval(val)  # try to evaluate input if it's not string type
+        except NameError:
+            pass
 
         if val is not None:
             try:
                 # cast input from string to datatype of query parameter
                 if param_dtype == bytes and val.startswith("0x"):
                     val = bytes.fromhex(val[2:])
                 val = param_dtype(val)
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/datafeed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/datafeed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/datasource.py` & `telliot_feeds-0.1.9/src/telliot_feeds/datasource.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/dtypes/float_type.py` & `telliot_feeds-0.1.9/src/telliot_feeds/dtypes/float_type.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/dtypes/value_type.py` & `telliot_feeds-0.1.9/src/telliot_feeds/dtypes/value_type.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/__init__.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,26 @@
 from telliot_feeds.feeds.gas_price_oracle_feed import gas_price_oracle_feed
 from telliot_feeds.feeds.gas_price_oracle_feed import gas_price_oracle_feed_example
 from telliot_feeds.feeds.gno_usd_feed import gno_usd_median_feed
 from telliot_feeds.feeds.idle_usd_feed import idle_usd_median_feed
 from telliot_feeds.feeds.link_usd_feed import link_usd_median_feed
 from telliot_feeds.feeds.ltc_usd_feed import ltc_usd_median_feed
 from telliot_feeds.feeds.matic_usd_feed import matic_usd_median_feed
-from telliot_feeds.feeds.mimicry_feed import mimicry_collection_stat_datafeed
-from telliot_feeds.feeds.mimicry_feed import mimicry_example_feed
+from telliot_feeds.feeds.mimicry.collection_stat_feed import mimicry_collection_stat_feed
+from telliot_feeds.feeds.mimicry.collection_stat_feed import mimicry_example_feed
+from telliot_feeds.feeds.mimicry.macro_market_mashup_feed import mimicry_mashup_example_feed
+from telliot_feeds.feeds.mimicry.macro_market_mashup_feed import mimicry_mashup_feed
+from telliot_feeds.feeds.mimicry.nft_index_feed import mimicry_nft_market_index_eth_feed
+from telliot_feeds.feeds.mimicry.nft_index_feed import mimicry_nft_market_index_feed
+from telliot_feeds.feeds.mimicry.nft_index_feed import mimicry_nft_market_index_usd_feed
 from telliot_feeds.feeds.mkr_usd_feed import mkr_usd_median_feed
 from telliot_feeds.feeds.numeric_api_response_feed import numeric_api_response_feed
 from telliot_feeds.feeds.numeric_api_response_manual_feed import numeric_api_response_manual_feed
 from telliot_feeds.feeds.olympus import ohm_eth_median_feed
+from telliot_feeds.feeds.op_usd_feed import op_usd_median_feed
 from telliot_feeds.feeds.pls_usd_feed import pls_usd_feed
 from telliot_feeds.feeds.rai_usd_feed import rai_usd_median_feed
 from telliot_feeds.feeds.reth_btc_feed import reth_btc_median_feed
 from telliot_feeds.feeds.reth_usd_feed import reth_usd_median_feed
 from telliot_feeds.feeds.ric_usd_feed import ric_usd_median_feed
 from telliot_feeds.feeds.shib_usd_feed import shib_usd_median_feed
 from telliot_feeds.feeds.snapshot_feed import snapshot_feed_example
@@ -58,14 +64,16 @@
 from telliot_feeds.feeds.twap_manual_feed import twap_30d_example_manual_feed
 from telliot_feeds.feeds.twap_manual_feed import twap_manual_feed
 from telliot_feeds.feeds.uni_usd_feed import uni_usd_median_feed
 from telliot_feeds.feeds.usdc_usd_feed import usdc_usd_median_feed
 from telliot_feeds.feeds.usdt_usd_feed import usdt_usd_median_feed
 from telliot_feeds.feeds.uspce_feed import uspce_feed
 from telliot_feeds.feeds.vesq import vsq_usd_median_feed
+from telliot_feeds.feeds.wsteth_feed import wsteth_eth_median_feed
+from telliot_feeds.feeds.wsteth_feed import wsteth_usd_median_feed
 from telliot_feeds.feeds.xdai_usd_feed import xdai_usd_median_feed
 from telliot_feeds.feeds.yfi_usd_feed import yfi_usd_median_feed
 
 
 CATALOG_FEEDS = {
     "ampleforth-custom": ampl_usd_vwap_feed,
     "ampleforth-uspce": uspce_feed,
@@ -112,18 +120,24 @@
     "link-usd-spot": link_usd_median_feed,
     "ltc-usd-spot": ltc_usd_median_feed,
     "shib-usd-spot": shib_usd_median_feed,
     "uni-usd-spot": uni_usd_median_feed,
     "usdt-usd-spot": usdt_usd_median_feed,
     "yfi-usd-spot": yfi_usd_median_feed,
     "mimicry-crypto-coven-tami": mimicry_example_feed,
+    "mimicry-nft-index-usd": mimicry_nft_market_index_usd_feed,
+    "mimicry-nft-index-eth": mimicry_nft_market_index_eth_feed,
+    "mimicry-mashup-example": mimicry_mashup_example_feed,
     "steth-btc-spot": steth_btc_median_feed,
     "steth-usd-spot": steth_usd_median_feed,
     "reth-btc-spot": reth_btc_median_feed,
     "reth-usd-spot": reth_usd_median_feed,
+    "wsteth-usd-spot": wsteth_usd_median_feed,
+    "wsteth-eth-spot": wsteth_eth_median_feed,
+    "op-usd-spot": op_usd_median_feed,
 }
 
 DATAFEED_BUILDER_MAPPING: Dict[str, DataFeed[Any]] = {
     "SpotPrice": spot_price_manual_feed,
     "DivaProtocol": diva_manual_feed,
     "SnapshotOracle": snapshot_manual_feed,
     "GasPriceOracle": gas_price_oracle_feed,
@@ -132,10 +146,12 @@
     "NumericApiResponse": numeric_api_response_feed,  # this build will parse and submit response value automatically
     "TWAP": twap_manual_feed,
     "DailyVolatility": daily_volatility_manual_feed,
     "TellorRNG": tellor_rng_feed,
     "TellorRNGManualResponse": tellor_rng_manual_feed,
     "AmpleforthCustomSpotPrice": ampl_usd_vwap_feed,
     "AmpleforthUSPCE": uspce_feed,
-    "MimicryCollectionStat": mimicry_collection_stat_datafeed,
+    "MimicryCollectionStat": mimicry_collection_stat_feed,
+    "MimicryNFTMarketIndex": mimicry_nft_market_index_feed,
+    "MimicryMacroMarketMashup": mimicry_mashup_feed,
     "EVMCall": evm_call_feed,
 }
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/aave_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/aave_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/albt_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/albt_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/avax_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/avax_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/badger_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/badger_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/bch_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/bch_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/bct_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/bct_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/btc_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/btc_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/comp_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/comp_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/crv_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/crv_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/dai_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/dai_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/doge_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/doge_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/dot_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/dot_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_btc_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_btc_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_jpy_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_jpy_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_usd_30day_volatility.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_usd_30day_volatility.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/eth_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/eth_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/eul_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/eul_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/eur_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/eur_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/evm_call_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/evm_call_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/fil_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/fil_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/gas_price_oracle_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/gas_price_oracle_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/gno_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/gno_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/idle_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/idle_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/link_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/link_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/ltc_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/ltc_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/matic_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/matic_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/mimicry_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/mimicry/collection_stat_feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """DataFeed for MimicryCollectionStat query type. Calculates TAMI index or NFT market cap"""
 from telliot_feeds.datafeed import DataFeed
-from telliot_feeds.queries.mimicry import MimicryCollectionStat
+from telliot_feeds.queries.mimicry.collection_stat import MimicryCollectionStat
 from telliot_feeds.sources.mimicry.collection_stat import MimicryCollectionStatSource
 
 chain_id = None
 collection_address = None
 metric = None
 
-mimicry_collection_stat_datafeed = DataFeed(
+mimicry_collection_stat_feed = DataFeed(
     query=MimicryCollectionStat(chainId=chain_id, collectionAddress=collection_address, metric=metric),
     source=MimicryCollectionStatSource(chainId=chain_id, collectionAddress=collection_address, metric=metric),
 )
 
 chain_id = 1
 collection_address = "0x5180db8F5c931aaE63c74266b211F580155ecac8"
 metric = 0
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/mkr_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/mkr_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/numeric_api_response_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/numeric_api_response_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/olympus.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/olympus.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/rai_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/rai_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/reth_btc_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/op_usd_feed.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from telliot_feeds.datafeed import DataFeed
 from telliot_feeds.queries.price.spot_price import SpotPrice
+from telliot_feeds.sources.price.spot.coinbase import CoinbaseSpotPriceSource
 from telliot_feeds.sources.price.spot.coingecko import CoinGeckoSpotPriceSource
 from telliot_feeds.sources.price_aggregator import PriceAggregator
 
-reth_btc_median_feed = DataFeed(
-    query=SpotPrice(asset="RETH", currency="BTC"),
+op_usd_median_feed = DataFeed(
+    query=SpotPrice(asset="OP", currency="USD"),
     source=PriceAggregator(
-        asset="reth",
-        currency="btc",
+        asset="op",
+        currency="usd",
         algorithm="median",
-        sources=[CoinGeckoSpotPriceSource(asset="reth", currency="btc")],
+        sources=[
+            CoinGeckoSpotPriceSource(asset="op", currency="usd"),
+            CoinbaseSpotPriceSource(asset="op", currency="usd"),
+        ],
     ),
 )
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/reth_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/uni_usd_feed.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from telliot_feeds.datafeed import DataFeed
 from telliot_feeds.queries.price.spot_price import SpotPrice
+from telliot_feeds.sources.price.spot.coinbase import CoinbaseSpotPriceSource
 from telliot_feeds.sources.price.spot.coingecko import CoinGeckoSpotPriceSource
-from telliot_feeds.sources.price.spot.uniswapV3 import UniswapV3PriceSource
+from telliot_feeds.sources.price.spot.gemini import GeminiSpotPriceSource
 from telliot_feeds.sources.price_aggregator import PriceAggregator
 
-reth_usd_median_feed = DataFeed(
-    query=SpotPrice(asset="RETH", currency="USD"),
+uni_usd_median_feed = DataFeed(
+    query=SpotPrice(asset="UNI", currency="USD"),
     source=PriceAggregator(
-        asset="reth",
+        asset="uni",
         currency="usd",
         algorithm="median",
         sources=[
-            CoinGeckoSpotPriceSource(asset="reth", currency="usd"),
-            UniswapV3PriceSource(asset="reth", currency="usd"),
+            CoinGeckoSpotPriceSource(asset="uni", currency="usd"),
+            CoinbaseSpotPriceSource(asset="uni", currency="usd"),
+            GeminiSpotPriceSource(asset="uni", currency="usd"),
         ],
     ),
 )
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/ric_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/ric_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/shib_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/shib_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/snapshot_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/snapshot_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/steth_btc_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/reth_btc_feed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from telliot_feeds.datafeed import DataFeed
 from telliot_feeds.queries.price.spot_price import SpotPrice
 from telliot_feeds.sources.price.spot.coingecko import CoinGeckoSpotPriceSource
+from telliot_feeds.sources.price.spot.coinpaprika import CoinpaprikaSpotPriceSource
 from telliot_feeds.sources.price_aggregator import PriceAggregator
 
-steth_btc_median_feed = DataFeed(
-    query=SpotPrice(asset="STETH", currency="BTC"),
+reth_btc_median_feed = DataFeed(
+    query=SpotPrice(asset="RETH", currency="BTC"),
     source=PriceAggregator(
-        asset="steth",
+        asset="reth",
         currency="btc",
         algorithm="median",
-        sources=[CoinGeckoSpotPriceSource(asset="steth", currency="btc")],
+        sources=[
+            CoinGeckoSpotPriceSource(asset="reth", currency="btc"),
+            CoinpaprikaSpotPriceSource(asset="reth-rocket-pool-eth", currency="btc"),
+        ],
     ),
 )
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/steth_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/yfi_usd_feed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from telliot_feeds.datafeed import DataFeed
 from telliot_feeds.queries.price.spot_price import SpotPrice
+from telliot_feeds.sources.price.spot.coinbase import CoinbaseSpotPriceSource
 from telliot_feeds.sources.price.spot.coingecko import CoinGeckoSpotPriceSource
-from telliot_feeds.sources.price.spot.uniswapV3 import UniswapV3PriceSource
+from telliot_feeds.sources.price.spot.gemini import GeminiSpotPriceSource
 from telliot_feeds.sources.price_aggregator import PriceAggregator
 
-steth_usd_median_feed = DataFeed(
-    query=SpotPrice(asset="STETH", currency="USD"),
+yfi_usd_median_feed = DataFeed(
+    query=SpotPrice(asset="YFI", currency="USD"),
     source=PriceAggregator(
-        asset="steth",
+        asset="yfi",
         currency="usd",
         algorithm="median",
         sources=[
-            CoinGeckoSpotPriceSource(asset="steth", currency="usd"),
-            UniswapV3PriceSource(asset="steth", currency="usd"),
+            CoinGeckoSpotPriceSource(asset="yfi", currency="usd"),
+            CoinbaseSpotPriceSource(asset="yfi", currency="usd"),
+            GeminiSpotPriceSource(asset="yfi", currency="usd"),
         ],
     ),
 )
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/sushi_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/sushi_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/tellor_rng_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/tellor_rng_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/trb_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/trb_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/twap_manual_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/twap_manual_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/uni_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/reth_usd_feed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from telliot_feeds.datafeed import DataFeed
 from telliot_feeds.queries.price.spot_price import SpotPrice
-from telliot_feeds.sources.price.spot.coinbase import CoinbaseSpotPriceSource
 from telliot_feeds.sources.price.spot.coingecko import CoinGeckoSpotPriceSource
-from telliot_feeds.sources.price.spot.gemini import GeminiSpotPriceSource
+from telliot_feeds.sources.price.spot.coinpaprika import CoinpaprikaSpotPriceSource
+from telliot_feeds.sources.price.spot.uniswapV3 import UniswapV3PriceSource
 from telliot_feeds.sources.price_aggregator import PriceAggregator
 
-uni_usd_median_feed = DataFeed(
-    query=SpotPrice(asset="UNI", currency="USD"),
+reth_usd_median_feed = DataFeed(
+    query=SpotPrice(asset="RETH", currency="USD"),
     source=PriceAggregator(
-        asset="uni",
+        asset="reth",
         currency="usd",
         algorithm="median",
         sources=[
-            CoinGeckoSpotPriceSource(asset="uni", currency="usd"),
-            CoinbaseSpotPriceSource(asset="uni", currency="usd"),
-            GeminiSpotPriceSource(asset="uni", currency="usd"),
+            CoinGeckoSpotPriceSource(asset="reth", currency="usd"),
+            CoinpaprikaSpotPriceSource(asset="reth-rocket-pool-eth", currency="usd"),
+            UniswapV3PriceSource(asset="reth", currency="usd"),
         ],
     ),
 )
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/usdc_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/usdc_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/usdt_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/usdt_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/vesq.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/vesq.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/feeds/xdai_usd_feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/feeds/xdai_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/flashbots/__init__.py` & `telliot_feeds-0.1.9/src/telliot_feeds/flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/flashbots/flashbots.py` & `telliot_feeds-0.1.9/src/telliot_feeds/flashbots/flashbots.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/flashbots/middleware.py` & `telliot_feeds-0.1.9/src/telliot_feeds/flashbots/middleware.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/flashbots/provider.py` & `telliot_feeds-0.1.9/src/telliot_feeds/flashbots/provider.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/flashbots/types.py` & `telliot_feeds-0.1.9/src/telliot_feeds/flashbots/types.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/abi.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/abi.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/cli.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/cli.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/contract.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/contract.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/feed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/generate_price_history_csv.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/generate_price_history_csv.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/pool.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/pool.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/report.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/report.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/sources.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/sources.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/integrations/diva_protocol/utils.py` & `telliot_feeds-0.1.9/src/telliot_feeds/integrations/diva_protocol/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/pricing/price_service.py` & `telliot_feeds-0.1.9/src/telliot_feeds/pricing/price_service.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/pricing/price_source.py` & `telliot_feeds-0.1.9/src/telliot_feeds/pricing/price_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/abi_query.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/abi_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/ampleforth/ampl_usd_vwap.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/ampleforth/ampl_usd_vwap.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/ampleforth/uspce.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/ampleforth/uspce.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/catalog.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/catalog.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/daily_volatility.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/daily_volatility.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/diva_protocol.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/diva_protocol.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/evm_call.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/evm_call.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/gas_price_oracle.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/gas_price_oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/json_query.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/json_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/legacy_query.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/legacy_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/mimicry.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/mimicry/collection_stat.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/numeric_api_response_query.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/numeric_api_response_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/price/spot_price.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/price/spot_price.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,17 @@
     "UNI/USD",
     "USDT/USD",
     "YFI/USD",
     "STETH/BTC",
     "STETH/USD",
     "RETH/BTC",
     "RETH/USD",
+    "WSTETH/USD",
+    "WSTETH/ETH",
+    "OP/USD",
 ]
 
 
 def format_spot_price_pairs() -> List[Tuple[str, str]]:
     """Read the list of valid spot price pairs"""
 
     pairs = []
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/price/twap.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/price/twap.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/query.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/query_catalog.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/query_catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from telliot_feeds.feeds.mimicry.macro_market_mashup_feed import COLLECTIONS
+from telliot_feeds.feeds.mimicry.macro_market_mashup_feed import TOKENS
 from telliot_feeds.queries.ampleforth.ampl_usd_vwap import AmpleforthCustomSpotPrice
 from telliot_feeds.queries.ampleforth.uspce import AmpleforthUSPCE
 from telliot_feeds.queries.catalog import Catalog
 from telliot_feeds.queries.daily_volatility import DailyVolatility
 from telliot_feeds.queries.diva_protocol import DIVAProtocol
 from telliot_feeds.queries.evm_call import EVMCall
 from telliot_feeds.queries.gas_price_oracle import GasPriceOracle
-from telliot_feeds.queries.mimicry import MimicryCollectionStat
+from telliot_feeds.queries.mimicry.collection_stat import MimicryCollectionStat
+from telliot_feeds.queries.mimicry.macro_market_mash_up import MimicryMacroMarketMashup
+from telliot_feeds.queries.mimicry.nft_market_index import MimicryNFTMarketIndex
 from telliot_feeds.queries.numeric_api_response_query import NumericApiResponse
 from telliot_feeds.queries.price.spot_price import SpotPrice
 from telliot_feeds.queries.price.twap import TWAP
 from telliot_feeds.queries.snapshot import Snapshot
 from telliot_feeds.queries.string_query import StringQuery
 from telliot_feeds.queries.tellor_rng import TellorRNG
 
@@ -292,14 +296,35 @@
 query_catalog.add_entry(
     tag="mimicry-crypto-coven-tami",
     title="Crypto Coven TAMI calculation for Mimicry",
     q=MimicryCollectionStat(collectionAddress="0x5180db8F5c931aaE63c74266b211F580155ecac8", chainId=1, metric=0),
 )
 
 query_catalog.add_entry(
+    tag="mimicry-nft-index-usd",
+    title="NFT Market Index usd",
+    q=MimicryNFTMarketIndex(chain="ethereum", currency="usd"),
+    active=True,
+)
+
+query_catalog.add_entry(
+    tag="mimicry-nft-index-eth",
+    title="NFT Market Index eth",
+    q=MimicryNFTMarketIndex(chain="ethereum", currency="eth"),
+    active=True,
+)
+
+query_catalog.add_entry(
+    tag="mimicry-mashup-example",
+    title="NFT market cap mashup",
+    q=MimicryMacroMarketMashup(metric="market-cap", currency="usd", collections=COLLECTIONS, tokens=TOKENS),
+    active=True,
+)
+
+query_catalog.add_entry(
     tag="steth-btc-spot",
     title="STETH/BTC spot price",
     q=SpotPrice(asset="steth", currency="btc"),
 )
 
 query_catalog.add_entry(
     tag="steth-usd-spot",
@@ -314,7 +339,25 @@
 )
 
 query_catalog.add_entry(
     tag="reth-usd-spot",
     title="RETH/USD spot price",
     q=SpotPrice(asset="reth", currency="usd"),
 )
+
+query_catalog.add_entry(
+    tag="wsteth-usd-spot",
+    title="WSTETH/USD spot price",
+    q=SpotPrice(asset="wsteth", currency="usd"),
+)
+
+query_catalog.add_entry(
+    tag="wsteth-eth-spot",
+    title="WSTETH/ETH spot price",
+    q=SpotPrice(asset="wsteth", currency="eth"),
+)
+
+query_catalog.add_entry(
+    tag="op-usd-spot",
+    title="OP/USD spot price",
+    q=SpotPrice(asset="op", currency="usd"),
+)
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/snapshot.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/snapshot.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/string_query.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/string_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/tellor/autopay_addresses.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/tellor/autopay_addresses.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/tellor/tellor_oracle_address.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/tellor/tellor_oracle_address.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/tellor_rng.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/tellor_rng.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/queries/utils.py` & `telliot_feeds-0.1.9/src/telliot_feeds/queries/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/custom_reporter.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/custom_reporter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/flashbot.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/flashbot.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/interval.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/interval.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/reporter_autopay_utils.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/reporter_autopay_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from telliot_feeds.reporters.tips import CATALOG_QUERY_IDS
 from telliot_feeds.utils.log import get_logger
 
 logger = get_logger(__name__)
 
 
 # chains where autopay contract is deployed
-AUTOPAY_CHAINS = (137, 80001, 69, 1666600000, 1666700000, 421611, 42161, 10200, 100, 10, 420, 421613, 3141)
+AUTOPAY_CHAINS = (137, 80001, 69, 1666600000, 1666700000, 421611, 42161, 10200, 100, 10, 420, 421613, 3141, 314)
 
 
 @dataclass
 class Tag:
     query_tag: str
     feed_id: str
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/rewards/time_based_rewards.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/rewards/time_based_rewards.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/rng_interval.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/rng_interval.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tellor_360.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tellor_360.py`

 * *Files 8% similar despite different names*

```diff
@@ -236,58 +236,55 @@
             msg = "Currently in reporter lock. Time left: " + hr_min_sec
             return error_status(msg, log=logger.info)
 
         return ResponseStatus()
 
     async def rewards(self) -> int:
         """Fetches total time based rewards plus tips for current datafeed"""
-        time_based_rewards: int = 0
-        fetch_autopay_tip: int = 0
-        total_rewards: int = 0
-
         if self.datafeed is not None:
             try:
                 qid = self.datafeed.query.query_id
-                fetch_autopay_tip = await fetch_feed_tip(self.autopay, qid)
+                self.autopaytip += await fetch_feed_tip(self.autopay, qid)
             except EncodingTypeError:
                 logger.warning(f"Unable to generate data/id for query: {self.datafeed.query}")
 
-            if fetch_autopay_tip is not None:
-                total_rewards += fetch_autopay_tip
-
         if self.chain_id in (1, 5):
             time_based_rewards = await get_time_based_rewards(self.oracle)
             if time_based_rewards is not None:
-                total_rewards += time_based_rewards
-
-        return total_rewards
+                self.autopaytip += time_based_rewards
+        return self.autopaytip
 
     async def fetch_datafeed(self) -> Optional[DataFeed[Any]]:
         """Fetches datafeed
 
         If the user did not select a query tag, there will have been no datafeed passed to
         the reporter upon instantiation.
         If the user uses the random feeds flag, the datafeed will be chosen randomly.
         If the user did not select a query tag or use the random feeds flag, the datafeed will
         be chosen based on the most funded datafeed in the AutoPay contract.
 
         If the no-rewards-check flag is used, the reporter will not check profitability or
         available tips for the datafeed unless the user has not selected a query tag or
         used the random feeds flag.
         """
+        # reset autopay tip every time fetch_datafeed is called
+        # so that tip is checked fresh every time and not carry older tips
+        self.autopaytip = 0
+        # TODO: This should be removed and moved to profit check method perhaps
+        if self.check_rewards:
+            # calculate tbr and
+            _ = await self.rewards()
+
         if self.use_random_feeds:
             self.datafeed = suggest_random_feed()
 
         # Fetch datafeed based on whichever is most funded in the AutoPay contract
         if self.datafeed is None:
             suggested_feed, tip_amount = await get_feed_and_tip(self.autopay)
 
-            if suggested_feed is not None:
-                self.autopaytip = tip_amount  # type: ignore
+            if suggested_feed is not None and tip_amount is not None:
+                self.autopaytip += tip_amount
+
                 self.datafeed = suggested_feed
                 return self.datafeed
 
-        # TODO: This should be removed and moved to profit check method perhaps
-        if self.check_rewards:
-            self.autopaytip = await self.rewards()
-
         return self.datafeed
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tellor_flex.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tellor_flex.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/__init__.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,12 +47,19 @@
     multicall3_address="0x08e08170712c7751b45b38865B97A50855c8ab13",
 )
 
 add_multicall_support(
     network="Filecoin Hyperspace Testnet",
     network_id=3141,
     state_override=False,
-    multicall3_address="0x08e08170712c7751b45b38865B97A50855c8ab13 ",
+    multicall3_address="0x08e08170712c7751b45b38865B97A50855c8ab13",
+)
+
+add_multicall_support(
+    network="Filecoin",
+    network_id=314,
+    state_override=False,
+    multicall3_address="0x5c691b93A8A77D9a36C1Cc8e4e08a4283d1665e1",
 )
 
 CATALOG_QUERY_IDS = {query_catalog._entries[tag].query.query_id: tag for tag in query_catalog._entries}
 CATALOG_QUERY_DATA = {query_catalog._entries[tag].query.query_data: tag for tag in query_catalog._entries}
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/assemble_call.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/assemble_call.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/dtypes.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/dtypes.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/funded_feeds.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/funded_feeds.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/funded_feeds_filter.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/funded_feeds_filter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/one_time_tips.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/one_time_tips.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/tip_listener_filter.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/tip_listener_filter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/listener/utils.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/listener/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/multicall_functions/call_functions.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/multicall_functions/call_functions.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/multicall_functions/multicall_autopay.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/multicall_functions/multicall_autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/suggest_datafeed.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/suggest_datafeed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/reporters/tips/tip_amount.py` & `telliot_feeds-0.1.9/src/telliot_feeds/reporters/tips/tip_amount.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/ampl_usd_vwap.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/ampl_usd_vwap.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/bitfinex.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/bitfinex.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/ampleforth/symbols.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/ampleforth/symbols.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/blockhash_aggregator.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/blockhash_aggregator.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/etherscan_gas.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/etherscan_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/evm_call.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/nft_market_index.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,85 @@
+import asyncio
 from dataclasses import dataclass
 from typing import Any
 from typing import Optional
 
-from hexbytes import HexBytes
+from requests.adapters import HTTPAdapter
+from requests.adapters import Retry
+from requests.exceptions import ConnectionError
+from requests.exceptions import HTTPError
+from requests.exceptions import RequestException
+from requests.exceptions import Timeout
+from requests.sessions import Session
 from telliot_core.apps.telliot_config import TelliotConfig
-from web3 import Web3
 
 from telliot_feeds.datasource import DataSource
 from telliot_feeds.dtypes.datapoint import datetime_now_utc
 from telliot_feeds.dtypes.datapoint import OptionalDataPoint
 from telliot_feeds.utils.log import get_logger
 
 
 logger = get_logger(__name__)
 
+retry_strat = Retry(total=3, backoff_factor=0.5, status_forcelist=[500, 502, 503, 504])
+adapter = HTTPAdapter(max_retries=retry_strat)
+
 
 @dataclass
-class EVMCallSource(DataSource[Any]):
-    """DataSource for returning the result of a read function on an EVM contract."""
+class NFTGoSource(DataSource[str]):
+    """DataSource for NFTGo expected response data.
+    For testing purposes this endpoint can be used to check the numbers:
+    https://runkit.io/aslangoldenhour/calculate-nft-market-index-via-nftgo/branches/master?queryData
+    """
 
-    chainId: Optional[int] = None
-    contractAddress: Optional[str] = None  # example: '0x1234567890123456789012345678901234567890'
-    calldata: Optional[bytes] = None
-    web3: Optional[Web3] = None
-    cfg: TelliotConfig = TelliotConfig()
-
-    def update_web3(self) -> None:
-        """Return a web3 instance for the given chain ID."""
-        if not self.chainId:
-            raise ValueError("Chain ID not provided")
-
-        eps = self.cfg.endpoints.find(chain_id=self.chainId)
-        if len(eps) > 0:
-            endpoint = eps[0]
-        else:
-            raise ValueError(f"Endpoint not found for chain_id={self.chainId}")
-
-        if not endpoint.connect():
-            raise Exception(f"Endpoint not connected for chain_id={self.chainId}")
-
-        self.web3 = endpoint.web3
-
-    def get_response(self) -> Optional[Any]:
-        """Return the response from the EVM contract."""
-        if not self.contractAddress:
-            raise ValueError("Contract address not provided")
-        if not self.calldata:
-            raise ValueError("Calldata not provided")
-        if not self.web3:
-            raise ValueError("Web3 not provided")
+    currency: Optional[str] = None
 
-        # convert address to checksum address
-        self.contractAddress = self.web3.toChecksumAddress(self.contractAddress)
+    async def fetch_nftgo_api(self) -> Optional[Any]:
+        """
+        Request NFTGo data from the api
+        """
+        api_key = TelliotConfig().api_keys.find(name="nftgo")
+        if not api_key:
+            logger.info("API key required for NFTGo API to fetch collection market cap.")
+            return None
+        url = "https://data-api.nftgo.io/eth/v1/market/rank/collection/all"
+        headers = {"X-API-KEY": api_key[0].key, "accept": "application/json"}
+        params = {"by": "market_cap", "with_rarity": "false", "asc": "false", "offset": 0, "limit": 50}
+
+        with Session() as session:
+            session.headers.update(headers)
+            session.mount("https://", adapter)
+            try:
+                response = session.get(url, params=params, timeout=(5, 10))  # type: ignore
+                response.raise_for_status()
+            except (HTTPError, Timeout, ConnectionError, RequestException) as e:
+                logger.error(f"Request errored: {e}.")
+                return None
 
         try:
-            result = self.web3.eth.call({"gasPrice": 0, "to": self.contractAddress, "data": self.calldata}, "latest")
-        except Exception as e:
-            if e.__module__.startswith("web3"):
-                logger.warning(f"Web3 exception occurred: {e}")
-                return (None, None)
-            raise e
-
-        if result is None or not isinstance(result, HexBytes):
-            raise ValueError(f"Result is not bytes: {str(result)}")
-
-        if result == HexBytes("0x"):
-            logger.info("Result is empty bytes, likely tried to call a non-view function")
-            return (None, None)
-
-        logger.info(f"EVMCallSource result bytes: {result.hex()}")
-
-        ts = int(datetime_now_utc().timestamp())
-        return (result, ts)
+            collection = response.json()["collections"]
+            return collection
+        except KeyError as e:
+            logger.error(f"Bad API response fetching top 50 collections market caps: {e}.")
+            return None
 
     async def fetch_new_datapoint(self) -> OptionalDataPoint[Any]:
-        """Update current value with time-stamped value fetched from EVM contract.
-
-        Returns:
-            Current time-stamped value
-        """
-        try:
-            self.update_web3()
-        except Exception as e:
-            logger.warning(f"Error occurred while updating web3 instance: {e}")
+        """Fetch new data point from NFTGo API."""
+        collections = await self.fetch_nftgo_api()
+        if collections is None:
+            logger.error("Failed to fetch collections details from NFTGo API.")
             return None, None
-
         try:
-            val = self.get_response()
+            market_cap = sum(cap[f"market_cap_{self.currency}"] for cap in collections)
         except Exception as e:
-            logger.warning(f"Error occurred while getting response: {e}")
+            logger.error(f"Failed to calculate total market cap for top 50 collections: {e}")
             return None, None
-
-        datapoint = (val, datetime_now_utc())
+        datapoint = (market_cap, datetime_now_utc())
         self.store_datapoint(datapoint)
-
         return datapoint
+
+
+if __name__ == "__main__":
+    source = NFTGoSource(currency="usd")
+    print(asyncio.run(source.fetch_new_datapoint()))
+    # https://docs.nftgo.io/docs/faq##Currently,
+    # NFTGo supports the Ethereum blockchain and is looking to support more mainstream blockchains in time to come.
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/gas_price_oracle.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/gas_price_oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/daily_volatility_manual_source.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/daily_volatility_manual_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/diva_manual_source.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/diva_manual_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/numeric_api_manual_response.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/numeric_api_manual_response.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/snapshot.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/snapshot.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/spot_price_input_source.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/spot_price_input_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/string_query_manual_source.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/string_query_manual_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/tellor_rng_manual_source.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/tellor_rng_manual_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/twap_manual_input_source.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/twap_manual_input_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/manual/uspce.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/manual/uspce.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/collection_stat.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/collection_stat.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/tami.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/tami.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/types.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/types.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/mimicry/utils.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/mimicry/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/numeric_api_response.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/numeric_api_response.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/currency/coinbase.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/currency/coinbase.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/currency/openexchangerate.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/currency/openexchangerate.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/coingecko_daily.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/coingecko_daily.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/cryptowatch.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/cryptowatch.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/cryptowatch_ohlc.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/cryptowatch_ohlc.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/kraken.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/kraken.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/kraken_ohlc.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/kraken_ohlc.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/historical/poloniex.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/historical/poloniex.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/binance.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/binance.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/bitfinex.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/bitfinex.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/bitflyer.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/bitflyer.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/bittrex.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/bittrex.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/coinbase.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/coinbase.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/coingecko.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/coingecko.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     "ltc": "litecoin",
     "shib": "shiba-inu",
     "uni": "uniswap",
     "usdt": "tether",
     "yfi": "yearn-finance",
     "steth": "staked-ether",
     "reth": "rocket-pool-eth",
+    "op": "optimism",
 }
 
 
 class CoinGeckoSpotPriceService(WebPriceService):
     """CoinGecko Price Service"""
 
     def __init__(self, **kwargs: Any) -> None:
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/coinmarketcap.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/gemini.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/gemini.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             logger.error(d)
             return None, None
 
         else:
             try:
                 r = GeminiPriceResponse(**d["response"])
             except Exception as e:
-                logger.error("Error parsing response from Gemini API:", e)
+                logger.error(f"Error parsing response from Gemini API: {e}")
                 return None, None
 
             if r.last is not None:
                 return float(r.last), datetime_now_utc()
             else:
                 logger.error(r)
                 return None, None
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/kraken.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/kraken.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/nomics.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/nomics.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/pancakeswap.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/pancakeswap.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/pulsechain_subgraph.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/pulsechain_subgraph.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price/spot/uniswapV3.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price/spot/uniswapV3.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/sources/price_aggregator.py` & `telliot_feeds-0.1.9/src/telliot_feeds/sources/price_aggregator.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/abi.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/abi.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/cfg.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/cfg.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/contract.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/contract.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/decode.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/decode.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/input_timeout.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/input_timeout.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/log.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/log.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/reporter_utils.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/reporter_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,13 @@
 
     # prevent division by zero in the extremely unlikely case that all fees within the polled fee
     # history range for the specified percentile are 0
     divisor = len(non_empty_block_fees) if len(non_empty_block_fees) != 0 else 1
 
     priority_fee_average_for_percentile = Wei(round(sum(non_empty_block_fees) / divisor))
 
-    return (  # keep estimated priority fee within a max / min range
-        priority_fee_max
-        if priority_fee_average_for_percentile > priority_fee_max
-        else priority_fee_min
-        if priority_fee_average_for_percentile < priority_fee_min
-        else priority_fee_average_for_percentile
-    )
+    if priority_fee_average_for_percentile > priority_fee_max:
+        return priority_fee_max
+    elif priority_fee_average_for_percentile < priority_fee_min:
+        return priority_fee_min
+    else:
+        return priority_fee_average_for_percentile
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds/utils/stdev_calculator.py` & `telliot_feeds-0.1.9/src/telliot_feeds/utils/stdev_calculator.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds.egg-info/PKG-INFO` & `telliot_feeds-0.1.9/src/telliot_feeds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot-feeds
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for interacting with Tellor Protocol smart contracts.
 Home-page: https://github.com/tellor-io/telliot-feeds
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,ethereum,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds.egg-info/SOURCES.txt` & `telliot_feeds-0.1.9/src/telliot_feeds.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -105,19 +105,19 @@
 src/telliot_feeds/feeds/fil_usd_feed.py
 src/telliot_feeds/feeds/gas_price_oracle_feed.py
 src/telliot_feeds/feeds/gno_usd_feed.py
 src/telliot_feeds/feeds/idle_usd_feed.py
 src/telliot_feeds/feeds/link_usd_feed.py
 src/telliot_feeds/feeds/ltc_usd_feed.py
 src/telliot_feeds/feeds/matic_usd_feed.py
-src/telliot_feeds/feeds/mimicry_feed.py
 src/telliot_feeds/feeds/mkr_usd_feed.py
 src/telliot_feeds/feeds/numeric_api_response_feed.py
 src/telliot_feeds/feeds/numeric_api_response_manual_feed.py
 src/telliot_feeds/feeds/olympus.py
+src/telliot_feeds/feeds/op_usd_feed.py
 src/telliot_feeds/feeds/pls_usd_feed.py
 src/telliot_feeds/feeds/rai_usd_feed.py
 src/telliot_feeds/feeds/reth_btc_feed.py
 src/telliot_feeds/feeds/reth_usd_feed.py
 src/telliot_feeds/feeds/ric_usd_feed.py
 src/telliot_feeds/feeds/shib_usd_feed.py
 src/telliot_feeds/feeds/snapshot_feed.py
@@ -131,16 +131,21 @@
 src/telliot_feeds/feeds/trb_usd_feed.py
 src/telliot_feeds/feeds/twap_manual_feed.py
 src/telliot_feeds/feeds/uni_usd_feed.py
 src/telliot_feeds/feeds/usdc_usd_feed.py
 src/telliot_feeds/feeds/usdt_usd_feed.py
 src/telliot_feeds/feeds/uspce_feed.py
 src/telliot_feeds/feeds/vesq.py
+src/telliot_feeds/feeds/wsteth_feed.py
 src/telliot_feeds/feeds/xdai_usd_feed.py
 src/telliot_feeds/feeds/yfi_usd_feed.py
+src/telliot_feeds/feeds/mimicry/__init__.py
+src/telliot_feeds/feeds/mimicry/collection_stat_feed.py
+src/telliot_feeds/feeds/mimicry/macro_market_mashup_feed.py
+src/telliot_feeds/feeds/mimicry/nft_index_feed.py
 src/telliot_feeds/flashbots/__init__.py
 src/telliot_feeds/flashbots/flashbots.py
 src/telliot_feeds/flashbots/middleware.py
 src/telliot_feeds/flashbots/provider.py
 src/telliot_feeds/flashbots/types.py
 src/telliot_feeds/integrations/__init__.py
 src/telliot_feeds/integrations/diva_protocol/__init__.py
@@ -162,25 +167,28 @@
 src/telliot_feeds/queries/daily_volatility.py
 src/telliot_feeds/queries/diva_protocol.py
 src/telliot_feeds/queries/evm_call.py
 src/telliot_feeds/queries/export_query_catalog.py
 src/telliot_feeds/queries/gas_price_oracle.py
 src/telliot_feeds/queries/json_query.py
 src/telliot_feeds/queries/legacy_query.py
-src/telliot_feeds/queries/mimicry.py
 src/telliot_feeds/queries/numeric_api_response_query.py
 src/telliot_feeds/queries/query.py
 src/telliot_feeds/queries/query_catalog.py
 src/telliot_feeds/queries/snapshot.py
 src/telliot_feeds/queries/string_query.py
 src/telliot_feeds/queries/tellor_rng.py
 src/telliot_feeds/queries/utils.py
 src/telliot_feeds/queries/ampleforth/__init__.py
 src/telliot_feeds/queries/ampleforth/ampl_usd_vwap.py
 src/telliot_feeds/queries/ampleforth/uspce.py
+src/telliot_feeds/queries/mimicry/__init__.py
+src/telliot_feeds/queries/mimicry/collection_stat.py
+src/telliot_feeds/queries/mimicry/macro_market_mash_up.py
+src/telliot_feeds/queries/mimicry/nft_market_index.py
 src/telliot_feeds/queries/price/__init__.py
 src/telliot_feeds/queries/price/spot_price.py
 src/telliot_feeds/queries/price/twap.py
 src/telliot_feeds/queries/tellor/autopay_addresses.py
 src/telliot_feeds/queries/tellor/tellor_oracle_address.py
 src/telliot_feeds/reporters/__init__.py
 src/telliot_feeds/reporters/custom_reporter.py
@@ -209,14 +217,15 @@
 src/telliot_feeds/sources/__init__.py
 src/telliot_feeds/sources/blockhash_aggregator.py
 src/telliot_feeds/sources/etherscan_gas.py
 src/telliot_feeds/sources/evm_call.py
 src/telliot_feeds/sources/gas_price_oracle.py
 src/telliot_feeds/sources/numeric_api_response.py
 src/telliot_feeds/sources/price_aggregator.py
+src/telliot_feeds/sources/wsteth_source.py
 src/telliot_feeds/sources/ampleforth/__init__.py
 src/telliot_feeds/sources/ampleforth/ampl_usd_vwap.py
 src/telliot_feeds/sources/ampleforth/bitfinex.py
 src/telliot_feeds/sources/ampleforth/symbols.py
 src/telliot_feeds/sources/manual/__init__.py
 src/telliot_feeds/sources/manual/daily_volatility_manual_source.py
 src/telliot_feeds/sources/manual/diva_manual_source.py
@@ -225,14 +234,16 @@
 src/telliot_feeds/sources/manual/spot_price_input_source.py
 src/telliot_feeds/sources/manual/string_query_manual_source.py
 src/telliot_feeds/sources/manual/tellor_rng_manual_source.py
 src/telliot_feeds/sources/manual/twap_manual_input_source.py
 src/telliot_feeds/sources/manual/uspce.py
 src/telliot_feeds/sources/mimicry/__init__.py
 src/telliot_feeds/sources/mimicry/collection_stat.py
+src/telliot_feeds/sources/mimicry/mashup_source.py
+src/telliot_feeds/sources/mimicry/nft_market_index.py
 src/telliot_feeds/sources/mimicry/tami.py
 src/telliot_feeds/sources/mimicry/types.py
 src/telliot_feeds/sources/mimicry/utils.py
 src/telliot_feeds/sources/price/__init__.py
 src/telliot_feeds/sources/price/currency/__init__.py
 src/telliot_feeds/sources/price/currency/coinbase.py
 src/telliot_feeds/sources/price/currency/openexchangerate.py
@@ -247,14 +258,16 @@
 src/telliot_feeds/sources/price/spot/binance.py
 src/telliot_feeds/sources/price/spot/bitfinex.py
 src/telliot_feeds/sources/price/spot/bitflyer.py
 src/telliot_feeds/sources/price/spot/bittrex.py
 src/telliot_feeds/sources/price/spot/coinbase.py
 src/telliot_feeds/sources/price/spot/coingecko.py
 src/telliot_feeds/sources/price/spot/coinmarketcap.py
+src/telliot_feeds/sources/price/spot/coinpaprika.py
+src/telliot_feeds/sources/price/spot/curvefi.py
 src/telliot_feeds/sources/price/spot/gemini.py
 src/telliot_feeds/sources/price/spot/kraken.py
 src/telliot_feeds/sources/price/spot/nomics.py
 src/telliot_feeds/sources/price/spot/pancakeswap.py
 src/telliot_feeds/sources/price/spot/pulsechain_subgraph.py
 src/telliot_feeds/sources/price/spot/uniswapV3.py
 src/telliot_feeds/utils/__init__.py
@@ -297,24 +310,26 @@
 tests/feeds/test_eur_usd_feed.py
 tests/feeds/test_gas_price_oracle_feed.py
 tests/feeds/test_idle_usd_feed.py
 tests/feeds/test_manual_snapshot_feed.py
 tests/feeds/test_matic_usd_feed.py
 tests/feeds/test_mimicry_feed.py
 tests/feeds/test_mkr_usd_feed.py
+tests/feeds/test_op_usd_feed.py
 tests/feeds/test_pop_spot_price_feeds.py
 tests/feeds/test_reth_btc_feed.py
 tests/feeds/test_reth_usd_feed.py
 tests/feeds/test_ric_usd_feed.py
 tests/feeds/test_steth_btc_feed.py
 tests/feeds/test_steth_usd_feed.py
 tests/feeds/test_sushi_usd_feed.py
 tests/feeds/test_trb_usd_feed.py
 tests/feeds/test_usdc_usd_feed.py
 tests/feeds/test_uspce_feed.py
+tests/feeds/test_wsteth_feed.py
 tests/integrations/diva_protocol/test_construct_datafeed.py
 tests/integrations/diva_protocol/test_diva_contracts.py
 tests/integrations/diva_protocol/test_e2e_create_report_settle_pool.py
 tests/integrations/diva_protocol/test_get_pools.py
 tests/integrations/diva_protocol/test_report.py
 tests/integrations/diva_protocol/utils.py
 tests/queries/test_abi_query.py
@@ -324,14 +339,16 @@
 tests/queries/test_query_catalog.py
 tests/queries/test_query_daily_volatility.py
 tests/queries/test_query_diva_protocol.py
 tests/queries/test_query_evm_call.py
 tests/queries/test_query_gas_price_oracle.py
 tests/queries/test_query_legacy_query.py
 tests/queries/test_query_mimicry.py
+tests/queries/test_query_mimicry_mashup.py
+tests/queries/test_query_mimicry_nft_index.py
 tests/queries/test_query_numeric_api_response.py
 tests/queries/test_query_snapshot.py
 tests/queries/test_query_spot_price.py
 tests/queries/test_query_string_query.py
 tests/queries/test_query_support.py
 tests/queries/test_query_tellor_addresses.py
 tests/queries/test_query_tellor_rng.py
```

### Comparing `telliot_feeds-0.1.8/src/telliot_feeds.egg-info/requires.txt` & `telliot_feeds-0.1.9/src/telliot_feeds.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 python-dateutil==2.8.1
 python-dotenv==0.21.0
 PyYAML==6.0
 requests==2.28.1
 rlp==2.0.1
 simple-term-menu==1.5.2
 six==1.16.0
-telliot-core==0.2.3
+telliot-core==0.2.4
 toolz==0.12.0
 typing_extensions==4.4.0
 urllib3==1.26.12
 varint==1.0.2
 web3==5.28.0
 websockets==9.1
 yarl==1.8.1
```

### Comparing `telliot_feeds-0.1.8/tests/cli/test_cli.py` & `telliot_feeds-0.1.9/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/cli/test_diva_cli.py` & `telliot_feeds-0.1.9/tests/cli/test_diva_cli.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/cli/test_query_cmd.py` & `telliot_feeds-0.1.9/tests/cli/test_query_cmd.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/conftest.py` & `telliot_feeds-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_bct_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_bct_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_btc_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_btc_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_diva_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_diva_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_eth_btc_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_eth_btc_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_eth_jpy_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_eth_jpy_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_eth_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_eth_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_gas_price_oracle_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_gas_price_oracle_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_idle_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_idle_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_manual_snapshot_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_manual_snapshot_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_matic_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_matic_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_mkr_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_mkr_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_pop_spot_price_feeds.py` & `telliot_feeds-0.1.9/tests/feeds/test_pop_spot_price_feeds.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_reth_btc_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_reth_btc_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_reth_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_reth_usd_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @pytest.mark.asyncio
 async def test_reth_usd_median_feed(caplog):
     """Retrieve median RETH/USD price."""
     v, _ = await reth_usd_median_feed.source.fetch_new_datapoint()
 
     assert v is not None
     assert v > 0
-    assert "sources used in aggregate: 2" in caplog.text.lower()
+    assert "sources used in aggregate: 3" in caplog.text.lower()
     print(f"RETH/USD Price: {v}")
 
     # Get list of data sources from sources dict
     source_prices = [source.latest[0] for source in reth_usd_median_feed.source.sources if source.latest[0]]
 
     # Make sure error is less than decimal tolerance
     assert (v - statistics.median(source_prices)) < 10**-6
```

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_ric_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_ric_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_steth_btc_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_steth_btc_feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @pytest.mark.asyncio
 async def test_steth_btc_median_feed(caplog):
     """Retrieve median STETH/BTC price."""
     v, _ = await steth_btc_median_feed.source.fetch_new_datapoint()
 
     assert v is not None
     assert v > 0
-    assert "sources used in aggregate: 1" in caplog.text.lower()
+    assert "sources used in aggregate: 3" in caplog.text.lower()
     print(f"STETH/BTC Price: {v}")
 
     # Get list of data sources from sources dict
     source_prices = [source.latest[0] for source in steth_btc_median_feed.source.sources if source.latest[0]]
 
     # Make sure error is less than decimal tolerance
     assert (v - statistics.median(source_prices)) < 10**-6
```

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_steth_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_steth_usd_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @pytest.mark.asyncio
 async def test_steth_usd_median_feed(caplog):
     """Retrieve median STETH/USD price."""
     v, _ = await steth_usd_median_feed.source.fetch_new_datapoint()
 
     assert v is not None
     assert v > 0
-    assert "sources used in aggregate: 2" in caplog.text.lower()
+    assert "sources used in aggregate: 4" in caplog.text.lower()
     print(f"STETH/USD Price: {v}")
 
     # Get list of data sources from sources dict
     source_prices = [source.latest[0] for source in steth_usd_median_feed.source.sources if source.latest[0]]
 
     # Make sure error is less than decimal tolerance
     assert (v - statistics.median(source_prices)) < 10**-6
```

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_sushi_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_sushi_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_trb_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_trb_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/feeds/test_usdc_usd_feed.py` & `telliot_feeds-0.1.9/tests/feeds/test_usdc_usd_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_construct_datafeed.py` & `telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_construct_datafeed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_diva_contracts.py` & `telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_diva_contracts.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_e2e_create_report_settle_pool.py` & `telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_e2e_create_report_settle_pool.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_get_pools.py` & `telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_get_pools.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/integrations/diva_protocol/test_report.py` & `telliot_feeds-0.1.9/tests/integrations/diva_protocol/test_report.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/integrations/diva_protocol/utils.py` & `telliot_feeds-0.1.9/tests/integrations/diva_protocol/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_abi_query.py` & `telliot_feeds-0.1.9/tests/queries/test_abi_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_ampl_usd_vwap.py` & `telliot_feeds-0.1.9/tests/queries/test_query_ampl_usd_vwap.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_base.py` & `telliot_feeds-0.1.9/tests/queries/test_query_base.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_catalog.py` & `telliot_feeds-0.1.9/tests/queries/test_query_catalog.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_daily_volatility.py` & `telliot_feeds-0.1.9/tests/queries/test_query_daily_volatility.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_diva_protocol.py` & `telliot_feeds-0.1.9/tests/queries/test_query_diva_protocol.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_evm_call.py` & `telliot_feeds-0.1.9/tests/queries/test_query_evm_call.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_gas_price_oracle.py` & `telliot_feeds-0.1.9/tests/queries/test_query_gas_price_oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_legacy_query.py` & `telliot_feeds-0.1.9/tests/queries/test_query_legacy_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_mimicry.py` & `telliot_feeds-0.1.9/tests/queries/test_query_mimicry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Unit tests for MimicryCollectionStat queries.
 
 Copyright (c) 2021-, Tellor Development Community
 Distributed under the terms of the MIT License.
 """
 from eth_abi import decode_abi
 
-from telliot_feeds.queries.mimicry import MimicryCollectionStat
+from telliot_feeds.queries.mimicry.collection_stat import MimicryCollectionStat
 
 
 def test_query_constructor():
     """Validate MimicryCollectionStat query."""
     q = MimicryCollectionStat(chainId=1, collectionAddress="0x495f947276749ce646f68ac8c248420045cb7b5e", metric=1)
 
     exp_query_data = bytes.fromhex(
```

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_numeric_api_response.py` & `telliot_feeds-0.1.9/tests/queries/test_query_numeric_api_response.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_snapshot.py` & `telliot_feeds-0.1.9/tests/queries/test_query_snapshot.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_spot_price.py` & `telliot_feeds-0.1.9/tests/queries/test_query_spot_price.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_string_query.py` & `telliot_feeds-0.1.9/tests/queries/test_query_string_query.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_support.py` & `telliot_feeds-0.1.9/tests/queries/test_query_support.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_tellor_addresses.py` & `telliot_feeds-0.1.9/tests/queries/test_query_tellor_addresses.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_tellor_rng.py` & `telliot_feeds-0.1.9/tests/queries/test_query_tellor_rng.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_twap.py` & `telliot_feeds-0.1.9/tests/queries/test_query_twap.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/queries/test_query_uspce.py` & `telliot_feeds-0.1.9/tests/queries/test_query_uspce.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/reporters/test_360_reporter.py` & `telliot_feeds-0.1.9/tests/reporters/test_360_reporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import math
 import time
 from datetime import timedelta
 from unittest import mock
+from unittest.mock import AsyncMock
+from unittest.mock import patch
 
 import pytest
 
 from telliot_feeds.feeds.eth_usd_feed import eth_usd_median_feed
+from telliot_feeds.feeds.matic_usd_feed import matic_usd_median_feed
 from telliot_feeds.feeds.snapshot_feed import snapshot_manual_feed
 from telliot_feeds.reporters.rewards.time_based_rewards import get_time_based_rewards
 from telliot_feeds.reporters.tellor_360 import Tellor360Reporter
 
 
 txn_kwargs = {"gas_limit": 3500000, "legacy_gas_price": 1}
 CHAIN_ID = 80001
@@ -272,7 +275,54 @@
     # trying to generate the query data for the query id.
     eth_usd_median_feed.query.asset = None
 
     reporter = Tellor360Reporter(**reporter_kwargs)
     _ = await reporter.rewards()
 
     assert "Unable to generate data/id for query" in caplog.text
+
+
+@pytest.mark.asyncio
+async def test_tbr_tip_increment(tellor_360, guaranteed_price_source, caplog):
+    contracts, account = tellor_360
+    feed = eth_usd_median_feed
+    feed.source = guaranteed_price_source
+    matic_usd_median_feed.source = guaranteed_price_source
+
+    _ = await contracts.autopay.write(
+        "tip",
+        **txn_kwargs,
+        _amount=1 * 10**18,
+        _queryId=matic_usd_median_feed.query.query_id,
+        _queryData=matic_usd_median_feed.query.query_data,
+    )
+    reporter_kwargs = {
+        "oracle": contracts.oracle,
+        "token": contracts.token,
+        "autopay": contracts.autopay,
+        "endpoint": contracts.oracle.node,
+        "account": account,
+        "chain_id": 5,  # set chain id to 5 so it checks tbr
+        "transaction_type": 0,
+        "wait_period": 0,
+        "min_native_token_balance": 0,
+        "expected_profit": 1000.0,  # set expected profit high so it won't report
+    }
+
+    def mock_tbr():
+        current_number = 0
+        while True:
+            yield current_number
+            current_number += 1e18
+
+    generator = mock_tbr()
+    mock_async_tbr = AsyncMock(side_effect=lambda _: next(generator))
+
+    reporter = Tellor360Reporter(**reporter_kwargs)
+    assert reporter.check_rewards
+
+    with patch("telliot_feeds.reporters.tellor_360.get_time_based_rewards", mock_async_tbr):
+        await reporter.report(report_count=3)
+        # tip amount should increase by 1e18 each time and not more
+        assert "Tips: 1.0" in caplog.text
+        assert "Tips: 2.0" in caplog.text
+        assert "Tips: 3.0" in caplog.text
```

### Comparing `telliot_feeds-0.1.8/tests/reporters/test_autopay_multicalls.py` & `telliot_feeds-0.1.9/tests/reporters/test_autopay_multicalls.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/reporters/test_custom_360_reporter.py` & `telliot_feeds-0.1.9/tests/reporters/test_custom_360_reporter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/reporters/test_flashbot_reporter.py` & `telliot_feeds-0.1.9/tests/reporters/test_flashbot_reporter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/reporters/test_flex_reporter.py` & `telliot_feeds-0.1.9/tests/reporters/test_flex_reporter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/reporters/test_interval_reporter.py` & `telliot_feeds-0.1.9/tests/reporters/test_interval_reporter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/reporters/test_rng_reporter.py` & `telliot_feeds-0.1.9/tests/reporters/test_rng_reporter.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/manual/test_diva_manual_entry_source.py` & `telliot_feeds-0.1.9/tests/sources/manual/test_diva_manual_entry_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/manual/test_rng_manual_input_source.py` & `telliot_feeds-0.1.9/tests/sources/manual/test_rng_manual_input_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/manual/test_spot_price_manual_source.py` & `telliot_feeds-0.1.9/tests/sources/manual/test_spot_price_manual_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/manual/test_string_query_manual_source.py` & `telliot_feeds-0.1.9/tests/sources/manual/test_string_query_manual_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/manual/test_twap_manual_source.py` & `telliot_feeds-0.1.9/tests/sources/manual/test_twap_manual_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/manual/test_uspce_source.py` & `telliot_feeds-0.1.9/tests/sources/manual/test_uspce_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_ampl_usd_vwap_source.py` & `telliot_feeds-0.1.9/tests/sources/test_ampl_usd_vwap_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_curr_exchange_sources.py` & `telliot_feeds-0.1.9/tests/sources/test_curr_exchange_sources.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_etherscan_gas.py` & `telliot_feeds-0.1.9/tests/sources/test_etherscan_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_gas_price_oracle_source.py` & `telliot_feeds-0.1.9/tests/sources/test_gas_price_oracle_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_historical_price_sources.py` & `telliot_feeds-0.1.9/tests/sources/test_historical_price_sources.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_source_numeric_api_response.py` & `telliot_feeds-0.1.9/tests/sources/test_source_numeric_api_response.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_spot_price_sources.py` & `telliot_feeds-0.1.9/tests/sources/test_spot_price_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 from unittest import mock
 
 import pytest
 from requests import Response
 from requests.exceptions import JSONDecodeError
 from telliot_core.apps.telliot_config import TelliotConfig
 
-from telliot_feeds.sources.price.spot import coingecko
 from telliot_feeds.sources.price.spot.bitfinex import BitfinexSpotPriceService
 from telliot_feeds.sources.price.spot.bittrex import BittrexSpotPriceService
 from telliot_feeds.sources.price.spot.coinbase import CoinbaseSpotPriceService
 from telliot_feeds.sources.price.spot.coingecko import CoinGeckoSpotPriceService
 from telliot_feeds.sources.price.spot.coinmarketcap import CoinMarketCapSpotPriceService
+from telliot_feeds.sources.price.spot.coinpaprika import CoinpaprikaSpotPriceService
+from telliot_feeds.sources.price.spot.curvefi import CurveFinanceSpotPriceService
 from telliot_feeds.sources.price.spot.gemini import GeminiSpotPriceService
 from telliot_feeds.sources.price.spot.kraken import KrakenSpotPriceService
 from telliot_feeds.sources.price.spot.nomics import NomicsSpotPriceService
 from telliot_feeds.sources.price.spot.pancakeswap import (
     PancakeswapPriceService,
 )
 from telliot_feeds.sources.price.spot.pulsechain_subgraph import PulsechainSupgraphService
@@ -34,14 +35,16 @@
     "nomics": NomicsSpotPriceService(),
     "pancakeswap": PancakeswapPriceService(),
     "uniswapV3": UniswapV3PriceService(),
     "pulsechain-subgraph": PulsechainSupgraphService(),
     "kraken": KrakenSpotPriceService(),
     "coinmarketcap": CoinMarketCapSpotPriceService(),
     "bitfinex": BitfinexSpotPriceService(),
+    "coinpaprika": CoinpaprikaSpotPriceService(),
+    "curvefi": CurveFinanceSpotPriceService(),
 }
 
 
 async def get_price(asset, currency, s, timeout=10.0):
     """Helper function for retrieving prices."""
     s.timeout = timeout
     v, t = await s.get_price(asset, currency)
@@ -260,36 +263,54 @@
     """Test retreiving from Pulsechain Subgraph PLS/USD feed"""
     v, t = await get_price("pls", "usd", service["pulsechain-subgraph"])
     validate_price(v, t)
 
 
 @pytest.mark.asyncio
 async def test_coingecko_price_service_rate_limit(caplog):
-    def mock_get_url(self, url):
+    def mock_get_url(self, url=""):
         return {
             "error": "<class 'requests.exceptions.JSONDecodeError'>",
             "exception": JSONDecodeError(
                 "CoinGecko API rate limit exceeded",
                 '<!DOCTYPE html>\n<!--[if lt IE 7]> <html class="no-js ie6 oldie" lang="en-US"> <![endif]-->\n<!--[if IE 7]>    <html class="no-js ie7 oldie" lang="en-US"> <![endif]-->\n<!--[if IE 8]>    <html class="no-js ie8 oldie" lang="en-US"> <![endif]-->\n<!--[if gt IE 8]><!--> <html class="no-js" lang="en-US"> <!--<![endif]-->\n<head>\n<title>Access denied | api.coingecko.com used Cloudflare to restrict access</title>\n<meta charset="UTF-8" />\n<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />\n<meta http-equiv="X-UA-Compatible" content="IE=Edge,chrome=1" />\n<meta name="robots" content="noindex, nofollow" />\n<meta name="viewport" content="width=device-width,initial-scale=1" />\n<link rel="stylesheet" id="cf_styles-css" href="/cdn-cgi/styles/main.css" type="text/css" media="screen,projection" />\n\n\n<script type="text/javascript">\n(function(){if(document.addEventListener&&window.XMLHttpRequest&&JSON&&JSON.stringify){var e=function(a){var c=document.getElementById("error-feedback-survey"),d=document.getElementById("error-feedback-success"),b=new XMLHttpRequest;a={event:"feedback clicked",properties:{errorCode:1015,helpful:a,version:1}};b.open("POST","https://sparrow.cloudflare.com/api/v1/event");b.setRequestHeader("Content-Type","application/json");b.setRequestHeader("Sparrow-Source-Key","c771f0e4b54944bebf4261d44bd79a1e");\nb.send(JSON.stringify(a));c.classList.add("feedback-hidden");d.classList.remove("feedback-hidden")};document.addEventListener("DOMContentLoaded",function(){var a=document.getElementById("error-feedback"),c=document.getElementById("feedback-button-yes"),d=document.getElementById("feedback-button-no");"classList"in a&&(a.classList.remove("feedback-hidden"),c.addEventListener("click",function(){e(!0)}),d.addEventListener("click",function(){e(!1)}))})}})();\n</script>\n\n<script defer src="https://api.radar.cloudflare.com/beacon.js"></script>\n</head>\n<body>\n  <div id="cf-wrapper">\n    <div class="cf-alert cf-alert-error cf-cookie-error hidden" id="cookie-alert" data-translate="enable_cookies">Please enable cookies.</div>\n    <div id="cf-error-details" class="p-0">\n      <header class="mx-auto pt-10 lg:pt-6 lg:px-8 w-240 lg:w-full mb-15 antialiased">\n         <h1 class="inline-block md:block mr-2 md:mb-2 font-light text-60 md:text-3xl text-black-dark leading-tight">\n           <span data-translate="error">Error</span>\n           <span>1015</span>\n         </h1>\n         <span class="inline-block md:block heading-ray-id font-mono text-15 lg:text-sm lg:leading-relaxed">Ray ID: 6fe62dfef8545773 &bull;</span>\n         <span class="inline-block md:block heading-ray-id font-mono text-15 lg:text-sm lg:leading-relaxed">2022-04-19 14:02:44 UTC</span>\n        <h2 class="text-gray-600 leading-1.3 text-3xl lg:text-2xl font-light">You are being rate limited</h2>\n      </header>\n\n      <section class="w-240 lg:w-full mx-auto mb-8 lg:px-8">\n          <div id="what-happened-section" class="w-1/2 md:w-full">\n            <h2 class="text-3xl leading-tight font-normal mb-4 text-black-dark antialiased" data-translate="what_happened">What happened?</h2>\n            <p>The owner of this website (api.coingecko.com) has banned you temporarily from accessing this website.</p>\n            \n          </div>\n\n          \n      </section>\n\n      <div class="feedback-hidden py-8 text-center" id="error-feedback">\n    <div id="error-feedback-survey" class="footer-line-wrapper">\n        Was this page helpful?\n        <button class="border border-solid bg-white cf-button cursor-pointer ml-4 px-4 py-2 rounded" id="feedback-button-yes" type="button">Yes</button>\n        <button class="border border-solid bg-white cf-button cursor-pointer ml-4 px-4 py-2 rounded" id="feedback-button-no" type="button">No</button>\n    </div>\n    <div class="feedback-success feedback-hidden" id="error-feedback-success">\n        Thank you for your feedback!\n    </div>\n</div>\n\n\n      <div class="cf-error-footer cf-wrapper w-240 lg:w-full py-10 sm:py-4 sm:px-8 mx-auto text-center sm:text-left border-solid border-0 border-t border-gray-300">\n  <p class="text-13">\n    <span class="cf-footer-item sm:block sm:mb-1">Cloudflare Ray ID: <strong class="font-semibold">6fe62dfef8545773</strong></span>\n    <span class="cf-footer-separator sm:hidden">&bull;</span>\n    <span class="cf-footer-item sm:block sm:mb-1"><span>Your IP</span>: 13.58.215.91</span>\n    <span class="cf-footer-separator sm:hidden">&bull;</span>\n    <span class="cf-footer-item sm:block sm:mb-1"><span>Performance &amp; security by</span> <a rel="noopener noreferrer" href="https://www.cloudflare.com/5xx-error-landing" id="brand_link" target="_blank">Cloudflare</a></span>\n    \n  </p>\n</div><!-- /.error-footer -->\n\n\n    </div><!-- /#cf-error-details -->\n  </div><!-- /#cf-wrapper -->\n\n  <script type="text/javascript">\n  window._cf_translation = {};\n  \n  \n</script>\n\n</body>\n</html>\n',  # noqa: E501
                 0,
             ),
         }
 
-    coingecko.WebPriceService.get_url = mock_get_url
-    ps = CoinGeckoSpotPriceService(timeout=0.5)
-    v, dt = await ps.get_price("trb", "usd")
+    with mock.patch("telliot_feeds.sources.price.spot.coingecko.WebPriceService.get_url", side_effect=mock_get_url):
+        ps = CoinGeckoSpotPriceService(timeout=0.5)
+        v, dt = await ps.get_price("trb", "usd")
 
-    assert v is None
-    assert dt is None
-    assert "CoinGecko API rate limit exceeded" in caplog.text
+        assert v is None
+        assert dt is None
+        assert "CoinGecko API rate limit exceeded" in caplog.text
 
 
 @pytest.mark.asyncio
 async def test_failed_price_service_request():
     """Assert web price service catches failed requests"""
 
     invalid_token_ticker = "abcxyz"
 
     v, t = await get_price(invalid_token_ticker, "usd", service["gemini"])
 
     assert v is None
     assert t is None
+
+
+@pytest.mark.asyncio
+async def test_coinpaprika():
+    """Test Coinpaprika price service"""
+    v, t = await get_price("steth-lido-staked-ether", "btc", service["coinpaprika"])
+    validate_price(v, t)
+    assert v is not None
+    assert t is not None
+
+
+@pytest.mark.asyncio
+async def test_curvefi():
+    """Test CurveFinance price service"""
+    v, t = await get_price("steth", "btc", service["curvefi"])
+    validate_price(v, t)
+    assert v is not None
+    assert t is not None
```

### Comparing `telliot_feeds-0.1.8/tests/sources/test_tami_calcuation.py` & `telliot_feeds-0.1.9/tests/sources/test_tami_calcuation.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/sources/test_tellor_rng_source.py` & `telliot_feeds-0.1.9/tests/sources/test_tellor_rng_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_autopay.py` & `telliot_feeds-0.1.9/tests/test_autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_bct_usd.py` & `telliot_feeds-0.1.9/tests/test_bct_usd.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_dai_usd.py` & `telliot_feeds-0.1.9/tests/test_dai_usd.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_data_source.py` & `telliot_feeds-0.1.9/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_examples.py` & `telliot_feeds-0.1.9/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_numeric_api_response_feed.py` & `telliot_feeds-0.1.9/tests/test_numeric_api_response_feed.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_olympus.py` & `telliot_feeds-0.1.9/tests/test_olympus.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_price_service.py` & `telliot_feeds-0.1.9/tests/test_price_service.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_value_type.py` & `telliot_feeds-0.1.9/tests/test_value_type.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/test_vesq.py` & `telliot_feeds-0.1.9/tests/test_vesq.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/tips/conftest.py` & `telliot_feeds-0.1.9/tests/tips/conftest.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/tips/test_feed_suggestion.py` & `telliot_feeds-0.1.9/tests/tips/test_feed_suggestion.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/tips/test_multicall_autopay.py` & `telliot_feeds-0.1.9/tests/tips/test_multicall_autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/tips/test_multicall_support.py` & `telliot_feeds-0.1.9/tests/tips/test_multicall_support.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/tips/test_one_time_tips.py` & `telliot_feeds-0.1.9/tests/tips/test_one_time_tips.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/tips/test_selected_queryid.py` & `telliot_feeds-0.1.9/tests/tips/test_selected_queryid.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/tips/test_tips_available_after_submission.py` & `telliot_feeds-0.1.9/tests/tips/test_tips_available_after_submission.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/utils/test_config_utils.py` & `telliot_feeds-0.1.9/tests/utils/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/utils/test_decode.py` & `telliot_feeds-0.1.9/tests/utils/test_decode.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/utils/test_input_timeout.py` & `telliot_feeds-0.1.9/tests/utils/test_input_timeout.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tests/utils/test_reporter_utils.py` & `telliot_feeds-0.1.9/tests/utils/test_reporter_utils.py`

 * *Files identical despite different names*

### Comparing `telliot_feeds-0.1.8/tox.ini` & `telliot_feeds-0.1.9/tox.ini`

 * *Files identical despite different names*

