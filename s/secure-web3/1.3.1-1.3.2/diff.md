# Comparing `tmp/secure_web3-1.3.1.tar.gz` & `tmp/secure_web3-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure_web3-1.3.1.tar", last modified: Mon Apr 17 21:17:55 2023, max compression
+gzip compressed data, was "secure_web3-1.3.2.tar", last modified: Mon Apr 17 21:22:30 2023, max compression
```

## Comparing `secure_web3-1.3.1.tar` & `secure_web3-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.632790 secure_web3-1.3.1/
--rw-r--r--   0 anon      (1000) anon      (1000)     1080 2023-02-21 22:28:09.000000 secure_web3-1.3.1/LICENSE.txt
--rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 21:17:55.632790 secure_web3-1.3.1/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)     2761 2023-04-03 00:13:38.000000 secure_web3-1.3.1/README.md
--rw-r--r--   0 anon      (1000) anon      (1000)      666 2023-04-17 21:17:39.000000 secure_web3-1.3.1/pyproject.toml
--rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-17 21:17:55.632790 secure_web3-1.3.1/setup.cfg
--rw-r--r--   0 anon      (1000) anon      (1000)      554 2023-04-17 21:17:39.000000 secure_web3-1.3.1/setup.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.624790 secure_web3-1.3.1/src/
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.624790 secure_web3-1.3.1/src/secure_web3/
--rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-03-08 04:05:51.000000 secure_web3-1.3.1/src/secure_web3/__init__.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3/data/
--rw-r--r--   0 anon      (1000) anon      (1000)      717 2023-02-21 22:41:47.000000 secure_web3-1.3.1/src/secure_web3/data/networks.json
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3/keys/
--rw-r--r--   0 anon      (1000) anon      (1000)      162 2023-01-26 23:28:56.000000 secure_web3-1.3.1/src/secure_web3/keys/default_wallet.json
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3/lib/
--rw-r--r--   0 anon      (1000) anon      (1000)     6187 2023-01-22 21:32:35.000000 secure_web3-1.3.1/src/secure_web3/lib/abi_lib.py
--rw-r--r--   0 anon      (1000) anon      (1000)      660 2023-03-08 05:44:20.000000 secure_web3-1.3.1/src/secure_web3/lib/inputs.py
--rw-r--r--   0 anon      (1000) anon      (1000)      257 2023-02-21 22:39:53.000000 secure_web3-1.3.1/src/secure_web3/lib/load_networks.py
--rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-01-22 21:27:26.000000 secure_web3-1.3.1/src/secure_web3/lib/style.py
--rw-r--r--   0 anon      (1000) anon      (1000)      580 2023-01-26 23:29:39.000000 secure_web3-1.3.1/src/secure_web3/lib/w3_validation.py
--rw-r--r--   0 anon      (1000) anon      (1000)     8025 2023-03-14 01:49:35.000000 secure_web3-1.3.1/src/secure_web3/lib/wallet_manager.py
--rw-r--r--   0 anon      (1000) anon      (1000)     6418 2023-04-17 20:51:08.000000 secure_web3-1.3.1/src/secure_web3/sw3.py
--rw-r--r--   0 anon      (1000) anon      (1000)    16528 2023-04-17 21:16:45.000000 secure_web3-1.3.1/src/secure_web3/sw3_wallet.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:17:55.628790 secure_web3-1.3.1/src/secure_web3.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)      598 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       50 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       12 2023-04-17 21:17:55.000000 secure_web3-1.3.1/src/secure_web3.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:22:30.052799 secure_web3-1.3.2/
+-rw-r--r--   0 anon      (1000) anon      (1000)     1080 2023-02-21 22:28:09.000000 secure_web3-1.3.2/LICENSE.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 21:22:30.052799 secure_web3-1.3.2/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)     2761 2023-04-03 00:13:38.000000 secure_web3-1.3.2/README.md
+-rw-r--r--   0 anon      (1000) anon      (1000)      666 2023-04-17 21:22:17.000000 secure_web3-1.3.2/pyproject.toml
+-rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-17 21:22:30.052799 secure_web3-1.3.2/setup.cfg
+-rw-r--r--   0 anon      (1000) anon      (1000)      554 2023-04-17 21:22:17.000000 secure_web3-1.3.2/setup.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:22:30.044799 secure_web3-1.3.2/src/
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:22:30.048799 secure_web3-1.3.2/src/secure_web3/
+-rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-03-08 04:05:51.000000 secure_web3-1.3.2/src/secure_web3/__init__.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:22:30.048799 secure_web3-1.3.2/src/secure_web3/data/
+-rw-r--r--   0 anon      (1000) anon      (1000)      717 2023-02-21 22:41:47.000000 secure_web3-1.3.2/src/secure_web3/data/networks.json
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:22:30.048799 secure_web3-1.3.2/src/secure_web3/keys/
+-rw-r--r--   0 anon      (1000) anon      (1000)      162 2023-01-26 23:28:56.000000 secure_web3-1.3.2/src/secure_web3/keys/default_wallet.json
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:22:30.052799 secure_web3-1.3.2/src/secure_web3/lib/
+-rw-r--r--   0 anon      (1000) anon      (1000)     6187 2023-01-22 21:32:35.000000 secure_web3-1.3.2/src/secure_web3/lib/abi_lib.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      660 2023-03-08 05:44:20.000000 secure_web3-1.3.2/src/secure_web3/lib/inputs.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      257 2023-02-21 22:39:53.000000 secure_web3-1.3.2/src/secure_web3/lib/load_networks.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-01-22 21:27:26.000000 secure_web3-1.3.2/src/secure_web3/lib/style.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      580 2023-01-26 23:29:39.000000 secure_web3-1.3.2/src/secure_web3/lib/w3_validation.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     8025 2023-03-14 01:49:35.000000 secure_web3-1.3.2/src/secure_web3/lib/wallet_manager.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     6418 2023-04-17 20:51:08.000000 secure_web3-1.3.2/src/secure_web3/sw3.py
+-rw-r--r--   0 anon      (1000) anon      (1000)    16528 2023-04-17 21:16:45.000000 secure_web3-1.3.2/src/secure_web3/sw3_wallet.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-17 21:22:30.048799 secure_web3-1.3.2/src/secure_web3.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)     3371 2023-04-17 21:22:30.000000 secure_web3-1.3.2/src/secure_web3.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)      598 2023-04-17 21:22:30.000000 secure_web3-1.3.2/src/secure_web3.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-17 21:22:30.000000 secure_web3-1.3.2/src/secure_web3.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       50 2023-04-17 21:22:30.000000 secure_web3-1.3.2/src/secure_web3.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       12 2023-04-17 21:22:30.000000 secure_web3-1.3.2/src/secure_web3.egg-info/top_level.txt
```

### Comparing `secure_web3-1.3.1/LICENSE.txt` & `secure_web3-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/PKG-INFO` & `secure_web3-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure_web3
-Version: 1.3.1
+Version: 1.3.2
 Summary: Secure wallet and development enviroment
 Home-page: https://github.com/darkerego/secure_web3
 Author: darkerego
 Author-email: Darkergo <chevisyoung@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/darkerego/secure_web3
 Project-URL: Bug Tracker, https://github.com/darkerego/secure_web3/issues
