# Comparing `tmp/OctoBot-Trading-2.3.4.tar.gz` & `tmp/OctoBot-Trading-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Trading-2.3.4.tar", last modified: Mon Jan  2 15:55:55 2023, max compression
+gzip compressed data, was "OctoBot-Trading-2.3.7.tar", last modified: Thu Jan 12 01:40:01 2023, max compression
```

## Comparing `OctoBot-Trading-2.3.4.tar` & `OctoBot-Trading-2.3.7.tar`

### file list

```diff
@@ -1,754 +1,756 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.817222 OctoBot-Trading-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    27457 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.737222 OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-02 15:55:55.000000 OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35576 2023-01-02 15:55:55.000000 OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 15:55:55.000000 OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 15:55:55.000000 OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-01-02 15:55:55.000000 OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-02 15:55:55.000000 OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-02 15:55:55.817222 OctoBot-Trading-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.741222 OctoBot-Trading-2.3.4/octobot_trading/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.741222 OctoBot-Trading-2.3.4/octobot_trading/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/api/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15214 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_channel.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.741222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.741222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/future_contract.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/margin_contract.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/margin_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbol_data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbols_data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.745222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.745222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/funding_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.745222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.745222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/kline_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.745222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_adapter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.749222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13620 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.749222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.749222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/order_book_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.749222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.749222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/price.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/price.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/price_events_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/prices_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.749222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.753222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/recent_trades_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.753222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.753222 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/ticker_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.757222 OctoBot-Trading-2.3.4/octobot_trading/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    26139 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_websocket_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/basic_exchange_wrapper.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/basic_exchange_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.757222 OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/backtesting_exchange_config.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/backtesting_exchange_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/exchange_config_data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/exchange_config_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.757222 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/abstract_websocket_connector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7018 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/abstract_websocket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/ccxt_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    30842 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/ccxt_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/ccxt_websocket_connector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/ccxt_websocket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/cryptofeed_websocket_connector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    40116 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/cryptofeed_websocket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/exchange_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    11200 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_builder.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_channels.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_websocket_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_websocket_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchanges.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.761222 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/ccxt_websocket_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/ccxt_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/cryptofeed_websocket_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/cryptofeed_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/default_spot_ccxt_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/future_ccxt_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/future_ccxt_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/future_exchange_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/future_exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/margin_ccxt_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/margin_ccxt_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/margin_exchange_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/margin_exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/rest_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/spot_ccxt_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    24998 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/spot_ccxt_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/spot_exchange_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/spot_exchange_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.761222 OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    35242 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.761222 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/future_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13120 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/future_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/margin_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/margin_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/spot_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/spot_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/websocket_exchange.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.761222 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/exchange_market_status_fixer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/exchange_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/exchange_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/websockets_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/websockets_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.765222 OctoBot-Trading-2.3.4/octobot_trading/modes/
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15822 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.765222 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_consumer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_producer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    19357 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/mode.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/channel/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/mode_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/modes_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/modes_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/modes_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/modes_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.765222 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.765222 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25436 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/context_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.765222 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/dsl/quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/dsl/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.765222 OctoBot-Trading-2.3.4/octobot_trading/modes/scripted_trading_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/scripted_trading_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/octobot_channel_consumer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.765222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/exchange_personal_data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/exchange_personal_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.769222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.769222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/decimal_order_adapter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/decimal_order_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.769222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    35023 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_adapter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_group.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    19907 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/orders_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/orders_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.773222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/cancel_order_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/close_order_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/fill_order_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/open_order_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/order_state_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/pending_creation_order_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.773222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.773222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/buy_limit_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/limit_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/sell_limit_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.777222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/buy_market_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/market_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/sell_market_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/sell_market_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.777222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/unknown_order.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/unknown_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.777222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/asset.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.777222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/future_asset.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/margin_asset.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/spot_asset.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.781222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.781222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_profitability.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_value_holder.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/sub_portfolio.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/sub_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.781222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/future_portfolio.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/margin_portfolio.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/spot_portfolio.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.781222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.785222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater_simulator.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    38200 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/positions_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.785222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/liquidate_position_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/liquidate_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/open_position_state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/open_position_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/position_state_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/position_state_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.785222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/inverse_position.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/linear_position.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/linear_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/state.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.785222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.793222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trades_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trades_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.793222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transactions_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.793222 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/blockchain_transaction.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/fee_transaction.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/fee_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/transfer_transaction.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/transfer_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.793222 OctoBot-Trading-2.3.4/octobot_trading/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.793222 OctoBot-Trading-2.3.4/octobot_trading/signals/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/channel/remote_trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/channel/signal_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/signal_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/signals/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.793222 OctoBot-Trading-2.3.4/octobot_trading/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/storage/abstract_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/storage/candles_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/storage/portfolio_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/storage/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/storage/trades_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/storage/transactions_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/octobot_trading/supervisors/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/supervisors/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/supervisors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/supervisors/abstract_portfolio_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/supervisors/abstract_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/octobot_trading/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/config_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/config_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/initializable.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/initializable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/initialization_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/simulator_updater_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/exchanges_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/websocket_test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 15:55:55.817222 OctoBot-Trading-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    13352 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.737222 OctoBot-Trading-2.3.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_symbol_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/api/test_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/tests/exchange_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/tests/exchange_data/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/contracts/test_future_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/contracts/test_margin_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.797222 OctoBot-Trading-2.3.4/tests/exchange_data/funding/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/funding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/funding/test_funding_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchange_data/kline/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/kline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/kline/test_kline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchange_data/ohlcv/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/ohlcv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/ohlcv/test_candles_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/ohlcv/test_candles_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchange_data/order_book/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/order_book/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/order_book/test_order_book_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchange_data/prices/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/prices/test_price_events_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/prices/test_prices_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchange_data/recent_trades/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/recent_trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/recent_trades/test_recent_trades_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/test_exchange_symbols_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchange_data/ticker/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchange_data/ticker/test_ticker_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchanges/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/connectors/test_ccxt_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchanges/implementations/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_abstract_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_abstract_websocket_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_basic_exchange_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_config_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/test_exchanges.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchanges/traders/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/traders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50708 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/traders/test_trader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchanges/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/types/test_websocket_exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.801222 OctoBot-Trading-2.3.4/tests/exchanges/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/util/test_exchange_market_status_fixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/exchanges/util/test_exchange_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/modes/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/modes/script_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/script_keywords/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/modes/script_keywords/basic_keywords/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/script_keywords/basic_keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/script_keywords/basic_keywords/test_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/script_keywords/basic_keywords/test_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/modes/script_keywords/dsl/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/script_keywords/dsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/script_keywords/dsl/test_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/test_abstract_mode_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14473 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/modes/test_abstract_trading_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/personal_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/personal_data/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/personal_data/orders/groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_cancel_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_close_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_fill_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_open_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_order_state_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_pending_creation_order_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/test_decimal_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/test_double_filled_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.805222 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_buy_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_sell_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_stop_loss_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_take_profit_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/market/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/market/test_buy_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/market/test_sell_market_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/test_unknown_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/trailing/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/trailing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/test_future_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/test_margin_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/test_spot_asset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    29998 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio_profitability.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio_value_holder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85487 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/test_future_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/test_margin_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/test_spot_portfolio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/positions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/positions/channel/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.809222 OctoBot-Trading-2.3.4/tests/personal_data/positions/states/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/test_position_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/test_positions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.813222 OctoBot-Trading-2.3.4/tests/personal_data/positions/types/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37444 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/types/test_inverse_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    45251 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/positions/types/test_linear_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.813222 OctoBot-Trading-2.3.4/tests/personal_data/trades/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/trades/test_trade_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/trades/test_trade_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.813222 OctoBot-Trading-2.3.4/tests/personal_data/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/transactions/test_transaction_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/personal_data/transactions/test_transactions_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.813222 OctoBot-Trading-2.3.4/tests/signals/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29656 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/signals/test_trading_signal_bundle_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/signals/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.813222 OctoBot-Trading-2.3.4/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/test_utils/order_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/test_utils/random_numbers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.813222 OctoBot-Trading-2.3.4/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests/util/test_config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.813222 OctoBot-Trading-2.3.4/tests_additional/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 15:55:55.817222 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/real_exchange_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_ascendex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_binance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitfinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bithumb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitso.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitstamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bittrex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bybit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_coinbasepro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_coinex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_gateio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_hitbtc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_hollaex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_huobi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_huobipro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_kraken.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_kucoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_ndax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_okcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_okx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_phemex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_poloniex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_upbit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-01-02 15:54:53.000000 OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_wavesexchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.697697 OctoBot-Trading-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.585694 OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-12 01:40:01.000000 OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35441 2023-01-12 01:40:01.000000 OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 01:40:01.000000 OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 01:40:01.000000 OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-12 01:40:01.000000 OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-01-12 01:40:01.000000 OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-01-12 01:40:01.697697 OctoBot-Trading-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.585694 OctoBot-Trading-2.3.7/octobot_trading/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.589694 OctoBot-Trading-2.3.7/octobot_trading/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/api/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_channel.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.589694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.589694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/future_contract.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/margin_contract.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/margin_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbol_data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbols_data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.589694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.593694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/funding_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.593694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.593694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/kline_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.593694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_adapter.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.597694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.597694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.597694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/order_book_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.597694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.601694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/price.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/price_events_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/prices_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.601694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.601694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/recent_trades_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.601694 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.605695 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/ticker_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.609695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_exchange.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_websocket_exchange.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.609695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/adapters/abstract_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/basic_exchange_wrapper.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/basic_exchange_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.609695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/backtesting_exchange_config.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/backtesting_exchange_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/exchange_config_data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/exchange_config_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.609695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.613695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    36623 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.613695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_builder.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_channels.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_websocket_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_websocket_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchanges.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.613695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/default_rest_exchange.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/default_websocket_exchange.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/exchange_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/exchange_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.613695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    37673 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.617695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/rest_exchange.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    34474 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/websocket_exchange.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.617695 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_market_status_fixer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/websockets_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/websockets_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.617695 OctoBot-Trading-2.3.7/octobot_trading/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.621695 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_consumer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_producer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    19750 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/mode.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/channel/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/mode_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/modes_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/modes_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/modes_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/modes_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.621695 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.621695 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25436 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/context_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.621695 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/dsl/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/dsl/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.621695 OctoBot-Trading-2.3.7/octobot_trading/modes/scripted_trading_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/scripted_trading_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15946 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/octobot_channel_consumer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.621695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/exchange_personal_data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/exchange_personal_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.625695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.629695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/decimal_order_adapter.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/decimal_order_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.629695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    35643 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_adapter.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_group.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    20857 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/orders_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/orders_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.629695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/cancel_order_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/close_order_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/fill_order_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/open_order_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/order_state_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/pending_creation_order_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/pending_creation_order_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.633695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.633695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/buy_limit_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/limit_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/sell_limit_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.637695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/buy_market_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/market_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/sell_market_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/sell_market_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.637695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/unknown_order.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/unknown_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.641695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/asset.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.641695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/future_asset.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/margin_asset.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/spot_asset.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.641695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.645695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_profitability.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_value_holder.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_value_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/sub_portfolio.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/sub_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.645695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/future_portfolio.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/margin_portfolio.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/spot_portfolio.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/spot_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.645695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.649695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater_simulator.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    38200 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/positions_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.649695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/liquidate_position_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/liquidate_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/open_position_state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/open_position_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/position_state_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/position_state_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.649695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/inverse_position.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/linear_position.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/linear_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/state.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.653695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.653695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trades_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trades_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.653695 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transactions_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.657696 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/blockchain_transaction.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/blockchain_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/fee_transaction.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/fee_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/transfer_transaction.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/transfer_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.657696 OctoBot-Trading-2.3.7/octobot_trading/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.657696 OctoBot-Trading-2.3.7/octobot_trading/signals/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/channel/remote_trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/channel/signal_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/signal_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/signals/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.661696 OctoBot-Trading-2.3.7/octobot_trading/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/storage/abstract_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/storage/candles_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/storage/portfolio_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/storage/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/storage/trades_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/storage/transactions_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.661696 OctoBot-Trading-2.3.7/octobot_trading/supervisors/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/supervisors/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/supervisors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/supervisors/abstract_portfolio_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/supervisors/abstract_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.661696 OctoBot-Trading-2.3.7/octobot_trading/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/config_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/config_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/initializable.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/initializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/initialization_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/simulator_updater_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.661696 OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/exchanges_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/websocket_test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 01:40:01.697697 OctoBot-Trading-2.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.581694 OctoBot-Trading-2.3.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.665696 OctoBot-Trading-2.3.7/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_symbol_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/api/test_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.665696 OctoBot-Trading-2.3.7/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.665696 OctoBot-Trading-2.3.7/tests/exchange_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.665696 OctoBot-Trading-2.3.7/tests/exchange_data/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/contracts/test_future_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/contracts/test_margin_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.665696 OctoBot-Trading-2.3.7/tests/exchange_data/funding/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/funding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/funding/test_funding_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.665696 OctoBot-Trading-2.3.7/tests/exchange_data/kline/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/kline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/kline/test_kline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.669696 OctoBot-Trading-2.3.7/tests/exchange_data/ohlcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/ohlcv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/ohlcv/test_candles_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/ohlcv/test_candles_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.669696 OctoBot-Trading-2.3.7/tests/exchange_data/order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/order_book/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/order_book/test_order_book_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.669696 OctoBot-Trading-2.3.7/tests/exchange_data/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10397 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/prices/test_price_events_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/prices/test_prices_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.669696 OctoBot-Trading-2.3.7/tests/exchange_data/recent_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/recent_trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/recent_trades/test_recent_trades_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/test_exchange_symbols_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.669696 OctoBot-Trading-2.3.7/tests/exchange_data/ticker/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/ticker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchange_data/ticker/test_ticker_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/exchanges/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/exchanges/connectors/ccxt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/connectors/ccxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/connectors/ccxt/test_ccxt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/exchanges/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/implementations/test_default_rest_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/implementations/test_default_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_abstract_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_abstract_websocket_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_basic_exchange_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/test_exchanges.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/exchanges/traders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/traders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50708 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/traders/test_trader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/exchanges/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/types/test_websocket_exchange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/exchanges/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/util/test_exchange_market_status_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/exchanges/util/test_exchange_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.673696 OctoBot-Trading-2.3.7/tests/modes/script_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/script_keywords/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.677696 OctoBot-Trading-2.3.7/tests/modes/script_keywords/basic_keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/script_keywords/basic_keywords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/script_keywords/basic_keywords/test_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/script_keywords/basic_keywords/test_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.677696 OctoBot-Trading-2.3.7/tests/modes/script_keywords/dsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/script_keywords/dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/script_keywords/dsl/test_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/test_abstract_mode_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/modes/test_abstract_trading_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.677696 OctoBot-Trading-2.3.7/tests/personal_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.677696 OctoBot-Trading-2.3.7/tests/personal_data/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.677696 OctoBot-Trading-2.3.7/tests/personal_data/orders/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.681696 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_cancel_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_close_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_fill_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_open_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_order_state_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_pending_creation_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/test_decimal_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/test_double_filled_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20330 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.681696 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.681696 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_buy_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_sell_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_stop_loss_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_take_profit_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.681696 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/market/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/market/test_buy_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/market/test_sell_market_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/test_unknown_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.681696 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/trailing/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/trailing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.685696 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.685696 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/test_future_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/test_margin_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/test_spot_asset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.685696 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29998 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52120 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio_profitability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio_value_holder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.685696 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85487 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/test_future_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/test_margin_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/test_spot_portfolio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/personal_data/positions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/personal_data/positions/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/personal_data/positions/states/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67901 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/test_position_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/test_positions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/personal_data/positions/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37444 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/types/test_inverse_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45251 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/positions/types/test_linear_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/personal_data/trades/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/trades/test_trade_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/trades/test_trade_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/personal_data/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/transactions/test_transaction_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/personal_data/transactions/test_transactions_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29656 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/signals/test_trading_signal_bundle_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/signals/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.689696 OctoBot-Trading-2.3.7/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/test_utils/order_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/test_utils/random_numbers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.693696 OctoBot-Trading-2.3.7/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests/util/test_config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.693696 OctoBot-Trading-2.3.7/tests_additional/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:40:01.697697 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/real_exchange_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_ascendex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitfinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bithumb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitstamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bittrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bybit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_coinbasepro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_coinex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_gateio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_hitbtc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_hollaex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_huobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_huobipro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_kucoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_ndax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_okcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_phemex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_poloniex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_upbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-01-12 01:39:04.000000 OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_wavesexchange.py
```

### Comparing `OctoBot-Trading-2.3.4/CHANGELOG.md` & `OctoBot-Trading-2.3.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.3.7] - 2023-01-11
+### Updated
+- [Orders] Properly handle pending creation orders for exchanges that work this way (ex: bybit)
+### Fixed
+- [Orders] Initial open order fetch timeout error### Fixed
+- [Adapters] Ticker, OHLCV and order issues
+
+## [2.3.6] - 2023-01-09
+### Added
+- [Config] Log trading mode and exchange config on load
+### Updated
+- [Exchanges] Migrate from cryptofeed to ccxt_pro for websocket exchanges
+
+## [2.3.5] - 2023-01-06
+### Updated
+- [Exchanges] Refactor exchanges to simplify into rest exchange, connectors and adapters
+
 ## [2.3.4] - 2023-01-02
 ### Updated
 - [CCXT] bump to 2.4.60
 
 ## [2.3.3] - 2023-01-01
 ### Updated
 - [API] add exchange data getter
```

### Comparing `OctoBot-Trading-2.3.4/LICENSE` & `OctoBot-Trading-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/PKG-INFO` & `OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.3.4
+Version: 2.3.7
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.3.4](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.3.7](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.3.4/OctoBot_Trading.egg-info/SOURCES.txt` & `OctoBot-Trading-2.3.7/OctoBot_Trading.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -151,66 +151,58 @@
 octobot_trading/exchanges/exchange_factory.py
 octobot_trading/exchanges/exchange_manager.pxd
 octobot_trading/exchanges/exchange_manager.py
 octobot_trading/exchanges/exchange_websocket_factory.pxd
 octobot_trading/exchanges/exchange_websocket_factory.py
 octobot_trading/exchanges/exchanges.pxd
 octobot_trading/exchanges/exchanges.py
+octobot_trading/exchanges/adapters/__init__.py
+octobot_trading/exchanges/adapters/abstract_adapter.py
 octobot_trading/exchanges/config/__init__.pxd
 octobot_trading/exchanges/config/__init__.py
 octobot_trading/exchanges/config/backtesting_exchange_config.pxd
 octobot_trading/exchanges/config/backtesting_exchange_config.py
 octobot_trading/exchanges/config/exchange_config_data.pxd
 octobot_trading/exchanges/config/exchange_config_data.py
 octobot_trading/exchanges/connectors/__init__.pxd
 octobot_trading/exchanges/connectors/__init__.py
-octobot_trading/exchanges/connectors/abstract_websocket_connector.pxd
-octobot_trading/exchanges/connectors/abstract_websocket_connector.py
-octobot_trading/exchanges/connectors/ccxt_exchange.pxd
-octobot_trading/exchanges/connectors/ccxt_exchange.py
-octobot_trading/exchanges/connectors/ccxt_websocket_connector.pxd
-octobot_trading/exchanges/connectors/ccxt_websocket_connector.py
-octobot_trading/exchanges/connectors/cryptofeed_websocket_connector.pxd
-octobot_trading/exchanges/connectors/cryptofeed_websocket_connector.py
-octobot_trading/exchanges/connectors/exchange_simulator.pxd
-octobot_trading/exchanges/connectors/exchange_simulator.py
+octobot_trading/exchanges/connectors/ccxt/__init__.pxd
+octobot_trading/exchanges/connectors/ccxt/__init__.py
+octobot_trading/exchanges/connectors/ccxt/ccxt_adapter.py
+octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.pxd
+octobot_trading/exchanges/connectors/ccxt/ccxt_client_util.py
+octobot_trading/exchanges/connectors/ccxt/ccxt_connector.pxd
+octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py
+octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.pxd
+octobot_trading/exchanges/connectors/ccxt/ccxt_websocket_connector.py
+octobot_trading/exchanges/connectors/ccxt/constants.py
+octobot_trading/exchanges/connectors/ccxt/enums.py
+octobot_trading/exchanges/connectors/simulator/__init__.pxd
+octobot_trading/exchanges/connectors/simulator/__init__.py
+octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py
+octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.pxd
+octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py
 octobot_trading/exchanges/implementations/__init__.pxd
 octobot_trading/exchanges/implementations/__init__.py
-octobot_trading/exchanges/implementations/ccxt_websocket_exchange.pxd
-octobot_trading/exchanges/implementations/ccxt_websocket_exchange.py
-octobot_trading/exchanges/implementations/cryptofeed_websocket_exchange.pxd
-octobot_trading/exchanges/implementations/cryptofeed_websocket_exchange.py
-octobot_trading/exchanges/implementations/default_spot_ccxt_exchange.py
-octobot_trading/exchanges/implementations/future_ccxt_exchange.pxd
-octobot_trading/exchanges/implementations/future_ccxt_exchange.py
-octobot_trading/exchanges/implementations/future_exchange_simulator.pxd
-octobot_trading/exchanges/implementations/future_exchange_simulator.py
-octobot_trading/exchanges/implementations/margin_ccxt_exchange.pxd
-octobot_trading/exchanges/implementations/margin_ccxt_exchange.py
-octobot_trading/exchanges/implementations/margin_exchange_simulator.pxd
-octobot_trading/exchanges/implementations/margin_exchange_simulator.py
-octobot_trading/exchanges/implementations/rest_exchange.py
-octobot_trading/exchanges/implementations/spot_ccxt_exchange.pxd
-octobot_trading/exchanges/implementations/spot_ccxt_exchange.py
-octobot_trading/exchanges/implementations/spot_exchange_simulator.pxd
-octobot_trading/exchanges/implementations/spot_exchange_simulator.py
+octobot_trading/exchanges/implementations/default_rest_exchange.pxd
+octobot_trading/exchanges/implementations/default_rest_exchange.py
+octobot_trading/exchanges/implementations/default_websocket_exchange.pxd
+octobot_trading/exchanges/implementations/default_websocket_exchange.py
+octobot_trading/exchanges/implementations/exchange_simulator.pxd
+octobot_trading/exchanges/implementations/exchange_simulator.py
 octobot_trading/exchanges/traders/__init__.pxd
 octobot_trading/exchanges/traders/__init__.py
 octobot_trading/exchanges/traders/trader.pxd
 octobot_trading/exchanges/traders/trader.py
 octobot_trading/exchanges/traders/trader_simulator.pxd
 octobot_trading/exchanges/traders/trader_simulator.py
 octobot_trading/exchanges/types/__init__.pxd
 octobot_trading/exchanges/types/__init__.py
-octobot_trading/exchanges/types/future_exchange.pxd
-octobot_trading/exchanges/types/future_exchange.py
-octobot_trading/exchanges/types/margin_exchange.pxd
-octobot_trading/exchanges/types/margin_exchange.py
-octobot_trading/exchanges/types/spot_exchange.pxd
-octobot_trading/exchanges/types/spot_exchange.py
+octobot_trading/exchanges/types/rest_exchange.pxd
+octobot_trading/exchanges/types/rest_exchange.py
 octobot_trading/exchanges/types/websocket_exchange.pxd
 octobot_trading/exchanges/types/websocket_exchange.py
 octobot_trading/exchanges/util/__init__.pxd
 octobot_trading/exchanges/util/__init__.py
 octobot_trading/exchanges/util/exchange_market_status_fixer.pxd
 octobot_trading/exchanges/util/exchange_market_status_fixer.py
 octobot_trading/exchanges/util/exchange_util.pxd
@@ -293,14 +285,16 @@
 octobot_trading/personal_data/orders/states/close_order_state.py
 octobot_trading/personal_data/orders/states/fill_order_state.pxd
 octobot_trading/personal_data/orders/states/fill_order_state.py
 octobot_trading/personal_data/orders/states/open_order_state.pxd
 octobot_trading/personal_data/orders/states/open_order_state.py
 octobot_trading/personal_data/orders/states/order_state_factory.pxd
 octobot_trading/personal_data/orders/states/order_state_factory.py
+octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.pxd
+octobot_trading/personal_data/orders/states/pending_creation_chained_order_state.py
 octobot_trading/personal_data/orders/states/pending_creation_order_state.pxd
 octobot_trading/personal_data/orders/states/pending_creation_order_state.py
 octobot_trading/personal_data/orders/types/__init__.pxd
 octobot_trading/personal_data/orders/types/__init__.py
 octobot_trading/personal_data/orders/types/unknown_order.pxd
 octobot_trading/personal_data/orders/types/unknown_order.py
 octobot_trading/personal_data/orders/types/limit/__init__.pxd
@@ -520,16 +514,19 @@
 tests/exchanges/test_exchange_builder.py
 tests/exchanges/test_exchange_config_data.py
 tests/exchanges/test_exchange_factory.py
 tests/exchanges/test_exchange_manager.py
 tests/exchanges/test_exchange_simulator.py
 tests/exchanges/test_exchanges.py
 tests/exchanges/connectors/__init__.py
-tests/exchanges/connectors/test_ccxt_exchange.py
+tests/exchanges/connectors/ccxt/__init__.py
+tests/exchanges/connectors/ccxt/test_ccxt_connector.py
 tests/exchanges/implementations/__init__.py
+tests/exchanges/implementations/test_default_rest_exchange.py
+tests/exchanges/implementations/test_default_websocket_exchange.py
 tests/exchanges/traders/__init__.py
 tests/exchanges/traders/test_trader.py
 tests/exchanges/types/__init__.py
 tests/exchanges/types/test_websocket_exchange.py
 tests/exchanges/util/__init__.py
 tests/exchanges/util/test_exchange_market_status_fixer.py
 tests/exchanges/util/test_exchange_util.py
@@ -556,14 +553,15 @@
 tests/personal_data/orders/states/__init__.py
 tests/personal_data/orders/states/test_cancel_order_state.py
 tests/personal_data/orders/states/test_close_order_state.py
 tests/personal_data/orders/states/test_fill_order_state.py
 tests/personal_data/orders/states/test_open_order_state.py
 tests/personal_data/orders/states/test_order_state.py
 tests/personal_data/orders/states/test_order_state_factory.py
+tests/personal_data/orders/states/test_pending_creation_chained_order_state.py
 tests/personal_data/orders/states/test_pending_creation_order_state.py
 tests/personal_data/orders/types/__init__.py
 tests/personal_data/orders/types/test_unknown_order.py
 tests/personal_data/orders/types/limit/__init__.py
 tests/personal_data/orders/types/limit/test_buy_limit_order.py
 tests/personal_data/orders/types/limit/test_sell_limit_order.py
 tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py
```

### Comparing `OctoBot-Trading-2.3.4/PKG-INFO` & `OctoBot-Trading-2.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot-Trading
-Version: 2.3.4
+Version: 2.3.7
 Summary: OctoBot project trading package
 Home-page: https://github.com/Drakkar-Software/OctoBot-Trading
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 License-File: LICENSE
 
-# OctoBot-Trading [2.3.4](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.3.7](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.3.4/README.md` & `OctoBot-Trading-2.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Trading [2.3.4](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
+# OctoBot-Trading [2.3.7](https://github.com/Drakkar-Software/OctoBot-Trading/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/903b6b22bceb4661b608a86fea655f69)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Trading?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Trading&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Trading.svg)](https://pypi.python.org/pypi/OctoBot-Trading/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Trading/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Trading?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Trading/workflows/OctoBot-Trading-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Trading/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Trading/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Trading)
 
 OctoBot trading package.
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 PROJECT_NAME = "OctoBot-Trading"
-VERSION = "2.3.4"  # major.minor.revision
+VERSION = "2.3.7"  # major.minor.revision
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     subscribe_to_trades_channel,
     subscribe_to_order_channel,
 )
 from octobot_trading.api.exchange import (
     create_exchange_builder,
     get_exchange_configurations_from_exchange_name,
     get_exchange_manager_from_exchange_name_and_id,
-    get_exchange_available_time_frames,
+    get_ccxt_exchange_available_time_frames,
     get_exchange_available_required_time_frames,
     get_exchange_configuration_from_exchange_id,
     get_exchange_manager_from_exchange_id,
     get_exchange_managers_from_exchange_ids,
     get_trading_exchanges,
     is_exchange_trading,
     get_exchange_manager_id,
@@ -216,15 +216,15 @@
     "get_win_rate",
     "subscribe_to_ohlcv_channel",
     "subscribe_to_trades_channel",
     "subscribe_to_order_channel",
     "create_exchange_builder",
     "get_exchange_configurations_from_exchange_name",
     "get_exchange_manager_from_exchange_name_and_id",
-    "get_exchange_available_time_frames",
+    "get_ccxt_exchange_available_time_frames",
     "get_exchange_available_required_time_frames",
     "get_exchange_configuration_from_exchange_id",
     "get_exchange_manager_from_exchange_id",
     "get_exchange_managers_from_exchange_ids",
     "get_trading_exchanges",
     "is_exchange_trading",
     "get_exchange_manager_id",
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/channels.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/contracts.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/contracts.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
 import trading_backend
 
 import octobot_trading.constants
 import octobot_trading.enums
+import octobot_trading.exchanges.connectors.ccxt.enums
 import octobot_trading.exchanges as exchanges
 import octobot_trading.exchange_data as exchange_data
 
 import octobot_backtesting.api as backtesting_api
 
 
 def create_exchange_builder(config, exchange_name: str) -> exchanges.ExchangeBuilder:
@@ -37,22 +38,23 @@
     return exchanges.Exchanges.instance().get_exchanges(exchange_name)
 
 
 def get_exchange_manager_from_exchange_name_and_id(exchange_name: str, exchange_id: str) -> object:
     return exchanges.Exchanges.instance().get_exchange(exchange_name, exchange_id).exchange_manager
 
 
-async def get_exchange_available_time_frames(
+async def get_ccxt_exchange_available_time_frames(
         exchange_name: str,
-        exchange_lib: octobot_trading.enums.ExchangeWrapperLibs = octobot_trading.enums.ExchangeWrapperLibs.CCXT
+        exchange_lib: octobot_trading.exchanges.connectors.ccxt.enums.ExchangeWrapperLibs =
+        octobot_trading.exchanges.connectors.ccxt.enums.ExchangeWrapperLibs.CCXT
 ) -> list:
     """
     When using CCXT, prefer using the sync lib since no request is required to get time frames
     :param exchange_name: name of the exchange
-    :param exchange_lib: octobot_trading.enums.ExchangeWrapperLibs to use
+    :param exchange_lib: octobot_trading.exchanges.connectors.ccxt.enums.ExchangeWrapperLibs to use
     :return: the list of time frames
     """
     try:
         # first try in available exchanges
         for exchange_configuration in get_exchange_configurations_from_exchange_name(exchange_name).values():
             return exchange_configuration.exchange_manager.client_time_frames
     except KeyError:
@@ -160,15 +162,15 @@
 
 
 def get_exchange_type(exchange_manager) -> octobot_trading.enums.ExchangeTypes:
     return exchanges.get_exchange_type(exchange_manager)
 
 
 def has_only_ohlcv(exchange_importers):
-    return exchanges.ExchangeSimulator.get_real_available_data(exchange_importers) == \
+    return exchanges.ExchangeSimulatorConnector.get_real_available_data(exchange_importers) == \
            set(exchange_data.SIMULATOR_PRODUCERS_TO_POSSIBLE_DATA_TYPE[octobot_trading.constants.OHLCV_CHANNEL])
 
 
 def get_is_backtesting(exchange_manager) -> bool:
     return exchange_manager.is_backtesting
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/modes.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/modes.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/orders.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/orders.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,21 +23,26 @@
 
 
 async def create_order(exchange_manager,
                        order_type: octobot_trading.enums.TraderOrderType,
                        symbol: str,
                        current_price: float,
                        quantity: float,
-                       price: float) -> personal_data.Order:
+                       price: float,
+                       wait_for_creation=True,
+                       creation_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT) -> personal_data.Order:
     return await exchange_manager.trader.create_order(
         exchange_manager.trader.create_order_instance(order_type=order_type,
                                                       symbol=symbol,
                                                       current_price=current_price,
                                                       quantity=quantity,
-                                                      price=price))
+                                                      price=price),
+        wait_for_creation=wait_for_creation,
+        creation_timeout=creation_timeout
+    )
 
 
 def get_open_orders(exchange_manager) -> list:
     return exchange_manager.exchange_personal_data.orders_manager.get_open_orders()
 
 
 async def cancel_all_open_orders(exchange_manager, emit_trading_signals=True) -> bool:
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/portfolio.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/positions.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/profitability.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/storage.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/symbol_data.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/trader.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/api/trades.py` & `OctoBot-Trading-2.3.7/octobot_trading/api/trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/constants.py` & `OctoBot-Trading-2.3.7/octobot_trading/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,28 +53,29 @@
 DEFAULT_CANDLE_HISTORY_SIZE = 200
 DEFAULT_FAILED_REQUEST_RETRY_TIME = 1
 DEFAULT_REQUEST_TIMEOUT = int(os.getenv("DEFAULT_REQUEST_TIMEOUT", "20000"))    # default ccxt is 10s, use 20
 ENABLE_EXCHANGE_HTTP_PROXY_FROM_ENV = os_util.parse_boolean_environment_var(
     "ENABLE_EXCHANGE_HTTP_PROXY_FROM_ENV", "True")
 ENABLE_CCXT_VERBOSE = os_util.parse_boolean_environment_var("ENABLE_CCXT_VERBOSE", "False")
 ENABLE_CCXT_RATE_LIMIT = os_util.parse_boolean_environment_var("ENABLE_CCXT_RATE_LIMIT", "True")
+THROTTLED_WS_UPDATES = float(os.getenv("THROTTLED_WS_UPDATES", "0.1"))  # avoid spamming CPU
 
 # Decimal default values (decimals are immutable, can be stored as constant)
 ZERO = decimal.Decimal(0)
 ONE = decimal.Decimal(1)
 ONE_HUNDRED = decimal.Decimal(100)
 NaN = decimal.Decimal("nan")
 
 FULL_CANDLE_HISTORY_EXCHANGES = ["bequant", "binance", "binanceus", "binanceusdm", "bitcoincom",
                                  "bitfinex", "bitfinex2", "bitmex", "idex", "bybit"]
 
 TESTED_EXCHANGES = ["binance", "okx", "gateio", "huobi", "bitget",
                     "ascendex", "kucoin", "coinbasepro", "bybit", "phemex", "hollaex"]
 DEFAULT_FUTURE_EXCHANGES = ["bybit"]
