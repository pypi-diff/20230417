# Comparing `tmp/unicorn-binance-websocket-api-1.46.0.tar.gz` & `tmp/unicorn-binance-websocket-api-1.46.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicorn-binance-websocket-api-1.46.0.tar", last modified: Wed Apr 12 21:37:44 2023, max compression
+gzip compressed data, was "unicorn-binance-websocket-api-1.46.1.tar", last modified: Mon Apr 17 10:29:37 2023, max compression
```

## Comparing `unicorn-binance-websocket-api-1.46.0.tar` & `unicorn-binance-websocket-api-1.46.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 21:37:44.612731 unicorn-binance-websocket-api-1.46.0/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1215 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.0/LICENSE
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    43944 2023-04-12 21:37:44.607577 unicorn-binance-websocket-api-1.46.0/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    42105 2023-04-12 19:43:57.000000 unicorn-binance-websocket-api-1.46.0/README.md
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-12 21:37:44.613907 unicorn-binance-websocket-api-1.46.0/setup.cfg
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4920 2023-04-12 19:43:57.000000 unicorn-binance-websocket-api-1.46.0/setup.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 21:37:44.423591 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      498 2023-04-10 02:58:46.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/__init__.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    86185 2023-04-12 21:14:34.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/api.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    26452 2023-04-06 12:13:20.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2744 2023-04-12 11:58:02.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection_settings.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2168 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/exceptions.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)   209597 2023-04-12 21:37:26.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/manager.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    17375 2023-04-12 13:37:19.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restclient.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3673 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restserver.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    18629 2023-04-12 12:04:53.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/sockets.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 21:37:44.575566 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    43944 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      680 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      162 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/requires.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       30 2023-04-12 21:37:43.000000 unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/top_level.txt
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-17 10:29:37.653548 unicorn-binance-websocket-api-1.46.1/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1215 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.1/LICENSE
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    44078 2023-04-17 10:29:37.637915 unicorn-binance-websocket-api-1.46.1/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    42241 2023-04-17 09:46:36.000000 unicorn-binance-websocket-api-1.46.1/README.md
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-17 10:29:37.653548 unicorn-binance-websocket-api-1.46.1/setup.cfg
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4920 2023-04-12 19:43:57.000000 unicorn-binance-websocket-api-1.46.1/setup.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-17 10:29:37.445396 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      498 2023-04-10 02:58:46.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/__init__.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    86183 2023-04-13 07:27:52.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/api.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    26452 2023-04-06 12:13:20.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/connection.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2744 2023-04-12 11:58:02.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/connection_settings.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     2168 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/exceptions.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)   209596 2023-04-17 10:29:04.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/manager.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    18959 2023-04-17 10:19:35.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/restclient.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3673 2023-04-03 15:49:16.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/restserver.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    18629 2023-04-12 12:04:53.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/sockets.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-17 10:29:37.606312 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    44078 2023-04-17 10:29:35.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      680 2023-04-17 10:29:36.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-17 10:29:35.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      162 2023-04-17 10:29:36.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/requires.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       30 2023-04-17 10:29:36.000000 unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/top_level.txt
```

### Comparing `unicorn-binance-websocket-api-1.46.0/LICENSE` & `unicorn-binance-websocket-api-1.46.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.46.0/PKG-INFO` & `unicorn-binance-websocket-api-1.46.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-websocket-api
-Version: 1.46.0
+Version: 1.46.1
 Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-websocket-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-websocket-api.docs.lucit.tech
