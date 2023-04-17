# Comparing `tmp/iqrfpy-0.1.6.tar.gz` & `tmp/iqrfpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy-0.1.6.tar", last modified: Sat Apr 15 08:21:22 2023, max compression
+gzip compressed data, was "iqrfpy-0.1.7.tar", last modified: Mon Apr 17 12:38:20 2023, max compression
```

## Comparing `iqrfpy-0.1.6.tar` & `iqrfpy-0.1.7.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.6/.editorconfig
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.6/.gitignore
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/.gitlab-ci.yml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/.pylintrc
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.6/LICENSE
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      699 2023-04-15 05:33:58.000000 iqrfpy-0.1.6/Makefile
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.6/README.md
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.223226 iqrfpy-0.1.6/examples/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2081 2023-03-25 07:08:59.000000 iqrfpy-0.1.6/examples/response_factories.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.223226 iqrfpy-0.1.6/iqrfpy/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      111 2023-04-15 08:21:05.000000 iqrfpy-0.1.6/iqrfpy/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       90 2023-03-24 10:27:58.000000 iqrfpy-0.1.6/iqrfpy/enums/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5379 2023-03-24 10:38:31.000000 iqrfpy-0.1.6/iqrfpy/enums/commands.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4646 2023-03-24 10:31:05.000000 iqrfpy-0.1.6/iqrfpy/enums/message_types.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      708 2023-03-24 10:49:19.000000 iqrfpy-0.1.6/iqrfpy/enums/peripherals.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-07 15:58:03.000000 iqrfpy-0.1.6/iqrfpy/exceptions.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.6/iqrfpy/messages/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2454 2023-04-15 07:42:07.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/IRequest.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      184 2023-04-15 05:52:25.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-04-15 07:16:20.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2023-04-15 07:17:50.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1595 2023-04-15 07:21:20.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2400 2023-04-15 07:23:56.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1044 2023-04-15 07:22:26.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2023-04-15 07:24:16.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1060 2023-04-15 07:24:30.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2044 2023-04-15 07:26:04.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1677 2023-04-15 07:26:47.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1879 2023-04-15 07:28:01.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1465 2023-04-15 07:28:26.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2389 2023-04-15 08:13:58.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2135 2023-04-15 07:33:11.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5293 2023-04-15 07:39:44.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2023-03-16 15:28:35.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/Raw.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/RawHdp.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      957 2023-04-15 07:43:28.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/uart/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     8383 2023-04-15 07:00:07.000000 iqrfpy-0.1.6/iqrfpy/messages/response_factory.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2735 2023-04-15 08:08:05.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/AsyncResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2484 2023-04-15 08:09:36.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/Confirmation.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3277 2023-04-15 08:09:43.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/IResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      214 2023-04-15 05:57:36.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2548 2023-04-15 07:49:09.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2023-04-15 07:51:29.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2468 2023-04-15 07:52:33.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2582 2023-04-15 07:55:01.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2023-04-15 07:54:09.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2231 2023-04-15 07:56:16.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2627 2023-04-15 07:57:08.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2475 2023-04-15 07:58:02.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2480 2023-04-15 07:58:52.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2039 2023-04-15 07:59:57.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2622 2023-04-15 08:01:05.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2634 2023-04-15 08:02:04.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2033 2023-04-15 08:03:57.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2023-04-15 08:04:34.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      983 2023-03-24 07:27:46.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:54.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:49.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:19.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2579 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/uart/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/transports/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/iqrfpy/transports/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2133 2023-04-06 09:43:24.000000 iqrfpy-0.1.6/iqrfpy/transports/itransport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2076 2023-03-24 09:57:48.000000 iqrfpy-0.1.6/iqrfpy/transports/mqtt_transport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-03-24 09:57:48.000000 iqrfpy-0.1.6/iqrfpy/transports/udp_transport.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.6/iqrfpy/utils/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    20492 2023-04-15 08:13:29.000000 iqrfpy-0.1.6/iqrfpy/utils/common.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1810 2023-04-15 07:47:59.000000 iqrfpy-0.1.6/iqrfpy/utils/dpa.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-04-15 06:15:47.000000 iqrfpy-0.1.6/iqrfpy/utils/enums.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.223226 iqrfpy-0.1.6/iqrfpy.egg-info/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6218 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.6/pyproject.toml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.6/requirements.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/setup.cfg
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/test_requirements.txt
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.6/tests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.6/tests/enums/Peripherals_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1292 2023-03-18 09:19:32.000000 iqrfpy-0.1.6/tests/messages/requests/IRequest_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      869 2023-03-18 09:24:49.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/AddrInfoRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4015 2023-04-02 10:26:13.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-03-18 09:44:00.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/BackupRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3758 2023-03-18 09:50:37.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/BondNodeRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      903 2023-03-18 09:24:46.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/BondedDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-03-18 09:57:38.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      925 2023-03-18 09:59:43.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-03-18 10:11:35.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveryRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2322 2023-03-18 10:17:19.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/RemoveBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-03-18 10:45:18.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/RestoreRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2257 2023-03-18 10:55:51.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3672 2023-03-18 11:08:56.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SetHopsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3511 2023-03-18 11:37:09.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SetMIDRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11030 2023-03-19 07:20:25.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SmartConnectRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4827 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/response_factory_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2162 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/AsyncResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/Confirmation_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4325 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/AddrInfoResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4514 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4765 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/BackupResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4391 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/BondNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4212 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/BondedDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3155 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4344 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveryResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3795 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/RemoveNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3055 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/RestoreResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3931 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4491 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SetHopsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3053 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SetMIDResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4487 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SmartConnectResponse_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    16223 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/utils/Common_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/tox.ini
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.7/.editorconfig
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.7/.gitignore
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/.gitlab-ci.yml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/.pylintrc
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.7/LICENSE
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      699 2023-04-15 05:33:58.000000 iqrfpy-0.1.7/Makefile
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.7/README.md
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.442591 iqrfpy-0.1.7/examples/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2151 2023-04-17 12:28:14.000000 iqrfpy-0.1.7/examples/response_factories.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.442591 iqrfpy-0.1.7/iqrfpy/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      111 2023-04-17 12:36:47.000000 iqrfpy-0.1.7/iqrfpy/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       90 2023-03-24 10:27:58.000000 iqrfpy-0.1.7/iqrfpy/enums/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5379 2023-03-24 10:38:31.000000 iqrfpy-0.1.7/iqrfpy/enums/commands.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4646 2023-03-24 10:31:05.000000 iqrfpy-0.1.7/iqrfpy/enums/message_types.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      708 2023-03-24 10:49:19.000000 iqrfpy-0.1.7/iqrfpy/enums/peripherals.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-07 15:58:03.000000 iqrfpy-0.1.7/iqrfpy/exceptions.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/messages/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.7/iqrfpy/messages/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/messages/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2454 2023-04-15 07:42:07.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/IRequest.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      184 2023-04-15 05:52:25.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.446591 iqrfpy-0.1.7/iqrfpy/messages/requests/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-04-15 07:16:20.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AddrInfo.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2023-04-17 12:15:28.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AuthorizeBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1595 2023-04-15 07:21:20.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2400 2023-04-15 07:23:56.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondNode.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1044 2023-04-15 07:22:26.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondedDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2023-04-15 07:24:16.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/ClearAllBonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1060 2023-04-15 07:24:30.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2044 2023-04-15 07:26:04.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1677 2023-04-15 07:26:47.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/RemoveBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1879 2023-04-15 07:28:01.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1465 2023-04-15 07:28:26.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetDpaParams.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2389 2023-04-15 08:13:58.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetHops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2135 2023-04-15 07:33:11.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetMID.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5293 2023-04-15 07:39:44.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SmartConnect.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2023-03-16 15:28:35.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/Raw.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/RawHdp.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      957 2023-04-15 07:43:28.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/node/Read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/requests/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.7/iqrfpy/messages/requests/uart/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     8383 2023-04-15 07:00:07.000000 iqrfpy-0.1.7/iqrfpy/messages/response_factory.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2735 2023-04-15 08:08:05.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/AsyncResponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2484 2023-04-15 08:09:36.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/Confirmation.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3277 2023-04-15 08:09:43.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/IResponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      214 2023-04-15 05:57:36.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.450591 iqrfpy-0.1.7/iqrfpy/messages/responses/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2548 2023-04-15 07:49:09.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AddrInfo.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2023-04-15 07:51:29.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AuthorizeBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2468 2023-04-15 07:52:33.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2582 2023-04-15 07:55:01.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondNode.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2023-04-15 07:54:09.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondedDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2231 2023-04-15 07:56:16.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/ClearAllBonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2627 2023-04-15 07:57:08.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2475 2023-04-15 07:58:02.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2480 2023-04-15 07:58:52.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/RemoveBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2039 2023-04-15 07:59:57.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2622 2023-04-15 08:01:05.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetDpaParams.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2634 2023-04-15 08:02:04.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetHops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2033 2023-04-15 08:03:57.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetMID.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2023-04-15 08:04:34.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SmartConnect.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      983 2023-03-24 07:27:46.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:54.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:49.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:19.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2579 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/node/Read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/messages/responses/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.7/iqrfpy/messages/responses/uart/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/transports/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/iqrfpy/transports/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2786 2023-04-17 12:36:20.000000 iqrfpy-0.1.7/iqrfpy/transports/itransport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2076 2023-03-24 09:57:48.000000 iqrfpy-0.1.7/iqrfpy/transports/mqtt_transport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-03-24 09:57:48.000000 iqrfpy-0.1.7/iqrfpy/transports/udp_transport.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/iqrfpy/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.7/iqrfpy/utils/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    20492 2023-04-15 08:13:29.000000 iqrfpy-0.1.7/iqrfpy/utils/common.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1810 2023-04-15 07:47:59.000000 iqrfpy-0.1.7/iqrfpy/utils/dpa.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-04-15 06:15:47.000000 iqrfpy-0.1.7/iqrfpy/utils/enums.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.442591 iqrfpy-0.1.7/iqrfpy.egg-info/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6218 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-17 12:38:20.000000 iqrfpy-0.1.7/iqrfpy.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.7/pyproject.toml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.7/requirements.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/setup.cfg
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/test_requirements.txt
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/tests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.7/tests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/tests/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.7/tests/enums/Peripherals_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.454591 iqrfpy-0.1.7/tests/messages/
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.458591 iqrfpy-0.1.7/tests/messages/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1292 2023-03-18 09:19:32.000000 iqrfpy-0.1.7/tests/messages/requests/IRequest_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.458591 iqrfpy-0.1.7/tests/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      869 2023-03-18 09:24:49.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/AddrInfoRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4015 2023-04-02 10:26:13.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-03-18 09:44:00.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/BackupRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3758 2023-03-18 09:50:37.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/BondNodeRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      903 2023-03-18 09:24:46.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/BondedDevicesRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-03-18 09:57:38.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      925 2023-03-18 09:59:43.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-03-18 10:11:35.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveryRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2322 2023-03-18 10:17:19.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/RemoveBondRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-03-18 10:45:18.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/RestoreRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2257 2023-03-18 10:55:51.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3672 2023-03-18 11:08:56.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SetHopsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3511 2023-03-18 11:37:09.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SetMIDRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11030 2023-03-19 07:20:25.000000 iqrfpy-0.1.7/tests/messages/requests/coordinator/SmartConnectRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4827 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/response_factory_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.458591 iqrfpy-0.1.7/tests/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2162 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/AsyncResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/Confirmation_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/tests/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4325 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/AddrInfoResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4514 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4765 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/BackupResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4391 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/BondNodeResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4212 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/BondedDevicesResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3155 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4344 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveryResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3795 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/RemoveNodeResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3055 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/RestoreResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3931 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4491 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SetHopsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3053 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SetMIDResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4487 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/messages/responses/coordinator/SmartConnectResponse_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-17 12:38:20.462592 iqrfpy-0.1.7/tests/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    16223 2023-04-15 05:36:55.000000 iqrfpy-0.1.7/tests/utils/Common_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.7/tox.ini
```

### Comparing `iqrfpy-0.1.6/.gitlab-ci.yml` & `iqrfpy-0.1.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/LICENSE` & `iqrfpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/Makefile` & `iqrfpy-0.1.7/Makefile`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/PKG-INFO` & `iqrfpy-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.6/examples/response_factories.py` & `iqrfpy-0.1.7/examples/response_factories.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from iqrfpy.messages.requests.coordinator import AuthorizeBondRequest
 from iqrfpy.messages.responses.coordinator import *
 from iqrfpy.messages.response_factory import ResponseFactory
 
 
 def handle_addr_info_response(response: AddrInfoResponse) -> None:
     print(f'peripheral: {response.get_pnum()}')
     print(f'peripheral command: {response.get_pcmd()}')
```

