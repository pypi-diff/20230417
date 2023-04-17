# Comparing `tmp/mls-api-1.5.0.tar.gz` & `tmp/mls-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.5.0.tar", last modified: Sun Apr 16 17:09:40 2023, max compression
+gzip compressed data, was "dist/mls-api-2.0.0.tar", last modified: Mon Apr 17 17:24:22 2023, max compression
```

## Comparing `mls-api-1.5.0.tar` & `mls-api-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 17:09:40.149324 mls-api-1.5.0/
--rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 17:09:40.149554 mls-api-1.5.0/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2258 2023-04-16 06:16:08.000000 mls-api-1.5.0/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 17:09:40.145877 mls-api-1.5.0/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      343 2023-04-16 16:43:33.000000 mls-api-1.5.0/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:55:53.000000 mls-api-1.5.0/mls_api/assists.py
--rw-r--r--   0 finn       (501) staff       (20)      655 2023-04-16 16:56:36.000000 mls-api-1.5.0/mls_api/auth.py
--rw-r--r--   0 finn       (501) staff       (20)     1500 2023-04-16 16:56:03.000000 mls-api-1.5.0/mls_api/fixtures.py
--rw-r--r--   0 finn       (501) staff       (20)     1510 2023-04-16 16:56:14.000000 mls-api-1.5.0/mls_api/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1496 2023-04-16 16:56:25.000000 mls-api-1.5.0/mls_api/latest_news.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:56:48.000000 mls-api-1.5.0/mls_api/offense.py
--rw-r--r--   0 finn       (501) staff       (20)     1691 2023-04-16 17:08:48.000000 mls-api-1.5.0/mls_api/players.py
--rw-r--r--   0 finn       (501) staff       (20)     1458 2023-04-16 16:57:12.000000 mls-api-1.5.0/mls_api/rtd.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2023-04-16 06:09:23.000000 mls-api-1.5.0/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)     1508 2023-04-16 16:57:23.000000 mls-api-1.5.0/mls_api/standings.py
--rw-r--r--   0 finn       (501) staff       (20)     1476 2023-04-16 16:57:34.000000 mls-api-1.5.0/mls_api/teams.py
--rw-r--r--   0 finn       (501) staff       (20)     1512 2023-04-16 16:57:46.000000 mls-api-1.5.0/mls_api/top_scorer.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 17:09:02.000000 mls-api-1.5.0/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 17:09:40.148885 mls-api-1.5.0/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 17:09:20.000000 mls-api-1.5.0/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 17:09:40.150051 mls-api-1.5.0/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 17:09:02.000000 mls-api-1.5.0/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-17 17:24:22.307008 mls-api-2.0.0/
+-rw-r--r--   0 finn       (501) staff       (20)     5415 2023-04-17 17:24:22.307538 mls-api-2.0.0/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2329 2023-04-17 17:23:31.000000 mls-api-2.0.0/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-17 17:24:22.296240 mls-api-2.0.0/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      343 2023-04-16 16:43:33.000000 mls-api-2.0.0/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:55:53.000000 mls-api-2.0.0/mls_api/assists.py
+-rw-r--r--   0 finn       (501) staff       (20)      658 2023-04-17 17:22:53.000000 mls-api-2.0.0/mls_api/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)     1500 2023-04-16 16:56:03.000000 mls-api-2.0.0/mls_api/fixtures.py
+-rw-r--r--   0 finn       (501) staff       (20)     1510 2023-04-16 16:56:14.000000 mls-api-2.0.0/mls_api/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1496 2023-04-16 16:56:25.000000 mls-api-2.0.0/mls_api/latest_news.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:56:48.000000 mls-api-2.0.0/mls_api/offense.py
+-rw-r--r--   0 finn       (501) staff       (20)     1691 2023-04-16 17:08:48.000000 mls-api-2.0.0/mls_api/players.py
+-rw-r--r--   0 finn       (501) staff       (20)     1458 2023-04-16 16:57:12.000000 mls-api-2.0.0/mls_api/rtd.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2023-04-16 06:09:23.000000 mls-api-2.0.0/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)     1508 2023-04-16 16:57:23.000000 mls-api-2.0.0/mls_api/standings.py
+-rw-r--r--   0 finn       (501) staff       (20)     1476 2023-04-16 16:57:34.000000 mls-api-2.0.0/mls_api/teams.py
+-rw-r--r--   0 finn       (501) staff       (20)     1512 2023-04-16 16:57:46.000000 mls-api-2.0.0/mls_api/top_scorer.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-17 17:22:41.000000 mls-api-2.0.0/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-17 17:24:22.306279 mls-api-2.0.0/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5415 2023-04-17 17:24:22.000000 mls-api-2.0.0/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-17 17:24:22.000000 mls-api-2.0.0/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-17 17:24:22.000000 mls-api-2.0.0/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-17 17:24:05.000000 mls-api-2.0.0/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-17 17:24:22.000000 mls-api-2.0.0/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-17 17:24:22.000000 mls-api-2.0.0/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-17 17:24:22.309198 mls-api-2.0.0/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-17 17:22:41.000000 mls-api-2.0.0/setup.py
```

### Comparing `mls-api-1.5.0/PKG-INFO` & `mls-api-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.5.0
+Version: 2.0.0
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -67,16 +67,20 @@
             print(mls_rtd)
         
             ## Retrieve MLS Historical Data
             mls_historical = mls_api.get_historical_data()
             print(mls_historical)
         
             ## Retrieve MLS Players Data
