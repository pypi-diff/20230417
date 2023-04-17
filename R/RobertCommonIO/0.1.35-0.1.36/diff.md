# Comparing `tmp/RobertCommonIO-0.1.35.tar.gz` & `tmp/RobertCommonIO-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonIO-0.1.35.tar", last modified: Thu Mar 23 06:57:00 2023, max compression
+gzip compressed data, was "RobertCommonIO-0.1.36.tar", last modified: Mon Apr 17 08:31:00 2023, max compression
```

## Comparing `RobertCommonIO-0.1.35.tar` & `RobertCommonIO-0.1.36.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.515713 RobertCommonIO-0.1.35/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.35/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.35/MANIFEST.in
--rw-rw-rw-   0        0        0     1724 2023-03-23 06:57:00.515713 RobertCommonIO-0.1.35/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2022-01-13 06:37:11.000000 RobertCommonIO-0.1.35/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.479749 RobertCommonIO-0.1.35/RobertCommonIO.egg-info/
--rw-rw-rw-   0        0        0     1724 2023-03-23 06:57:00.000000 RobertCommonIO-0.1.35/RobertCommonIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2023-03-23 06:57:00.000000 RobertCommonIO-0.1.35/RobertCommonIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 06:57:00.000000 RobertCommonIO-0.1.35/RobertCommonIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2023-03-23 06:57:00.000000 RobertCommonIO-0.1.35/RobertCommonIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-23 06:57:00.000000 RobertCommonIO-0.1.35/RobertCommonIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      302 2023-03-23 06:49:55.000000 RobertCommonIO-0.1.35/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.483049 RobertCommonIO-0.1.35/robertcommonio/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.35/robertcommonio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.483049 RobertCommonIO-0.1.35/robertcommonio/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.35/robertcommonio/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.500223 RobertCommonIO-0.1.35/robertcommonio/system/io/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/__init__.py
--rw-rw-rw-   0        0        0    18829 2023-03-14 09:51:31.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/data_storage.py
--rw-rw-rw-   0        0        0     1051 2022-11-22 07:37:12.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/email.py
--rw-rw-rw-   0        0        0     7390 2023-01-11 07:38:01.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/file.py
--rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/ftp.py
--rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/http.py
--rw-rw-rw-   0        0        0     3334 2023-01-31 09:43:08.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/ini.py
--rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/license.py
--rw-rw-rw-   0        0        0    25643 2023-01-04 09:57:01.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/mongo.py
--rw-rw-rw-   0        0        0     6883 2023-03-23 06:56:31.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/mqtt.py
--rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/mysql.py
--rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/oss.py
--rw-rw-rw-   0        0        0     7191 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/rabitmq.py
--rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/redis.py
--rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/redis_cache.py
--rw-rw-rw-   0        0        0     7286 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/response.py
--rw-rw-rw-   0        0        0    37639 2023-02-23 08:23:07.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/socket.py
--rw-rw-rw-   0        0        0     7211 2023-01-19 14:33:43.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/sqlalche.py
--rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/transport.py
--rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.35/robertcommonio/system/io/version.py
--rw-rw-rw-   0        0        0       42 2023-03-23 06:57:00.515713 RobertCommonIO-0.1.35/setup.cfg
--rw-rw-rw-   0        0        0     3869 2023-03-16 09:05:39.000000 RobertCommonIO-0.1.35/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.501707 RobertCommonIO-0.1.35/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.35/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.501707 RobertCommonIO-0.1.35/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.35/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-23 06:57:00.514380 RobertCommonIO-0.1.35/tests/test_system/test_io/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test.py
--rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_data_storage.py
--rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_file.py
--rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_ftp.py
--rw-rw-rw-   0        0        0      399 2022-12-14 07:23:38.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_http.py
--rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_ini.py
--rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_license.py
--rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_mqtt.py
--rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_oracle.py
--rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_rabbitmq.py
--rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_socket.py
--rw-rw-rw-   0        0        0     3153 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_sqlalche.py
--rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.35/tests/test_system/test_io/test_transport.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.073378 RobertCommonIO-0.1.36/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.36/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.36/MANIFEST.in
+-rw-rw-rw-   0        0        0     1724 2023-04-17 08:31:00.073378 RobertCommonIO-0.1.36/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2022-01-13 06:37:11.000000 RobertCommonIO-0.1.36/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.025275 RobertCommonIO-0.1.36/RobertCommonIO.egg-info/
+-rw-rw-rw-   0        0        0     1724 2023-04-17 08:30:59.000000 RobertCommonIO-0.1.36/RobertCommonIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-04-17 08:30:59.000000 RobertCommonIO-0.1.36/RobertCommonIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 08:30:59.000000 RobertCommonIO-0.1.36/RobertCommonIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      269 2023-04-17 08:30:59.000000 RobertCommonIO-0.1.36/RobertCommonIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-17 08:30:59.000000 RobertCommonIO-0.1.36/RobertCommonIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      295 2023-04-17 08:30:55.000000 RobertCommonIO-0.1.36/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.026274 RobertCommonIO-0.1.36/robertcommonio/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.36/robertcommonio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.027279 RobertCommonIO-0.1.36/robertcommonio/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.36/robertcommonio/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.052194 RobertCommonIO-0.1.36/robertcommonio/system/io/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/__init__.py
+-rw-rw-rw-   0        0        0    19281 2023-04-04 06:29:48.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/data_storage.py
+-rw-rw-rw-   0        0        0     1051 2022-11-22 07:37:12.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/email.py
+-rw-rw-rw-   0        0        0     7390 2023-01-11 07:38:01.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/file.py
+-rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/ftp.py
+-rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/http.py
+-rw-rw-rw-   0        0        0     3334 2023-01-31 09:43:08.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/ini.py
+-rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/license.py
+-rw-rw-rw-   0        0        0    26671 2023-04-04 06:38:40.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/mongo.py
+-rw-rw-rw-   0        0        0     6883 2023-03-23 06:56:31.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/mqtt.py
+-rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/mysql.py
+-rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/oss.py
+-rw-rw-rw-   0        0        0     7191 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/rabitmq.py
+-rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/redis.py
+-rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/redis_cache.py
+-rw-rw-rw-   0        0        0     7286 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/response.py
+-rw-rw-rw-   0        0        0    37639 2023-02-23 08:23:07.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/socket.py
+-rw-rw-rw-   0        0        0     7211 2023-01-19 14:33:43.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/sqlalche.py
+-rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/transport.py
+-rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.36/robertcommonio/system/io/version.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 08:31:00.073378 RobertCommonIO-0.1.36/setup.cfg
+-rw-rw-rw-   0        0        0     3869 2023-04-17 08:28:21.000000 RobertCommonIO-0.1.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.053195 RobertCommonIO-0.1.36/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.36/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.053195 RobertCommonIO-0.1.36/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.36/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 08:31:00.072255 RobertCommonIO-0.1.36/tests/test_system/test_io/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test.py
+-rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_data_storage.py
+-rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_file.py
+-rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_ftp.py
+-rw-rw-rw-   0        0        0      399 2022-12-14 07:23:38.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_http.py
+-rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_ini.py
+-rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_license.py
+-rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_mongo.py
+-rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_mqtt.py
+-rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_oracle.py
+-rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_rabbitmq.py
+-rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_socket.py
+-rw-rw-rw-   0        0        0     3153 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_sqlalche.py
+-rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.36/tests/test_system/test_io/test_transport.py
```

### Comparing `RobertCommonIO-0.1.35/LICENSE` & `RobertCommonIO-0.1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/PKG-INFO` & `RobertCommonIO-0.1.36/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.35
+Version: 0.1.36
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.35/README.md` & `RobertCommonIO-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/RobertCommonIO.egg-info/PKG-INFO` & `RobertCommonIO-0.1.36/RobertCommonIO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.35
+Version: 0.1.36
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.35/RobertCommonIO.egg-info/SOURCES.txt` & `RobertCommonIO-0.1.36/RobertCommonIO.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,13 +36,14 @@
 tests/test_system/test_io/test.py
 tests/test_system/test_io/test_data_storage.py
 tests/test_system/test_io/test_file.py
 tests/test_system/test_io/test_ftp.py
 tests/test_system/test_io/test_http.py
 tests/test_system/test_io/test_ini.py
 tests/test_system/test_io/test_license.py
