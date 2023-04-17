# Comparing `tmp/OctoBot-Backtesting-1.8.0.tar.gz` & `tmp/OctoBot-Backtesting-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Backtesting-1.8.0.tar", last modified: Fri Dec 23 00:31:11 2022, max compression
+gzip compressed data, was "OctoBot-Backtesting-1.8.1.tar", last modified: Mon Apr 17 16:53:37 2023, max compression
```

## Comparing `OctoBot-Backtesting-1.8.0.tar` & `OctoBot-Backtesting-1.8.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.439118 OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-23 00:31:11.000000 OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2022-12-23 00:31:11.000000 OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 00:31:11.000000 OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 00:31:11.000000 OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-23 00:31:11.000000 OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-23 00:31:11.000000 OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.439118 OctoBot-Backtesting-1.8.0/octobot_backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      847 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.439118 OctoBot-Backtesting-1.8.0/octobot_backtesting/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/api/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/api/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/api/data_file_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/api/exchange_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/api/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/backtest_data.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/backtest_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/backtesting.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/channels_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/channels_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/data_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      899 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/exchange_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/exchange_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/social_collector.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/social_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      897 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/data_converter.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/data_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/data/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/data/data_file_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/data/data_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/data_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/data_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/exchange_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/exchange_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/social_importer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/social_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.443119 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/time_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/time/time_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/octobot_backtesting/util/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/util/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/util/backtesting_util.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/octobot_backtesting/util/backtesting_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.439118 OctoBot-Backtesting-1.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/api/test_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/api/test_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/api/test_data_file_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/api/test_exchange_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/api/test_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/tests/importers/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/importers/test_exchange_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/tests/producers/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/producers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 00:31:11.447119 OctoBot-Backtesting-1.8.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2022-12-23 00:30:44.000000 OctoBot-Backtesting-1.8.0/tests/util/test_backtesting_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.566236 OctoBot-Backtesting-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.554236 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-17 16:53:37.000000 OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/exchange_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/api/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.558236 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:53:37.566236 OctoBot-Backtesting-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.554236 OctoBot-Backtesting-1.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_data_file_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_exchange_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/api/test_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/importers/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/importers/test_exchange_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/producers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:53:37.562236 OctoBot-Backtesting-1.8.1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-17 16:53:07.000000 OctoBot-Backtesting-1.8.1/tests/util/test_backtesting_util.py
```

### Comparing `OctoBot-Backtesting-1.8.0/CHANGELOG.md` & `OctoBot-Backtesting-1.8.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.8.1] - 2022-04-17
+### Updated
+- [ExchangeCollector] delete_all
+
 ## [1.8.0] - 2022-12-23
 ### Updated
 - [ChannelsManager] drop unused producers and priority levels
 - cython version
 
 ## [1.7.5] - 2022-10-13
 ### Updated
```

### Comparing `OctoBot-Backtesting-1.8.0/LICENSE` & `OctoBot-Backtesting-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/PKG-INFO` & `OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: OctoBot-Backtesting
-Version: 1.8.0
+Version: 1.8.1
 Summary: OctoBot project backtesting engine
 Home-page: https://github.com/Drakkar-Software/OctoBot-Backtesting
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `OctoBot-Backtesting-1.8.0/OctoBot_Backtesting.egg-info/SOURCES.txt` & `OctoBot-Backtesting-1.8.1/OctoBot_Backtesting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/PKG-INFO` & `OctoBot-Backtesting-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: OctoBot-Backtesting
-Version: 1.8.0
+Version: 1.8.1
 Summary: OctoBot project backtesting engine
 Home-page: https://github.com/Drakkar-Software/OctoBot-Backtesting
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `OctoBot-Backtesting-1.8.0/README.md` & `OctoBot-Backtesting-1.8.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Backtesting [1.8.0](https://github.com/Drakkar-Software/OctoBot-Backtesting/blob/master/CHANGELOG.md)
+# OctoBot-Backtesting [1.8.1](https://github.com/Drakkar-Software/OctoBot-Backtesting/blob/master/CHANGELOG.md)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/aa0b156e99604b3c98923fffeaea6a49)](https://app.codacy.com/gh/Drakkar-Software/OctoBot-Backtesting?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot-Backtesting&utm_campaign=Badge_Grade_Dashboard)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Backtesting.svg)](https://pypi.python.org/pypi/OctoBot-Backtesting/)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot-Backtesting/badge.svg?branch=master)](https://coveralls.io/github/Drakkar-Software/OctoBot-Backtesting?branch=master)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Backtesting/workflows/OctoBot-Backtesting-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Backtesting/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot-Backtesting/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot-Backtesting)
 
 OctoBot backtesting engine package.
```

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 import logging
 
 PROJECT_NAME = "OctoBot-Backtesting"
-VERSION = "1.8.0"
+VERSION = "1.8.1"
 
 logging.getLogger('aiosqlite').setLevel(logging.ERROR)
```

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/api/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/api/backtesting.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/api/data_file.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/api/data_file_converters.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/data_file_converters.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/api/exchange_data_collector.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/exchange_data_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/api/importer.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/api/importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/backtest_data.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/backtest_data.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtest_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/backtesting.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/backtesting.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/channels_manager.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/channels_manager.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/channels_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/data_collector.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/data_collector.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/data_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_bot_snapshot_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_history_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/abstract_exchange_live_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/exchange_collector.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/exchanges/exchange_collector.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/exchanges/exchange_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import json
 import logging
 import abc 
 
 import time
 
 import octobot_commons.constants as commons_constants
-import octobot_commons.enums as commons_enums
 import octobot_backtesting.collectors.data_collector as data_collector
 import octobot_backtesting.enums as enums
 import octobot_backtesting.importers as importers
 
 try:
     import octobot_trading.constants as trading_constants
 except ImportError:
@@ -145,7 +144,17 @@
                                        symbol=symbol, time_frame=time_frame.value,
                                        candle=json.dumps(kline))
         else:
             await self.database.insert_all(enums.ExchangeDataTables.KLINE, timestamp=timestamp,
                                            exchange_name=exchange, cryptocurrency=cryptocurrency,
                                            symbol=symbol, time_frame=time_frame.value,
                                            candle=[json.dumps(kl) for kl in kline])
