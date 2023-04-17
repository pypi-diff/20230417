# Comparing `tmp/coinlib-2.2.1.tar.gz` & `tmp/coinlib-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coinlib-2.2.1.tar", last modified: Wed Mar 22 20:17:11 2023, max compression
+gzip compressed data, was "dist/coinlib-2.2.2.tar", last modified: Mon Apr 17 07:56:52 2023, max compression
```

## Comparing `coinlib-2.2.1.tar` & `coinlib-2.2.2.tar`

### file list

```diff
@@ -1,132 +1,134 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.946020 coinlib-2.2.1/
--rw-r--r--   0 root         (0) root         (0)      642 2023-03-22 20:17:11.945103 coinlib-2.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.913017 coinlib-2.2.1/coinlib/
--rw-rw-rw-   0 root         (0) root         (0)    27241 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/BasicJob.py
--rw-rw-rw-   0 root         (0) root         (0)     7817 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/BasicJobSessionStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/ChartsFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9331 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/ChartsIndicatorJob.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/ChartsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/CoinlibCrypto.py
--rw-rw-rw-   0 root         (0) root         (0)     3625 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/CoinlibDataInterface.py
--rw-rw-rw-   0 root         (0) root         (0)    26721 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/DataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/Functions.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/InfluxDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     3985 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/PluginLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     6388 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/PluginsWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5960 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/Registrar.py
--rw-rw-rw-   0 root         (0) root         (0)    17647 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/Simulator.py
--rw-rw-rw-   0 root         (0) root         (0)    12594 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/WorkerJobProcess.py
--rw-rw-rw-   0 root         (0) root         (0)     5435 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.918518 coinlib-2.2.1/coinlib/broker/
--rw-rw-rw-   0 root         (0) root         (0)     7229 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/Broker.py
--rw-rw-rw-   0 root         (0) root         (0)     4411 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/BrokerDTO.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/CoinlibBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/CoinlibBrokerFuture.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/CoinlibBrokerMargin.py
--rw-rw-rw-   0 root         (0) root         (0)     1160 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/CoinlibBrokerSpot.py
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/CoinlibSessionManager.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.920351 coinlib-2.2.1/coinlib/brokerWorker/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/brokerWorker/BrokerFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     7841 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/brokerWorker/BrokerSession.py
--rw-rw-rw-   0 root         (0) root         (0)     2930 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/brokerWorker/BrokerSessionWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/brokerWorker/BrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      806 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/brokerWorker/TestProtocolResult.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/brokerWorker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/coinlibFactory.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.922185 coinlib-2.2.1/coinlib/data/
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/data/CollectionInterface.py
--rw-rw-rw-   0 root         (0) root         (0)    11386 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/data/DataTable.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    78322 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/dataWorker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   162652 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/dataWorker_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.923101 coinlib-2.2.1/coinlib/drawable/
--rw-rw-rw-   0 root         (0) root         (0)     3528 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/drawable/CoinlibDrawable.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/drawable/DrawableComponent.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/drawable/WindowGrid.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/drawable/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.924018 coinlib-2.2.1/coinlib/event/
--rw-rw-rw-   0 root         (0) root         (0)     2820 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/event/EventConsumer.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/event/EventInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.926768 coinlib-2.2.1/coinlib/feature/
--rw-rw-rw-   0 root         (0) root         (0)    13862 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/CoinlibFeature.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/CoinlibFeatureFetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/CoinlibFeatureLake.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/CoinlibFeatureProcessor.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/FeatureDTO.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/FeatureFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     9545 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/FeatureWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     6042 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/Features.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/feature/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13456 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/helper.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/index.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.934102 coinlib-2.2.1/coinlib/logics/
--rw-rw-rw-   0 root         (0) root         (0)    13495 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/Logic.py
--rw-rw-rw-   0 root         (0) root         (0)     8794 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicBasicWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicDTo.py
--rw-rw-rw-   0 root         (0) root         (0)     7477 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicJob.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicLoader.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOfflineJob.py
--rw-rw-rw-   0 root         (0) root         (0)     9819 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOfflineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOfflineWorkerData.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOfflineWorkerScreener.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOfflineWorkerTrader.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOnlineDataWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOnlineJob.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOnlineScreenerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOnlineTraderWorker.py
--rw-rw-rw-   0 root         (0) root         (0)    14919 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOnlineWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8512 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicRegistrationInstance.py
--rw-rw-rw-   0 root         (0) root         (0)    16758 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/LogicTestBrokerWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.935019 coinlib-2.2.1/coinlib/logics/broker/
--rw-rw-rw-   0 root         (0) root         (0)     3107 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/broker/LogicBrokerInterface.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/broker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.935936 coinlib-2.2.1/coinlib/logics/manager/
--rw-rw-rw-   0 root         (0) root         (0)     7098 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/manager/LogicJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     8814 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/manager/LogicManager.py
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/manager/PortfolioModel.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/manager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.937769 coinlib-2.2.1/coinlib/logics/offlineManager/
--rw-rw-rw-   0 root         (0) root         (0)    20282 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
--rw-rw-rw-   0 root         (0) root         (0)    11492 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/offlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.938686 coinlib-2.2.1/coinlib/logics/onlineManager/
--rw-rw-rw-   0 root         (0) root         (0)     6706 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/logics/onlineManager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.940519 coinlib-2.2.1/coinlib/notification/
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/notification/Notification.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/notification/NotificationFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5781 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/notification/NotificationWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.943270 coinlib-2.2.1/coinlib/statistics/
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/StatisticMethodJob.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/StatisticRuleJob.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/Statistics.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/StatisticsMethodFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/StatisticsMethodWorker.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/StatisticsRuleFactory.py
--rw-rw-rw-   0 root         (0) root         (0)     6204 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/StatisticsRuleWorker.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/statistics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.944186 coinlib-2.2.1/coinlib/symbols/
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/symbols/SymbolFactory.py
--rw-rw-rw-   0 root         (0) root         (0)    14991 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/symbols/SymbolWorker.py
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/symbols/Symbols.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-22 20:16:55.000000 coinlib-2.2.1/coinlib/symbols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.915767 coinlib-2.2.1/coinlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2023-03-22 20:17:11.000000 coinlib-2.2.1/coinlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3744 2023-03-22 20:17:11.000000 coinlib-2.2.1/coinlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 20:17:11.000000 coinlib-2.2.1/coinlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-03-22 20:17:11.000000 coinlib-2.2.1/coinlib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-03-22 20:17:11.000000 coinlib-2.2.1/coinlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-22 20:17:11.000000 coinlib-2.2.1/coinlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-22 20:17:11.946020 coinlib-2.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-03-22 20:16:55.000000 coinlib-2.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 20:17:11.945103 coinlib-2.2.1/test/
--rw-rw-rw-   0 root         (0) root         (0)     4048 2023-03-22 20:16:55.000000 coinlib-2.2.1/test/testchartworker.py
--rw-rw-rw-   0 root         (0) root         (0)    10860 2023-03-22 20:16:55.000000 coinlib-2.2.1/test/testcross.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.215870 coinlib-2.2.2/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-04-17 07:56:52.214870 coinlib-2.2.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.179867 coinlib-2.2.2/coinlib/
+-rw-rw-rw-   0 root         (0) root         (0)    27933 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/BasicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     7817 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/BasicJobSessionStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/ChartsFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9331 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/ChartsIndicatorJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     9308 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/ChartsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/CoinlibCrypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     3625 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/CoinlibDataInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     8338 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/CoinlibWorkspace.py
+-rw-rw-rw-   0 root         (0) root         (0)    26721 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/DataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5777 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/Functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/InfluxDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     3985 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/PluginLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     6388 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/PluginsWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5960 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/Registrar.py
+-rw-rw-rw-   0 root         (0) root         (0)    17647 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/Simulator.py
+-rw-rw-rw-   0 root         (0) root         (0)    12973 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/WorkerJobProcess.py
+-rw-rw-rw-   0 root         (0) root         (0)     5812 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.184868 coinlib-2.2.2/coinlib/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     7229 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/Broker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4411 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/BrokerDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBrokerFuture.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBrokerMargin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1160 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibBrokerSpot.py
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/CoinlibSessionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.187868 coinlib-2.2.2/coinlib/brokerWorker/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     7841 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerSession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerSessionWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/BrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      806 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/TestProtocolResult.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/brokerWorker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/coinlibFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.188868 coinlib-2.2.2/coinlib/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/data/CollectionInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/data/DataTable.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    78656 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/dataWorker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   164353 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/dataWorker_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.190868 coinlib-2.2.2/coinlib/drawable/
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/CoinlibDrawable.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/DrawableComponent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/WindowGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/drawable/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.191868 coinlib-2.2.2/coinlib/event/
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/event/EventConsumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/event/EventInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.194868 coinlib-2.2.2/coinlib/feature/
+-rw-rw-rw-   0 root         (0) root         (0)    13862 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeature.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeatureFetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeatureLake.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/CoinlibFeatureProcessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/FeatureDTO.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/FeatureFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     9545 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/FeatureWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/Features.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/feature/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13456 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.202869 coinlib-2.2.2/coinlib/logics/
+-rw-rw-rw-   0 root         (0) root         (0)    13495 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/Logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     8794 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicBasicWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicDTo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)    10021 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerData.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerScreener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerTrader.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineDataWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineScreenerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineTraderWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14919 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOnlineWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8512 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicRegistrationInstance.py
+-rw-rw-rw-   0 root         (0) root         (0)    16758 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/LogicTestBrokerWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.203869 coinlib-2.2.2/coinlib/logics/broker/
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/broker/LogicBrokerInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/broker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.204869 coinlib-2.2.2/coinlib/logics/manager/
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/LogicJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8814 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/LogicManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4375 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/PortfolioModel.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/manager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.206869 coinlib-2.2.2/coinlib/logics/offlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)    20273 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11492 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/offlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.207870 coinlib-2.2.2/coinlib/logics/onlineManager/
+-rw-rw-rw-   0 root         (0) root         (0)     6706 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/onlineManager/LogicOnlineJobBroker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/logics/onlineManager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.208870 coinlib-2.2.2/coinlib/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/Notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/NotificationFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5781 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/NotificationWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.211870 coinlib-2.2.2/coinlib/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticMethodJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticRuleJob.py
+-rw-rw-rw-   0 root         (0) root         (0)     6228 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/Statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsMethodFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsMethodWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsRuleFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/StatisticsRuleWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/statistics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.213870 coinlib-2.2.2/coinlib/symbols/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/SymbolFactory.py
+-rw-rw-rw-   0 root         (0) root         (0)    14991 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/SymbolWorker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/Symbols.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 07:56:35.000000 coinlib-2.2.2/coinlib/symbols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.181867 coinlib-2.2.2/coinlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 07:56:52.000000 coinlib-2.2.2/coinlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 07:56:52.215870 coinlib-2.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-17 07:56:35.000000 coinlib-2.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 07:56:52.214870 coinlib-2.2.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)     4048 2023-04-17 07:56:35.000000 coinlib-2.2.2/test/testchartworker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10860 2023-04-17 07:56:35.000000 coinlib-2.2.2/test/testcross.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-04-17 07:56:35.000000 coinlib-2.2.2/test/testplot.py
```

### Comparing `coinlib-2.2.1/PKG-INFO` & `coinlib-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.1
+Version: 2.2.2
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.1/coinlib/BasicJob.py` & `coinlib-2.2.2/coinlib/BasicJob.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,18 +479,35 @@
                     "value": data["data"][i],
                     "distance_index": math.floor(distance.seconds/60) if distance.seconds > 0 else 0,
                     "distance": distance
                 })
         relevantData.reverse()
         return relevantData
 
+    def subtract(self, data_or_name1, data_or_name2):
+        if type(data_or_name1) == str:
+            data_or_name1 = self.get(data_or_name1)
+        if type(data_or_name2) == str:
+            data_or_name2 = self.get(data_or_name2)
+
+        if len(data_or_name1) > len(data_or_name2):
+            data_or_name1 = data_or_name1[len(data_or_name1)-len(data_or_name2):]
+        elif len(data_or_name1) < len(data_or_name2):
+            data_or_name2 = data_or_name2[len(data_or_name2)-len(data_or_name1):]
+
+        return data_or_name1 - data_or_name2
+
 
     def get(self, name, index=None, filterNone = False, replaceNone=None, limit=None,
             keepPaddingNones=False, with_dates=False, clear_nan=True, to_date=None, from_date=None):
 
+        # if the name is a number, so we return it directly
+        if type(name) == int or type(name) == float:
+            return name
+
         data = None
         try:
                 maybe_col_name = name
                 child_col_name = ""
                 if ":" in maybe_col_name:
                     maybe_col_name = maybe_col_name.split(":")[0]
                     child_col_name = ":"+name.split(":")[1]
```

### Comparing `coinlib-2.2.1/coinlib/BasicJobSessionStorage.py` & `coinlib-2.2.2/coinlib/BasicJobSessionStorage.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/ChartsIndicatorJob.py` & `coinlib-2.2.2/coinlib/ChartsIndicatorJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/ChartsWorker.py` & `coinlib-2.2.2/coinlib/ChartsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/CoinlibCrypto.py` & `coinlib-2.2.2/coinlib/CoinlibCrypto.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/CoinlibDataInterface.py` & `coinlib-2.2.2/coinlib/CoinlibDataInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/DataWorker.py` & `coinlib-2.2.2/coinlib/DataWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/Functions.py` & `coinlib-2.2.2/coinlib/Functions.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/InfluxDatabase.py` & `coinlib-2.2.2/coinlib/InfluxDatabase.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/PluginLoader.py` & `coinlib-2.2.2/coinlib/PluginLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/PluginsWorker.py` & `coinlib-2.2.2/coinlib/PluginsWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/Registrar.py` & `coinlib-2.2.2/coinlib/Registrar.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/Simulator.py` & `coinlib-2.2.2/coinlib/Simulator.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/WorkerJobProcess.py` & `coinlib-2.2.2/coinlib/WorkerJobProcess.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     feature: str
     original: any
     subfeature: str
     name: str
 
 class WorkerJobProcess:
     def __init__(self, workerJob, factory):
+        self.workerChannel = None
         if factory is not None:
             self.workerChannel = factory.createChannel()
         self.registrar = Registrar()
         self.chipmunkDb = None
         ##self.chipmunkDb = ChipmunkDb(self.registrar.chipmunkdb)
         if factory is not None:
             self.stub = stats.DataWorkerStub(self.workerChannel)
@@ -282,19 +283,21 @@
         self.onFinishedProcess()
     
     def run(self):
         pass
 
     def onErrorProcess(self, e):
         self.stop()
-        self.factory.onWorkerJobProcessError(self, e)
+        if self.factory is not None:
+            self.factory.onWorkerJobProcessError(self, e)
 
     def onFinishedProcess(self):
         self.stop()
-        self.factory.onWorkerJobProcessFinished(self)
+        if self.factory is not None:
+            self.factory.onWorkerJobProcessFinished(self)
         
     def stop(self):
         self.stopped = True
         #self.listenThread.join()
         
     def onBeforeDownloadData(self):
         pass
@@ -311,14 +314,15 @@
             self.dataFrame = self.getWorkerJobDataFrame(self.workerJob)
             if (self.stopped == False):
                 self.stop()
                 self.stopped = True
 
             self.listenThread = threading.Thread(target=self.runProcess, daemon=True)
             self.listenThread.start()
+            self.onWorkerJobProcessStarted(self.listenThread)
         except Exception as e:
             self.onErrorProcess(e)
             return False
             
         return True
 
     def startProcessWithDataFrame(self, dataFrame):
@@ -336,18 +340,25 @@
 
         except Exception as e:
             self.onErrorProcess(e)
             return False
 
         return True
 
+    def onWorkerJobProcessStarted(self, thread):
+        pass
+
+    def onWorkerJobProcessStarted(self, thread):
+        pass
+
     def startProcess(self):
         
         downloadThread = threading.Thread(target=self.downloadAndRunprocess, daemon=True)
         downloadThread.start()
+        self.onWorkerJobProcessStarted(downloadThread)
 
-        pass
+        return self.finishedData
 
     def setConfig(self, configuration):
         pass
```

### Comparing `coinlib-2.2.1/coinlib/__init__.py` & `coinlib-2.2.2/coinlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 pip_install_or_ignore("ipynb_path", "ipynb-path", "0.1.4")
 # pip_install_or_ignore("import_ipynb", "import_ipynb")
 pip_install_or_ignore("websocket", "websocket-client", "0.58.0")
 pip_install_or_ignore("plotly", "plotly", "4.14.3")
 pip_install_or_ignore("simplejson", "simplejson", "3.17.2")
 pip_install_or_ignore("aio_pika", "aio_pika", "6.8.0")
 pip_install_or_ignore("grpc", "grpcio-tools", "1.35.0")
-pip_install_or_ignore("matplotlib", "matplotlib", "3.3.4")
+pip_install_or_ignore("matplotlib", "matplotlib", "3.7.1")
+pip_install_or_ignore("mplfinance", "mplfinance", "0.12.9b7")
 pip_install_or_ignore("pandas", "pandas", "1.2.4")
 #pip_install_or_ignore("timeit", "timeit")
 pip_install_or_ignore("dateutil", "python-dateutil", "2.8.1")
 pip_install_or_ignore("chipmunkdb", "chipmunkdb-python-client", "2.0.6")
 
 global coinlib_job_task
 
 from coinlib.feature import Features
 from coinlib.Registrar import Registrar
+from coinlib.logics.LogicJob import LogicJob
 from coinlib.logics.Logic import Logic
 from coinlib.Functions import Functions
 from coinlib.CoinlibDataInterface import CoinlibDataInterface
+from coinlib.CoinlibWorkspace import CoinlibWorkspace
 from coinlib.statistics.Statistics import Statistics
 from coinlib.Simulator import Simulator
 from coinlib.ChartsIndicatorJob import ChartsIndicatorJob
 from coinlib.broker.Broker import Broker
 from coinlib.notification.Notification import Notification
 from coinlib.symbols.Symbols import Symbols
 from coinlib.helper import trendline, to_trendline
@@ -67,14 +70,18 @@
 def addLogicToWorkspace(identifier, type, logicComponentId, params=None, workspaceId=registrar.workspaceId,
                         autostart=True, autoStartLogic=False):
     return logic.addLogicToWorkspace(identifier,
                                      type,
                                      logicComponentId,
                                      params, workspaceId, autostart, autoStartLogic)
 
+def connectAsDataAnalytics(apiKey=None, apiKeySecret=None, workspaceId=None):
+    logicModule = "offlineLogics"
+    return connectCoinlib(apiKey, apiKeySecret, workspaceId=workspaceId, worker_modules=[logicModule])
+
 def connectAsLogic(apiKey=None, apiKeySecret=None, workspaceId=None):
     logicModule = "offlineLogics"
     if registrar.isLiveEnvironment():
         logicModule = "onlineLogics"
     return connectCoinlib(apiKey, apiKeySecret, workspaceId=workspaceId, worker_modules=[logicModule])
 
 def connectAsBrokerSymbol(apiKey=None, apiKeySecret=None, workspaceId=None):
```

### Comparing `coinlib-2.2.1/coinlib/broker/Broker.py` & `coinlib-2.2.2/coinlib/broker/Broker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/broker/BrokerDTO.py` & `coinlib-2.2.2/coinlib/broker/BrokerDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/broker/CoinlibBroker.py` & `coinlib-2.2.2/coinlib/broker/CoinlibBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/broker/CoinlibBrokerFuture.py` & `coinlib-2.2.2/coinlib/broker/CoinlibBrokerFuture.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/broker/CoinlibBrokerMargin.py` & `coinlib-2.2.2/coinlib/broker/CoinlibBrokerMargin.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/broker/CoinlibBrokerSpot.py` & `coinlib-2.2.2/coinlib/broker/CoinlibBrokerSpot.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/brokerWorker/BrokerSession.py` & `coinlib-2.2.2/coinlib/brokerWorker/BrokerSession.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/brokerWorker/BrokerSessionWorker.py` & `coinlib-2.2.2/coinlib/brokerWorker/BrokerSessionWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/brokerWorker/BrokerWorker.py` & `coinlib-2.2.2/coinlib/brokerWorker/BrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/brokerWorker/TestProtocolResult.py` & `coinlib-2.2.2/coinlib/brokerWorker/TestProtocolResult.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/coinlibFactory.py` & `coinlib-2.2.2/coinlib/coinlibFactory.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/config.py` & `coinlib-2.2.2/coinlib/config.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/data/CollectionInterface.py` & `coinlib-2.2.2/coinlib/data/CollectionInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/data/DataTable.py` & `coinlib-2.2.2/coinlib/data/DataTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,17 @@
                         le = LastEntry()
                         le.value = e
                         le.distanceTicks = length
                         return le
             return None
         return None
 
+    def getLastIndex(self):
+        return self.index[-1]
+
     def getLast(self, name, maxLength=100):
         row = self.getColumn(name)
         if row is False:
             return False
         length = 0
         if row is not None:
             for i, e in enumerate(reversed(row)):
