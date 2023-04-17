# Comparing `tmp/ln-markets-1.0.8.tar.gz` & `tmp/ln-markets-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ln-markets-1.0.8.tar", last modified: Thu May 19 14:26:32 2022, max compression
+gzip compressed data, was "ln-markets-1.0.9.tar", last modified: Mon May 23 14:48:14 2022, max compression
```

## Comparing `ln-markets-1.0.8.tar` & `ln-markets-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-19 14:26:32.276371 ln-markets-1.0.8/
--rw-rw-r--   0 romain    (1000) romain    (1000)     1067 2022-05-10 09:43:34.000000 ln-markets-1.0.8/LICENSE
--rw-rw-r--   0 romain    (1000) romain    (1000)    14261 2022-05-19 14:26:32.276371 ln-markets-1.0.8/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)    13424 2022-05-10 10:57:09.000000 ln-markets-1.0.8/README.md
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-19 14:26:32.276371 ln-markets-1.0.8/ln_markets.egg-info/
--rw-rw-r--   0 romain    (1000) romain    (1000)    14261 2022-05-19 14:26:31.000000 ln-markets-1.0.8/ln_markets.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      284 2022-05-19 14:26:32.000000 ln-markets-1.0.8/ln_markets.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-19 14:26:31.000000 ln-markets-1.0.8/ln_markets.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       82 2022-05-19 14:26:32.000000 ln-markets-1.0.8/ln_markets.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       10 2022-05-19 14:26:32.000000 ln-markets-1.0.8/ln_markets.egg-info/top_level.txt
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-19 14:26:32.276371 ln-markets-1.0.8/lnmarkets/
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-1.0.8/lnmarkets/__init__.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     9944 2022-05-10 10:28:50.000000 ln-markets-1.0.8/lnmarkets/rest.py
--rw-rw-r--   0 romain    (1000) romain    (1000)     2361 2022-05-19 14:26:20.000000 ln-markets-1.0.8/lnmarkets/websockets.py
--rw-rw-r--   0 romain    (1000) romain    (1000)      104 2022-05-10 09:43:34.000000 ln-markets-1.0.8/pyproject.toml
--rw-rw-r--   0 romain    (1000) romain    (1000)       89 2022-05-19 14:26:32.276371 ln-markets-1.0.8/setup.cfg
--rw-rw-r--   0 romain    (1000) romain    (1000)     1347 2022-05-19 14:26:20.000000 ln-markets-1.0.8/setup.py
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-23 14:48:14.146736 ln-markets-1.0.9/
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1067 2022-05-10 09:43:34.000000 ln-markets-1.0.9/LICENSE
+-rw-rw-r--   0 romain    (1000) romain    (1000)    14261 2022-05-23 14:48:14.146736 ln-markets-1.0.9/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)    13424 2022-05-10 10:57:09.000000 ln-markets-1.0.9/README.md
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-23 14:48:14.146736 ln-markets-1.0.9/ln_markets.egg-info/
+-rw-rw-r--   0 romain    (1000) romain    (1000)    14261 2022-05-23 14:48:13.000000 ln-markets-1.0.9/ln_markets.egg-info/PKG-INFO
+-rw-rw-r--   0 romain    (1000) romain    (1000)      284 2022-05-23 14:48:14.000000 ln-markets-1.0.9/ln_markets.egg-info/SOURCES.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-23 14:48:13.000000 ln-markets-1.0.9/ln_markets.egg-info/dependency_links.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       19 2022-05-23 14:48:14.000000 ln-markets-1.0.9/ln_markets.egg-info/requires.txt
+-rw-rw-r--   0 romain    (1000) romain    (1000)       10 2022-05-23 14:48:14.000000 ln-markets-1.0.9/ln_markets.egg-info/top_level.txt
+drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2022-05-23 14:48:14.146736 ln-markets-1.0.9/lnmarkets/
+-rw-rw-r--   0 romain    (1000) romain    (1000)        1 2022-05-10 09:43:34.000000 ln-markets-1.0.9/lnmarkets/__init__.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)     9944 2022-05-10 10:28:50.000000 ln-markets-1.0.9/lnmarkets/rest.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)     2349 2022-05-23 14:47:06.000000 ln-markets-1.0.9/lnmarkets/websockets.py
+-rw-rw-r--   0 romain    (1000) romain    (1000)      104 2022-05-10 09:43:34.000000 ln-markets-1.0.9/pyproject.toml
+-rw-rw-r--   0 romain    (1000) romain    (1000)       89 2022-05-23 14:48:14.146736 ln-markets-1.0.9/setup.cfg
+-rw-rw-r--   0 romain    (1000) romain    (1000)     1185 2022-05-23 14:47:06.000000 ln-markets-1.0.9/setup.py
```

### Comparing `ln-markets-1.0.8/LICENSE` & `ln-markets-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ln-markets-1.0.8/PKG-INFO` & `ln-markets-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 1.0.8
+Version: 1.0.9
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ln-markets-1.0.8/README.md` & `ln-markets-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ln-markets-1.0.8/ln_markets.egg-info/PKG-INFO` & `ln-markets-1.0.9/ln_markets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ln-markets
-Version: 1.0.8
+Version: 1.0.9
 Summary: LN Markets API python implementation
 Home-page: https://github.com/ln-markets/api-python
 Author: Romain ROUPHAEL
 License: MIT
 Keywords: lnmarkets trading rest api bitcoin lightning network futures options
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ln-markets-1.0.8/lnmarkets/rest.py` & `ln-markets-1.0.9/lnmarkets/rest.py`

 * *Files identical despite different names*

### Comparing `ln-markets-1.0.8/lnmarkets/websockets.py` & `ln-markets-1.0.9/lnmarkets/websockets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import websocket
-import time
 import os
 import secrets
 import json
 
 def get_hostname(network):
     hostname = os.environ.get('LNMARKETS_API_HOSTNAME')
```

### Comparing `ln-markets-1.0.8/setup.py` & `ln-markets-1.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,35 +3,26 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ln-markets',
-    version='1.0.8',
+    version='1.0.9',
     packages=['lnmarkets'],
     description='LN Markets API python implementation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/ln-markets/api-python',
     author='Romain ROUPHAEL',
     license='MIT',
     keywords='lnmarkets trading rest api bitcoin lightning network futures options',
     install_requires=[
-        'os',
-        'urllib.parse',
-        'datetime',
-        'base64',
         'requests',
-        'hashlib',
-        'hmac',
-        'json',
-        'websocket',
-        'time',
-        'secrets'
+        'websocket'
       ],
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
```