-SIMULATOR_TESTED_EXCHANGES = ["bitfinex", "bithumb", "bitstamp", "bittrex", "coinex",
+SIMULATOR_TESTED_EXCHANGES = ["bitfinex2", "bithumb", "bitstamp", "bittrex", "coinex",
                               "hitbtc", "kraken", "poloniex", "bitso", "ndax", "upbit",
                               "wavesexchange"]
 
 CONFIG_DEFAULT_FEES = 0.001
 CONFIG_DEFAULT_SIMULATOR_FEES = 0
 
 DEFAULT_SYMBOL_LEVERAGE = ONE
@@ -114,17 +115,14 @@
 
 # 946742400 is 01/01/2000, if trade time is lower, there is an issue.
 MINIMUM_VAL_TRADE_TIME = 946688400
 
 # Internal
 MODE_CHANNEL = "Mode"
 
-# CCXT library constants
-CCXT_INFO = "info"
-
 WEBSOCKET_FEEDS_TO_TRADING_CHANNELS = {
     TICKER_CHANNEL: [enums.WebsocketFeeds.TICKER],
     MINI_TICKER_CHANNEL: [enums.WebsocketFeeds.MINI_TICKER],
     RECENT_TRADES_CHANNEL: [enums.WebsocketFeeds.TRADES],
     LIQUIDATIONS_CHANNEL: [enums.WebsocketFeeds.LIQUIDATIONS],
     ORDER_BOOK_CHANNEL: [enums.WebsocketFeeds.L2_BOOK, enums.WebsocketFeeds.L3_BOOK],
     ORDER_BOOK_TICKER_CHANNEL: [enums.WebsocketFeeds.BOOK_TICKER],
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/enums.py` & `OctoBot-Trading-2.3.7/octobot_trading/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,81 +156,14 @@
 
 
 class PositionMode(enum.Enum):
     HEDGE = "hedge_mode"
     ONE_WAY = "one_way_mode"
 
 
-class ExchangeConstantsCCXTColumns(enum.Enum):
-    TIMESTAMP = "timestamp"
-    DATETIME = "datetime"
-
-
-class ExchangePositionCCXTColumns(enum.Enum):
-    CONTRACTS = "contracts"
-    CONTRACT_SIZE = "contractSize"
-    MARGIN_TYPE = "marginType"
-    MARGIN_MODE = "marginMode"
-    LEVERAGE = "leverage"
-    SYMBOL = "symbol"
-    COLLATERAL = "collateral"
-    INITIAL_MARGIN = "initialMargin"
-    INITIAL_MARGIN_PERCENTAGE = "initialMarginPercentage"
-    MAINTENANCE_MARGIN = "maintenanceMargin"
-    MAINTENANCE_MARGIN_PERCENTAGE = "maintenanceMarginPercentage"
-    NOTIONAL = "notional"
-    MARGIN_RATIO = "marginRatio"
-    UNREALISED_PNL = "unrealizedPnl"
-    REALISED_PNL = "realizedPnl"
-    LIQUIDATION_PRICE = "liquidationPrice"
-    MARK_PRICE = "markPrice"
-    ENTRY_PRICE = "entryPrice"
-    TIMESTAMP = "timestamp"
-    DATETIME = "datetime"
-    PERCENTAGE = "percentage"
-    SIDE = "side"
-    INFO = "info"
-
-
-class ExchangeFundingCCXTColumns(enum.Enum):
-    SYMBOL = "symbol"
-    LAST_FUNDING_TIME = "lastFundingTime"
-    FUNDING_RATE = "fundingRate"
-    NEXT_FUNDING_TIME = "nextFundingTime"
-    PREDICTED_FUNDING_RATE = "predictedFundingRate"
-
-
-class ExchangeOrderCCXTColumns(enum.Enum):
-    INFO = "info"
-    ID = "id"
-    TIMESTAMP = "timestamp"
-    DATETIME = 'datetime'
-    LAST_TRADE_TIMESTAMP = "lastTradeTimestamp"
-    SYMBOL = "symbol"
-    QUANTITY_CURRENCY = "quantityCurrency"
-    TYPE = "type"
-    SIDE = "side"
-    PRICE = "price"
-    AMOUNT = "amount"
-    COST = "cost"
-    AVERAGE = "average"
-    FILLED = "filled"
-    REMAINING = "remaining"
-    STATUS = "status"
-    FEE = "fee"
-    TRADES = "trades"
-    MAKER = "maker"
-    TAKER = "taker"
-    ORDER = "order"
-    TAKER_OR_MAKER = "takerOrMaker"
-    REDUCE_ONLY = "reduceOnly"
-    STOP_PRICE = "stopPrice"
-    TRIGGER_ABOVE = "triggerAbove"
-    TAG = "tag"
-
 class ExchangeConstantsFundingColumns(enum.Enum):
     SYMBOL = "symbol"
     LAST_FUNDING_TIME = "last_funding_time"
     FUNDING_RATE = "funding_rate"
     NEXT_FUNDING_TIME = "next_funding_time"
     PREDICTED_FUNDING_RATE = "predicted_funding_rate"
 
@@ -470,14 +403,17 @@
     TICKER = 'ticker'
     CANDLE = 'candle'
     KLINE = 'kline'
     FUNDING = 'funding'
     MARK_PRICE = 'mark_price'
     LAST_PRICE = 'last_price'
     ORDERS = 'orders'
+    LEDGER = 'ledger'
+    CREATE_ORDER = 'create_order'
+    CANCEL_ORDER = 'cancel_order'
     FUTURES_INDEX = 'futures_index'
     OPEN_INTEREST = 'open_interest'
     PORTFOLIO = 'portfolio'
     POSITION = 'position'
     TRADE = 'trade'
     TRANSACTIONS = 'transactions'
     VOLUME = 'volume'
@@ -508,19 +444,14 @@
 
 
 class SubAccountColumns(enum.Enum):
     ID = "id"
     NAME = "name"
 
 
-class ExchangeWrapperLibs(enum.Enum):
-    ASYNC_CCXT = "async_ccxt"
-    CCXT = "ccxt"
-
-
 class ExchangeTypes(enum.Enum):
     SPOT = "spot"
     FUTURE = "future"
     MARGIN = "margin"
     UNKNOWN = "unknown"
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/errors.py` & `OctoBot-Trading-2.3.7/octobot_trading/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,7 +182,19 @@
     """
 
 
 class OrderDescriptionNotFoundError(Exception):
     """
     Raised when an order description is not found
     """
+
+
+class AdapterError(Exception):
+    """
+    Raised when an error occurs in an adapter
+    """
+
+
+class UnexpectedAdapterError(Exception):
+    """
+    Raised when an unexpected error occurs in an adapter
+    """
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_channel.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_channel.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_channel.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/contract_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/future_contract.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/future_contract.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/future_contract.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/margin_contract.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/margin_contract.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/contracts/margin_contract.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/contracts/margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbol_data.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbol_data.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbol_data.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbols_data.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbols_data.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/exchange_symbols_data.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,16 @@
             funding: dict = await self.channel.exchange_manager.exchange.get_funding_rate(symbol)
 
             if funding:
                 next_funding_time = funding[enums.ExchangeConstantsFundingColumns.NEXT_FUNDING_TIME.value]
                 predicted_funding_rate = \
                     funding.get(enums.ExchangeConstantsFundingColumns.PREDICTED_FUNDING_RATE.value, constants.NaN)
                 await self._push_funding(
-                    symbol=symbol,
-                    funding_rate=decimal.Decimal(funding[enums.ExchangeConstantsFundingColumns.FUNDING_RATE.value]),
+                    symbol,
+                    decimal.Decimal(funding[enums.ExchangeConstantsFundingColumns.FUNDING_RATE.value]),
                     predicted_funding_rate=decimal.Decimal(str(predicted_funding_rate or constants.NaN)),
                     next_funding_time=next_funding_time,
                     last_funding_time=funding[enums.ExchangeConstantsFundingColumns.LAST_FUNDING_TIME.value])
                 return next_funding_time
         except (errors.NotSupported, NotImplementedError) as ne:
             self.logger.exception(ne, True, f"get_funding_rate is not supported by "
                                             f"{self.channel.exchange_manager.exchange.name} : {ne}")
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/channel/funding_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/funding_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/funding_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/funding/funding_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/funding/funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/channel/kline_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/kline_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/kline_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/kline/kline_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/kline/kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_adapter.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_adapter.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_adapter.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/candles_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,14 @@
             candles = []
             async for new_candles in exchanges.get_historical_ohlcv(self.channel.exchange_manager, pair,
                                                                     time_frame, start_time, end_time):
                 candles += new_candles
             return candles
         candles: list = await self.channel.exchange_manager.exchange \
             .get_symbol_prices(pair, time_frame, limit=self.OHLCV_OLD_LIMIT)
-        self.channel.exchange_manager.exchange.uniformize_candles_if_necessary(candles)
         return candles
 
     async def _initialize_candles(self, time_frame, pair, should_retry) \
             -> (str, common_enums.TimeFrames, list):
         """
         Manage timeframe OHLCV data refreshing for all pairs
         :return: a tuple with (trading pair, time_frame, fetched candles)
@@ -178,15 +177,14 @@
                 if self.initialized_candles_by_tf_by_symbol[pair][time_frame]:
                     candles: list = await self.channel.exchange_manager.exchange.get_symbol_prices(
                         pair,
                         time_frame,
                         limit=self.OHLCV_LIMIT)
                     if candles:
                         last_candle: list = candles[-1]
-                        self.channel.exchange_manager.exchange.uniformize_candles_if_necessary(candles)
                     else:
                         last_candle: list = []
 
                     if last_candle and len(candles) > 1:
                         last_candle_timestamp, sleep_time = await self._refresh_current_candle(
                             time_frame, pair, candles, last_candle, last_candle_timestamp, time_frame_sleep
                         )
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/channel/ohlcv_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ohlcv/preloaded_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/channel/order_book_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/order_book_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/order_book_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/order_book/order_book_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/order_book/order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/price.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/price.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/price.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/price.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/channel/prices_updater_simulator.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,29 +10,33 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import octobot_trading.constants as constants
+import octobot_trading.exchanges as exchanges
 import octobot_trading.exchange_data.prices.channel.prices_updater as prices_updater
 import octobot_trading.exchange_channel as exchanges_channel
 
 
 class MarkPriceUpdaterSimulator(prices_updater.MarkPriceUpdater):
     def __init__(self, channel, importer):
         super().__init__(channel)
         self.exchange_data_importer = importer
 
     async def start(self):
         exchange = self.channel.exchange_manager.exchange
-        available_data = exchange.get_real_available_data(exchange.exchange_importers)
-        real_data_for_recent_trades = exchange.handles_real_data_for_updater(constants.RECENT_TRADES_CHANNEL,
-                                                                             available_data)
-        real_data_for_ticker = exchange.handles_real_data_for_updater(constants.TICKER_CHANNEL, available_data)
+        available_data = exchanges.ExchangeSimulatorConnector.get_real_available_data(exchange.exchange_importers)
+        real_data_for_recent_trades = exchanges.ExchangeSimulatorConnector.handles_real_data_for_updater(
+            constants.RECENT_TRADES_CHANNEL, available_data
+        )
+        real_data_for_ticker = exchanges.ExchangeSimulatorConnector.handles_real_data_for_updater(
+            constants.TICKER_CHANNEL, available_data
+        )
         # if recent trades and ticker channels are both generated from ohlcv, do not watch them both,
         # prefer ticker
         if real_data_for_ticker or not (real_data_for_recent_trades or real_data_for_ticker):
             await exchanges_channel.get_chan(constants.TICKER_CHANNEL,
                                              self.channel.exchange_manager.id).new_consumer(self.handle_ticker_update)
         if real_data_for_recent_trades:
             await exchanges_channel.get_chan(constants.RECENT_TRADES_CHANNEL, self.channel.exchange_manager.id) \
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/price_events_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/price_events_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/price_events_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/prices_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/prices_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/prices/prices_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/prices/prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,15 @@
 
     async def init_recent_trades(self):
         try:
             for pair in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
                 recent_trades = await self.channel.exchange_manager.exchange.\
                     get_recent_trades(pair, limit=self.RECENT_TRADE_LIMIT)
                 if recent_trades:
-                    await self.push(pair,
-                                    list(map(self.channel.exchange_manager.exchange.clean_recent_trade,
-                                             recent_trades)))
+                    await self.push(pair, recent_trades)
             await asyncio.sleep(self.refresh_time)
         except Exception as e:
             self.logger.exception(e, True, f"Fail to initialize recent trades : {e}")
 
     async def start(self):
         refresh_threshold = self.channel.exchange_manager.get_rest_pairs_refresh_threshold()
         if refresh_threshold is enums.RestExchangePairsRefreshMaxThresholds.MEDIUM:
@@ -62,17 +60,15 @@
         while not self.should_stop and not self.channel.is_paused:
             try:
                 for pair in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
                     recent_trades = await self.channel.exchange_manager.exchange.\
                         get_recent_trades(pair, limit=self.RECENT_TRADE_LIMIT)
                     if recent_trades:
                         try:
-                            await self.push(pair,
-                                            list(map(self.channel.exchange_manager.exchange.clean_recent_trade,
-                                                     recent_trades)))
+                            await self.push(pair, recent_trades)
                         except TypeError:
                             pass
                 await asyncio.sleep(self.refresh_time)
             except errors.FailedRequest as e:
                 self.logger.warning(str(e))
                 # avoid spamming on disconnected situation
                 await asyncio.sleep(constants.DEFAULT_FAILED_REQUEST_RETRY_TIME)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/channel/recent_trade_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/recent_trades_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/recent_trades_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/recent_trades/recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater.pxd`

 * *Files 19% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchange_data.ticker.channel.ticker as ticker_channel
+cimport octobot_trading.personal_data.positions.channel.positions as positions_channel
 
-cdef class TickerUpdater(ticker_channel.TickerProducer):
-    cdef list _added_pairs
-    cdef bint is_fetching_future_data
-    cdef int refresh_time
+cimport octobot_commons.async_job as async_job
 
-    cdef dict _cleanup_ticker_dict(self, dict ticker)
-    cdef list _get_pairs_to_update(self)
-    cdef bint _should_use_future(self)
-    cdef void _update_refresh_time(self)
+cdef class PositionsUpdater(positions_channel.PositionsProducer):
+    cdef public bint should_use_position_per_symbol
+
+    cdef async_job.AsyncJob position_update_job
+
+    cdef bint _should_run(self)
+    cdef bint _should_push_mark_price(self)
+    cdef bint _has_mark_price_in_position(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=E0611
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,196 +9,186 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import decimal
-
 import asyncio
 
+import trading_backend
+
+import octobot_commons.authentication as authentication
 import octobot_trading.errors as errors
-import octobot_trading.exchange_channel as exchanges_channel
-import octobot_trading.constants as constants
-import octobot_trading.exchange_data.ticker.channel.ticker as ticker_channel
-import octobot_trading.enums as enums
-
-
-class TickerUpdater(ticker_channel.TickerProducer):
-    CHANNEL_NAME = constants.TICKER_CHANNEL
-    TICKER_REFRESH_TIME = 64
-    TICKER_FUTURE_REFRESH_TIME = 14
-    TICKER_REFRESH_DELAY_THRESHOLD = 10
-
-    def __init__(self, channel):
-        super().__init__(channel)
-        self._added_pairs = []
-        self.is_fetching_future_data = False
-        self.refresh_time = self.TICKER_REFRESH_TIME
-
-    async def start(self):
-        if self._should_use_future():
-            self.is_fetching_future_data = True
-            self.refresh_time = self.TICKER_FUTURE_REFRESH_TIME
-        if self.channel.is_paused:
-            await self.pause()
-        else:
-            # initialize ticker
-            await asyncio.gather(*[self._fetch_ticker(pair)
-                                   for pair in self._get_pairs_to_update()])
-            await asyncio.sleep(self.refresh_time)
-            await self.start_update_loop()
-
-    async def start_update_loop(self):
-        while not self.should_stop and not self.channel.is_paused:
-            try:
-                for pair in self._get_pairs_to_update():
-                    await self._fetch_ticker(pair)
-
-                await asyncio.sleep(self.refresh_time)
-            except errors.NotSupported:
-                self.logger.warning(f"{self.channel.exchange_manager.exchange_name} is not supporting updates")
-                await self.pause()
-            except Exception as e:
-                self.logger.exception(e, True, f"Fail to update ticker : {e}")
+import octobot_trading.exchanges as exchanges
 
-    async def _fetch_ticker(self, pair):
-        try:
-            ticker: dict = await self.channel.exchange_manager.exchange.get_price_ticker(pair)
-            if self._is_valid(ticker):
-                await self.push(pair, ticker)
-                await self.parse_mini_ticker(pair, ticker)
-                if self.channel.exchange_manager.is_future:
-                    await self.parse_future_data(pair, ticker)
-            else:
-                self.logger.debug(f"Ignored incomplete ticker: {ticker}")
-        except errors.FailedRequest as e:
-            self.logger.warning(str(e))
-            # avoid spamming on disconnected situation
-            await asyncio.sleep(constants.DEFAULT_FAILED_REQUEST_RETRY_TIME)
 
-    @staticmethod
-    def _is_valid(ticker):
-        try:
-            # at least require close, volume and timestamp
-            return ticker and \
-                   all(ticker[field] is not None
-                       for field in (
-                           enums.ExchangeConstantsTickersColumns.CLOSE.value,
-                           enums.ExchangeConstantsTickersColumns.BASE_VOLUME.value,
-                           enums.ExchangeConstantsTickersColumns.TIMESTAMP.value
-                       ))
-        except KeyError:
-            return False
+async def create_exchanges(exchange_manager):
+    if exchange_manager.is_sandboxed and not exchange_manager.exchange_only:
+        exchange_manager.logger.info(f"Using sandbox exchange for {exchange_manager.exchange_name}")
 
-    def _cleanup_ticker_dict(self, ticker):
-        try:
-            ticker.pop("info")
-            ticker.pop("symbol")
-            ticker.pop("datetime")
-        except KeyError as e:
-            self.logger.error(f"Fail to cleanup ticker dict ({e})")
-        return ticker
-
-    def _get_pairs_to_update(self):
-        return self.channel.exchange_manager.exchange_config.traded_symbol_pairs + self._added_pairs
-
-    async def parse_mini_ticker(self, pair, ticker):
-        """
-        Mini ticker
-        """
-        try:
-            await exchanges_channel.get_chan(constants.MINI_TICKER_CHANNEL,
-                                             self.channel.exchange_manager.id).get_internal_producer(). \
-                push(pair, {
-                enums.ExchangeConstantsMiniTickerColumns.HIGH_PRICE.value:
-                    ticker[enums.ExchangeConstantsTickersColumns.HIGH.value],
-                enums.ExchangeConstantsMiniTickerColumns.LOW_PRICE.value:
-                    ticker[enums.ExchangeConstantsTickersColumns.LOW.value],
-                enums.ExchangeConstantsMiniTickerColumns.OPEN_PRICE.value:
-                    ticker[enums.ExchangeConstantsTickersColumns.OPEN.value],
-                enums.ExchangeConstantsMiniTickerColumns.CLOSE_PRICE.value:
-                    ticker[enums.ExchangeConstantsTickersColumns.CLOSE.value],
-                enums.ExchangeConstantsMiniTickerColumns.VOLUME.value:
-                    ticker[enums.ExchangeConstantsTickersColumns.BASE_VOLUME.value],
-                enums.ExchangeConstantsMiniTickerColumns.TIMESTAMP.value:
-                    ticker[enums.ExchangeConstantsTickersColumns.TIMESTAMP.value]})
-        except Exception as e:
-            self.logger.error(f"Failed to parse mini ticker : {e}")
-
-    """
-    Future data management
-    """
-
-    def _should_use_future(self):
-        return self.channel.exchange_manager.is_future and \
-               (
-                       self.channel.exchange_manager.exchange.FUNDING_IN_TICKER
-                       or self.channel.exchange_manager.exchange.MARK_PRICE_IN_TICKER
-               )
-
-    async def parse_future_data(self, symbol: str, ticker: dict):
-        if self.channel.exchange_manager.exchange.MARK_PRICE_IN_TICKER:
-            await self.extract_mark_price(symbol, ticker)
+    if exchange_manager.is_backtesting:
+        # simulated : create exchange simulator instance
+        await create_simulated_exchange(exchange_manager)
+        exchange_manager.load_constants()
+    else:
+        # real : create a rest or websocket exchange instance
+        await create_real_exchange(exchange_manager)
+        exchange_manager.load_constants()
+        await initialize_real_exchange(exchange_manager)
 
-        if self.channel.exchange_manager.exchange.FUNDING_IN_TICKER:
-            await self.extract_funding_rate(symbol, ticker)
+    if not exchange_manager.exchange_only:
+        # create exchange producers if necessary
+        await exchanges.create_exchange_producers(exchange_manager)
 
-    async def extract_mark_price(self, symbol: str, ticker: dict):
-        try:
-            ticker = self.channel.exchange_manager.exchange.parse_mark_price(ticker, from_ticker=True)
-            await exchanges_channel.get_chan(constants.MARK_PRICE_CHANNEL,
-                                             self.channel.exchange_manager.id).get_internal_producer(). \
-                push(symbol,
-                     decimal.Decimal(str(ticker[enums.ExchangeConstantsMarkPriceColumns.MARK_PRICE.value])))
-        except Exception as e:
-            self.logger.exception(e, True, f"Fail to update mark price from ticker : {e}")
+    if exchange_manager.is_backtesting:
+        await init_simulated_exchange(exchange_manager)
 
-    async def extract_funding_rate(self, symbol: str, ticker: dict):
-        try:
-            ticker = self.channel.exchange_manager.exchange.parse_funding(ticker, from_ticker=True)
-            predicted_funding_rate = ticker.get(enums.ExchangeConstantsFundingColumns.PREDICTED_FUNDING_RATE.value,
-                                                constants.NaN)
-            await exchanges_channel.get_chan(constants.FUNDING_CHANNEL,
-                                             self.channel.exchange_manager.id).get_internal_producer(). \
-                push(symbol,
-                     decimal.Decimal(str(ticker[enums.ExchangeConstantsFundingColumns.FUNDING_RATE.value])),
-                     decimal.Decimal(str(predicted_funding_rate or constants.NaN)),
-                     ticker[enums.ExchangeConstantsFundingColumns.NEXT_FUNDING_TIME.value],
-                     ticker[enums.ExchangeConstantsFundingColumns.LAST_FUNDING_TIME.value])
-        except Exception as e:
-            self.logger.exception(e, True, f"Fail to update funding rate from ticker : {e}")
-
-    async def modify(self, added_pairs=None, removed_pairs=None):
-        if added_pairs:
-            to_add_pairs = [pair
-                            for pair in added_pairs
-                            if pair not in self._get_pairs_to_update()]
-            if to_add_pairs:
-                self._added_pairs += to_add_pairs
-                self.logger.info(f"Added pairs : {to_add_pairs}")
-                self._update_refresh_time()
-
-        if removed_pairs:
-            self._added_pairs -= removed_pairs
-            self.logger.info(f"Removed pairs : {removed_pairs}")
-            self._update_refresh_time()
-
-    def _update_refresh_time(self):
-        if self.is_fetching_future_data:
-            # do not change ticker update rate on futures
+    exchange_manager.exchange_name = exchange_manager.exchange.name
+    exchange_manager.is_ready = True
+
+
+async def create_real_exchange(exchange_manager) -> None:
+    """
+    Create and initialize real REST exchange
+    :param exchange_manager: the related exchange manager
+    """
+    await _create_rest_exchange(exchange_manager)
+    try:
+        await exchange_manager.exchange.initialize()
+        if exchange_manager.exchange_only:
             return
-        pairs_to_update_count = len(self._get_pairs_to_update())
-        delay_multiplier = pairs_to_update_count // self.TICKER_REFRESH_DELAY_THRESHOLD + 1
-        # there can be many ticker requests when a large number of currency is in a
-        # portfolio, in this case, limit those requests
-        self.refresh_time = self.TICKER_REFRESH_TIME * delay_multiplier
-
-    # async def config_callback(self, exchange, cryptocurrency, symbols, time_frames):
-    #     if symbols:
-    #         await self.modify(added_pairs=symbols)
-
-    async def resume(self) -> None:
-        await super().resume()
-        if not self.is_running:
-            await self.run()
+        _create_exchange_backend(exchange_manager)
+        await _initialize_exchange_backend(exchange_manager)
+        _ensure_exchange_validity(exchange_manager)
+    except errors.AuthenticationError:
+        exchange_manager.logger.error("Authentication error, retrying without authentication...")
+        exchange_manager.without_auth = True
+        await create_real_exchange(exchange_manager)
+        return
+
+
+async def initialize_real_exchange(exchange_manager):
+    if not exchange_manager.exchange_only:
+        await exchanges.create_exchange_channels(exchange_manager)
+
+    # create Websocket exchange if possible
+    if not exchange_manager.rest_only:
+        # search for websocket
+        if exchanges.check_web_socket_config(exchange_manager.config, exchange_manager.exchange.name):
+            await exchanges.search_and_create_websocket(exchange_manager)
+
+
+def _ensure_exchange_validity(exchange_manager):
+    if exchange_manager.is_future and \
+            not exchange_manager.is_trader_simulated and \
+            not exchange_manager.is_valid_account:
+        error_message = f"Impossible to check exchange sponsoring due to" \
+                        f" {exchange_manager.init_error.__class__.__name__}." \
+            if isinstance(exchange_manager.init_error, trading_backend.TimeSyncError) \
+            else \
+            f"Impossible to start futures trading for {exchange_manager.exchange.name.capitalize()}: " \
+            f"incompatible account with no registered donation. Your OctoBot will work normally " \
+            f"for spot trading but will be *limited to backtesting for futures trading. " \
+            f"Please select spot trading on your exchange configuration."
+        raise errors.NotSupported(error_message)
+
+
+def _create_exchange_backend(exchange_manager):
+    try:
+        exchange_manager.exchange_backend = trading_backend.exchange_factory.create_exchange_backend(
+            exchange_manager.exchange
+        )
+    except Exception as e:
+        exchange_manager.logger.exception(e, True, f"Error when creating exchange backend: {e}")
+
+
+async def _initialize_exchange_backend(exchange_manager):
+    if exchange_manager.exchange_backend is not None and exchange_manager.exchange.authenticated() \
+            and not exchange_manager.is_trader_simulated:
+        exchange_manager.logger.debug(await exchange_manager.exchange_backend.initialize())
+        if not exchange_manager.is_future:
+            return
+        try:
+            exchange_manager.is_valid_account = await _is_supporting_octobot()
+            if exchange_manager.is_valid_account:
+                return True
+            exchange_manager.is_valid_account, message = await exchange_manager.exchange_backend.is_valid_account()
+            if not exchange_manager.is_valid_account:
+                exchange_manager.logger.error(
+                    f"Incompatible {exchange_manager.exchange.name.capitalize()} account to use futures trading: "
+                    f"{message}. OctoBot relies on exchanges profits sharing to remain 100% free, please create a "
+                    f"new {exchange_manager.exchange.name.capitalize()} account or register a donation to support "
+                    f"the project. {exchanges.get_partners_explanation_message()}")
+        except trading_backend.TimeSyncError as err:
+            exchanges.log_time_sync_error(exchange_manager.logger, exchange_manager.exchange.name,
+                                          err, "account details")
+            exchange_manager.is_valid_account = False
+            exchange_manager.init_error = err
+        except Exception as err:
+            exchange_manager.is_valid_account = False
+            exchange_manager.init_error = err
+            exchange_manager.logger.exception(err, True, f"Error when loading exchange account: {err}")
+        finally:
+            if exchange_manager.is_valid_account:
+                exchange_manager.logger.info("On behalf of the OctoBot team, thank you for "
+                                             "actively supporting the project !")
+
+
+async def _is_supporting_octobot() -> bool:
+    try:
+        authenticator = authentication.Authenticator.instance()
+        if not authenticator.is_initialized():
+            initialization_timeout = 5
+            await authenticator.await_initialization(initialization_timeout)
+        if authenticator.user_account.supports.is_supporting():
+            return True
+    except asyncio.TimeoutError:
+        pass
+    return False
+
+
+async def _create_rest_exchange(exchange_manager) -> None:
+    """
+    create REST based on ccxt exchange
+    :param exchange_manager: the related exchange manager
+    """
+    await _search_and_create_rest_exchange(exchange_manager)
+
+    if not exchange_manager.exchange:
+        raise Exception(f"Can't create an exchange instance that match the exchange configuration ({exchange_manager})")
+
+
+async def create_simulated_exchange(exchange_manager):
+    exchange_manager.exchange = exchanges.ExchangeSimulator(
+        exchange_manager.config, exchange_manager, exchange_manager.backtesting
+    )
+
+    await exchange_manager.exchange.initialize()
+    _initialize_simulator_time_frames(exchange_manager)
+    exchange_manager.exchange_config.set_config_time_frame()
+    exchange_manager.exchange_config.set_config_traded_pairs()
+    await exchanges.create_exchange_channels(exchange_manager)
+
+
+async def init_simulated_exchange(exchange_manager):
+    await exchange_manager.exchange.create_backtesting_exchange_producers()
+
+
+async def _search_and_create_rest_exchange(exchange_manager) -> None:
+    """
+    Create a rest exchange if a RestExchange matching class is found
+    :param exchange_manager: the related exchange manager
+    """
+    rest_exchange_class = exchanges.get_rest_exchange_class(exchange_manager.exchange_name,
+                                                            exchange_manager.tentacles_setup_config)
+    if rest_exchange_class:
+        exchange_manager.exchange = rest_exchange_class(config=exchange_manager.config,
+                                                        exchange_manager=exchange_manager)
+
+
+def _initialize_simulator_time_frames(exchange_manager):
+    """
+    Initialize simulator client time frames
+    :param exchange_manager: the related exchange manager
+    """
+    exchange_manager.client_time_frames = exchange_manager.exchange.get_available_time_frames()
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/channel/ticker_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/ticker_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/ticker_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchange_data/ticker/ticker_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchange_data/ticker/ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/__init__.pxd`

 * *Files 16% similar despite different names*

```diff
@@ -42,116 +42,89 @@
 from octobot_trading.exchanges.basic_exchange_wrapper cimport (
     BasicExchangeWrapper,
 )
 
 from octobot_trading.exchanges.exchange_manager cimport (
     ExchangeManager,
 )
-from octobot_trading.exchanges.util.exchange_util cimport (
-    get_margin_exchange_class,
-    get_future_exchange_class,
-    get_spot_exchange_class,
-    get_order_side,
-)
 from octobot_trading.exchanges.util cimport (
     ExchangeMarketStatusFixer,
     is_ms_valid,
     force_disable_web_socket,
     check_web_socket_config,
     search_websocket_class,
 )
 from octobot_trading.exchanges.types cimport (
-    FutureExchange,
     WebSocketExchange,
-    MarginExchange,
-    SpotExchange,
+    RestExchange,
 )
 from octobot_trading.exchanges.util cimport (
     ExchangeMarketStatusFixer,
     is_ms_valid,
-    get_margin_exchange_class,
-    get_future_exchange_class,
-    get_spot_exchange_class,
+    get_rest_exchange_class,
     get_order_side,
     force_disable_web_socket,
     check_web_socket_config,
     search_websocket_class,
     get_exchange_type,
     get_default_exchange_type,
     get_supported_exchange_types,
     get_exchange_class_from_name,
 )
 
 from octobot_trading.exchanges cimport implementations
 from octobot_trading.exchanges.implementations cimport (
-    SpotExchangeSimulator,
-    SpotCCXTExchange,
-    FutureExchangeSimulator,
-    FutureCCXTExchange,
-    MarginExchangeSimulator,
-    MarginCCXTExchange,
-    CCXTWebSocketExchange,
-    CryptofeedWebSocketExchange,
+    DefaultWebSocketExchange,
+    DefaultRestExchange,
+    ExchangeSimulator,
 )
 
 from octobot_trading.exchanges.exchange_builder cimport (
     ExchangeBuilder,
 )
 
 from octobot_trading.exchanges cimport connectors
 from octobot_trading.exchanges.connectors cimport (
-    ExchangeSimulator,
-    CCXTExchange,
     CCXTWebsocketConnector,
-    AbstractWebsocketConnector,
-    CryptofeedWebsocketConnector,
+    CCXTConnector,
+    ExchangeSimulatorConnector,
 )
 
 from octobot_trading.exchanges cimport abstract_websocket_exchange
 from octobot_trading.exchanges.abstract_websocket_exchange cimport (
     AbstractWebsocketExchange,
 )
 
 __all__ = [
     "requires_refresh_trigger",
     "ExchangeConfig",
     "ExchangeManager",
     "ExchangeBuilder",
     "ExchangeConfiguration",
     "Exchanges",
-    "get_margin_exchange_class",
-    "get_future_exchange_class",
-    "get_spot_exchange_class",
+    "get_rest_exchange_class",
     "get_order_side",
     "AbstractExchange",
     "TraderSimulator",
     "Trader",
     "ExchangeSimulator",
-    "CCXTExchange",
-    "AbstractWebsocketConnector",
     "CCXTWebsocketConnector",
+    "CCXTConnector",
+    "ExchangeSimulatorConnector",
     "AbstractWebsocketExchange",
     "BasicExchangeWrapper",
-    "FutureExchange",
-    "MarginExchange",
-    "SpotExchange",
+    "RestExchange",
     "WebSocketExchange",
     "ExchangeMarketStatusFixer",
     "is_ms_valid",
     "AbstractWebsocketExchange",
     "force_disable_web_socket",
     "check_web_socket_config",
     "search_websocket_class",
     "get_exchange_type",
     "get_default_exchange_type",
     "get_supported_exchange_types",
     "get_exchange_class_from_name",
-    "SpotExchangeSimulator",
-    "SpotCCXTExchange",
-    "FutureExchangeSimulator",
-    "FutureCCXTExchange",
-    "MarginExchangeSimulator",
-    "MarginCCXTExchange",
-    "CCXTWebSocketExchange",
-    "CryptofeedWebSocketExchange",
-    "CryptofeedWebsocketConnector",
+    "DefaultWebSocketExchange",
+    "DefaultRestExchange",
+    "ExchangeSimulator",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+from octobot_trading.exchanges import adapters
+from octobot_trading.exchanges.adapters import (
+    AbstractAdapter,
+)
 from octobot_trading.exchanges import exchanges
 from octobot_trading.exchanges.exchanges import (
     ExchangeConfiguration,
     Exchanges,
 )
 from octobot_trading.exchanges import exchange_channels
 from octobot_trading.exchanges.exchange_channels import (
@@ -54,17 +58,15 @@
     initialize_real_exchange,
     create_simulated_exchange,
     init_simulated_exchange,
 )
 from octobot_trading.exchanges.util import (
     ExchangeMarketStatusFixer,
     is_ms_valid,
-    get_margin_exchange_class,
-    get_future_exchange_class,
-    get_spot_exchange_class,
+    get_rest_exchange_class,
     get_order_side,
     log_time_sync_error,
     get_partners_explanation_message,
     is_compatible_account,
     get_historical_ohlcv,
     get_exchange_type,
     get_default_exchange_type,
@@ -89,61 +91,52 @@
 from octobot_trading.exchanges import traders
 from octobot_trading.exchanges.traders import (
     Trader,
     TraderSimulator,
 )
 from octobot_trading.exchanges import types
 from octobot_trading.exchanges.types import (
-    FutureExchange,
     WebSocketExchange,
-    MarginExchange,
-    SpotExchange,
+    RestExchange,
 )
 from octobot_trading.exchanges import implementations
 from octobot_trading.exchanges.implementations import (
-    CCXTWebSocketExchange,
-    DefaultCCXTSpotExchange,
-    SpotExchangeSimulator,
-    SpotCCXTExchange,
-    FutureExchangeSimulator,
-    FutureCCXTExchange,
-    MarginExchangeSimulator,
-    MarginCCXTExchange,
-    CryptofeedWebSocketExchange,
+    DefaultWebSocketExchange,
+    ExchangeSimulator,
+    DefaultRestExchange,
 )
 from octobot_trading.exchanges import exchange_builder
 from octobot_trading.exchanges.exchange_builder import (
     ExchangeBuilder,
     create_exchange_builder_instance,
 )
 from octobot_trading.exchanges import connectors
 from octobot_trading.exchanges.connectors import (
-    ExchangeSimulator,
-    CCXTExchange,
     CCXTWebsocketConnector,
-    AbstractWebsocketConnector,
-    CryptofeedWebsocketConnector,
+    CCXTConnector,
+    CCXTAdapter,
+    ExchangeSimulatorConnector,
+    ExchangeSimulatorAdapter,
 )
 
 __all__ = [
+    "AbstractAdapter",
     "ExchangeConfig",
     "BacktestingExchangeConfig",
     "ExchangeManager",
     "ExchangeBuilder",
     "create_exchange_builder_instance",
     "create_exchanges",
     "create_real_exchange",
     "initialize_real_exchange",
     "create_simulated_exchange",
     "init_simulated_exchange",
     "ExchangeConfiguration",
     "Exchanges",
-    "get_margin_exchange_class",
-    "get_future_exchange_class",
-    "get_spot_exchange_class",
+    "get_rest_exchange_class",
     "get_order_side",
     "log_time_sync_error",
     "get_partners_explanation_message",
     "is_compatible_account",
     "get_historical_ohlcv",
     "get_exchange_type",
     "get_default_exchange_type",
@@ -155,35 +148,27 @@
     "search_and_create_websocket",
     "requires_refresh_trigger",
     "create_exchange_channels",
     "create_exchange_producers",
     "create_authenticated_producer_from_parent",
     "TraderSimulator",
     "Trader",
-    "CCXTWebSocketExchange",
-    "DefaultCCXTSpotExchange",
-    "CryptofeedWebSocketExchange",
-    "SpotExchangeSimulator",
-    "SpotCCXTExchange",
-    "FutureExchangeSimulator",
-    "FutureCCXTExchange",
-    "MarginExchangeSimulator",
-    "MarginCCXTExchange",
+    "DefaultWebSocketExchange",
+    "DefaultRestExchange",
     "ExchangeSimulator",
-    "CCXTExchange",
-    "AbstractWebsocketConnector",
     "CCXTWebsocketConnector",
-    "FutureExchange",
-    "MarginExchange",
-    "SpotExchange",
     "WebSocketExchange",
+    "RestExchange",
     "ExchangeMarketStatusFixer",
     "is_ms_valid",
     "AbstractWebsocketExchange",
     "BasicExchangeWrapper",
     "temporary_exchange_wrapper",
-    "CryptofeedWebsocketConnector",
     "force_disable_web_socket",
     "check_web_socket_config",
     "search_websocket_class",
     "supports_websocket",
+    "CCXTConnector",
+    "CCXTAdapter",
+    "ExchangeSimulatorConnector",
+    "ExchangeSimulatorAdapter",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_exchange.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -62,19 +62,14 @@
     cpdef object parse_timestamp(self, dict data_dict, str timestamp_key, object default_value=*, bint ms=*)
     cpdef str parse_currency(self, str currency)
     cpdef str parse_order_id(self, dict order)
     cpdef object parse_status(self, str status)
     cpdef object parse_side(self, str side)
     cpdef object parse_account(self, str account)
 
-    # cleaners
-    cpdef dict clean_recent_trade(self, dict recent_trade)
-    cpdef dict clean_trade(self, dict trade)
-    cpdef dict clean_order(self, dict order)
-
     # uniformization
     cpdef object get_exchange_current_time(self)
     cpdef object uniformize_candles_if_necessary(self, object candle_or_candles)
     cpdef object get_uniformized_timestamp(self, object candle_or_candles)
     cpdef long long get_candle_since_timestamp(self, object time_frame, int count)
 
     cpdef object uniformize_candles_timestamps(self, list candles)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_exchange.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import typing
 import decimal
+import time
 
 import octobot_commons.constants
 import octobot_commons.enums as common_enums
 import octobot_commons.logging as logging
 import octobot_commons.timestamp_util as timestamp_util
 import octobot_commons.configuration as configuration
 
 import octobot_tentacles_manager.api as octobot_tentacles_manager_api
 
 import octobot_trading.constants
 import octobot_trading.enums as enums
 import octobot_trading.util as util
+import octobot_trading.errors as errors
 
 
 class AbstractExchange(util.Initializable):
     UI: configuration.UserInputFactory = configuration.UserInputFactory(
         common_enums.UserInputTentacleTypes.EXCHANGE
     )
     BUY_STR = enums.TradeOrderSide.BUY.value
@@ -410,14 +412,29 @@
 
     async def get_sub_account_list(self):
         """
         :return: the exchange sub account list if supported by the exchange
         """
         raise NotImplementedError("get_sub_account_list is not available on this exchange")
 
+    async def retry_till_success(self, timeout, request_func, *args, **kwargs):
+        t0 = time.time()
+        attempt = 1
+        while time.time() - t0 < timeout:
+            try:
+                result = await request_func(*args, **kwargs)
+                if attempt > 1:
+                    self.logger.debug(f"Request retrier success for {request_func.__name__} after {attempt} attempts")
+                return result
+            except errors.FailedRequest:
+                self.logger.debug(f"Request retrier failed for {request_func.__name__} (attempt {attempt})")
+                attempt += 1
+        raise errors.FailedRequest(f"Failed to successfully run request {request_func.__name__} after {attempt} "
+                                   f"attempts.")
+
     """
     Parsers
     """
 
     def parse_balance(self, balance):
         """
         :param balance: the balance dict
@@ -517,42 +534,14 @@
         """
         :param account: the raw account
         :return: the AccountTypes related to the account
         """
         raise NotImplementedError("parse_account is not implemented")
 
     """
-    Cleaners
-    """
-
-    def clean_recent_trade(self, recent_trade):
-        """
-        Clean the specified recent trade list
-        :param recent_trade: the recent trade list
-        :return: the cleaned recent trade list
-        """
-        raise NotImplementedError("clean_recent_trade is not implemented")
-
-    def clean_trade(self, trade):
-        """
-        Clean the specified trade dict
-        :param trade: the trade dict
-        :return: the cleaned trade dict
-        """
-        raise NotImplementedError("clean_trade is not implemented")
-
-    def clean_order(self, order):
-        """
-        Clean the specified order dict
-        :param order: the order dict
-        :return: the cleaned order dict
-        """
-        raise NotImplementedError("clean_order is not implemented")
-
-    """
     Uniformization
     """
 
     def need_to_uniformize_timestamp(self, timestamp):
         """
         Return True if the timestamp should be uniformized
         :param timestamp: the timestamp to check
@@ -644,29 +633,32 @@
 
     def handle_token_error(self, error):
         self.logger.error(f"Exchange configuration is invalid : please check your configuration ! "
                           f"({error.__class__.__name__}: {error})")
 
     @classmethod
     def load_user_inputs(cls, tentacles_setup_config, tentacle_config):
+        logger = logging.get_logger(cls.get_name())
         inputs = {}
         try:
             tentacle_config.update(
                 octobot_tentacles_manager_api.get_tentacle_config(
                     tentacles_setup_config, cls
                 )
             )
         except NotImplementedError:
             # get_name not implemented, no tentacle config
             return inputs
         try:
             with cls.UI.local_factory(cls, lambda: tentacle_config):
                 cls.init_user_inputs(inputs)
         except Exception as e:
-            logging.get_logger(cls.get_name()).exception(e, True, f"Error when initializing user inputs: {e}")
+            logger.exception(e, True, f"Error when initializing user inputs: {e}")
+        if tentacle_config:
+            logger.debug(f"Using config: {tentacle_config}")
         return inputs
 
     @classmethod
     async def get_raw_config_and_user_inputs(
             cls, _, tentacles_setup_config, __
     ):
         # use user inputs from init_user_inputs
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_websocket_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_websocket_exchange.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -41,11 +41,11 @@
     cpdef void add_pairs(self, list pairs, bint watching_only=*)
     cpdef void initialize(self, list currencies=*, list pairs=*, list time_frames=*, list channels=*)
 
     cpdef bint _should_authenticate(self)
 
     cpdef int get_max_handled_pair_with_time_frame(self)
 
-    cpdef str feed_to_exchange(self, object feed)
+    cpdef object feed_to_exchange(self, object feed)
     cpdef str get_pair_from_exchange(self, str pair)
     cpdef str get_exchange_pair(self, str pair)
     cpdef void clear(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/abstract_websocket_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/abstract_websocket_exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 import octobot_trading.exchange_channel as exchange_channel
 import octobot_trading.exchange_data as exchange_data
 
 
 class AbstractWebsocketExchange:
     __metaclass__ = abc.ABCMeta
 
+    REQUIRED_ACTIVATED_TENTACLES = []
     EXCHANGE_FEEDS = {}
 
     INIT_REQUIRING_EXCHANGE_FEEDS = set()
 
     # Used to ignore a feed when at least one of the corresponding feed is supported
     IGNORED_FEED_PAIRS = {}
 
-    def __init__(self,
-                 config: object,
-                 exchange_manager: object):
+    SUPPORTS_LIVE_PAIR_ADDITION = False
+
+    def __init__(self, config, exchange_manager):
         self.config = config
 
         self.exchange_manager = exchange_manager
         self.exchange = self.exchange_manager.exchange
         self.exchange_id = self.exchange_manager.id
 
         self.bot_mainloop = asyncio.get_event_loop()
@@ -84,70 +85,48 @@
     def get_name(cls):
         raise NotImplementedError("get_name not implemented")
 
     @classmethod
     def has_name(cls, name: str) -> bool:
         raise NotImplementedError("has_name not implemented")
 
-    @staticmethod
-    def get_websocket_client(config, exchange_manager):
-        raise NotImplementedError("get_websocket_client not implemented")
-
-    @abc.abstractmethod
-    def is_handling(self, feed_name):
-        raise NotImplementedError("is_handling not implemented")
-
     @abc.abstractmethod
     async def init_websocket(self, time_frames, trader_pairs, tentacles_setup_config):
         raise NotImplementedError("init_websocket not implemented")
 
     @abc.abstractmethod
     async def start_sockets(self):
         raise NotImplementedError("start_sockets not implemented")
 
     @abc.abstractmethod
     async def wait_sockets(self):
         raise NotImplementedError("wait_sockets not implemented")
 
     @abc.abstractmethod
-    async def subscribe(self):
-        raise NotImplementedError("subscribe is not implemented")
+    def update_followed_pairs(self):
+        raise NotImplementedError("updated_followed_pairs not implemented")
 
     @abc.abstractmethod
-    async def close_and_restart_sockets(self, debounce_duration=0):
-        raise NotImplementedError("close_and_restart_sockets not implemented")
+    async def _close_and_restart_sockets(self, debounce_duration=0):
+        raise NotImplementedError("_close_and_restart_sockets not implemented")
 
     @abc.abstractmethod
     async def stop_sockets(self):
+        """
+        Stops the websocket. Can be restarted
+        """
         raise NotImplementedError("stop_sockets not implemented")
 
     @abc.abstractmethod
     async def close_sockets(self):
+        """
+        Closes the websocket. Can't be restarted
+        """
         raise NotImplementedError("close_sockets not implemented")
 
-    @abc.abstractmethod
-    async def do_auth(self):
-        NotImplementedError("do_auth is not implemented")
-
-    @classmethod
-    def is_handling_spot(cls) -> bool:
-        return False
-
-    @classmethod
-    def is_handling_margin(cls) -> bool:
-        return False
-
-    @classmethod
-    def is_handling_future(cls) -> bool:
-        return False
-
-    @classmethod
-    def get_feeds(cls) -> dict:
-        return cls.EXCHANGE_FEEDS
-
     @classmethod
     def get_exchange_feed(cls, feed) -> str:
         return cls.EXCHANGE_FEEDS.get(feed, octobot_trading.enums.WebsocketFeeds.UNSUPPORTED.value)
 
     @classmethod
     def is_feed_requiring_init(cls, feed) -> bool:
         return feed in cls.INIT_REQUIRING_EXCHANGE_FEEDS
@@ -162,26 +141,26 @@
         Checks if a feed should be ignored
         :param feed: the feed (instance of octobot_trading.enums.WebsocketFeeds)
         :return: True when the feed is already covered by another one
         """
         ignored_feed_candidate_list = cls.IGNORED_FEED_PAIRS.get(feed, [])
         if not ignored_feed_candidate_list:
             return False
-        for feed_candidate in list(cls.EXCHANGE_FEEDS.keys()):
+        for feed_candidate, feed_value in cls.EXCHANGE_FEEDS.items():
             if feed_candidate in ignored_feed_candidate_list and \
-                    cls.is_feed_supported(cls.EXCHANGE_FEEDS[feed_candidate]):
+                    cls.is_feed_supported(feed_value):
                 return True
         return False
 
     def feed_to_exchange(self, feed):
         feed_name: str = self.get_exchange_feed(feed)
         if not self.is_feed_supported(feed_name):
             self.logger.error("{} is not supported on {}".format(feed, self.get_name()))
             raise ValueError(f"{feed} is not supported on {self.get_name()}")
-        return feed_name
+        return feed
 
     def get_book_instance(self, symbol):
         try:
             return self.books[symbol]
         except KeyError:
             self.books[symbol] = exchange_data.OrderBookManager()
             return self.books[symbol]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/basic_exchange_wrapper.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/basic_exchange_wrapper.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/basic_exchange_wrapper.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/basic_exchange_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,52 +13,52 @@
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import contextlib
 import ccxt.async_support
 import ccxt
 
-import octobot_trading.enums as enums
 import octobot_trading.constants as constants
+import octobot_trading.exchanges.connectors.ccxt.enums as ccxt_enums
 
 
 class BasicExchangeWrapper:
-    def __init__(self, exchange_class_string: str, exchange_lib: enums.ExchangeWrapperLibs):
+    def __init__(self, exchange_class_string: str, exchange_lib: ccxt_enums.ExchangeWrapperLibs):
         """
         Always call self.stop() when done with an async ccxt exchange wrapper
         :param exchange_class_string: name of the exchange to create
         :param exchange_lib: lib to use to connect to the exchange
         """
         self.exchange_class_string = exchange_class_string
         self.exchange_lib = exchange_lib
         self.exchange = None
 
         self._exchange_factory()
 
     async def get_available_time_frames(self):
-        if self.exchange_lib in (enums.ExchangeWrapperLibs.CCXT, enums.ExchangeWrapperLibs.ASYNC_CCXT):
+        if self.exchange_lib in (ccxt_enums.ExchangeWrapperLibs.CCXT, ccxt_enums.ExchangeWrapperLibs.ASYNC_CCXT):
             return self.exchange.timeframes
 
     async def stop(self):
-        if self.exchange_lib is enums.ExchangeWrapperLibs.ASYNC_CCXT:
+        if self.exchange_lib is ccxt_enums.ExchangeWrapperLibs.ASYNC_CCXT:
             await self.exchange.close()
 
     def _exchange_factory(self):
-        if self.exchange_lib is enums.ExchangeWrapperLibs.ASYNC_CCXT:
+        if self.exchange_lib is ccxt_enums.ExchangeWrapperLibs.ASYNC_CCXT:
             self.exchange = getattr(ccxt.async_support, self.exchange_class_string)()
-        elif self.exchange_lib is enums.ExchangeWrapperLibs.CCXT:
+        elif self.exchange_lib is ccxt_enums.ExchangeWrapperLibs.CCXT:
             self.exchange = getattr(ccxt, self.exchange_class_string)()
         else:
             raise NotImplementedError(
                 f"{self.exchange_lib} exchange lib is not implemented in {self.__class__.__name__}")
         self.exchange.aiohttp_trust_env = constants.ENABLE_EXCHANGE_HTTP_PROXY_FROM_ENV
 
 
 @contextlib.asynccontextmanager
-async def temporary_exchange_wrapper(exchange_class_string: str, exchange_lib: enums.ExchangeWrapperLibs):
+async def temporary_exchange_wrapper(exchange_class_string: str, exchange_lib: ccxt_enums.ExchangeWrapperLibs):
     """
     Automatically call to on exchange wrapper
     :param exchange_class_string: name of the exchange to create
     :param exchange_lib: lib to use to connect to the exchange
     :return:
     """
     wrapper = BasicExchangeWrapper(exchange_class_string, exchange_lib)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/backtesting_exchange_config.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/backtesting_exchange_config.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/backtesting_exchange_config.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/backtesting_exchange_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/exchange_config_data.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/exchange_config_data.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/config/exchange_config_data.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/config/exchange_config_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,19 +140,20 @@
         ]
         try:
             if new_valid_symbols:
                 self.watched_pairs += new_valid_symbols
                 self._logger.debug(f"Adding watched symbols: {new_valid_symbols}")
                 if self.exchange_manager.has_websocket:
                     self.exchange_manager.exchange_web_socket.add_pairs(new_valid_symbols, watching_only=True)
-                    await self.exchange_manager.exchange_web_socket.close_and_restart_sockets(debounce_duration=1)
+                    await self.exchange_manager.exchange_web_socket.handle_new_pairs(debounce_duration=1)
 
                 await exchange_channel.get_chan(trading_constants.TICKER_CHANNEL,
                                                 self.exchange_manager.id).modify(added_pairs=new_valid_symbols)
         except Exception as e:
+            self._logger.exception(e, True, f"Failed to add new watched symbols {symbols} : {e}")
             self._logger.error(f"Failed to add new watched symbols {symbols} : {e}")
 
     def _set_config_traded_pairs(self):
         self.traded_cryptocurrencies = {}
         traded_symbol_pairs_set = set()
         existing_pairs = set()
         for cryptocurrency in self.config[constants.CONFIG_CRYPTO_CURRENCIES]:
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,35 +10,27 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_trading.exchanges.connectors cimport exchange_simulator
-from octobot_trading.exchanges.connectors.exchange_simulator cimport (
-    ExchangeSimulator,
-)
-from octobot_trading.exchanges.connectors cimport ccxt_exchange
-from octobot_trading.exchanges.connectors.ccxt_exchange cimport (
-    CCXTExchange,
-)
-from octobot_trading.exchanges.connectors cimport abstract_websocket_connector
-from octobot_trading.exchanges.connectors.abstract_websocket_connector cimport (
-    AbstractWebsocketConnector,
-)
-from octobot_trading.exchanges.connectors cimport ccxt_websocket_connector
-from octobot_trading.exchanges.connectors.ccxt_websocket_connector cimport (
+from octobot_trading.exchanges.connectors import ccxt
+from octobot_trading.exchanges.connectors.ccxt import (
+    CCXTAdapter,
+    CCXTConnector,
     CCXTWebsocketConnector,
 )
-from octobot_trading.exchanges.connectors cimport cryptofeed_websocket_connector
-from octobot_trading.exchanges.connectors.cryptofeed_websocket_connector cimport (
-    CryptofeedWebsocketConnector,
+
+from octobot_trading.exchanges.connectors import simulator
+from octobot_trading.exchanges.connectors.simulator import (
+    ExchangeSimulatorAdapter,
+    ExchangeSimulatorConnector,
 )
 
 __all__ = [
-    "ExchangeSimulator",
-    "CCXTExchange",
-    "AbstractWebsocketConnector",
+    "CCXTAdapter",
+    "CCXTConnector",
     "CCXTWebsocketConnector",
-    "CryptofeedWebsocketConnector",
+    "ExchangeSimulatorAdapter",
+    "ExchangeSimulatorConnector",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,35 +10,26 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_trading.exchanges.connectors import exchange_simulator
-from octobot_trading.exchanges.connectors.exchange_simulator import (
-    ExchangeSimulator,
+from octobot_trading.exchanges.connectors.ccxt import ccxt_adapter
+from octobot_trading.exchanges.connectors.ccxt.ccxt_adapter import (
+    CCXTAdapter,
 )
-from octobot_trading.exchanges.connectors import ccxt_exchange
-from octobot_trading.exchanges.connectors.ccxt_exchange import (
-    CCXTExchange,
+from octobot_trading.exchanges.connectors.ccxt import ccxt_connector
+from octobot_trading.exchanges.connectors.ccxt.ccxt_connector import (
+    CCXTConnector,
 )
-from octobot_trading.exchanges.connectors import abstract_websocket_connector
-from octobot_trading.exchanges.connectors.abstract_websocket_connector import (
-    AbstractWebsocketConnector,
-)
-from octobot_trading.exchanges.connectors import ccxt_websocket_connector
-from octobot_trading.exchanges.connectors.ccxt_websocket_connector import (
+
+from octobot_trading.exchanges.connectors.ccxt import ccxt_websocket_connector
+from octobot_trading.exchanges.connectors.ccxt.ccxt_websocket_connector import (
     CCXTWebsocketConnector,
 )
-from octobot_trading.exchanges.connectors import cryptofeed_websocket_connector
-from octobot_trading.exchanges.connectors.cryptofeed_websocket_connector import (
-    CryptofeedWebsocketConnector,
-)
 
 __all__ = [
-    "ExchangeSimulator",
-    "CCXTExchange",
-    "AbstractWebsocketConnector",
+    "CCXTAdapter",
+    "CCXTConnector",
     "CCXTWebsocketConnector",
-    "CryptofeedWebsocketConnector",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/abstract_websocket_connector.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/limit_order.pxd`

 * *Files 20% similar despite different names*

```diff
@@ -6,35 +6,26 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchanges.abstract_websocket_exchange as abstract_websocket
+cimport octobot_trading.personal_data.orders.order as order_class
 
-cdef class AbstractWebsocketConnector(abstract_websocket.AbstractWebsocketExchange):
-    cdef int timeout
-    cdef int timeout_interval
-    cdef int last_ping_time
+cdef class LimitOrder(order_class.Order):
+    cdef object limit_price_hit_event # object is asyncio.Event
+    cdef object wait_for_hit_event_task # object is asyncio.Task
 
-    cdef bint is_connected
-    cdef bint should_stop
-    cdef bint is_authenticated
-    cdef bint use_testnet
+    cdef bint trigger_above
+    cdef public bint allow_instant_fill
 
-    cdef public dict endpoint_args
-
-    # objects
-    cdef public object websocket
-    cdef object _watch_task
-    cdef object last_msg
-
-    cpdef void on_open(self)
-    cpdef void on_auth(self, bint status)
-    cpdef void on_close(self)
-    cpdef void on_error(self, str error)
-    cpdef void start(self)
+    cpdef str _filled_maker_or_taker(self)
+    # return object to allow exception raising
+    cdef object _create_hit_event(self, object price_time)
+    cdef object _create_hit_task(self)
+    cdef object _reset_events(self, object price_time)
+    cdef object _clear_event_and_tasks(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/ccxt_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.pxd`

 * *Files 10% similar despite different names*

```diff
@@ -12,39 +12,38 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 cimport octobot_trading.exchanges.abstract_exchange as abstract_exchange
 
-cdef class CCXTExchange(abstract_exchange.AbstractExchange):
+cdef class CCXTConnector(abstract_exchange.AbstractExchange):
     cdef object all_currencies_price_ticker
 
     cdef public object client
     cdef public object exchange_type
+    cdef public object adapter
 
     cdef public bint is_authenticated
 
+    cdef object additional_config
     cdef dict options
     cdef dict headers
 
-    cdef object additional_ccxt_config
 
     # private
-    cdef void _create_client(self)
+    cdef object _create_client(self)
 
     # @staticmethod waiting for a future version of cython
     # cdef bint _ensure_order_details_completeness(object order, list order_required_fields=*)
 
+    cpdef object get_adapter_class(self, object adapter_class)
     cpdef void add_headers(self, dict headers_dict)
     cpdef void add_options(self, dict options_dict)
     cpdef set get_client_symbols(self)
     cpdef set get_client_time_frames(self)
-    cpdef dict get_ccxt_client_login_options(self)
     cpdef str get_ccxt_order_type(self, object order_type)
     cpdef void set_sandbox_mode(self, bint is_sandboxed)
     cpdef dict get_bundled_order_parameters(self, object stop_loss_price=*, object take_profit_price=*)
+    cpdef object unauthenticated_exchange_fallback(self, object err)
 
-    cdef void _unauthenticated_exchange_fallback(self, object err)
-    cdef object _get_unauthenticated_exchange(self)
-    cdef object _get_client_config(self, object api_key=*, object secret=*, object password=*)
     cdef bint _should_authenticate(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/ccxt_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/ccxt_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,196 +12,157 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import contextlib
 import decimal
-import logging
 
 import ccxt.async_support as ccxt
 import typing
 
-import octobot_commons.constants
 import octobot_commons.enums
 import octobot_commons.symbols as commons_symbols
 
 import octobot_trading
 import octobot_trading.constants as constants
 import octobot_trading.enums as enums
 import octobot_trading.errors
 import octobot_trading.exchanges as exchanges
 import octobot_trading.exchanges.abstract_exchange as abstract_exchange
+import octobot_trading.exchanges.connectors.ccxt.ccxt_adapter as ccxt_adapter
+import octobot_trading.exchanges.connectors.ccxt.ccxt_client_util as ccxt_client_util
 import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import ExchangeConstantsOrderColumns as ecoc
 
 
-class CCXTExchange(abstract_exchange.AbstractExchange):
+class CCXTConnector(abstract_exchange.AbstractExchange):
     """
-    CCXT library wrapper
+    CCXT library connector. Everything ccxt related should be in this connector.
+    When possible, each call is supposed to create only one request to the exchange.
+    Uses self.adapter to parse (and fix if necessary) ccxt raw data.
+
+    Always returns adapted data. Always throws octobot_trading errors
+    Never returns row ccxt data or throw ccxt errors
     """
     CCXT_ISOLATED = "ISOLATED"
     CCXT_CROSSED = "CROSSED"
 
-    def __init__(self, config, exchange_manager, additional_ccxt_config=None):
+    def __init__(self, config, exchange_manager, adapter_class=None, additional_config=None):
         super().__init__(config, exchange_manager)
         self.client = None
         self.exchange_type = None
+        self.adapter = self.get_adapter_class(adapter_class)(self)
         self.all_currencies_price_ticker = None
         self.is_authenticated = False
 
-        self.additional_ccxt_config = additional_ccxt_config
+        self.additional_config = additional_config
         self.headers = {}
         self.options = {}
         # add default options
-        self.add_options(self.get_ccxt_client_login_options())
+        self.add_options(
+            ccxt_client_util.get_ccxt_client_login_options(self.exchange_manager)
+        )
 
         self._create_exchange_type()
         self._create_client()
 
     async def initialize_impl(self):
         try:
             if self.exchange_manager.exchange.is_supporting_sandbox():
                 self.set_sandbox_mode(self.exchange_manager.is_sandboxed)
 
             if self._should_authenticate() and not self.exchange_manager.exchange_only:
                 await self._ensure_auth()
 
             if self.exchange_manager.is_loading_markets:
                 with self.error_describer():
-                    await self.client.load_markets()
+                    await self.load_symbol_markets()
 
             # initialize symbols and timeframes
             self.symbols = self.get_client_symbols()
             self.time_frames = self.get_client_time_frames()
 
         except (ccxt.ExchangeNotAvailable, ccxt.RequestTimeout) as e:
             raise octobot_trading.errors.UnreachableExchange() from e
         except ccxt.AuthenticationError:
             raise ccxt.AuthenticationError
 
+    def get_adapter_class(self, adapter_class):
+        return adapter_class or ccxt_adapter.CCXTAdapter
+
+    @classmethod
+    def load_user_inputs(cls, tentacles_setup_config, tentacle_config):
+        # no user input in connector
+        pass
+
+    async def load_symbol_markets(self, reload=False):
+        await self.client.load_markets(reload=reload)
+
     def get_client_symbols(self):
-        return set(self.client.symbols) \
-            if hasattr(self.client, "symbols") and self.client.symbols is not None else set()
+        return ccxt_client_util.get_symbols(self.client)
 
     def get_client_time_frames(self):
-        return set(self.client.timeframes) \
-            if hasattr(self.client, "timeframes") and self.client.timeframes is not None else set()
+        return ccxt_client_util.get_time_frames(self.client)
 
     @classmethod
     def is_supporting_exchange(cls, exchange_candidate_name) -> bool:
         return isinstance(exchange_candidate_name, str)
 
     def _create_exchange_type(self):
         if self.is_supporting_exchange(self.exchange_manager.exchange_class_string):
             self.exchange_type = getattr(ccxt, self.exchange_manager.exchange_class_string)
         else:
             self.exchange_type = self.exchange_manager.exchange_class_string
 
-    def get_ccxt_client_login_options(self):
-        """
-        :return: ccxt client login option dict, can be overwritten to custom exchange login
-        """
-        if self.exchange_manager.is_future:
-            return {'defaultType': 'future'}
-        if self.exchange_manager.is_margin:
-            return {'defaultType': 'margin'}
-        return {'defaultType': 'spot'}
-
     def add_headers(self, headers_dict):
         """
         Add new headers to ccxt client
         :param headers_dict: the additional header keys and values as dict
         """
-        for header_key, header_value in headers_dict.items():
-            self.headers[header_key] = header_value
-            if self.client is not None:
-                self.client.headers[header_key] = header_value
+        self.headers.update(headers_dict)
+        if self.client is not None:
+            ccxt_client_util.add_headers(self.client, headers_dict)
 
     def add_options(self, options_dict):
         """
         Add new options to ccxt client
         :param options_dict: the additional option keys and values as dict
         """
-        for option_key, option_value in options_dict.items():
-            self.options[option_key] = option_value
-            if self.client is not None:
-                self.client.options[option_key] = option_value
+        self.options.update(options_dict)
+        if self.client is not None:
+            ccxt_client_util.add_options(self.client, options_dict)
 
     async def _ensure_auth(self):
         try:
             await self.get_balance()
         except ccxt.AuthenticationError as e:
             await self.client.close()
-            self._unauthenticated_exchange_fallback(e)
+            self.unauthenticated_exchange_fallback(e)
         except Exception as e:
             # Is probably handled in exchange tentacles, important thing here is that authentication worked
             self.logger.debug(f"Error when checking exchange connection: {e}. This should not be an issue.")
 
     def _create_client(self):
-        """
-        Exchange instance creation
-        :return:
-        """
-        if not self.exchange_manager.exchange_only:
-            # avoid logging version on temporary exchange_only exchanges
-            self.logger.info(f"Creating {self.exchange_type.__name__} exchange with ccxt in version {ccxt.__version__}")
-        if self.exchange_manager.ignore_config or self.exchange_manager.check_config(self.name):
-            try:
-                key, secret, password = self.exchange_manager.get_exchange_credentials(self.logger, self.name)
-                if not(key and secret) and not self.exchange_manager.is_simulated:
-                    self.logger.warning(f"No exchange API key set for {self.exchange_manager.exchange_name}. "
-                                        f"Enter your account details to enable real trading on this exchange.")
-                if self._should_authenticate():
-                    self.client = self.exchange_type(self._get_client_config(key, secret, password))
-                    self.is_authenticated = True
-                    if self.exchange_manager.check_credentials:
-                        self.client.checkRequiredCredentials()
-                else:
-                    self.client = self.exchange_type(self._get_client_config())
-            except (ccxt.AuthenticationError, Exception) as e:
-                self._unauthenticated_exchange_fallback(e)
-        else:
-            self.client = self._get_unauthenticated_exchange()
-            self.logger.error("configuration issue: missing login information !")
-        self.client.logger.setLevel(logging.INFO)
-        self.use_http_proxy_if_necessary()
-
-    def use_http_proxy_if_necessary(self):
-        self.client.aiohttp_trust_env = constants.ENABLE_EXCHANGE_HTTP_PROXY_FROM_ENV
+        self.client, self.is_authenticated = ccxt_client_util.create_client(
+            self.exchange_type, self.name, self.exchange_manager, self.logger,
+            self.options, self.headers, self.additional_config,
+            self._should_authenticate(), self.unauthenticated_exchange_fallback
+        )
 
     def _should_authenticate(self):
         return not (self.exchange_manager.is_simulated or
                     self.exchange_manager.is_backtesting)
 
-    def _unauthenticated_exchange_fallback(self, err):
-        self.is_authenticated = False
+    def unauthenticated_exchange_fallback(self, err):
         self.handle_token_error(err)
-        self.client = self._get_unauthenticated_exchange()
-
-    def _get_unauthenticated_exchange(self):
-        return self.exchange_type(self._get_client_config())
-
-    def _get_client_config(self, api_key=None, secret=None, password=None):
-        config = {
-            'verbose': constants.ENABLE_CCXT_VERBOSE,
-            'enableRateLimit': constants.ENABLE_CCXT_RATE_LIMIT,
-            'timeout': constants.DEFAULT_REQUEST_TIMEOUT,
-            'options': self.options,
-            'headers': self.headers
-        }
-        if api_key is not None:
-            config['apiKey'] = api_key
-        if secret is not None:
-            config['secret'] = secret
-        if password is not None:
-            config['password'] = password
-        # apply self.additional_ccxt_config
-        config.update(self.additional_ccxt_config or {})
-        return config
+        return ccxt_client_util.get_unauthenticated_exchange(
+            self.exchange_type,
+            self.options, self.headers, self.additional_config
+        )
 
     def get_market_status(self, symbol, price_example=None, with_fixer=True):
         try:
             if with_fixer:
                 return exchanges.ExchangeMarketStatusFixer(self.client.market(symbol), price_example).market_status
             return self.client.market(symbol)
         except ccxt.NotSupported:
@@ -215,24 +176,17 @@
         fetch balance (free + used) by currency
         :return: balance dict
         """
         if not kwargs:
             kwargs = {}
         try:
             with self.error_describer():
-                balance = await self.client.fetch_balance(params=kwargs)
-
-                # remove not currency specific keys
-                balance.pop(constants.CONFIG_PORTFOLIO_FREE, None)
-                balance.pop(constants.CONFIG_PORTFOLIO_USED, None)
-                balance.pop(constants.CONFIG_PORTFOLIO_TOTAL, None)
-                balance.pop(constants.CCXT_INFO, None)
-                balance.pop(enums.ExchangeConstantsCCXTColumns.DATETIME.value, None)
-                balance.pop(enums.ExchangeConstantsCCXTColumns.TIMESTAMP.value, None)
-                return personal_data.parse_decimal_portfolio(balance)
+                return self.adapter.adapt_balance(
+                    await self.client.fetch_balance(params=kwargs)
+                )
 
         except ccxt.InvalidNonce as err:
             exchanges.log_time_sync_error(self.logger, self.name, err, "real trader portfolio")
             raise err
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
 
@@ -240,83 +194,93 @@
                                 symbol: str,
                                 time_frame: octobot_commons.enums.TimeFrames,
                                 limit: int = None,
                                 since: int = None,
                                 **kwargs: dict) -> typing.Optional[list]:
         try:
             with self.error_describer():
-                if limit:
-                    return await self.client.fetch_ohlcv(symbol, time_frame.value, limit=limit,
-                                                         since=since, params=kwargs)
-                return await self.client.fetch_ohlcv(symbol, time_frame.value, since=since, params=kwargs)
+                return self.adapter.adapt_ohlcv(
+                    await self.client.fetch_ohlcv(symbol, time_frame.value, limit=limit, since=since, params=kwargs)
+                )
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
         except ccxt.BaseError as e:
             raise octobot_trading.errors.FailedRequest(f"Failed to get_symbol_prices: {e.__class__.__name__} on {e}")
 
     async def get_kline_price(self,
                               symbol: str,
                               time_frame: octobot_commons.enums.TimeFrames,
                               **kwargs: dict) -> typing.Optional[list]:
         try:
             # default implementation
+            # already adapted in get_symbol_prices
             return await self.get_symbol_prices(symbol, time_frame, limit=1, **kwargs)
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
         except ccxt.BaseError as e:
             raise octobot_trading.errors.FailedRequest(f"Failed to get_kline_price {e}")
 
     # return up to ten bidasks on each side of the order book stack
     async def get_order_book(self, symbol: str, limit: int = 5, **kwargs: dict) -> typing.Optional[dict]:
         try:
             with self.error_describer():
-                return await self.client.fetch_order_book(symbol, limit=limit, params=kwargs)
+                return self.adapter.adapt_order_book(
+                    await self.client.fetch_order_book(symbol, limit=limit, params=kwargs)
+                )
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
         except ccxt.BaseError as e:
             raise octobot_trading.errors.FailedRequest(f"Failed to get_order_book {e}")
 
     async def get_recent_trades(self, symbol: str, limit: int = 50, **kwargs: dict) -> typing.Optional[list]:
         try:
             with self.error_describer():
-                return await self.client.fetch_trades(symbol, limit=limit, params=kwargs)
+                return self.adapter.adapt_public_recent_trades(
+                    await self.client.fetch_trades(symbol, limit=limit, params=kwargs)
+                )
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
         except ccxt.BaseError as e:
             raise octobot_trading.errors.FailedRequest(f"Failed to get_recent_trades {e}")
 
     # A price ticker contains statistics for a particular market/symbol for some period of time in recent past (24h)
     async def get_price_ticker(self, symbol: str, **kwargs: dict) -> typing.Optional[dict]:
         try:
             with self.error_describer():
-                return await self.client.fetch_ticker(symbol, params=kwargs)
+                return self.adapter.adapt_ticker(
+                    await self.client.fetch_ticker(symbol, params=kwargs)
+                )
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
         except ccxt.BaseError as e:
             raise octobot_trading.errors.FailedRequest(f"Failed to get_price_ticker {e}")
 
     async def get_all_currencies_price_ticker(self, **kwargs: dict) -> typing.Optional[list]:
         try:
             with self.error_describer():
                 symbols = kwargs.pop("symbols", None)
-                self.all_currencies_price_ticker = await self.client.fetch_tickers(symbols, params=kwargs)
+                self.all_currencies_price_ticker = {
+                    symbol: self.adapter.adapt_ticker(ticker)
+                    for symbol, ticker in (await self.client.fetch_tickers(symbols, params=kwargs)).items()
+                }
             return self.all_currencies_price_ticker
         except ccxt.NotSupported:
             raise octobot_trading.errors.NotSupported
         except ccxt.BaseError as e:
             raise octobot_trading.errors.FailedRequest(f"Failed to get_all_currencies_price_ticker {e}")
 
     # ORDERS
     async def get_order(self, order_id: str, symbol: str = None, **kwargs: dict) -> dict:
         if self.client.has['fetchOrder']:
             try:
                 with self.error_describer():
                     params = kwargs.pop("params", {})
-                    return await self.client.fetch_order(order_id, symbol, params=params, **kwargs)
-                # self.exchange_manager.exchange_personal_data.upsert_order(order_id, updated_order) TODO
+                    return self.adapter.adapt_order(
+                        await self.client.fetch_order(order_id, symbol, params=params, **kwargs)
+                    )
             except ccxt.OrderNotFound:
                 # some exchanges are throwing this error when an order is cancelled (ex: coinbase pro)
                 pass
             except ccxt.NotSupported as e:
                 # some exchanges are throwing this error when an order is cancelled (ex: coinbase pro)
                 raise octobot_trading.errors.NotSupported from e
         else:
@@ -327,53 +291,113 @@
                     return order
         return None  # OrderNotFound
 
     async def get_all_orders(self, symbol: str = None, since: int = None,
                              limit: int = None, **kwargs: dict) -> list:
         if self.client.has['fetchOrders']:
             with self.error_describer():
-                return await self.client.fetch_orders(symbol=symbol, since=since, limit=limit, params=kwargs)
+                return [
+                    self.adapter.adapt_order(order)
+                    for order in await self.client.fetch_orders(symbol=symbol, since=since, limit=limit, params=kwargs)
+                ]
         else:
             raise octobot_trading.errors.NotSupported("This exchange doesn't support fetchOrders")
 
     async def get_open_orders(self, symbol: str = None, since: int = None,
                               limit: int = None, **kwargs: dict) -> list:
         if self.client.has['fetchOpenOrders']:
             with self.error_describer():
-                return await self.client.fetch_open_orders(symbol=symbol, since=since, limit=limit, params=kwargs)
+                return [
+                    self.adapter.adapt_order(order)
+                    for order in await self.client.fetch_open_orders(symbol=symbol, since=since,
+                                                                     limit=limit, params=kwargs)
+                ]
         else:
             raise octobot_trading.errors.NotSupported("This exchange doesn't support fetchOpenOrders")
 
     async def get_closed_orders(self, symbol: str = None, since: int = None,
                                 limit: int = None, **kwargs: dict) -> list:
         if self.client.has['fetchClosedOrders']:
             with self.error_describer():
-                return await self.client.fetch_closed_orders(symbol=symbol, since=since, limit=limit, params=kwargs)
+                return [
+                    self.adapter.adapt_order(order)
+                    for order in await self.client.fetch_closed_orders(symbol=symbol, since=since,
+                                                                       limit=limit, params=kwargs)
+                ]
         else:
             raise octobot_trading.errors.NotSupported("This exchange doesn't support fetchClosedOrders")
 
     async def get_my_recent_trades(self, symbol: str = None, since: int = None,
                                    limit: int = None, **kwargs: dict) -> list:
         if self.client.has['fetchMyTrades'] or self.client.has['fetchTrades']:
             with self.error_describer():
-                if self.client.has['fetchMyTrades']:
-                    return await self.client.fetch_my_trades(symbol=symbol, since=since, limit=limit, params=kwargs)
-                elif self.client.has['fetchTrades']:
-                    return await self.client.fetch_trades(symbol=symbol, since=since, limit=limit, params=kwargs)
+                method = self.client.fetch_my_trades if self.client.has['fetchMyTrades'] else self.client.fetch_trades
+                return self.adapter.adapt_trades(await method(symbol=symbol, since=since, limit=limit, params=kwargs))
         else:
             raise octobot_trading.errors.NotSupported("This exchange doesn't support fetchMyTrades nor fetchTrades")
 
+    async def create_market_buy_order(self, symbol, quantity, price=None, params=None) -> dict:
+        return self.adapter.adapt_order(
+            await self.client.create_market_buy_order(symbol, quantity, params=params)
+        )
+
+    async def create_limit_buy_order(self, symbol, quantity, price=None, params=None) -> dict:
+        return self.adapter.adapt_order(
+            await self.client.create_limit_buy_order(symbol, quantity, price, params=params)
+        )
+
+    async def create_market_sell_order(self, symbol, quantity, price=None, params=None) -> dict:
+        return self.adapter.adapt_order(
+            await self.client.create_market_sell_order(symbol, quantity, params=params)
+        )
+
+    async def create_limit_sell_order(self, symbol, quantity, price=None, params=None) -> dict:
+        return self.adapter.adapt_order(
+            await self.client.create_limit_sell_order(symbol, quantity, price, params=params)
+        )
+
+    async def create_market_stop_loss_order(self, symbol, quantity, price, side, current_price, params=None) -> dict:
+        raise NotImplementedError("create_market_stop_loss_order is not implemented")
+
+    async def create_limit_stop_loss_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
+        raise NotImplementedError("create_limit_stop_loss_order is not implemented")
+
+    async def create_market_take_profit_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
+        raise NotImplementedError("create_market_take_profit_order is not implemented")
+
+    async def create_limit_take_profit_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
+        raise NotImplementedError("create_limit_take_profit_order is not implemented")
+
+    async def create_market_trailing_stop_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
+        raise NotImplementedError("create_market_trailing_stop_order is not implemented")
+
+    async def create_limit_trailing_stop_order(self, symbol, quantity, price=None, side=None, params=None) -> dict:
+        raise NotImplementedError("create_limit_trailing_stop_order is not implemented")
+
+    async def edit_order(self, order_id: str, order_type: enums.TraderOrderType, symbol: str,
+                         quantity: float, price: float, stop_price: float = None, side: str = None,
+                         current_price: float = None, params: dict = None):
+        ccxt_order_type = self.get_ccxt_order_type(order_type)
+        price_to_use = price
+        if ccxt_order_type == enums.TradeOrderType.MARKET.value:
+            # can't set price in market orders
+            price_to_use = None
+        # do not use keyword arguments here as default ccxt edit order is passing *args (and not **kwargs)
+        return self.adapter.adapt_order(
+            await self.client.edit_order(order_id, symbol, ccxt_order_type, side, quantity, price_to_use, params)
+        )
+
     async def cancel_order(self, order_id: str, symbol: str = None, **kwargs: dict) -> enums.OrderStatus:
         try:
             with self.error_describer():
                 await self.client.cancel_order(order_id, symbol=symbol, params=kwargs)
                 # no exception, cancel worked
             try:
                 # make sure order is canceled
-                cancelled_order = await self.exchange_manager.exchange.get_order(
+                cancelled_order = await self.get_order(
                     order_id, symbol=symbol
                 )
                 if cancelled_order is None or personal_data.parse_is_cancelled(cancelled_order):
                     return enums.OrderStatus.CANCELED
                 elif personal_data.parse_is_open(cancelled_order):
                     return enums.OrderStatus.PENDING_CANCEL
                 # cancel command worked but order is still existing and is not open or canceled. unhandled case
@@ -392,24 +416,33 @@
             raise octobot_trading.errors.NotSupported from e
         except Exception as e:
             self.logger.exception(e, True, f"Unexpected error when cancelling order with id: "
                                            f"{order_id} failed to cancel | {e} ({e.__class__.__name__})")
             raise e
 
     async def get_positions(self, symbols=None, **kwargs: dict) -> list:
-        return await self.client.fetch_positions(symbols=symbols, params=kwargs)
+        return [
+            self.adapter.adapt_position(position)
+            for position in await self.client.fetch_positions(symbols=symbols, params=kwargs)
+        ]
 
     async def get_position(self, symbol: str, **kwargs: dict) -> dict:
-        return await self.client.fetch_position(symbol=symbol, params=kwargs)
+        return self.adapter.adapt_position(
+            await self.client.fetch_position(symbol=symbol, params=kwargs)
+        )
 
     async def get_funding_rate(self, symbol: str, **kwargs: dict) -> dict:
-        return await self.client.fetch_funding_rate(symbol=symbol, params=kwargs)
+        return self.adapter.adapt_funding_rate(
+            await self.client.fetch_funding_rate(symbol=symbol, params=kwargs)
+        )
 
     async def get_funding_rate_history(self, symbol: str, limit: int = 1, **kwargs: dict) -> list:
-        return await self.client.fetch_funding_rate_history(symbol=symbol, limit=limit, params=kwargs)
+        return self.adapter.adapt_funding_rate(
+            await self.client.fetch_funding_rate_history(symbol=symbol, limit=limit, params=kwargs)
+        )
 
     async def set_symbol_leverage(self, symbol: str, leverage: int, **kwargs: dict):
         return await self.client.set_leverage(leverage=int(leverage), symbol=symbol, params=kwargs)
 
     async def set_symbol_margin_type(self, symbol: str, isolated: bool):
         return await self.client.set_margin_mode(symbol=symbol,
                                                  marginType=self.CCXT_ISOLATED if isolated else self.CCXT_CROSSED)
@@ -478,20 +511,20 @@
             self.logger.error(f"Fees data for {symbol} was not found ({e})")
             return {
                 enums.ExchangeConstantsMarketPropertyColumns.TAKER.value: constants.CONFIG_DEFAULT_FEES,
                 enums.ExchangeConstantsMarketPropertyColumns.MAKER.value: constants.CONFIG_DEFAULT_FEES,
                 enums.ExchangeConstantsMarketPropertyColumns.FEE.value: constants.CONFIG_DEFAULT_FEES
             }
 
-    def get_uniform_timestamp(self, timestamp):
-        return timestamp / octobot_commons.constants.MSECONDS_TO_SECONDS
-
     def get_exchange_current_time(self):
         return self.get_uniform_timestamp(self.client.milliseconds())
 
+    def get_uniform_timestamp(self, timestamp):
+        return self.adapter.get_uniformized_timestamp(timestamp)
+
     async def stop(self) -> None:
         self.logger.info(f"Closing connection.")
         await self.client.close()
         self.logger.info(f"Connection closed.")
         self.exchange_manager = None
 
     def get_pair_from_exchange(self, pair) -> typing.Optional[str]:
@@ -512,47 +545,55 @@
             try:
                 return self.client.markets_by_id[pair]["base"], self.client.markets_by_id[pair]["quote"]
             except KeyError:
                 self.logger.error(f"Failed to get market of {pair}")
                 return None, None
 
     def get_exchange_pair(self, pair) -> str:
-        if pair in self.client.symbols:
-            try:
-                return self.client.market(pair)["id"]
-            except KeyError:
-                pass
-        raise ValueError(f'{pair} is not supported')
+        return ccxt_client_util.get_exchange_pair(self.client, pair)
 
     def get_pair_cryptocurrency(self, pair) -> str:
-        if pair in self.client.symbols:
-            try:
-                return self.client.market(pair)["base"]
-            except KeyError:
-                pass
-        raise ValueError(f'{pair} is not supported')
+        return ccxt_client_util.get_pair_cryptocurrency(self.client, pair)
 
     def get_default_balance(self):
         return self.client.account()
 
     def get_rate_limit(self):
         return self.exchange_type.rateLimit / 1000
 
+    def supports_trading_type(self, symbol, trading_type: enums.FutureContractType) -> bool:
+        trading_type_to_ccxt_property = {
+            enums.FutureContractType.LINEAR_PERPETUAL: "linear",
+            enums.FutureContractType.LINEAR_EXPIRABLE: "linear",
+            enums.FutureContractType.INVERSE_PERPETUAL: "inverse",
+            enums.FutureContractType.INVERSE_EXPIRABLE: "inverse",
+        }
+        return self.client.safe_string(
+            self.client.market(symbol),
+            trading_type_to_ccxt_property[trading_type],
+            "False"
+        ) == "True"
+
+    def get_pair_market_type(self, pair, property_name, def_value=False):
+        return self.client.safe_string(
+            self.client.safe_value(self.client.markets, pair, {}), property_name, def_value
+        )
+
     def set_sandbox_mode(self, is_sandboxed):
         try:
-            self.client.setSandboxMode(is_sandboxed)
+            ccxt_client_util.set_sandbox_mode(self.client, is_sandboxed)
         except ccxt.NotSupported as e:
             default_type = self.client.options.get('defaultType', None)
             additional_info = f" in type {default_type}" if default_type else ""
             self.logger.warning(f"{self.name} does not support sandboxing {additional_info}: {e}")
             # raise exception to stop this exchange and prevent dealing with a real funds exchange
             raise e
 
     """
-    Parsers
+    Parsers todo: remove all parsers
     """
 
     def parse_balance(self, balance):
         return self.client.parse_balance(balance)
 
     def parse_trade(self, trade):
         return self.client.parse_trade(trade)
@@ -590,51 +631,19 @@
 
     def parse_side(self, side):
         return enums.TradeOrderSide.BUY if side == self.BUY_STR else enums.TradeOrderSide.SELL
 
     def parse_account(self, account):
         return enums.AccountTypes[account]
 
-    """
-    Cleaners
-    """
+    def parse_funding(self, funding_dict, from_ticker=False) -> dict:
+        return self.adapter.adapt_funding_rate(funding_dict, from_ticker=from_ticker)
 
-    def clean_recent_trade(self, recent_trade):
-        try:
-            recent_trade.pop(ecoc.INFO.value)
-            recent_trade.pop(ecoc.DATETIME.value)
-            recent_trade.pop(ecoc.ID.value)
-            recent_trade.pop(ecoc.ORDER.value)
-            recent_trade.pop(ecoc.FEE.value)
-            recent_trade.pop(ecoc.TYPE.value)
-            recent_trade.pop(ecoc.TAKER_OR_MAKER.value)
-            recent_trade[ecoc.TIMESTAMP.value] = \
-                self.get_uniformized_timestamp(recent_trade[ecoc.TIMESTAMP.value])
-        except KeyError as e:
-            self.logger.error(f"Fail to clean recent_trade dict ({e})")
-        return recent_trade
-
-    def clean_trade(self, trade):
-        try:
-            trade.pop(ecoc.INFO.value)
-            trade[ecoc.TIMESTAMP.value] = \
-                self.get_uniformized_timestamp(trade[ecoc.TIMESTAMP.value])
-        except KeyError as e:
-            self.logger.error(f"Fail to clean trade dict ({e})")
-        return trade
-
-    def clean_order(self, order):
-        try:
-            order.pop(ecoc.INFO.value)
-            exchange_timestamp = order[ecoc.TIMESTAMP.value]
-            order[ecoc.TIMESTAMP.value] = \
-                self.get_uniformized_timestamp(exchange_timestamp)
-        except KeyError as e:
-            self.logger.error(f"Fail to cleanup order dict ({e})")
-        return order
+    def parse_mark_price(self, mark_price_dict, from_ticker=False) -> dict:
+        return self.adapter.adapt_mark_price(mark_price_dict, from_ticker=from_ticker)
 
     def get_max_handled_pair_with_time_frame(self) -> int:
         """
         Override when necessary
         :return: the maximum number of simultaneous pairs * time_frame that this exchange can handle.
         """
         # 15 pairs, each on 3 time frames
@@ -649,7 +658,9 @@
             if self.exchange_manager.exchange.should_log_on_ddos_exception(e):
                 self.logger.error(
                     f"DDoSProtection triggered [{e} ({e.__class__.__name__})]. "
                     f"Last response headers: {self.client.last_response_headers} "
                     f"Last json response: {self.client.last_json_response}"
                 )
             raise
+        except ccxt.RequestTimeout as e:
+            raise octobot_trading.errors.FailedRequest(f"Request timeout: {e}") from e
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/ccxt_websocket_connector.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/__init__.pxd`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchanges.connectors.abstract_websocket_connector as abstract_websocket_connector
 
-cdef class CCXTWebsocketConnector(abstract_websocket_connector.AbstractWebsocketConnector):
-    cdef public object ccxt_client
-    cdef public object async_ccxt_client
+from octobot_trading.exchanges.connectors.ccxt cimport ccxt_connector
+from octobot_trading.exchanges.connectors.ccxt.ccxt_connector cimport (
+    CCXTConnector,
+)
+from octobot_trading.exchanges.connectors.ccxt cimport ccxt_websocket_connector
+from octobot_trading.exchanges.connectors.ccxt.ccxt_websocket_connector cimport (
+    CCXTWebsocketConnector,
+)
+
+__all__ = [
+    "CCXTConnector",
+    "CCXTWebsocketConnector",
+]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/exchange_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.pxd`

 * *Files 15% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 cimport octobot_backtesting.backtesting as backtesting
 cimport octobot_trading.exchanges.abstract_exchange as abstract_exchange
 
-cdef class ExchangeSimulator(abstract_exchange.AbstractExchange):
+cdef class ExchangeSimulatorConnector(abstract_exchange.AbstractExchange):
     cdef public backtesting.Backtesting backtesting
+    cdef public object adapter
 
     cdef public list exchange_importers
 
     cdef public dict current_future_candles
 
     cdef public bint is_authenticated
 
+    cpdef object get_adapter_class(self, object adapter_class)
     cpdef str get_pair_cryptocurrency(self, str pair)
     cpdef list get_available_time_frames(self)
     cpdef list get_backtesting_data_files(self)
     cpdef list get_time_frames(self, object importer)
 
     cdef void _read_fees_from_config(self, dict result_fees)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/connectors/exchange_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,25 @@
 import octobot_commons.time_frame_manager as time_frame_manager
 import octobot_commons.constants as commons_constants
 
 import octobot_trading.exchange_channel as exchange_channel
 import octobot_trading.constants as constants
 import octobot_trading.enums as enums
 import octobot_trading.exchanges.abstract_exchange as abstract_exchange
+import octobot_trading.exchanges.connectors.simulator.exchange_simulator_adapter as exchange_simulator_adapter
 import octobot_trading.exchange_data as exchange_data
 import octobot_trading.exchanges.util as util
 
 
-class ExchangeSimulator(abstract_exchange.AbstractExchange):
-    def __init__(self, config, exchange_manager, backtesting):
+class ExchangeSimulatorConnector(abstract_exchange.AbstractExchange):
+    def __init__(self, config, exchange_manager, backtesting, adapter_class=None):
         super().__init__(config, exchange_manager)
         self.backtesting = backtesting
         self.allowed_time_lag = constants.DEFAULT_BACKTESTING_TIME_LAG
+        self.adapter = self.get_adapter_class(adapter_class)(self)
 
         self.exchange_importers = []
 
         self.current_future_candles = {}
 
         self.is_authenticated = False
 
@@ -55,14 +57,22 @@
             symbol: {}
             for symbol in self.symbols
         }
 
         # set exchange manager attributes
         self.exchange_manager.client_symbols = list(self.symbols)
 
+    def get_adapter_class(self, adapter_class):
+        return adapter_class or exchange_simulator_adapter.ExchangeSimulatorAdapter
+
+    @classmethod
+    def load_user_inputs(cls, tentacles_setup_config, tentacle_config):
+        # no user input in connector
+        pass
+
     @classmethod
     def is_supporting_exchange(cls, exchange_candidate_name) -> bool:
         return True
 
     @classmethod
     def is_simulated_exchange(cls) -> bool:
         return True
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_builder.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_builder.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_builder.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_channels.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_channels.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_channels.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_util.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,225 +5,222 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General Public License for more details.
+#  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import asyncio
-
 import trading_backend
 
-import octobot_commons.authentication as authentication
-import octobot_trading.errors as errors
-import octobot_trading.exchanges as exchanges
-
-
-async def create_exchanges(exchange_manager):
-    if exchange_manager.is_sandboxed and not exchange_manager.exchange_only:
-        exchange_manager.logger.info(f"Using sandbox exchange for {exchange_manager.exchange_name}")
-
-    if exchange_manager.is_backtesting:
-        # simulated : create exchange simulator instance
-        await create_simulated_exchange(exchange_manager)
-        exchange_manager.load_constants()
-    else:
-        # real : create a rest or websocket exchange instance
-        await create_real_exchange(exchange_manager)
-        exchange_manager.load_constants()
-        await initialize_real_exchange(exchange_manager)
-
-    if not exchange_manager.exchange_only:
-        # create exchange producers if necessary
-        await exchanges.create_exchange_producers(exchange_manager)
-
-    if exchange_manager.is_backtesting:
-        await init_simulated_exchange(exchange_manager)
-
-    exchange_manager.exchange_name = exchange_manager.exchange.name
-    exchange_manager.is_ready = True
+import octobot_commons.logging as logging
+import octobot_commons.constants as common_constants
+import octobot_commons.enums as common_enums
+import octobot_commons.tentacles_management as tentacles_management
+
+import octobot_tentacles_manager.api as api
+
+import octobot_trading.enums as enums
+import octobot_trading.constants as constants
+import octobot_trading.exchanges.types as exchanges_types
+import octobot_trading.exchanges.implementations as exchanges_implementations
+import octobot_trading.exchanges.exchange_builder as exchange_builder
+
+
+def get_rest_exchange_class(exchange_name, tentacles_setup_config):
+    return search_exchange_class_from_exchange_name(exchanges_types.RestExchange, exchange_name, tentacles_setup_config)
+
+
+def search_exchange_class_from_exchange_name(exchange_class, exchange_name,
+                                             tentacles_setup_config, enable_default=False):
+    exchange_class = get_exchange_class_from_name(exchange_class, exchange_name,  tentacles_setup_config, enable_default)
+    if exchange_class is not None:
+        return exchange_class
+    if enable_default:
+        return None
+
+    logging.get_logger("ExchangeUtil").debug(f"No specific exchange implementation for {exchange_name} found, "
+                                             f"using a default one.")
+    children_classes = tentacles_management.get_all_classes_from_parent(exchanges_implementations.DefaultRestExchange)
+    if children_classes:
+        # last one is the most advanced one
+        return children_classes[-1]
+    # fallback to DefaultRestExchange
+    return exchanges_implementations.DefaultRestExchange
+
+
+def get_exchange_class_from_name(exchange_parent_class, exchange_name, tentacles_setup_config, enable_default,
+                                 strict_name_matching=False):
+    for exchange_candidate in tentacles_management.get_all_classes_from_parent(exchange_parent_class):
+        try:
+            if _is_exchange_candidate_matching(exchange_candidate, exchange_name,
+                                               tentacles_setup_config, enable_default=enable_default) and \
+               (not strict_name_matching or exchange_candidate.get_name() == exchange_name):
+                return exchange_candidate
+        except NotImplementedError:
+            # A subclass of AbstractExchange will raise a NotImplementedError when calling its get_name() method
+            # Here we are returning only a subclass that matches the expected name
+            # Only Exchange Tentacles are implementing get_name() to specify the related exchange
+            # As we are searching for an exchange_type specific subclass
+            # We should ignore classes that raises NotImplementedError
+            pass
+    return None
+
+
+def _is_exchange_candidate_matching(exchange_candidate, exchange_name, tentacles_setup_config, enable_default=False):
+    return not exchange_candidate.is_simulated_exchange() and \
+           (not exchange_candidate.is_default_exchange() or enable_default) and \
+           exchange_candidate.is_supporting_exchange(exchange_name) and \
+           (tentacles_setup_config is None or
+            api.is_tentacle_activated_in_tentacles_setup_config(tentacles_setup_config,
+                                                                exchange_candidate.__name__))
+
+
+def get_order_side(order_type):
+    return enums.TradeOrderSide.BUY.value if order_type in (enums.TraderOrderType.BUY_LIMIT,
+                                                            enums.TraderOrderType.BUY_MARKET) \
+        else enums.TradeOrderSide.SELL.value
+
+
+def log_time_sync_error(logger, exchange_name, error, details):
+    logger.error(
+        f"{_get_time_sync_error_message(exchange_name, details)} Error: {error}")
 
 
-async def create_real_exchange(exchange_manager) -> None:
-    """
-    Create and initialize real REST exchange
-    :param exchange_manager: the related exchange manager
-    """
-    await _create_rest_exchange(exchange_manager)
+def _get_docs_url():
     try:
-        await exchange_manager.exchange.initialize()
-        if exchange_manager.exchange_only:
-            return
-        _create_exchange_backend(exchange_manager)
-        await _initialize_exchange_backend(exchange_manager)
-        _ensure_exchange_validity(exchange_manager)
-    except errors.AuthenticationError:
-        exchange_manager.logger.error("Authentication error, retrying without authentication...")
-        exchange_manager.without_auth = True
-        await create_real_exchange(exchange_manager)
-        return
-
-
-async def initialize_real_exchange(exchange_manager):
-    if not exchange_manager.exchange_only:
-        await exchanges.create_exchange_channels(exchange_manager)
-
-    # create Websocket exchange if possible
-    if not exchange_manager.rest_only:
-        # search for websocket
-        if exchanges.check_web_socket_config(exchange_manager.config, exchange_manager.exchange.name):
-            await exchanges.search_and_create_websocket(exchange_manager)
-
-
-def _ensure_exchange_validity(exchange_manager):
-    if exchange_manager.is_future and \
-            not exchange_manager.is_trader_simulated and \
-            not exchange_manager.is_valid_account:
-        error_message = f"Impossible to check exchange sponsoring due to" \
-                        f" {exchange_manager.init_error.__class__.__name__}." \
-            if isinstance(exchange_manager.init_error, trading_backend.TimeSyncError) \
-            else \
-            f"Impossible to start futures trading for {exchange_manager.exchange.name.capitalize()}: " \
-            f"incompatible account with no registered donation. Your OctoBot will work normally " \
-            f"for spot trading but will be *limited to backtesting for futures trading. " \
-            f"Please select spot trading on your exchange configuration."
-        raise errors.NotSupported(error_message)
+        import octobot.constants
+        return octobot.constants.OCTOBOT_DOCS_URL
+    except ImportError:
+        return "https://www.octobot.info"
 
 
-def _create_exchange_backend(exchange_manager):
+def _get_exchanges_docs_url():
     try:
-        exchange_manager.exchange_backend = trading_backend.exchange_factory.create_exchange_backend(
-            exchange_manager.exchange
-        )
-    except Exception as e:
-        exchange_manager.logger.exception(e, True, f"Error when creating exchange backend: {e}")
-
-
-async def _initialize_exchange_backend(exchange_manager):
-    if exchange_manager.exchange_backend is not None and exchange_manager.exchange.authenticated() \
-            and not exchange_manager.is_trader_simulated:
-        exchange_manager.logger.debug(await exchange_manager.exchange_backend.initialize())
-        if not exchange_manager.is_future:
-            return
-        try:
-            exchange_manager.is_valid_account = await _is_supporting_octobot()
-            if exchange_manager.is_valid_account:
-                return True
-            exchange_manager.is_valid_account, message = await exchange_manager.exchange_backend.is_valid_account()
-            if not exchange_manager.is_valid_account:
-                exchange_manager.logger.error(
-                    f"Incompatible {exchange_manager.exchange.name.capitalize()} account to use futures trading: "
-                    f"{message}. OctoBot relies on exchanges profits sharing to remain 100% free, please create a "
-                    f"new {exchange_manager.exchange.name.capitalize()} account or register a donation to support "
-                    f"the project. {exchanges.get_partners_explanation_message()}")
-        except trading_backend.TimeSyncError as err:
-            exchanges.log_time_sync_error(exchange_manager.logger, exchange_manager.exchange.name,
-                                          err, "account details")
-            exchange_manager.is_valid_account = False
-            exchange_manager.init_error = err
-        except Exception as err:
-            exchange_manager.is_valid_account = False
-            exchange_manager.init_error = err
-            exchange_manager.logger.exception(err, True, f"Error when loading exchange account: {err}")
-        finally:
-            if exchange_manager.is_valid_account:
-                exchange_manager.logger.info("On behalf of the OctoBot team, thank you for "
-                                             "actively supporting the project !")
-
-
-async def _is_supporting_octobot() -> bool:
+        import octobot.constants
+        return octobot.constants.EXCHANGES_DOCS_URL
+    except ImportError:
+        return "https://exchanges.octobot.info"
+
+
+def _get_time_sync_error_message(exchange_name, details):
+    return f"Time synchronization error when loading your {exchange_name.capitalize()} {details}. " \
+        f"To fix this, please synchronize your computer's clock. See " \
+        f"{_get_docs_url()}/installation/installation-troubleshoot#time-synchronization"
+
+
+def get_partners_explanation_message():
+    return f"More info on partner exchanges on {_get_exchanges_docs_url()}#partner-exchanges-support-octobot"
+
+
+def _get_minimal_exchange_config(exchange_name, exchange_config):
+    return {
+        common_constants.CONFIG_EXCHANGES: {
+            exchange_name: exchange_config
+        },
+        common_constants.CONFIG_TRADER: {
+            common_constants.CONFIG_ENABLED_OPTION: False
+        },
+        common_constants.CONFIG_SIMULATOR: {
+            common_constants.CONFIG_ENABLED_OPTION: False
+        },
+        common_constants.CONFIG_TIME_FRAME: [],
+        common_constants.CONFIG_CRYPTO_CURRENCIES: []
+    }
+
+
+async def is_compatible_account(exchange_name: str, exchange_config: dict, tentacles_setup_config, is_sandboxed: bool) \
+        -> (bool, bool, str):
+    """
+    Returns details regarding the compatibility of the account given in parameters
+    :return: (True if compatible, True if successful login, error explanation if any)
+    """
+    exchange_type = exchange_config.get(common_constants.CONFIG_EXCHANGE_TYPE, get_default_exchange_type(exchange_name))
+    builder = exchange_builder.ExchangeBuilder(
+        _get_minimal_exchange_config(exchange_name, exchange_config),
+        exchange_name
+    )
+    local_exchange_manager = await builder.use_tentacles_setup_config(tentacles_setup_config) \
+        .is_checking_credentials(False) \
+        .is_sandboxed(is_sandboxed) \
+        .is_using_exchange_type(exchange_type) \
+        .is_exchange_only() \
+        .is_rest_only() \
+        .is_loading_markets(False) \
+        .disable_trading_mode() \
+        .build()
+    backend = trading_backend.exchange_factory.create_exchange_backend(local_exchange_manager.exchange)
     try:
-        authenticator = authentication.Authenticator.instance()
-        if not authenticator.is_initialized():
-            initialization_timeout = 5
-            await authenticator.await_initialization(initialization_timeout)
-        if authenticator.user_account.supports.is_supporting():
-            return True
-    except asyncio.TimeoutError:
-        pass
-    return False
-
-
-async def _create_rest_exchange(exchange_manager) -> None:
-    """
-    create REST based on ccxt exchange
-    :param exchange_manager: the related exchange manager
-    """
-    if exchange_manager.is_future and not exchange_manager.is_spot_only:
-        await _search_and_create_future_exchange(exchange_manager)
-    elif exchange_manager.is_margin and not exchange_manager.is_spot_only:
-        await _search_and_create_margin_exchange(exchange_manager)
-    else:
-        await _search_and_create_spot_exchange(exchange_manager)
-
-    if not exchange_manager.exchange:
-        raise Exception(f"Can't create an exchange instance that match the exchange configuration ({exchange_manager})")
-
-
-async def create_simulated_exchange(exchange_manager):
-    if exchange_manager.is_future and not exchange_manager.is_spot_only:
-        exchange_manager.exchange = exchanges.FutureExchangeSimulator(exchange_manager.config, exchange_manager,
-                                                                      exchange_manager.backtesting)
-    elif exchange_manager.is_margin and not exchange_manager.is_spot_only:
-        exchange_manager.exchange = exchanges.MarginExchangeSimulator(exchange_manager.config, exchange_manager,
-                                                                      exchange_manager.backtesting)
-    else:
-        exchange_manager.exchange = exchanges.SpotExchangeSimulator(exchange_manager.config, exchange_manager,
-                                                                    exchange_manager.backtesting)
-
-    await exchange_manager.exchange.initialize()
-    _initialize_simulator_time_frames(exchange_manager)
-    exchange_manager.exchange_config.set_config_time_frame()
-    exchange_manager.exchange_config.set_config_traded_pairs()
-    await exchanges.create_exchange_channels(exchange_manager)
-
-
-async def init_simulated_exchange(exchange_manager):
-    await exchange_manager.exchange.create_backtesting_exchange_producers()
-
-
-async def _search_and_create_spot_exchange(exchange_manager) -> None:
-    """
-    Create a spot exchange if a SpotExchange matching class is found
-    :param exchange_manager: the related exchange manager
-    """
-    spot_exchange_class = exchanges.get_spot_exchange_class(exchange_manager.exchange_name,
-                                                            exchange_manager.tentacles_setup_config)
-    if spot_exchange_class:
-        exchange_manager.exchange = spot_exchange_class(config=exchange_manager.config,
-                                                        exchange_manager=exchange_manager)
-
-
-async def _search_and_create_margin_exchange(exchange_manager) -> None:
-    """
-    Create a margin exchange if a MarginExchange matching class is found
-    :param exchange_manager: the related exchange manager
-    """
-    margin_exchange_class = exchanges.get_margin_exchange_class(exchange_manager.exchange_name,
-                                                                exchange_manager.tentacles_setup_config)
-    if margin_exchange_class:
-        exchange_manager.exchange = margin_exchange_class(config=exchange_manager.config,
-                                                          exchange_manager=exchange_manager)
-
-
-async def _search_and_create_future_exchange(exchange_manager) -> None:
-    """
-    Create a future exchange if a FutureExchange matching class is found
-    :param exchange_manager: the related exchange manager
-    """
-    future_exchange_class = exchanges.get_future_exchange_class(exchange_manager.exchange_name,
-                                                                exchange_manager.tentacles_setup_config)
-    if future_exchange_class:
-        exchange_manager.exchange = future_exchange_class(config=exchange_manager.config,
-                                                          exchange_manager=exchange_manager)
-
-
-def _initialize_simulator_time_frames(exchange_manager):
-    """
-    Initialize simulator client time frames
-    :param exchange_manager: the related exchange manager
-    """
-    exchange_manager.client_time_frames = exchange_manager.exchange.get_available_time_frames()
+        is_compatible, error = await backend.is_valid_account()
+        if not local_exchange_manager.is_spot_only:
+            message = f"Future trading on {exchange_name.capitalize()} requires a supporting account. {error}." \
+                      f"Please create a new {exchange_name.capitalize()} account to use futures trading. "
+            # only ensure compatibility for non spot trading
+            return is_compatible, True, message if error else error
+        else:
+            # auth didn't fail, spot trading is always allowed
+            return True, True, None
+    except trading_backend.TimeSyncError:
+        return False, False, _get_time_sync_error_message(exchange_name, "account details")
+    except trading_backend.ExchangeAuthError:
+        return False, False, f"Invalid {exchange_name.capitalize()} authentication details"
+    except Exception as e:
+        return False, True, f"Error when loading exchange account: {e}"
+    finally:
+        # do not log stopping message
+        logger = local_exchange_manager.exchange.connector.logger
+        logger.disable(True)
+        await local_exchange_manager.stop(enable_logs=False)
+        logger.disable(False)
+
+
+async def get_historical_ohlcv(local_exchange_manager, symbol, time_frame, start_time, end_time):
+    """
+    Async generator, use as follows:
+        async for candles in get_historical_ohlcv(exchange_manager, pair, time_frame, start_time, end_time):
+            # candles stuff
+    WARNING: start_time and end_time should be milliseconds timestamps
+    """
+    reached_max = False
+    while start_time < end_time and not reached_max:
+        candles = await local_exchange_manager.exchange.get_symbol_prices(symbol, time_frame, since=int(start_time))
+        if candles:
+            while candles[-1][common_enums.PriceIndexes.IND_PRICE_TIME.value] * 1000 > end_time and candles:
+                candles.pop(-1)
+                reached_max = True
+            if candles:
+                yield candles
+                start_time = candles[-1][common_enums.PriceIndexes.IND_PRICE_TIME.value] * 1000
+                # avoid fetching the last element twice
+                start_time += 1
+            else:
+                reached_max = True
+        else:
+            reached_max = True
+
+
+def get_exchange_type(exchange_manager_instance):
+    if exchange_manager_instance.is_spot_only:
+        return enums.ExchangeTypes.SPOT
+    if exchange_manager_instance.is_future:
+        return enums.ExchangeTypes.FUTURE
+    if exchange_manager_instance.is_margin:
+        return enums.ExchangeTypes.MARGIN
+    return enums.ExchangeTypes.SPOT
+
+
+def get_default_exchange_type(exchange_name):
+    if exchange_name in constants.DEFAULT_FUTURE_EXCHANGES:
+        return common_constants.CONFIG_EXCHANGE_FUTURE
+    return common_constants.DEFAULT_EXCHANGE_TYPE
+
+
+def get_supported_exchange_types(exchange_name):
+    exchange_class = get_exchange_class_from_name(exchanges_types.RestExchange, exchange_name, None, False,
+                                                  strict_name_matching=True)
+    if exchange_class is None:
+        # default
+        return [enums.ExchangeTypes.SPOT]
+    return exchange_class.get_supported_exchange_types()
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_websocket_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_websocket_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchange_websocket_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchange_websocket_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,38 +18,37 @@
 
 
 def is_exchange_managed_by_websocket(exchange_manager, channel):
     """
     # TODO improve checker
     """
     return not exchange_manager.rest_only \
-           and exchange_manager.has_websocket \
-           and not exchange_manager.is_backtesting \
-           and channel in octobot_trading.constants.WEBSOCKET_FEEDS_TO_TRADING_CHANNELS \
-           and any([exchange_manager.exchange_web_socket.is_feed_available(feed)
-                    for feed in octobot_trading.constants.WEBSOCKET_FEEDS_TO_TRADING_CHANNELS[channel]])
+        and exchange_manager.has_websocket \
+        and not exchange_manager.is_backtesting \
+        and channel in octobot_trading.constants.WEBSOCKET_FEEDS_TO_TRADING_CHANNELS \
+        and any([exchange_manager.exchange_web_socket.is_feed_available(feed)
+                 for feed in octobot_trading.constants.WEBSOCKET_FEEDS_TO_TRADING_CHANNELS[channel]])
 
 
 def is_websocket_feed_requiring_init(exchange_manager, channel):
     return any([exchange_manager.exchange_web_socket.is_feed_requiring_init(feed)
                 for feed in octobot_trading.constants.WEBSOCKET_FEEDS_TO_TRADING_CHANNELS[channel]])
 
 
 async def search_and_create_websocket(exchange_manager):
-    socket_manager = exchanges.search_websocket_class(exchanges.WebSocketExchange, exchange_manager)
-    if socket_manager is not None:
-        await _create_websocket(exchange_manager, exchanges.WebSocketExchange.__name__, socket_manager)
+    ws_exchange_class = exchanges.search_websocket_class(exchanges.WebSocketExchange, exchange_manager)
+    if ws_exchange_class is not None:
+        await _create_websocket(exchange_manager, exchanges.WebSocketExchange.__name__, ws_exchange_class)
 
 
-async def _create_websocket(exchange_manager, websocket_class_name, socket_manager):
+async def _create_websocket(exchange_manager, websocket_class_name, ws_exchange_class):
     try:
-        exchange_manager.exchange_web_socket = socket_manager.get_websocket_client(exchange_manager.config,
-                                                                                   exchange_manager)
+        exchange_manager.exchange_web_socket = ws_exchange_class(exchange_manager.config, exchange_manager)
         await _init_websocket(exchange_manager)
-        exchange_manager.logger.info(f"{socket_manager.get_name()} connected to "
+        exchange_manager.logger.info(f"{ws_exchange_class.get_name()} connected to "
                                      f"{exchange_manager.exchange.name.capitalize()}")
     except Exception as e:
         exchange_manager.logger.error(f"Fail to init websocket for {websocket_class_name} "
                                       f"({exchange_manager.exchange.name}): {e}")
         exchange_manager.exchange_web_socket = None
         exchange_manager.has_websocket = False
         raise e
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchanges.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchanges.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/exchanges.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/ccxt_websocket_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/default_websocket_exchange.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 cimport octobot_trading.exchanges.types as exchanges_types
 
-cdef class CCXTWebSocketExchange(exchanges_types.WebSocketExchange):
+cdef class DefaultWebSocketExchange(exchanges_types.WebSocketExchange):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/ccxt_websocket_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/default_websocket_exchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,32 +10,28 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-import octobot_trading.exchanges.connectors.ccxt_websocket_connector as ccxt_websocket_connector
+import octobot_trading.exchanges.connectors.ccxt.ccxt_websocket_connector as ccxt_websocket_connector
 import octobot_trading.exchanges.types as exchanges_types
 import octobot_tentacles_manager.api as api
 
 
-#TODO remove?
-class CCXTWebSocketExchange(exchanges_types.WebSocketExchange):
-    @staticmethod
-    def get_websocket_client(config, exchange_manager):
-        return CCXTWebSocketExchange(config, exchange_manager)
+class DefaultWebSocketExchange(exchanges_types.WebSocketExchange):
+    DEFAULT_CONNECTOR_CLASS = ccxt_websocket_connector.CCXTWebsocketConnector
 
     @classmethod
-    def get_exchange_connector_class(cls, exchange_manager: object):
+    def get_exchange_connector_class(cls, exchange_manager):
         return api.get_class_from_name_with_activated_required_tentacles(
             name=exchange_manager.exchange_name,
             tentacles_setup_config=exchange_manager.tentacles_setup_config,
-            with_class_method=cls.get_class_method_name_to_get_compatible_websocket(exchange_manager),
-            parent_class=ccxt_websocket_connector.CCXTWebsocketConnector
+            parent_class=cls.DEFAULT_CONNECTOR_CLASS
         )
 
     def create_feeds(self):
         try:
             connector = self.websocket_connector(config=self.config, exchange_manager=self.exchange_manager)
             connector.initialize(pairs=self.pairs, time_frames=self.time_frames, channels=self.channels)
             self.websocket_connectors.append(connector)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/cryptofeed_websocket_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader_simulator.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-cimport octobot_trading.exchanges.types as exchanges_types
+cimport octobot_trading.exchanges.traders.trader as trader
 
-cdef class CryptofeedWebSocketExchange(exchanges_types.WebSocketExchange):
+cdef class TraderSimulator(trader.Trader):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/cryptofeed_websocket_exchange.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_builder.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,34 +9,49 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import pytest
+import octobot_trading.api as api
+import octobot_trading.exchanges as exchanges
 
-import octobot_trading.exchanges.connectors.cryptofeed_websocket_connector as cryptofeed_websocket_connector
-import octobot_trading.exchanges.types as exchanges_types
-import octobot_tentacles_manager.api as api
-
-
-class CryptofeedWebSocketExchange(exchanges_types.WebSocketExchange):
-    @staticmethod
-    def get_websocket_client(config, exchange_manager):
-        return CryptofeedWebSocketExchange(config, exchange_manager)
-
-    @classmethod
-    def get_exchange_connector_class(cls, exchange_manager: object):
-        return api.get_class_from_name_with_activated_required_tentacles(
-            name=exchange_manager.exchange_name,
-            tentacles_setup_config=exchange_manager.tentacles_setup_config,
-            with_class_method=cls.get_class_method_name_to_get_compatible_websocket(exchange_manager),
-            parent_class=cryptofeed_websocket_connector.CryptofeedWebsocketConnector
-        )
-
-    def create_feeds(self):
-        try:
-            connector = self.websocket_connector(config=self.config, exchange_manager=self.exchange_manager)
-            connector.initialize(pairs=self.pairs, time_frames=self.time_frames, channels=self.channels)
-            self.websocket_connectors.append(connector)
-        except ValueError as e:
-            self.logger.exception(e, True, f"Fail to create feed : {e}")
+from tests.exchanges import exchange_manager
+from tests import event_loop
+
+
+# All test coroutines will be treated as marked.
+pytestmark = pytest.mark.asyncio
+
+
+async def test_build_trading_modes_if_required(exchange_manager):
+    builder = exchanges.ExchangeBuilder({}, "binanceus")
+    builder.exchange_manager = exchange_manager
+
+    # no set trader: no trading mode creation attempt
+    assert builder.exchange_manager.trader is None
+    await builder._build_trading_modes_if_required(None)
+    assert builder.exchange_manager.trader is None
+
+    # with trader simulator: will attempt to create a trading mode and fail (because of the None arg)
+    builder.is_simulated()
+    with pytest.raises(AttributeError):
+        await builder._build_trading_modes_if_required(None)
+
+
+async def test_build_collector_exchange(exchange_manager):
+    new_exchange_manager = await api.create_exchange_builder(exchange_manager.config, exchange_manager.exchange_name) \
+        .is_simulated() \
+        .is_rest_only() \
+        .is_exchange_only() \
+        .is_without_auth() \
+        .is_ignoring_config() \
+        .disable_trading_mode() \
+        .use_tentacles_setup_config(exchange_manager.tentacles_setup_config) \
+        .build()
+    assert new_exchange_manager is not exchange_manager
+    assert new_exchange_manager.config is exchange_manager.config
+    assert new_exchange_manager.exchange_name == exchange_manager.exchange_name
+    assert new_exchange_manager.tentacles_setup_config is exchange_manager.tentacles_setup_config
+    await new_exchange_manager.stop()
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/default_spot_ccxt_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/transfer_transaction.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,21 @@
-#  Drakkar-Software OctoBot-Private-Tentacles
+# cython: language_level=3
+#  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General Public License for more details.
+#  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_trading.enums
-import octobot_trading.exchanges.implementations.spot_ccxt_exchange as spot_ccxt_exchange
 
+cimport octobot_trading.personal_data.transactions.transaction as transaction
 
-#TODO remove
-class DefaultCCXTSpotExchange(spot_ccxt_exchange.SpotCCXTExchange):
-    @classmethod
-    def get_name(cls) -> str:
-        return cls.__name__
-
-    @classmethod
-    def is_default_exchange(cls) -> bool:
-        return True
-
-    async def switch_to_account(self, account_type: octobot_trading.enums.AccountTypes):
-        # Currently not supported
-        pass
+cdef class TransferTransaction(transaction.Transaction):
+    pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/future_ccxt_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/default_rest_exchange.pxd`

 * *Files 17% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchanges.types as exchanges_types
 
-cdef class FutureCCXTExchange(exchanges_types.FutureExchange):
-    # cpdef str get_default_type(self)   generating a segfault on exchange that both extend spot and future exchanges
-    cpdef str get_pair_market_type(self, str pair, str property_name, bint def_value=*)
+cimport octobot_trading.exchanges.types.rest_exchange as rest_exchange
+
+cdef class DefaultRestExchange(rest_exchange.RestExchange):
+    pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/future_exchange_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/exchange_simulator.pxd`

 * *Files 7% similar despite different names*

```diff
@@ -11,13 +11,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 cimport octobot_backtesting.backtesting as backtesting
-cimport octobot_trading.exchanges.types as exchanges_types
+cimport octobot_trading.exchanges.types.rest_exchange as rest_exchange
 
-cdef class FutureExchangeSimulator(exchanges_types.FutureExchange):
+cdef class ExchangeSimulator(rest_exchange.RestExchange):
     cdef public backtesting.Backtesting backtesting
 
     cdef public list exchange_importers
+
+    cpdef list get_backtesting_data_files(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/future_exchange_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/exchange_simulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,85 +10,56 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import octobot_trading.constants as constants
-import octobot_trading.exchanges.connectors as exchange_connectors
-import octobot_trading.exchanges.types as exchanges_types
+import octobot_trading.exchanges.connectors.simulator.exchange_simulator_connector as exchange_simulator_connector
+import octobot_trading.exchanges.types.rest_exchange as rest_exchange
 
 
-#TODO remove
-class FutureExchangeSimulator(exchanges_types.FutureExchange):
+class ExchangeSimulator(rest_exchange.RestExchange):
+    DEFAULT_CONNECTOR_CLASS = exchange_simulator_connector.ExchangeSimulatorConnector
+
     def __init__(self, config, exchange_manager, backtesting):
-        super().__init__(config, exchange_manager)
-        self.exchange_importers = []
         self.backtesting = backtesting
-        self.connector = exchange_connectors.ExchangeSimulator(config, exchange_manager, backtesting=backtesting)
+        self.exchange_importers = []
+        super().__init__(config, exchange_manager)
+
+    def _create_connector(self, config, exchange_manager, connector_class):
+        return (connector_class or self.DEFAULT_CONNECTOR_CLASS)(
+            config,
+            exchange_manager,
+            self.backtesting,
+            adapter_class=self.get_adapter_class(),
+        )
 
     async def initialize_impl(self):
-        await self.connector.initialize()
-        self.symbols = self.connector.symbols
-        self.time_frames = self.connector.time_frames
+        await super().initialize_impl()
         self.exchange_importers = self.connector.exchange_importers
 
     async def stop(self) -> None:
-        await self.connector.stop()
-        self.exchange_manager = None
+        await super().stop()
         self.backtesting = None
         self.exchange_importers = None
 
     @classmethod
-    def get_name(cls) -> str:
-        return cls.__name__
-
-    @classmethod
     def is_supporting_exchange(cls, exchange_candidate_name) -> bool:
-        return exchange_connectors.ExchangeSimulator.is_supporting_exchange(exchange_candidate_name)
+        return exchange_simulator_connector.ExchangeSimulatorConnector.is_supporting_exchange(exchange_candidate_name)
 
     @classmethod
     def is_simulated_exchange(cls) -> bool:
-        return exchange_connectors.ExchangeSimulator.is_simulated_exchange()
-
-    def get_exchange_current_time(self):
-        return self.connector.get_exchange_current_time()
-
-    def get_available_time_frames(self):
-        return self.connector.get_available_time_frames()
-
-    def get_split_pair_from_exchange(self, pair) -> (str, str):
-        return self.connector.get_split_pair_from_exchange(pair)
-
-    def get_pair_cryptocurrency(self, pair) -> str:
-        return self.connector.get_pair_cryptocurrency(pair)
-
-    @staticmethod
-    def get_real_available_data(exchange_importers):
-        return exchange_connectors.ExchangeSimulator.get_real_available_data(exchange_importers)
-
-    @staticmethod
-    def handles_real_data_for_updater(channel_type, available_data):
-        return exchange_connectors.ExchangeSimulator.handles_real_data_for_updater(channel_type=channel_type,
-                                                                                   available_data=available_data)
+        return exchange_simulator_connector.ExchangeSimulatorConnector.is_simulated_exchange()
 
     async def create_backtesting_exchange_producers(self):
         return await self.connector.create_backtesting_exchange_producers()
 
-    def get_market_status(self, symbol, price_example=None, with_fixer=True):
-        return self.connector.get_market_status(symbol, price_example=price_example, with_fixer=with_fixer)
-
-    def get_uniform_timestamp(self, timestamp):
-        return self.connector.get_uniform_timestamp(timestamp)
-
-    def get_fees(self, symbol):
-        return self.connector.get_fees(symbol)
-
-    def get_trade_fee(self, symbol, order_type, quantity, price, taker_or_maker):
-        return self.connector.get_trade_fee(symbol, order_type, quantity, price, taker_or_maker)
+    def get_available_time_frames(self):
+        return self.connector.get_available_time_frames()
 
     def get_time_frames(self, importer):
         return self.connector.get_time_frames(importer)
 
     def get_current_future_candles(self):
         return self.connector.current_future_candles
 
@@ -121,15 +92,15 @@
 
     async def get_funding_rate(self, symbol: str, **kwargs: dict):
         return self.exchange_manager.exchange_config.backtesting_exchange_config.funding_rate
 
     async def get_position_mode(self, symbol: str, **kwargs: dict):
         return constants.DEFAULT_SYMBOL_POSITION_MODE
 
-    async def set_symbol_leverage(self, symbol: str, leverage: int):
+    async def set_symbol_leverage(self, symbol: str, leverage: int, **kwargs):
         pass  # let trader update the contract
 
     async def set_symbol_margin_type(self, symbol: str, isolated: bool):
         pass  # let trader update the contract
 
     async def set_symbol_position_mode(self, symbol: str, one_way: bool):
         pass  # let trader update the contract
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/margin_ccxt_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchanges.types as exchanges_types
-cimport octobot_trading.exchanges.implementations as exchange_implementations
+cimport octobot_trading.exchange_channel as exchanges_channel
 
+cdef class OrdersProducer(exchanges_channel.ExchangeChannelProducer):
+    pass
 
-cdef class MarginCCXTExchange(exchanges_types.MarginExchange):
+cdef class OrdersChannel(exchanges_channel.ExchangeChannel):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/margin_exchange_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/__init__.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_backtesting.backtesting as backtesting
-cimport octobot_trading.exchanges.types as exchanges_types
 
-cdef class MarginExchangeSimulator(exchanges_types.MarginExchange):
-    cdef public backtesting.Backtesting backtesting
+from octobot_trading.exchanges.types.rest_exchange cimport (
+    RestExchange,
+)
+from octobot_trading.exchanges.types.websocket_exchange cimport (
+    WebSocketExchange,
+)
 
-    cdef public list exchange_importers
+__all__ = [
+    "RestExchange",
+    "WebSocketExchange",
+]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/rest_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/__init__.pxd`

 * *Files 27% similar despite different names*

```diff
@@ -9,37 +9,42 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_trading.exchanges.abstract_exchange as abstract_exchange
-import octobot_trading.exchanges.connectors as exchange_connectors
 
+from octobot_trading.exchanges.util cimport exchange_market_status_fixer
+from octobot_trading.exchanges.util.exchange_market_status_fixer cimport (
+    ExchangeMarketStatusFixer,
+    is_ms_valid,
+)
+from octobot_trading.exchanges.util cimport exchange_util
+from octobot_trading.exchanges.util.exchange_util cimport (
+    get_rest_exchange_class,
+    get_order_side,
+    get_exchange_type,
+    get_default_exchange_type,
+    get_supported_exchange_types,
+    get_exchange_class_from_name,
+)
+from octobot_trading.exchanges.util cimport websockets_util
+from octobot_trading.exchanges.util.websockets_util cimport (
+    force_disable_web_socket,
+    check_web_socket_config,
+    search_websocket_class,
+)
 
-# TODO
-class RestExchange(abstract_exchange.AbstractExchange):
-    """
-    RestExchange is only calling the right exchange connector and should be used for each exchange
-    request regardless of the trading type (spot / future / etc)
-    """
-    DEFAULT_CONNECTOR_CLASS = exchange_connectors.CCXTExchange
-
-    def __init__(self, config, exchange_manager, connector_class=DEFAULT_CONNECTOR_CLASS):
-        super().__init__(config, exchange_manager)
-        self.connector = connector_class(
-            config,
-            exchange_manager,
-            additional_ccxt_config=self.get_additional_connector_config()  # move to connector
-        )
-        # commented for pylint
-        # self.connector.client.options['defaultType'] = self.get_default_type() # move to connector
-
-    async def initialize_impl(self):
-        await self.connector.initialize()
-        self.symbols = self.connector.symbols
-        self.time_frames = self.connector.time_frames
-
-    async def stop(self) -> None:
-        await self.connector.stop()
-        self.exchange_manager = None
+__all__ = [
+    "ExchangeMarketStatusFixer",
+    "is_ms_valid",
+    "get_rest_exchange_class",
+    "get_order_side",
+    "force_disable_web_socket",
+    "check_web_socket_config",
+    "search_websocket_class",
+    "get_exchange_type",
+    "get_default_exchange_type",
+    "get_supported_exchange_types",
+    "get_exchange_class_from_name",
+]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/spot_ccxt_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/market_order.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchanges.types as exchanges_types
+cimport octobot_trading.personal_data.orders.order as order_class
 
-cdef class SpotCCXTExchange(exchanges_types.SpotExchange):
-    # cpdef str get_default_type(self)   generating a segfault on exchange that both extend spot and future exchanges
+cdef class MarketOrder(order_class.Order):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/implementations/spot_exchange_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater_simulator.pxd`

 * *Files 17% similar despite different names*

```diff
@@ -6,20 +6,15 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_backtesting.backtesting as backtesting
-cimport octobot_trading.exchanges.types as exchanges_types
+cimport octobot_trading.personal_data.orders.channel.orders_updater as orders_updater
 
-cdef class SpotExchangeSimulator(exchanges_types.SpotExchange):
-    cdef public backtesting.Backtesting backtesting
-
-    cdef public list exchange_importers
-
-    cpdef list get_backtesting_data_files(self)
+cdef class OrdersUpdaterSimulator(orders_updater.OrdersUpdater):
+    pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         super().__init__()
         self.exchange_manager = exchange_manager
         self.config = config
 
         self.risk = octobot_trading.constants.ZERO
         try:
             self.set_risk(decimal.Decimal(str(self.config[octobot_commons.constants.CONFIG_TRADING]
-                          [octobot_commons.constants.CONFIG_TRADER_RISK])))
+                                              [octobot_commons.constants.CONFIG_TRADER_RISK])))
         except KeyError:
             self.set_risk(octobot_trading.constants.ZERO)
         self.allow_artificial_orders = self.config.get(octobot_commons.constants.CONFIG_TRADER_ALLOW_ARTIFICIAL_ORDERS,
                                                        True)
 
         # logging
         self.trader_type_str = octobot_trading.constants.REAL_TRADER_STR