```

### Comparing `coinlib-2.2.1/coinlib/dataWorker_pb2.py` & `coinlib-2.2.2/coinlib/dataWorker_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61taWorker.proto\x12\x07\x63oinlib\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x19google/protobuf/any.proto\"P\n\tWorkerJob\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\"k\n\x0eWorkerJobError\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\x12\x14\n\x0c\x65rrorMessage\x18\x04 \x01(\t\"E\n\x16WorkerAvailablePlugins\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"\xb7\x01\n\x06Worker\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x02 \x01(\t\x12\x13\n\x0bworker_mode\x18\x03 \x01(\t\x12\x39\n\x10\x61vailablePlugins\x18\x04 \x03(\x0b\x32\x1f.coinlib.WorkerAvailablePlugins\x12\n\n\x02os\x18\x05 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x06 \x01(\t\x12\x15\n\ractiveModules\x18\x07 \x03(\t\"\x1a\n\x07RowData\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\";\n\x15WorkerJobDataResponse\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x16\n\x14WorkerJobDataPartial\"\xec\x01\n\x1a\x43hartWorkerPartialDataInfo\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x02\x12\x0f\n\x07opacity\x18\x05 \x01(\x02\x12\x15\n\rchartTypeIcon\x18\x06 \x01(\t\x12\x0f\n\x07tooltip\x18\x07 \x01(\x08\x12\r\n\x05\x63hart\x18\x08 \x01(\t\x12\x13\n\x0b\x63onnectGaps\x18\t \x01(\x08\x12\x11\n\tfill_from\x18\n \x01(\x02\x12\x0c\n\x04\x66ill\x18\x0b \x01(\t\x12\x12\n\nadditional\x18\x0c \x01(\t\"\xad\x01\n\x1d\x43hartsWorkerPartialDataLayout\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x02 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x36\n\tchartInfo\x18\x03 \x01(\x0b\x32#.coinlib.ChartWorkerPartialDataInfo\"\xdd\x01\n\x14\x43hartWorkerIndicator\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07\x66\x65\x61ture\x18\x03 \x01(\t\x12\x12\n\nsubfeature\x18\x04 \x01(\t\x12\r\n\x05short\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\t\x12\x11\n\telementId\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tid_output\x18\n \x01(\t\x12\x10\n\x08\x66inished\x18\x0b \x01(\x08\x12\x0f\n\x07\x63hartId\x18\x0c \x01(\t\"\xdc\x02\n ChartWorkerIndicatorRegistration\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x11\n\tid_output\x18\x06 \x01(\t\x12\x0e\n\x06inputs\x18\x07 \x01(\x0c\x12\x0c\n\x04mode\x18\x08 \x01(\t\x12\x19\n\x11short_description\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07process\x18\x0b \x01(\t\x12\x16\n\x0eunstablePeriod\x18\x0c \x01(\x08\x12\x19\n\x11\x64ynamicTimeseries\x18\r \x01(\x08\x12\x0e\n\x06plugin\x18\x0e \x01(\t\x12\x15\n\rpluginVersion\x18\x0f \x01(\t\x12\x11\n\tcode_type\x18\x10 \x01(\t\x12\x0c\n\x04\x63ode\x18\x11 \x01(\t\"n\n!ChartWorkerIndicatorConfigElement\x12\x30\n\tindicator\x18\x01 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x17\n\x0findicatorConfig\x18\x02 \x01(\x0c\"\xac\x01\n\x12\x43hartsWorkerConfig\x12<\n\x08\x65lements\x18\x01 \x03(\x0b\x32*.coinlib.ChartWorkerIndicatorConfigElement\x12-\n\x08\x63hildren\x18\x02 \x01(\x0b\x32\x1b.coinlib.ChartsWorkerConfig\x12)\n\tchartData\x18\x03 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\"-\n\x0eStatisticInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"A\n\tDataError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x11\n\terrorCode\x18\x02 \x01(\x03\x12\x10\n\x08\x63ritical\x18\x03 \x01(\x08\"\x89\x01\n\x0eIndicatorError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x03 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\"\xa3\x01\n\x1aStatisticRuleFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa5\x01\n\x1cStatisticMethodFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xb2\x01\n\"StatisticsMethodWorkerWindowConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\x10\n\x08windowId\x18\x03 \x01(\t\x12)\n\tchartData\x18\x04 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x05 \x01(\x0b\x32\x17.coinlib.ParameterTable\"R\n\x13ParameterTableEntry\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08required\x18\x04 \x01(\x08\"B\n\x0eParameterTable\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.coinlib.ParameterTableEntry\"z\n\rChartDataInfo\x12\x10\n\x08\x63hart_id\x18\x01 \x01(\t\x12\x14\n\x0c\x63hart_prefix\x18\x02 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\t\x12\x13\n\x0b\x61\x63tivity_id\x18\x04 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x05 \x01(\t\"\xf6\x02\n\x1aStatisticsRuleWorkerConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x05rules\x18\x02 \x03(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x19\n\x11statisticFunction\x18\x03 \x01(\t\x12?\n\x06inputs\x18\x04 \x03(\x0b\x32/.coinlib.StatisticsRuleWorkerConfig.InputsEntry\x12\x12\n\ncombinator\x18\x05 \x01(\t\x12\x16\n\x0e\x63ombinator_not\x18\x06 \x01(\x08\x12\x0c\n\x04type\x18\x07 \x01(\t\x12)\n\tchartData\x18\x08 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x1a\x46\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.coinlib.StatisticInput:\x02\x38\x01\"\xa8\x01\n\x1eStatisticsRuleWorkerConfigType\x12\x33\n\x04rule\x18\x01 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfigH\x00\x12\x43\n\x0cmethodWindow\x18\x02 \x01(\x0b\x32+.coinlib.StatisticsMethodWorkerWindowConfigH\x00\x42\x0c\n\ntest_oneof\"\xb4\x01\n\x1cStatisticsBulkedWorkerConfig\x12\x38\n\x07\x63onfigs\x18\x01 \x03(\x0b\x32\'.coinlib.StatisticsRuleWorkerConfigType\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x03 \x01(\x0b\x32\x17.coinlib.ParameterTable\"\x9f\x01\n\x16StatisticFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa7\x01\n\x1cStatisticMethodPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x12\n\ndocumentId\x18\x03 \x01(\t\x12\r\n\x05width\x18\x04 \x01(\t\x12\x0e\n\x06height\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x10\n\x08windowId\x18\x07 \x01(\t\"\xa6\x01\n\x1aStatisticRulePartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12:\n\rstatisticRule\x18\x02 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x14\n\x0c\x63ollectionid\x18\x03 \x01(\t\x12\x12\n\nresultName\x18\x05 \x01(\t\"\xa2\x01\n\x1cStatisticBulkedPartiallyData\x12;\n\nmethodData\x18\x01 \x01(\x0b\x32%.coinlib.StatisticMethodPartiallyDataH\x00\x12\x37\n\x08ruleData\x18\x02 \x01(\x0b\x32#.coinlib.StatisticRulePartiallyDataH\x00\x42\x0c\n\ntest_oneof\"m\n\x11SymbolBrokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"U\n\x19SymbolBrokerConsumerError\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\"\x95\x02\n\x16SymbolBrokerMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04open\x18\x02 \x01(\x02\x12\r\n\x05\x63lose\x18\x03 \x01(\x02\x12\x0c\n\x04high\x18\x04 \x01(\x02\x12\x0b\n\x03low\x18\x05 \x01(\x02\x12\x0e\n\x06volume\x18\x06 \x01(\x02\x12\r\n\x05trade\x18\x07 \x01(\x02\x12\x10\n\x08\x64\x61tetime\x18\x08 \x01(\t\x12\x11\n\tsymbol_id\x18\t \x01(\t\x12\x0e\n\x06symbol\x18\n \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x0b \x01(\t\x12\x12\n\nevent_time\x18\x0c \x01(\t\x12\x0f\n\x07isfinal\x18\r \x01(\x08\x12\x11\n\tcloseTime\x18\x0e \x01(\t\"\x96\x01\n\x10SymbolBrokerInfo\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\texchanges\x18\x02 \x03(\x0b\x32\x1d.coinlib.SymbolBrokerExchange\x12,\n\x07symbols\x18\x03 \x03(\x0b\x32\x1b.coinlib.SymbolBrokerSymbol\";\n\x15SymbolBrokerOrderbook\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"F\n SymbolBrokerHistoricalMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\xba\x01\n\x14SymbolBrokerExchange\x12\x0c\n\x04icon\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07website\x18\x04 \x01(\t\x12\x15\n\rsymbols_count\x18\x05 \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x06 \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\x07 \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x08 \x01(\x02\"\x8c\x04\n\x12SymbolBrokerSymbol\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x38\n\tassetType\x18\x04 \x01(\x0e\x32%.coinlib.SymbolBrokerSymbol.AssetType\x12>\n\x0c\x63ontractType\x18\x05 \x01(\x0e\x32(.coinlib.SymbolBrokerSymbol.ContractType\x12\x0c\n\x04\x62\x61se\x18\x06 \x01(\t\x12\r\n\x05quote\x18\x07 \x01(\t\x12\x1a\n\x12\x65xchange_symbol_id\x18\x08 \x01(\t\x12\x16\n\x0esize_precision\x18\t \x01(\x02\x12\x17\n\x0fprice_precision\x18\n \x01(\x02\x12\r\n\x05price\x18\x0b \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x0c \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\r \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x0e \x01(\x02\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"O\n\x1cSymbolBrokerBrokerInfoConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\"\xdd\x03\n#SymbolBrokerConsumeMarketdataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12O\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x39.coinlib.SymbolBrokerConsumeMarketdataConfig.ContractType\x12I\n\tassetType\x18\t \x01(\x0e\x32\x36.coinlib.SymbolBrokerConsumeMarketdataConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xda\x03\n\"SymbolBrokerConsumeOrderbookConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12N\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x38.coinlib.SymbolBrokerConsumeOrderbookConfig.ContractType\x12H\n\tassetType\x18\t \x01(\x0e\x32\x35.coinlib.SymbolBrokerConsumeOrderbookConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xb8\x04\n#SymbolBrokerGetHistoricalDataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05start\x18\x07 \x01(\t\x12\x0b\n\x03\x65nd\x18\x08 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\t \x01(\t\x12)\n\tchartData\x18\n \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12O\n\x0c\x63ontractType\x18\x0b \x01(\x0e\x32\x39.coinlib.SymbolBrokerGetHistoricalDataConfig.ContractType\x12I\n\tassetType\x18\x0c \x01(\x0e\x32\x36.coinlib.SymbolBrokerGetHistoricalDataConfig.AssetType\x12\x12\n\nreturnData\x18\r \x01(\x08\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xc5\x02\n\x18SymbolBrokerWorkerConfig\x12;\n\ninfoConfig\x18\x01 \x01(\x0b\x32%.coinlib.SymbolBrokerBrokerInfoConfigH\x00\x12\x45\n\rconsumeConfig\x18\x02 \x01(\x0b\x32,.coinlib.SymbolBrokerConsumeMarketdataConfigH\x00\x12M\n\x16\x63onsumeOrderbookConfig\x18\x03 \x01(\x0b\x32+.coinlib.SymbolBrokerConsumeOrderbookConfigH\x00\x12H\n\x10historicalConfig\x18\x04 \x01(\x0b\x32,.coinlib.SymbolBrokerGetHistoricalDataConfigH\x00\x42\x0c\n\ntest_oneof\"F\n SymbolBrokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"2\n\x1fSymbolBrokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"j\n\x15SymbolBrokerFetchData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12-\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x1f.coinlib.SymbolBrokerMarketData\"u\n$NotificationExtractMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\t\x12\x0f\n\x07options\x18\x04 \x01(\t\"\xd3\x01\n!NotificationSendMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0e\n\x06images\x18\x04 \x01(\t\x12\x0f\n\x07\x62uttons\x18\x05 \x01(\t\x12\x0f\n\x07options\x18\x06 \x01(\t\x12\x13\n\x0b\x63\x61llback_id\x18\x07 \x01(\t\x12\x14\n\x0c\x63\x61llback_url\x18\x08 \x01(\t\x12\x10\n\x08\x63hannels\x18\t \x01(\t\"\xbd\x01\n\x18NotificationWorkerConfig\x12G\n\x11sendMessageConfig\x18\x01 \x01(\x0b\x32*.coinlib.NotificationSendMessageDataConfigH\x00\x12J\n\x11\x65xtractDataConfig\x18\x02 \x01(\x0b\x32-.coinlib.NotificationExtractMessageDataConfigH\x00\x42\x0c\n\ntest_oneof\"Z\n\x11NotificationError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"b\n\x1bNotificationCallbackExtract\x12\x11\n\tbutton_id\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x98\x01\n\x0eLogicComponent\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x18\n\x10logicComponentId\x18\x03 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\x0c\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x14\n\x0clogicDetails\x18\x07 \x01(\t\"\xde\x03\n\x12\x42rokerAccountModel\x12:\n\nbrokerType\x18\x01 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerType\x12\x34\n\x04mode\x18\x02 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerMode\x12\x10\n\x08\x65xchange\x18\x03 \x01(\t\x12\x10\n\x08makerFee\x18\x04 \x01(\x02\x12\x10\n\x08takerFee\x18\x05 \x01(\x02\x12\x39\n\x0cmakerFeeMode\x18\x06 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\x12\x39\n\x0ctakerFeeMode\x18\x07 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\"Q\n\nBrokerType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"1\n\nBrokerMode\x12\x0e\n\nBACKTRADER\x10\x00\x12\t\n\x05PAPER\x10\x01\x12\x08\n\x04LIVE\x10\x02\"$\n\x07\x46\x65\x65Mode\x12\x0e\n\nPERCENTAGE\x10\x00\x12\t\n\x05\x46IXED\x10\x01\"~\n\x0ePortfolioAsset\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x03 \x01(\x02\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\x0e\n\x06locked\x18\x05 \x01(\x02\x12\x11\n\tlastPrice\x18\x06 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x07 \x01(\t\"o\n\x13\x43\x61lculatedBaseMoney\x12\r\n\x05total\x18\x01 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x0f\n\x07summary\x18\x04 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\"\xc0\x01\n\x0ePortfolioModel\x12\'\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x17.coinlib.PortfolioAsset\x12@\n\x1a\x63urrentCalculatedBaseMoney\x18\x02 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\x43\n\x1dhistoricalCalculatedBaseMoney\x18\x03 \x03(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\"\x82\x03\n\x10LogicRunnerLogic\x12)\n\tchartData\x18\x01 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x30\n\x0flogicComponents\x18\x02 \x03(\x0b\x32\x17.coinlib.LogicComponent\x12\x11\n\tstartDate\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x04 \x01(\t\x12*\n\tportfolio\x18\x05 \x01(\x0b\x32\x17.coinlib.PortfolioModel\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\x12/\n\x0eparameterTable\x18\x07 \x01(\x0b\x32\x17.coinlib.ParameterTable\x12\x11\n\tlogicMode\x18\x08 \x01(\t\x12\x15\n\rapp_worker_id\x18\t \x01(\t\x12\x1c\n\x14\x61pp_worker_runner_id\x18\n \x01(\t\x12\x14\n\x0coptions_json\x18\x0b \x01(\t\"\xd5\x01\n\x1eLogicRunnerOfflineWorkerConfig\x12,\n\tlogicInfo\x18\x01 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12+\n\tportfolio\x18\x03 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x18\n\x10\x61\x64vancedDataInfo\x18\x04 \x01(\t\x12\x13\n\x0bonlySignals\x18\x05 \x01(\x08\"\xcf\x04\n\x15LogicRunnerStatistics\x12\x1f\n\x17highestProfitPercentage\x18\x01 \x01(\x02\x12\x1d\n\x15highestLossPercentage\x18\x02 \x01(\x02\x12\x11\n\tsinceDate\x18\x03 \x01(\t\x12\x0e\n\x06\x61tDate\x18\x04 \x01(\t\x12\x11\n\ttradesCnt\x18\x05 \x01(\x02\x12\x35\n\x0f\x63\x61lculatedMoney\x18\x06 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\"\n\x1aunrealizedProfitPercentage\x18\x07 \x01(\x02\x12\x0c\n\x04\x66\x65\x65s\x18\x08 \x01(\x02\x12 \n\x18profitCompletePercentage\x18\t \x01(\x02\x12\x1d\n\x15highestProfitPerGroup\x18\n \x01(\x02\x12\x1b\n\x13highestLossPerGroup\x18\x0b \x01(\x02\x12\x18\n\x10slippagePerGroup\x18\x0c \x01(\x02\x12\x1a\n\x12\x61verageAmountQuote\x18\r \x01(\x02\x12\'\n\x1f\x61verageProfitPercentagePergroup\x18\x0e \x01(\x02\x12\x19\n\x11portfolioTimeline\x18\x0f \x01(\t\x12\x14\n\x0cwinLossRatio\x18\x10 \x01(\x02\x12\x0e\n\x06winCnt\x18\x11 \x01(\x02\x12\x0f\n\x07lossCnt\x18\x12 \x01(\x02\x12\x17\n\x0fsecondsInMarket\x18\x13 \x01(\x02\x12\x1d\n\x15\x61verageSecondsInTrade\x18\x14 \x01(\x02\x12\x10\n\x08\x64rawDown\x18\x15 \x01(\x02\"\xa6\x01\n%LogicRunnerOfflineWorkerPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\npercentage\x18\x02 \x01(\x02\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x05 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"w\n\x1dLogicRunnerOfflineWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xb4\x01\n$LogicRunnerOfflineWorkerFinishedData\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x04 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"@\n\x17WorkerPluginInformation\x12%\n\x06plugin\x18\x01 \x03(\x0b\x32\x15.coinlib.PluginConfig\"<\n\x0eWorkerSettings\x12\x15\n\ractiveModules\x18\x01 \x03(\t\x12\x13\n\x0bworker_mode\x18\x02 \x01(\t\"\'\n\x12WorkerRegistration\x12\x11\n\tworker_id\x18\x01 \x01(\t\"b\n\x15\x43ollectionNodeRequest\x12\x16\n\x0e\x63ollectionName\x18\x01 \x01(\t\x12\r\n\x05stage\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\":\n\x16\x43ollectionNodeResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsize_in_mb\x18\x02 \x01(\t\"`\n\x0c\x45ventRequest\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\r\n\x05stage\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"t\n\x0cPluginConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x13\n\x0b\x66ilecontent\x18\x04 \x01(\t\x12\x10\n\x08testOnly\x18\x05 \x01(\x08\x12\x10\n\x08\x66iletype\x18\x06 \x01(\t\"U\n\x18PluginInstallationOutput\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x15\n\routputMessage\x18\x02 \x01(\t\"\xcb\x01\n\x1dSimulatorChartConfigIndicator\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nsubfeature\x18\x02 \x01(\t\x12\x42\n\x06inputs\x18\x03 \x03(\x0b\x32\x32.coinlib.SimulatorChartConfigIndicator.InputsEntry\x12\x12\n\nchartIndex\x18\x04 \x01(\t\x1a-\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x14SimulatorChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62roker\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\x97\x01\n\x1dSimulatorStatisticChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\xc7\x01\n\x1eSimulatorMethodCallChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\x12-\n\x07methods\x18\x07 \x03(\x0b\x32\x1c.coinlib.SimulatorMethodCall\"@\n\x11SimulatorResponse\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"\x83\x01\n\x1cSymbolBrokerSimulatorRequest\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x13\n\x0btestSymbol1\x18\x04 \x01(\t\x12\x13\n\x0btestSymbol2\x18\x05 \x01(\t\"g\n\x1dSymbolBrokerSimulatorResponse\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"@\n\x1e\x42rokerSimulatorBrokerLoginData\x12\x0e\n\x06\x61pikey\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"\x95\x01\n\x19\x42rokerSimulatorBrokerData\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12:\n\tloginInfo\x18\x02 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x11\n\tassetType\x18\x03 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x04 \x01(\t\"\x98\x01\n\x16\x42rokerSimulatorRequest\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x36\n\nbrokerInfo\x18\x04 \x01(\x0b\x32\".coinlib.BrokerSimulatorBrokerData\x12\x11\n\tpaperMode\x18\x05 \x01(\x08\"\xb2\x01\n\x17\x42rokerSimulatorResponse\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\x12\x11\n\tsessionId\x18\x04 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x05 \x01(\t\x12\x15\n\rtargetdepotId\x18\x06 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"f\n\x1cNotificationSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0e\n\x06inputs\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x10\n\x08\x63hannels\x18\x04 \x01(\t\"c\n\x1dNotificationSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"P\n\x17\x46\x65\x61tureSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\"^\n\x18\x46\x65\x61tureSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"c\n\nLogicInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x85\x02\n\x17LogicTraderRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x84\x02\n\x16LogicAlertRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x83\x02\n\x15LogicDataRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x87\x02\n\x19LogicScreenerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x91\x02\n\x1aWorkspaceLogicRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x18\n\x10logicComponentId\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\x0c\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0e\n\x06plugin\x18\x05 \x01(\t\x12\x15\n\rpluginVersion\x18\x06 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x07 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x10\n\x08workerId\x18\x0b \x01(\t\x12\x11\n\tautostart\x18\x0c \x01(\x08\x12\x16\n\x0e\x61utostartLogic\x18\r \x01(\x08\"\"\n\x0bLogicRunJob\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\"\xb3\x02\n\x0eLogicDataUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05group\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06symbol\x18\x06 \x01(\x08\x12\x10\n\x08\x65xchange\x18\x07 \x01(\x08\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf3\x01\n\x11LogicMonitorEvent\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf6\x01\n\x14LogicCollectionUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xe2\x01\n\x0fLogicEventUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\\\n\x13SymbolBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xe4\x01\n\x18SymbolBrokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12-\n\x07options\x18\x04 \x03(\x0b\x32\x1c.coinlib.SymbolBrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\"V\n\rBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xda\x03\n\x0e\x42rokerExchange\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x34\n\tloginMode\x18\x04 \x01(\x0e\x32!.coinlib.BrokerExchange.LoginMode\x12;\n\rcontractTypes\x18\x05 \x03(\x0e\x32$.coinlib.BrokerExchange.ContractType\x12\x35\n\nassetTypes\x18\x06 \x03(\x0e\x32!.coinlib.BrokerExchange.AssetType\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0bsupportDemo\x18\x08 \x01(\x08\x12\x13\n\x0bsupportLive\x18\t \x01(\x08\x12\x1a\n\x12positionModeFuture\x18\n \x01(\t\"\x18\n\tLoginMode\x12\x0b\n\x07\x41PI_KEY\x10\x00\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\xa8\x03\n\x12\x42rokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\'\n\x07options\x18\x04 \x03(\x0b\x32\x16.coinlib.BrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12*\n\texchanges\x18\x0b \x03(\x0b\x32\x17.coinlib.BrokerExchange\x12\x45\n\x0b\x62rokerTypes\x18\x0c \x03(\x0e\x32\x30.coinlib.BrokerRegistration.SupportedBrokerTypes\"[\n\x14SupportedBrokerTypes\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"?\n\x0f\x42rokerPortfolio\x12,\n\x05\x61sset\x18\x01 \x03(\x0b\x32\x1d.coinlib.BrokerPortfolioAsset\"Z\n\x14\x42rokerPortfolioAsset\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x11\n\tlastPrice\x18\x04 \x01(\x02\"\x84\x03\n\x18\x42rokerSessionAccountInfo\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x44\n\x0c\x63ontractType\x18\x02 \x01(\x0e\x32..coinlib.BrokerSessionAccountInfo.ContractType\x12>\n\tassetType\x18\x03 \x01(\x0e\x32+.coinlib.BrokerSessionAccountInfo.AssetType\x12:\n\tloginInfo\x18\x04 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x0f\n\x07sandbox\x18\x05 \x01(\x08\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\x9b\x01\n\x1c\x42rokerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\"\xf4\x01\n\x14\x42rokerInfoTestConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\"g\n\x12\x42rokerWorkerConfig\x12\x43\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"@\n\x1a\x42rokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\",\n\x19\x42rokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"\x18\n\x16\x42rokerStartSessionInfo\"g\n\x0b\x42rokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"j\n\x0e\x42rokerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x15\n\rbrokerCommand\x18\x03 \x01(\t\x12\x1b\n\x13\x62rokerCommandParams\x18\x04 \x01(\t\".\n\x19\x42rokerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"P\n\x14\x42rokerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"d\n\x19\x42rokerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"e\n\x0f\x42rokerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\".\n\x19\x42rokerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"J\n\x16\x42rokerTestProtocolData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\"\x9c\x01\n\x0f\x41ppWorkerConfig\x12\x46\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32(.coinlib.AppWorkerInfoStartSessionConfigH\x00\x12\x33\n\ntestConfig\x18\x02 \x01(\x0b\x32\x1d.coinlib.BrokerInfoTestConfigH\x00\x42\x0c\n\ntest_oneof\"\xa9\x02\n\x1f\x41ppWorkerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x02 \x01(\t\x12,\n\tlogicInfo\x18\x03 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12;\n\x0c\x62rokerConfig\x18\x04 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfig\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x10\n\x08\x63odeType\x18\x07 \x01(\t\x12\x0e\n\x06\x63odeId\x18\x08 \x01(\t\x12\x13\n\x0b\x63odeVersion\x18\t \x01(\t\"1\n\x1c\x41ppWorkerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"W\n\x0e\x41ppWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"q\n\x11\x41ppWorkerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\x12\x0e\n\x06target\x18\x05 \x01(\t\"U\n\x1c\x41ppWorkerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"S\n\x17\x41ppWorkerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"g\n\x1c\x41ppWorkerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"h\n\x12\x41ppWorkerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x83\x01\n\x16\x41ppWorkerBrokerCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x0e\n\x06params\x18\x04 \x01(\t\x12\x11\n\tcommandId\x18\x05 \x01(\t\"\x9f\x01\n\x1c\x41ppWorkerBrokerCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tcommandId\x18\x03 \x01(\t\x12\x10\n\x08response\x18\x04 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12\r\n\x05\x65rror\x18\x06 \x01(\x08\"\x93\x01\n\x16\x41ppWorkerModuleCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\"\xd0\x01\n\x1c\x41ppWorkerModuleCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x07 \x01(\t\x12\r\n\x05\x65rror\x18\x08 \x01(\x08\x12\x10\n\x08response\x18\t \x01(\t\"g\n\x1a\x41ppWorkerFinishedStepInfos\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\"c\n\x19\x41ppWorkerRegistrationInfo\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07success\x18\x03 \x01(\x08\"\xad\x02\n\x1d\x46\x65\x61tureInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x14\n\x0coptionValues\x18\x03 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12\x1c\n\x14targetDatabaseServer\x18\x05 \x01(\t\x12\x18\n\x10targetDatabaseID\x18\x06 \x01(\t\x12\x13\n\x0bsessionData\x18\x07 \x01(\t\x12\x14\n\x0crabbitServer\x18\x08 \x01(\t\x12\x12\n\nrabbitUser\x18\t \x01(\t\x12\x11\n\trabbitPwd\x18\n \x01(\t\x12\x12\n\nrabbitPort\x18\x0b \x01(\t\x12\x19\n\x11rabbitQueuePrefix\x18\x0c \x01(\t\"i\n\x13\x46\x65\x61tureWorkerConfig\x12\x44\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32&.coinlib.FeatureInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"U\n\x0c\x46\x65\x61tureError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"_\n\x0f\x46\x65\x61tureCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\"Q\n\x15\x46\x65\x61tureCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"e\n\x1a\x46\x65\x61tureCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"/\n\x1a\x46\x65\x61tureSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"f\n\x10\x46\x65\x61tureEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\">\n\x17RegistrationInformation\x12\x12\n\nduplicated\x18\x01 \x01(\x08\x12\x0f\n\x07success\x18\x02 \x01(\x08\"I\n\x15SymbolDataRequestInfo\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x02 \x01(\t\"G\n\x12SymbolDataResponse\x12\x31\n\x07symbols\x18\x01 \x03(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\"\x19\n\x17\x45xchangeDataRequestInfo\"L\n\x13\x42rokerExchangeSmall\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04mode\x18\x04 \x01(\t\"G\n\x14\x45xchangeDataResponse\x12/\n\texchanges\x18\x02 \x03(\x0b\x32\x1c.coinlib.BrokerExchangeSmall\"\xae\x02\n\x17SymbolBrokerSymbolSmall\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x11\n\tsymbol_id\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\t\x12\x0c\n\x04\x62\x61se\x18\x05 \x01(\t\x12\r\n\x05quote\x18\x06 \x01(\t\x12\x16\n\x0epricePrecision\x18\x07 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12>\n\x07\x63olumns\x18\n \x03(\x0b\x32-.coinlib.SymbolBrokerSymbolSmall.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb2\x01\n\x11MarketDataRequest\x12\x30\n\x06symbol\x18\x01 \x01(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x05 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x06 \x01(\t\"h\n\x12MarketDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"i\n\x13\x46\x65\x61tureDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"\xa0\x01\n\x12\x46\x65\x61tureDataRequest\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x01 \x03(\t\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x15\n\rtarget_symbol\x18\x04 \x01(\t\x12\x17\n\x0ftarget_exchange\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05stage\x18\x07 \x01(\t\"\x1e\n\x1c\x41\x64\x64itionalDataFeatureRequest\"y\n\x19\x41\x64\x64itionalDataFeatureInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\r\n\x05group\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"Y\n\x1d\x41\x64\x64itionalDataFeatureResponse\x12\x38\n\x0c\x66\x65\x61tureInfos\x18\x01 \x03(\x0b\x32\".coinlib.AdditionalDataFeatureInfo\"\\\n\x13NotificationOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\x8f\x02\n\x18NotificationRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12,\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.coinlib.NotificationOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12\x15\n\risInteractive\x18\x0c \x01(\x08\"W\n\x0e\x46\x65\x61tureOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xc2\x02\n\x13\x46\x65\x61tureRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12(\n\x07options\x18\x04 \x03(\x0b\x32\x17.coinlib.FeatureOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\x15\n\rfeature_infos\x18\r \x01(\t\x12\x1d\n\x15\x65stimatedDataInterval\x18\x0e \x01(\x03\x12\r\n\x05group\x18\x0f \x01(\t\"5\n\x13SimulatorMethodCall\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\"`\n\x17StatisticFunctionInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"n\n\x15StatisticMethodInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x9d\x02\n\x1bStatisticMethodRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\trefreshOn\x18\x03 \x03(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x1c\n\x14targetPositionLayout\x18\x07 \x01(\t\x12.\n\x06inputs\x18\x08 \x03(\x0b\x32\x1e.coinlib.StatisticMethodInputs\x12\x0e\n\x06plugin\x18\t \x01(\t\x12\x15\n\rpluginVersion\x18\n \x01(\t\x12\x11\n\tcode_type\x18\x0b \x01(\t\x12\x0c\n\x04\x63ode\x18\x0c \x01(\t\"\x83\x02\n!StatisticRuleFunctionRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x30\n\x06inputs\x18\x07 \x03(\x0b\x32 .coinlib.StatisticFunctionInputs\x12\x0e\n\x06plugin\x18\x08 \x01(\t\x12\x15\n\rpluginVersion\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\"A\n\x15WorkerRegistryRequest\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12\x15\n\ractiveModules\x18\x02 \x03(\t\"D\n\x16WorkerRegistryResponse\x12\x16\n\x0etargetendpoint\x18\x01 \x01(\t\x12\x12\n\ntargetport\x18\x02 \x01(\t\"-\n\x06\x41piKey\x12\x12\n\napi_key_id\x18\x01 \x01(\t\x12\x0f\n\x07modules\x18\x02 \x01(\t\"0\n\x07\x41uthKey\x12\x10\n\x08\x61uth_key\x18\x01 \x01(\t\x12\x13\n\x0bvalid_until\x18\x02 \x01(\t2\xf6\x01\n\x0c\x43hartsWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.ChartsWorkerConfig\"\x00\x12L\n\x17OnIndicatorErrorOccured\x12\x17.coinlib.IndicatorError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnPartialChartLayout\x12&.coinlib.ChartsWorkerPartialDataLayout\x1a\x16.google.protobuf.Empty\"\x00\x32\x9d\x02\n\x16StatisticsMethodWorker\x12H\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a%.coinlib.StatisticsBulkedWorkerConfig\"\x00\x12[\n\x18OnStatisticPartiallyData\x12%.coinlib.StatisticBulkedPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12\\\n\x1fOnStatisticFunctionErrorOccured\x12\x1f.coinlib.StatisticFunctionError\x1a\x16.google.protobuf.Empty\"\x00\x32\xae\x06\n\x12SymbolBrokerWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.SymbolBrokerWorkerConfig\"\x00\x12l\n\x0fwaitForCommands\x12).coinlib.SymbolBrokerStopConsumerListener\x1a(.coinlib.SymbolBrokerStopConsumerCommand\"\x00(\x01\x30\x01\x12[\n\x1fonBrokerFetchSymbolDataReceived\x12\x1e.coinlib.SymbolBrokerFetchData\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x18onHistoricalDataReceived\x12).coinlib.SymbolBrokerHistoricalMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x1aonBrokerSymbolInfoReceived\x12\x19.coinlib.SymbolBrokerInfo\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x14onMarketDataReceived\x12\x1f.coinlib.SymbolBrokerMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x13onOrderbookReceived\x12\x1e.coinlib.SymbolBrokerOrderbook\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnSymbolBrokerErrorOccured\x12\x1a.coinlib.SymbolBrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12[\n\x1bonBrokerSymbolTickerCrashed\x12\".coinlib.SymbolBrokerConsumerError\x1a\x16.google.protobuf.Empty\"\x00\x32\x89\x02\n\x12NotificationWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.NotificationWorkerConfig\"\x00\x12Y\n\x17OnCallbackDataExtracted\x12$.coinlib.NotificationCallbackExtract\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnNotificationErrorOccured\x12\x1a.coinlib.NotificationError\x1a\x16.google.protobuf.Empty\"\x00\x32\x89\x03\n\x19LogicRunnerOfflineService\x12J\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\'.coinlib.LogicRunnerOfflineWorkerConfig\"\x00\x12\x61\n\x15OnRunnerPartiallyData\x12..coinlib.LogicRunnerOfflineWorkerPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnRunnerErrorOccured\x12&.coinlib.LogicRunnerOfflineWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12\x63\n\x18OnRunnerFinishedComplete\x12-.coinlib.LogicRunnerOfflineWorkerFinishedData\x1a\x16.google.protobuf.Empty\"\x00\x32\xcd\x05\n\nDataWorker\x12?\n\x0f\x41\x63\x63\x65ptWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x10\x44\x65\x63lineWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\tFireEvent\x12\x15.coinlib.EventRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x14GetNodeForCollection\x12\x1e.coinlib.CollectionNodeRequest\x1a\x1f.coinlib.CollectionNodeResponse\"\x00\x12<\n\x0eRegisterWorker\x12\x0f.coinlib.Worker\x1a\x17.coinlib.WorkerSettings\"\x00\x12\x44\n\rGetAllPlugins\x12\x0f.coinlib.Worker\x1a .coinlib.WorkerPluginInformation\"\x00\x12K\n\x0fUpdateWorkerJob\x12\x1e.coinlib.WorkerJobDataResponse\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0fWatchWorkerJobs\x12\x1b.coinlib.WorkerRegistration\x1a\x12.coinlib.WorkerJob\"\x00(\x01\x30\x01\x12\x41\n\x11\x46inishedWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x10\x45rroredWorkerJob\x12\x17.coinlib.WorkerJobError\x1a\x16.google.protobuf.Empty\"\x00\x32\x9f\x01\n\x0cPluginWorker\x12\x38\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x15.coinlib.PluginConfig\"\x00\x12U\n\x14OnInstallationOutput\x12!.coinlib.PluginInstallationOutput\x1a\x16.google.protobuf.Empty\"\x00(\x01\x32\x9f\x05\n\tSimulator\x12X\n\x0fsimulateFeature\x12 .coinlib.FeatureSimulatorRequest\x1a!.coinlib.FeatureSimulatorResponse\"\x00\x12L\n\rsimulateChart\x12\x1d.coinlib.SimulatorChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12^\n\x16simulateStatisticsRule\x12&.coinlib.SimulatorStatisticChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12\x61\n\x18simulateStatisticsMethod\x12\'.coinlib.SimulatorMethodCallChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12g\n\x14simulateSymbolBroker\x12%.coinlib.SymbolBrokerSimulatorRequest\x1a&.coinlib.SymbolBrokerSimulatorResponse\"\x00\x12U\n\x0esimulateBroker\x12\x1f.coinlib.BrokerSimulatorRequest\x1a .coinlib.BrokerSimulatorResponse\"\x00\x12g\n\x14simulateNotification\x12%.coinlib.NotificationSimulatorRequest\x1a&.coinlib.NotificationSimulatorResponse\"\x00\x32m\n\tFunctions\x12`\n\x19registerIndicatorFunction\x12).coinlib.ChartWorkerIndicatorRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xbc\x05\n\x05Logic\x12\x46\n\x11registerDataUsage\x12\x17.coinlib.LogicDataUsage\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x14registerMonitorEvent\x12\x1a.coinlib.LogicMonitorEvent\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x12registerEventUsage\x12\x18.coinlib.LogicEventUsage\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x17registerCollectionUsage\x12\x1d.coinlib.LogicCollectionUsage\x1a\x16.google.protobuf.Empty\"\x00\x12:\n\x08runLogic\x12\x14.coinlib.LogicRunJob\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x0eregisterTrader\x12 .coinlib.LogicTraderRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x10registerScreener\x12\".coinlib.LogicScreenerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x11registerDataLogic\x12\x1e.coinlib.LogicDataRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x13\x61\x64\x64LogicToWorkspace\x12#.coinlib.WorkspaceLogicRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32Q\n\x06\x42roker\x12G\n\x0eregisterBroker\x12\x1b.coinlib.BrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xb2\x04\n\x0c\x42rokerWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.BrokerWorkerConfig\"\x00\x12\x46\n\x14OnBrokerErrorOccured\x12\x14.coinlib.BrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13WatchBrokerCommands\x12\".coinlib.BrokerCommandRegistration\x1a\x17.coinlib.BrokerCommands\"\x00(\x01\x30\x01\x12L\n\x11SendCommandAnswer\x12\x1d.coinlib.BrokerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x16SendCommandAnswerError\x12\".coinlib.BrokerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12U\n\x15RegisterBrokerSession\x12\".coinlib.BrokerSessionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rOnBrokerEvent\x12\x18.coinlib.BrokerEventData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa1\x08\n\tAppWorker\x12;\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x18.coinlib.AppWorkerConfig\"\x00\x12L\n\x17OnAppWorkerErrorOccured\x12\x17.coinlib.AppWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x13WatchBrokerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12\\\n\x10RunModuleCommand\x12\x1f.coinlib.AppWorkerModuleCommand\x1a%.coinlib.AppWorkerModuleCommandAnswer\"\x00\x12\\\n\x10RunBrokerCommand\x12\x1f.coinlib.AppWorkerBrokerCommand\x1a%.coinlib.AppWorkerBrokerCommandAnswer\"\x00\x12\x61\n\x16WatchAppWorkerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12O\n\x11SendCommandAnswer\x12 .coinlib.AppWorkerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x16SendCommandAnswerError\x12%.coinlib.AppWorkerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x18OnAppWorkerLogicFinished\x12#.coinlib.AppWorkerFinishedStepInfos\x1a\x16.google.protobuf.Empty\"\x00\x12g\n\x18RegisterAppWorkerSession\x12%.coinlib.AppWorkerSessionRegistration\x1a\".coinlib.AppWorkerRegistrationInfo\"\x00\x12I\n\x10OnAppWorkerEvent\x12\x1b.coinlib.AppWorkerEventData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x12OnBrokerTestResult\x12\x1f.coinlib.BrokerTestProtocolData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa2\x04\n\rFeatureWorker\x12?\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1c.coinlib.FeatureWorkerConfig\"\x00\x12\x41\n\x0eOnErrorOccured\x12\x15.coinlib.FeatureError\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\rWatchCommands\x12\x18.coinlib.FeatureCommands\x1a\x18.coinlib.FeatureCommands\"\x00(\x01\x30\x01\x12M\n\x11SendCommandAnswer\x12\x1e.coinlib.FeatureCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x16SendCommandAnswerError\x12#.coinlib.FeatureCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Z\n\x0fRegisterSession\x12#.coinlib.FeatureSessionRegistration\x1a .coinlib.RegistrationInformation\"\x00\x12>\n\x07OnEvent\x12\x19.coinlib.FeatureEventData\x1a\x16.google.protobuf.Empty\"\x00\x32]\n\x06Symbol\x12S\n\x14registerSymbolBroker\x12!.coinlib.SymbolBrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xc1\x03\n\x10\x44\x61taLoaderWorker\x12N\n\rgetAllSymbols\x12\x1e.coinlib.SymbolDataRequestInfo\x1a\x1b.coinlib.SymbolDataResponse\"\x00\x12T\n\x0fgetAllExchanges\x12 .coinlib.ExchangeDataRequestInfo\x1a\x1d.coinlib.ExchangeDataResponse\"\x00\x12J\n\rgetMarketData\x12\x1a.coinlib.MarketDataRequest\x1a\x1b.coinlib.MarketDataResponse\"\x00\x12M\n\x0egetFeatureData\x12\x1b.coinlib.FeatureDataRequest\x1a\x1c.coinlib.FeatureDataResponse\"\x00\x12l\n\x19getAdditionalDataFeatures\x12%.coinlib.AdditionalDataFeatureRequest\x1a&.coinlib.AdditionalDataFeatureResponse\"\x00\x32\x63\n\x0cNotification\x12S\n\x14registerNotification\x12!.coinlib.NotificationRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32U\n\x08\x46\x65\x61tures\x12I\n\x0fregisterFeature\x12\x1c.coinlib.FeatureRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xce\x01\n\nStatistics\x12\x65\n\x1dregisterStatisticRuleFunction\x12*.coinlib.StatisticRuleFunctionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x17registerStatisticMethod\x12$.coinlib.StatisticMethodRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xf5\x01\n\x12\x44\x61taWorkerRegistry\x12\x31\n\ngetAuthKey\x12\x0f.coinlib.ApiKey\x1a\x10.coinlib.AuthKey\"\x00\x12J\n\x16getAllDataWorkerServer\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x1bgetDataWorkerServerEndpoint\x12\x1e.coinlib.WorkerRegistryRequest\x1a\x1f.coinlib.WorkerRegistryResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64\x61taWorker.proto\x12\x07\x63oinlib\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x19google/protobuf/any.proto\"P\n\tWorkerJob\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\"k\n\x0eWorkerJobError\x12\x13\n\x0bworkerJobId\x18\x01 \x01(\t\x12\x15\n\rworkerJobType\x18\x02 \x01(\t\x12\x17\n\x0fworkerJobConfig\x18\x03 \x01(\x0c\x12\x14\n\x0c\x65rrorMessage\x18\x04 \x01(\t\"E\n\x16WorkerAvailablePlugins\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"\xb7\x01\n\x06Worker\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x02 \x01(\t\x12\x13\n\x0bworker_mode\x18\x03 \x01(\t\x12\x39\n\x10\x61vailablePlugins\x18\x04 \x03(\x0b\x32\x1f.coinlib.WorkerAvailablePlugins\x12\n\n\x02os\x18\x05 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x06 \x01(\t\x12\x15\n\ractiveModules\x18\x07 \x03(\t\"\x1a\n\x07RowData\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\";\n\x15WorkerJobDataResponse\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x16\n\x14WorkerJobDataPartial\"\xec\x01\n\x1a\x43hartWorkerPartialDataInfo\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x63olor\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\x02\x12\x0f\n\x07opacity\x18\x05 \x01(\x02\x12\x15\n\rchartTypeIcon\x18\x06 \x01(\t\x12\x0f\n\x07tooltip\x18\x07 \x01(\x08\x12\r\n\x05\x63hart\x18\x08 \x01(\t\x12\x13\n\x0b\x63onnectGaps\x18\t \x01(\x08\x12\x11\n\tfill_from\x18\n \x01(\x02\x12\x0c\n\x04\x66ill\x18\x0b \x01(\t\x12\x12\n\nadditional\x18\x0c \x01(\t\"\xad\x01\n\x1d\x43hartsWorkerPartialDataLayout\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x02 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x36\n\tchartInfo\x18\x03 \x01(\x0b\x32#.coinlib.ChartWorkerPartialDataInfo\"\xdd\x01\n\x14\x43hartWorkerIndicator\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0f\n\x07\x66\x65\x61ture\x18\x03 \x01(\t\x12\x12\n\nsubfeature\x18\x04 \x01(\t\x12\r\n\x05short\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\n\n\x02id\x18\x07 \x01(\t\x12\x11\n\telementId\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tid_output\x18\n \x01(\t\x12\x10\n\x08\x66inished\x18\x0b \x01(\x08\x12\x0f\n\x07\x63hartId\x18\x0c \x01(\t\"\xdc\x02\n ChartWorkerIndicatorRegistration\x12\x11\n\tchartType\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x11\n\tid_output\x18\x06 \x01(\t\x12\x0e\n\x06inputs\x18\x07 \x01(\x0c\x12\x0c\n\x04mode\x18\x08 \x01(\t\x12\x19\n\x11short_description\x18\t \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\n \x01(\t\x12\x0f\n\x07process\x18\x0b \x01(\t\x12\x16\n\x0eunstablePeriod\x18\x0c \x01(\x08\x12\x19\n\x11\x64ynamicTimeseries\x18\r \x01(\x08\x12\x0e\n\x06plugin\x18\x0e \x01(\t\x12\x15\n\rpluginVersion\x18\x0f \x01(\t\x12\x11\n\tcode_type\x18\x10 \x01(\t\x12\x0c\n\x04\x63ode\x18\x11 \x01(\t\"n\n!ChartWorkerIndicatorConfigElement\x12\x30\n\tindicator\x18\x01 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\x12\x17\n\x0findicatorConfig\x18\x02 \x01(\x0c\"\xac\x01\n\x12\x43hartsWorkerConfig\x12<\n\x08\x65lements\x18\x01 \x03(\x0b\x32*.coinlib.ChartWorkerIndicatorConfigElement\x12-\n\x08\x63hildren\x18\x02 \x01(\x0b\x32\x1b.coinlib.ChartsWorkerConfig\x12)\n\tchartData\x18\x03 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\"-\n\x0eStatisticInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"A\n\tDataError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x11\n\terrorCode\x18\x02 \x01(\x03\x12\x10\n\x08\x63ritical\x18\x03 \x01(\x08\"\x89\x01\n\x0eIndicatorError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\tindicator\x18\x03 \x01(\x0b\x32\x1d.coinlib.ChartWorkerIndicator\"\xa3\x01\n\x1aStatisticRuleFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa5\x01\n\x1cStatisticMethodFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xb2\x01\n\"StatisticsMethodWorkerWindowConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\x10\n\x08windowId\x18\x03 \x01(\t\x12)\n\tchartData\x18\x04 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x05 \x01(\x0b\x32\x17.coinlib.ParameterTable\"R\n\x13ParameterTableEntry\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08required\x18\x04 \x01(\x08\"B\n\x0eParameterTable\x12\x30\n\nparameters\x18\x01 \x03(\x0b\x32\x1c.coinlib.ParameterTableEntry\"z\n\rChartDataInfo\x12\x10\n\x08\x63hart_id\x18\x01 \x01(\t\x12\x14\n\x0c\x63hart_prefix\x18\x02 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x03 \x01(\t\x12\x13\n\x0b\x61\x63tivity_id\x18\x04 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x05 \x01(\t\"\xf6\x02\n\x1aStatisticsRuleWorkerConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x05rules\x18\x02 \x03(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x19\n\x11statisticFunction\x18\x03 \x01(\t\x12?\n\x06inputs\x18\x04 \x03(\x0b\x32/.coinlib.StatisticsRuleWorkerConfig.InputsEntry\x12\x12\n\ncombinator\x18\x05 \x01(\t\x12\x16\n\x0e\x63ombinator_not\x18\x06 \x01(\x08\x12\x0c\n\x04type\x18\x07 \x01(\t\x12)\n\tchartData\x18\x08 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x1a\x46\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.coinlib.StatisticInput:\x02\x38\x01\"\xa8\x01\n\x1eStatisticsRuleWorkerConfigType\x12\x33\n\x04rule\x18\x01 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfigH\x00\x12\x43\n\x0cmethodWindow\x18\x02 \x01(\x0b\x32+.coinlib.StatisticsMethodWorkerWindowConfigH\x00\x42\x0c\n\ntest_oneof\"\xb4\x01\n\x1cStatisticsBulkedWorkerConfig\x12\x38\n\x07\x63onfigs\x18\x01 \x03(\x0b\x32\'.coinlib.StatisticsRuleWorkerConfigType\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12/\n\x0eparameterTable\x18\x03 \x01(\x0b\x32\x17.coinlib.ParameterTable\"\x9f\x01\n\x16StatisticFunctionError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12>\n\x11statisticFunction\x18\x03 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\"\xa7\x01\n\x1cStatisticMethodPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x12\n\ndocumentId\x18\x03 \x01(\t\x12\r\n\x05width\x18\x04 \x01(\t\x12\x0e\n\x06height\x18\x05 \x01(\t\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x10\n\x08windowId\x18\x07 \x01(\t\"\xa6\x01\n\x1aStatisticRulePartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12:\n\rstatisticRule\x18\x02 \x01(\x0b\x32#.coinlib.StatisticsRuleWorkerConfig\x12\x14\n\x0c\x63ollectionid\x18\x03 \x01(\t\x12\x12\n\nresultName\x18\x05 \x01(\t\"\xa2\x01\n\x1cStatisticBulkedPartiallyData\x12;\n\nmethodData\x18\x01 \x01(\x0b\x32%.coinlib.StatisticMethodPartiallyDataH\x00\x12\x37\n\x08ruleData\x18\x02 \x01(\x0b\x32#.coinlib.StatisticRulePartiallyDataH\x00\x42\x0c\n\ntest_oneof\"m\n\x11SymbolBrokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"U\n\x19SymbolBrokerConsumerError\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x14\n\x0c\x65rrorMessage\x18\x02 \x01(\t\"\x95\x02\n\x16SymbolBrokerMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04open\x18\x02 \x01(\x02\x12\r\n\x05\x63lose\x18\x03 \x01(\x02\x12\x0c\n\x04high\x18\x04 \x01(\x02\x12\x0b\n\x03low\x18\x05 \x01(\x02\x12\x0e\n\x06volume\x18\x06 \x01(\x02\x12\r\n\x05trade\x18\x07 \x01(\x02\x12\x10\n\x08\x64\x61tetime\x18\x08 \x01(\t\x12\x11\n\tsymbol_id\x18\t \x01(\t\x12\x0e\n\x06symbol\x18\n \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x0b \x01(\t\x12\x12\n\nevent_time\x18\x0c \x01(\t\x12\x0f\n\x07isfinal\x18\r \x01(\x08\x12\x11\n\tcloseTime\x18\x0e \x01(\t\"\x96\x01\n\x10SymbolBrokerInfo\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x30\n\texchanges\x18\x02 \x03(\x0b\x32\x1d.coinlib.SymbolBrokerExchange\x12,\n\x07symbols\x18\x03 \x03(\x0b\x32\x1b.coinlib.SymbolBrokerSymbol\";\n\x15SymbolBrokerOrderbook\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"F\n SymbolBrokerHistoricalMarketData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\xba\x01\n\x14SymbolBrokerExchange\x12\x0c\n\x04icon\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0f\n\x07website\x18\x04 \x01(\t\x12\x15\n\rsymbols_count\x18\x05 \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x06 \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\x07 \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x08 \x01(\x02\"\x8c\x04\n\x12SymbolBrokerSymbol\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x38\n\tassetType\x18\x04 \x01(\x0e\x32%.coinlib.SymbolBrokerSymbol.AssetType\x12>\n\x0c\x63ontractType\x18\x05 \x01(\x0e\x32(.coinlib.SymbolBrokerSymbol.ContractType\x12\x0c\n\x04\x62\x61se\x18\x06 \x01(\t\x12\r\n\x05quote\x18\x07 \x01(\t\x12\x1a\n\x12\x65xchange_symbol_id\x18\x08 \x01(\t\x12\x16\n\x0esize_precision\x18\t \x01(\x02\x12\x17\n\x0fprice_precision\x18\n \x01(\x02\x12\r\n\x05price\x18\x0b \x01(\x02\x12\x17\n\x0fvolume_1mth_usd\x18\x0c \x01(\x02\x12\x17\n\x0fvolume_1day_usd\x18\r \x01(\x02\x12\x17\n\x0fvolume_1hrs_usd\x18\x0e \x01(\x02\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"O\n\x1cSymbolBrokerBrokerInfoConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\"\xdd\x03\n#SymbolBrokerConsumeMarketdataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12O\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x39.coinlib.SymbolBrokerConsumeMarketdataConfig.ContractType\x12I\n\tassetType\x18\t \x01(\x0e\x32\x36.coinlib.SymbolBrokerConsumeMarketdataConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xda\x03\n\"SymbolBrokerConsumeOrderbookConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\x07 \x01(\t\x12N\n\x0c\x63ontractType\x18\x08 \x01(\x0e\x32\x38.coinlib.SymbolBrokerConsumeOrderbookConfig.ContractType\x12H\n\tassetType\x18\t \x01(\x0e\x32\x35.coinlib.SymbolBrokerConsumeOrderbookConfig.AssetType\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xb8\x04\n#SymbolBrokerGetHistoricalDataConfig\x12\x0f\n\x07options\x18\x01 \x01(\t\x12\x1e\n\x16symbolBrokerIdentifier\x18\x02 \x01(\t\x12\x12\n\nquoteAsset\x18\x03 \x01(\t\x12\x11\n\tbaseAsset\x18\x04 \x01(\t\x12\x18\n\x10\x63lient_symbol_id\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05start\x18\x07 \x01(\t\x12\x0b\n\x03\x65nd\x18\x08 \x01(\t\x12\x13\n\x0b\x65xchange_id\x18\t \x01(\t\x12)\n\tchartData\x18\n \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12O\n\x0c\x63ontractType\x18\x0b \x01(\x0e\x32\x39.coinlib.SymbolBrokerGetHistoricalDataConfig.ContractType\x12I\n\tassetType\x18\x0c \x01(\x0e\x32\x36.coinlib.SymbolBrokerGetHistoricalDataConfig.AssetType\x12\x12\n\nreturnData\x18\r \x01(\x08\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"\xc5\x02\n\x18SymbolBrokerWorkerConfig\x12;\n\ninfoConfig\x18\x01 \x01(\x0b\x32%.coinlib.SymbolBrokerBrokerInfoConfigH\x00\x12\x45\n\rconsumeConfig\x18\x02 \x01(\x0b\x32,.coinlib.SymbolBrokerConsumeMarketdataConfigH\x00\x12M\n\x16\x63onsumeOrderbookConfig\x18\x03 \x01(\x0b\x32+.coinlib.SymbolBrokerConsumeOrderbookConfigH\x00\x12H\n\x10historicalConfig\x18\x04 \x01(\x0b\x32,.coinlib.SymbolBrokerGetHistoricalDataConfigH\x00\x42\x0c\n\ntest_oneof\"F\n SymbolBrokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\"2\n\x1fSymbolBrokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"j\n\x15SymbolBrokerFetchData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12-\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x1f.coinlib.SymbolBrokerMarketData\"u\n$NotificationExtractMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\t\x12\x0f\n\x07options\x18\x04 \x01(\t\"\xd3\x01\n!NotificationSendMessageDataConfig\x12\x0e\n\x06inputs\x18\x01 \x01(\t\x12\x1e\n\x16notificationIdentifier\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0e\n\x06images\x18\x04 \x01(\t\x12\x0f\n\x07\x62uttons\x18\x05 \x01(\t\x12\x0f\n\x07options\x18\x06 \x01(\t\x12\x13\n\x0b\x63\x61llback_id\x18\x07 \x01(\t\x12\x14\n\x0c\x63\x61llback_url\x18\x08 \x01(\t\x12\x10\n\x08\x63hannels\x18\t \x01(\t\"\xbd\x01\n\x18NotificationWorkerConfig\x12G\n\x11sendMessageConfig\x18\x01 \x01(\x0b\x32*.coinlib.NotificationSendMessageDataConfigH\x00\x12J\n\x11\x65xtractDataConfig\x18\x02 \x01(\x0b\x32-.coinlib.NotificationExtractMessageDataConfigH\x00\x42\x0c\n\ntest_oneof\"Z\n\x11NotificationError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"b\n\x1bNotificationCallbackExtract\x12\x11\n\tbutton_id\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x98\x01\n\x0eLogicComponent\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x18\n\x10logicComponentId\x18\x03 \x01(\t\x12\x13\n\x0b\x65nvironment\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\x0c\x12\x0c\n\x04type\x18\x06 \x01(\t\x12\x14\n\x0clogicDetails\x18\x07 \x01(\t\"\xde\x03\n\x12\x42rokerAccountModel\x12:\n\nbrokerType\x18\x01 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerType\x12\x34\n\x04mode\x18\x02 \x01(\x0e\x32&.coinlib.BrokerAccountModel.BrokerMode\x12\x10\n\x08\x65xchange\x18\x03 \x01(\t\x12\x10\n\x08makerFee\x18\x04 \x01(\x02\x12\x10\n\x08takerFee\x18\x05 \x01(\x02\x12\x39\n\x0cmakerFeeMode\x18\x06 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\x12\x39\n\x0ctakerFeeMode\x18\x07 \x01(\x0e\x32#.coinlib.BrokerAccountModel.FeeMode\"Q\n\nBrokerType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"1\n\nBrokerMode\x12\x0e\n\nBACKTRADER\x10\x00\x12\t\n\x05PAPER\x10\x01\x12\x08\n\x04LIVE\x10\x02\"$\n\x07\x46\x65\x65Mode\x12\x0e\n\nPERCENTAGE\x10\x00\x12\t\n\x05\x46IXED\x10\x01\"~\n\x0ePortfolioAsset\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x03 \x01(\x02\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\x0e\n\x06locked\x18\x05 \x01(\x02\x12\x11\n\tlastPrice\x18\x06 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x07 \x01(\t\"o\n\x13\x43\x61lculatedBaseMoney\x12\r\n\x05total\x18\x01 \x01(\x02\x12\x0c\n\x04\x66ree\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x0f\n\x07summary\x18\x04 \x01(\x02\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\"\xc0\x01\n\x0ePortfolioModel\x12\'\n\x06\x61ssets\x18\x01 \x03(\x0b\x32\x17.coinlib.PortfolioAsset\x12@\n\x1a\x63urrentCalculatedBaseMoney\x18\x02 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\x43\n\x1dhistoricalCalculatedBaseMoney\x18\x03 \x03(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\"\x82\x03\n\x10LogicRunnerLogic\x12)\n\tchartData\x18\x01 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12\x30\n\x0flogicComponents\x18\x02 \x03(\x0b\x32\x17.coinlib.LogicComponent\x12\x11\n\tstartDate\x18\x03 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x04 \x01(\t\x12*\n\tportfolio\x18\x05 \x01(\x0b\x32\x17.coinlib.PortfolioModel\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\x12/\n\x0eparameterTable\x18\x07 \x01(\x0b\x32\x17.coinlib.ParameterTable\x12\x11\n\tlogicMode\x18\x08 \x01(\t\x12\x15\n\rapp_worker_id\x18\t \x01(\t\x12\x1c\n\x14\x61pp_worker_runner_id\x18\n \x01(\t\x12\x14\n\x0coptions_json\x18\x0b \x01(\t\"\xd5\x01\n\x1eLogicRunnerOfflineWorkerConfig\x12,\n\tlogicInfo\x18\x01 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12)\n\tchartData\x18\x02 \x01(\x0b\x32\x16.coinlib.ChartDataInfo\x12+\n\tportfolio\x18\x03 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x18\n\x10\x61\x64vancedDataInfo\x18\x04 \x01(\t\x12\x13\n\x0bonlySignals\x18\x05 \x01(\x08\"\xcf\x04\n\x15LogicRunnerStatistics\x12\x1f\n\x17highestProfitPercentage\x18\x01 \x01(\x02\x12\x1d\n\x15highestLossPercentage\x18\x02 \x01(\x02\x12\x11\n\tsinceDate\x18\x03 \x01(\t\x12\x0e\n\x06\x61tDate\x18\x04 \x01(\t\x12\x11\n\ttradesCnt\x18\x05 \x01(\x02\x12\x35\n\x0f\x63\x61lculatedMoney\x18\x06 \x01(\x0b\x32\x1c.coinlib.CalculatedBaseMoney\x12\"\n\x1aunrealizedProfitPercentage\x18\x07 \x01(\x02\x12\x0c\n\x04\x66\x65\x65s\x18\x08 \x01(\x02\x12 \n\x18profitCompletePercentage\x18\t \x01(\x02\x12\x1d\n\x15highestProfitPerGroup\x18\n \x01(\x02\x12\x1b\n\x13highestLossPerGroup\x18\x0b \x01(\x02\x12\x18\n\x10slippagePerGroup\x18\x0c \x01(\x02\x12\x1a\n\x12\x61verageAmountQuote\x18\r \x01(\x02\x12\'\n\x1f\x61verageProfitPercentagePergroup\x18\x0e \x01(\x02\x12\x19\n\x11portfolioTimeline\x18\x0f \x01(\t\x12\x14\n\x0cwinLossRatio\x18\x10 \x01(\x02\x12\x0e\n\x06winCnt\x18\x11 \x01(\x02\x12\x0f\n\x07lossCnt\x18\x12 \x01(\x02\x12\x17\n\x0fsecondsInMarket\x18\x13 \x01(\x02\x12\x1d\n\x15\x61verageSecondsInTrade\x18\x14 \x01(\x02\x12\x10\n\x08\x64rawDown\x18\x15 \x01(\x02\"\xa6\x01\n%LogicRunnerOfflineWorkerPartiallyData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\npercentage\x18\x02 \x01(\x02\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x05 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"w\n\x1dLogicRunnerOfflineWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xb4\x01\n$LogicRunnerOfflineWorkerFinishedData\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\x12\x31\n\tstatistic\x18\x04 \x01(\x0b\x32\x1e.coinlib.LogicRunnerStatistics\"K\n\rWorkspaceInfo\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\x12\x11\n\tdataSetId\x18\x02 \x01(\t\x12\x12\n\nactivityId\x18\x03 \x01(\t\"@\n\x17WorkerPluginInformation\x12%\n\x06plugin\x18\x01 \x03(\x0b\x32\x15.coinlib.PluginConfig\"<\n\x0eWorkerSettings\x12\x15\n\ractiveModules\x18\x01 \x03(\t\x12\x13\n\x0bworker_mode\x18\x02 \x01(\t\"\'\n\x12WorkerRegistration\x12\x11\n\tworker_id\x18\x01 \x01(\t\"b\n\x15\x43ollectionNodeRequest\x12\x16\n\x0e\x63ollectionName\x18\x01 \x01(\t\x12\r\n\x05stage\x18\x02 \x01(\t\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x12.coinlib.WorkerJob\":\n\x16\x43ollectionNodeResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nsize_in_mb\x18\x02 \x01(\t\"`\n\x0c\x45ventRequest\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\x12\r\n\x05stage\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"t\n\x0cPluginConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x13\n\x0b\x66ilecontent\x18\x04 \x01(\t\x12\x10\n\x08testOnly\x18\x05 \x01(\x08\x12\x10\n\x08\x66iletype\x18\x06 \x01(\t\"U\n\x18PluginInstallationOutput\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x15\n\routputMessage\x18\x02 \x01(\t\"\xcb\x01\n\x1dSimulatorChartConfigIndicator\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nsubfeature\x18\x02 \x01(\t\x12\x42\n\x06inputs\x18\x03 \x03(\x0b\x32\x32.coinlib.SimulatorChartConfigIndicator.InputsEntry\x12\x12\n\nchartIndex\x18\x04 \x01(\t\x1a-\n\x0bInputsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x14SimulatorChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x0e\n\x06\x62roker\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\x97\x01\n\x1dSimulatorStatisticChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\"\xc7\x01\n\x1eSimulatorMethodCallChartConfig\x12\x11\n\tkernel_id\x18\x01 \x01(\t\x12\x15\n\rsimulatorName\x18\x02 \x01(\t\x12:\n\nindicators\x18\x05 \x03(\x0b\x32&.coinlib.SimulatorChartConfigIndicator\x12\x10\n\x08workerId\x18\x06 \x01(\t\x12-\n\x07methods\x18\x07 \x03(\x0b\x32\x1c.coinlib.SimulatorMethodCall\"@\n\x11SimulatorResponse\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"\x83\x01\n\x1cSymbolBrokerSimulatorRequest\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x13\n\x0btestSymbol1\x18\x04 \x01(\t\x12\x13\n\x0btestSymbol2\x18\x05 \x01(\t\"g\n\x1dSymbolBrokerSimulatorResponse\x12\x16\n\x0esymbolBrokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"@\n\x1e\x42rokerSimulatorBrokerLoginData\x12\x0e\n\x06\x61pikey\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"\x95\x01\n\x19\x42rokerSimulatorBrokerData\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12:\n\tloginInfo\x18\x02 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x11\n\tassetType\x18\x03 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x04 \x01(\t\"\x98\x01\n\x16\x42rokerSimulatorRequest\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x36\n\nbrokerInfo\x18\x04 \x01(\x0b\x32\".coinlib.BrokerSimulatorBrokerData\x12\x11\n\tpaperMode\x18\x05 \x01(\x08\"\xb2\x01\n\x17\x42rokerSimulatorResponse\x12\x10\n\x08\x62rokerId\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\x12\x11\n\tsessionId\x18\x04 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x05 \x01(\t\x12\x15\n\rtargetdepotId\x18\x06 \x01(\t\x12\x16\n\x0erootServerPath\x18\x07 \x01(\t\"f\n\x1cNotificationSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0e\n\x06inputs\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\x12\x10\n\x08\x63hannels\x18\x04 \x01(\t\"c\n\x1dNotificationSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"P\n\x17\x46\x65\x61tureSimulatorRequest\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07options\x18\x02 \x01(\t\x12\x10\n\x08workerId\x18\x03 \x01(\t\"^\n\x18\x46\x65\x61tureSimulatorResponse\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x1d\n\x15simulatorResponseText\x18\x03 \x01(\t\"c\n\nLogicInput\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x85\x02\n\x17LogicTraderRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x84\x02\n\x16LogicAlertRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x83\x02\n\x15LogicDataRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x87\x02\n\x19LogicScreenerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12#\n\x06inputs\x18\x04 \x03(\x0b\x32\x13.coinlib.LogicInput\x12\x0f\n\x07modules\x18\x05 \x03(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x13\n\x0bworkspaceId\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\x12\x10\n\x08workerId\x18\x0c \x01(\t\"\x91\x02\n\x1aWorkspaceLogicRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x18\n\x10logicComponentId\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\x0c\x12\r\n\x05stage\x18\x04 \x01(\t\x12\x0e\n\x06plugin\x18\x05 \x01(\t\x12\x15\n\rpluginVersion\x18\x06 \x01(\t\x12\x13\n\x0bworkspaceId\x18\x07 \x01(\t\x12\x0c\n\x04type\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x10\n\x08workerId\x18\x0b \x01(\t\x12\x11\n\tautostart\x18\x0c \x01(\x08\x12\x16\n\x0e\x61utostartLogic\x18\r \x01(\x08\"\"\n\x0bLogicRunJob\x12\x13\n\x0bworkspaceId\x18\x01 \x01(\t\"\xb3\x02\n\x0eLogicDataUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05group\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04type\x18\x05 \x01(\t\x12\x0e\n\x06symbol\x18\x06 \x01(\x08\x12\x10\n\x08\x65xchange\x18\x07 \x01(\x08\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf3\x01\n\x11LogicMonitorEvent\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06params\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xf6\x01\n\x14LogicCollectionUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\xe2\x01\n\x0fLogicEventUsage\x12\r\n\x05stage\x18\x01 \x01(\t\x12\r\n\x05\x65vent\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0c\n\x04\x63ode\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0e\n\x06plugin\x18\x0b \x01(\t\x12\x15\n\rpluginVersion\x18\x0c \x01(\t\x12\x10\n\x08workerId\x18\r \x01(\t\x12\x18\n\x10logic_identifier\x18\x0e \x01(\t\x12\x15\n\rlogic_version\x18\x0f \x01(\t\x12\x11\n\tlogicType\x18\x10 \x01(\t\"\\\n\x13SymbolBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xe4\x01\n\x18SymbolBrokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12-\n\x07options\x18\x04 \x03(\x0b\x32\x1c.coinlib.SymbolBrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\"V\n\rBrokerOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xda\x03\n\x0e\x42rokerExchange\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04icon\x18\x03 \x01(\t\x12\x34\n\tloginMode\x18\x04 \x01(\x0e\x32!.coinlib.BrokerExchange.LoginMode\x12;\n\rcontractTypes\x18\x05 \x03(\x0e\x32$.coinlib.BrokerExchange.ContractType\x12\x35\n\nassetTypes\x18\x06 \x03(\x0e\x32!.coinlib.BrokerExchange.AssetType\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x13\n\x0bsupportDemo\x18\x08 \x01(\x08\x12\x13\n\x0bsupportLive\x18\t \x01(\x08\x12\x1a\n\x12positionModeFuture\x18\n \x01(\t\"\x18\n\tLoginMode\x12\x0b\n\x07\x41PI_KEY\x10\x00\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\xa8\x03\n\x12\x42rokerRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12\'\n\x07options\x18\x04 \x03(\x0b\x32\x16.coinlib.BrokerOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12*\n\texchanges\x18\x0b \x03(\x0b\x32\x17.coinlib.BrokerExchange\x12\x45\n\x0b\x62rokerTypes\x18\x0c \x03(\x0e\x32\x30.coinlib.BrokerRegistration.SupportedBrokerTypes\"[\n\x14SupportedBrokerTypes\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"?\n\x0f\x42rokerPortfolio\x12,\n\x05\x61sset\x18\x01 \x03(\x0b\x32\x1d.coinlib.BrokerPortfolioAsset\"Z\n\x14\x42rokerPortfolioAsset\x12\x0c\n\x04\x62\x61se\x18\x01 \x01(\t\x12\x11\n\tavailable\x18\x02 \x01(\x02\x12\x0e\n\x06locked\x18\x03 \x01(\x02\x12\x11\n\tlastPrice\x18\x04 \x01(\x02\"\x84\x03\n\x18\x42rokerSessionAccountInfo\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x44\n\x0c\x63ontractType\x18\x02 \x01(\x0e\x32..coinlib.BrokerSessionAccountInfo.ContractType\x12>\n\tassetType\x18\x03 \x01(\x0e\x32+.coinlib.BrokerSessionAccountInfo.AssetType\x12:\n\tloginInfo\x18\x04 \x01(\x0b\x32\'.coinlib.BrokerSimulatorBrokerLoginData\x12\x0f\n\x07sandbox\x18\x05 \x01(\x08\"S\n\x0c\x43ontractType\x12\x08\n\x04SPOT\x10\x00\x12\n\n\x06\x46UTURE\x10\x01\x12\n\n\x06MARGIN\x10\x02\x12\n\n\x06OPTION\x10\x03\x12\t\n\x05INDEX\x10\x04\x12\n\n\x06\x43REDIT\x10\x05\"+\n\tAssetType\x12\x08\n\x04\x43OIN\x10\x00\x12\t\n\x05\x46OREX\x10\x01\x12\t\n\x05STOCK\x10\x02\"\x9b\x01\n\x1c\x42rokerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\"\xf4\x01\n\x14\x42rokerInfoTestConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x18\n\x10\x62rokerIdentifier\x18\x02 \x01(\t\x12\x36\n\x0b\x61\x63\x63ountInfo\x18\x03 \x01(\x0b\x32!.coinlib.BrokerSessionAccountInfo\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x32\n\rbrokerAccount\x18\x06 \x01(\x0b\x32\x1b.coinlib.BrokerAccountModel\"g\n\x12\x42rokerWorkerConfig\x12\x43\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"@\n\x1a\x42rokerStopConsumerListener\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\",\n\x19\x42rokerStopConsumerCommand\x12\x0f\n\x07stopped\x18\x01 \x01(\x08\"\x18\n\x16\x42rokerStartSessionInfo\"g\n\x0b\x42rokerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tsessionId\x18\x03 \x01(\t\"j\n\x0e\x42rokerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x15\n\rbrokerCommand\x18\x03 \x01(\t\x12\x1b\n\x13\x62rokerCommandParams\x18\x04 \x01(\t\".\n\x19\x42rokerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"P\n\x14\x42rokerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"d\n\x19\x42rokerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"e\n\x0f\x42rokerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\".\n\x19\x42rokerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"J\n\x16\x42rokerTestProtocolData\x12\"\n\x06worker\x18\x01 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\"\x9c\x01\n\x0f\x41ppWorkerConfig\x12\x46\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32(.coinlib.AppWorkerInfoStartSessionConfigH\x00\x12\x33\n\ntestConfig\x18\x02 \x01(\x0b\x32\x1d.coinlib.BrokerInfoTestConfigH\x00\x42\x0c\n\ntest_oneof\"\xa9\x02\n\x1f\x41ppWorkerInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x02 \x01(\t\x12,\n\tlogicInfo\x18\x03 \x01(\x0b\x32\x19.coinlib.LogicRunnerLogic\x12;\n\x0c\x62rokerConfig\x18\x04 \x01(\x0b\x32%.coinlib.BrokerInfoStartSessionConfig\x12+\n\tportfolio\x18\x05 \x01(\x0b\x32\x18.coinlib.BrokerPortfolio\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x10\n\x08\x63odeType\x18\x07 \x01(\t\x12\x0e\n\x06\x63odeId\x18\x08 \x01(\t\x12\x13\n\x0b\x63odeVersion\x18\t \x01(\t\"1\n\x1c\x41ppWorkerCommandRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"W\n\x0e\x41ppWorkerError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"q\n\x11\x41ppWorkerCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\x12\x0e\n\x06target\x18\x05 \x01(\t\"U\n\x1c\x41ppWorkerSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"S\n\x17\x41ppWorkerCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"g\n\x1c\x41ppWorkerCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"h\n\x12\x41ppWorkerEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\"\x83\x01\n\x16\x41ppWorkerBrokerCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x0e\n\x06params\x18\x04 \x01(\t\x12\x11\n\tcommandId\x18\x05 \x01(\t\"\x9f\x01\n\x1c\x41ppWorkerBrokerCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x11\n\tcommandId\x18\x03 \x01(\t\x12\x10\n\x08response\x18\x04 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x05 \x01(\t\x12\r\n\x05\x65rror\x18\x06 \x01(\x08\"\x93\x01\n\x16\x41ppWorkerModuleCommand\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\"\xd0\x01\n\x1c\x41ppWorkerModuleCommandAnswer\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0e\n\x06module\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x0e\n\x06params\x18\x05 \x01(\t\x12\x11\n\tcommandId\x18\x06 \x01(\t\x12\x14\n\x0c\x65rrorMessage\x18\x07 \x01(\t\x12\r\n\x05\x65rror\x18\x08 \x01(\x08\x12\x10\n\x08response\x18\t \x01(\t\"g\n\x1a\x41ppWorkerFinishedStepInfos\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x12\n\nsignalData\x18\x03 \x01(\t\"c\n\x19\x41ppWorkerRegistrationInfo\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\x12\x0f\n\x07success\x18\x03 \x01(\x08\"\xad\x02\n\x1d\x46\x65\x61tureInfoStartSessionConfig\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x14\n\x0coptionValues\x18\x03 \x01(\t\x12\x16\n\x0eshortSessionId\x18\x04 \x01(\t\x12\x1c\n\x14targetDatabaseServer\x18\x05 \x01(\t\x12\x18\n\x10targetDatabaseID\x18\x06 \x01(\t\x12\x13\n\x0bsessionData\x18\x07 \x01(\t\x12\x14\n\x0crabbitServer\x18\x08 \x01(\t\x12\x12\n\nrabbitUser\x18\t \x01(\t\x12\x11\n\trabbitPwd\x18\n \x01(\t\x12\x12\n\nrabbitPort\x18\x0b \x01(\t\x12\x19\n\x11rabbitQueuePrefix\x18\x0c \x01(\t\"i\n\x13\x46\x65\x61tureWorkerConfig\x12\x44\n\x12startSessionConfig\x18\x01 \x01(\x0b\x32&.coinlib.FeatureInfoStartSessionConfigH\x00\x42\x0c\n\ntest_oneof\"U\n\x0c\x46\x65\x61tureError\x12!\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x12.coinlib.DataError\x12\"\n\x06worker\x18\x02 \x01(\x0b\x32\x12.coinlib.WorkerJob\"_\n\x0f\x46\x65\x61tureCommands\x12\x11\n\tsessionId\x18\x01 \x01(\t\x12\x11\n\tcommandId\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x15\n\rcommandParams\x18\x04 \x01(\t\"Q\n\x15\x46\x65\x61tureCommandsAnswer\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\"e\n\x1a\x46\x65\x61tureCommandsAnswerError\x12\x11\n\tcommandId\x18\x01 \x01(\t\x12\x12\n\nanswerData\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"/\n\x1a\x46\x65\x61tureSessionRegistration\x12\x11\n\tsessionId\x18\x01 \x01(\t\"f\n\x10\x46\x65\x61tureEventData\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\t\x12\x11\n\tsessionId\x18\x03 \x01(\t\x12\"\n\x06worker\x18\x04 \x01(\x0b\x32\x12.coinlib.WorkerJob\">\n\x17RegistrationInformation\x12\x12\n\nduplicated\x18\x01 \x01(\x08\x12\x0f\n\x07success\x18\x02 \x01(\x08\"I\n\x15SymbolDataRequestInfo\x12\x10\n\x08\x65xchange\x18\x01 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x02 \x01(\t\"G\n\x12SymbolDataResponse\x12\x31\n\x07symbols\x18\x01 \x03(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\"\x19\n\x17\x45xchangeDataRequestInfo\"L\n\x13\x42rokerExchangeSmall\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04mode\x18\x04 \x01(\t\"G\n\x14\x45xchangeDataResponse\x12/\n\texchanges\x18\x02 \x03(\x0b\x32\x1c.coinlib.BrokerExchangeSmall\"\xae\x02\n\x17SymbolBrokerSymbolSmall\x12\x13\n\x0b\x65xchange_id\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x11\n\tsymbol_id\x18\x03 \x01(\t\x12\x12\n\naccount_id\x18\x04 \x01(\t\x12\x0c\n\x04\x62\x61se\x18\x05 \x01(\t\x12\r\n\x05quote\x18\x06 \x01(\t\x12\x16\n\x0epricePrecision\x18\x07 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12>\n\x07\x63olumns\x18\n \x03(\x0b\x32-.coinlib.SymbolBrokerSymbolSmall.ColumnsEntry\x1a.\n\x0c\x43olumnsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb2\x01\n\x11MarketDataRequest\x12\x30\n\x06symbol\x18\x01 \x01(\x0b\x32 .coinlib.SymbolBrokerSymbolSmall\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x11\n\ttimeframe\x18\x04 \x01(\t\x12\x14\n\x0c\x63ontractType\x18\x05 \x01(\t\x12\x1e\n\x16\x61\x64\x64itionalDataFeatures\x18\x06 \x01(\t\"h\n\x12MarketDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"i\n\x13\x46\x65\x61tureDataResponse\x12\x13\n\x0b\x64\x61ta_server\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x61tabase_id\x18\x02 \x01(\t\x12\x10\n\x08\x63hart_id\x18\x03 \x01(\t\x12\x16\n\x0e\x63hipmunkdbHost\x18\x04 \x01(\t\"\xa0\x01\n\x12\x46\x65\x61tureDataRequest\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x01 \x03(\t\x12\x11\n\tstartDate\x18\x02 \x01(\t\x12\x0f\n\x07\x65ndDate\x18\x03 \x01(\t\x12\x15\n\rtarget_symbol\x18\x04 \x01(\t\x12\x17\n\x0ftarget_exchange\x18\x05 \x01(\t\x12\x11\n\ttimeframe\x18\x06 \x01(\t\x12\r\n\x05stage\x18\x07 \x01(\t\"\x1e\n\x1c\x41\x64\x64itionalDataFeatureRequest\"y\n\x19\x41\x64\x64itionalDataFeatureInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08\x65xchange\x18\x04 \x01(\t\x12\r\n\x05group\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\"Y\n\x1d\x41\x64\x64itionalDataFeatureResponse\x12\x38\n\x0c\x66\x65\x61tureInfos\x18\x01 \x03(\x0b\x32\".coinlib.AdditionalDataFeatureInfo\"\\\n\x13NotificationOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\x8f\x02\n\x18NotificationRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12,\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.coinlib.NotificationOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0b \x01(\t\x12\x15\n\risInteractive\x18\x0c \x01(\x08\"W\n\x0e\x46\x65\x61tureOptions\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"\xc2\x02\n\x13\x46\x65\x61tureRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07iconUrl\x18\x03 \x01(\t\x12(\n\x07options\x18\x04 \x03(\x0b\x32\x17.coinlib.FeatureOptions\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x0e\n\x06plugin\x18\x07 \x01(\t\x12\x15\n\rpluginVersion\x18\x08 \x01(\t\x12\x11\n\tcode_type\x18\t \x01(\t\x12\x0c\n\x04\x63ode\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x0c \x01(\t\x12\x15\n\rfeature_infos\x18\r \x01(\t\x12\x1d\n\x15\x65stimatedDataInterval\x18\x0e \x01(\x03\x12\r\n\x05group\x18\x0f \x01(\t\"5\n\x13SimulatorMethodCall\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x0e\n\x06params\x18\x02 \x01(\t\"`\n\x17StatisticFunctionInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\"n\n\x15StatisticMethodInputs\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05label\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x04 \x01(\t\x12\x0e\n\x06values\x18\x05 \x01(\t\"\x9d\x02\n\x1bStatisticMethodRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\trefreshOn\x18\x03 \x03(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x1c\n\x14targetPositionLayout\x18\x07 \x01(\t\x12.\n\x06inputs\x18\x08 \x03(\x0b\x32\x1e.coinlib.StatisticMethodInputs\x12\x0e\n\x06plugin\x18\t \x01(\t\x12\x15\n\rpluginVersion\x18\n \x01(\t\x12\x11\n\tcode_type\x18\x0b \x01(\t\x12\x0c\n\x04\x63ode\x18\x0c \x01(\t\"\x83\x02\n!StatisticRuleFunctionRegistration\x12\x12\n\nidentifier\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05group\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05stage\x18\x06 \x01(\t\x12\x30\n\x06inputs\x18\x07 \x03(\x0b\x32 .coinlib.StatisticFunctionInputs\x12\x0e\n\x06plugin\x18\x08 \x01(\t\x12\x15\n\rpluginVersion\x18\t \x01(\t\x12\x11\n\tcode_type\x18\n \x01(\t\x12\x0c\n\x04\x63ode\x18\x0b \x01(\t\"A\n\x15WorkerRegistryRequest\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12\x15\n\ractiveModules\x18\x02 \x03(\t\"D\n\x16WorkerRegistryResponse\x12\x16\n\x0etargetendpoint\x18\x01 \x01(\t\x12\x12\n\ntargetport\x18\x02 \x01(\t\"-\n\x06\x41piKey\x12\x12\n\napi_key_id\x18\x01 \x01(\t\x12\x0f\n\x07modules\x18\x02 \x01(\t\"0\n\x07\x41uthKey\x12\x10\n\x08\x61uth_key\x18\x01 \x01(\t\x12\x13\n\x0bvalid_until\x18\x02 \x01(\t2\xf6\x01\n\x0c\x43hartsWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.ChartsWorkerConfig\"\x00\x12L\n\x17OnIndicatorErrorOccured\x12\x17.coinlib.IndicatorError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnPartialChartLayout\x12&.coinlib.ChartsWorkerPartialDataLayout\x1a\x16.google.protobuf.Empty\"\x00\x32\x9d\x02\n\x16StatisticsMethodWorker\x12H\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a%.coinlib.StatisticsBulkedWorkerConfig\"\x00\x12[\n\x18OnStatisticPartiallyData\x12%.coinlib.StatisticBulkedPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12\\\n\x1fOnStatisticFunctionErrorOccured\x12\x1f.coinlib.StatisticFunctionError\x1a\x16.google.protobuf.Empty\"\x00\x32\xae\x06\n\x12SymbolBrokerWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.SymbolBrokerWorkerConfig\"\x00\x12l\n\x0fwaitForCommands\x12).coinlib.SymbolBrokerStopConsumerListener\x1a(.coinlib.SymbolBrokerStopConsumerCommand\"\x00(\x01\x30\x01\x12[\n\x1fonBrokerFetchSymbolDataReceived\x12\x1e.coinlib.SymbolBrokerFetchData\x1a\x16.google.protobuf.Empty\"\x00\x12_\n\x18onHistoricalDataReceived\x12).coinlib.SymbolBrokerHistoricalMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x1aonBrokerSymbolInfoReceived\x12\x19.coinlib.SymbolBrokerInfo\x1a\x16.google.protobuf.Empty\"\x00\x12Q\n\x14onMarketDataReceived\x12\x1f.coinlib.SymbolBrokerMarketData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x13onOrderbookReceived\x12\x1e.coinlib.SymbolBrokerOrderbook\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnSymbolBrokerErrorOccured\x12\x1a.coinlib.SymbolBrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12[\n\x1bonBrokerSymbolTickerCrashed\x12\".coinlib.SymbolBrokerConsumerError\x1a\x16.google.protobuf.Empty\"\x00\x32\x89\x02\n\x12NotificationWorker\x12\x44\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a!.coinlib.NotificationWorkerConfig\"\x00\x12Y\n\x17OnCallbackDataExtracted\x12$.coinlib.NotificationCallbackExtract\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x1aOnNotificationErrorOccured\x12\x1a.coinlib.NotificationError\x1a\x16.google.protobuf.Empty\"\x00\x32\xea\x03\n\x19LogicRunnerOfflineService\x12J\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\'.coinlib.LogicRunnerOfflineWorkerConfig\"\x00\x12_\n\x1aGetLogicConfigForWorkspace\x12\x16.coinlib.WorkspaceInfo\x1a\'.coinlib.LogicRunnerOfflineWorkerConfig\"\x00\x12\x61\n\x15OnRunnerPartiallyData\x12..coinlib.LogicRunnerOfflineWorkerPartiallyData\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x14OnRunnerErrorOccured\x12&.coinlib.LogicRunnerOfflineWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12\x63\n\x18OnRunnerFinishedComplete\x12-.coinlib.LogicRunnerOfflineWorkerFinishedData\x1a\x16.google.protobuf.Empty\"\x00\x32\xcd\x05\n\nDataWorker\x12?\n\x0f\x41\x63\x63\x65ptWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x10\x44\x65\x63lineWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12<\n\tFireEvent\x12\x15.coinlib.EventRequest\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x14GetNodeForCollection\x12\x1e.coinlib.CollectionNodeRequest\x1a\x1f.coinlib.CollectionNodeResponse\"\x00\x12<\n\x0eRegisterWorker\x12\x0f.coinlib.Worker\x1a\x17.coinlib.WorkerSettings\"\x00\x12\x44\n\rGetAllPlugins\x12\x0f.coinlib.Worker\x1a .coinlib.WorkerPluginInformation\"\x00\x12K\n\x0fUpdateWorkerJob\x12\x1e.coinlib.WorkerJobDataResponse\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0fWatchWorkerJobs\x12\x1b.coinlib.WorkerRegistration\x1a\x12.coinlib.WorkerJob\"\x00(\x01\x30\x01\x12\x41\n\x11\x46inishedWorkerJob\x12\x12.coinlib.WorkerJob\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x10\x45rroredWorkerJob\x12\x17.coinlib.WorkerJobError\x1a\x16.google.protobuf.Empty\"\x00\x32\x9f\x01\n\x0cPluginWorker\x12\x38\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x15.coinlib.PluginConfig\"\x00\x12U\n\x14OnInstallationOutput\x12!.coinlib.PluginInstallationOutput\x1a\x16.google.protobuf.Empty\"\x00(\x01\x32\x9f\x05\n\tSimulator\x12X\n\x0fsimulateFeature\x12 .coinlib.FeatureSimulatorRequest\x1a!.coinlib.FeatureSimulatorResponse\"\x00\x12L\n\rsimulateChart\x12\x1d.coinlib.SimulatorChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12^\n\x16simulateStatisticsRule\x12&.coinlib.SimulatorStatisticChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12\x61\n\x18simulateStatisticsMethod\x12\'.coinlib.SimulatorMethodCallChartConfig\x1a\x1a.coinlib.SimulatorResponse\"\x00\x12g\n\x14simulateSymbolBroker\x12%.coinlib.SymbolBrokerSimulatorRequest\x1a&.coinlib.SymbolBrokerSimulatorResponse\"\x00\x12U\n\x0esimulateBroker\x12\x1f.coinlib.BrokerSimulatorRequest\x1a .coinlib.BrokerSimulatorResponse\"\x00\x12g\n\x14simulateNotification\x12%.coinlib.NotificationSimulatorRequest\x1a&.coinlib.NotificationSimulatorResponse\"\x00\x32m\n\tFunctions\x12`\n\x19registerIndicatorFunction\x12).coinlib.ChartWorkerIndicatorRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xbc\x05\n\x05Logic\x12\x46\n\x11registerDataUsage\x12\x17.coinlib.LogicDataUsage\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x14registerMonitorEvent\x12\x1a.coinlib.LogicMonitorEvent\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x12registerEventUsage\x12\x18.coinlib.LogicEventUsage\x1a\x16.google.protobuf.Empty\"\x00\x12R\n\x17registerCollectionUsage\x12\x1d.coinlib.LogicCollectionUsage\x1a\x16.google.protobuf.Empty\"\x00\x12:\n\x08runLogic\x12\x14.coinlib.LogicRunJob\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\x0eregisterTrader\x12 .coinlib.LogicTraderRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x10registerScreener\x12\".coinlib.LogicScreenerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12M\n\x11registerDataLogic\x12\x1e.coinlib.LogicDataRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x13\x61\x64\x64LogicToWorkspace\x12#.coinlib.WorkspaceLogicRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32Q\n\x06\x42roker\x12G\n\x0eregisterBroker\x12\x1b.coinlib.BrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xb2\x04\n\x0c\x42rokerWorker\x12>\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1b.coinlib.BrokerWorkerConfig\"\x00\x12\x46\n\x14OnBrokerErrorOccured\x12\x14.coinlib.BrokerError\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13WatchBrokerCommands\x12\".coinlib.BrokerCommandRegistration\x1a\x17.coinlib.BrokerCommands\"\x00(\x01\x30\x01\x12L\n\x11SendCommandAnswer\x12\x1d.coinlib.BrokerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12V\n\x16SendCommandAnswerError\x12\".coinlib.BrokerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12U\n\x15RegisterBrokerSession\x12\".coinlib.BrokerSessionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rOnBrokerEvent\x12\x18.coinlib.BrokerEventData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa1\x08\n\tAppWorker\x12;\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x18.coinlib.AppWorkerConfig\"\x00\x12L\n\x17OnAppWorkerErrorOccured\x12\x17.coinlib.AppWorkerError\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x13WatchBrokerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12\\\n\x10RunModuleCommand\x12\x1f.coinlib.AppWorkerModuleCommand\x1a%.coinlib.AppWorkerModuleCommandAnswer\"\x00\x12\\\n\x10RunBrokerCommand\x12\x1f.coinlib.AppWorkerBrokerCommand\x1a%.coinlib.AppWorkerBrokerCommandAnswer\"\x00\x12\x61\n\x16WatchAppWorkerCommands\x12%.coinlib.AppWorkerCommandRegistration\x1a\x1a.coinlib.AppWorkerCommands\"\x00(\x01\x30\x01\x12O\n\x11SendCommandAnswer\x12 .coinlib.AppWorkerCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x16SendCommandAnswerError\x12%.coinlib.AppWorkerCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x18OnAppWorkerLogicFinished\x12#.coinlib.AppWorkerFinishedStepInfos\x1a\x16.google.protobuf.Empty\"\x00\x12g\n\x18RegisterAppWorkerSession\x12%.coinlib.AppWorkerSessionRegistration\x1a\".coinlib.AppWorkerRegistrationInfo\"\x00\x12I\n\x10OnAppWorkerEvent\x12\x1b.coinlib.AppWorkerEventData\x1a\x16.google.protobuf.Empty\"\x00\x12O\n\x12OnBrokerTestResult\x12\x1f.coinlib.BrokerTestProtocolData\x1a\x16.google.protobuf.Empty\"\x00\x32\xa2\x04\n\rFeatureWorker\x12?\n\tGetConfig\x12\x12.coinlib.WorkerJob\x1a\x1c.coinlib.FeatureWorkerConfig\"\x00\x12\x41\n\x0eOnErrorOccured\x12\x15.coinlib.FeatureError\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\rWatchCommands\x12\x18.coinlib.FeatureCommands\x1a\x18.coinlib.FeatureCommands\"\x00(\x01\x30\x01\x12M\n\x11SendCommandAnswer\x12\x1e.coinlib.FeatureCommandsAnswer\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x16SendCommandAnswerError\x12#.coinlib.FeatureCommandsAnswerError\x1a\x16.google.protobuf.Empty\"\x00\x12Z\n\x0fRegisterSession\x12#.coinlib.FeatureSessionRegistration\x1a .coinlib.RegistrationInformation\"\x00\x12>\n\x07OnEvent\x12\x19.coinlib.FeatureEventData\x1a\x16.google.protobuf.Empty\"\x00\x32]\n\x06Symbol\x12S\n\x14registerSymbolBroker\x12!.coinlib.SymbolBrokerRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xc1\x03\n\x10\x44\x61taLoaderWorker\x12N\n\rgetAllSymbols\x12\x1e.coinlib.SymbolDataRequestInfo\x1a\x1b.coinlib.SymbolDataResponse\"\x00\x12T\n\x0fgetAllExchanges\x12 .coinlib.ExchangeDataRequestInfo\x1a\x1d.coinlib.ExchangeDataResponse\"\x00\x12J\n\rgetMarketData\x12\x1a.coinlib.MarketDataRequest\x1a\x1b.coinlib.MarketDataResponse\"\x00\x12M\n\x0egetFeatureData\x12\x1b.coinlib.FeatureDataRequest\x1a\x1c.coinlib.FeatureDataResponse\"\x00\x12l\n\x19getAdditionalDataFeatures\x12%.coinlib.AdditionalDataFeatureRequest\x1a&.coinlib.AdditionalDataFeatureResponse\"\x00\x32\x63\n\x0cNotification\x12S\n\x14registerNotification\x12!.coinlib.NotificationRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32U\n\x08\x46\x65\x61tures\x12I\n\x0fregisterFeature\x12\x1c.coinlib.FeatureRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xce\x01\n\nStatistics\x12\x65\n\x1dregisterStatisticRuleFunction\x12*.coinlib.StatisticRuleFunctionRegistration\x1a\x16.google.protobuf.Empty\"\x00\x12Y\n\x17registerStatisticMethod\x12$.coinlib.StatisticMethodRegistration\x1a\x16.google.protobuf.Empty\"\x00\x32\xf5\x01\n\x12\x44\x61taWorkerRegistry\x12\x31\n\ngetAuthKey\x12\x0f.coinlib.ApiKey\x1a\x10.coinlib.AuthKey\"\x00\x12J\n\x16getAllDataWorkerServer\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12`\n\x1bgetDataWorkerServerEndpoint\x12\x1e.coinlib.WorkerRegistryRequest\x1a\x1f.coinlib.WorkerRegistryResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dataWorker_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _STATISTICSRULEWORKERCONFIG_INPUTSENTRY._options = None
@@ -171,276 +171,278 @@
   _LOGICRUNNERSTATISTICS._serialized_end=11030
   _LOGICRUNNEROFFLINEWORKERPARTIALLYDATA._serialized_start=11033
   _LOGICRUNNEROFFLINEWORKERPARTIALLYDATA._serialized_end=11199
   _LOGICRUNNEROFFLINEWORKERERROR._serialized_start=11201
   _LOGICRUNNEROFFLINEWORKERERROR._serialized_end=11320
   _LOGICRUNNEROFFLINEWORKERFINISHEDDATA._serialized_start=11323
   _LOGICRUNNEROFFLINEWORKERFINISHEDDATA._serialized_end=11503
-  _WORKERPLUGININFORMATION._serialized_start=11505
-  _WORKERPLUGININFORMATION._serialized_end=11569
-  _WORKERSETTINGS._serialized_start=11571
-  _WORKERSETTINGS._serialized_end=11631
-  _WORKERREGISTRATION._serialized_start=11633
-  _WORKERREGISTRATION._serialized_end=11672
-  _COLLECTIONNODEREQUEST._serialized_start=11674
-  _COLLECTIONNODEREQUEST._serialized_end=11772
-  _COLLECTIONNODERESPONSE._serialized_start=11774
-  _COLLECTIONNODERESPONSE._serialized_end=11832
-  _EVENTREQUEST._serialized_start=11834
-  _EVENTREQUEST._serialized_end=11930
-  _PLUGINCONFIG._serialized_start=11932
-  _PLUGINCONFIG._serialized_end=12048
-  _PLUGININSTALLATIONOUTPUT._serialized_start=12050
-  _PLUGININSTALLATIONOUTPUT._serialized_end=12135
-  _SIMULATORCHARTCONFIGINDICATOR._serialized_start=12138
-  _SIMULATORCHARTCONFIGINDICATOR._serialized_end=12341
-  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_start=12296
-  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_end=12341
-  _SIMULATORCHARTCONFIG._serialized_start=12344
-  _SIMULATORCHARTCONFIG._serialized_end=12514
-  _SIMULATORSTATISTICCHARTCONFIG._serialized_start=12517
-  _SIMULATORSTATISTICCHARTCONFIG._serialized_end=12668
-  _SIMULATORMETHODCALLCHARTCONFIG._serialized_start=12671
-  _SIMULATORMETHODCALLCHARTCONFIG._serialized_end=12870
-  _SIMULATORRESPONSE._serialized_start=12872
-  _SIMULATORRESPONSE._serialized_end=12936
-  _SYMBOLBROKERSIMULATORREQUEST._serialized_start=12939
-  _SYMBOLBROKERSIMULATORREQUEST._serialized_end=13070
-  _SYMBOLBROKERSIMULATORRESPONSE._serialized_start=13072
-  _SYMBOLBROKERSIMULATORRESPONSE._serialized_end=13175
-  _BROKERSIMULATORBROKERLOGINDATA._serialized_start=13177
-  _BROKERSIMULATORBROKERLOGINDATA._serialized_end=13241
-  _BROKERSIMULATORBROKERDATA._serialized_start=13244
-  _BROKERSIMULATORBROKERDATA._serialized_end=13393
-  _BROKERSIMULATORREQUEST._serialized_start=13396
-  _BROKERSIMULATORREQUEST._serialized_end=13548
-  _BROKERSIMULATORRESPONSE._serialized_start=13551
-  _BROKERSIMULATORRESPONSE._serialized_end=13729
-  _NOTIFICATIONSIMULATORREQUEST._serialized_start=13731
-  _NOTIFICATIONSIMULATORREQUEST._serialized_end=13833
-  _NOTIFICATIONSIMULATORRESPONSE._serialized_start=13835
-  _NOTIFICATIONSIMULATORRESPONSE._serialized_end=13934
-  _FEATURESIMULATORREQUEST._serialized_start=13936
-  _FEATURESIMULATORREQUEST._serialized_end=14016
-  _FEATURESIMULATORRESPONSE._serialized_start=14018
-  _FEATURESIMULATORRESPONSE._serialized_end=14112
-  _LOGICINPUT._serialized_start=14114
-  _LOGICINPUT._serialized_end=14213
-  _LOGICTRADERREGISTRATION._serialized_start=14216
-  _LOGICTRADERREGISTRATION._serialized_end=14477
-  _LOGICALERTREGISTRATION._serialized_start=14480
-  _LOGICALERTREGISTRATION._serialized_end=14740
-  _LOGICDATAREGISTRATION._serialized_start=14743
-  _LOGICDATAREGISTRATION._serialized_end=15002
-  _LOGICSCREENERREGISTRATION._serialized_start=15005
-  _LOGICSCREENERREGISTRATION._serialized_end=15268
-  _WORKSPACELOGICREGISTRATION._serialized_start=15271
-  _WORKSPACELOGICREGISTRATION._serialized_end=15544
-  _LOGICRUNJOB._serialized_start=15546
-  _LOGICRUNJOB._serialized_end=15580
-  _LOGICDATAUSAGE._serialized_start=15583
-  _LOGICDATAUSAGE._serialized_end=15890
-  _LOGICMONITOREVENT._serialized_start=15893
-  _LOGICMONITOREVENT._serialized_end=16136
-  _LOGICCOLLECTIONUSAGE._serialized_start=16139
-  _LOGICCOLLECTIONUSAGE._serialized_end=16385
-  _LOGICEVENTUSAGE._serialized_start=16388
-  _LOGICEVENTUSAGE._serialized_end=16614
-  _SYMBOLBROKEROPTIONS._serialized_start=16616
-  _SYMBOLBROKEROPTIONS._serialized_end=16708
-  _SYMBOLBROKERREGISTRATION._serialized_start=16711
-  _SYMBOLBROKERREGISTRATION._serialized_end=16939
-  _BROKEROPTIONS._serialized_start=16941
-  _BROKEROPTIONS._serialized_end=17027
-  _BROKEREXCHANGE._serialized_start=17030
-  _BROKEREXCHANGE._serialized_end=17504
-  _BROKEREXCHANGE_LOGINMODE._serialized_start=17350
-  _BROKEREXCHANGE_LOGINMODE._serialized_end=17374
+  _WORKSPACEINFO._serialized_start=11505
+  _WORKSPACEINFO._serialized_end=11580
+  _WORKERPLUGININFORMATION._serialized_start=11582
+  _WORKERPLUGININFORMATION._serialized_end=11646
+  _WORKERSETTINGS._serialized_start=11648
+  _WORKERSETTINGS._serialized_end=11708
+  _WORKERREGISTRATION._serialized_start=11710
+  _WORKERREGISTRATION._serialized_end=11749
+  _COLLECTIONNODEREQUEST._serialized_start=11751
+  _COLLECTIONNODEREQUEST._serialized_end=11849
+  _COLLECTIONNODERESPONSE._serialized_start=11851
+  _COLLECTIONNODERESPONSE._serialized_end=11909
+  _EVENTREQUEST._serialized_start=11911
+  _EVENTREQUEST._serialized_end=12007
+  _PLUGINCONFIG._serialized_start=12009
+  _PLUGINCONFIG._serialized_end=12125
+  _PLUGININSTALLATIONOUTPUT._serialized_start=12127
+  _PLUGININSTALLATIONOUTPUT._serialized_end=12212
+  _SIMULATORCHARTCONFIGINDICATOR._serialized_start=12215
+  _SIMULATORCHARTCONFIGINDICATOR._serialized_end=12418
+  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_start=12373
+  _SIMULATORCHARTCONFIGINDICATOR_INPUTSENTRY._serialized_end=12418
+  _SIMULATORCHARTCONFIG._serialized_start=12421
+  _SIMULATORCHARTCONFIG._serialized_end=12591
+  _SIMULATORSTATISTICCHARTCONFIG._serialized_start=12594
+  _SIMULATORSTATISTICCHARTCONFIG._serialized_end=12745
+  _SIMULATORMETHODCALLCHARTCONFIG._serialized_start=12748
+  _SIMULATORMETHODCALLCHARTCONFIG._serialized_end=12947
+  _SIMULATORRESPONSE._serialized_start=12949
+  _SIMULATORRESPONSE._serialized_end=13013
+  _SYMBOLBROKERSIMULATORREQUEST._serialized_start=13016
+  _SYMBOLBROKERSIMULATORREQUEST._serialized_end=13147
+  _SYMBOLBROKERSIMULATORRESPONSE._serialized_start=13149
+  _SYMBOLBROKERSIMULATORRESPONSE._serialized_end=13252
+  _BROKERSIMULATORBROKERLOGINDATA._serialized_start=13254
+  _BROKERSIMULATORBROKERLOGINDATA._serialized_end=13318
+  _BROKERSIMULATORBROKERDATA._serialized_start=13321
+  _BROKERSIMULATORBROKERDATA._serialized_end=13470
+  _BROKERSIMULATORREQUEST._serialized_start=13473
+  _BROKERSIMULATORREQUEST._serialized_end=13625
+  _BROKERSIMULATORRESPONSE._serialized_start=13628
+  _BROKERSIMULATORRESPONSE._serialized_end=13806
+  _NOTIFICATIONSIMULATORREQUEST._serialized_start=13808
+  _NOTIFICATIONSIMULATORREQUEST._serialized_end=13910
+  _NOTIFICATIONSIMULATORRESPONSE._serialized_start=13912
+  _NOTIFICATIONSIMULATORRESPONSE._serialized_end=14011
+  _FEATURESIMULATORREQUEST._serialized_start=14013
+  _FEATURESIMULATORREQUEST._serialized_end=14093
+  _FEATURESIMULATORRESPONSE._serialized_start=14095
+  _FEATURESIMULATORRESPONSE._serialized_end=14189
+  _LOGICINPUT._serialized_start=14191
+  _LOGICINPUT._serialized_end=14290
+  _LOGICTRADERREGISTRATION._serialized_start=14293
+  _LOGICTRADERREGISTRATION._serialized_end=14554
+  _LOGICALERTREGISTRATION._serialized_start=14557
+  _LOGICALERTREGISTRATION._serialized_end=14817
+  _LOGICDATAREGISTRATION._serialized_start=14820
+  _LOGICDATAREGISTRATION._serialized_end=15079
+  _LOGICSCREENERREGISTRATION._serialized_start=15082
+  _LOGICSCREENERREGISTRATION._serialized_end=15345
+  _WORKSPACELOGICREGISTRATION._serialized_start=15348
+  _WORKSPACELOGICREGISTRATION._serialized_end=15621
+  _LOGICRUNJOB._serialized_start=15623
+  _LOGICRUNJOB._serialized_end=15657
+  _LOGICDATAUSAGE._serialized_start=15660
+  _LOGICDATAUSAGE._serialized_end=15967
+  _LOGICMONITOREVENT._serialized_start=15970
+  _LOGICMONITOREVENT._serialized_end=16213
+  _LOGICCOLLECTIONUSAGE._serialized_start=16216
+  _LOGICCOLLECTIONUSAGE._serialized_end=16462
+  _LOGICEVENTUSAGE._serialized_start=16465
+  _LOGICEVENTUSAGE._serialized_end=16691
+  _SYMBOLBROKEROPTIONS._serialized_start=16693
+  _SYMBOLBROKEROPTIONS._serialized_end=16785
+  _SYMBOLBROKERREGISTRATION._serialized_start=16788
+  _SYMBOLBROKERREGISTRATION._serialized_end=17016
+  _BROKEROPTIONS._serialized_start=17018
+  _BROKEROPTIONS._serialized_end=17104
+  _BROKEREXCHANGE._serialized_start=17107
+  _BROKEREXCHANGE._serialized_end=17581
+  _BROKEREXCHANGE_LOGINMODE._serialized_start=17427
+  _BROKEREXCHANGE_LOGINMODE._serialized_end=17451
   _BROKEREXCHANGE_CONTRACTTYPE._serialized_start=5790
   _BROKEREXCHANGE_CONTRACTTYPE._serialized_end=5873
   _BROKEREXCHANGE_ASSETTYPE._serialized_start=5745
   _BROKEREXCHANGE_ASSETTYPE._serialized_end=5788
-  _BROKERREGISTRATION._serialized_start=17507
-  _BROKERREGISTRATION._serialized_end=17931
-  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_start=17840
-  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_end=17931
-  _BROKERPORTFOLIO._serialized_start=17933
-  _BROKERPORTFOLIO._serialized_end=17996
-  _BROKERPORTFOLIOASSET._serialized_start=17998
-  _BROKERPORTFOLIOASSET._serialized_end=18088
-  _BROKERSESSIONACCOUNTINFO._serialized_start=18091
-  _BROKERSESSIONACCOUNTINFO._serialized_end=18479
+  _BROKERREGISTRATION._serialized_start=17584
+  _BROKERREGISTRATION._serialized_end=18008
+  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_start=17917
+  _BROKERREGISTRATION_SUPPORTEDBROKERTYPES._serialized_end=18008
+  _BROKERPORTFOLIO._serialized_start=18010
+  _BROKERPORTFOLIO._serialized_end=18073
+  _BROKERPORTFOLIOASSET._serialized_start=18075
+  _BROKERPORTFOLIOASSET._serialized_end=18165
+  _BROKERSESSIONACCOUNTINFO._serialized_start=18168
+  _BROKERSESSIONACCOUNTINFO._serialized_end=18556
   _BROKERSESSIONACCOUNTINFO_CONTRACTTYPE._serialized_start=5790
   _BROKERSESSIONACCOUNTINFO_CONTRACTTYPE._serialized_end=5873
   _BROKERSESSIONACCOUNTINFO_ASSETTYPE._serialized_start=5745
   _BROKERSESSIONACCOUNTINFO_ASSETTYPE._serialized_end=5788
-  _BROKERINFOSTARTSESSIONCONFIG._serialized_start=18482
-  _BROKERINFOSTARTSESSIONCONFIG._serialized_end=18637
-  _BROKERINFOTESTCONFIG._serialized_start=18640
-  _BROKERINFOTESTCONFIG._serialized_end=18884
-  _BROKERWORKERCONFIG._serialized_start=18886
-  _BROKERWORKERCONFIG._serialized_end=18989
-  _BROKERSTOPCONSUMERLISTENER._serialized_start=18991
-  _BROKERSTOPCONSUMERLISTENER._serialized_end=19055
-  _BROKERSTOPCONSUMERCOMMAND._serialized_start=19057
-  _BROKERSTOPCONSUMERCOMMAND._serialized_end=19101
-  _BROKERSTARTSESSIONINFO._serialized_start=19103
-  _BROKERSTARTSESSIONINFO._serialized_end=19127
-  _BROKERERROR._serialized_start=19129
-  _BROKERERROR._serialized_end=19232
-  _BROKERCOMMANDS._serialized_start=19234
-  _BROKERCOMMANDS._serialized_end=19340
-  _BROKERSESSIONREGISTRATION._serialized_start=19342
-  _BROKERSESSIONREGISTRATION._serialized_end=19388
-  _BROKERCOMMANDSANSWER._serialized_start=19390
-  _BROKERCOMMANDSANSWER._serialized_end=19470
-  _BROKERCOMMANDSANSWERERROR._serialized_start=19472
-  _BROKERCOMMANDSANSWERERROR._serialized_end=19572
-  _BROKEREVENTDATA._serialized_start=19574
-  _BROKEREVENTDATA._serialized_end=19675
-  _BROKERCOMMANDREGISTRATION._serialized_start=19677
-  _BROKERCOMMANDREGISTRATION._serialized_end=19723
-  _BROKERTESTPROTOCOLDATA._serialized_start=19725
-  _BROKERTESTPROTOCOLDATA._serialized_end=19799
-  _APPWORKERCONFIG._serialized_start=19802
-  _APPWORKERCONFIG._serialized_end=19958
-  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_start=19961
-  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_end=20258
-  _APPWORKERCOMMANDREGISTRATION._serialized_start=20260
-  _APPWORKERCOMMANDREGISTRATION._serialized_end=20309
-  _APPWORKERERROR._serialized_start=20311
-  _APPWORKERERROR._serialized_end=20398
-  _APPWORKERCOMMANDS._serialized_start=20400
-  _APPWORKERCOMMANDS._serialized_end=20513
-  _APPWORKERSESSIONREGISTRATION._serialized_start=20515
-  _APPWORKERSESSIONREGISTRATION._serialized_end=20600
-  _APPWORKERCOMMANDSANSWER._serialized_start=20602
-  _APPWORKERCOMMANDSANSWER._serialized_end=20685
-  _APPWORKERCOMMANDSANSWERERROR._serialized_start=20687
-  _APPWORKERCOMMANDSANSWERERROR._serialized_end=20790
-  _APPWORKEREVENTDATA._serialized_start=20792
-  _APPWORKEREVENTDATA._serialized_end=20896
-  _APPWORKERBROKERCOMMAND._serialized_start=20899
-  _APPWORKERBROKERCOMMAND._serialized_end=21030
-  _APPWORKERBROKERCOMMANDANSWER._serialized_start=21033
-  _APPWORKERBROKERCOMMANDANSWER._serialized_end=21192
-  _APPWORKERMODULECOMMAND._serialized_start=21195
-  _APPWORKERMODULECOMMAND._serialized_end=21342
-  _APPWORKERMODULECOMMANDANSWER._serialized_start=21345
-  _APPWORKERMODULECOMMANDANSWER._serialized_end=21553
-  _APPWORKERFINISHEDSTEPINFOS._serialized_start=21555
-  _APPWORKERFINISHEDSTEPINFOS._serialized_end=21658
-  _APPWORKERREGISTRATIONINFO._serialized_start=21660
-  _APPWORKERREGISTRATIONINFO._serialized_end=21759
-  _FEATUREINFOSTARTSESSIONCONFIG._serialized_start=21762
-  _FEATUREINFOSTARTSESSIONCONFIG._serialized_end=22063
-  _FEATUREWORKERCONFIG._serialized_start=22065
-  _FEATUREWORKERCONFIG._serialized_end=22170
-  _FEATUREERROR._serialized_start=22172
-  _FEATUREERROR._serialized_end=22257
-  _FEATURECOMMANDS._serialized_start=22259
-  _FEATURECOMMANDS._serialized_end=22354
-  _FEATURECOMMANDSANSWER._serialized_start=22356
-  _FEATURECOMMANDSANSWER._serialized_end=22437
-  _FEATURECOMMANDSANSWERERROR._serialized_start=22439
-  _FEATURECOMMANDSANSWERERROR._serialized_end=22540
-  _FEATURESESSIONREGISTRATION._serialized_start=22542
-  _FEATURESESSIONREGISTRATION._serialized_end=22589
-  _FEATUREEVENTDATA._serialized_start=22591
-  _FEATUREEVENTDATA._serialized_end=22693
-  _REGISTRATIONINFORMATION._serialized_start=22695
-  _REGISTRATIONINFORMATION._serialized_end=22757
-  _SYMBOLDATAREQUESTINFO._serialized_start=22759
-  _SYMBOLDATAREQUESTINFO._serialized_end=22832
-  _SYMBOLDATARESPONSE._serialized_start=22834
-  _SYMBOLDATARESPONSE._serialized_end=22905
-  _EXCHANGEDATAREQUESTINFO._serialized_start=22907
-  _EXCHANGEDATAREQUESTINFO._serialized_end=22932
-  _BROKEREXCHANGESMALL._serialized_start=22934
-  _BROKEREXCHANGESMALL._serialized_end=23010
-  _EXCHANGEDATARESPONSE._serialized_start=23012
-  _EXCHANGEDATARESPONSE._serialized_end=23083
-  _SYMBOLBROKERSYMBOLSMALL._serialized_start=23086
-  _SYMBOLBROKERSYMBOLSMALL._serialized_end=23388
-  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_start=23342
-  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_end=23388
-  _MARKETDATAREQUEST._serialized_start=23391
-  _MARKETDATAREQUEST._serialized_end=23569
-  _MARKETDATARESPONSE._serialized_start=23571
-  _MARKETDATARESPONSE._serialized_end=23675
-  _FEATUREDATARESPONSE._serialized_start=23677
-  _FEATUREDATARESPONSE._serialized_end=23782
-  _FEATUREDATAREQUEST._serialized_start=23785
-  _FEATUREDATAREQUEST._serialized_end=23945
-  _ADDITIONALDATAFEATUREREQUEST._serialized_start=23947
-  _ADDITIONALDATAFEATUREREQUEST._serialized_end=23977
-  _ADDITIONALDATAFEATUREINFO._serialized_start=23979
-  _ADDITIONALDATAFEATUREINFO._serialized_end=24100
-  _ADDITIONALDATAFEATURERESPONSE._serialized_start=24102
-  _ADDITIONALDATAFEATURERESPONSE._serialized_end=24191
-  _NOTIFICATIONOPTIONS._serialized_start=24193
-  _NOTIFICATIONOPTIONS._serialized_end=24285
-  _NOTIFICATIONREGISTRATION._serialized_start=24288
-  _NOTIFICATIONREGISTRATION._serialized_end=24559
-  _FEATUREOPTIONS._serialized_start=24561
-  _FEATUREOPTIONS._serialized_end=24648
-  _FEATUREREGISTRATION._serialized_start=24651
-  _FEATUREREGISTRATION._serialized_end=24973
-  _SIMULATORMETHODCALL._serialized_start=24975
-  _SIMULATORMETHODCALL._serialized_end=25028
-  _STATISTICFUNCTIONINPUTS._serialized_start=25030
-  _STATISTICFUNCTIONINPUTS._serialized_end=25126
-  _STATISTICMETHODINPUTS._serialized_start=25128
-  _STATISTICMETHODINPUTS._serialized_end=25238
-  _STATISTICMETHODREGISTRATION._serialized_start=25241
-  _STATISTICMETHODREGISTRATION._serialized_end=25526
-  _STATISTICRULEFUNCTIONREGISTRATION._serialized_start=25529
-  _STATISTICRULEFUNCTIONREGISTRATION._serialized_end=25788
-  _WORKERREGISTRYREQUEST._serialized_start=25790
-  _WORKERREGISTRYREQUEST._serialized_end=25855
-  _WORKERREGISTRYRESPONSE._serialized_start=25857
-  _WORKERREGISTRYRESPONSE._serialized_end=25925
-  _APIKEY._serialized_start=25927
-  _APIKEY._serialized_end=25972
-  _AUTHKEY._serialized_start=25974
-  _AUTHKEY._serialized_end=26022
-  _CHARTSWORKER._serialized_start=26025
-  _CHARTSWORKER._serialized_end=26271
-  _STATISTICSMETHODWORKER._serialized_start=26274
-  _STATISTICSMETHODWORKER._serialized_end=26559
-  _SYMBOLBROKERWORKER._serialized_start=26562
-  _SYMBOLBROKERWORKER._serialized_end=27376
-  _NOTIFICATIONWORKER._serialized_start=27379
-  _NOTIFICATIONWORKER._serialized_end=27644
-  _LOGICRUNNEROFFLINESERVICE._serialized_start=27647
-  _LOGICRUNNEROFFLINESERVICE._serialized_end=28040
-  _DATAWORKER._serialized_start=28043
-  _DATAWORKER._serialized_end=28760
-  _PLUGINWORKER._serialized_start=28763
-  _PLUGINWORKER._serialized_end=28922
-  _SIMULATOR._serialized_start=28925
-  _SIMULATOR._serialized_end=29596
-  _FUNCTIONS._serialized_start=29598
-  _FUNCTIONS._serialized_end=29707
-  _LOGIC._serialized_start=29710
-  _LOGIC._serialized_end=30410
-  _BROKER._serialized_start=30412
-  _BROKER._serialized_end=30493
-  _BROKERWORKER._serialized_start=30496
-  _BROKERWORKER._serialized_end=31058
-  _APPWORKER._serialized_start=31061
-  _APPWORKER._serialized_end=32118
-  _FEATUREWORKER._serialized_start=32121
-  _FEATUREWORKER._serialized_end=32667
-  _SYMBOL._serialized_start=32669
-  _SYMBOL._serialized_end=32762
-  _DATALOADERWORKER._serialized_start=32765
-  _DATALOADERWORKER._serialized_end=33214
-  _NOTIFICATION._serialized_start=33216
-  _NOTIFICATION._serialized_end=33315
-  _FEATURES._serialized_start=33317
-  _FEATURES._serialized_end=33402
-  _STATISTICS._serialized_start=33405
-  _STATISTICS._serialized_end=33611
-  _DATAWORKERREGISTRY._serialized_start=33614
-  _DATAWORKERREGISTRY._serialized_end=33859
+  _BROKERINFOSTARTSESSIONCONFIG._serialized_start=18559
+  _BROKERINFOSTARTSESSIONCONFIG._serialized_end=18714
+  _BROKERINFOTESTCONFIG._serialized_start=18717
+  _BROKERINFOTESTCONFIG._serialized_end=18961
+  _BROKERWORKERCONFIG._serialized_start=18963
+  _BROKERWORKERCONFIG._serialized_end=19066
+  _BROKERSTOPCONSUMERLISTENER._serialized_start=19068
+  _BROKERSTOPCONSUMERLISTENER._serialized_end=19132
+  _BROKERSTOPCONSUMERCOMMAND._serialized_start=19134
+  _BROKERSTOPCONSUMERCOMMAND._serialized_end=19178
+  _BROKERSTARTSESSIONINFO._serialized_start=19180
+  _BROKERSTARTSESSIONINFO._serialized_end=19204
+  _BROKERERROR._serialized_start=19206
+  _BROKERERROR._serialized_end=19309
+  _BROKERCOMMANDS._serialized_start=19311
+  _BROKERCOMMANDS._serialized_end=19417
+  _BROKERSESSIONREGISTRATION._serialized_start=19419
+  _BROKERSESSIONREGISTRATION._serialized_end=19465
+  _BROKERCOMMANDSANSWER._serialized_start=19467
+  _BROKERCOMMANDSANSWER._serialized_end=19547
+  _BROKERCOMMANDSANSWERERROR._serialized_start=19549
+  _BROKERCOMMANDSANSWERERROR._serialized_end=19649
+  _BROKEREVENTDATA._serialized_start=19651
+  _BROKEREVENTDATA._serialized_end=19752
+  _BROKERCOMMANDREGISTRATION._serialized_start=19754
+  _BROKERCOMMANDREGISTRATION._serialized_end=19800
+  _BROKERTESTPROTOCOLDATA._serialized_start=19802
+  _BROKERTESTPROTOCOLDATA._serialized_end=19876
+  _APPWORKERCONFIG._serialized_start=19879
+  _APPWORKERCONFIG._serialized_end=20035
+  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_start=20038
+  _APPWORKERINFOSTARTSESSIONCONFIG._serialized_end=20335
+  _APPWORKERCOMMANDREGISTRATION._serialized_start=20337
+  _APPWORKERCOMMANDREGISTRATION._serialized_end=20386
+  _APPWORKERERROR._serialized_start=20388
+  _APPWORKERERROR._serialized_end=20475
+  _APPWORKERCOMMANDS._serialized_start=20477
+  _APPWORKERCOMMANDS._serialized_end=20590
+  _APPWORKERSESSIONREGISTRATION._serialized_start=20592
+  _APPWORKERSESSIONREGISTRATION._serialized_end=20677
+  _APPWORKERCOMMANDSANSWER._serialized_start=20679
+  _APPWORKERCOMMANDSANSWER._serialized_end=20762
+  _APPWORKERCOMMANDSANSWERERROR._serialized_start=20764
+  _APPWORKERCOMMANDSANSWERERROR._serialized_end=20867
+  _APPWORKEREVENTDATA._serialized_start=20869
+  _APPWORKEREVENTDATA._serialized_end=20973
+  _APPWORKERBROKERCOMMAND._serialized_start=20976
+  _APPWORKERBROKERCOMMAND._serialized_end=21107
+  _APPWORKERBROKERCOMMANDANSWER._serialized_start=21110
+  _APPWORKERBROKERCOMMANDANSWER._serialized_end=21269
+  _APPWORKERMODULECOMMAND._serialized_start=21272
+  _APPWORKERMODULECOMMAND._serialized_end=21419
+  _APPWORKERMODULECOMMANDANSWER._serialized_start=21422
+  _APPWORKERMODULECOMMANDANSWER._serialized_end=21630
+  _APPWORKERFINISHEDSTEPINFOS._serialized_start=21632
+  _APPWORKERFINISHEDSTEPINFOS._serialized_end=21735
+  _APPWORKERREGISTRATIONINFO._serialized_start=21737
+  _APPWORKERREGISTRATIONINFO._serialized_end=21836
+  _FEATUREINFOSTARTSESSIONCONFIG._serialized_start=21839
+  _FEATUREINFOSTARTSESSIONCONFIG._serialized_end=22140
+  _FEATUREWORKERCONFIG._serialized_start=22142
+  _FEATUREWORKERCONFIG._serialized_end=22247
+  _FEATUREERROR._serialized_start=22249
+  _FEATUREERROR._serialized_end=22334
+  _FEATURECOMMANDS._serialized_start=22336
+  _FEATURECOMMANDS._serialized_end=22431
+  _FEATURECOMMANDSANSWER._serialized_start=22433
+  _FEATURECOMMANDSANSWER._serialized_end=22514
+  _FEATURECOMMANDSANSWERERROR._serialized_start=22516
+  _FEATURECOMMANDSANSWERERROR._serialized_end=22617
+  _FEATURESESSIONREGISTRATION._serialized_start=22619
+  _FEATURESESSIONREGISTRATION._serialized_end=22666
+  _FEATUREEVENTDATA._serialized_start=22668
+  _FEATUREEVENTDATA._serialized_end=22770
+  _REGISTRATIONINFORMATION._serialized_start=22772
+  _REGISTRATIONINFORMATION._serialized_end=22834
+  _SYMBOLDATAREQUESTINFO._serialized_start=22836
+  _SYMBOLDATAREQUESTINFO._serialized_end=22909
+  _SYMBOLDATARESPONSE._serialized_start=22911
+  _SYMBOLDATARESPONSE._serialized_end=22982
+  _EXCHANGEDATAREQUESTINFO._serialized_start=22984
+  _EXCHANGEDATAREQUESTINFO._serialized_end=23009
+  _BROKEREXCHANGESMALL._serialized_start=23011
+  _BROKEREXCHANGESMALL._serialized_end=23087
+  _EXCHANGEDATARESPONSE._serialized_start=23089
+  _EXCHANGEDATARESPONSE._serialized_end=23160
+  _SYMBOLBROKERSYMBOLSMALL._serialized_start=23163
+  _SYMBOLBROKERSYMBOLSMALL._serialized_end=23465
+  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_start=23419
+  _SYMBOLBROKERSYMBOLSMALL_COLUMNSENTRY._serialized_end=23465
+  _MARKETDATAREQUEST._serialized_start=23468
+  _MARKETDATAREQUEST._serialized_end=23646
+  _MARKETDATARESPONSE._serialized_start=23648
+  _MARKETDATARESPONSE._serialized_end=23752
+  _FEATUREDATARESPONSE._serialized_start=23754
+  _FEATUREDATARESPONSE._serialized_end=23859
+  _FEATUREDATAREQUEST._serialized_start=23862
+  _FEATUREDATAREQUEST._serialized_end=24022
+  _ADDITIONALDATAFEATUREREQUEST._serialized_start=24024
+  _ADDITIONALDATAFEATUREREQUEST._serialized_end=24054
+  _ADDITIONALDATAFEATUREINFO._serialized_start=24056
+  _ADDITIONALDATAFEATUREINFO._serialized_end=24177
+  _ADDITIONALDATAFEATURERESPONSE._serialized_start=24179
+  _ADDITIONALDATAFEATURERESPONSE._serialized_end=24268
+  _NOTIFICATIONOPTIONS._serialized_start=24270
+  _NOTIFICATIONOPTIONS._serialized_end=24362
+  _NOTIFICATIONREGISTRATION._serialized_start=24365
+  _NOTIFICATIONREGISTRATION._serialized_end=24636
+  _FEATUREOPTIONS._serialized_start=24638
+  _FEATUREOPTIONS._serialized_end=24725
+  _FEATUREREGISTRATION._serialized_start=24728
+  _FEATUREREGISTRATION._serialized_end=25050
+  _SIMULATORMETHODCALL._serialized_start=25052
+  _SIMULATORMETHODCALL._serialized_end=25105
+  _STATISTICFUNCTIONINPUTS._serialized_start=25107
+  _STATISTICFUNCTIONINPUTS._serialized_end=25203
+  _STATISTICMETHODINPUTS._serialized_start=25205
+  _STATISTICMETHODINPUTS._serialized_end=25315
+  _STATISTICMETHODREGISTRATION._serialized_start=25318
+  _STATISTICMETHODREGISTRATION._serialized_end=25603
+  _STATISTICRULEFUNCTIONREGISTRATION._serialized_start=25606
+  _STATISTICRULEFUNCTIONREGISTRATION._serialized_end=25865
+  _WORKERREGISTRYREQUEST._serialized_start=25867
+  _WORKERREGISTRYREQUEST._serialized_end=25932
+  _WORKERREGISTRYRESPONSE._serialized_start=25934
+  _WORKERREGISTRYRESPONSE._serialized_end=26002
+  _APIKEY._serialized_start=26004
+  _APIKEY._serialized_end=26049
+  _AUTHKEY._serialized_start=26051
+  _AUTHKEY._serialized_end=26099
+  _CHARTSWORKER._serialized_start=26102
+  _CHARTSWORKER._serialized_end=26348
+  _STATISTICSMETHODWORKER._serialized_start=26351
+  _STATISTICSMETHODWORKER._serialized_end=26636
+  _SYMBOLBROKERWORKER._serialized_start=26639
+  _SYMBOLBROKERWORKER._serialized_end=27453
+  _NOTIFICATIONWORKER._serialized_start=27456
+  _NOTIFICATIONWORKER._serialized_end=27721
+  _LOGICRUNNEROFFLINESERVICE._serialized_start=27724
+  _LOGICRUNNEROFFLINESERVICE._serialized_end=28214
+  _DATAWORKER._serialized_start=28217
+  _DATAWORKER._serialized_end=28934
+  _PLUGINWORKER._serialized_start=28937
+  _PLUGINWORKER._serialized_end=29096
+  _SIMULATOR._serialized_start=29099
+  _SIMULATOR._serialized_end=29770
+  _FUNCTIONS._serialized_start=29772
+  _FUNCTIONS._serialized_end=29881
+  _LOGIC._serialized_start=29884
+  _LOGIC._serialized_end=30584
+  _BROKER._serialized_start=30586
+  _BROKER._serialized_end=30667
+  _BROKERWORKER._serialized_start=30670
+  _BROKERWORKER._serialized_end=31232
+  _APPWORKER._serialized_start=31235
+  _APPWORKER._serialized_end=32292
+  _FEATUREWORKER._serialized_start=32295
+  _FEATUREWORKER._serialized_end=32841
+  _SYMBOL._serialized_start=32843
+  _SYMBOL._serialized_end=32936
+  _DATALOADERWORKER._serialized_start=32939
+  _DATALOADERWORKER._serialized_end=33388
+  _NOTIFICATION._serialized_start=33390
+  _NOTIFICATION._serialized_end=33489
+  _FEATURES._serialized_start=33491
+  _FEATURES._serialized_end=33576
+  _STATISTICS._serialized_start=33579
+  _STATISTICS._serialized_end=33785
+  _DATAWORKERREGISTRY._serialized_start=33788
+  _DATAWORKERREGISTRY._serialized_end=34033
 # @@protoc_insertion_point(module_scope)
```

### Comparing `coinlib-2.2.1/coinlib/dataWorker_pb2_grpc.py` & `coinlib-2.2.2/coinlib/dataWorker_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -722,14 +722,19 @@
             channel: A grpc.Channel.
         """
         self.GetConfig = channel.unary_unary(
                 '/coinlib.LogicRunnerOfflineService/GetConfig',
                 request_serializer=dataWorker__pb2.WorkerJob.SerializeToString,
                 response_deserializer=dataWorker__pb2.LogicRunnerOfflineWorkerConfig.FromString,
                 )
+        self.GetLogicConfigForWorkspace = channel.unary_unary(
+                '/coinlib.LogicRunnerOfflineService/GetLogicConfigForWorkspace',
+                request_serializer=dataWorker__pb2.WorkspaceInfo.SerializeToString,
+                response_deserializer=dataWorker__pb2.LogicRunnerOfflineWorkerConfig.FromString,
+                )
         self.OnRunnerPartiallyData = channel.unary_unary(
                 '/coinlib.LogicRunnerOfflineService/OnRunnerPartiallyData',
                 request_serializer=dataWorker__pb2.LogicRunnerOfflineWorkerPartiallyData.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.OnRunnerErrorOccured = channel.unary_unary(
                 '/coinlib.LogicRunnerOfflineService/OnRunnerErrorOccured',
@@ -748,14 +753,20 @@
 
     def GetConfig(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetLogicConfigForWorkspace(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def OnRunnerPartiallyData(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def OnRunnerErrorOccured(self, request, context):
@@ -774,14 +785,19 @@
 def add_LogicRunnerOfflineServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetConfig': grpc.unary_unary_rpc_method_handler(
                     servicer.GetConfig,
                     request_deserializer=dataWorker__pb2.WorkerJob.FromString,
                     response_serializer=dataWorker__pb2.LogicRunnerOfflineWorkerConfig.SerializeToString,
             ),
+            'GetLogicConfigForWorkspace': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetLogicConfigForWorkspace,
+                    request_deserializer=dataWorker__pb2.WorkspaceInfo.FromString,
+                    response_serializer=dataWorker__pb2.LogicRunnerOfflineWorkerConfig.SerializeToString,
+            ),
             'OnRunnerPartiallyData': grpc.unary_unary_rpc_method_handler(
                     servicer.OnRunnerPartiallyData,
                     request_deserializer=dataWorker__pb2.LogicRunnerOfflineWorkerPartiallyData.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'OnRunnerErrorOccured': grpc.unary_unary_rpc_method_handler(
                     servicer.OnRunnerErrorOccured,
@@ -817,14 +833,31 @@
         return grpc.experimental.unary_unary(request, target, '/coinlib.LogicRunnerOfflineService/GetConfig',
             dataWorker__pb2.WorkerJob.SerializeToString,
             dataWorker__pb2.LogicRunnerOfflineWorkerConfig.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetLogicConfigForWorkspace(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/coinlib.LogicRunnerOfflineService/GetLogicConfigForWorkspace',
+            dataWorker__pb2.WorkspaceInfo.SerializeToString,
+            dataWorker__pb2.LogicRunnerOfflineWorkerConfig.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def OnRunnerPartiallyData(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `coinlib-2.2.1/coinlib/drawable/CoinlibDrawable.py` & `coinlib-2.2.2/coinlib/drawable/CoinlibDrawable.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/drawable/WindowGrid.py` & `coinlib-2.2.2/coinlib/drawable/WindowGrid.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/event/EventConsumer.py` & `coinlib-2.2.2/coinlib/event/EventConsumer.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/event/EventInterface.py` & `coinlib-2.2.2/coinlib/event/EventInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/feature/CoinlibFeature.py` & `coinlib-2.2.2/coinlib/feature/CoinlibFeature.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/feature/CoinlibFeatureFetcher.py` & `coinlib-2.2.2/coinlib/feature/CoinlibFeatureFetcher.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/feature/CoinlibFeatureLake.py` & `coinlib-2.2.2/coinlib/feature/CoinlibFeatureLake.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/feature/FeatureDTO.py` & `coinlib-2.2.2/coinlib/feature/FeatureDTO.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/feature/FeatureWorker.py` & `coinlib-2.2.2/coinlib/feature/FeatureWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/feature/Features.py` & `coinlib-2.2.2/coinlib/feature/Features.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/helper.py` & `coinlib-2.2.2/coinlib/helper.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logger.py` & `coinlib-2.2.2/coinlib/logger.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/Logic.py` & `coinlib-2.2.2/coinlib/logics/Logic.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicBasicWorker.py` & `coinlib-2.2.2/coinlib/logics/LogicBasicWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicJob.py` & `coinlib-2.2.2/coinlib/logics/LogicJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicLoader.py` & `coinlib-2.2.2/coinlib/logics/LogicLoader.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicOfflineJob.py` & `coinlib-2.2.2/coinlib/logics/LogicOfflineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicOfflineWorker.py` & `coinlib-2.2.2/coinlib/logics/LogicOfflineWorker.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,35 +25,39 @@
 from coinlib.logics.offlineManager.LogicOfflineJobFakeSpotBroker import LogicOfflineJobFakeSpotBroker
 
 from coinlib.logics.manager.PortfolioModel import PortfolioModel
 
 class LogicOfflineWorker(LogicBasicWorker):
     _portfolio: PortfolioModel
 
+    def getJobConfig(self):
+        return self.logicInterface.GetConfig(self.workerJob, metadata=self.registrar.getAuthMetadata())
+
     def initialize(self):
         super().initialize()
-        self.logicInterface = stats.LogicRunnerOfflineServiceStub(self.getChannel())
-        logicInfoFullData = self.logicInterface.GetConfig(self.workerJob, metadata=self.registrar.getAuthMetadata())
-        self.logicConfig = logicInfoFullData.logicInfo
-        self.appWorkerId = self.logicConfig.app_worker_id
-        self.onlySignals = logicInfoFullData.onlySignals
-        self.appWorkerRunnerId = self.logicConfig.app_worker_runner_id
-        self.logicMode = self.logicConfig.logicMode
-        self._portfolio = PortfolioModel()
-        self.logicOptions = {}
-        try:
-            self.logicOptions = json.loads(self.logicConfig.options_json)
-        except:
-            pass
-        self.makerFee = self.logicOptions["makerFee"]
-        self.takerFee = self.logicOptions["takerFee"]
-        self.advancedDataInfo = json.loads(logicInfoFullData.advancedDataInfo)
-        self.startDate = pd.Timestamp(self.logicConfig.startDate)  # .tz_localize(None)
-        self.endDate = pd.Timestamp(self.logicConfig.endDate) #  .tz_localize(None)
-        self.chartConfigData = logicInfoFullData.chartData
+        if self.getChannel() is not None:
+            self.logicInterface = stats.LogicRunnerOfflineServiceStub(self.getChannel())
+            logicInfoFullData = self.getJobConfig()
+            self.logicConfig = logicInfoFullData.logicInfo
+            self.appWorkerId = self.logicConfig.app_worker_id
+            self.onlySignals = logicInfoFullData.onlySignals
+            self.appWorkerRunnerId = self.logicConfig.app_worker_runner_id
+            self.logicMode = self.logicConfig.logicMode
+            self._portfolio = PortfolioModel()
+            self.logicOptions = {}
+            try:
+                self.logicOptions = json.loads(self.logicConfig.options_json)
+            except:
+                pass
+            self.makerFee = self.logicOptions["makerFee"]
+            self.takerFee = self.logicOptions["takerFee"]
+            self.advancedDataInfo = json.loads(logicInfoFullData.advancedDataInfo)
+            self.startDate = pd.Timestamp(self.logicConfig.startDate)  # .tz_localize(None)
+            self.endDate = pd.Timestamp(self.logicConfig.endDate) #  .tz_localize(None)
+            self.chartConfigData = logicInfoFullData.chartData
         return True
 
 
     def getLogicMode(self):
         return self.logicMode
 
     def onLogicRunnerError(self, job, error):
@@ -213,15 +217,15 @@
             self.logger().error(tb)
             self.extractLogicInfosFromManagerData(infoBlock)
             self.onLogicRunnerError(None, e)
             return False
 
         self.extractLogicInfosFromManagerData(infoBlock)
 
-        self.onLogicRunningFinished()
+        self.finishedData = self.onLogicRunningFinished()
 
         return True
 
     def onNextSubTableReceived(self, fakeManager: LogicManager, subTable: DataTable):
         pass
```

### Comparing `coinlib-2.2.1/coinlib/logics/LogicOfflineWorkerTrader.py` & `coinlib-2.2.2/coinlib/logics/LogicOfflineWorkerTrader.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from coinlib.logics.manager.PortfolioModel import PortfolioModel
 from coinlib.logics.offlineManager.LogicOfflineJobFakeFutureBroker import LogicOfflineJobFakeFutureBroker
 from coinlib.logics.offlineManager.LogicOfflineJobFakeSpotBroker import LogicOfflineJobFakeSpotBroker
 
 
 class LogicOfflineWorkerTrader(LogicOfflineWorker):
 
+    _portfolio: PortfolioModel = None
     def initialize(self):
         super().initialize()
-
         self._portfolio = PortfolioModel.from_stats_model(self.logicConfig.portfolio)
 
     def onNextSubTableReceived(self, fakeManager: LogicManager, subTable: DataTable):
         fakeManager.broker.setTable(subTable)
 
     def onBeforeSingleStepRunng(self, fakeManager: LogicManager, subTable: DataTable):
         # first we run this and then the next one
```

### Comparing `coinlib-2.2.1/coinlib/logics/LogicOnlineJob.py` & `coinlib-2.2.2/coinlib/logics/LogicOnlineJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicOnlineWorker.py` & `coinlib-2.2.2/coinlib/logics/LogicOnlineWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicRegistrationInstance.py` & `coinlib-2.2.2/coinlib/logics/LogicRegistrationInstance.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/LogicTestBrokerWorker.py` & `coinlib-2.2.2/coinlib/logics/LogicTestBrokerWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/broker/LogicBrokerInterface.py` & `coinlib-2.2.2/coinlib/logics/broker/LogicBrokerInterface.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/manager/LogicJobBroker.py` & `coinlib-2.2.2/coinlib/logics/manager/LogicJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/manager/LogicManager.py` & `coinlib-2.2.2/coinlib/logics/manager/LogicManager.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/manager/PortfolioModel.py` & `coinlib-2.2.2/coinlib/logics/manager/PortfolioModel.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py` & `coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeBroker.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,19 +202,19 @@
         if len(foundCharts) > 0:
             foundCharts.sort(key=lambda x: x["timeframe"])
             return foundCharts[0]["chartId"]
 
         return None
 
     def getNow_date(self):
-        dt = self.table.getLast("datetime")
+        dt = self.table.getLastIndex()
         return dt
 
     def getNow(self):
-        dt = self.table.getLast("datetime")
+        dt = self.table.getLastIndex()
         date =  datetime.datetime.strftime(dt, "%Y-%m-%dT%H:%M:%S.%fZ")
         return date
 
     def getPrice(self, symbol:str=None, base: str = None, quote: str = None):
 
         if symbol is None:
             price = self.getPrice(symbol=base+"/"+quote)
@@ -402,14 +402,15 @@
         self._portfolioPercentage = ((self._moneyInPortfolio / self._startMoney) - 1) * 100
 
         if self._lastMoney is not None and self._lastMoney != self._moneyInPortfolio:
             self._portfolioTimeline.append({"date": self.getNow(), "portfolioMoney": self._moneyInPortfolio})
 
         self._lastMoney = self._moneyInPortfolio
 
+
         return True
 
     def executeOrder(self, order: FakeOrder):
         self._tradesCnt = self._tradesCnt + 1
         symbol_price = self.getPrice(order.symbol.symbol)
         if symbol_price is None:
             print("ERROR")
```

### Comparing `coinlib-2.2.1/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py` & `coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeFutureBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py` & `coinlib-2.2.2/coinlib/logics/offlineManager/LogicOfflineJobFakeSpotBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/logics/onlineManager/LogicOnlineJobBroker.py` & `coinlib-2.2.2/coinlib/logics/onlineManager/LogicOnlineJobBroker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/notification/Notification.py` & `coinlib-2.2.2/coinlib/notification/Notification.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/notification/NotificationWorker.py` & `coinlib-2.2.2/coinlib/notification/NotificationWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/statistics/StatisticMethodJob.py` & `coinlib-2.2.2/coinlib/statistics/StatisticMethodJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/statistics/StatisticRuleJob.py` & `coinlib-2.2.2/coinlib/statistics/StatisticRuleJob.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/statistics/Statistics.py` & `coinlib-2.2.2/coinlib/statistics/Statistics.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/statistics/StatisticsMethodWorker.py` & `coinlib-2.2.2/coinlib/statistics/StatisticsMethodWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/statistics/StatisticsRuleWorker.py` & `coinlib-2.2.2/coinlib/statistics/StatisticsRuleWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/symbols/SymbolWorker.py` & `coinlib-2.2.2/coinlib/symbols/SymbolWorker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib/symbols/Symbols.py` & `coinlib-2.2.2/coinlib/symbols/Symbols.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/coinlib.egg-info/PKG-INFO` & `coinlib-2.2.2/coinlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinlib
-Version: 2.2.1
+Version: 2.2.2
 Summary: Develop new code for your coindeck environment
 Home-page: https://gitlab.com/coindeck/coinlib
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `coinlib-2.2.1/coinlib.egg-info/SOURCES.txt` & `coinlib-2.2.2/coinlib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 coinlib/BasicJob.py
 coinlib/BasicJobSessionStorage.py
 coinlib/ChartsFactory.py
 coinlib/ChartsIndicatorJob.py
 coinlib/ChartsWorker.py
 coinlib/CoinlibCrypto.py
 coinlib/CoinlibDataInterface.py
+coinlib/CoinlibWorkspace.py
 coinlib/DataWorker.py
 coinlib/Functions.py
 coinlib/InfluxDatabase.py
 coinlib/PluginLoader.py
 coinlib/PluginsWorker.py
 coinlib/Registrar.py
 coinlib/Simulator.py
@@ -105,8 +106,9 @@
 coinlib/statistics/StatisticsRuleWorker.py
 coinlib/statistics/__init__.py
 coinlib/symbols/SymbolFactory.py
 coinlib/symbols/SymbolWorker.py
 coinlib/symbols/Symbols.py
 coinlib/symbols/__init__.py
 test/testchartworker.py
-test/testcross.py
+test/testcross.py
+test/testplot.py
```

### Comparing `coinlib-2.2.1/setup.py` & `coinlib-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README_pip.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="coinlib",
-    version="2.2.1",
+    version="2.2.2",
     description="Develop new code for your coindeck environment",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/coindeck/coinlib",
     author="coindeck",
     author_email="donnercody86@gmail.com",
     license="MIT",
```

### Comparing `coinlib-2.2.1/test/testchartworker.py` & `coinlib-2.2.2/test/testchartworker.py`

 * *Files identical despite different names*

### Comparing `coinlib-2.2.1/test/testcross.py` & `coinlib-2.2.2/test/testcross.py`

 * *Files identical despite different names*

