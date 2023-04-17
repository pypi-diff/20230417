# Comparing `tmp/novalabs-backtest-1.1.8.tar.gz` & `tmp/novalabs-backtest-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novalabs-backtest-1.1.8.tar", last modified: Fri Mar 31 16:07:05 2023, max compression
+gzip compressed data, was "novalabs-backtest-1.1.9.tar", last modified: Mon Apr  3 12:56:48 2023, max compression
```

## Comparing `novalabs-backtest-1.1.8.tar` & `novalabs-backtest-1.1.9.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.467182 novalabs-backtest-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.459182 novalabs-backtest-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.463182 novalabs-backtest-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/.pypirc
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-31 16:07:05.467182 novalabs-backtest-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.463182 novalabs-backtest-1.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.463182 novalabs-backtest-1.1.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.463182 novalabs-backtest-1.1.8/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   130148 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/docs/source/images/profits.png
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.463182 novalabs-backtest-1.1.8/novalabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.463182 novalabs-backtest-1.1.8/novalabs/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/binance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/btcex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/mexc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21128 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/oanda.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/clients/okx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.463182 novalabs-backtest-1.1.8/novalabs/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/data/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/data/orderbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/data/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/data/telegram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.467182 novalabs-backtest-1.1.8/novalabs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57864 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/utils/backtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/utils/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23277 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/novalabs/utils/indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.467182 novalabs-backtest-1.1.8/novalabs_backtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-31 16:07:04.000000 novalabs-backtest-1.1.8/novalabs_backtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-31 16:07:05.000000 novalabs-backtest-1.1.8/novalabs_backtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 16:07:04.000000 novalabs-backtest-1.1.8/novalabs_backtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 16:07:04.000000 novalabs-backtest-1.1.8/novalabs_backtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 16:07:04.000000 novalabs-backtest-1.1.8/novalabs_backtest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 16:07:05.467182 novalabs-backtest-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.459182 novalabs-backtest-1.1.8/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.467182 novalabs-backtest-1.1.8/test/backtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/backtest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 16:07:05.467182 novalabs-backtest-1.1.8/test/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/clients/test_format_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/clients/test_get_earliest_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/clients/test_get_historical_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/clients/test_get_pairs_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/clients/test_get_server_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-31 16:06:51.000000 novalabs-backtest-1.1.8/test/clients/test_update_historical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.449262 novalabs-backtest-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.441262 novalabs-backtest-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/.pypirc
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-03 12:56:48.449262 novalabs-backtest-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   130148 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/docs/source/images/profits.png
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/novalabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/novalabs/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/btcex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/mexc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21128 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/oanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/clients/okx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/novalabs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/data/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/data/orderbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/data/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/data/telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/novalabs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57864 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/utils/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/utils/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28283 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/novalabs/utils/indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/novalabs_backtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-03 12:56:48.000000 novalabs-backtest-1.1.9/novalabs_backtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-03 12:56:48.000000 novalabs-backtest-1.1.9/novalabs_backtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 12:56:48.000000 novalabs-backtest-1.1.9/novalabs_backtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-03 12:56:48.000000 novalabs-backtest-1.1.9/novalabs_backtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 12:56:48.000000 novalabs-backtest-1.1.9/novalabs_backtest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 12:56:48.449262 novalabs-backtest-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.441262 novalabs-backtest-1.1.9/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.445262 novalabs-backtest-1.1.9/test/backtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/backtest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.449262 novalabs-backtest-1.1.9/test/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/clients/test_format_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/clients/test_get_earliest_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/clients/test_get_historical_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/clients/test_get_pairs_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/clients/test_get_server_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/clients/test_update_historical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:48.449262 novalabs-backtest-1.1.9/test/indicators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-03 12:56:36.000000 novalabs-backtest-1.1.9/test/indicators/test_indicators.py
```

### Comparing `novalabs-backtest-1.1.8/.github/workflows/publish-to-pypi.yml` & `novalabs-backtest-1.1.9/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/LICENSE` & `novalabs-backtest-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/PKG-INFO` & `novalabs-backtest-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: novalabs-backtest
-Version: 1.1.8
+Version: 1.1.9
 Summary: Wrappers around Nova Labs utilities focused on safety and testability
 Home-page: https://github.com/Nova-DevTeam/nova-backtest
 Author: Nova Labs
 Author-email: devteam@novalabs.ai
 License: UNKNOWN
 Description: # nova-backtest