### Comparing `iqrfpy-0.1.6/iqrfpy/enums/commands.py` & `iqrfpy-0.1.7/iqrfpy/enums/commands.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/enums/message_types.py` & `iqrfpy-0.1.7/iqrfpy/enums/message_types.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/enums/peripherals.py` & `iqrfpy-0.1.7/iqrfpy/enums/peripherals.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/exceptions.py` & `iqrfpy-0.1.7/iqrfpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/IRequest.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/IRequest.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AddrInfo.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AddrInfo.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/AuthorizeBond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Backup.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Backup.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondNode.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondNode.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondedDevices.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/BondedDevices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/ClearAllBonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Discovery.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Discovery.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/RemoveBond.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/RemoveBond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Restore.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/Restore.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetDpaParams.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetDpaParams.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetHops.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetHops.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetMID.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SetMID.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SmartConnect.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/SmartConnect.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/__init__.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/requests/node/Read.py` & `iqrfpy-0.1.7/iqrfpy/messages/requests/node/Read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/response_factory.py` & `iqrfpy-0.1.7/iqrfpy/messages/response_factory.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/AsyncResponse.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/AsyncResponse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/Confirmation.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/Confirmation.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/IResponse.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/IResponse.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/AddrInfo.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AddrInfo.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/AuthorizeBond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Backup.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Backup.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondNode.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondNode.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondedDevices.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/BondedDevices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/ClearAllBonds.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Discovery.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Discovery.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/RemoveBond.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/RemoveBond.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Restore.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/Restore.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetDpaParams.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetDpaParams.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetHops.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetHops.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetMID.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SetMID.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SmartConnect.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/SmartConnect.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/__init__.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/messages/responses/node/Read.py` & `iqrfpy-0.1.7/iqrfpy/messages/responses/node/Read.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/transports/itransport.py` & `iqrfpy-0.1.7/iqrfpy/transports/itransport.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
 Transport abstract class.
 """
 from abc import ABC, abstractmethod
 from typing import Callable
 from iqrfpy.messages.requests.IRequest import IRequest
 from iqrfpy.messages.responses.IResponse import IResponse
+from iqrfpy.messages.responses.Confirmation import Confirmation
 
 
 class ITransport(ABC):
     """
     Abstract class providing interface for communication channels.
 
     Methods
     -------
     initialize() -> None:
         Initializes transport and creates connection if applicable.
     send(request: IRequest) -> None:
         Serialize passed request to format acceptable by the communication channel and send request.
     receive() -> IResponse:
         Receive a response synchronously, deserialize data from communication channel to a response object.
