# Comparing `tmp/RobertCommonDriver-0.1.37.tar.gz` & `tmp/RobertCommonDriver-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonDriver-0.1.37.tar", last modified: Mon Apr 17 08:33:04 2023, max compression
+gzip compressed data, was "RobertCommonDriver-0.1.38.tar", last modified: Mon Apr 17 09:35:37 2023, max compression
```

## Comparing `RobertCommonDriver-0.1.37.tar` & `RobertCommonDriver-0.1.38.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.870225 RobertCommonDriver-0.1.37/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.37/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.37/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2023-04-17 08:33:04.869225 RobertCommonDriver-0.1.37/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.37/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.807397 RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/
--rw-rw-rw-   0        0        0     1744 2023-04-17 08:33:04.000000 RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2802 2023-04-17 08:33:04.000000 RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 08:33:04.000000 RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-04-17 08:33:04.000000 RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-17 08:33:04.000000 RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      199 2023-04-14 13:23:29.000000 RobertCommonDriver-0.1.37/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.808396 RobertCommonDriver-0.1.37/robertcommondriver/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.37/robertcommondriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.809395 RobertCommonDriver-0.1.37/robertcommondriver/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.822557 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/__init__.py
--rw-rw-rw-   0        0        0    87343 2023-03-23 08:25:35.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/bacnet.py
--rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/bacnetc.py
--rw-rw-rw-   0        0        0     4980 2022-12-01 08:57:24.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/base.py
--rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/iec104.py
--rw-rw-rw-   0        0        0    38296 2022-12-01 08:59:47.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/modbus.py
--rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/obix.py
--rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/opcda.py
--rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/opcda_openopc.py
--rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/opcua.py
--rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/plcs7.py
--rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/driver/snmp.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.839704 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/__init__.py
--rw-rw-rw-   0        0        0    62666 2023-04-12 09:12:47.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/base.py
--rw-rw-rw-   0        0        0    62735 2023-04-12 07:42:27.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_bacnet.py
--rw-rw-rw-   0        0        0   565998 2023-04-17 06:45:54.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0    46969 2023-04-14 08:33:27.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_iec104.py
--rw-rw-rw-   0        0        0    33721 2023-04-14 08:37:47.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_modbus.py
--rw-rw-rw-   0        0        0    18312 2023-04-13 03:18:43.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_obix.py
--rw-rw-rw-   0        0        0    61955 2023-04-13 08:15:39.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_opcda.py
--rw-rw-rw-   0        0        0    23955 2023-04-14 09:08:35.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_opcua.py
--rw-rw-rw-   0        0        0    43387 2023-04-13 08:35:41.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_ab.py
--rw-rw-rw-   0        0        0    51617 2023-04-13 08:22:42.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0    41508 2023-04-13 08:32:25.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_omron.py
--rw-rw-rw-   0        0        0    32748 2023-04-14 09:33:24.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_s7.py
--rw-rw-rw-   0        0        0    44632 2023-04-14 09:40:13.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_siemens.py
--rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_snmp.py
--rw-rw-rw-   0        0        0       42 2023-04-17 08:33:04.870225 RobertCommonDriver-0.1.37/setup.cfg
--rw-rw-rw-   0        0        0     3881 2023-04-17 08:32:09.000000 RobertCommonDriver-0.1.37/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.840705 RobertCommonDriver-0.1.37/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.37/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.842045 RobertCommonDriver-0.1.37/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.37/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.854051 RobertCommonDriver-0.1.37/tests/test_system/test_driver/
--rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/__init__.py
--rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnet.py
--rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnet1.py
--rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnetc.py
--rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnetv1.py
--rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_modbus.py
--rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_obix.py
--rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_opcda.py
--rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_opcua.py
--rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_plcs7.py
--rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_snmp.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:33:04.868222 RobertCommonDriver-0.1.37/tests/test_system/test_iot/
--rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/__init__.py
--rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_bacnet1.py
--rw-rw-rw-   0        0        0    22764 2023-04-13 09:16:01.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_bacnet.py
--rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_bacnet_mstp.py
--rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_iec104.py
--rw-rw-rw-   0        0        0     9711 2023-04-14 08:35:25.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_modbus.py
--rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_obix.py
--rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_opcda.py
--rw-rw-rw-   0        0        0     3646 2023-04-14 09:02:11.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_opcua.py
--rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_ab.py
--rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
--rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_omron.py
--rw-rw-rw-   0        0        0     7609 2023-04-14 09:31:32.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_s7.py
--rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_siemens.py
--rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_simenses1.py
--rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_snmp.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.648023 RobertCommonDriver-0.1.38/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonDriver-0.1.38/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonDriver-0.1.38/MANIFEST.in
+-rw-rw-rw-   0        0        0     1744 2023-04-17 09:35:37.648023 RobertCommonDriver-0.1.38/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2022-01-13 07:06:32.000000 RobertCommonDriver-0.1.38/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.584677 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/
+-rw-rw-rw-   0        0        0     1744 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2802 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-17 09:35:37.000000 RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      199 2023-04-14 13:23:29.000000 RobertCommonDriver-0.1.38/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.584677 RobertCommonDriver-0.1.38/robertcommondriver/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonDriver-0.1.38/robertcommondriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.585677 RobertCommonDriver-0.1.38/robertcommondriver/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.597677 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/__init__.py
+-rw-rw-rw-   0        0        0    87343 2023-03-23 08:25:35.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnet.py
+-rw-rw-rw-   0        0        0   495630 2023-04-11 03:08:18.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnetc.py
+-rw-rw-rw-   0        0        0     4980 2022-12-01 08:57:24.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/base.py
+-rw-rw-rw-   0        0        0        0 2021-10-25 01:55:43.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/iec104.py
+-rw-rw-rw-   0        0        0    38296 2022-12-01 08:59:47.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/modbus.py
+-rw-rw-rw-   0        0        0    14000 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/obix.py
+-rw-rw-rw-   0        0        0    60819 2023-04-03 06:02:51.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda.py
+-rw-rw-rw-   0        0        0    17013 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda_openopc.py
+-rw-rw-rw-   0        0        0    15955 2022-12-01 09:27:31.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcua.py
+-rw-rw-rw-   0        0        0    33482 2022-12-14 03:05:41.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/plcs7.py
+-rw-rw-rw-   0        0        0    16586 2022-12-14 03:07:06.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/driver/snmp.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.615893 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:27:26.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/__init__.py
+-rw-rw-rw-   0        0        0    62987 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/base.py
+-rw-rw-rw-   0        0        0    62779 2023-04-17 09:22:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet.py
+-rw-rw-rw-   0        0        0   566042 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0    46969 2023-04-14 08:33:27.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_iec104.py
+-rw-rw-rw-   0        0        0    33721 2023-04-14 08:37:47.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_modbus.py
+-rw-rw-rw-   0        0        0    18312 2023-04-13 03:18:43.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_obix.py
+-rw-rw-rw-   0        0        0    62003 2023-04-17 09:34:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcda.py
+-rw-rw-rw-   0        0        0    23955 2023-04-14 09:08:35.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcua.py
+-rw-rw-rw-   0        0        0    43387 2023-04-13 08:35:41.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_ab.py
+-rw-rw-rw-   0        0        0    51617 2023-04-13 08:22:42.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0    41508 2023-04-13 08:32:25.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_omron.py
+-rw-rw-rw-   0        0        0    32748 2023-04-14 09:33:24.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_s7.py
+-rw-rw-rw-   0        0        0    44632 2023-04-14 09:40:13.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_siemens.py
+-rw-rw-rw-   0        0        0    13003 2023-04-17 05:43:15.000000 RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_snmp.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 09:35:37.648960 RobertCommonDriver-0.1.38/setup.cfg
+-rw-rw-rw-   0        0        0     3881 2023-04-17 09:35:17.000000 RobertCommonDriver-0.1.38/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.616893 RobertCommonDriver-0.1.38/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonDriver-0.1.38/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.617892 RobertCommonDriver-0.1.38/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonDriver-0.1.38/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.628894 RobertCommonDriver-0.1.38/tests/test_system/test_driver/
+-rw-rw-rw-   0        0        0        0 2021-08-06 06:51:11.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/__init__.py
+-rw-rw-rw-   0        0        0     6948 2022-06-08 07:19:27.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet.py
+-rw-rw-rw-   0        0        0     2038 2022-04-14 03:52:19.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet1.py
+-rw-rw-rw-   0        0        0     3839 2022-08-02 01:50:14.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetc.py
+-rw-rw-rw-   0        0        0     7865 2022-06-14 02:23:23.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetv1.py
+-rw-rw-rw-   0        0        0     2008 2022-01-13 07:23:11.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_modbus.py
+-rw-rw-rw-   0        0        0     9784 2022-07-21 02:42:09.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_obix.py
+-rw-rw-rw-   0        0        0     5912 2022-07-07 09:34:12.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcda.py
+-rw-rw-rw-   0        0        0     1686 2022-07-13 03:25:06.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcua.py
+-rw-rw-rw-   0        0        0     2443 2022-08-12 05:55:46.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_plcs7.py
+-rw-rw-rw-   0        0        0     1444 2022-07-12 05:58:47.000000 RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_snmp.py
+drwxrwxrwx   0        0        0        0 2023-04-17 09:35:37.646964 RobertCommonDriver-0.1.38/tests/test_system/test_iot/
+-rw-rw-rw-   0        0        0        0 2022-06-15 07:28:45.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/__init__.py
+-rw-rw-rw-   0        0        0     3227 2022-06-20 07:43:32.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_bacnet1.py
+-rw-rw-rw-   0        0        0    22764 2023-04-13 09:16:01.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet.py
+-rw-rw-rw-   0        0        0    20074 2023-04-17 06:34:20.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet_mstp.py
+-rw-rw-rw-   0        0        0     1283 2023-04-14 08:30:44.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_iec104.py
+-rw-rw-rw-   0        0        0     9711 2023-04-14 08:35:25.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_modbus.py
+-rw-rw-rw-   0        0        0     4714 2023-04-13 03:12:39.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_obix.py
+-rw-rw-rw-   0        0        0     2288 2023-04-13 02:01:19.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcda.py
+-rw-rw-rw-   0        0        0     3646 2023-04-14 09:02:11.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcua.py
+-rw-rw-rw-   0        0        0     1374 2023-04-14 09:46:49.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_ab.py
+-rw-rw-rw-   0        0        0     2510 2023-04-14 09:44:42.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_mitsubishi.py
+-rw-rw-rw-   0        0        0     2836 2023-04-14 09:45:55.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_omron.py
+-rw-rw-rw-   0        0        0     7609 2023-04-14 09:31:32.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_s7.py
+-rw-rw-rw-   0        0        0     4154 2023-04-14 09:43:43.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_siemens.py
+-rw-rw-rw-   0        0        0      350 2022-08-16 09:35:34.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_simenses1.py
+-rw-rw-rw-   0        0        0     2292 2023-04-17 05:38:28.000000 RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_snmp.py
```

### Comparing `RobertCommonDriver-0.1.37/LICENSE` & `RobertCommonDriver-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/PKG-INFO` & `RobertCommonDriver-0.1.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.37
+Version: 0.1.38
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.37/README.md` & `RobertCommonDriver-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/PKG-INFO` & `RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonDriver
-Version: 0.1.37
+Version: 0.1.38
 Summary: Robert Common Driver Library
 Home-page: https://github.com/hun0423/RobertCommonDriver
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonDriver-0.1.37/RobertCommonDriver.egg-info/SOURCES.txt` & `RobertCommonDriver-0.1.38/RobertCommonDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/bacnet.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/bacnetc.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/base.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/base.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/modbus.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/obix.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/opcda.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/opcda_openopc.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcda_openopc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/opcua.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/plcs7.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/driver/snmp.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/driver/snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/base.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1391,14 +1391,19 @@
         if 'call_logging' in kwargs.keys():
             self.callbacks['call_logging'] = kwargs.get('call_logging')
 
         if 'content' in kwargs.keys():
             call_logging = self.callbacks.get('call_logging')
             if call_logging:
                 call_logging(content=kwargs.get('content'))