+
+    async def delete_all(self, table, exchange, cryptocurrency, symbol, time_frame=None):
+        kwargs = {
+            "exchange_name": exchange,
+            "cryptocurrency": cryptocurrency,
+            "symbol": symbol,
+        }
+        if time_frame:
+            kwargs["time_frame"] = time_frame.value
+        await self.database.delete(table, **kwargs)
```

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/social_collector.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/collectors/social/social_collector.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/collectors/social/social_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/constants.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 #  This library is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
+import os
 
 import octobot_commons.enums as enums
 
 CONFIG_BACKTESTING = "backtesting"
 CONFIG_BACKTESTING_DATA_FILES = "files"
 CONFIG_ANALYSIS_ENABLED_OPTION = "post_analysis_enabled"
 CONFIG_BACKTESTING_OTHER_MARKETS_STARTING_PORTFOLIO = 10000
 BACKTESTING_DATA_OHLCV = "ohlcv"
 BACKTESTING_DATA_TRADES = "trades"
-BACKTESTING_FILE_PATH = f"{CONFIG_BACKTESTING}/data"
+BACKTESTING_FILE_PATH = os.path.join(CONFIG_BACKTESTING, "data")
 BACKTESTING_DATA_FILE_EXT = ".data"
 BACKTESTING_DATA_FILE_TEMP_EXT = ".part"
 BACKTESTING_DATA_FILE_SEPARATOR = "_"
 BACKTESTING_DATA_FILE_TIME_WRITE_FORMAT = '%Y%m%d_%H%M%S'
 BACKTESTING_DATA_FILE_TIME_READ_FORMAT = BACKTESTING_DATA_FILE_TIME_WRITE_FORMAT.replace("_", "")
 BACKTESTING_DATA_FILE_TIME_DISPLAY_FORMAT = '%d %B %Y at %H:%M:%S'
 BACKTESTING_DEFAULT_JOIN_TIMEOUT = 1800  # 30min
```

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/data_converter.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/converters/data_converter.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/converters/data_converter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/data/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/data/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/data/data_file_manager.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/data/data_file_manager.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/data/data_file_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/enums.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/errors.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/data_importer.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/data_importer.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/data_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/exchange_importer.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/exchange_importer.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/exchange_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/util.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/exchanges/util.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/exchanges/util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/social_importer.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/importers/social/social_importer.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/importers/social/social_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time_updater.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/channel/time_updater.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/channel/time_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/time_manager.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/time/time_manager.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/time/time_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/util/__init__.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/util/__init__.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/util/backtesting_util.pxd` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/octobot_backtesting/util/backtesting_util.py` & `OctoBot-Backtesting-1.8.1/octobot_backtesting/util/backtesting_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/setup.py` & `OctoBot-Backtesting-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/api/__init__.py` & `OctoBot-Backtesting-1.8.1/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/api/test_backtesting.py` & `OctoBot-Backtesting-1.8.1/tests/api/test_backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/api/test_data_file.py` & `OctoBot-Backtesting-1.8.1/tests/api/test_data_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/api/test_data_file_converters.py` & `OctoBot-Backtesting-1.8.1/tests/api/test_data_file_converters.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/api/test_exchange_data_collector.py` & `OctoBot-Backtesting-1.8.1/tests/api/test_exchange_data_collector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/api/test_importer.py` & `OctoBot-Backtesting-1.8.1/tests/api/test_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/importers/__init__.py` & `OctoBot-Backtesting-1.8.1/tests/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/importers/test_exchange_importer.py` & `OctoBot-Backtesting-1.8.1/tests/importers/test_exchange_importer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/producers/__init__.py` & `OctoBot-Backtesting-1.8.1/tests/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/util/__init__.py` & `OctoBot-Backtesting-1.8.1/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Backtesting-1.8.0/tests/util/test_backtesting_util.py` & `OctoBot-Backtesting-1.8.1/tests/util/test_backtesting_util.py`

 * *Files identical despite different names*