+tests/test_system/test_io/test_mongo.py
 tests/test_system/test_io/test_mqtt.py
 tests/test_system/test_io/test_oracle.py
 tests/test_system/test_io/test_rabbitmq.py
 tests/test_system/test_io/test_socket.py
 tests/test_system/test_io/test_sqlalche.py
 tests/test_system/test_io/test_transport.py
```

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/data_storage.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/data_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,18 +148,18 @@
         if ds_ref.ref_type == DsRefType.FILES:
             return f"{starter}{ds_ref.files_id}|{ds_ref.ds_name}"
         else:
             return f"{starter}{ds_ref.proj_id}|{ds_ref.ds_name}"
 
     @classmethod
     def parse_as_groups(cls, ds_item_ids: List[str]) -> Dict[Union[int, ObjectId], List[str]]:
-        result: Dict[Union[int, ObjectId], List[str]] = {}
+        result: Dict[Union[str, int, ObjectId], List[str]] = {}
         for ds_item_id in cls.parse_as_list(ds_item_ids):
             ds_repo_id = str(ds_item_id.ds_repo_id)
-            if ds_repo_id in result:
+            if ds_repo_id in result.keys():
                 result[ds_repo_id].append(ds_item_id.his_point_name)
             else:
                 result[ds_repo_id] = [ds_item_id.his_point_name]
         return result
 
 
 class DataEngineBase(object):
@@ -167,21 +167,21 @@
     def __init__(self,  accessor: Any, proj_id: str, point_names: List[str] = None, date_range: Optional[DateRange] = None):
         self.accessor = accessor
         self.proj_id = proj_id
         self.point_names = point_names
         self.date_range = date_range
 
     def get_history_tb(self) -> str:
-        return f"history_{self.proj_id}"
+        return f"proj_history_{self.proj_id}"
 
     def get_real_tb(self) -> str:
-        return f"rtdata_{self.proj_id}"
+        return f"proj_rtdata_{self.proj_id}"
 
     def get_log_tb(self) -> str:
-        return f"log_{self.proj_id}"
+        return f"proj_log_{self.proj_id}"
 
     def load_history_data(self) -> pd.DataFrame:
         result = pd.DataFrame()
         if isinstance(self.accessor, MongoAccessor):
             query_match = {'time': MongoFunc.get_time_query_match(self.date_range.start_time, self.date_range.end_time, self.date_range.interval.value)}
             if self.point_names:
                 query_match.update({'name': {'$in': self.point_names}})
@@ -207,14 +207,21 @@
             data_df.reset_index(inplace=True)
             data: pd.Series = data_df.apply(lambda record: MongoFunc.convert_point_df(record), axis=1)
             self.accessor.mdbBb[self.get_history_tb()].bulk_write(data.to_list())
             self.accessor.mdbBb[self.get_history_tb()].create_index([('time', ASCENDING), ('name', ASCENDING)], unique=True)
             return True
         return False
 
+    def del_history_data(self):
+        if isinstance(self.accessor, MongoAccessor):
+            query_match = {'time': MongoFunc.get_time_query_match(self.date_range.start_time, self.date_range.end_time, self.date_range.interval.value)}
+            if self.point_names:
+                query_match.update({'name': {'$in': self.point_names}})
+            self.accessor.delete_many(self.get_history_tb(), query_match)
+
     def load_real_data(self) -> pd.DataFrame:
         df = pd.DataFrame()
         if isinstance(self.accessor, MySqlAccessor):
             sql = f"""SELECT time, name, value FROM {self.get_real_tb()} {f'''WHERE name in ('{"','".join(self.point_names)}')''' if self.point_names is not None and len(self.point_names) > 0 else ""}"""
             df = pd.read_sql(sql, con=self.accessor.get_conn(), index_col='name', coerce_float=True)
             if not df.empty:
                 df['time'] = df['time'].apply(lambda time: datetime.strftime(time, '%Y-%m-%d %H:%M:%S'))
```

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/email.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/email.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/file.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/ftp.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/http.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/http.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/ini.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/license.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/mongo.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/mongo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
+import pytz
 import numpy as np
 import pandas as pd
 from bson.objectid import ObjectId