@@ -80,66 +80,75 @@
             self.risk = risk
         return self.risk
 
     """
     Orders
     """
 
-    async def create_order(self, order, loaded: bool = False, params: dict = None, pre_init_callback=None):
+    async def create_order(self, order, loaded: bool = False, params: dict = None,
+                           wait_for_creation=True,
+                           creation_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT):
         """
         Create a new order from an OrderFactory created order, update portfolio, registers order in order manager and
         notifies order channel.
         :param order: Order to create
         :param loaded: True if this order is fetched from an exchange only and therefore not created by this OctoBot
         :param params: Additional parameters to give to the order upon creation (used in real trading only)
-        :param pre_init_callback: A callback function that will be called just before initializing the order
+        :param wait_for_creation: when True, always make sure the order is completely created before returning.
+        On exchanges async api, a create request will return before the order is actually live on exchange, in this case
+        the associated order state will make sure that the order is creating by polling the order from the exchange.
+        :param creation_timeout: time before raising a timeout error when waiting for an order creation
         :return: The crated order instance
         """
-        created_order = order
         if loaded:
             order.is_from_this_octobot = False
             self.logger.debug(f"Order loaded : {order.to_string()} ")
-        else:
-            try:
-                params = params or {}
-                self.logger.info(f"Creating order: {created_order}")
-                created_order = await self._create_new_order(order, params)
-                if created_order is None:
-                    self.logger.warning(f"Order not created order on {self.exchange_manager.exchange_name} "
-                                        f"(failed attempt to create: {order}). This is likely due to "
-                                        f"the order being refused by the exchange.")
-                    return None
-            except Exception as e:
-                self.logger.exception(e, True, f"Unexpected error when creating order: {e}")
-                return None
-
-        if pre_init_callback is not None:
-            await pre_init_callback(created_order)
+            # force initialize to always create open state
+            await order.initialize()
+            return order
+        # octobot order
+        created_order = order
+        try:
+            params = params or {}
+            self.logger.info(f"Creating order: {created_order}")
+            created_order = await self._create_new_order(order, params, wait_for_creation=wait_for_creation,
+                                                         creation_timeout=creation_timeout)
+            if created_order is None:
+                self.logger.warning(f"Order not created order on {self.exchange_manager.exchange_name} "
+                                    f"(failed attempt to create: {order}). This is likely due to "
+                                    f"the order being refused by the exchange.")
+        except Exception as e:
+            import traceback
+            print(traceback.format_exc())
+            self.logger.exception(e, True, f"Unexpected error when creating order: {e}")
+            return None
 