```

### Comparing `secure_web3-1.3.1/README.md` & `secure_web3-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/pyproject.toml` & `secure_web3-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "secure_web3"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Darkergo", email="chevisyoung@gmail.com" },
 ]
 description = "Secure wallet and development enviroment"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `secure_web3-1.3.1/setup.py` & `secure_web3-1.3.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='secure_web3',
-    version='1.3.1',
+    version='1.3.2',
     packages=['secure_web3'],
     install_requires=['web3', 'pycryptodome', 'python-dotenv', 'eth-utils', 'colored'],
     package_dir={"": "src"},
     include_package_data=True,
     data_files=[('', ['src/secure_web3/keys/default_wallet.json', 'src/secure_web3/data/networks.json'])],
     url='https://github.com/darkerego/secure_web3',
     license='MIT',
```

### Comparing `secure_web3-1.3.1/src/secure_web3/data/networks.json` & `secure_web3-1.3.2/src/secure_web3/data/networks.json`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3/lib/abi_lib.py` & `secure_web3-1.3.2/src/secure_web3/lib/abi_lib.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3/lib/inputs.py` & `secure_web3-1.3.2/src/secure_web3/lib/inputs.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3/lib/style.py` & `secure_web3-1.3.2/src/secure_web3/lib/style.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3/lib/w3_validation.py` & `secure_web3-1.3.2/src/secure_web3/lib/w3_validation.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3/lib/wallet_manager.py` & `secure_web3-1.3.2/src/secure_web3/lib/wallet_manager.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3/sw3.py` & `secure_web3-1.3.2/src/secure_web3/sw3.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3/sw3_wallet.py` & `secure_web3-1.3.2/src/secure_web3/sw3_wallet.py`

 * *Files identical despite different names*

### Comparing `secure_web3-1.3.1/src/secure_web3.egg-info/PKG-INFO` & `secure_web3-1.3.2/src/secure_web3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-web3
-Version: 1.3.1
+Version: 1.3.2
 Summary: Secure wallet and development enviroment
 Home-page: https://github.com/darkerego/secure_web3
 Author: darkerego
 Author-email: Darkergo <chevisyoung@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/darkerego/secure_web3
 Project-URL: Bug Tracker, https://github.com/darkerego/secure_web3/issues
```

### Comparing `secure_web3-1.3.1/src/secure_web3.egg-info/SOURCES.txt` & `secure_web3-1.3.2/src/secure_web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