+from bson.codec_options import CodecOptions
 from datetime import datetime
 from typing import NamedTuple, Optional, Iterator, List, Union, Any, Tuple
 import math
 
 from pymongo import MongoClient, ASCENDING
 from pymongo.read_concern import ReadConcern
 from pymongo.write_concern import WriteConcern
@@ -28,14 +30,16 @@
     PORT: int
     USER: Optional[str]
     PWD: Optional[str]
     DB_NAME: Optional[str]
     REPLICA_SET: Optional[str]
     READ_PREFERENCE: Optional[str]
     READ_PREFERENCE_TAGS: Optional[str] = None
+    TZ_AWARE: Optional[bool] = None
+    TZ_INFO: Optional[str] = None
 
 
 class MongoAccessor:
 
     def __init__(self, config: MongoConfig):
         config = input.ensure_not_none_of('config', config, MongoConfig)
         self._config = config._replace(
@@ -43,14 +47,16 @@
             PORT=input.ensure_int('PORT', config.PORT) or 27017,
             DB_NAME=input.ensure_str('DB_NAME', config.DB_NAME) or 'beopdata',
             USER=input.ensure_not_none_str('USER', config.USER),
             PWD=input.ensure_not_none_str('PWD', config.PWD),
             REPLICA_SET=input.ensure_str('REPLICA_SET', config.REPLICA_SET) or None,
             READ_PREFERENCE=input.ensure_str('READ_PREFERENCE', config.READ_PREFERENCE) or None,
             READ_PREFERENCE_TAGS=input.ensure_str('READ_PREFERENCE_TAGS', config.READ_PREFERENCE_TAGS) or None,
+            TZ_AWARE=input.ensure_bool('TZ_AWARE', config.TZ_AWARE) or None,
+            TZ_INFO=input.ensure_str('TZ_INFO', config.TZ_INFO) or None,
         )
         self._safe_log_config = self._config._replace(PWD='*')
         self._conn = None
 
     def __str__(self):
         return f"[{self._config.HOST}:{self._config.PORT}]"
 