-    receive_async(callback: Callable[[IResponse], None]) -> None:
+    confirmation() -> Confirmation:
+
+    set_receive_callback(callback: Callable[[IResponse], None]) -> None:
         Receive a response asynchronously, deserialize data from communication channel to a response object
         and execute a callback if a function was passed.
     """
 
     def initialize(self) -> None:
         """
         Initialize transport and create a connection if applicable.
@@ -45,14 +48,36 @@
 
         Returns
         -------
         None
         """
         raise NotImplementedError("Abstract method not implemented.")
 
+    def receive(self) -> IResponse:
+        """
+        Return first unhandled response.
+
+        Returns
+        -------
+        response: IResponse
+            Response object
+        """
+        raise NotImplementedError("Abstract method not implemented.")
+
+    def confirmation(self) -> Confirmation:
+        """
+        Return first unhandled confirmation.
+
+        Returns
+        -------
+        confirmation: Confirmation
+            Confirmation object
+        """
+        raise NotImplementedError("Abstract method not implemented.")
+
     def set_receive_callback(self, callback: Callable[[IResponse], None]) -> None:
         """
         Receive a response asynchronously, deserialize data from communication channel to a response object
         and execute a callback if a function was passed.
 
         Parameters
         ----------
```

### Comparing `iqrfpy-0.1.6/iqrfpy/transports/mqtt_transport.py` & `iqrfpy-0.1.7/iqrfpy/transports/mqtt_transport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/transports/udp_transport.py` & `iqrfpy-0.1.7/iqrfpy/transports/udp_transport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/utils/common.py` & `iqrfpy-0.1.7/iqrfpy/utils/common.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy/utils/dpa.py` & `iqrfpy-0.1.7/iqrfpy/utils/dpa.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/iqrfpy.egg-info/PKG-INFO` & `iqrfpy-0.1.7/iqrfpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.6/iqrfpy.egg-info/SOURCES.txt` & `iqrfpy-0.1.7/iqrfpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/setup.cfg` & `iqrfpy-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/enums/Peripherals_test.py` & `iqrfpy-0.1.7/tests/enums/Peripherals_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/IRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/IRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/AddrInfoRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/AddrInfoRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/BackupRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/BackupRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/BondNodeRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/BondNodeRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/BondedDevicesRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/BondedDevicesRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveryRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/DiscoveryRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/RemoveBondRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/RemoveBondRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/RestoreRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/RestoreRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/SetHopsRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/SetHopsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/SetMIDRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/SetMIDRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/requests/coordinator/SmartConnectRequest_test.py` & `iqrfpy-0.1.7/tests/messages/requests/coordinator/SmartConnectRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/response_factory_test.py` & `iqrfpy-0.1.7/tests/messages/response_factory_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/AsyncResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/AsyncResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/Confirmation_test.py` & `iqrfpy-0.1.7/tests/messages/responses/Confirmation_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/AddrInfoResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/AddrInfoResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/BackupResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/BackupResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/BondNodeResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/BondNodeResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/BondedDevicesResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/BondedDevicesResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveryResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/DiscoveryResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/RemoveNodeResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/RemoveNodeResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/RestoreResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/RestoreResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/SetHopsResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/SetHopsResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/SetMIDResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/SetMIDResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/messages/responses/coordinator/SmartConnectResponse_test.py` & `iqrfpy-0.1.7/tests/messages/responses/coordinator/SmartConnectResponse_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.6/tests/utils/Common_test.py` & `iqrfpy-0.1.7/tests/utils/Common_test.py`

 * *Files identical despite different names*