-        # force initialize to always create open state
-        await created_order.initialize()
         return created_order
 
     async def create_artificial_order(self, order_type, symbol, current_price, quantity, price,
-                                      emit_trading_signals=False):
+                                      emit_trading_signals=False,
+                                      wait_for_creation=True,
+                                      creation_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT):
         """
         Creates an OctoBot managed order (managed orders example: stop loss that is not published on the exchange and
         that is maintained internally).
         """
         order = order_factory.create_order_instance(trader=self,
                                                     order_type=order_type,
                                                     symbol=symbol,
                                                     current_price=current_price,
                                                     quantity=quantity,
                                                     price=price)
         async with signals.remote_signal_publisher(self.exchange_manager, order.symbol, emit_trading_signals):
             await signals.create_order(
                 self.exchange_manager,
                 emit_trading_signals and signals.should_emit_trading_signal(self.exchange_manager),
-                order
+                order,
+                wait_for_creation=wait_for_creation,
+                creation_timeout=creation_timeout
             )
 
     async def edit_order(self, order: object,
                          edited_quantity: decimal.Decimal = None,
                          edited_price: decimal.Decimal = None,
                          edited_stop_price: decimal.Decimal = None,
                          edited_current_price: decimal.Decimal = None,
@@ -207,20 +216,23 @@
                 self.logger.info(f"Edited order: {order}")
             return changed
         finally:
             if previous_order_id != order.order_id:
                 # order id changed: update orders_manager to keep consistency
                 self.exchange_manager.exchange_personal_data.orders_manager.replace_order(previous_order_id, order)
 
-    async def _create_new_order(self, new_order: object, params: dict) -> object:
+    async def _create_new_order(self, new_order: object, params: dict,
+                                wait_for_creation=True,
+                                creation_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT) -> object:
         """
         Creates an exchange managed order, it might be a simulated or a real order.
-        Portfolio will be updated by the create order state after order will be initialized
+        Portfolio will be updated by the created order state after order will be initialized
         """
         updated_order = new_order
+        is_pending_creation = False
         if not self.simulate and not new_order.is_self_managed():
             order_params = self.exchange_manager.exchange.get_order_additional_params(new_order)
             order_params.update(params)
             created_order = await self.exchange_manager.exchange.create_order(new_order.order_type,
                                                                               new_order.symbol,
                                                                               new_order.origin_quantity,
                                                                               new_order.origin_price,
@@ -229,28 +241,40 @@
                                                                               new_order.created_last_price,
                                                                               params=order_params)
             if created_order is None:
                 return None
             self.logger.debug(f"Successfully created order on {self.exchange_manager.exchange_name}: {created_order}")
 
             # get real order from exchange
-            updated_order = order_factory.create_order_instance_from_raw(self, created_order, force_open=True)
+            updated_order = order_factory.create_order_instance_from_raw(
+                self, created_order, force_open_or_pending_creation=True
+            )
+            is_pending_creation = updated_order.status == enums.OrderStatus.PENDING_CREATION
 
             # rebind local elements to new order instance
             if new_order.order_group:
                 updated_order.add_to_order_group(new_order.order_group)
             updated_order.tag = new_order.tag
             updated_order.chained_orders = new_order.chained_orders
             for chained_order in new_order.chained_orders:
                 chained_order.triggered_by = updated_order
             updated_order.triggered_by = new_order.triggered_by
             updated_order.has_been_bundled = new_order.has_been_bundled
             updated_order.exchange_creation_params = new_order.exchange_creation_params
             updated_order.is_waiting_for_chained_trigger = new_order.is_waiting_for_chained_trigger
             updated_order.set_shared_signal_order_id(new_order.shared_signal_order_id)
+
+            if is_pending_creation:
+                # register order as pending order, it will then be added to live orders in order manager once open
+                self.exchange_manager.exchange_personal_data.orders_manager.register_pending_creation_order(updated_order)
+
+        await updated_order.initialize()
+        if is_pending_creation and wait_for_creation \
+                and updated_order.state is not None and updated_order.state.is_pending():
+            await updated_order.state.wait_for_terminate(creation_timeout)
         return updated_order
 
     async def bundle_chained_order_with_uncreated_order(self, order, chained_order, **kwargs):
         """
         Creates and bundles an order as a chained order to the given order.
         When supported and in real trading, return the stop loss parameters to be given when
         pushing the initial order on exchange
@@ -318,15 +342,15 @@
                         # retry to cancel order
                         self.logger.debug(f"Failed to cancel order ({err}), retrying")
                         order_status = await self.exchange_manager.exchange.cancel_order(order.order_id, order.symbol)
                 except Exception as e:
                     self.logger.exception(e, True, f"Failed to cancel order {order}")
                     return False
                 if order_status is enums.OrderStatus.CANCELED:
-                    order.status = octobot_trading.enums.OrderStatus.CLOSED
+                    order.status = octobot_trading.enums.OrderStatus.CANCELED
                     self.logger.debug(f"Successfully cancelled order {order}")
                 elif order_status is enums.OrderStatus.PENDING_CANCEL:
                     order.status = octobot_trading.enums.OrderStatus.PENDING_CANCEL
                     self.logger.debug(f"Order cancel in progress for {order}")
             else:
                 order.status = octobot_trading.enums.OrderStatus.CANCELED
 
@@ -386,24 +410,24 @@
                     (cancel_loaded_orders or order.is_from_this_octobot):
                 async with signals.remote_signal_publisher(self.exchange_manager, order.symbol, emit_trading_signals):
                     cancelled = await signals.cancel_order(
                         self.exchange_manager,
                         emit_trading_signals and signals.should_emit_trading_signal(self.exchange_manager),
                         order,
                         wait_for_cancelling=wait_for_cancelling,
-                        cancelling_timeout=cancelling_timeout,)
+                        cancelling_timeout=cancelling_timeout, )
                 if cancelled:
                     cancelled_orders.append(order)
                 all_cancelled = cancelled and all_cancelled
         return all_cancelled, cancelled_orders
 
     async def cancel_all_open_orders_with_currency(
-        self, currency, emit_trading_signals=False,
-        wait_for_cancelling=True,
-        cancelling_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT
+            self, currency, emit_trading_signals=False,
+            wait_for_cancelling=True,
+            cancelling_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT
     ) -> bool:
         """
         Should be called only if the goal is to cancel all open orders for each traded symbol containing the
         given currency.
         :param currency: Currency to find trading pairs to cancel orders on.
         :param emit_trading_signals: when true, trading signals will be emitted
         :param wait_for_cancelling: when True, always make sure the order is completely cancelled before returning.
@@ -417,17 +441,17 @@
                 all_cancelled = (await self.cancel_open_orders(symbol, emit_trading_signals=emit_trading_signals,
                                                                wait_for_cancelling=wait_for_cancelling,
                                                                cancelling_timeout=cancelling_timeout))[0] \
                                 and all_cancelled
         return all_cancelled
 
     async def cancel_all_open_orders(
-        self, emit_trading_signals=False,
-        wait_for_cancelling=True,
-        cancelling_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT
+            self, emit_trading_signals=False,
+            wait_for_cancelling=True,
+            cancelling_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT
     ) -> bool:
         """
         Cancel all open orders registered on this bot.
         :param emit_trading_signals: when true, trading signals will be emitted
         :param wait_for_cancelling: when True, always make sure the order is completely cancelled before returning.
         :param cancelling_timeout: time before raising a timeout error when waiting for an order cancel
         :return: True if all orders got cancelled, False if an error occurred
@@ -437,15 +461,15 @@
             if not order.is_cancelled():
                 async with signals.remote_signal_publisher(self.exchange_manager, order.symbol, emit_trading_signals):
                     all_cancelled = await signals.cancel_order(
                         self.exchange_manager,
                         emit_trading_signals and signals.should_emit_trading_signal(self.exchange_manager),
                         order,
                         wait_for_cancelling=wait_for_cancelling,
-                        cancelling_timeout=cancelling_timeout,) and all_cancelled
+                        cancelling_timeout=cancelling_timeout, ) and all_cancelled
         return all_cancelled
 
     async def _sell_everything(self, symbol, inverted, timeout=None):
         created_orders = []
         order_type = octobot_trading.enums.TraderOrderType.BUY_MARKET \
             if inverted else octobot_trading.enums.TraderOrderType.SELL_MARKET
         async with self.exchange_manager.exchange_personal_data.portfolio_manager.portfolio.lock:
@@ -454,16 +478,17 @@
             if inverted:
                 if price > 0:
                     quantity = current_market_quantity / price
                 else:
                     quantity = 0
             else:
                 quantity = current_symbol_holding
-            for order_quantity, order_price in decimal_order_adapter.decimal_check_and_adapt_order_details_if_necessary(quantity, price,
-                                                                                                        symbol_market):
+            for order_quantity, order_price in decimal_order_adapter.decimal_check_and_adapt_order_details_if_necessary(
+                    quantity, price,
+                    symbol_market):
                 current_order = order_factory.create_order_instance(trader=self,
                                                                     order_type=order_type,
                                                                     symbol=symbol,
                                                                     current_price=order_price,
                                                                     quantity=order_quantity,
                                                                     price=order_price)
                 created_orders.append(
@@ -503,21 +528,27 @@
         """
         return trade_factory.create_trade_from_order(order)
 
     """
     Positions
     """
 
-    async def close_position(self, position, limit_price=None, timeout=1, emit_trading_signals=False):
+    async def close_position(self, position, limit_price=None, timeout=1, emit_trading_signals=False,
+                             wait_for_creation=True,
+                             creation_timeout=octobot_trading.constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT):
         """
         Creates a close position order
         :param position: the position to close
         :param limit_price: the close order limit price if None uses a market order
         :param timeout: the mark price timeout
         :param emit_trading_signals: when true, trading signals will be emitted
+        :param wait_for_creation: when True, always make sure the order is completely created before returning.
+        On exchanges async api, a create request will return before the order is actually live on exchange, in this case
+        the associated order state will make sure that the order is creating by polling the order from the exchange.
+        :param creation_timeout: time before raising a timeout error when waiting for an order creation
         :return: the list of created orders
         """
         created_orders = []
         async with self.exchange_manager.exchange_personal_data.portfolio_manager.portfolio.lock:
             _, _, _, price, symbol_market = await order_util.get_pre_order_data(self.exchange_manager,
                                                                                 position.symbol,
                                                                                 timeout=timeout)
@@ -541,15 +572,18 @@
                                                                     reduce_only=True,
                                                                     close_position=True)
                 async with signals.remote_signal_publisher(self.exchange_manager, current_order.symbol,
                                                            emit_trading_signals):
                     order = await signals.create_order(
                         self.exchange_manager,
                         emit_trading_signals and signals.should_emit_trading_signal(self.exchange_manager),
-                        current_order)
+                        current_order,
+                        wait_for_creation=wait_for_creation,
+                        creation_timeout=creation_timeout
+                    )
                 created_orders.append(order)
         return created_orders
 
     async def withdraw(self, amount, currency):
         """
         Removes the given amount from the portfolio. Only works in simulated portfolios
         :param amount: the amount to withdraw
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/unknown_order.pxd`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+cimport octobot_trading.personal_data.orders.order as order_class
 
-cimport octobot_trading.exchanges.traders.trader as trader
-
-cdef class TraderSimulator(trader.Trader):
+cdef class UnknownOrder(order_class.Order):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/traders/trader_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/traders/trader_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,20 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_trading.exchanges.types.future_exchange cimport (
-    FutureExchange,
-)
-from octobot_trading.exchanges.types.margin_exchange cimport (
-    MarginExchange,
-)
-from octobot_trading.exchanges.types.spot_exchange cimport (
-    SpotExchange,
-)
-from octobot_trading.exchanges.types.websocket_exchange cimport (
+from octobot_trading.exchanges.types import websocket_exchange
+from octobot_trading.exchanges.types.websocket_exchange import (
     WebSocketExchange,
 )
+from octobot_trading.exchanges.types import rest_exchange
+from octobot_trading.exchanges.types.rest_exchange import (
+    RestExchange,
+)
 
 __all__ = [
-    "FutureExchange",
     "WebSocketExchange",
-    "MarginExchange",
-    "SpotExchange",
+    "RestExchange",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/future_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/rest_exchange.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -13,34 +13,31 @@
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 cimport octobot_trading.exchanges.abstract_exchange as abstract_exchange
 cimport octobot_trading.exchange_data.contracts as contracts
 
-cdef class FutureExchange(abstract_exchange.AbstractExchange):
+cdef class RestExchange(abstract_exchange.AbstractExchange):
     cdef public dict pair_contracts
 
+    cpdef object get_adapter_class(self)
     cpdef contracts.FutureContract create_pair_contract(
             self, str pair,
             object current_leverage, object margin_type,
             object contract_type, object position_mode,
             object maintenance_margin_rate,
             object maximum_leverage=*
     )
-    cpdef double calculate_position_value(self, double quantity, double mark_price)
     cpdef contracts.FutureContract get_pair_future_contract(self, str pair)
     cpdef void set_pair_future_contract(self, str pair, contracts.FutureContract future_contract)
     cpdef bint is_linear_symbol(self, str symbol)
     cpdef bint is_inverse_symbol(self, str symbol)
-    cpdef bint is_futures_symbol(self, str symbol)
+    cpdef bint supports_trading_type(self, str symbol, object trading_type)
 
     """
     Parsers
     """
-    cpdef list parse_positions(self, list positions)
-    cpdef dict parse_position(self, dict position_dict)
     cpdef dict parse_funding(self, dict funding_dict, bint from_ticker=*)
     cpdef dict parse_mark_price(self, dict mark_price_dict, bint from_ticker=*)
-    cpdef dict parse_liquidation(self, dict liquidation_dict)
-    cpdef object parse_position_status(self, str status)
-    cpdef object parse_position_side(self, str side, object mode)
+
+    cdef object _create_connector(self, dict config, object exchange_manager, object connector_class)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/margin_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_util.pxd`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,13 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchanges.abstract_exchange as abstract_exchange
 
-cdef class MarginExchange(abstract_exchange.AbstractExchange):
-    pass
+cpdef object parse_position_status(dict raw_position)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/margin_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/open_position_state.pxd`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -9,12 +10,11 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_trading.exchanges.abstract_exchange as abstract_exchange
+cimport octobot_trading.personal_data.positions.position_state as position_state
 
-
-class MarginExchange(abstract_exchange.AbstractExchange):
-    pass
+cdef class OpenPositionState(position_state.PositionState):
+    cdef bint has_terminated
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/spot_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchanges.abstract_exchange as abstract_exchange
+import octobot_trading.enums as enums
 
-cdef class SpotExchange(abstract_exchange.AbstractExchange):
-    pass
+
+def parse_position_status(raw_position):
+    try:
+        return enums.PositionStatus(raw_position[enums.ExchangeConstantsPositionColumns.STATUS.value])
+    except KeyError:
+        return None
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/spot_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/adapters/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,12 +9,17 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_trading.exchanges.abstract_exchange as abstract_exchange
 
 
-class SpotExchange(abstract_exchange.AbstractExchange):
-    pass
+from octobot_trading.exchanges.adapters import abstract_adapter
+from octobot_trading.exchanges.adapters.abstract_adapter import (
+    AbstractAdapter,
+)
+
+__all__ = [
+    "AbstractAdapter",
+]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/websocket_exchange.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/websocket_exchange.pxd`

 * *Files 8% similar despite different names*

```diff
@@ -31,11 +31,10 @@
 
     cdef public bint is_websocket_running
     cdef public bint is_websocket_authenticated
 
     cdef public object restart_task
 
     # public
-    cpdef bint is_handling(self, str feed_name)
     cpdef bint is_feed_available(self, object feed)
     cpdef bint is_feed_requiring_init(self, object feed)
     cpdef void create_feeds(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/types/websocket_exchange.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/types/websocket_exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #  License along with this library.
 import asyncio
 import concurrent.futures as futures
 
 import octobot_commons.thread_util as thread_util
 import octobot_trading.enums
 import octobot_trading.exchanges.abstract_websocket_exchange as abstract_websocket
-import octobot_trading.exchanges.connectors.abstract_websocket_connector as abstract_websocket_connector
 
 
 class WebSocketExchange(abstract_websocket.AbstractWebsocketExchange):
     def __init__(self, config, exchange_manager):
         super().__init__(config, exchange_manager)
         self.exchange_manager = exchange_manager
         self.exchange_name = exchange_manager.exchange_name
@@ -41,22 +40,30 @@
         self.handled_feeds = {}
 
         self.is_websocket_running = False
         self.is_websocket_authenticated = False
 
         self.restart_task = None
 
+    @classmethod
+    def get_exchange_connector_class(cls, exchange_manager):
+        raise NotImplementedError("get_exchange_connector_class is not implemented")
+
+    def create_feeds(self):
+        raise NotImplementedError("create_feeds is not implemented")
+
     async def init_websocket(self, time_frames, trader_pairs, tentacles_setup_config):
         self.websocket_connector = self.get_exchange_connector_class(self.exchange_manager)
         self.pairs = trader_pairs
         self.time_frames = time_frames
 
         if self.pairs:
             # unauthenticated
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.TRADES)
+            await self.add_feed(octobot_trading.enums.WebsocketFeeds.L1_BOOK)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.L2_BOOK)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.L3_BOOK)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.BOOK_DELTA)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.BOOK_TICKER)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.OPEN_INTEREST)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.MINI_TICKER)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.TICKER)
@@ -71,14 +78,17 @@
                 await self.add_feed(octobot_trading.enums.WebsocketFeeds.KLINE)
 
             # authenticated
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.POSITION)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.PORTFOLIO)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.TRADE)
             await self.add_feed(octobot_trading.enums.WebsocketFeeds.ORDERS)
+            await self.add_feed(octobot_trading.enums.WebsocketFeeds.CREATE_ORDER)
+            await self.add_feed(octobot_trading.enums.WebsocketFeeds.CANCEL_ORDER)
+            await self.add_feed(octobot_trading.enums.WebsocketFeeds.LEDGER)
 
             # ensure feeds are added
             self.create_feeds()
         else:
             self.logger.warning(f"{self.exchange_manager.exchange_name.title()}'s "
                                 f"websocket has no symbol to feed")
 
@@ -105,88 +115,90 @@
     def get_name(cls):
         return cls.__name__
 
     @classmethod
     def has_name(cls, exchange_manager: object) -> bool:  # pylint: disable=arguments-renamed
         return cls.get_exchange_connector_class(exchange_manager) is not None
 
-    def create_feeds(self):
-        raise NotImplementedError("create_feeds is not implemented")
-
-    @classmethod
-    def get_exchange_connector_class(cls, exchange_manager: object):
-        raise NotImplementedError("get_exchange_connector_class is not implemented")
-
-    @staticmethod
-    def get_websocket_client(config, exchange_manager):
-        raise NotImplementedError("get_websocket_client is not implemented")
-
-    @classmethod
-    def get_class_method_name_to_get_compatible_websocket(cls, exchange_manager: object) -> str:
-        if exchange_manager.is_future:
-            return abstract_websocket_connector.AbstractWebsocketConnector.is_handling_future.__name__
-        if exchange_manager.is_margin:
-            return abstract_websocket_connector.AbstractWebsocketConnector.is_handling_margin.__name__
-        return abstract_websocket_connector.AbstractWebsocketConnector.is_handling_spot.__name__
-
     async def start_sockets(self):
         if any(self.handled_feeds.values() and self.websocket_connectors):
             try:
                 self.websocket_connectors_executors = futures.ThreadPoolExecutor(
                     max_workers=len(self.websocket_connectors),
-                    thread_name_prefix=f"{self.get_name()}-{self.exchange_name}-pool-executor")
+                    thread_name_prefix=f"{self.get_name()}-{self.exchange_name}-pool-executor"
+                )
 
                 self.websocket_connectors_tasks = [
                     asyncio.get_event_loop().run_in_executor(self.websocket_connectors_executors, websocket.start)
-                    for websocket in self.websocket_connectors]
+                    for websocket in self.websocket_connectors
+                ]
 
                 self.is_websocket_running = True
             except ValueError as e:
                 self.logger.error(f"Failed to start websocket on {self.exchange_name} : {e}")
 
         if self.websocket_connectors and not self.is_websocket_running:
             self.logger.debug(f"{self.exchange_manager.exchange_name.title()}'s "
                               f"websocket is not handling anything, it will not be started.")
 
     async def wait_sockets(self):
         await asyncio.wait(self.websocket_connectors_tasks)
 
+    def _supports_live_pair_addition(self):
+        for websocket in self.websocket_connectors:
+            if not websocket.SUPPORTS_LIVE_PAIR_ADDITION:
+                return False
+        return True
+
+    async def updated_followed_pairs(self):
+        for websocket in self.websocket_connectors:
+            websocket.update_followed_pairs()
+
     async def _inner_close_and_restart_sockets(self, debounce_duration):
         # asyncio.sleep to make it easily cancellable to reschedule later calls
         await asyncio.sleep(debounce_duration)
         for websocket in self.websocket_connectors:
             await websocket.reset()
 
-    async def close_and_restart_sockets(self, debounce_duration=0):
+    async def handle_new_pairs(self, debounce_duration=0):
+        if self._supports_live_pair_addition():
+            await self.updated_followed_pairs()
+        else:
+            await self._close_and_restart_sockets(debounce_duration=debounce_duration)
+
+    async def _close_and_restart_sockets(self, debounce_duration=0):
         if self.restart_task is not None and not self.restart_task.done():
             self.restart_task.cancel()
         self.restart_task = asyncio.create_task(self._inner_close_and_restart_sockets(debounce_duration))
 
     async def stop_sockets(self):
+        """
+        Stops the websocket. Can be restarted
+        """
         try:
             for websocket in self.websocket_connectors:
                 await websocket.stop()
         except Exception as e:
             self.logger.error(f"Error when stopping sockets : {e}")
 
     async def close_sockets(self):
+        """
+        Closes the websocket. Can't be restarted
+        """
         try:
             for websocket in self.websocket_connectors:
                 await websocket.close()
         except Exception as e:
             self.logger.error(f"Error when closing sockets : {e}")
         for websocket_task in self.websocket_connectors_tasks:
             websocket_task.cancel()
         thread_util.stop_thread_pool_executor_non_gracefully(self.websocket_connectors_executors)
         self.websocket_connectors_executors = None
 
     def add_pairs(self, pairs, watching_only=False):
         for websocket in self.websocket_connectors:
             websocket.add_pairs(pairs, watching_only=watching_only)
 
-    def is_handling(self, feed_name):
-        return feed_name in self.handled_feeds[feed_name] and self.handled_feeds[feed_name]
-
     def clear(self):
         super(WebSocketExchange, self).clear()
         for connector in self.websocket_connectors:
             connector.clear()
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,45 +10,51 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_trading.exchanges.util cimport exchange_market_status_fixer
-from octobot_trading.exchanges.util.exchange_market_status_fixer cimport (
+from octobot_trading.exchanges.util import exchange_market_status_fixer
+from octobot_trading.exchanges.util.exchange_market_status_fixer import (
     ExchangeMarketStatusFixer,
     is_ms_valid,
 )
-from octobot_trading.exchanges.util cimport exchange_util
-from octobot_trading.exchanges.util.exchange_util cimport (
-    get_margin_exchange_class,
-    get_future_exchange_class,
-    get_spot_exchange_class,
+from octobot_trading.exchanges.util import exchange_util
+from octobot_trading.exchanges.util.exchange_util import (
+    get_rest_exchange_class,
     get_order_side,
+    log_time_sync_error,
+    get_partners_explanation_message,
+    is_compatible_account,
+    get_historical_ohlcv,
     get_exchange_type,
     get_default_exchange_type,
     get_supported_exchange_types,
     get_exchange_class_from_name,
 )
-from octobot_trading.exchanges.util cimport websockets_util
-from octobot_trading.exchanges.util.websockets_util cimport (
+from octobot_trading.exchanges.util import websockets_util
+from octobot_trading.exchanges.util.websockets_util import (
     force_disable_web_socket,
     check_web_socket_config,
     search_websocket_class,
+    supports_websocket,
 )
 
 __all__ = [
     "ExchangeMarketStatusFixer",
     "is_ms_valid",
-    "get_margin_exchange_class",
-    "get_future_exchange_class",
-    "get_spot_exchange_class",
+    "get_rest_exchange_class",
     "get_order_side",
-    "force_disable_web_socket",
-    "check_web_socket_config",
-    "search_websocket_class",
+    "log_time_sync_error",
+    "get_partners_explanation_message",
+    "is_compatible_account",
+    "get_historical_ohlcv",
     "get_exchange_type",
     "get_default_exchange_type",
     "get_supported_exchange_types",
     "get_exchange_class_from_name",
+    "force_disable_web_socket",
+    "check_web_socket_config",
+    "search_websocket_class",
+    "supports_websocket",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/exchange_market_status_fixer.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_market_status_fixer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/exchange_market_status_fixer.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_market_status_fixer.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 
     if not is_ms_valid(
             market_limit[Ecmsc.LIMITS_COST.value][Ecmsc.LIMITS_COST_MIN.value]):
         market_limit[Ecmsc.LIMITS_COST.value][Ecmsc.LIMITS_COST_MIN.value] = 0
 
 
 class ExchangeMarketStatusFixer:
+    # todo move to connector/ccxt
     LIMIT_PRICE_MULTIPLIER = 1000
     LIMIT_COST_MULTIPLIER = 1
 
     # calculated from popular exchanges
     LIMIT_AMOUNT_MAX_SUP_ATTENUATION = 6  # when log(price, 10) >= 0
     LIMIT_AMOUNT_MAX_MINUS_3_ATTENUATION = 1  # when log(price, 10) > -3
     LIMIT_AMOUNT_MIN_ATTENUATION = 3  # when log(price, 10) < 0
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/exchange_util.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/exchange_util.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-cpdef object get_margin_exchange_class(str exchange_name, object tentacles_setup_config)
-cpdef object get_future_exchange_class(str exchange_name, object tentacles_setup_config)
-cpdef object get_spot_exchange_class(str exchange_name, object tentacles_setup_config)
+cpdef object get_rest_exchange_class(str exchange_name, object tentacles_setup_config)
 cpdef str get_order_side(object order_type)
 cpdef void log_time_sync_error(object logger, str exchange_name, object error, str details)
 cpdef str get_partners_explanation_message()
 cpdef object get_exchange_type(object exchange_manager_instance)
 cpdef str get_default_exchange_type(str exchange_name)
 cpdef list get_supported_exchange_types(str exchange_name)
 cpdef object get_exchange_class_from_name(object exchange_parent_class,
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/websockets_util.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/websockets_util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/exchanges/util/websockets_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/util/websockets_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/modes/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/abstract_trading_mode.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/abstract_trading_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,15 @@
             self.set_default_config()
         await self.load_and_save_user_inputs(bot_id)
         for element in self.consumers + self.producers:
             if isinstance(element, (abstract_mode_consumer.AbstractTradingModeConsumer,
                                     abstract_mode_producer.AbstractTradingModeProducer)):
                 element.on_reload_config()
                 await element.init_user_inputs(False)
+        self.logger.debug(f"Using config: {self.trading_config}")
 
     def get_local_config(self):
         return self.trading_config
 
     @classmethod
     def create_local_instance(cls, config, tentacles_setup_config, tentacle_config):
         return modes_factory.create_temporary_trading_mode_with_local_config(
@@ -341,18 +342,21 @@
 
     @contextlib.asynccontextmanager
     async def remote_signal_publisher(self, symbol: str):
         async with signals.remote_signal_publisher(self.exchange_manager, symbol, self.should_emit_trading_signal()) \
              as signal_builder:
             yield signal_builder
 
-    async def create_order(self, order, loaded: bool = False, params: dict = None, pre_init_callback=None):
+    async def create_order(self, order, loaded: bool = False, params: dict = None,
+                           wait_for_creation=True,
+                           creation_timeout=constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT):
         return await signals.create_order(
             self.exchange_manager, self.should_emit_trading_signal(), order,
-            loaded=loaded, params=params, pre_init_callback=pre_init_callback
+            loaded=loaded, params=params,
+            wait_for_creation=wait_for_creation, creation_timeout=creation_timeout
         )
 
     async def cancel_order(self, order, ignored_order: object = None) -> bool:
         return await signals.cancel_order(
             self.exchange_manager, self.should_emit_trading_signal(), order,
             ignored_order=ignored_order
         )
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_consumer.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_consumer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_consumer.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_producer.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_producer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/abstract_mode_producer.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/abstract_mode_producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         common_enums.ActivationTopics.FULL_CANDLES.value:
             channels_name.OctoBotTradingChannelsName.OHLCV_CHANNEL.value,
         common_enums.ActivationTopics.IN_CONSTRUCTION_CANDLES.value:
             channels_name.OctoBotTradingChannelsName.KLINE_CHANNEL.value,
         common_enums.ActivationTopics.EVALUATION_CYCLE.value:
             channels_name.OctoBotEvaluatorsChannelsName.MATRIX_CHANNEL.value,
     }
+    CONFIG_INIT_TIMEOUT = 30
 
     def __init__(self, channel, config, trading_mode, exchange_manager):
         super().__init__(channel)
         # the trading mode instance logger
         self.logger = logging.get_logger(self.__class__.__name__)
 
         # the trading mode instance
@@ -369,22 +370,27 @@
                 databases.RunDatabasesProvider.instance().get_run_db(self.trading_mode.bot_id)
             )
         await self._register_and_apply_required_user_inputs(
             script_keywords.get_base_context(self.trading_mode, init_call=True)
         )
 
     async def _register_and_apply_required_user_inputs(self, context):
-        if context.exchange_manager.is_future:
-            await script_keywords.set_leverage(context, await script_keywords.user_select_leverage(context))
-
         if self.trading_mode.ALLOW_CUSTOM_TRIGGER_SOURCE:
             # register activating topics user input
             activation_topic_values = [
                 common_enums.ActivationTopics.EVALUATION_CYCLE.value,
                 common_enums.ActivationTopics.FULL_CANDLES.value,
                 common_enums.ActivationTopics.IN_CONSTRUCTION_CANDLES.value
             ]
             await script_keywords.get_activation_topics(
                 context,
                 common_enums.ActivationTopics.EVALUATION_CYCLE.value,
                 activation_topic_values
             )
+        await self._apply_exchange_side_config(context)
+
+    async def _apply_exchange_side_config(self, context):
+        # can be slow, call in a task if necessary
+        if context.exchange_manager.is_future:
+            await util.wait_for_topic_init(self.exchange_manager, self.CONFIG_INIT_TIMEOUT,
+                                           common_enums.InitializationEventExchangeTopics.CONTRACTS.value)
+            await script_keywords.set_leverage(context, await script_keywords.user_select_leverage(context))
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/mode.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/mode.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/channel/mode.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/channel/mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/mode_config.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/mode_config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/modes_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/modes/modes_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/modes_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/modes_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/modes_util.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/modes/modes_util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/modes_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/modes_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/amount.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/configuration.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,17 +45,14 @@
         side = None
         try:
             await ctx.exchange_manager.trader.set_leverage(ctx.symbol, side, decimal.Decimal(str(leverage)))
         except errors.ContractExistsError as e:
             ctx.logger.debug(str(e))
         except NotImplementedError as e:
             ctx.logger.exception(e, True, str(e))
-        except AttributeError:
-            # TODO remove this except when bybit tentacle is up
-            ctx.logger.warning("TODO: rebase tentacles when bybit exchange is up")
         except Exception as e:
             ctx.logger.exception(e, True, str(e))
 
 
 async def set_partial_take_profit_stop_loss(ctx, tp_sl_mode=enums.TakeProfitStopLossMode.PARTIAL.value):
     if ctx.exchange_manager.is_future:
         await ctx.exchange_manager.trader.set_symbol_take_profit_stop_loss_mode(
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/run_persistence.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/trading_signals.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/basic_keywords/user_inputs.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/context_management.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/context_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/dsl/quantity.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/dsl/quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/script_keywords/dsl/values.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/script_keywords/dsl/values.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/scripted_trading_mode/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/scripted_trading_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py` & `OctoBot-Trading-2.3.7/octobot_trading/modes/scripted_trading_mode/abstract_scripted_trading_mode.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/octobot_channel_consumer.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/octobot_channel_consumer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/octobot_channel_consumer.py` & `OctoBot-Trading-2.3.7/octobot_trading/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     get_fees_for_currency,
     parse_raw_fees,
     parse_order_status,
     parse_is_cancelled,
     parse_is_open,
     get_pnl_transaction_source_from_order,
     is_stop_order,
+    get_trade_order_type,
     create_as_chained_order,
     ensure_orders_relevancy,
     get_order_quantity_currency,
     get_order_size_portfolio_percent,
     generate_order_id,
     is_associated_pending_order,
     apply_pending_order_from_created_order,
@@ -78,14 +79,15 @@
     OrdersUpdaterSimulator,
     CloseOrderState,
     CancelOrderState,
     OpenOrderState,
     create_order_state,
     FillOrderState,
     PendingCreationOrderState,
+    PendingCreationChainedOrderState,
     UnknownOrder,
     MarketOrder,
     SellMarketOrder,
     BuyMarketOrder,
     BuyLimitOrder,
     SellLimitOrder,
     LimitOrder,
@@ -224,14 +226,15 @@
     "get_fees_for_currency",
     "parse_raw_fees",
     "parse_order_status",
     "parse_is_cancelled",
     "parse_is_open",
     "get_pnl_transaction_source_from_order",
     "is_stop_order",
+    "get_trade_order_type",
     "create_as_chained_order",
     "ensure_orders_relevancy",
     "get_order_quantity_currency",
     "get_order_size_portfolio_percent",
     "generate_order_id",
     "is_associated_pending_order",
     "apply_pending_order_from_created_order",
@@ -269,14 +272,15 @@
     "OrdersUpdaterSimulator",
     "CloseOrderState",
     "CancelOrderState",
     "OpenOrderState",
     "create_order_state",
     "FillOrderState",
     "PendingCreationOrderState",
+    "PendingCreationChainedOrderState",
     "UnknownOrder",
     "MarketOrder",
     "SellMarketOrder",
     "BuyMarketOrder",
     "BuyLimitOrder",
     "SellLimitOrder",
     "LimitOrder",
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/exchange_personal_data.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/exchange_personal_data.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/exchange_personal_data.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/exchange_personal_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from octobot_trading.personal_data.orders.states import (
     CloseOrderState,
     CancelOrderState,
     OpenOrderState,
     create_order_state,
     FillOrderState,
     PendingCreationOrderState,
+    PendingCreationChainedOrderState,
 )
 from octobot_trading.personal_data.orders import channel
 from octobot_trading.personal_data.orders.channel import (
     OrdersProducer,
     OrdersChannel,
     OrdersUpdater,
     OrdersUpdaterSimulator,
@@ -81,14 +82,15 @@
     parse_order_status,
     parse_is_cancelled,
     parse_is_open,
     get_up_to_date_price,
     get_pre_order_data,
     get_pnl_transaction_source_from_order,
     is_stop_order,
+    get_trade_order_type,
     create_as_chained_order,
     is_associated_pending_order,
     apply_pending_order_from_created_order,
     ensure_orders_relevancy,
     get_order_quantity_currency,
     get_order_size_portfolio_percent,
     generate_order_id,
@@ -179,14 +181,15 @@
     "OrdersUpdaterSimulator",
     "CloseOrderState",
     "CancelOrderState",
     "OpenOrderState",
     "create_order_state",
     "FillOrderState",
     "PendingCreationOrderState",
+    "PendingCreationChainedOrderState",
     "UnknownOrder",
     "MarketOrder",
     "SellMarketOrder",
     "BuyMarketOrder",
     "BuyLimitOrder",
     "SellLimitOrder",
     "LimitOrder",
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,24 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+
+"""
+Handles balance changes
+"""
 cimport octobot_trading.exchange_channel as exchanges_channel
 
-cdef class OrdersProducer(exchanges_channel.ExchangeChannelProducer):
+cdef class BalanceProducer(exchanges_channel.ExchangeChannelProducer):
+    pass
+
+cdef class BalanceChannel(exchanges_channel.ExchangeChannel):
+    pass
+
+cdef class BalanceProfitabilityProducer(exchanges_channel.ExchangeChannelProducer):
     pass
 
-cdef class OrdersChannel(exchanges_channel.ExchangeChannel):
+cdef class BalanceProfitabilityChannel(exchanges_channel.ExchangeChannel):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import asyncio
 
 import octobot_commons.async_job as async_job
 import octobot_commons.tree as commons_tree
 import octobot_commons.enums as commons_enums
+import octobot_commons.constants as commons_constants
 
 import octobot_trading.errors as errors
 import octobot_trading.personal_data.orders.channel.orders as orders_channel
 import octobot_trading.constants as constants
 
 
 class OrdersUpdater(orders_channel.OrdersProducer):
@@ -34,14 +35,15 @@
     CHANNEL_NAME = constants.ORDERS_CHANNEL
     ORDERS_UPDATE_LIMIT = 200
     ORDERS_STARTING_REFRESH_TIME = 10
     OPEN_ORDER_REFRESH_TIME = 7
     CLOSE_ORDER_REFRESH_TIME = 81
     TIME_BETWEEN_ORDERS_REFRESH = 2
     DEPENDENCIES_TIMEOUT = 30
+    OPEN_ORDER_INITIAL_FETCH_GIVE_UP_TIMEOUT = 3 * commons_constants.MINUTE_TO_SECONDS
 
     def __init__(self, channel):
         super().__init__(channel)
 
         self._is_initialized_event_set = False
         # create async jobs
         self.open_orders_job = async_job.AsyncJob(self._open_orders_fetch_and_push,
@@ -70,58 +72,69 @@
                     commons_tree.get_exchange_path(
                         self.channel.exchange_manager.exchange_name,
                         commons_enums.InitializationEventExchangeTopics.POSITIONS.value
                     ),
                 ],
                 self.DEPENDENCIES_TIMEOUT
             )
-            await self.fetch_and_push(is_from_bot=False)
+            await self.fetch_and_push(is_from_bot=False, retry_till_success=True)
         except errors.NotSupported:
             self.logger.error(f"{self.channel.exchange_manager.exchange_name} is not supporting open orders updates")
             await self.pause()
         except Exception as e:
             self.logger.exception(e, True, f"Fail to initialize orders : {e}")
         finally:
-            self.channel.exchange_manager.exchange_personal_data.orders_manager.are_exchange_orders_initialized = True
+            if self.channel is not None:
+                self.channel.exchange_manager.exchange_personal_data.orders_manager.are_exchange_orders_initialized = True
 
     async def start(self) -> None:
         """
         Start updater jobs
         """
         await self.initialize()
         await asyncio.sleep(self.ORDERS_STARTING_REFRESH_TIME)
         await self.open_orders_job.run()
         # await self.closed_orders_job.run()
 
-    async def fetch_and_push(self, is_from_bot=True, limit=ORDERS_UPDATE_LIMIT):
+    async def fetch_and_push(self, is_from_bot=True, limit=ORDERS_UPDATE_LIMIT, retry_till_success=False):
         """
         Update open and closed orders from exchange
         :param is_from_bot: True if the order was created by OctoBot
         :param limit: the exchange request orders count limit
