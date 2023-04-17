# Comparing `tmp/tonplay-sdk-0.0.6.tar.gz` & `tmp/tonplay-sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonplay-sdk-0.0.6.tar", last modified: Wed Apr 12 15:24:51 2023, max compression
+gzip compressed data, was "tonplay-sdk-0.0.7.tar", last modified: Mon Apr 17 07:34:10 2023, max compression
```

## Comparing `tonplay-sdk-0.0.6.tar` & `tonplay-sdk-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.066251 tonplay-sdk-0.0.6/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1067 2023-04-04 16:07:16.000000 tonplay-sdk-0.0.6/LICENSE.md
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       31 2023-04-04 17:12:11.000000 tonplay-sdk-0.0.6/MANIFEST.in
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1205 2023-04-12 15:24:51.066354 tonplay-sdk-0.0.6/PKG-INFO
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      884 2023-04-10 04:04:10.000000 tonplay-sdk-0.0.6/README.md
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.059259 tonplay-sdk-0.0.6/examples/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:15:02.000000 tonplay-sdk-0.0.6/examples/__init__.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.061280 tonplay-sdk-0.0.6/examples/api/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:39:44.000000 tonplay-sdk-0.0.6/examples/api/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      215 2023-04-05 11:27:56.000000 tonplay-sdk-0.0.6/examples/api/asset.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1830 2023-04-06 04:59:01.000000 tonplay-sdk-0.0.6/examples/api/asset_deploy.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      966 2023-04-05 11:28:42.000000 tonplay-sdk-0.0.6/examples/api/auth.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      238 2023-04-07 13:37:32.000000 tonplay-sdk-0.0.6/examples/api/game.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1167 2023-04-06 05:40:30.000000 tonplay-sdk-0.0.6/examples/api/market.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      841 2023-04-06 04:49:44.000000 tonplay-sdk-0.0.6/examples/api/ton.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      387 2023-04-06 04:05:39.000000 tonplay-sdk-0.0.6/examples/api/user.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.061587 tonplay-sdk-0.0.6/requirements/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-04 16:16:05.000000 tonplay-sdk-0.0.6/requirements/common.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      106 2023-04-12 15:24:51.066640 tonplay-sdk-0.0.6/setup.cfg
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1059 2023-04-06 05:35:46.000000 tonplay-sdk-0.0.6/setup.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.061715 tonplay-sdk-0.0.6/tests/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       76 2023-04-06 05:04:17.000000 tonplay-sdk-0.0.6/tests/test_api.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.062450 tonplay-sdk-0.0.6/tonplay/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 07:17:37.000000 tonplay-sdk-0.0.6/tonplay/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       22 2023-04-12 15:24:32.000000 tonplay-sdk-0.0.6/tonplay/__version__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3268 2023-04-05 12:24:06.000000 tonplay-sdk-0.0.6/tonplay/api.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1473 2023-04-03 13:03:23.000000 tonplay-sdk-0.0.6/tonplay/error.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.063105 tonplay-sdk-0.0.6/tonplay/lib/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 08:07:09.000000 tonplay-sdk-0.0.6/tonplay/lib/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       87 2023-04-04 08:08:15.000000 tonplay-sdk-0.0.6/tonplay/lib/enums.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1273 2023-04-06 04:17:04.000000 tonplay-sdk-0.0.6/tonplay/lib/utils.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.065243 tonplay-sdk-0.0.6/tonplay/methods/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1391 2023-04-07 13:29:36.000000 tonplay-sdk-0.0.6/tonplay/methods/__init__.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      293 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.6/tonplay/methods/_asset.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      260 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.6/tonplay/methods/_auth.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1044 2023-04-07 13:37:15.000000 tonplay-sdk-0.0.6/tonplay/methods/_game.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3026 2023-04-05 11:59:01.000000 tonplay-sdk-0.0.6/tonplay/methods/_market.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     6376 2023-04-12 15:23:46.000000 tonplay-sdk-0.0.6/tonplay/methods/_ton.py
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      628 2023-04-05 12:26:07.000000 tonplay-sdk-0.0.6/tonplay/methods/_user.py
-drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-12 15:24:51.066141 tonplay-sdk-0.0.6/tonplay_sdk.egg-info/
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1205 2023-04-12 15:24:51.000000 tonplay-sdk-0.0.6/tonplay_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      791 2023-04-12 15:24:51.000000 tonplay-sdk-0.0.6/tonplay_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        1 2023-04-12 15:24:51.000000 tonplay-sdk-0.0.6/tonplay_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-12 15:24:51.000000 tonplay-sdk-0.0.6/tonplay_sdk.egg-info/requires.txt
--rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-12 15:24:51.000000 tonplay-sdk-0.0.6/tonplay_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.911307 tonplay-sdk-0.0.7/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1068 2023-04-17 07:25:48.000000 tonplay-sdk-0.0.7/LICENSE.md
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       31 2023-04-04 17:12:11.000000 tonplay-sdk-0.0.7/MANIFEST.in
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1202 2023-04-17 07:34:10.911394 tonplay-sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      881 2023-04-17 07:33:41.000000 tonplay-sdk-0.0.7/README.md
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.904435 tonplay-sdk-0.0.7/examples/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:15:02.000000 tonplay-sdk-0.0.7/examples/__init__.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.906629 tonplay-sdk-0.0.7/examples/api/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-05 11:39:44.000000 tonplay-sdk-0.0.7/examples/api/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      215 2023-04-05 11:27:56.000000 tonplay-sdk-0.0.7/examples/api/asset.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1830 2023-04-06 04:59:01.000000 tonplay-sdk-0.0.7/examples/api/asset_deploy.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      966 2023-04-05 11:28:42.000000 tonplay-sdk-0.0.7/examples/api/auth.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      238 2023-04-07 13:37:32.000000 tonplay-sdk-0.0.7/examples/api/game.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1167 2023-04-06 05:40:30.000000 tonplay-sdk-0.0.7/examples/api/market.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      841 2023-04-06 04:49:44.000000 tonplay-sdk-0.0.7/examples/api/ton.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      387 2023-04-06 04:05:39.000000 tonplay-sdk-0.0.7/examples/api/user.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.906904 tonplay-sdk-0.0.7/requirements/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-04 16:16:05.000000 tonplay-sdk-0.0.7/requirements/common.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      106 2023-04-17 07:34:10.911639 tonplay-sdk-0.0.7/setup.cfg
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1059 2023-04-06 05:35:46.000000 tonplay-sdk-0.0.7/setup.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.907037 tonplay-sdk-0.0.7/tests/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       76 2023-04-06 05:04:17.000000 tonplay-sdk-0.0.7/tests/test_api.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.907773 tonplay-sdk-0.0.7/tonplay/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 07:17:37.000000 tonplay-sdk-0.0.7/tonplay/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       22 2023-04-17 07:30:52.000000 tonplay-sdk-0.0.7/tonplay/__version__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3268 2023-04-05 12:24:06.000000 tonplay-sdk-0.0.7/tonplay/api.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1473 2023-04-03 13:03:23.000000 tonplay-sdk-0.0.7/tonplay/error.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.908434 tonplay-sdk-0.0.7/tonplay/lib/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-04 08:07:09.000000 tonplay-sdk-0.0.7/tonplay/lib/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       87 2023-04-04 08:08:15.000000 tonplay-sdk-0.0.7/tonplay/lib/enums.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1273 2023-04-06 04:17:04.000000 tonplay-sdk-0.0.7/tonplay/lib/utils.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.910372 tonplay-sdk-0.0.7/tonplay/methods/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1391 2023-04-07 13:29:36.000000 tonplay-sdk-0.0.7/tonplay/methods/__init__.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      293 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.7/tonplay/methods/_asset.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      260 2023-04-04 11:34:18.000000 tonplay-sdk-0.0.7/tonplay/methods/_auth.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1044 2023-04-07 13:37:15.000000 tonplay-sdk-0.0.7/tonplay/methods/_game.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     3026 2023-04-05 11:59:01.000000 tonplay-sdk-0.0.7/tonplay/methods/_market.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     6376 2023-04-12 15:23:46.000000 tonplay-sdk-0.0.7/tonplay/methods/_ton.py
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      628 2023-04-05 12:26:07.000000 tonplay-sdk-0.0.7/tonplay/methods/_user.py
+drwxr-xr-x   0 ellijahvashkevich   (501) staff       (20)        0 2023-04-17 07:34:10.911200 tonplay-sdk-0.0.7/tonplay_sdk.egg-info/
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)     1202 2023-04-17 07:34:10.000000 tonplay-sdk-0.0.7/tonplay_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)      791 2023-04-17 07:34:10.000000 tonplay-sdk-0.0.7/tonplay_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)        1 2023-04-17 07:34:10.000000 tonplay-sdk-0.0.7/tonplay_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-17 07:34:10.000000 tonplay-sdk-0.0.7/tonplay_sdk.egg-info/requires.txt
+-rw-r--r--   0 ellijahvashkevich   (501) staff       (20)       17 2023-04-17 07:34:10.000000 tonplay-sdk-0.0.7/tonplay_sdk.egg-info/top_level.txt
```

### Comparing `tonplay-sdk-0.0.6/LICENSE.md` & `tonplay-sdk-0.0.7/LICENSE.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [2023] [Binance]
+Copyright (c) [2023] [TON Play]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tonplay-sdk-0.0.6/PKG-INFO` & `tonplay-sdk-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: tonplay-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is a lightweight library that works as a connector to TON Play public API
 Author: TON Play
 License: MIT
 Keywords: TON Play,Ton Play API,Tonplay API,ton sdk,ton
 Requires-Python: >=3.11.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # TON Play Public API Connector Python
 
 [![PyPI version](https://img.shields.io/pypi/v/tonplay-sdk)](https://pypi.python.org/pypi/tonplay-sdk)
 
-This is a [lightweight library](https://github.com/90K2/tonplay-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
+This is a [lightweight library](https://gitlab.com/ton-play/python-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
 ## Installation
 
 ```bash
-pip install tonplay-connector
+pip install tonplay-sdk
 ```
 
 ## Get API Key
 
 To get API Key [follow the link](https://docs.tonplay.io/digital-assets-api/api-key)
 
 ## RESTful APIs
```

### Comparing `tonplay-sdk-0.0.6/README.md` & `tonplay-sdk-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # TON Play Public API Connector Python
 
 [![PyPI version](https://img.shields.io/pypi/v/tonplay-sdk)](https://pypi.python.org/pypi/tonplay-sdk)
 
-This is a [lightweight library](https://github.com/90K2/tonplay-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
+This is a [lightweight library](https://gitlab.com/ton-play/python-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
 ## Installation
 
 ```bash
-pip install tonplay-connector
+pip install tonplay-sdk
 ```
 
 ## Get API Key
 
 To get API Key [follow the link](https://docs.tonplay.io/digital-assets-api/api-key)
 
 ## RESTful APIs
```

### Comparing `tonplay-sdk-0.0.6/examples/api/asset_deploy.py` & `tonplay-sdk-0.0.7/examples/api/asset_deploy.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/examples/api/auth.py` & `tonplay-sdk-0.0.7/examples/api/auth.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/examples/api/market.py` & `tonplay-sdk-0.0.7/examples/api/market.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/examples/api/ton.py` & `tonplay-sdk-0.0.7/examples/api/ton.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/setup.py` & `tonplay-sdk-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/api.py` & `tonplay-sdk-0.0.7/tonplay/api.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/error.py` & `tonplay-sdk-0.0.7/tonplay/error.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/lib/utils.py` & `tonplay-sdk-0.0.7/tonplay/lib/utils.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/methods/__init__.py` & `tonplay-sdk-0.0.7/tonplay/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/methods/_game.py` & `tonplay-sdk-0.0.7/tonplay/methods/_game.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/methods/_market.py` & `tonplay-sdk-0.0.7/tonplay/methods/_market.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/methods/_ton.py` & `tonplay-sdk-0.0.7/tonplay/methods/_ton.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay/methods/_user.py` & `tonplay-sdk-0.0.7/tonplay/methods/_user.py`

 * *Files identical despite different names*

### Comparing `tonplay-sdk-0.0.6/tonplay_sdk.egg-info/PKG-INFO` & `tonplay-sdk-0.0.7/tonplay_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: tonplay-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is a lightweight library that works as a connector to TON Play public API
 Author: TON Play
 License: MIT
 Keywords: TON Play,Ton Play API,Tonplay API,ton sdk,ton
 Requires-Python: >=3.11.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # TON Play Public API Connector Python
 
 [![PyPI version](https://img.shields.io/pypi/v/tonplay-sdk)](https://pypi.python.org/pypi/tonplay-sdk)
 
-This is a [lightweight library](https://github.com/90K2/tonplay-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
+This is a [lightweight library](https://gitlab.com/ton-play/python-sdk) that works as a connector to [TON Play public API](https://docs.tonplay.io/)
 ## Installation
 
 ```bash
-pip install tonplay-connector
+pip install tonplay-sdk
 ```
 
 ## Get API Key
 
 To get API Key [follow the link](https://docs.tonplay.io/digital-assets-api/api-key)
 
 ## RESTful APIs
```

### Comparing `tonplay-sdk-0.0.6/tonplay_sdk.egg-info/SOURCES.txt` & `tonplay-sdk-0.0.7/tonplay_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