@@ -33,30 +33,31 @@
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Get professional and fast support](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-suite/master/images/support/LUCIT-get-professional-and-fast-support.png)](https://www.lucit.tech/get-support.html)
 
+[![Github](https://img.shields.io/badge/source-github-cbc2c8)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 [![GitHub Release](https://img.shields.io/github/release/LUCIT-Systems-and-Development/unicorn-binance-websocket-api.svg?label=github)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases)
 [![GitHub Downloads](https://img.shields.io/github/downloads/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/total?color=blue)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases)
 [![Conda Release](https://img.shields.io/conda/vn/conda-forge/unicorn-binance-websocket-api.svg?color=blue)](https://anaconda.org/conda-forge/unicorn-binance-websocket-api)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/unicorn-binance-websocket-api.svg?color=blue)](https://anaconda.org/conda-forge/unicorn-binance-websocket-api)
 [![PyPi Release](https://img.shields.io/pypi/v/unicorn-binance-websocket-api?color=blue)](https://pypi.org/project/unicorn-binance-websocket-api/)
 [![PyPi Downloads](https://pepy.tech/badge/unicorn-binance-websocket-api)](https://pepy.tech/project/unicorn-binance-websocket-api)
 [![License](https://img.shields.io/github/license/LUCIT-Systems-and-Development/unicorn-binance-websocket-api.svg?color=blue)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/LICENSE)
 [![Supported Python Version](https://img.shields.io/pypi/pyversions/unicorn_binance_websocket_api.svg)](https://www.python.org/downloads/)
 [![PyPI - Status](https://img.shields.io/pypi/status/unicorn_binance_websocket_api.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/issues)
 [![CodeQL](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/codeql-analysis.yml)
 [![Unit Tests](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml)
 [![Azure Pipelines](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/unicorn-binance-websocket-api-feedstock?branchName=main)](https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=15698&branchName=main)
 [![codecov](https://codecov.io/gh/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/branch/master/graph/badge.svg?token=5I03AZ3F5S)](https://codecov.io/gh/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
-[![Read the Docs](https://img.shields.io/badge/read-%20docs-yellow)](https://unicorn-binance-websocket-api.docs.lucit.tech/)
-[![Github](https://img.shields.io/badge/source-github-yellow)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
-[![Telegram](https://img.shields.io/badge/chat-telegram-yellow)](https://t.me/unicorndevs)
+[![Read the Docs](https://img.shields.io/badge/read-%20docs-yellow)](https://unicorn-binance-websocket-api.docs.lucit.tech)
+[![Read How To`s](https://img.shields.io/badge/read-%20howto-yellow)](https://medium.lucit.tech)
+[![Telegram](https://img.shields.io/badge/chat-telegram-41ab8c)](https://t.me/unicorndevs)
 [![Gitter](https://badges.gitter.im/unicorn-binance-suite/unicorn-binance-websocket-api.svg)](https://gitter.im/unicorn-binance-suite/unicorn-binance-websocket-api?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [![LUCIT-UBWA-Banner](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/master/images/logo/LUCIT-UBWA-Banner-Readme.png)](https://www.lucit.tech/unicorn-binance-websocket-api.html)
 
 # UNICORN Binance WebSocket API
 
 [Description](#description) | [Live Demo](#live-demo) | [Installation](#installation-and-upgrade) | [How To](#howto) |
@@ -182,18 +183,19 @@
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
 [Binance US](https://github.com/binance-us/binance-official-api-docs), 
 [Binance TR](https://www.trbinance.com/apidocs), 
 [Binance DEX](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and 
 [Binance DEX Testnet](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and supports sending requests 
 to the [Binance Websocket API](https://developers.binance.com/docs/binance-trading-api/websocket_api) and the streaming 
 of all public streams like trade, kline, ticker, depth, bookTicker, forceOrder, compositeIndex, blockheight etc. and 
-also all private userData streams which needs to be used with a valid api_key and api_secret from the Binance Exchange 
-[www.binance.com](https://www.binance.com/userCenter/createApi.html), 
+also all private userData streams which needs to be used with a valid 
+[api_key and api_secret](https://medium.lucit.tech/how-to-create-a-binance-api-key-and-api-secret-3bb5f47e360d)
+from the Binance Exchange [www.binance.com](https://www.binance.com/), 
 [testnet.binance.vision](https://testnet.binance.vision/) or 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) - for the DEX you need a user address from 
+[www.binance.us](https://www.binance.us) - for the DEX you need a user address from 
 [www.binance.org](https://www.binance.org/en/create) or [testnet.binance.org](https://testnet.binance.org/en/create) 
 and you can [get funds](https://www.binance.vision/tutorials/binance-dex-funding-your-testnet-account) for the testnet.
 
 Use the [UNICORN Binance REST API](https://www.lucit.tech/unicorn-binance-rest-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance WebSocket API?
 - Fully managed websockets and 100% auto-reconnect! Also handles maintenance windows!
```

### Comparing `unicorn-binance-websocket-api-1.46.0/README.md` & `unicorn-binance-websocket-api-1.46.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [![Get professional and fast support](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-suite/master/images/support/LUCIT-get-professional-and-fast-support.png)](https://www.lucit.tech/get-support.html)
 
+[![Github](https://img.shields.io/badge/source-github-cbc2c8)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 [![GitHub Release](https://img.shields.io/github/release/LUCIT-Systems-and-Development/unicorn-binance-websocket-api.svg?label=github)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases)
 [![GitHub Downloads](https://img.shields.io/github/downloads/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/total?color=blue)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases)
 [![Conda Release](https://img.shields.io/conda/vn/conda-forge/unicorn-binance-websocket-api.svg?color=blue)](https://anaconda.org/conda-forge/unicorn-binance-websocket-api)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/unicorn-binance-websocket-api.svg?color=blue)](https://anaconda.org/conda-forge/unicorn-binance-websocket-api)
 [![PyPi Release](https://img.shields.io/pypi/v/unicorn-binance-websocket-api?color=blue)](https://pypi.org/project/unicorn-binance-websocket-api/)
 [![PyPi Downloads](https://pepy.tech/badge/unicorn-binance-websocket-api)](https://pepy.tech/project/unicorn-binance-websocket-api)
 [![License](https://img.shields.io/github/license/LUCIT-Systems-and-Development/unicorn-binance-websocket-api.svg?color=blue)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/LICENSE)
 [![Supported Python Version](https://img.shields.io/pypi/pyversions/unicorn_binance_websocket_api.svg)](https://www.python.org/downloads/)
 [![PyPI - Status](https://img.shields.io/pypi/status/unicorn_binance_websocket_api.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/issues)
 [![CodeQL](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/codeql-analysis.yml)
 [![Unit Tests](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml)
 [![Azure Pipelines](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/unicorn-binance-websocket-api-feedstock?branchName=main)](https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=15698&branchName=main)
 [![codecov](https://codecov.io/gh/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/branch/master/graph/badge.svg?token=5I03AZ3F5S)](https://codecov.io/gh/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
-[![Read the Docs](https://img.shields.io/badge/read-%20docs-yellow)](https://unicorn-binance-websocket-api.docs.lucit.tech/)
-[![Github](https://img.shields.io/badge/source-github-yellow)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
-[![Telegram](https://img.shields.io/badge/chat-telegram-yellow)](https://t.me/unicorndevs)
+[![Read the Docs](https://img.shields.io/badge/read-%20docs-yellow)](https://unicorn-binance-websocket-api.docs.lucit.tech)
+[![Read How To`s](https://img.shields.io/badge/read-%20howto-yellow)](https://medium.lucit.tech)
+[![Telegram](https://img.shields.io/badge/chat-telegram-41ab8c)](https://t.me/unicorndevs)
 [![Gitter](https://badges.gitter.im/unicorn-binance-suite/unicorn-binance-websocket-api.svg)](https://gitter.im/unicorn-binance-suite/unicorn-binance-websocket-api?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [![LUCIT-UBWA-Banner](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/master/images/logo/LUCIT-UBWA-Banner-Readme.png)](https://www.lucit.tech/unicorn-binance-websocket-api.html)
 
 # UNICORN Binance WebSocket API
 
 [Description](#description) | [Live Demo](#live-demo) | [Installation](#installation-and-upgrade) | [How To](#howto) |
@@ -145,18 +146,19 @@
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
 [Binance US](https://github.com/binance-us/binance-official-api-docs), 
 [Binance TR](https://www.trbinance.com/apidocs), 
 [Binance DEX](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and 
 [Binance DEX Testnet](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and supports sending requests 
 to the [Binance Websocket API](https://developers.binance.com/docs/binance-trading-api/websocket_api) and the streaming 
 of all public streams like trade, kline, ticker, depth, bookTicker, forceOrder, compositeIndex, blockheight etc. and 
-also all private userData streams which needs to be used with a valid api_key and api_secret from the Binance Exchange 
-[www.binance.com](https://www.binance.com/userCenter/createApi.html), 
+also all private userData streams which needs to be used with a valid 
+[api_key and api_secret](https://medium.lucit.tech/how-to-create-a-binance-api-key-and-api-secret-3bb5f47e360d)
+from the Binance Exchange [www.binance.com](https://www.binance.com/), 
 [testnet.binance.vision](https://testnet.binance.vision/) or 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) - for the DEX you need a user address from 
+[www.binance.us](https://www.binance.us) - for the DEX you need a user address from 
 [www.binance.org](https://www.binance.org/en/create) or [testnet.binance.org](https://testnet.binance.org/en/create) 
 and you can [get funds](https://www.binance.vision/tutorials/binance-dex-funding-your-testnet-account) for the testnet.
 
 Use the [UNICORN Binance REST API](https://www.lucit.tech/unicorn-binance-rest-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance WebSocket API?
 - Fully managed websockets and 100% auto-reconnect! Also handles maintenance windows!
```

### Comparing `unicorn-binance-websocket-api-1.46.0/setup.py` & `unicorn-binance-websocket-api-1.46.1/setup.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/api.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1230,15 +1230,15 @@
         which symbol the orders belong to.
 
         Official documentation:
 
             - https://developers.binance.com/docs/binance-trading-api/websocket_api#current-open-orders-user_data
 
         If you need to continuously monitor order status updates, please consider using
-        'WebSocket Streams <https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.create_stream>'_:
+        'WebSocket Streams <https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.create_stream>`_
 
           - `userData`
 
           - `executionReport` user data stream event
 
         :param process_response: Provide a function/method to process the received webstream data (callback)
                                  of this specific request.
@@ -1523,15 +1523,15 @@
                        symbol: str = None) -> bool:
         """
         Get current order book.
 
         Note that this request returns limited market depth.
 
         If you need to continuously monitor order book updates, please consider using
-        'WebSocket Streams <https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.create_stream>'_:
+        'WebSocket Streams <https://unicorn-binance-websocket-api.docs.lucit.tech/unicorn_binance_websocket_api.html#unicorn_binance_websocket_api.manager.BinanceWebSocketApiManager.create_stream>'_
 
           - <symbol>@depth<levels>
 
           - <symbol>@depth
 
         Official documentation:
```

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/connection.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/connection_settings.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/connection_settings.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/exceptions.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/manager.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
                                 <https://websockets.readthedocs.io/en/stable/topics/timeouts.html?highlight=ping_interval#keepalive-in-websock ets>`_
     :type ping_interval_default: int
     :param ping_timeout_default: If the corresponding `Pong frame` isn't received within
                                `ping_timeout` seconds, the connection is considered unusable and is closed with
                                code 1011. This ensures that the remote endpoint remains responsive. Set
                                `ping_timeout` to `None` to disable this behavior.
                                This parameter is passed through to the `websockets.client.connect()
-                               <https://websockets.readthedocs.io/en/stable/topics/timeouts.html?highlight=ping_interval#keepalive-in-websockets>`_
+                               <https://websockets.readthedocs.io/en/stable/topics/timeouts.html?highlight=ping_timeout#keepalive-in-websockets>`_
     :type ping_timeout_default: int
     :param high_performance: Set to True makes `create_stream()` a non-blocking function
     :type high_performance:  bool
     :param debug: If True the lib adds additional information to logging outputs
     :type debug:  bool
     :param restful_base_uri: Override `restful_base_uri`. Example: `https://127.0.0.1`
     :type restful_base_uri:  str
@@ -226,15 +226,15 @@
                  exchange_type: Optional[Literal['cex', 'dex']] = None,
                  socks5_proxy_server: Optional[str] = None,
                  socks5_proxy_user: Optional[str] = None,
                  socks5_proxy_pass: Optional[str] = None,
                  socks5_proxy_ssl_verification: Optional[bool] = True,):
         threading.Thread.__init__(self)
         self.name = "unicorn-binance-websocket-api"
-        self.version = "1.46.0"
+        self.version = "1.46.1"
         logger.info(f"New instance of {self.get_user_agent()} on "
                     f"{str(platform.system())} {str(platform.release())} for exchange {exchange} started ...")
         self.debug = debug
         logger.info(f"Debug is {self.debug}")
         if disable_colorama is not True:
             logger.info(f"Initiating `colorama_{colorama.__version__}`")
             colorama.init()
```

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restclient.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/restclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
 from unicorn_binance_rest_api import BinanceRestApiManager
 import logging
 import threading
 import time
+from typing import Optional, Union
 
 logger = logging.getLogger("unicorn_binance_websocket_api")
 
 
 class BinanceWebSocketApiRestclient(object):
     def __init__(self, manager):
         """
@@ -50,26 +51,26 @@
         :type manager: object
         """
         self.manager = manager
         self.api_key = False
         self.api_secret = False
         self.symbol = False
         self.listen_key = False
-        self.last_static_ping_listen_key = False
+        self.last_static_ping_listen_key: Optional[Union[bool, int]] = False
         self.listen_key_output = False
         self.threading_lock = threading.Lock()
         self.restful_base_uri = self.manager.restful_base_uri
 
     def _init_vars(self,
                    stream_id,
                    api_key=False,
                    api_secret=False,
                    symbol=False,
                    listen_key=False,
-                   last_static_ping_listen_key=False):
+                   last_static_ping_listen_key: Optional[Union[bool, int]] = False):
         """
         set default values and load values from stream_list
 
         :param stream_id: provide a stream_id (only needed for userData Streams (acquiring a listenKey)
         :type stream_id: str
         :param api_key: provide a valid Binance API key
         :type api_key: str
@@ -141,15 +142,25 @@
                             last_static_ping_listen_key=last_static_ping_listen_key)
             ubra = BinanceRestApiManager(api_key=self.api_key, api_secret=self.api_secret,
                                          exchange=self.manager.exchange,
                                          socks5_proxy_server=self.manager.socks5_proxy_server,
                                          socks5_proxy_user=self.manager.socks5_proxy_user,
                                          socks5_proxy_pass=self.manager.socks5_proxy_pass,
                                          warn_on_update=self.manager.warn_on_update)
-            if self.manager.exchange == "binance.com-isolated_margin" or \
+            if self.manager.exchange == "binance.com-margin" or \
+                    self.manager.exchange == "binance.com-margin-testnet":
+                try:
+                    if self.manager.restful_base_uri is not None:
+                        ubra.MARGIN_API_URL = self.manager.restful_base_uri
+                    response = ubra.margin_stream_get_listen_key(output="raw_data", throw_exception=False)
+                except AttributeError as error_msg:
+                    logger.critical(f"BinanceWebSocketApiRestclient.get_listen_key() - error: 8 - "
+                                    f"error_msg: {error_msg} - Can not acquire listen_key for margin!")
+                    return False
+            elif self.manager.exchange == "binance.com-isolated_margin" or \
                     self.manager.exchange == "binance.com-isolated_margin-testnet":
                 if self.symbol is False:
                     logger.critical("BinanceWebSocketApiRestclient.get_listen_key() - error_msg: Parameter "
                                     "`symbol` is missing!")
                     return False
                 else:
                     try:
@@ -229,15 +240,20 @@
             self._init_vars(stream_id, api_key, api_secret, listen_key)
             ubra = BinanceRestApiManager(api_key=self.api_key, api_secret=self.api_secret,
                                          exchange=self.manager.exchange,
                                          socks5_proxy_server=self.manager.socks5_proxy_server,
                                          socks5_proxy_user=self.manager.socks5_proxy_user,
                                          socks5_proxy_pass=self.manager.socks5_proxy_pass,
                                          warn_on_update=self.manager.warn_on_update)
-            if self.manager.exchange == "binance.com-isolated_margin" or \
+            if self.manager.exchange == "binance.com-margin" or \
+                    self.manager.exchange == "binance.com-margin-testnet":
+                if self.manager.restful_base_uri is not None:
+                    ubra.MARGIN_API_URL = self.manager.restful_base_uri
+                result = ubra.margin_stream_close(listenKey=str(self.listen_key), throw_exception=False)
+            elif self.manager.exchange == "binance.com-isolated_margin" or \
                     self.manager.exchange == "binance.com-isolated_margin-testnet":
                 if self.manager.restful_base_uri is not None:
                     ubra.MARGIN_API_URL = self.manager.restful_base_uri
                 result = ubra.isolated_margin_stream_close(symbol=str(self.symbol), listenKey=str(self.listen_key),
                                                            throw_exception=False)
                 self.symbol = False
             elif self.manager.exchange == "binance.com-futures":
@@ -290,15 +306,20 @@
             self._init_vars(stream_id, api_key, api_secret, listen_key, last_static_ping_listen_key)
             ubra = BinanceRestApiManager(api_key=self.api_key, api_secret=self.api_secret,
                                          exchange=self.manager.exchange,
                                          socks5_proxy_server=self.manager.socks5_proxy_server,
                                          socks5_proxy_user=self.manager.socks5_proxy_user,
                                          socks5_proxy_pass=self.manager.socks5_proxy_pass,
                                          warn_on_update=self.manager.warn_on_update)
-            if self.manager.exchange == "binance.com-isolated_margin" or \
+            if self.manager.exchange == "binance.com-margin" or \
+                    self.manager.exchange == "binance.com-margin-testnet":
+                if self.manager.restful_base_uri is not None:
+                    ubra.MARGIN_API_URL = self.manager.restful_base_uri
+                result = ubra.margin_stream_keepalive(listenKey=str(self.listen_key), throw_exception=False)
+            elif self.manager.exchange == "binance.com-isolated_margin" or \
                     self.manager.exchange == "binance.com-isolated_margin-testnet":
                 if self.manager.restful_base_uri is not None:
                     ubra.MARGIN_API_URL = self.manager.restful_base_uri
                 result = ubra.isolated_margin_stream_keepalive(symbol=str(self.symbol), listenKey=str(self.listen_key),
                                                                throw_exception=False)
             elif self.manager.exchange == "binance.com-futures":
                 if self.manager.restful_base_uri is not None:
```

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/restserver.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/restserver.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api/sockets.py` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api/sockets.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/PKG-INFO` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-websocket-api
-Version: 1.46.0
+Version: 1.46.1
 Summary: An unofficial Python API to use the Binance Websocket API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, jersey, us, dex/chain+testnet) in a easy, fast, flexible, robust and fully-featured way.
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-websocket-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-websocket-api.docs.lucit.tech
@@ -33,30 +33,31 @@
 Classifier: Framework :: AsyncIO
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Get professional and fast support](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-suite/master/images/support/LUCIT-get-professional-and-fast-support.png)](https://www.lucit.tech/get-support.html)
 
+[![Github](https://img.shields.io/badge/source-github-cbc2c8)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
 [![GitHub Release](https://img.shields.io/github/release/LUCIT-Systems-and-Development/unicorn-binance-websocket-api.svg?label=github)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases)
 [![GitHub Downloads](https://img.shields.io/github/downloads/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/total?color=blue)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/releases)
 [![Conda Release](https://img.shields.io/conda/vn/conda-forge/unicorn-binance-websocket-api.svg?color=blue)](https://anaconda.org/conda-forge/unicorn-binance-websocket-api)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/unicorn-binance-websocket-api.svg?color=blue)](https://anaconda.org/conda-forge/unicorn-binance-websocket-api)
 [![PyPi Release](https://img.shields.io/pypi/v/unicorn-binance-websocket-api?color=blue)](https://pypi.org/project/unicorn-binance-websocket-api/)
 [![PyPi Downloads](https://pepy.tech/badge/unicorn-binance-websocket-api)](https://pepy.tech/project/unicorn-binance-websocket-api)
 [![License](https://img.shields.io/github/license/LUCIT-Systems-and-Development/unicorn-binance-websocket-api.svg?color=blue)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/LICENSE)
 [![Supported Python Version](https://img.shields.io/pypi/pyversions/unicorn_binance_websocket_api.svg)](https://www.python.org/downloads/)
 [![PyPI - Status](https://img.shields.io/pypi/status/unicorn_binance_websocket_api.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/issues)
 [![CodeQL](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/codeql-analysis.yml)
 [![Unit Tests](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/actions/workflows/unit-tests.yml)
 [![Azure Pipelines](https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/unicorn-binance-websocket-api-feedstock?branchName=main)](https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=15698&branchName=main)
 [![codecov](https://codecov.io/gh/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/branch/master/graph/badge.svg?token=5I03AZ3F5S)](https://codecov.io/gh/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
-[![Read the Docs](https://img.shields.io/badge/read-%20docs-yellow)](https://unicorn-binance-websocket-api.docs.lucit.tech/)
-[![Github](https://img.shields.io/badge/source-github-yellow)](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api)
-[![Telegram](https://img.shields.io/badge/chat-telegram-yellow)](https://t.me/unicorndevs)
+[![Read the Docs](https://img.shields.io/badge/read-%20docs-yellow)](https://unicorn-binance-websocket-api.docs.lucit.tech)
+[![Read How To`s](https://img.shields.io/badge/read-%20howto-yellow)](https://medium.lucit.tech)
+[![Telegram](https://img.shields.io/badge/chat-telegram-41ab8c)](https://t.me/unicorndevs)
 [![Gitter](https://badges.gitter.im/unicorn-binance-suite/unicorn-binance-websocket-api.svg)](https://gitter.im/unicorn-binance-suite/unicorn-binance-websocket-api?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 [![LUCIT-UBWA-Banner](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/master/images/logo/LUCIT-UBWA-Banner-Readme.png)](https://www.lucit.tech/unicorn-binance-websocket-api.html)
 
 # UNICORN Binance WebSocket API
 
 [Description](#description) | [Live Demo](#live-demo) | [Installation](#installation-and-upgrade) | [How To](#howto) |
@@ -182,18 +183,19 @@
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
 [Binance US](https://github.com/binance-us/binance-official-api-docs), 
 [Binance TR](https://www.trbinance.com/apidocs), 
 [Binance DEX](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and 
 [Binance DEX Testnet](https://docs.binance.org/api-reference/dex-api/ws-connection.html) and supports sending requests 
 to the [Binance Websocket API](https://developers.binance.com/docs/binance-trading-api/websocket_api) and the streaming 
 of all public streams like trade, kline, ticker, depth, bookTicker, forceOrder, compositeIndex, blockheight etc. and 
-also all private userData streams which needs to be used with a valid api_key and api_secret from the Binance Exchange 
-[www.binance.com](https://www.binance.com/userCenter/createApi.html), 
+also all private userData streams which needs to be used with a valid 
+[api_key and api_secret](https://medium.lucit.tech/how-to-create-a-binance-api-key-and-api-secret-3bb5f47e360d)
+from the Binance Exchange [www.binance.com](https://www.binance.com/), 
 [testnet.binance.vision](https://testnet.binance.vision/) or 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) - for the DEX you need a user address from 
+[www.binance.us](https://www.binance.us) - for the DEX you need a user address from 
 [www.binance.org](https://www.binance.org/en/create) or [testnet.binance.org](https://testnet.binance.org/en/create) 
 and you can [get funds](https://www.binance.vision/tutorials/binance-dex-funding-your-testnet-account) for the testnet.
 
 Use the [UNICORN Binance REST API](https://www.lucit.tech/unicorn-binance-rest-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance WebSocket API?
 - Fully managed websockets and 100% auto-reconnect! Also handles maintenance windows!
```

### Comparing `unicorn-binance-websocket-api-1.46.0/unicorn_binance_websocket_api.egg-info/SOURCES.txt` & `unicorn-binance-websocket-api-1.46.1/unicorn_binance_websocket_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