+        :param retry_till_success: retry request till it works. Should be rarely used as it might take some time
         """
         # should not raise: open orders are necessary
-        await self._open_orders_fetch_and_push(is_from_bot=is_from_bot, limit=limit)
+        await self._open_orders_fetch_and_push(is_from_bot=is_from_bot, limit=limit,
+                                               retry_till_success=retry_till_success)
         await asyncio.sleep(self.TIME_BETWEEN_ORDERS_REFRESH)
         try:
             # can raise, closed orders are not critical data
             await self._closed_orders_fetch_and_push(limit=limit)
         except errors.NotSupported:
             self.logger.debug(f"{self.channel.exchange_manager.exchange_name} is not supporting closed orders updates")
 
-    async def _open_orders_fetch_and_push(self, is_from_bot=True, limit=ORDERS_UPDATE_LIMIT):
+    async def _open_orders_fetch_and_push(self, is_from_bot=True, limit=ORDERS_UPDATE_LIMIT, retry_till_success=False):
         """
         Update open orders from exchange
         :param is_from_bot: True if the order was created by OctoBot
         :param limit: the exchange request orders count limit
+        :param retry_till_success: retry request till it works. Should be rarely used as it might take some time
         """
         for symbol in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
-            open_orders: list = await self.channel.exchange_manager.exchange.get_open_orders(symbol=symbol, limit=limit)
+            if retry_till_success:
+                open_orders: list = await self.channel.exchange_manager.exchange.retry_till_success(
+                    self.OPEN_ORDER_INITIAL_FETCH_GIVE_UP_TIMEOUT,
+                    self.channel.exchange_manager.exchange.get_open_orders, symbol=symbol, limit=limit
+                )
+            else:
+                open_orders: list = await self.channel.exchange_manager.exchange.get_open_orders(
+                    symbol=symbol, limit=limit
+                )
             if open_orders:
-                await self.push(list(map(self.channel.exchange_manager.exchange.clean_order, open_orders)),
-                                is_from_bot=is_from_bot)
+                await self.push(open_orders, is_from_bot=is_from_bot)
             else:
                 await self.handle_post_open_order_update(symbol, open_orders, False)
             if not self._is_initialized_event_set:
                 self._set_initialized_event(symbol)
         self._is_initialized_event_set = True
 
     def _set_initialized_event(self, symbol):
@@ -140,16 +153,15 @@
         :param limit: the exchange request orders count limit
         """
         for symbol in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
             close_orders: list = await self.channel.exchange_manager.exchange.get_closed_orders(
                 symbol=symbol, limit=limit)
 
             if close_orders:
-                await self.push(list(map(self.channel.exchange_manager.exchange.clean_order, close_orders)),
-                                are_closed=True)
+                await self.push(close_orders, are_closed=True)
 
     async def update_order_from_exchange(self, order,
                                          should_notify=False,
                                          wait_for_refresh=False,
                                          force_job_execution=False,
                                          create_order_producer_if_missing=True):
         """
@@ -173,15 +185,14 @@
         :return: True if the order was updated
         """
         exchange_name = order.exchange_manager.exchange_name if order.exchange_manager else "cleared order's exchange"
         self.logger.debug(f"Requested update for {order} on {exchange_name}")
         raw_order = await self.channel.exchange_manager.exchange.get_order(order.order_id, order.symbol)
 
         if raw_order is not None:
-            raw_order = self.channel.exchange_manager.exchange.clean_order(raw_order)
             self.logger.debug(f"Received update for {order} on {exchange_name}: {raw_order}")
 
             await self.channel.exchange_manager.exchange_personal_data.handle_order_update_from_raw(
                 order.order_id, raw_order, should_notify=should_notify
             )
 
     async def stop(self) -> None:
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/close_order_state.pxd`

 * *Files 11% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.orders.channel.orders_updater as orders_updater
+cimport octobot_trading.personal_data.orders.order_state as order_state
 
-cdef class OrdersUpdaterSimulator(orders_updater.OrdersUpdater):
+cdef class CloseOrderState(order_state.OrderState):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/channel/orders_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/decimal_order_adapter.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/decimal_order_adapter.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/decimal_order_adapter.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/groups/one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,25 +136,15 @@
 
         if symbol and self.symbol != symbol:
             self.currency, self.market = self.exchange_manager.get_exchange_quote_and_base(symbol)
             self.symbol = symbol
 
         if quantity_currency is None:
             if self.quantity_currency is None and self.symbol is not None:
-                try:
-                    side = self.get_position_side(
-                        self.exchange_manager.exchange.get_pair_future_contract(self.symbol)
-                    ) if self.exchange_manager.is_future else None
-                    self.quantity_currency = order_util.get_order_quantity_currency(
-                        self.exchange_manager,
-                        self.symbol,
-                        side
-                    )
-                except (errors.InvalidPositionSide, errors.ContractExistsError) as e:
-                    logging.get_logger(self.get_logger_name()).warning(f"Can't infer quantity_currency: {e}")
+                self.quantity_currency = order_util.get_order_quantity_currency(self.exchange_manager, self.symbol)
         else:
             self.quantity_currency = quantity_currency
 
         if status and self.status != status:
             # ensure the order status is compatible with the state to avoid exchange sync issues
             if self.state is None or self.state.allows_new_status(status):
                 self.status = status
@@ -351,19 +341,29 @@
         try:
             yield
         except errors.InvalidOrderState as exc:
             logging.get_logger(self.get_logger_name()).exception(exc, True, f"Error when creating order state: {exc}")
 
     async def on_pending_creation(self, is_from_exchange_data=False):
         with self.order_state_creation():
-            self.state = orders_states.PendingCreationOrderState(self, is_from_exchange_data=is_from_exchange_data)
+            state_class = orders_states.PendingCreationChainedOrderState if self.is_waiting_for_chained_trigger \
+                else orders_states.PendingCreationOrderState
+            self.state = state_class(self, is_from_exchange_data=is_from_exchange_data)
             await self.state.initialize()
 
     async def on_open(self, force_open=False, is_from_exchange_data=False):
         with self.order_state_creation():
+            if isinstance(self.state, orders_states.PendingCreationOrderState):
+                await self.state.trigger_terminate()
+            if isinstance(self.state, orders_states.OpenOrderState):
+                if not self.state.is_initialized:
+                    logging.get_logger(self.get_logger_name()).error(f"on_open called with existing "
+                                                                     f"uninitialized OpenOrderState.")
+                # state has already been created and initialized
+                return
             self.state = orders_states.OpenOrderState(self, is_from_exchange_data=is_from_exchange_data)
             await self.state.initialize(forced=force_open)
 
     async def on_fill(self, force_fill=False, is_from_exchange_data=False):
         logging.get_logger(self.get_logger_name()).debug(f"on_fill triggered for {self}")
         if self.is_open() and not self.is_refreshing():
             with self.order_state_creation():
@@ -529,14 +529,24 @@
             reduce_only=raw_order.get(enums.ExchangeConstantsOrderColumns.REDUCE_ONLY.value, False)
         )
 
     async def update_from_order(self, other_order):
         self.is_synchronized_with_exchange = other_order.is_synchronized_with_exchange
         self.is_from_this_octobot = other_order.is_from_this_octobot
 
+        self.origin_quantity = other_order.origin_quantity
+        self.origin_price = other_order.origin_price
+        self.origin_stop_price = other_order.origin_stop_price
+        self.symbol = other_order.symbol
+        self.currency = other_order.currency
+        self.market = other_order.market
+        self.quantity_currency = other_order.quantity_currency
+        self.taker_or_maker = other_order.taker_or_maker
+        self.side = other_order.side
+
         self.order_id = other_order.order_id
         self.status = other_order.status
 
         self.filled_quantity = other_order.filled_quantity
         self.filled_price = other_order.filled_price
         self.fee = other_order.fee
         self.fees_currency_side = other_order.fees_currency_side
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_adapter.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_adapter.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_adapter.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_factory.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  License along with this library.
 
 cpdef object create_order_from_raw(object trader,
                                    dict raw_order)
 
 cpdef object create_order_instance_from_raw(object trader,
                                             dict raw_order,
-                                            bint force_open= *)
+                                            bint force_open_or_pending_creation= *)
 
 cpdef object create_order_from_type(object trader,
                                     object order_type,
                                     object side= *)
 
 cpdef object create_order_instance(object trader,
                                    object order_type,
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 
 
 def create_order_from_raw(trader, raw_order):
     _, order_type = personal_data.parse_order_type(raw_order)
     return create_order_from_type(trader, order_type)
 
 
-def create_order_instance_from_raw(trader, raw_order, force_open=False):
+def create_order_instance_from_raw(trader, raw_order, force_open_or_pending_creation=False):
     order = create_order_from_raw(trader, raw_order)
     order.update_from_raw(raw_order)
-    if force_open:
+    if force_open_or_pending_creation \
+            and order.status not in (enums.OrderStatus.OPEN, enums.OrderStatus.PENDING_CREATION):
         order.status = enums.OrderStatus.OPEN
     return order
 
 
 def create_order_from_type(trader, order_type, side=None):
     if side is None:
         return personal_data.TraderOrderTypeClasses[order_type](trader)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_group.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_group.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_group.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_state.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_util.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_util.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 cpdef object parse_is_cancelled(dict raw_order)
 cpdef object parse_is_open(dict raw_order)
 cpdef object get_max_order_quantity_for_price(object position, object available_quantity,
                                               object price, object side, str symbol)
 cpdef object get_pnl_transaction_source_from_order(object order)
 cpdef bint is_stop_order(object order_type)
 cpdef bint is_associated_pending_order(object pending_order, object created_order)
-cpdef object get_order_quantity_currency(object exchange_manager, str symbol, object side)
+cpdef object get_order_quantity_currency(object exchange_manager, str symbol)
 cpdef str generate_order_id()
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/order_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/order_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -264,14 +264,34 @@
 
 
 def is_stop_order(order_type):
     return order_type in [enums.TraderOrderType.STOP_LOSS, enums.TraderOrderType.STOP_LOSS_LIMIT,
                           enums.TraderOrderType.TRAILING_STOP, enums.TraderOrderType.TRAILING_STOP_LIMIT]
 
 
+def get_trade_order_type(order_type: enums.TraderOrderType):
+    if order_type in (enums.TraderOrderType.BUY_MARKET, enums.TraderOrderType.SELL_MARKET):
+        return enums.TradeOrderType.MARKET
+    if order_type in (enums.TraderOrderType.BUY_LIMIT, enums.TraderOrderType.SELL_LIMIT):
+        return enums.TradeOrderType.LIMIT
+    if order_type is enums.TraderOrderType.STOP_LOSS:
+        return enums.TradeOrderType.STOP_LOSS
+    if order_type is enums.TraderOrderType.TRAILING_STOP:
+        return enums.TradeOrderType.TRAILING_STOP
+    if order_type is enums.TraderOrderType.STOP_LOSS_LIMIT:
+        return enums.TradeOrderType.STOP_LOSS_LIMIT
+    if order_type is enums.TraderOrderType.TRAILING_STOP_LIMIT:
+        return enums.TradeOrderType.TRAILING_STOP_LIMIT
+    if order_type is enums.TraderOrderType.TAKE_PROFIT:
+        return enums.TradeOrderType.TAKE_PROFIT
+    if order_type is enums.TraderOrderType.TAKE_PROFIT_LIMIT:
+        return enums.TradeOrderType.TAKE_PROFIT_LIMIT
+    raise ValueError(order_type)
+
+
 async def create_as_chained_order(order):
     order.is_waiting_for_chained_trigger = False
     if not order.trader.simulate and order.has_been_bundled:
         # exchange should have created it already, it is either already fetched or
         # will automatically be fetched at the next update
         # warning: not handling instantly filled bundled orders as there is no easy way to do this
         # TODO: figure out instantly filled bundled orders
@@ -288,19 +308,21 @@
             loaded=False,
             params=order.exchange_creation_params,
             **order.trader_creation_kwargs
         )
 
 
 def is_associated_pending_order(pending_order, created_order):
-    return created_order.symbol == pending_order.symbol and \
-           created_order.origin_quantity == pending_order.origin_quantity and \
-           created_order.origin_price == pending_order.origin_price and \
-           created_order.__class__ is pending_order.__class__ and \
-           created_order.trader is pending_order.trader
+    return created_order.order_id == pending_order.order_id or (
+        created_order.symbol == pending_order.symbol and
+        created_order.origin_quantity == pending_order.origin_quantity and
+        created_order.origin_price == pending_order.origin_price and
+        created_order.__class__ is pending_order.__class__ and
+        created_order.trader is pending_order.trader
+    )
 
 
 async def apply_pending_order_from_created_order(pending_order, created_order, to_be_initialized):
     await pending_order.update_from_order(created_order)
     if to_be_initialized:
         pending_order.is_initialized = False
     logging.get_logger(LOGGER_NAME).debug(f"Updated pending order: {pending_order} using {created_order}")
@@ -343,25 +365,23 @@
         if (exchange_manager.is_trader_simulated or order.is_self_managed()) \
                 and order.is_open() and order.reduce_only:
             await order.trader.cancel_order(order)
             if order.order_group:
                 await order.order_group.on_cancel(order)
 
 
-def get_order_quantity_currency(exchange_manager, symbol, side):
+def get_order_quantity_currency(exchange_manager, symbol):
     try:
-        base, quote = symbol_util.parse_symbol(symbol).base_and_quote()
+        parsed_symbol = symbol_util.parse_symbol(symbol)
+        base, quote = parsed_symbol.base_and_quote()
     except ValueError:
         # symbol that can't be split
         return None
     if exchange_manager.is_future:
-        position = exchange_manager.exchange_personal_data.positions_manager.get_symbol_position(
-            symbol, side
-        )
-        return quote if position.symbol_contract.is_inverse_contract() else base
+        return quote if parsed_symbol.is_inverse() else base
     # always base in spot
     return base
 
 
 async def get_order_size_portfolio_percent(exchange_manager, order_amount, side, symbol):
     current_symbol_holding, current_market_holding, market_quantity, _, _ = \
         await get_pre_order_data(exchange_manager,
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/orders_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/orders_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/orders_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/orders_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/__init__.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -30,20 +30,26 @@
 )
 
 from octobot_trading.personal_data.orders.states cimport pending_creation_order_state
 from octobot_trading.personal_data.orders.states.pending_creation_order_state cimport (
     PendingCreationOrderState
 )
 
+from octobot_trading.personal_data.orders.states cimport pending_creation_chained_order_state
+from octobot_trading.personal_data.orders.states.pending_creation_chained_order_state cimport (
+    PendingCreationChainedOrderState
+)
+
 from octobot_trading.personal_data.orders.states cimport fill_order_state
 from octobot_trading.personal_data.orders.states.fill_order_state cimport (
     FillOrderState
 )
 
 
 __all__ = [
     "CloseOrderState",
     "CancelOrderState",
     "OpenOrderState",
     "PendingCreationOrderState",
+    "PendingCreationChainedOrderState",
     "FillOrderState",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,16 +36,20 @@
 )
 from octobot_trading.personal_data.orders.states.fill_order_state import (
     FillOrderState,
 )
 from octobot_trading.personal_data.orders.states.pending_creation_order_state import (
     PendingCreationOrderState,
 )
+from octobot_trading.personal_data.orders.states.pending_creation_chained_order_state import (
+    PendingCreationChainedOrderState,
+)
 
 __all__ = [
     "CloseOrderState",
     "CancelOrderState",
     "OpenOrderState",
     "create_order_state",
     "FillOrderState",
     "PendingCreationOrderState",
+    "PendingCreationChainedOrderState",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/cancel_order_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/cancel_order_state.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/cancel_order_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/close_order_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/liquidate_position_state.pxd`

 * *Files 10% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.orders.order_state as order_state
+cimport octobot_trading.personal_data.positions.position_state as position_state
 
-cdef class CloseOrderState(order_state.OrderState):
+cdef class LiquidatePositionState(position_state.PositionState):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/close_order_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/close_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/fill_order_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/fill_order_state.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/fill_order_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/open_order_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/open_order_state.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/open_order_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/open_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/order_state_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/order_state_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/order_state_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/order_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/pending_creation_order_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/pending_creation_order_state.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/states/pending_creation_order_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/states/pending_creation_order_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,31 +23,27 @@
         super().__init__(order, is_from_exchange_data)
         self.state = enums.States.PENDING_CREATION
 
     def is_created(self) -> bool:
         """
         :return: True if the Order is created
         """
-        return False
+        # order is created on exchange but not open yet
+        return True
 
     def is_open(self) -> bool:
         """
         :return: True if the Order is considered as open
         """
         return False
 
-    async def update(self) -> None:
-        # nothing to do as no actual order exists yet
-        pass
-
     async def on_refresh_successful(self):
-        # nothing to do as no actual order exists yet
         pass
 
     async def terminate(self):
         """
         Should wait for being replaced by an OpenOrderState or be cancelled
         """
         self.log_event_message(enums.StatesMessages.PENDING_CREATION)
 
     def is_pending(self) -> bool:
-        return False
+        return True
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/buy_limit_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/buy_limit_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/limit_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/spot_asset.pxd`

 * *Files 20% similar despite different names*

```diff
@@ -6,26 +6,17 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General Public License for more details.
+#  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.orders.order as order_class
+cimport octobot_trading.personal_data.portfolios.asset as asset_class
 
-cdef class LimitOrder(order_class.Order):
-    cdef object limit_price_hit_event # object is asyncio.Event
-    cdef object wait_for_hit_event_task # object is asyncio.Task
 
-    cdef bint trigger_above
-    cdef public bint allow_instant_fill
-
-    cpdef str _filled_maker_or_taker(self)
-    # return object to allow exception raising
-    cdef object _create_hit_event(self, object price_time)
-    cdef object _create_hit_task(self)
-    cdef object _reset_events(self, object price_time)
-    cdef object _clear_event_and_tasks(self)
+cdef class SpotAsset(asset_class.Asset):
+    cpdef object update(self, object available=*, object total=*)
+    cpdef object set(self, object available, object total)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/limit_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/sell_limit_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/sell_limit_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/limit/take_profit_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/limit/take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/buy_market_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/buy_market_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/buy_market_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/market_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/sell_market_order.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.orders.order as order_class
+cimport octobot_trading.personal_data.orders.types.market.market_order as market_order
 
-cdef class MarketOrder(order_class.Order):
+cdef class SellMarketOrder(market_order.MarketOrder):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/market_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/sell_market_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.orders.types.market.market_order as market_order
+cimport octobot_trading.personal_data.orders.types.trailing.trailing_stop_order as trailing_stop_order
 
-cdef class SellMarketOrder(market_order.MarketOrder):
+cdef class TrailingStopLimitOrder(trailing_stop_order.TrailingStopOrder):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/market/sell_market_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/market/sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/inverse_position.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.orders.types.trailing.trailing_stop_order as trailing_stop_order
+cimport octobot_trading.personal_data.positions.position as position_class
 
-cdef class TrailingStopLimitOrder(trailing_stop_order.TrailingStopOrder):
+cdef class InversePosition(position_class.Position):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/trailing/trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/unknown_order.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/linear_position.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.orders.order as order_class
+cimport octobot_trading.personal_data.positions.position as position_class
 
-cdef class UnknownOrder(order_class.Order):
+cdef class LinearPosition(position_class.Position):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/orders/types/unknown_order.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/orders/types/unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/asset.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/asset.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/asset.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/future_asset.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/future_asset.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/future_asset.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/margin_asset.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/margin_asset.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/margin_asset.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/spot_asset.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.pxd`

 * *Files 16% similar despite different names*

```diff
@@ -10,13 +10,10 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.portfolios.asset as asset_class
 
 
-cdef class SpotAsset(asset_class.Asset):
-    cpdef object update(self, object available=*, object total=*)
-    cpdef object set(self, object available, object total)
+cpdef object create_historical_asset_value_from_dict_like_object(object historical_asset_class, object asset_values)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/assets/spot_asset.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/assets/spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions.pxd`

 * *Files 22% similar despite different names*

```diff
@@ -10,24 +10,15 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-
-"""
-Handles balance changes
-"""
 cimport octobot_trading.exchange_channel as exchanges_channel
 
-cdef class BalanceProducer(exchanges_channel.ExchangeChannelProducer):
-    pass
-
-cdef class BalanceChannel(exchanges_channel.ExchangeChannel):
-    pass
 
-cdef class BalanceProfitabilityProducer(exchanges_channel.ExchangeChannelProducer):
+cdef class PositionsProducer(exchanges_channel.ExchangeChannelProducer):
     pass
 
-cdef class BalanceProfitabilityChannel(exchanges_channel.ExchangeChannel):
+cdef class PositionsChannel(exchanges_channel.ExchangeChannel):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/channel/balance_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.pxd` & `OctoBot-Trading-2.3.7/tests/api/test_modes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
+import pytest
 
-cpdef object create_historical_asset_value_from_dict_like_object(object historical_asset_class, object asset_values)
+# All test coroutines will be treated as marked.
+pytestmark = pytest.mark.asyncio
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/history/historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_profitability.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_profitability.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_profitability.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_util.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_value_holder.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_value_holder.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/portfolio_value_holder.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/sub_portfolio.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/sub_portfolio.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/sub_portfolio.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/sub_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/future_portfolio.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/future_portfolio.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/future_portfolio.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/margin_portfolio.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/margin_portfolio.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/margin_portfolio.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/spot_portfolio.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/spot_portfolio.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/portfolios/types/spot_portfolio.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/portfolios/types/spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -12,13 +12,12 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 cimport octobot_trading.exchange_channel as exchanges_channel
 
-
-cdef class PositionsProducer(exchanges_channel.ExchangeChannelProducer):
+cdef class TradesProducer(exchanges_channel.ExchangeChannelProducer):
     pass
 
-cdef class PositionsChannel(exchanges_channel.ExchangeChannel):
+cdef class TradesChannel(exchanges_channel.ExchangeChannel):
     pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/fee_transaction.pxd`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General Public License for more details.
+#  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.positions.channel.positions as positions_channel
 
-cimport octobot_commons.async_job as async_job
+cimport octobot_trading.personal_data.transactions.transaction as transaction
 
-cdef class PositionsUpdater(positions_channel.PositionsProducer):
-    cdef public bint should_use_position_per_symbol
+cdef class FeeTransaction(transaction.Transaction):
+    cdef readonly object quantity
+    cdef readonly object funding_rate
 
-    cdef async_job.AsyncJob position_update_job
+    cdef readonly str order_id
 
-    cdef bint _should_run(self)
-    cdef bint _should_push_mark_price(self)
-    cdef bint _has_mark_price_in_position(self)
+    cpdef bint is_funding_fee(self)
+    cpdef bint is_trading_fee(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         for pair in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
             try:
                 await self.channel.exchange_manager.exchange.load_pair_future_contract(pair)
             except NotImplementedError as e:
                 self.logger.debug(f"Can't to load {pair} contract info from exchange: {e}. "
                                   f"This contract will be created from fetched positions.")
             except Exception as e:
+                self.logger.exception(e, False)
                 self.logger.warning(f"Failed to load {pair} contract info : {e}")
 
     async def initialize_positions(self) -> None:
         """
         Initialize data before starting jobs
         """
         try:
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater_simulator.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater_simulator.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/channel/positions_updater_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_state.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_util.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/exchange_simulator_adapter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -11,8 +10,12 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-cpdef object parse_position_status(dict raw_position)
+import octobot_trading.exchanges.adapters as adapters
+
+
+class ExchangeSimulatorAdapter(adapters.AbstractAdapter):
+    pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/position_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/supervisors/__init__.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,9 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-import octobot_trading.enums as enums
 
-
-def parse_position_status(raw_position):
-    try:
-        return enums.PositionStatus(raw_position[enums.ExchangeConstantsPositionColumns.STATUS.value])
-    except KeyError:
-        return None
+__all__ = []
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/positions_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/positions_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/positions_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/liquidate_position_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/position_state_factory.pxd`

 * *Files 17% similar despite different names*

```diff
@@ -10,11 +10,7 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.positions.position_state as position_state
-
-cdef class LiquidatePositionState(position_state.PositionState):
-    pass
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/liquidate_position_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/liquidate_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/open_position_state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,11 +9,23 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.positions.position_state as position_state
 
-cdef class OpenPositionState(position_state.PositionState):
-    cdef bint has_terminated
+from octobot_trading.personal_data.positions.types import linear_position
+from octobot_trading.personal_data.positions.types import inverse_position
+
+from octobot_trading.personal_data.positions.types.linear_position import (
+    LinearPosition,
+)
+
+from octobot_trading.personal_data.positions.types.inverse_position import (
+    InversePosition,
+)
+
+__all__ = [
+    "LinearPosition",
+    "InversePosition",
+]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/open_position_state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/open_position_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/position_state_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/ccxt/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,7 +9,9 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+
+CCXT_INFO = "info"
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/states/position_state_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/states/position_state_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_trading.personal_data.positions.types import linear_position
-from octobot_trading.personal_data.positions.types import inverse_position
-
-from octobot_trading.personal_data.positions.types.linear_position import (
-    LinearPosition,
+from octobot_trading.personal_data.trades.channel import trades
+from octobot_trading.personal_data.trades.channel.trades import (
+    TradesProducer,
+    TradesChannel,
 )
 
-from octobot_trading.personal_data.positions.types.inverse_position import (
-    InversePosition,
+from octobot_trading.personal_data.trades.channel import trades_updater
+from octobot_trading.personal_data.trades.channel.trades_updater import (
+    TradesUpdater,
 )
 
 __all__ = [
-    "LinearPosition",
-    "InversePosition",
+    "TradesProducer",
+    "TradesChannel",
+    "TradesUpdater",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/inverse_position.pxd` & `OctoBot-Trading-2.3.7/tests/api/test_orders.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,11 +9,12 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.positions.position as position_class
 
-cdef class InversePosition(position_class.Position):
-    pass
+import pytest
+
+# All test coroutines will be treated as marked.
+pytestmark = pytest.mark.asyncio
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/inverse_position.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/linear_position.pxd` & `OctoBot-Trading-2.3.7/tests/api/test_portfolio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,11 +9,12 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.personal_data.positions.position as position_class
 
-cdef class LinearPosition(position_class.Position):
-    pass
+import pytest
+
+# All test coroutines will be treated as marked.
+pytestmark = pytest.mark.asyncio
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/positions/types/linear_position.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/positions/types/linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/state.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/state.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/state.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,22 +99,25 @@
         Try to fix the pending state or terminate
         """
         if not self.is_refreshing():
             if self.is_pending() and not await self.should_be_updated():
                 self.log_event_message(enums.StatesMessages.SYNCHRONIZING)
                 await self.synchronize()
             else:
-                try:
-                    async with self.lock:
-                        await self.terminate()
-                finally:
-                    self.on_terminate()
+                await self.trigger_terminate()
         else:
             self.log_event_message(enums.StatesMessages.ALREADY_SYNCHRONIZING)
 
+    async def trigger_terminate(self):
+        try:
+            async with self.lock:
+                await self.terminate()
+        finally:
+            self.on_terminate()
+
     async def synchronize(self, force_synchronization=False, catch_exception=False) -> None:
         """
         Implement the exchange synchronization process
         Should begin by setting the state to REFRESHING
         Should end by :
         - calling terminate if the state is terminated
         - restoring the initial state if nothing has been changed with synchronization or if sync failed
@@ -173,24 +176,27 @@
         raise NotImplementedError("terminate not implemented")
 
     def on_terminate(self) -> None:
         """
         Called after terminate is complete
         """
         self.get_logger().debug(f"{self.__class__.__name__} terminated")
-        self.terminated.set()
+        if not self.terminated.is_set():
+            self.terminated.set()
 
     def __del__(self):
         if not self.terminated.is_set() and self.terminated._waiters:
             self.get_logger().error(f"{self.__class__.__name__} deleted before the terminated "
                                     f"event has been set while tasks are waiting for it. "
                                     f"Force setting event.")
             self.terminated.set()
 
     async def wait_for_terminate(self, timeout) -> None:
+        if self.terminated.is_set():
+            return
         await asyncio.wait_for(self.terminated.wait(), timeout=timeout)
 
     async def on_refresh_successful(self):
         """
         Called when synchronize succeed to update the instance
         """
         raise NotImplementedError("on_refresh_successful not implemented")
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-from octobot_trading.personal_data.trades.channel import trades
-from octobot_trading.personal_data.trades.channel.trades import (
-    TradesProducer,
-    TradesChannel,
+from octobot_trading.exchanges.implementations import default_websocket_exchange
+from octobot_trading.exchanges.implementations.default_websocket_exchange import (
+    DefaultWebSocketExchange,
 )
-
-from octobot_trading.personal_data.trades.channel import trades_updater
-from octobot_trading.personal_data.trades.channel.trades_updater import (
-    TradesUpdater,
+from octobot_trading.exchanges.implementations import default_rest_exchange
+from octobot_trading.exchanges.implementations.default_rest_exchange import (
+    DefaultRestExchange,
+)
+from octobot_trading.exchanges.implementations import exchange_simulator
+from octobot_trading.exchanges.implementations.exchange_simulator import (
+    ExchangeSimulator,
 )
 
 __all__ = [
-    "TradesProducer",
-    "TradesChannel",
-    "TradesUpdater",
+    "DefaultWebSocketExchange",
+    "DefaultRestExchange",
+    "ExchangeSimulator",
 ]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/implementations/__init__.pxd`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
@@ -10,14 +9,26 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-cimport octobot_trading.exchange_channel as exchanges_channel
 
-cdef class TradesProducer(exchanges_channel.ExchangeChannelProducer):
-    pass
+from octobot_trading.exchanges.implementations cimport default_websocket_exchange
+from octobot_trading.exchanges.implementations.default_websocket_exchange cimport (
+    DefaultWebSocketExchange,
+)
+from octobot_trading.exchanges.implementations cimport default_rest_exchange
+from octobot_trading.exchanges.implementations.default_rest_exchange cimport (
+    DefaultRestExchange,
+)
+from octobot_trading.exchanges.implementations cimport exchange_simulator
+from octobot_trading.exchanges.implementations.exchange_simulator cimport (
+    ExchangeSimulator,
+)
 