+            else:
+                error = kwargs.get('level')
+                if error == 'ERROR':
+                    logging.error(kwargs.get('content'))
+                    # logging.error(f"[{kwargs.get('pos')}]: {kwargs.get('content')}")
             self.save_log(kwargs.get('content'))
 
     def simulate(self, **kwargs):
         raise NotImplementedError()
 
     def info(self, **kwargs) -> dict:
         return self.infos
@@ -1444,20 +1449,21 @@
         point = {}
         templates = self.template(0, 'point', 'en')
         for template in templates:
             point[template.get('code')] = template.get('default')
         point.update(**kwargs)
         return point
 
+    @property
     def stack_pos(self):
-        return f"{stack()[1][3]}({stack()[1][2]})"
+        return f"{IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]})"
 
     def add_stack(self, content: Optional[str] = None):
         """添加程序位置"""
-        self.debug_pos = f"{IOTBaseCommon.get_datetime_str()}: {stack()[1][3]}({stack()[1][2]}){'' if content is None else content}"
+        self.debug_pos = f"{IOTBaseCommon.get_datetime_str()}: {IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]}){'' if content is None else content}"
 
     def debug(self):
         return self.debug_pos
 
     def update_device(self, device_address: Optional[str], address: Optional[Any], **kwargs):
         if device_address not in self.devices.keys():
             self.devices[device_address] = {}