-            limit = 10
+            limit = 5
             offset = 5
+        
+            mls_players_l = mls_api.get_players(limit=limit)
+            print(mls_players_l)
+        
             mls_players = mls_api.get_players(limit=limit, offset=offset)
             print(mls_players)
         
             ## Retrieve MLS Assist Data
             mls_assists = mls_api.get_assists()
             print(mls_assists)
```

### Comparing `mls-api-1.5.0/README.md` & `mls-api-2.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -46,16 +46,20 @@
 print(mls_rtd)
 
 ## Retrieve MLS Historical Data
 mls_historical = mls_api.get_historical_data()
 print(mls_historical)
 
 ## Retrieve MLS Players Data
-limit = 10
+limit = 5
 offset = 5
+
+mls_players_l = mls_api.get_players(limit=limit)
+print(mls_players_l)
+
 mls_players = mls_api.get_players(limit=limit, offset=offset)
 print(mls_players)
 
 ## Retrieve MLS Assist Data
 mls_assists = mls_api.get_assists()
 print(mls_assists)
```

### Comparing `mls-api-1.5.0/mls_api/assists.py` & `mls-api-2.0.0/mls_api/assists.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/auth.py` & `mls-api-2.0.0/mls_api/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         # Already added when you pass json= but not when you pass data=
         # 'Content-Type': 'application/json',
     }
     payload = {
         'username': username, 
         'password': password
     }
-    response = requests.post(url='https://mlssoccerapi.com/login', headers=headers, json=payload)
+    response = requests.post(url='https://mlssoccerapi.com/v1/login', headers=headers, json=payload)
     statusCode = response.status_code
     bearerToken = response.json().get('Document')
     if statusCode == 200: 
         os.environ['BEARER_TOKEN'] = bearerToken    
     return {
         'statusCode': statusCode, 
         'bearerToken': bearerToken
```

### Comparing `mls-api-1.5.0/mls_api/fixtures.py` & `mls-api-2.0.0/mls_api/fixtures.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/historical.py` & `mls-api-2.0.0/mls_api/historical.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/latest_news.py` & `mls-api-2.0.0/mls_api/latest_news.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/offense.py` & `mls-api-2.0.0/mls_api/offense.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/players.py` & `mls-api-2.0.0/mls_api/players.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/rtd.py` & `mls-api-2.0.0/mls_api/rtd.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/six.py` & `mls-api-2.0.0/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/standings.py` & `mls-api-2.0.0/mls_api/standings.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/teams.py` & `mls-api-2.0.0/mls_api/teams.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api/top_scorer.py` & `mls-api-2.0.0/mls_api/top_scorer.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.5.0/mls_api.egg-info/PKG-INFO` & `mls-api-2.0.0/mls_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.5.0
+Version: 2.0.0
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -67,16 +67,20 @@
             print(mls_rtd)
         
             ## Retrieve MLS Historical Data
             mls_historical = mls_api.get_historical_data()
             print(mls_historical)
         
             ## Retrieve MLS Players Data
-            limit = 10
+            limit = 5
             offset = 5
+        
+            mls_players_l = mls_api.get_players(limit=limit)
+            print(mls_players_l)
+        
             mls_players = mls_api.get_players(limit=limit, offset=offset)
             print(mls_players)
         
             ## Retrieve MLS Assist Data
             mls_assists = mls_api.get_assists()
             print(mls_assists)
```

### Comparing `mls-api-1.5.0/setup.py` & `mls-api-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.5.0"
+VERSION = "2.0.0"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