-cdef class TradesChannel(exchanges_channel.ExchangeChannel):
-    pass
+__all__ = [
+    "DefaultWebSocketExchange",
+    "DefaultRestExchange",
+    "ExchangeSimulator",
+]
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades_updater.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/channel/trades_updater.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/channel/trades_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     async def fetch_and_push(self):
         for symbol in self.channel.exchange_manager.exchange_config.traded_symbol_pairs:
             trades: list = await self.channel.exchange_manager.exchange.get_my_recent_trades(
                 symbol=symbol,
                 limit=self.MAX_OLD_TRADES_TO_FETCH)
 
             if trades:
-                await self.push(list(map(self.channel.exchange_manager.exchange.clean_trade, trades)))
+                await self.push(trades)
             if not self._is_initialized_event_set:
                 self._set_initialized_event(symbol)
         self._is_initialized_event_set = True
 
     def _set_initialized_event(self, symbol):
         # set init in updater as it's the only place we know if we fetched trades or not regardless of trades existence
         commons_tree.EventProvider.instance().trigger_event(
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trade_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trades_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trades_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trades_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/trades/trades_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/trades/trades_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction_factory.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transaction_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transactions_manager.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transactions_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/transactions_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/blockchain_transaction.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/blockchain_transaction.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/blockchain_transaction.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/blockchain_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/fee_transaction.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.pxd`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 #  Lesser General License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
 cimport octobot_trading.personal_data.transactions.transaction as transaction
 
-cdef class FeeTransaction(transaction.Transaction):
-    cdef readonly object quantity
-    cdef readonly object funding_rate
+cdef class RealisedPnlTransaction(transaction.Transaction):
+    cdef readonly object realised_pnl
+    cdef readonly object closed_quantity
+    cdef readonly object cumulated_closed_quantity
+    cdef readonly double first_entry_time
+    cdef readonly object average_entry_price
+    cdef readonly object average_exit_price
+    cdef readonly object order_exit_price
+    cdef readonly object leverage
+    cdef readonly object trigger_source
+    cdef readonly object side
 
-    cdef readonly str order_id
-
-    cpdef bint is_funding_fee(self)
-    cpdef bint is_trading_fee(self)
+    cpdef bint is_closed_pnl(self)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/fee_transaction.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/fee_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/realised_pnl_transaction.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/transfer_transaction.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/personal_data/transactions/types/transfer_transaction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-# cython: language_level=3
 #  Drakkar-Software OctoBot-Trading
 #  Copyright (c) Drakkar-Software, All rights reserved.
 #
 #  This library is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU Lesser General Public
 #  License as published by the Free Software Foundation; either
 #  version 3.0 of the License, or (at your option) any later version.
 #
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-#  Lesser General License for more details.
+#  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-cimport octobot_trading.personal_data.transactions.transaction as transaction
+import octobot_trading.enums as enums
+import octobot_trading.personal_data.transactions.transaction as transaction
 
-cdef class TransferTransaction(transaction.Transaction):
-    pass
+
+class TransferTransaction(transaction.Transaction):
+    def __init__(self, exchange_name, creation_time, currency, symbol):
+        super().__init__(exchange_name, creation_time,
+                         transaction_type=enums.TransactionType.TRANSFER,
+                         currency=currency,
+                         symbol=symbol)
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/personal_data/transactions/types/transfer_transaction.py` & `OctoBot-Trading-2.3.7/tests/personal_data/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,21 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-import octobot_trading.enums as enums
-import octobot_trading.personal_data.transactions.transaction as transaction
+DEFAULT_ORDER_SYMBOL = "BTC/USDT"
+DEFAULT_SYMBOL_QUANTITY = 10
+DEFAULT_MARKET_QUANTITY = 1000
 
 
-class TransferTransaction(transaction.Transaction):
-    def __init__(self, exchange_name, creation_time, currency, symbol):
-        super().__init__(exchange_name, creation_time,
-                         transaction_type=enums.TransactionType.TRANSFER,
-                         currency=currency,
-                         symbol=symbol)
+def check_created_transaction(exchange_manager, closed_quantity, cumulated_closed_quantity):
+    transaction = get_latest_transaction(exchange_manager)
+    assert transaction.closed_quantity == closed_quantity
+    assert transaction.cumulated_closed_quantity == cumulated_closed_quantity
+
+
+def get_latest_transaction(exchange_manager):
+    transactions = exchange_manager.exchange_personal_data.transactions_manager.transactions
+    return list(transactions.values())[-1] if transactions else None
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/channel/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/channel/remote_trading_signal.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/channel/remote_trading_signal.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/channel/remote_trading_signal_channel_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/channel/signal_producer.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/channel/signal_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/signal_creation.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/signal_creation.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,26 +57,29 @@
     try:
         return exchange_manager.trading_modes[0].should_emit_trading_signal()
     except IndexError:
         return False
 
 
 async def create_order(exchange_manager, should_emit_signal, order,
-                       loaded: bool = False, params: dict = None, pre_init_callback=None):
+                       loaded: bool = False, params: dict = None,
+                       wait_for_creation=True,
+                       creation_timeout=constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT):
     order_pf_percent = f"0{script_keywords.QuantityType.PERCENT.value}"
     if should_emit_signal:
         percent = await orders.get_order_size_portfolio_percent(
             exchange_manager,
             order.origin_quantity,
             order.side,
             order.symbol
         )
         order_pf_percent = f"{float(percent)}{script_keywords.QuantityType.PERCENT.value}"
     created_order = await exchange_manager.trader.create_order(
-        order, loaded=loaded, params=params, pre_init_callback=pre_init_callback
+        order, loaded=loaded, params=params,
+        wait_for_creation=wait_for_creation, creation_timeout=creation_timeout
     )
     if created_order is not None and should_emit_signal:
         signals.SignalPublisher.instance().get_signal_bundle_builder(order.symbol).add_created_order(
             created_order, exchange_manager, target_amount=order_pf_percent
         )
     return created_order
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/trading_signal_bundle_builder.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/signals/util.py` & `OctoBot-Trading-2.3.7/octobot_trading/signals/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/storage/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/storage/abstract_storage.py` & `OctoBot-Trading-2.3.7/octobot_trading/storage/abstract_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/storage/candles_storage.py` & `OctoBot-Trading-2.3.7/octobot_trading/storage/candles_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/storage/portfolio_storage.py` & `OctoBot-Trading-2.3.7/octobot_trading/storage/portfolio_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/storage/storage_manager.py` & `OctoBot-Trading-2.3.7/octobot_trading/storage/storage_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/storage/trades_storage.py` & `OctoBot-Trading-2.3.7/octobot_trading/storage/trades_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/storage/transactions_storage.py` & `OctoBot-Trading-2.3.7/octobot_trading/storage/transactions_storage.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/supervisors/__init__.pxd` & `OctoBot-Trading-2.3.7/tests/api/test_profitability.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,8 +10,11 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-__all__ = []
+import pytest
+
+# All test coroutines will be treated as marked.
+pytestmark = pytest.mark.asyncio
```

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/supervisors/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/supervisors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/supervisors/abstract_portfolio_supervisor.py` & `OctoBot-Trading-2.3.7/octobot_trading/supervisors/abstract_portfolio_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/supervisors/abstract_supervisor.py` & `OctoBot-Trading-2.3.7/octobot_trading/supervisors/abstract_supervisor.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/__init__.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/util/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/config_util.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/util/config_util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/config_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/initializable.pxd` & `OctoBot-Trading-2.3.7/octobot_trading/util/initializable.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/initializable.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/initializable.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/initialization_util.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/initialization_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/simulator_updater_utils.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/simulator_updater_utils.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/__init__.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/exchanges_test_tools.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/exchanges_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/spot_rest_exchange_test_tools.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/octobot_trading/util/test_tools/websocket_test_tools.py` & `OctoBot-Trading-2.3.7/octobot_trading/util/test_tools/websocket_test_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,21 +46,24 @@
         yield exchange_manager_instance
     finally:
         await exchanges_test_tools.stop_test_exchange_manager(exchange_manager_instance)
 
 
 async def test_unauthenticated_push_to_channel_coverage_websocket(
         websocket_exchange_class: exchanges.AbstractWebsocketExchange,
-        websocket_connector_class: exchanges.AbstractWebsocketConnector,
+        websocket_connector_class,
         exchange_manager: exchanges.ExchangeManager,
         config: object,
         symbols: list,
         time_frames: list,
         expected_pushed_channels: set = None,
         time_before_assert: int = 120):
+    """
+    DEPRECATED: TODO udpate for ccxt ws
+    """
 
     # To fix `TypeError: can't set attributes of built-in/extension type 'datetime.date'`
     class TestAbstractWebsocketExchange(websocket_exchange_class):
         pass
 
     pushed_channel_names = set()
     if expected_pushed_channels is None:
```

### Comparing `OctoBot-Trading-2.3.4/requirements.txt` & `OctoBot-Trading-2.3.7/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,12 @@
 trading-backend>=1.0.12
 
 # Exchange connection requirements
 ccxt==2.4.60 # always ensure real exchanges tests (in tests_additional and authenticated exchange tests) are passing before changing the ccxt version
 
 cryptography # Never specify a version (managed by https://github.com/Drakkar-Software/OctoBot-PyPi-Linux-Deployer)
 
-# Websocket requirements
-websockets==10.3
-cryptofeed==2.3.1
-
 # OrderBook requirement
 sortedcontainers==2.4.0
 
 # Scripting requirements
 tinydb==4.5.2
```

### Comparing `OctoBot-Trading-2.3.4/setup.py` & `OctoBot-Trading-2.3.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,16 @@
     "octobot_trading.personal_data.orders.orders_manager",
     "octobot_trading.personal_data.orders.order_state",
     "octobot_trading.personal_data.orders.order_group",
     "octobot_trading.personal_data.orders.order_util",
     "octobot_trading.personal_data.orders.order_factory",
     "octobot_trading.personal_data.orders.groups.balanced_take_profit_and_stop_order_group",
     "octobot_trading.personal_data.orders.groups.one_cancels_the_other_order_group",
+    "octobot_trading.personal_data.orders.states.pending_creation_order_state",
+    "octobot_trading.personal_data.orders.states.pending_creation_chained_order_state",
     "octobot_trading.personal_data.orders.states.fill_order_state",
     "octobot_trading.personal_data.orders.states.cancel_order_state",
     "octobot_trading.personal_data.orders.states.close_order_state",
     "octobot_trading.personal_data.orders.states.order_state_factory",
     "octobot_trading.personal_data.orders.states.open_order_state",
     "octobot_trading.personal_data.orders.types.unknown_order",
     "octobot_trading.personal_data.orders.types.market.buy_market_order",
@@ -172,37 +174,28 @@
     "octobot_trading.exchanges.basic_exchange_wrapper",
     "octobot_trading.exchanges.exchange_websocket_factory",
     "octobot_trading.exchanges.config.exchange_config_data",
     "octobot_trading.exchanges.config.backtesting_exchange_config",
     "octobot_trading.exchanges.exchange_builder",
     "octobot_trading.exchanges.exchange_channels",
     "octobot_trading.exchanges.exchange_factory",
-    "octobot_trading.exchanges.connectors.ccxt_exchange",
-    "octobot_trading.exchanges.connectors.exchange_simulator",
-    "octobot_trading.exchanges.connectors.abstract_websocket_connector",
-    "octobot_trading.exchanges.connectors.ccxt_websocket_connector",
-    "octobot_trading.exchanges.connectors.cryptofeed_websocket_connector",
+    "octobot_trading.exchanges.connectors.ccxt.ccxt_client_util",
+    "octobot_trading.exchanges.connectors.ccxt.ccxt_connector",
+    "octobot_trading.exchanges.connectors.ccxt.ccxt_websocket_connector",
+    "octobot_trading.exchanges.connectors.simulator.exchange_simulator_connector",
     "octobot_trading.exchanges.traders.trader",
     "octobot_trading.exchanges.traders.trader_simulator",
     "octobot_trading.exchanges.util.exchange_market_status_fixer",
     "octobot_trading.exchanges.util.websockets_util",
     "octobot_trading.exchanges.util.exchange_util",
-    "octobot_trading.exchanges.types.spot_exchange",
-    "octobot_trading.exchanges.types.margin_exchange",
-    "octobot_trading.exchanges.types.future_exchange",
+    "octobot_trading.exchanges.types.rest_exchange",
     "octobot_trading.exchanges.types.websocket_exchange",
-    "octobot_trading.exchanges.implementations.future_ccxt_exchange",
-    "octobot_trading.exchanges.implementations.future_exchange_simulator",
-    "octobot_trading.exchanges.implementations.margin_ccxt_exchange",
-    "octobot_trading.exchanges.implementations.margin_exchange_simulator",
-    "octobot_trading.exchanges.implementations.spot_ccxt_exchange",
-    "octobot_trading.exchanges.implementations.spot_exchange_simulator",
-    "octobot_trading.exchanges.implementations.ccxt_websocket_exchange",
-    "octobot_trading.exchanges.implementations.cryptofeed_websocket_exchange",
-    # "octobot_trading.exchanges.implementations.default_spot_ccxt_exchange",
+    "octobot_trading.exchanges.implementations.default_websocket_exchange",
+    "octobot_trading.exchanges.implementations.default_rest_exchange",
+    "octobot_trading.exchanges.implementations.exchange_simulator",
     "octobot_trading.exchange_channel",
 ]
 
 ext_modules = [
     Extension(package, [f"{package.replace('.', '/')}.py"], include_dirs=[np.get_include()])
     for package in packages_list]
```

### Comparing `OctoBot-Trading-2.3.4/tests/api/__init__.py` & `OctoBot-Trading-2.3.7/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/api/test_channels.py` & `OctoBot-Trading-2.3.7/tests/api/test_channels.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/api/test_exchange.py` & `OctoBot-Trading-2.3.7/tests/api/test_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/api/test_modes.py` & `OctoBot-Trading-2.3.7/tests/api/test_symbol_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/api/test_orders.py` & `OctoBot-Trading-2.3.7/tests/api/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/api/test_portfolio.py` & `OctoBot-Trading-2.3.7/tests/api/test_trades.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/api/test_profitability.py` & `OctoBot-Trading-2.3.7/octobot_trading/exchanges/connectors/simulator/__init__.pxd`

 * *Files 22% similar despite different names*

```diff
@@ -10,11 +10,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-import pytest
+from octobot_trading.exchanges.connectors.simulator cimport exchange_simulator_connector
+from octobot_trading.exchanges.connectors.simulator.exchange_simulator_connector cimport (
+    ExchangeSimulatorConnector,
+)
 
-# All test coroutines will be treated as marked.
-pytestmark = pytest.mark.asyncio
+__all__ = [
+    "ExchangeSimulatorConnector",
+]
```

### Comparing `OctoBot-Trading-2.3.4/tests/cli/__init__.py` & `OctoBot-Trading-2.3.7/tests/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/contracts/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/contracts/test_future_contract.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/contracts/test_future_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/contracts/test_margin_contract.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/contracts/test_margin_contract.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/funding/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/funding/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/funding/test_funding_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/funding/test_funding_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/kline/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/kline/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/kline/test_kline_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/kline/test_kline_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/ohlcv/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/ohlcv/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/ohlcv/test_candles_adapter.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/ohlcv/test_candles_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/ohlcv/test_candles_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/ohlcv/test_candles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/order_book/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/order_book/test_order_book_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/order_book/test_order_book_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/prices/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/prices/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/prices/test_price_events_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/prices/test_price_events_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/prices/test_prices_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/prices/test_prices_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/recent_trades/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/recent_trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/recent_trades/test_recent_trades_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/recent_trades/test_recent_trades_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/test_exchange_symbols_data.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/test_exchange_symbols_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/ticker/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/ticker/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchange_data/ticker/test_ticker_manager.py` & `OctoBot-Trading-2.3.7/tests/exchange_data/ticker/test_ticker_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/connectors/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchanges/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/connectors/test_ccxt_exchange.py` & `OctoBot-Trading-2.3.7/tests/exchanges/connectors/ccxt/test_ccxt_connector.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import decimal
+import pytest
 
 import ccxt.async_support
 from mock import patch, Mock
 
 import octobot_trading.exchanges.connectors as exchange_connectors
 import octobot_trading.enums as enums
 import octobot_trading.exchange_data.contracts as contracts
@@ -28,56 +29,58 @@
 from tests.exchanges.traders import future_trader, future_trader_simulator_with_default_linear, DEFAULT_FUTURE_SYMBOL, \
     DEFAULT_FUTURE_SYMBOL_MARGIN_TYPE, DEFAULT_FUTURE_SYMBOL_LEVERAGE
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-async def test_initialize_impl_with_none_symbols_and_timeframes(exchange_manager):
-    ccxt_exchange = exchange_connectors.CCXTExchange(exchange_manager.config, exchange_manager)
+@pytest.fixture
+def ccxt_connector(exchange_manager):
+    yield exchange_connectors.CCXTConnector(exchange_manager.config, exchange_manager)
+
+
+async def test_initialize_impl_with_none_symbols_and_timeframes(ccxt_connector):
 
     class MockCCXT:
         def __init__(self):
             self.symbols = None
             self.timeframes = None
 
-        async def load_markets(self):
+        async def load_markets(self, reload=False):
             pass
 
         def setSandboxMode(self, is_sandboxed):
             pass
 
-    with patch.object(ccxt_exchange, 'client', new=MockCCXT()):
-        await ccxt_exchange.initialize_impl()
-        assert ccxt_exchange.symbols == set()
-        assert ccxt_exchange.time_frames == set()
+    with patch.object(ccxt_connector, 'client', new=MockCCXT()):
+        await ccxt_connector.initialize_impl()
+        assert ccxt_connector.symbols == set()
+        assert ccxt_connector.time_frames == set()
 
 
-async def test_initialize_impl_with_empty_symbols_and_timeframes(exchange_manager):
-    ccxt_exchange = exchange_connectors.CCXTExchange(exchange_manager.config, exchange_manager)
+async def test_initialize_impl_with_empty_symbols_and_timeframes(ccxt_connector):
 
     class MockCCXT:
         def __init__(self):
             self.symbols = []
             self.timeframes = []
 
-        async def load_markets(self):
+        async def load_markets(self, reload=False):
             pass
 
         def setSandboxMode(self, is_sandboxed):
             pass
 
-    with patch.object(ccxt_exchange, 'client', new=MockCCXT()):
-        await ccxt_exchange.initialize_impl()
-        assert ccxt_exchange.symbols == set()
-        assert ccxt_exchange.time_frames == set()
+    with patch.object(ccxt_connector, 'client', new=MockCCXT()):
+        await ccxt_connector.initialize_impl()
+        assert ccxt_connector.symbols == set()
+        assert ccxt_connector.time_frames == set()
 
 
-async def test_initialize_impl(exchange_manager):
-    ccxt_exchange = exchange_connectors.CCXTExchange(exchange_manager.config, exchange_manager)
+async def test_initialize_impl(ccxt_connector):
 
     class MockCCXT:
         def __init__(self):
             self.symbols = [
                 "BTC/USDT",
                 "ETH/USDT",
                 "ETH/BTC",
@@ -86,62 +89,60 @@
             self.timeframes = [
                 "1h",
                 "2h",
                 "4h",
                 "2h"
             ]
 
-        async def load_markets(self):
+        async def load_markets(self, reload=False):
             pass
 
         def setSandboxMode(self, is_sandboxed):
             pass
 
-    with patch.object(ccxt_exchange, 'client', new=MockCCXT()):
-        await ccxt_exchange.initialize_impl()
-        assert ccxt_exchange.symbols == {
+    with patch.object(ccxt_connector, 'client', new=MockCCXT()):
+        await ccxt_connector.initialize_impl()
+        assert ccxt_connector.symbols == {
             "BTC/USDT",
             "ETH/USDT",
             "ETH/BTC",
         }
-        assert ccxt_exchange.time_frames == {
+        assert ccxt_connector.time_frames == {
             "1h",
             "2h",
             "4h",
         }
 
 
-async def test_set_symbol_partial_take_profit_stop_loss(exchange_manager):
-    ccxt_exchange = exchange_connectors.CCXTExchange(exchange_manager.config, exchange_manager)
+async def test_set_symbol_partial_take_profit_stop_loss(ccxt_connector):
     with pytest.raises(NotImplementedError):
-        await ccxt_exchange.set_symbol_partial_take_profit_stop_loss("BTC/USDT", False,
+        await ccxt_connector.set_symbol_partial_take_profit_stop_loss("BTC/USDT", False,
                                                                      enums.TakeProfitStopLossMode.PARTIAL)
 
 
-async def test_get_ccxt_order_type(exchange_manager):
-    ccxt_exchange = exchange_connectors.CCXTExchange(exchange_manager.config, exchange_manager)
+async def test_get_ccxt_order_type(ccxt_connector):
     with pytest.raises(RuntimeError):
-        ccxt_exchange.get_ccxt_order_type(None)
+        ccxt_connector.get_ccxt_order_type(None)
     with pytest.raises(RuntimeError):
-        ccxt_exchange.get_ccxt_order_type(enums.TraderOrderType.UNKNOWN)
-    assert ccxt_exchange.get_ccxt_order_type(enums.TraderOrderType.BUY_LIMIT) == enums.TradeOrderType.LIMIT.value
-    assert ccxt_exchange.get_ccxt_order_type(enums.TraderOrderType.STOP_LOSS_LIMIT) == enums.TradeOrderType.LIMIT.value
-    assert ccxt_exchange.get_ccxt_order_type(enums.TraderOrderType.TRAILING_STOP) == enums.TradeOrderType.MARKET.value
-    assert ccxt_exchange.get_ccxt_order_type(enums.TraderOrderType.SELL_MARKET) == enums.TradeOrderType.MARKET.value
+        ccxt_connector.get_ccxt_order_type(enums.TraderOrderType.UNKNOWN)
+    assert ccxt_connector.get_ccxt_order_type(enums.TraderOrderType.BUY_LIMIT) == enums.TradeOrderType.LIMIT.value
+    assert ccxt_connector.get_ccxt_order_type(enums.TraderOrderType.STOP_LOSS_LIMIT) == enums.TradeOrderType.LIMIT.value
+    assert ccxt_connector.get_ccxt_order_type(enums.TraderOrderType.TRAILING_STOP) == enums.TradeOrderType.MARKET.value
+    assert ccxt_connector.get_ccxt_order_type(enums.TraderOrderType.SELL_MARKET) == enums.TradeOrderType.MARKET.value
 
 
 async def test_get_trade_fee(exchange_manager, future_trader_simulator_with_default_linear):
     spot_fees_value = 0.001
     future_symbol = "BTC/USDT:USDT"
     future_fees_value = 0.0004
     spot_symbol = "BTC/USDT"
     config, fut_exchange_manager_inst, trader_inst, default_contract = future_trader_simulator_with_default_linear
     fut_exchange_manager_inst.is_future = True
-    fut_ccxt_exchange = exchange_connectors.CCXTExchange(config, fut_exchange_manager_inst)
-    spot_ccxt_exchange = exchange_connectors.CCXTExchange(exchange_manager.config, exchange_manager)
+    fut_ccxt_exchange = exchange_connectors.CCXTConnector(config, fut_exchange_manager_inst)
+    spot_ccxt_exchange = exchange_connectors.CCXTConnector(exchange_manager.config, exchange_manager)
 
     # spot trading
     spot_ccxt_exchange.client.options['defaultType'] = enums.ExchangeTypes.SPOT.value
     await spot_ccxt_exchange.client.load_markets()
     assert spot_fees_value / 5 <= spot_ccxt_exchange.client.markets[spot_symbol]['taker'] <= spot_fees_value * 5
     assert spot_ccxt_exchange.get_trade_fee(spot_symbol, enums.TraderOrderType.BUY_LIMIT, decimal.Decimal("0.45"),
                                             decimal.Decimal(10000), "taker") == \
```

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/implementations/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchanges/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_abstract_exchange.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_abstract_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_abstract_websocket_exchange.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_abstract_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_basic_exchange_wrapper.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_basic_exchange_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 import pytest
 import pytest_asyncio
 import mock
 import ccxt.async_support
 
 
 import octobot_trading.exchanges as exchanges
-import octobot_trading.enums as enums
+import octobot_trading.exchanges.connectors.ccxt.enums as ccxt_enums
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
 @pytest_asyncio.fixture
 async def basic_exchange_wrapper():
-    async with exchanges.temporary_exchange_wrapper("binanceus", enums.ExchangeWrapperLibs.ASYNC_CCXT) as wrapper:
+    async with exchanges.temporary_exchange_wrapper("binanceus", ccxt_enums.ExchangeWrapperLibs.ASYNC_CCXT) as wrapper:
         return wrapper
 
 
 async def test_constructor(basic_exchange_wrapper):
     assert isinstance(basic_exchange_wrapper.exchange, ccxt.async_support.binanceus)
-    async with exchanges.temporary_exchange_wrapper("okx", enums.ExchangeWrapperLibs.CCXT) as wrapper:
+    async with exchanges.temporary_exchange_wrapper("okx", ccxt_enums.ExchangeWrapperLibs.CCXT) as wrapper:
         assert isinstance(wrapper.exchange, ccxt.okx)
 
 
 async def test_temporary_exchange_wrapper():
     with mock.patch.object(ccxt.async_support.okx, "close", mock.AsyncMock()) as close_mock:
         with pytest.raises(ZeroDivisionError):
-            async with exchanges.temporary_exchange_wrapper("okx", enums.ExchangeWrapperLibs.ASYNC_CCXT) as wrapper:
+            async with exchanges.temporary_exchange_wrapper("okx", ccxt_enums.ExchangeWrapperLibs.ASYNC_CCXT) as wrapper:
                 assert isinstance(wrapper.exchange, ccxt.async_support.okx)
                 close_mock.assert_not_called()
                 1/0
         close_mock.assert_called_once()
 
 
 async def test_unsupported_lib():
```

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_config_data.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_config_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_factory.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_manager.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 import pytest
 from octobot_backtesting.backtesting import Backtesting
 
 from octobot_commons.tests.test_config import load_test_config
 from octobot_trading.exchanges.exchange_manager import ExchangeManager
 from octobot_trading.api.exchange import cancel_ccxt_throttle_task
-from octobot_trading.exchanges.types.spot_exchange import SpotExchange
-from octobot_trading.exchanges.implementations.spot_exchange_simulator import SpotExchangeSimulator
+from octobot_trading.exchanges.types import RestExchange
+from octobot_trading.exchanges.implementations import ExchangeSimulator
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
 class TestExchangeManager:
@@ -53,26 +53,26 @@
         assert exchange_manager is not None
         assert exchange_manager.exchange_name is TestExchangeManager.EXCHANGE_NAME
 
         assert exchange_manager.exchange.authenticated() is False
 
         assert exchange_manager.config is config
 
-        assert isinstance(exchange_manager.exchange, SpotExchangeSimulator)
+        assert isinstance(exchange_manager.exchange, ExchangeSimulator)
         await exchange_manager.stop()
 
         # real
         config, exchange_manager = await self.init_default(simulated=False)
 
         assert exchange_manager is not None
         assert exchange_manager.exchange_name is TestExchangeManager.EXCHANGE_NAME
 
         assert exchange_manager.config is config
 
-        assert isinstance(exchange_manager.exchange, SpotExchange)
+        assert isinstance(exchange_manager.exchange, RestExchange)
         cancel_ccxt_throttle_task()
         await exchange_manager.stop()
 
     async def test_get_is_overloaded(self):
         # simulated
         config, exchange_manager = await self.init_default(simulated=True, backtesting=True)
```

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_exchange_simulator.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/test_exchanges.py` & `OctoBot-Trading-2.3.7/tests/exchanges/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/traders/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchanges/traders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/traders/test_trader.py` & `OctoBot-Trading-2.3.7/tests/exchanges/traders/test_trader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/types/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchanges/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/types/test_websocket_exchange.py` & `OctoBot-Trading-2.3.7/tests/exchanges/types/test_websocket_exchange.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/util/__init__.py` & `OctoBot-Trading-2.3.7/tests/exchanges/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/util/test_exchange_market_status_fixer.py` & `OctoBot-Trading-2.3.7/tests/exchanges/util/test_exchange_market_status_fixer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/exchanges/util/test_exchange_util.py` & `OctoBot-Trading-2.3.7/tests/exchanges/util/test_exchange_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 pytestmark = pytest.mark.asyncio
 
 
 @pytest.fixture
 def tentacles_setup_config():
     setup_config = mock.Mock()
     setup_config.is_tentacle_activated = mock.Mock(return_value=True)
-    setup_config.get_config_folder = mock.Mock(return_value="")
     return setup_config
 
 
 @pytest.fixture()
 def exchange_config():
     return {
         commons_constants.CONFIG_EXCHANGE_KEY: commons_configuration.encrypt("01234").decode(),
```

### Comparing `OctoBot-Trading-2.3.4/tests/modes/__init__.py` & `OctoBot-Trading-2.3.7/tests/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/modes/script_keywords/__init__.py` & `OctoBot-Trading-2.3.7/tests/modes/script_keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/modes/script_keywords/basic_keywords/test_account_balance.py` & `OctoBot-Trading-2.3.7/tests/modes/script_keywords/basic_keywords/test_account_balance.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/modes/script_keywords/basic_keywords/test_amount.py` & `OctoBot-Trading-2.3.7/tests/modes/script_keywords/basic_keywords/test_amount.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/modes/script_keywords/dsl/__init__.py` & `OctoBot-Trading-2.3.7/tests/modes/script_keywords/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/modes/script_keywords/dsl/test_quantity.py` & `OctoBot-Trading-2.3.7/tests/modes/script_keywords/dsl/test_quantity.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/modes/test_abstract_mode_consumer.py` & `OctoBot-Trading-2.3.7/tests/modes/test_abstract_mode_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/modes/test_abstract_trading_mode.py` & `OctoBot-Trading-2.3.7/tests/modes/test_abstract_trading_mode.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,59 +72,62 @@
     buy_limit_order.origin_quantity = decimal.Decimal("0.1")
     buy_limit_order.symbol = "BTC/USDT"
     trading_mode.exchange_manager.trader = mock.Mock(create_order=mock.AsyncMock(return_value=buy_limit_order))
     create_order_mock = trading_mode.exchange_manager.trader.create_order
     # without context manager
     with mock.patch.object(trading_mode, "should_emit_trading_signal", mock.Mock(return_value=False)) \
          as should_emit_trading_signal_mock:
-        assert await trading_mode.create_order(buy_limit_order, loaded=False, params=None, pre_init_callback=None) \
+        assert await trading_mode.create_order(buy_limit_order, loaded=False, params=None) \
                is buy_limit_order
         assert should_emit_trading_signal_mock.call_count == 1
         create_order_mock.assert_called_once_with(
-            buy_limit_order, loaded=False, params=None, pre_init_callback=None
+            buy_limit_order, loaded=False, params=None, wait_for_creation=True,
+            creation_timeout=constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT
         )
         create_order_mock.reset_mock()
         should_emit_trading_signal_mock.reset_mock()
     with mock.patch.object(trading_mode, "should_emit_trading_signal", mock.Mock(return_value=True)) \
          as should_emit_trading_signal_mock:
         with pytest.raises(common_errors.MissingSignalBuilder):
-            await trading_mode.create_order(buy_limit_order, loaded=False, params=None, pre_init_callback=None)
+            await trading_mode.create_order(buy_limit_order, loaded=False, params=None,
+                                            wait_for_creation=False, creation_timeout=0)
         assert should_emit_trading_signal_mock.call_count == 1
         create_order_mock.assert_called_once_with(
-            buy_limit_order, loaded=False, params=None, pre_init_callback=None
+            buy_limit_order, loaded=False, params=None, wait_for_creation=False, creation_timeout=0
         )
         # created order but failed to register signal
         create_order_mock.reset_mock()
         should_emit_trading_signal_mock.reset_mock()
     # with context manager
     with mock.patch.object(signals_emitter, "emit_signal_bundle", mock.AsyncMock()) as emit_signal_bundle_mock:
         with mock.patch.object(trading_mode, "should_emit_trading_signal", mock.Mock(return_value=False)) \
                 as should_emit_trading_signal_mock:
             async with trading_mode.remote_signal_publisher("BTC/USDT") as builder:
                 assert await trading_mode.create_order(buy_limit_order, loaded=False,
-                                                       params=None, pre_init_callback=None) \
+                                                       params=None) \
                        is buy_limit_order
                 assert builder is None
                 assert should_emit_trading_signal_mock.call_count == 2
                 create_order_mock.assert_called_once_with(
-                    buy_limit_order, loaded=False, params=None, pre_init_callback=None
+                    buy_limit_order, loaded=False, params=None, wait_for_creation=True,
+                    creation_timeout=constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT
                 )
                 create_order_mock.reset_mock()
                 should_emit_trading_signal_mock.reset_mock()
             emit_signal_bundle_mock.assert_not_called()
         with mock.patch.object(trading_mode, "should_emit_trading_signal", mock.Mock(return_value=True)) \
                 as should_emit_trading_signal_mock:
             async with trading_mode.remote_signal_publisher("BTC/USDT") as builder:
-                assert await trading_mode.create_order(buy_limit_order, loaded=False, params=None,
-                                                       pre_init_callback=None) \
+                assert await trading_mode.create_order(buy_limit_order, loaded=False, params=None) \
                        is buy_limit_order
                 assert not builder.is_empty()
                 assert should_emit_trading_signal_mock.call_count == 2
                 create_order_mock.assert_called_once_with(
-                    buy_limit_order, loaded=False, params=None, pre_init_callback=None
+                    buy_limit_order, loaded=False, params=None, wait_for_creation=True,
+                    creation_timeout=constants.INDIVIDUAL_ORDER_SYNC_TIMEOUT
                 )
                 # created order but failed to register signal
                 create_order_mock.reset_mock()
                 should_emit_trading_signal_mock.reset_mock()
             emit_signal_bundle_mock.assert_called_once()
```

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/groups/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/groups/test_balanced_take_profit_and_stop_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/groups/test_one_cancels_the_other_order_group.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_cancel_order_state.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_cancel_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_close_order_state.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_close_order_state.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import OrderStatus
 from tests import event_loop
 from tests.exchanges import simulated_trader, simulated_exchange_manager
 from tests.personal_data.orders import sell_limit_order
 
 import pytest
 
 pytestmark = pytest.mark.asyncio
 
 
 async def test_on_order_refresh_successful(sell_limit_order):
     sell_limit_order.status = OrderStatus.CLOSED
     sell_limit_order.exchange_manager.is_backtesting = True
     await sell_limit_order.initialize()
+    assert isinstance(sell_limit_order.state, personal_data.CloseOrderState)
     await sell_limit_order.state.on_refresh_successful()
     assert sell_limit_order.is_closed()
     sell_limit_order.clear()
```

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_fill_order_state.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_fill_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_open_order_state.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_open_order_state.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import OrderStatus, OrderStates, States
 from octobot_trading.personal_data.orders.states.order_state_factory import create_order_state
 from tests import event_loop
 from tests.exchanges import simulated_trader, simulated_exchange_manager
 from tests.personal_data.orders import buy_limit_order
 import pytest
 
 pytestmark = pytest.mark.asyncio
 
 
 async def test_on_order_refresh_successful(buy_limit_order):
     buy_limit_order.exchange_manager.is_backtesting = True
     await buy_limit_order.initialize()
+    assert isinstance(buy_limit_order.state, personal_data.OpenOrderState)
     await buy_limit_order.state.on_refresh_successful()
     assert buy_limit_order.state.state is States.OPEN
     buy_limit_order.status = OrderStatus.FILLED
     await buy_limit_order.state.on_refresh_successful()
     assert buy_limit_order.is_filled()
```

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_order_state.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_order_state.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_order_state_factory.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_order_state_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,74 +9,95 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import octobot_trading.personal_data as personal_data
 from octobot_trading.enums import OrderStatus, OrderStates, States
 from octobot_trading.personal_data.orders import create_order_state
 
 import pytest
 from tests import event_loop
 from tests.exchanges import simulated_trader, simulated_exchange_manager
 from tests.personal_data.orders import buy_limit_order
 
 pytestmark = pytest.mark.asyncio
 
 
 async def test_create_order_state_pending_creation(buy_limit_order):
     buy_limit_order.status = OrderStatus.PENDING_CREATION
     await create_order_state(buy_limit_order)
+    assert isinstance(buy_limit_order.state, personal_data.PendingCreationOrderState)
+    assert buy_limit_order.state.state is States.PENDING_CREATION
+
+
+async def test_create_order_state_pending_chained_creation(buy_limit_order):
+    buy_limit_order.status = OrderStatus.PENDING_CREATION
+    buy_limit_order.is_waiting_for_chained_trigger = True
+    await create_order_state(buy_limit_order)
+    assert isinstance(buy_limit_order.state, personal_data.PendingCreationChainedOrderState)
     assert buy_limit_order.state.state is States.PENDING_CREATION
 
 
 async def test_create_order_state_open(buy_limit_order):
     buy_limit_order.status = OrderStatus.OPEN
     await create_order_state(buy_limit_order)
+    assert isinstance(buy_limit_order.state, personal_data.OpenOrderState)
     assert buy_limit_order.state.state is States.OPEN
 
 
 async def test_create_order_state_cancel(buy_limit_order):
     buy_limit_order.status = OrderStatus.CANCELED
     await create_order_state(buy_limit_order)
     # can be CANCELED or instant CLOSED
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     assert buy_limit_order.state.state in [OrderStates.FILLED, States.CLOSED]
 
 
 async def test_create_order_state_fill(buy_limit_order):
     buy_limit_order.status = OrderStatus.FILLED
     await create_order_state(buy_limit_order)
     # can be FILLED or instant CLOSED
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     assert buy_limit_order.state.state in [OrderStates.FILLED, States.CLOSED]
 
 
 async def test_create_order_state_close(buy_limit_order):
     buy_limit_order.status = OrderStatus.CLOSED
     await create_order_state(buy_limit_order)
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     assert buy_limit_order.state.state is States.CLOSED
 
 
 async def test_create_order_state_fill_to_open_without_ignore(buy_limit_order):
     buy_limit_order.status = OrderStatus.FILLED
     await create_order_state(buy_limit_order)
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     buy_limit_order.status = OrderStatus.OPEN
     await create_order_state(buy_limit_order, ignore_states=[])
+    assert isinstance(buy_limit_order.state, personal_data.OpenOrderState)
     assert buy_limit_order.state.state is States.OPEN
 
 
 async def test_create_order_state_fill_to_open_with_ignore(buy_limit_order):
     buy_limit_order.status = OrderStatus.FILLED
     await create_order_state(buy_limit_order)
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     buy_limit_order.status = OrderStatus.OPEN
     await create_order_state(buy_limit_order, ignore_states=[States.OPEN])
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     # can be FILLED or instant CLOSED
     assert buy_limit_order.state.state in [OrderStates.FILLED, States.CLOSED]
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
 
 
 async def test_create_order_state_cancel_to_open_with_ignore(buy_limit_order):
     buy_limit_order.status = OrderStatus.CANCELED
     await create_order_state(buy_limit_order)
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     buy_limit_order.status = OrderStatus.OPEN
     await create_order_state(buy_limit_order, ignore_states=[States.OPEN])
+    assert isinstance(buy_limit_order.state, personal_data.CloseOrderState)
     # can be CANCELED or instant CLOSED
     assert buy_limit_order.state.state in [OrderStates.CANCELED, States.CLOSED]
```

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/states/test_pending_creation_order_state.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/states/test_pending_creation_chained_order_state.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
-from octobot_trading.enums import OrderStatus, OrderStates, States
+import octobot_trading.personal_data as personal_data
+from octobot_trading.enums import OrderStatus, States
 from octobot_trading.personal_data.orders.states.order_state_factory import create_order_state
 from tests import event_loop
 from tests.exchanges import simulated_trader, simulated_exchange_manager
 from tests.personal_data.orders import buy_limit_order
 import pytest
 
 pytestmark = pytest.mark.asyncio
 
 
 async def test_on_order_refresh_successful(buy_limit_order):
     buy_limit_order.exchange_manager.is_backtesting = True
     buy_limit_order.status = OrderStatus.PENDING_CREATION
+    buy_limit_order.is_waiting_for_chained_trigger = True
     await buy_limit_order.initialize()
+    assert isinstance(buy_limit_order.state, personal_data.PendingCreationChainedOrderState)
     await buy_limit_order.state.on_refresh_successful()
     assert buy_limit_order.state.state is States.PENDING_CREATION
     buy_limit_order.status = OrderStatus.PENDING_CREATION
     await buy_limit_order.state.on_refresh_successful()
     buy_limit_order.status = OrderStatus.PENDING_CREATION
     assert buy_limit_order.is_created() is False
```

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/test_decimal_order_adapter.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/test_decimal_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/test_double_filled_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/test_double_filled_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order_adapter.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order_adapter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order_factory.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/test_order_util.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/test_order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_buy_limit_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_buy_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_sell_limit_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_sell_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_stop_loss_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_stop_loss_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_stop_loss_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_take_profit_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/limit/test_take_profit_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/limit/test_take_profit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/market/test_buy_market_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/market/test_buy_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/market/test_sell_market_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/market/test_sell_market_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/test_unknown_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/test_unknown_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/trailing/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/trailing/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/trailing/test_trailing_stop_limit_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py` & `OctoBot-Trading-2.3.7/tests/personal_data/orders/types/trailing/test_trailing_stop_order.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/test_future_asset.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/test_future_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/test_margin_asset.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/test_margin_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/assets/test_spot_asset.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/assets/test_spot_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/history/test_historical_asset_value_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/history/test_historical_portfolio_value_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_asset.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_asset.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio_manager.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio_profitability.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio_profitability.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/test_portfolio_value_holder.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/test_portfolio_value_holder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/test_future_portfolio.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/test_future_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/test_margin_portfolio.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/test_margin_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/portfolios/types/test_spot_portfolio.py` & `OctoBot-Trading-2.3.7/tests/personal_data/portfolios/types/test_spot_portfolio.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/channel/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/states/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/states/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/test_position.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/test_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/test_position_factory.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/test_position_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/test_positions_manager.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/test_positions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/types/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/types/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/types/test_inverse_position.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/types/test_inverse_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/positions/types/test_linear_position.py` & `OctoBot-Trading-2.3.7/tests/personal_data/positions/types/test_linear_position.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/trades/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/trades/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/trades/test_trade_factory.py` & `OctoBot-Trading-2.3.7/tests/personal_data/trades/test_trade_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/trades/test_trade_manager.py` & `OctoBot-Trading-2.3.7/tests/personal_data/trades/test_trade_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/transactions/__init__.py` & `OctoBot-Trading-2.3.7/tests/personal_data/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/transactions/test_transaction_factory.py` & `OctoBot-Trading-2.3.7/tests/personal_data/transactions/test_transaction_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/personal_data/transactions/test_transactions_manager.py` & `OctoBot-Trading-2.3.7/tests/personal_data/transactions/test_transactions_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/signals/__init__.py` & `OctoBot-Trading-2.3.7/tests/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/signals/test_trading_signal_bundle_builder.py` & `OctoBot-Trading-2.3.7/tests/signals/test_trading_signal_bundle_builder.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/signals/test_util.py` & `OctoBot-Trading-2.3.7/tests/signals/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     await buy_limit_order.set_as_chained_order(sell_limit_order, True, {})
     assert signals.create_order_signal_content(
         buy_limit_order,
         enums.TradingSignalOrdersActions.CREATE,
         "strat",
         exchange_manager,
         target_amount="1%",
-        target_position="2"
+        target_position="2",
     ) == {
         enums.TradingSignalCommonsAttrs.ACTION.value: enums.TradingSignalOrdersActions.CREATE.value,
         enums.TradingSignalOrdersAttrs.SIDE.value: enums.TradeOrderSide.BUY.value,
         enums.TradingSignalOrdersAttrs.STRATEGY.value: "strat",
         enums.TradingSignalOrdersAttrs.SYMBOL.value: "BTC/ETH",
         enums.TradingSignalOrdersAttrs.EXCHANGE.value: "binanceus",
         enums.TradingSignalOrdersAttrs.EXCHANGE_TYPE.value: enums.ExchangeTypes.SPOT.value,
```

### Comparing `OctoBot-Trading-2.3.4/tests/test_utils/order_util.py` & `OctoBot-Trading-2.3.7/tests/test_utils/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/test_utils/random_numbers.py` & `OctoBot-Trading-2.3.7/tests/test_utils/random_numbers.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/util/__init__.py` & `OctoBot-Trading-2.3.7/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests/util/test_config_util.py` & `OctoBot-Trading-2.3.7/tests/util/test_config_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests_additional/__init__.py` & `OctoBot-Trading-2.3.7/tests_additional/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/__init__.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/real_exchange_tester.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/real_exchange_tester.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     EXCHANGE_TYPE = trading_enums.ExchangeTypes.SPOT.value
     SYMBOL = None
     SYMBOL_2 = None
     SYMBOL_3 = None
     # default is 1h, change if necessary
     TIME_FRAME = commons_enums.TimeFrames.ONE_HOUR
     ALLOWED_TIMEFRAMES_WITHOUT_CANDLE = 0
+    CANDLE_SINCE = 631152000000    # 01/01/1990
+    CANDLE_SINCE_SEC = CANDLE_SINCE / 1000
 
     # Public methods: to be implemented as tests
     # Use await self._[method_name] to get the test request result
     # ex: market_status = await self.get_market_status()
 
     # unauthenticated API
     async def test_time_frames(self):
@@ -134,19 +136,23 @@
     async def get_all_currencies_price_ticker(self, **kwargs):
         async with get_exchange_manager(self.EXCHANGE_NAME, self.get_config()) as exchange_manager:
             return await exchange_manager.exchange.get_all_currencies_price_ticker(**kwargs)
 
     def get_allowed_time_delta(self):
         return (self.ALLOWED_TIMEFRAMES_WITHOUT_CANDLE + 1) * \
                commons_enums.TimeFramesMinutes[self.TIME_FRAME] * \
-               constants.MINUTE_TO_SECONDS * constants.MSECONDS_TO_SECONDS * 1.3
+               constants.MINUTE_TO_SECONDS * 1.3
 
     @staticmethod
     def get_time():
-        return Exchange.milliseconds()
+        return Exchange.seconds()
+
+    @staticmethod
+    def get_ms_time():
+        return int(Exchange.milliseconds())
 
     @staticmethod
     def ensure_elements_order(elements, sort_key, reverse=False):
         assert sorted(elements, key=lambda x: x[sort_key], reverse=reverse) == elements
 
     def check_market_status_limits(self, market_status,
                                    normal_price_max=10000, normal_price_min=1e-06,
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_ascendex.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_ascendex.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,17 @@
         symbol_prices = await self.get_symbol_prices(limit=5)
         assert len(symbol_prices) == 5
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_binance.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_wavesexchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,43 +16,41 @@
 import pytest
 
 from octobot_commons.enums import TimeFrames, PriceIndexes
 from octobot_trading.enums import ExchangeConstantsMarketStatusColumns as Ecmsc, \
     ExchangeConstantsOrderBookInfoColumns as Ecobic, ExchangeConstantsOrderColumns as Ecoc, \
     ExchangeConstantsTickersColumns as Ectc
 from tests_additional.real_exchanges.real_exchange_tester import RealExchangeTester
+import octobot_trading.errors as errors
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestBinanceRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "binanceus"  # use binanceus for tests as binance is blocked in the us
-    SYMBOL = "BTC/USDT"
+class TestWavesExchangeRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "wavesexchange"
+    SYMBOL = "BTC/USDN"
     SYMBOL_2 = "ETH/BTC"
-    SYMBOL_3 = "XRP/BTC"
+    SYMBOL_3 = "WAVES/BTC"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
-            TimeFrames.THREE_MINUTES.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
             TimeFrames.TWO_HOURS.value,
             TimeFrames.FOUR_HOURS.value,
             TimeFrames.SIX_HOURS.value,
-            TimeFrames.HEIGHT_HOURS.value,
             TimeFrames.TWELVE_HOURS.value,
             TimeFrames.ONE_DAY.value,
-            TimeFrames.THREE_DAYS.value,
             TimeFrames.ONE_WEEK.value,
             TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
@@ -67,58 +65,57 @@
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
             self.check_market_status_limits(market_status, expect_invalid_price_limit_values=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 500
+        assert len(symbol_prices) == 1440
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        with pytest.raises(errors.UnexpectedAdapterError):
+            # try with since and limit (used in data collector)
+            assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_order_book(self):
         order_book = await self.get_order_book()
-        assert len(order_book[Ecobic.ASKS.value]) == 5
+        assert len(order_book[Ecobic.ASKS.value]) == 6
         assert len(order_book[Ecobic.ASKS.value][0]) == 2
-        assert len(order_book[Ecobic.BIDS.value]) == 5
+        assert len(order_book[Ecobic.BIDS.value]) == 6
         assert len(order_book[Ecobic.BIDS.value][0]) == 2
 
     async def test_get_recent_trades(self):
         recent_trades = await self.get_recent_trades()
         assert len(recent_trades) == 50
         # check trades order (oldest first)
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
         self._check_ticker(ticker, self.SYMBOL, check_content=True)
 
-    async def test_get_all_currencies_price_ticker(self):
-        tickers = await self.get_all_currencies_price_ticker()
-        for symbol, ticker in tickers.items():
-            self._check_ticker(ticker, symbol)
-
     @staticmethod
     def _check_ticker(ticker, symbol, check_content=False):
         assert ticker[Ectc.SYMBOL.value] == symbol
         assert all(key in ticker for key in (
             Ectc.HIGH.value,
             Ectc.LOW.value,
             Ectc.BID.value,
@@ -129,18 +126,18 @@
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
-            assert ticker[Ectc.BID.value]
-            assert ticker[Ectc.BID_VOLUME.value]
-            assert ticker[Ectc.ASK.value]
-            assert ticker[Ectc.ASK_VOLUME.value]
+            assert ticker[Ectc.BID.value] is None
+            assert ticker[Ectc.BID_VOLUME.value] is None
+            assert ticker[Ectc.ASK.value] is None
+            assert ticker[Ectc.ASK_VOLUME.value] is None
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
-            assert ticker[Ectc.PREVIOUS_CLOSE.value]
+            assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
             assert ticker[Ectc.BASE_VOLUME.value]
-            assert ticker[Ectc.TIMESTAMP.value]
-            RealExchangeTester.check_ticker_typing(ticker)
+            assert ticker[Ectc.TIMESTAMP.value] is None  # will trigger an 'Ignored incomplete ticker'
+            RealExchangeTester.check_ticker_typing(ticker, check_timestamp=False)
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitfinex.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitfinex.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             TimeFrames.TWELVE_HOURS.value,
             TimeFrames.ONE_DAY.value,
             TimeFrames.ONE_WEEK.value,
             TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
-        # await asyncio.sleep(self.SLEEP_TIME)  # prevent rate api limit
+        await asyncio.sleep(self.SLEEP_TIME)  # prevent rate api limit
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
             assert int(market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_AMOUNT.value]) == \
                    market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_AMOUNT.value]
             assert int(market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_PRICE.value]) == \
@@ -94,14 +94,23 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert 200 >= len(symbol_prices) >= 200 - candle_limit_error
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50)
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         # await asyncio.sleep(10) # prevent rate api limit
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitget.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitget.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,25 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 100
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []
+        # "until" param is required: add in tentacle
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50, until=self.get_ms_time())
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bithumb.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bithumb.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,24 @@
         symbol_prices = (await self.get_symbol_prices())[-200:]
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50)
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
+
     async def test_get_kline_price(self):
         # kline_price = await self.get_kline_price()
         client = bithumb()
         await client.fetch_markets()
         kline_price = [(await client.fetch_ohlcv(TestBithumbRealExchangeTester.SYMBOL, TimeFrames.ONE_HOUR.value))[-1]]
 
         assert len(kline_price) == 1
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitso.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitso.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,17 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bitstamp.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bitstamp.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,17 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bittrex.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bittrex.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         symbol_prices = (await self.get_symbol_prices())[-200:]
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         # kline_price = await self.get_kline_price()
         client = bittrex()
         await client.fetch_markets()
         kline_price = [(await client.fetch_ohlcv(TestBittrexRealExchangeTester.SYMBOL, TimeFrames.ONE_HOUR.value))[-1]]
 
         assert len(kline_price) == 1
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_bybit.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_bybit.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import pytest
+import time
 
 from octobot_commons.enums import TimeFrames, PriceIndexes
 from octobot_trading.enums import ExchangeConstantsMarketStatusColumns as Ecmsc, \
     ExchangeConstantsOrderBookInfoColumns as Ecobic, ExchangeConstantsOrderColumns as Ecoc, \
     ExchangeConstantsTickersColumns as Ectc
 import octobot_trading.enums as trading_enums
 import octobot_trading.errors as errors
@@ -97,14 +98,25 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []
+        # "end" param is required: add in tentacle
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50, end=self.get_ms_time())
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_coinbasepro.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_coinbasepro.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         symbol_prices = await self.get_symbol_prices(limit=100)
         assert len(symbol_prices) == 100
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_coinex.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_upbit.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,36 +23,33 @@
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestCoinexRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "coinex"
+class TestUpbitRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "upbit"
     SYMBOL = "BTC/USDT"
     SYMBOL_2 = "ETH/BTC"
     SYMBOL_3 = "XRP/BTC"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
             TimeFrames.THREE_MINUTES.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