```

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_bacnet.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,16 +936,17 @@
                 self.logging(content=f"refresh object({object.get('point_type')} {object.get('point_address')}) fail({e.__str__()})", level='ERROR', pos=self.stack_pos)
 
     def logging(self, **kwargs):
         if self.parent:
             if hasattr(self.parent, 'logging'):
                 self.parent.logging(**kwargs)
 
+    @property
     def stack_pos(self):
-        return f"{stack()[1][3]}({stack()[1][2]})"
+        return f"{IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]})"
 
 
 class IOTBacnet(IOTDriver):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.reinit()
```

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_bacnet_mstp.py`

 * *Files 0% similar despite different names*

```diff
@@ -11655,16 +11655,17 @@
         self.reset()
 
     def logging(self, **kwargs):
         if self.parent:
             if hasattr(self.parent, 'logging'):
                 self.parent.logging(**kwargs)
 
+    @property
     def stack_pos(self):
-        return f"{stack()[1][3]}({stack()[1][2]})"
+        return f"{IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]})"
 
     def callback_whois(self, sender: BACnetClient, adr: BACnetAddress, low_limit: int, high_limit: int):
         if low_limit != -1 and self.default_id < low_limit:
             return
         elif high_limit != -1 and self.default_id > high_limit:
             return
         sender.Iam(self.default_id, BACnetDefine.BACnetSegmentations.SEGMENTATION_BOTH, 61440)