```

### Comparing `novalabs-backtest-1.1.8/docs/Makefile` & `novalabs-backtest-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/docs/make.bat` & `novalabs-backtest-1.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/docs/source/conf.py` & `novalabs-backtest-1.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/docs/source/images/profits.png` & `novalabs-backtest-1.1.9/docs/source/images/profits.png`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/docs/source/index.rst` & `novalabs-backtest-1.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/docs/source/usage.rst` & `novalabs-backtest-1.1.9/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/binance.py` & `novalabs-backtest-1.1.9/novalabs/clients/binance.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/btcex.py` & `novalabs-backtest-1.1.9/novalabs/clients/btcex.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/bybit.py` & `novalabs-backtest-1.1.9/novalabs/clients/bybit.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/client_interface.py` & `novalabs-backtest-1.1.9/novalabs/clients/client_interface.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/clients.py` & `novalabs-backtest-1.1.9/novalabs/clients/clients.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/huobi.py` & `novalabs-backtest-1.1.9/novalabs/clients/huobi.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/kucoin.py` & `novalabs-backtest-1.1.9/novalabs/clients/kucoin.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/mexc.py` & `novalabs-backtest-1.1.9/novalabs/clients/mexc.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/oanda.py` & `novalabs-backtest-1.1.9/novalabs/clients/oanda.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/clients/okx.py` & `novalabs-backtest-1.1.9/novalabs/clients/okx.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/data/discord.py` & `novalabs-backtest-1.1.9/novalabs/data/discord.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/data/orderbook.py` & `novalabs-backtest-1.1.9/novalabs/data/orderbook.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/data/reddit.py` & `novalabs-backtest-1.1.9/novalabs/data/reddit.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/data/telegram.py` & `novalabs-backtest-1.1.9/novalabs/data/telegram.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/utils/backtest.py` & `novalabs-backtest-1.1.9/novalabs/utils/backtest.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/utils/constant.py` & `novalabs-backtest-1.1.9/novalabs/utils/constant.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs/utils/helpers.py` & `novalabs-backtest-1.1.9/novalabs/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/novalabs_backtest.egg-info/PKG-INFO` & `novalabs-backtest-1.1.9/novalabs_backtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: novalabs-backtest
-Version: 1.1.8
+Version: 1.1.9
 Summary: Wrappers around Nova Labs utilities focused on safety and testability
 Home-page: https://github.com/Nova-DevTeam/nova-backtest
 Author: Nova Labs
 Author-email: devteam@novalabs.ai
 License: UNKNOWN
 Description: # nova-backtest
```

### Comparing `novalabs-backtest-1.1.8/novalabs_backtest.egg-info/SOURCES.txt` & `novalabs-backtest-1.1.9/novalabs_backtest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -43,8 +43,10 @@
 test/backtest/__init__.py
 test/clients/__init__.py
 test/clients/test_format_data.py
 test/clients/test_get_earliest_timestamp.py
 test/clients/test_get_historical_data.py
 test/clients/test_get_pairs_info.py
 test/clients/test_get_server_time.py
-test/clients/test_update_historical.py
+test/clients/test_update_historical.py
+test/indicators/__init__.py
+test/indicators/test_indicators.py
```

### Comparing `novalabs-backtest-1.1.8/setup.py` & `novalabs-backtest-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/test/clients/test_format_data.py` & `novalabs-backtest-1.1.9/test/clients/test_format_data.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/test/clients/test_get_earliest_timestamp.py` & `novalabs-backtest-1.1.9/test/clients/test_get_earliest_timestamp.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/test/clients/test_get_historical_data.py` & `novalabs-backtest-1.1.9/test/clients/test_get_historical_data.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/test/clients/test_get_pairs_info.py` & `novalabs-backtest-1.1.9/test/clients/test_get_pairs_info.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/test/clients/test_get_server_time.py` & `novalabs-backtest-1.1.9/test/clients/test_get_server_time.py`

 * *Files identical despite different names*

### Comparing `novalabs-backtest-1.1.8/test/clients/test_update_historical.py` & `novalabs-backtest-1.1.9/test/clients/test_update_historical.py`

 * *Files identical despite different names*