-            TimeFrames.TWO_HOURS.value,
             TimeFrames.FOUR_HOURS.value,
-            TimeFrames.SIX_HOURS.value,
-            TimeFrames.TWELVE_HOURS.value,
             TimeFrames.ONE_DAY.value,
-            TimeFrames.THREE_DAYS.value,
             TimeFrames.ONE_WEEK.value,
+            TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
@@ -66,44 +63,44 @@
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
             self.check_market_status_limits(market_status, expect_invalid_price_limit_values=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        # default 100 candles
-        assert len(symbol_prices) == 100
+        assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
-        symbol_prices = await self.get_symbol_prices(limit=550)
-        assert len(symbol_prices) == 550
+        symbol_prices = await self.get_symbol_prices(limit=200)
+        assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
-
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_order_book(self):
-        # fetchOrderBook() limit argument must be None, 5/10/20/50. Default is 20
-        order_book = await self.get_order_book(limit=10)
-        assert len(order_book[Ecobic.ASKS.value]) == 10
+        order_book = await self.get_order_book()
+        assert len(order_book[Ecobic.ASKS.value]) == 15
         assert len(order_book[Ecobic.ASKS.value][0]) == 2
-        assert len(order_book[Ecobic.BIDS.value]) == 10
+        assert len(order_book[Ecobic.BIDS.value]) == 15
         assert len(order_book[Ecobic.BIDS.value][0]) == 2
 
     async def test_get_recent_trades(self):
         recent_trades = await self.get_recent_trades()
         assert len(recent_trades) == 50
         # check trades order (oldest first)
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
@@ -131,18 +128,18 @@
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
-            assert ticker[Ectc.BID.value]
+            assert ticker[Ectc.BID.value] is None
             assert ticker[Ectc.BID_VOLUME.value] is None
-            assert ticker[Ectc.ASK.value]
+            assert ticker[Ectc.ASK.value] is None
             assert ticker[Ectc.ASK_VOLUME.value] is None
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
-            assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
+            assert ticker[Ectc.PREVIOUS_CLOSE.value]
             assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
-            RealExchangeTester.check_ticker_typing(ticker, check_open=False)
+            RealExchangeTester.check_ticker_typing(ticker)
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_gateio.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_gateio.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import pytest
 
 from octobot_commons.enums import TimeFrames, PriceIndexes
 from octobot_trading.enums import ExchangeConstantsMarketStatusColumns as Ecmsc, \
     ExchangeConstantsOrderBookInfoColumns as Ecobic, ExchangeConstantsOrderColumns as Ecoc, \
     ExchangeConstantsTickersColumns as Ectc
 from tests_additional.real_exchanges.real_exchange_tester import RealExchangeTester
+import octobot_trading.errors as errors
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
@@ -77,14 +78,18 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        with pytest.raises(errors.FailedRequest):
+            assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_hitbtc.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_huobi.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 import pytest
 
 from octobot_commons.enums import TimeFrames, PriceIndexes
 from octobot_trading.enums import ExchangeConstantsMarketStatusColumns as Ecmsc, \
     ExchangeConstantsOrderBookInfoColumns as Ecobic, ExchangeConstantsOrderColumns as Ecoc, \
     ExchangeConstantsTickersColumns as Ectc
 from tests_additional.real_exchanges.real_exchange_tester import RealExchangeTester
+import octobot_trading.errors as errors
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestHitBtcRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "hitbtc"
+class TestHuobiRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "huobipro"
     SYMBOL = "BTC/USDT"
     SYMBOL_2 = "ETH/BTC"
     SYMBOL_3 = "XRP/BTC"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
-            TimeFrames.THREE_MINUTES.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
             TimeFrames.FOUR_HOURS.value,
             TimeFrames.ONE_DAY.value,
             TimeFrames.ONE_WEEK.value,
@@ -49,48 +49,51 @@
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
-            assert 1e-08 <= market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_AMOUNT.value] < 1  # to be fixed in hitbtc tentacle
+            assert 1e-06 <= market_status[Ecmsc.PRECISION.value][
+                Ecmsc.PRECISION_AMOUNT.value] <= 1  # to be fixed in tentacle
             assert 1e-09 <= market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_PRICE.value] < 1  # to be fixed in hitbtc tentacle
+                Ecmsc.PRECISION_PRICE.value] <= 1   # to be fixed in tentacle
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
+            # invalid values => remove price limit in tentacle
             self.check_market_status_limits(market_status,
-                                            normal_price_min=1e-09,
-                                            normal_cost_min=1e-10,
-                                            low_cost_min=1e-10,
-                                            expect_invalid_price_limit_values=False,
+                                            normal_price_max=100000,    # way too high (BTC/USDT)
+                                            expect_invalid_price_limit_values=True,
                                             enable_price_and_cost_comparison=False)
 
     async def test_get_symbol_prices(self):
         # without limit
-        symbol_prices = await self.get_symbol_prices(sort='DESC')
-        assert len(symbol_prices) == 100
+        symbol_prices = await self.get_symbol_prices()
+        assert len(symbol_prices) == 150
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
-        symbol_prices = await self.get_symbol_prices(limit=200, sort='DESC')  # to be fixed in hitbtc tentacle
+        symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        with pytest.raises(errors.FailedRequest):
+            assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
-        kline_price = await self.get_kline_price(sort='DESC')  # to be fixed in hitbtc tentacle
+        kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_order_book(self):
@@ -130,17 +133,17 @@
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
             assert ticker[Ectc.BID.value]
-            assert ticker[Ectc.BID_VOLUME.value] is None
+            assert ticker[Ectc.BID_VOLUME.value]
             assert ticker[Ectc.ASK.value]
-            assert ticker[Ectc.ASK_VOLUME.value] is None
+            assert ticker[Ectc.ASK_VOLUME.value]
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
             assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
             assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
             RealExchangeTester.check_ticker_typing(ticker)
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_hollaex.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_hollaex.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,14 +77,17 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_huobi.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_poloniex.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,70 +23,78 @@
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestHuobiRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "huobipro"
+class TestPoloniexRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "poloniex"
     SYMBOL = "BTC/USDT"
     SYMBOL_2 = "ETH/BTC"
     SYMBOL_3 = "XRP/BTC"
+    TIME_FRAME = TimeFrames.THIRTY_MINUTES  # 1h doesn't exist on Poloniex
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
-            TimeFrames.ONE_MINUTE.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
-            TimeFrames.ONE_HOUR.value,
+            TimeFrames.TWO_HOURS.value,
             TimeFrames.FOUR_HOURS.value,
             TimeFrames.ONE_DAY.value,
-            TimeFrames.ONE_WEEK.value,
-            TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
-            assert 1e-06 <= market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_AMOUNT.value] <= 1  # to be fixed in tentacle
-            assert 1e-09 <= market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_PRICE.value] <= 1   # to be fixed in tentacle
+            assert 1e-08 <= market_status[Ecmsc.PRECISION.value][
+                Ecmsc.PRECISION_AMOUNT.value] <= 1   # to be fixed in tentacle
+            assert 1e-08 <= market_status[Ecmsc.PRECISION.value][
+                Ecmsc.PRECISION_PRICE.value] < 1    # to be fixed in tentacle
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
             # invalid values => remove price limit in tentacle
             self.check_market_status_limits(market_status,
-                                            normal_price_max=100000,    # way too high (BTC/USDT)
+                                            normal_price_min=1e-05,  # 1000000 for BTC/USDT, 1e-05 for XRP/BTC, lol
+                                            normal_price_max=10000000,
                                             expect_invalid_price_limit_values=True,
                                             enable_price_and_cost_comparison=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 150
+        assert len(symbol_prices) == 100
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50)
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
@@ -127,18 +135,18 @@
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
-            assert ticker[Ectc.BID.value]
-            assert ticker[Ectc.BID_VOLUME.value]
-            assert ticker[Ectc.ASK.value]
-            assert ticker[Ectc.ASK_VOLUME.value]
+            assert ticker[Ectc.BID.value] is None
+            assert ticker[Ectc.BID_VOLUME.value] is None
+            assert ticker[Ectc.ASK.value] is None
+            assert ticker[Ectc.ASK_VOLUME.value] is None
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
             assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
             assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
             RealExchangeTester.check_ticker_typing(ticker)
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_huobipro.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_huobipro.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_kraken.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_kraken.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,23 @@
         symbol_prices = (await self.get_symbol_prices())[-200:]
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50)
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         # kline_price = await self.get_kline_price()
         client = kraken()
         await client.fetch_markets()
         kline_price = [(await client.fetch_ohlcv(TestKrakenRealExchangeTester.SYMBOL, TimeFrames.ONE_HOUR.value))[-1]]
 
         assert len(kline_price) == 1
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_kucoin.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_hitbtc.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,93 +23,96 @@
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestKucoinRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "kucoin"
+class TestHitBtcRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "hitbtc"
     SYMBOL = "BTC/USDT"
     SYMBOL_2 = "ETH/BTC"
     SYMBOL_3 = "XRP/BTC"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
             TimeFrames.THREE_MINUTES.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
-            TimeFrames.TWO_HOURS.value,
             TimeFrames.FOUR_HOURS.value,
-            TimeFrames.SIX_HOURS.value,
-            TimeFrames.HEIGHT_HOURS.value,
-            TimeFrames.TWELVE_HOURS.value,
             TimeFrames.ONE_DAY.value,
-            TimeFrames.ONE_WEEK.value
+            TimeFrames.ONE_WEEK.value,
+            TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
-            # on this exchange, precision is a decimal instead of a number of digits
-            assert 0 < market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_AMOUNT.value] <= 1  # to be fixed in this exchange tentacle
-            assert 0 < market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_PRICE.value] <= 1  # to be fixed in this exchange tentacle
+            assert 1e-08 <= market_status[Ecmsc.PRECISION.value][
+                Ecmsc.PRECISION_AMOUNT.value] < 1  # to be fixed in hitbtc tentacle
+            assert 1e-09 <= market_status[Ecmsc.PRECISION.value][
+                Ecmsc.PRECISION_PRICE.value] < 1  # to be fixed in hitbtc tentacle
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
-            # invalid values (should be much lower for XRP/BTC => remove price limit in tentacle
             self.check_market_status_limits(market_status,
-                                            expect_invalid_price_limit_values=True,
+                                            normal_price_min=1e-09,
+                                            normal_cost_min=1e-10,
+                                            low_cost_min=1e-10,
+                                            expect_invalid_price_limit_values=False,
                                             enable_price_and_cost_comparison=False)
 
     async def test_get_symbol_prices(self):
         # without limit
-        symbol_prices = await self.get_symbol_prices()
+        symbol_prices = await self.get_symbol_prices(sort='DESC')
         assert len(symbol_prices) == 100
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
-        symbol_prices = await self.get_symbol_prices(limit=100)
-        assert len(symbol_prices) == 100
+        symbol_prices = await self.get_symbol_prices(limit=200, sort='DESC')  # to be fixed in hitbtc tentacle
+        assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50)
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
-        kline_price = await self.get_kline_price()
+        kline_price = await self.get_kline_price(sort='DESC')  # to be fixed in hitbtc tentacle
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_order_book(self):
-        # kucoin requires a limit of None, 20 or 100 in order book
-        order_book = await self.get_order_book(limit=20)
-        assert len(order_book[Ecobic.ASKS.value]) == 20
+        order_book = await self.get_order_book()
+        assert len(order_book[Ecobic.ASKS.value]) == 5
         assert len(order_book[Ecobic.ASKS.value][0]) == 2
-        assert len(order_book[Ecobic.BIDS.value]) == 20
+        assert len(order_book[Ecobic.BIDS.value]) == 5
         assert len(order_book[Ecobic.BIDS.value][0]) == 2
 
     async def test_get_recent_trades(self):
-        # note: on ccxt kucoin recent trades are received in reverse order from exchange and therefore should never be
-        # filtered by limit before reversing (or most recent trades are lost)
         recent_trades = await self.get_recent_trades()
         assert len(recent_trades) == 50
         # check trades order (oldest first)
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
@@ -144,8 +147,8 @@
             assert ticker[Ectc.ASK_VOLUME.value] is None
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
             assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
             assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
-            RealExchangeTester.check_ticker_typing(ticker, check_open=False)
+            RealExchangeTester.check_ticker_typing(ticker)
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_ndax.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_ndax.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_okcoin.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_okcoin.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_okx.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_okx.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,25 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []
+        # "until" param is required: add in tentacle
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50, until=self.get_ms_time())
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_phemex.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_phemex.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,17 @@
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []    # not supported
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_poloniex.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_binance.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,69 +23,81 @@
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestPoloniexRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "poloniex"
+class TestBinanceRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "binanceus"  # use binanceus for tests as binance is blocked in the us
     SYMBOL = "BTC/USDT"
     SYMBOL_2 = "ETH/BTC"
     SYMBOL_3 = "XRP/BTC"
-    TIME_FRAME = TimeFrames.THIRTY_MINUTES  # 1h doesn't exist on Poloniex
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
+            TimeFrames.ONE_MINUTE.value,
+            TimeFrames.THREE_MINUTES.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
+            TimeFrames.ONE_HOUR.value,
             TimeFrames.TWO_HOURS.value,
             TimeFrames.FOUR_HOURS.value,
+            TimeFrames.SIX_HOURS.value,
+            TimeFrames.HEIGHT_HOURS.value,
+            TimeFrames.TWELVE_HOURS.value,
             TimeFrames.ONE_DAY.value,
+            TimeFrames.THREE_DAYS.value,
+            TimeFrames.ONE_WEEK.value,
+            TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
-            assert 1e-08 <= market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_AMOUNT.value] <= 1   # to be fixed in tentacle
-            assert 1e-08 <= market_status[Ecmsc.PRECISION.value][
-                Ecmsc.PRECISION_PRICE.value] < 1    # to be fixed in tentacle
+            assert int(market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_AMOUNT.value]) == \
+                   market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_AMOUNT.value]
+            assert int(market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_PRICE.value]) == \
+                   market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_PRICE.value]
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
-            # invalid values => remove price limit in tentacle
-            self.check_market_status_limits(market_status,
-                                            normal_price_min=1e-05,  # 1000000 for BTC/USDT, 1e-05 for XRP/BTC, lol
-                                            normal_price_max=10000000,
-                                            expect_invalid_price_limit_values=True,
-                                            enable_price_and_cost_comparison=False)
+            self.check_market_status_limits(market_status, expect_invalid_price_limit_values=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 100
+        assert len(symbol_prices) == 500
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
         symbol_prices = await self.get_symbol_prices(limit=200)
         assert len(symbol_prices) == 200
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50)
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
@@ -126,18 +138,18 @@
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
-            assert ticker[Ectc.BID.value] is None
-            assert ticker[Ectc.BID_VOLUME.value] is None
-            assert ticker[Ectc.ASK.value] is None
-            assert ticker[Ectc.ASK_VOLUME.value] is None
+            assert ticker[Ectc.BID.value]
+            assert ticker[Ectc.BID_VOLUME.value]
+            assert ticker[Ectc.ASK.value]
+            assert ticker[Ectc.ASK_VOLUME.value]
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
-            assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
+            assert ticker[Ectc.PREVIOUS_CLOSE.value]
             assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
             RealExchangeTester.check_ticker_typing(ticker)
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_upbit.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_coinex.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,33 +23,36 @@
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestUpbitRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "upbit"
+class TestCoinexRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "coinex"
     SYMBOL = "BTC/USDT"
     SYMBOL_2 = "ETH/BTC"
     SYMBOL_3 = "XRP/BTC"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
             TimeFrames.THREE_MINUTES.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
+            TimeFrames.TWO_HOURS.value,
             TimeFrames.FOUR_HOURS.value,
+            TimeFrames.SIX_HOURS.value,
+            TimeFrames.TWELVE_HOURS.value,
             TimeFrames.ONE_DAY.value,
+            TimeFrames.THREE_DAYS.value,
             TimeFrames.ONE_WEEK.value,
-            TimeFrames.ONE_MONTH.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
@@ -63,41 +66,53 @@
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
             self.check_market_status_limits(market_status, expect_invalid_price_limit_values=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 200
+        # default 100 candles
+        assert len(symbol_prices) == 100
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
-        symbol_prices = await self.get_symbol_prices(limit=200)
-        assert len(symbol_prices) == 200
+        symbol_prices = await self.get_symbol_prices(limit=550)
+        assert len(symbol_prices) == 550
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50)
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
+
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_order_book(self):
-        order_book = await self.get_order_book()
-        assert len(order_book[Ecobic.ASKS.value]) == 15
+        # fetchOrderBook() limit argument must be None, 5/10/20/50. Default is 20
+        order_book = await self.get_order_book(limit=10)
+        assert len(order_book[Ecobic.ASKS.value]) == 10
         assert len(order_book[Ecobic.ASKS.value][0]) == 2
-        assert len(order_book[Ecobic.BIDS.value]) == 15
+        assert len(order_book[Ecobic.BIDS.value]) == 10
         assert len(order_book[Ecobic.BIDS.value][0]) == 2
 
     async def test_get_recent_trades(self):
         recent_trades = await self.get_recent_trades()
         assert len(recent_trades) == 50
         # check trades order (oldest first)
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
@@ -125,18 +140,18 @@
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
-            assert ticker[Ectc.BID.value] is None
+            assert ticker[Ectc.BID.value]
             assert ticker[Ectc.BID_VOLUME.value] is None
-            assert ticker[Ectc.ASK.value] is None
+            assert ticker[Ectc.ASK.value]
             assert ticker[Ectc.ASK_VOLUME.value] is None
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
-            assert ticker[Ectc.PREVIOUS_CLOSE.value]
+            assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
             assert ticker[Ectc.BASE_VOLUME.value]
             assert ticker[Ectc.TIMESTAMP.value]
-            RealExchangeTester.check_ticker_typing(ticker)
+            RealExchangeTester.check_ticker_typing(ticker, check_open=False)
```

### Comparing `OctoBot-Trading-2.3.4/tests_additional/real_exchanges/test_wavesexchange.py` & `OctoBot-Trading-2.3.7/tests_additional/real_exchanges/test_kucoin.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,94 +23,118 @@
 # required to catch async loop context exceptions
 from tests import event_loop
 
 # All test coroutines will be treated as marked.
 pytestmark = pytest.mark.asyncio
 
 
-class TestWavesExchangeRealExchangeTester(RealExchangeTester):
-    EXCHANGE_NAME = "wavesexchange"
-    SYMBOL = "BTC/USDN"
+class TestKucoinRealExchangeTester(RealExchangeTester):
+    EXCHANGE_NAME = "kucoin"
+    SYMBOL = "BTC/USDT"
     SYMBOL_2 = "ETH/BTC"
-    SYMBOL_3 = "WAVES/BTC"
+    SYMBOL_3 = "XRP/BTC"
 
     async def test_time_frames(self):
         time_frames = await self.time_frames()
         assert all(time_frame in time_frames for time_frame in (
             TimeFrames.ONE_MINUTE.value,
+            TimeFrames.THREE_MINUTES.value,
             TimeFrames.FIVE_MINUTES.value,
             TimeFrames.FIFTEEN_MINUTES.value,
             TimeFrames.THIRTY_MINUTES.value,
             TimeFrames.ONE_HOUR.value,
             TimeFrames.TWO_HOURS.value,
             TimeFrames.FOUR_HOURS.value,
             TimeFrames.SIX_HOURS.value,
+            TimeFrames.HEIGHT_HOURS.value,
             TimeFrames.TWELVE_HOURS.value,
             TimeFrames.ONE_DAY.value,
-            TimeFrames.ONE_WEEK.value,
-            TimeFrames.ONE_MONTH.value
+            TimeFrames.ONE_WEEK.value
         ))
 
     async def test_get_market_status(self):
         for market_status in await self.get_market_statuses():
             assert market_status
             assert market_status[Ecmsc.SYMBOL.value] in (self.SYMBOL, self.SYMBOL_2, self.SYMBOL_3)
             assert market_status[Ecmsc.PRECISION.value]
-            assert int(market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_AMOUNT.value]) == \
-                   market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_AMOUNT.value]
-            assert int(market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_PRICE.value]) == \
-                   market_status[Ecmsc.PRECISION.value][Ecmsc.PRECISION_PRICE.value]
+            # on this exchange, precision is a decimal instead of a number of digits
+            assert 0 < market_status[Ecmsc.PRECISION.value][
+                Ecmsc.PRECISION_AMOUNT.value] <= 1  # to be fixed in this exchange tentacle
+            assert 0 < market_status[Ecmsc.PRECISION.value][
+                Ecmsc.PRECISION_PRICE.value] <= 1  # to be fixed in this exchange tentacle
             assert all(elem in market_status[Ecmsc.LIMITS.value]
                        for elem in (Ecmsc.LIMITS_AMOUNT.value,
                                     Ecmsc.LIMITS_PRICE.value,
                                     Ecmsc.LIMITS_COST.value))
-            self.check_market_status_limits(market_status, expect_invalid_price_limit_values=False)
+            # invalid values (should be much lower for XRP/BTC => remove price limit in tentacle
+            self.check_market_status_limits(market_status,
+                                            expect_invalid_price_limit_values=True,
+                                            enable_price_and_cost_comparison=False)
 
     async def test_get_symbol_prices(self):
         # without limit
         symbol_prices = await self.get_symbol_prices()
-        assert len(symbol_prices) == 1440
+        assert len(symbol_prices) == 100
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
         # try with candles limit (used in candled updater)
-        symbol_prices = await self.get_symbol_prices(limit=200)
-        assert len(symbol_prices) == 200
+        symbol_prices = await self.get_symbol_prices(limit=100)
+        assert len(symbol_prices) == 100
         # check candles order (oldest first)
         self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
         # check last candle is the current candle
         assert symbol_prices[-1][PriceIndexes.IND_PRICE_TIME.value] >= self.get_time() - self.get_allowed_time_delta()
 
+        # try with since and limit (used in data collector)
+        assert await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50) == []
+        # "endAt" param is required: add in tentacle
+        symbol_prices = await self.get_symbol_prices(since=self.CANDLE_SINCE, limit=50, endAt=self.get_ms_time())
+        assert len(symbol_prices) == 50
+        # check candles order (oldest first)
+        self.ensure_elements_order(symbol_prices, PriceIndexes.IND_PRICE_TIME.value)
+        # check last candle is the current candle
+        for candle in symbol_prices:
+            assert candle[PriceIndexes.IND_PRICE_TIME.value] >= self.CANDLE_SINCE_SEC
+
     async def test_get_kline_price(self):
         kline_price = await self.get_kline_price()
         assert len(kline_price) == 1
         assert len(kline_price[0]) == 6
         kline_start_time = kline_price[0][PriceIndexes.IND_PRICE_TIME.value]
         # assert kline is the current candle
         assert kline_start_time >= self.get_time() - self.get_allowed_time_delta()
 
     async def test_get_order_book(self):
-        order_book = await self.get_order_book()
-        assert len(order_book[Ecobic.ASKS.value]) == 6
+        # kucoin requires a limit of None, 20 or 100 in order book
+        order_book = await self.get_order_book(limit=20)
+        assert len(order_book[Ecobic.ASKS.value]) == 20
         assert len(order_book[Ecobic.ASKS.value][0]) == 2
-        assert len(order_book[Ecobic.BIDS.value]) == 6
+        assert len(order_book[Ecobic.BIDS.value]) == 20
         assert len(order_book[Ecobic.BIDS.value][0]) == 2
 
     async def test_get_recent_trades(self):
+        # note: on ccxt kucoin recent trades are received in reverse order from exchange and therefore should never be
+        # filtered by limit before reversing (or most recent trades are lost)
         recent_trades = await self.get_recent_trades()
         assert len(recent_trades) == 50
         # check trades order (oldest first)
         self.ensure_elements_order(recent_trades, Ecoc.TIMESTAMP.value)
 
     async def test_get_price_ticker(self):
         ticker = await self.get_price_ticker()
         self._check_ticker(ticker, self.SYMBOL, check_content=True)
 
+    async def test_get_all_currencies_price_ticker(self):
+        tickers = await self.get_all_currencies_price_ticker()
+        for symbol, ticker in tickers.items():
+            self._check_ticker(ticker, symbol)
+
     @staticmethod
     def _check_ticker(ticker, symbol, check_content=False):
         assert ticker[Ectc.SYMBOL.value] == symbol
         assert all(key in ticker for key in (
             Ectc.HIGH.value,
             Ectc.LOW.value,
             Ectc.BID.value,
@@ -121,18 +145,18 @@
             Ectc.CLOSE.value,
             Ectc.LAST.value,
             Ectc.PREVIOUS_CLOSE.value
         ))
         if check_content:
             assert ticker[Ectc.HIGH.value]
             assert ticker[Ectc.LOW.value]
-            assert ticker[Ectc.BID.value] is None
+            assert ticker[Ectc.BID.value]
             assert ticker[Ectc.BID_VOLUME.value] is None
-            assert ticker[Ectc.ASK.value] is None
+            assert ticker[Ectc.ASK.value]
             assert ticker[Ectc.ASK_VOLUME.value] is None
             assert ticker[Ectc.OPEN.value]
             assert ticker[Ectc.CLOSE.value]
             assert ticker[Ectc.LAST.value]
             assert ticker[Ectc.PREVIOUS_CLOSE.value] is None
             assert ticker[Ectc.BASE_VOLUME.value]
-            assert ticker[Ectc.TIMESTAMP.value] is None  # will trigger an 'Ignored incomplete ticker'
-            RealExchangeTester.check_ticker_typing(ticker, check_timestamp=False)
+            assert ticker[Ectc.TIMESTAMP.value]
+            RealExchangeTester.check_ticker_typing(ticker, check_open=False)
```