```

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_iec104.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_modbus.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_obix.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_opcda.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,16 +159,17 @@
 
         def disconnect(self):
             self._update_info(used=time.time(), connected=self.opc_connected)
             self.logging(content=f"disconnect", pos=self.stack_pos)
             if self.opc_client is not None:
                 self.opc_client.Disconnect()
 
+        @property
         def stack_pos(self):
-            return f"{stack()[1][3]}({stack()[1][2]})"
+            return f"{IOTBaseCommon.get_file_name(stack()[1][1])}({stack()[1][2]})"
 
         def close(self, del_object: bool = True):
             self._update_info(used=time.time())
             self.logging(content=f"close({del_object})", pos=self.stack_pos)
 
             opc_connected = self.opc_connected
             try:
```

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_opcua.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_ab.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_omron.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_s7.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_plc_siemens.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/robertcommondriver/system/iot/iot_snmp.py` & `RobertCommonDriver-0.1.38/robertcommondriver/system/iot/iot_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/setup.py` & `RobertCommonDriver-0.1.38/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'RobertCommonDriver'
 DESCRIPTION = 'Robert Common Driver Library'
 URL = 'https://github.com/hun0423/RobertCommonDriver'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.37'
+VERSION = '0.1.38'
 DATE = '2023-04-17'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnet.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnet1.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnetc.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetc.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_bacnetv1.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_bacnetv1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_modbus.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_obix.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_opcda.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_opcua.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_plcs7.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_plcs7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_driver/test_snmp.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_driver/test_snmp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_bacnet1.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_bacnet1.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_bacnet.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_bacnet_mstp.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_bacnet_mstp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_iec104.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_iec104.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_modbus.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_modbus.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_obix.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_obix.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_opcda.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcda.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_opcua.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_opcua.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_ab.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_ab.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_mitsubishi.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_mitsubishi.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_omron.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_omron.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_s7.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_s7.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_plc_siemens.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_plc_siemens.py`

 * *Files identical despite different names*

### Comparing `RobertCommonDriver-0.1.37/tests/test_system/test_iot/test_iot_snmp.py` & `RobertCommonDriver-0.1.38/tests/test_system/test_iot/test_iot_snmp.py`

 * *Files identical despite different names*