@@ -84,32 +90,34 @@
                     password=self._config.PWD,
                     maxPoolSize=300,
                     maxIdleTimeMS=60000,
                     serverSelectionTimeoutMS=120000,
                     waitQueueTimeoutMS=20000,
                     socketTimeoutMS=60000,
                     ssl=False,
-                    authSource=self._config.DB_NAME
+                    authSource=self._config.DB_NAME,
                 )
+                if self._config.TZ_AWARE is not None:
+                    args.update(tz_aware=self._config.TZ_AWARE, tzinfo=None if self._config.TZ_INFO is None else pytz.timezone(self._config.TZ_INFO))
                 if self._config.REPLICA_SET is not None and self._config.READ_PREFERENCE is not None:
                     args.update(dict(replicaset=self._config.REPLICA_SET, readPreference=self._config.READ_PREFERENCE, readPreferenceTags=self._config.READ_PREFERENCE_TAGS or ''))
                 self._conn = MongoClient(host=self._config.HOST, port=self._config.PORT, **args)
                 logging.info(f"Successfully connected to {self._safe_log_config}!")
             except Exception as e:
                 raise ConnectionRefusedError(f'Failed to connect to {self._safe_log_config}!')
         return self._conn
 
-    def _get_coll(self, coll_name: str):
-        return self.mdbBb.get_collection(coll_name)
+    def _get_coll(self, coll_name: str, tz_info: Optional[str] = None):
+        return self.mdbBb.get_collection(coll_name) if tz_info is None else self.mdbBb.get_collection(coll_name).with_options(codec_options=CodecOptions(tz_aware=True, tzinfo=pytz.timezone(tz_info)))
 
     def get_coll_names(self, include_system_collections: bool = True) -> List[str]:
         return self.mdbBb.collection_names(include_system_collections)
 
-    def find(self, coll_name: str, query: dict, projection: Optional[dict] = None, skip: Optional[int] = None, limit: Optional[int] = None, sort: Optional[List[Tuple[str, int]]] = None, session: Optional[ClientSession] = None) -> Iterator[dict]:
-        coll = self._get_coll(coll_name)
+    def find(self, coll_name: str, query: dict, projection: Optional[dict] = None, skip: Optional[int] = None, limit: Optional[int] = None, sort: Optional[List[Tuple[str, int]]] = None, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> Iterator[dict]:
+        coll = self._get_coll(coll_name, tz_info)
         kwargs = {}
         if projection:
             kwargs['projection'] = projection
         if skip:
             kwargs['skip'] = skip
         if limit:
             kwargs['limit'] = limit
@@ -117,55 +125,55 @@
             kwargs['sort'] = sort
         if session:
             kwargs['session'] = session
         with coll.find(filter=query, **kwargs) as cursor:
             for doc in cursor:
                 yield doc
 
-    def aggr(self, coll_name: str, pipeline: List, allow_disk_use: bool = False, session: Optional[ClientSession] = None) -> Iterator[dict]:
-        coll = self._get_coll(coll_name)
+    def aggr(self, coll_name: str, pipeline: List, allow_disk_use: bool = False, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> Iterator[dict]:
+        coll = self._get_coll(coll_name, tz_info)
         with coll.aggregate(pipeline, allowDiskUse=allow_disk_use, session=session) as cursor:
             for doc in cursor:
                 yield doc
 
-    def insert_many(self, coll_name: str, docs: List[dict], session: Optional[ClientSession] = None) -> InsertManyResult:
-        coll = self._get_coll(coll_name)
+    def insert_many(self, coll_name: str, docs: List[dict], session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> InsertManyResult:
+        coll = self._get_coll(coll_name, tz_info)
         result = coll.insert_many(docs, session=session)
         return result
 
-    def update_many(self, coll_name: str, query: dict, update: dict, upsert: bool = False, session: Optional[ClientSession] = None) -> UpdateResult:
-        coll = self._get_coll(coll_name)
+    def update_many(self, coll_name: str, query: dict, update: dict, upsert: bool = False, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> UpdateResult:
+        coll = self._get_coll(coll_name, tz_info)
         result = coll.update_many(query, update, upsert, session=session)
         return result
 
-    def delete_many(self, coll_name: str, query: dict, session: Optional[ClientSession] = None) -> DeleteResult:
-        coll = self._get_coll(coll_name)
+    def delete_many(self, coll_name: str, query: dict, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> DeleteResult:
+        coll = self._get_coll(coll_name, tz_info)
         result = coll.delete_many(query, session=session)
         return result
 
     def start_session(self):
         return self.conn.start_session()
 
     def start_session_transaction(self, read_concern: Optional[ReadConcern] = None, write_concern: Optional[WriteConcern] = None, read_preference: Optional[RP] = RP.PRIMARY) -> 'MongoSessionContext':
         return MongoSessionContext(self, read_concern, write_concern, read_preference)
 
-    def bulk_write(self, coll_name: str, ops: List[MongoWriteOp], ordered: bool = True, session: Optional[ClientSession] = None) -> BulkWriteResult:
-        coll = self._get_coll(coll_name)
+    def bulk_write(self, coll_name: str, ops: List[MongoWriteOp], ordered: bool = True, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> BulkWriteResult:
+        coll = self._get_coll(coll_name, tz_info)
         return coll.bulk_write(ops, ordered, session=session)
 
-    def create_index(self, coll_name: str, keys, session: Optional[ClientSession] = None, **kwargs):
-        coll = self._get_coll(coll_name)
+    def create_index(self, coll_name: str, keys, session: Optional[ClientSession] = None, tz_info: Optional[str] = None, **kwargs):
+        coll = self._get_coll(coll_name, tz_info)
         return coll.create_index(keys, session=session, **kwargs)
 
-    def drop_coll(self, coll_name: str, session: ClientSession = None):
-        coll = self._get_coll(coll_name)
+    def drop_coll(self, coll_name: str, session: ClientSession = None, tz_info: Optional[str] = None):
+        coll = self._get_coll(coll_name, tz_info)
         coll.drop(session=session)
 
-    def distinct(self, coll_name: str, key: str, query: Optional[dict] = None, session: Optional[ClientSession] = None) -> Any:
-        coll = self._get_coll(coll_name)
+    def distinct(self, coll_name: str, key: str, query: Optional[dict] = None, session: Optional[ClientSession] = None, tz_info: Optional[str] = None) -> Any:
+        coll = self._get_coll(coll_name, tz_info)
         rv = coll.distinct(key=key, filter=query, session=session)
         return rv
 
 
 class MongoTransactionalSession:
 
     def __init__(self, accessor: MongoAccessor, read_concern: Optional[ReadConcern] = None, write_concern: Optional[WriteConcern] = None, read_preference: Optional[RP] = RP.PRIMARY):
```

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/mqtt.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/mysql.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/mysql.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/oss.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/oss.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/rabitmq.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/rabitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/redis.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/redis.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/redis_cache.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/redis_cache.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/response.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/response.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/socket.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/sqlalche.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/sqlalche.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/transport.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/transport.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/robertcommonio/system/io/version.py` & `RobertCommonIO-0.1.36/robertcommonio/system/io/version.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/setup.py` & `RobertCommonIO-0.1.36/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonIO'
 DESCRIPTION = 'Robert Common IO Library'
 URL = 'https://github.com/hun0423/RobertCommonIO'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.35'
-DATE = '2023-03-16'
+VERSION = '0.1.36'
+DATE = '2023-04-17'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_data_storage.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_file.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_ftp.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_license.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_mqtt.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_oracle.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_oracle.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_rabbitmq.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_socket.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_sqlalche.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_sqlalche.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.35/tests/test_system/test_io/test_transport.py` & `RobertCommonIO-0.1.36/tests/test_system/test_io/test_transport.py`

 * *Files identical despite different names*

