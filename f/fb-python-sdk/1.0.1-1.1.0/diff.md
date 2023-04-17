# Comparing `tmp/fb-python-sdk-1.0.1.tar.gz` & `tmp/fb-python-sdk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb-python-sdk-1.0.1.tar", last modified: Fri Jan 20 17:25:52 2023, max compression
+gzip compressed data, was "fb-python-sdk-1.1.0.tar", last modified: Sun Apr 16 09:37:38 2023, max compression
```

## Comparing `fb-python-sdk-1.0.1.tar` & `fb-python-sdk-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-20 17:25:52.975526 fb-python-sdk-1.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.0.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)     7387 2023-01-20 17:25:52.975021 fb-python-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     6378 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/dev-requirements.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-20 17:25:52.961613 fb-python-sdk-1.0.1/fb_python_sdk.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     7387 2023-01-20 17:25:52.000000 fb-python-sdk-1.0.1/fb_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1070 2023-01-20 17:25:52.000000 fb-python-sdk-1.0.1/fb_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-01-20 17:25:52.000000 fb-python-sdk-1.0.1/fb_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      218 2023-01-20 17:25:52.000000 fb-python-sdk-1.0.1/fb_python_sdk.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       34 2023-01-20 17:25:52.000000 fb-python-sdk-1.0.1/fb_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-20 17:25:52.967024 fb-python-sdk-1.0.1/fbclient/
--rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/category.py
--rw-r--r--   0 mac        (501) staff       (20)    18331 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/fbclient/client.py
--rw-r--r--   0 mac        (501) staff       (20)    10597 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/fbclient/common_types.py
--rw-r--r--   0 mac        (501) staff       (20)     8913 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/config.py
--rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)    12389 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/fbclient/evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     8523 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/event_types.py
--rw-r--r--   0 mac        (501) staff       (20)     9517 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)     3688 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/fbclient/status.py
--rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/status_types.py
--rw-r--r--   0 mac        (501) staff       (20)    10678 2023-01-19 10:19:35.000000 fb-python-sdk-1.0.1/fbclient/streaming.py
--rw-r--r--   0 mac        (501) staff       (20)      489 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/update_processor.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-20 17:25:52.969617 fb-python-sdk-1.0.1/fbclient/utils/
--rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/fbclient/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/utils/exponential_backoff_jitter_strategy.py
--rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/utils/http_client.py
--rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/utils/repeatable_task.py
--rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/fbclient/utils/rwlock.py
--rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/fbclient/utils/variation_splitting_algorithm.py
--rw-r--r--   0 mac        (501) staff       (20)       18 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/fbclient/version.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-20 17:25:52.970429 fb-python-sdk-1.0.1/intergration_tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.0.1/intergration_tests/__init__.py
--rw-------   0 mac        (501) staff       (20)     1439 2023-01-19 07:50:07.000000 fb-python-sdk-1.0.1/intergration_tests/run_in_start_wait.py
--rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-01-20 17:25:52.975704 fb-python-sdk-1.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1788 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-20 17:25:52.974351 fb-python-sdk-1.0.1/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/tests/test_data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/tests/test_data_update_status_provider.py
--rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/tests/test_evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.0.1/tests/test_event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)    10707 2023-01-20 17:20:21.000000 fb-python-sdk-1.0.1/tests/test_fbclient.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-16 09:37:38.866149 fb-python-sdk-1.1.0/
+-rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.0/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)    10429 2023-04-16 09:37:38.865652 fb-python-sdk-1.1.0/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     9369 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.0/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/dev-requirements.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-16 09:37:38.842927 fb-python-sdk-1.1.0/fb_python_sdk.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)    10429 2023-04-16 09:37:38.000000 fb-python-sdk-1.1.0/fb_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1070 2023-04-16 09:37:38.000000 fb-python-sdk-1.1.0/fb_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-16 09:37:38.000000 fb-python-sdk-1.1.0/fb_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      218 2023-04-16 09:37:38.000000 fb-python-sdk-1.1.0/fb_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       34 2023-04-16 09:37:38.000000 fb-python-sdk-1.1.0/fb_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-16 09:37:38.854014 fb-python-sdk-1.1.0/fbclient/
+-rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/category.py
+-rw-r--r--   0 mac        (501) staff       (20)    18094 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.0/fbclient/client.py
+-rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.0/fbclient/common_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.0/fbclient/config.py
+-rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)    12389 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.0/fbclient/evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     8523 2023-04-14 07:20:29.000000 fb-python-sdk-1.1.0/fbclient/event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/event_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     9517 2023-04-16 06:51:44.000000 fb-python-sdk-1.1.0/fbclient/interfaces.py
+-rw-r--r--   0 mac        (501) staff       (20)     3688 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.0/fbclient/status.py
+-rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/status_types.py
+-rw-r--r--   0 mac        (501) staff       (20)    10647 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.0/fbclient/streaming.py
+-rw-r--r--   0 mac        (501) staff       (20)      489 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.0/fbclient/update_processor.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-16 09:37:38.858521 fb-python-sdk-1.1.0/fbclient/utils/
+-rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.0/fbclient/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/utils/exponential_backoff_jitter_strategy.py
+-rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/utils/http_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/utils/repeatable_task.py
+-rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/fbclient/utils/rwlock.py
+-rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.0/fbclient/utils/variation_splitting_algorithm.py
+-rw-r--r--   0 mac        (501) staff       (20)       18 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.0/fbclient/version.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-16 09:37:38.859958 fb-python-sdk-1.1.0/intergration_tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.0/intergration_tests/__init__.py
+-rw-------   0 mac        (501) staff       (20)     1437 2023-04-16 02:24:41.000000 fb-python-sdk-1.1.0/intergration_tests/run_in_start_wait.py
+-rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-16 09:37:38.866279 fb-python-sdk-1.1.0/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1838 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.0/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-16 09:37:38.864935 fb-python-sdk-1.1.0/tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.0/tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/tests/test_data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.0/tests/test_data_update_status_provider.py
+-rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/tests/test_evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.0/tests/test_event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)    10605 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.0/tests/test_fbclient.py
```

### Comparing `fb-python-sdk-1.0.1/LICENSE` & `fb-python-sdk-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/PKG-INFO` & `fb-python-sdk-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,156 +1,188 @@
-Metadata-Version: 2.1
-Name: fb-python-sdk
-Version: 1.0.1
-Summary: A Python SDK for FeatBit plateform
-Home-page: https://github.com/featbit/featbit-python-sdk
-Author: Dian SUN
-Author-email: featbit.master@gmail.com
-Project-URL: Code, https://github.com/featbit/featbit-python-sdk
-Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# FeatBit python sdk
+# FeatBit Server-Side SDK for Python
 
 ## Introduction
 
-This is the Python Server SDK for the feature management platform FeatBit. It is
-intended for use in a multiple-users python server applications.
-
-This SDK has two main purposes:
+This is the Python Server-Side SDK for the 100% open-source feature flags management platform [FeatBit](https://github.com/featbit/featbit).
 
-- Store the available feature flags and evaluate the feature flags by given user in the server side SDK
-- Sends feature flags usage, and custom events for the insights and A/B/n testing.
+The FeatBit Server-Side SDK for Python is designed primarily for use in multi-user systems such as web servers and applications.
 
 ## Data synchonization
 
-We use websocket to make the local data synchronized with the server, and then store them in the memory by default.
-Whenever there is any changes to a feature flag or his related data, the changes would be pushed to the SDK, the average
-synchronization time is less than **100** ms. Be aware the websocket connection can be interrupted by any error or
-internet interruption, but it would be restored automatically right after the problem is gone.
+We use websocket to make the local data synchronized with the FeatBit server, and then store them in memory by
+default. Whenever there is any change to a feature flag or its related data, this change will be pushed to the SDK and
+the average synchronization time is less than 100 ms. Be aware the websocket connection may be interrupted due to
+internet outage, but it will be resumed automatically once the problem is gone.
 
-## Offline mode support
+If you want to use your own data source, see [Offline Mode](#offline-mode).
 
-In the offline mode, SDK DOES not exchange any data with feature flag center, this mode is only use for internal test for instance.
+## Get Started
 
-To open the offline mode:
-```python
-config = Config(env_secret, event_url, streaming_url, offline=True)
+### Installation
+install the sdk in using pip, this version of the SDK is compatible with Python 3.6 through 3.11.
+
+```shell
+pip install fb-python-sdk
 ```
 
-## Evaluation of a feature flag
+### Quick Start
 
-SDK will initialize all the related data(feature flags, segments etc.) in the bootstrapping and receive the data updates
-in real time, as mentioned in the above
+> Note that the _**env_secret**_, _**streaming_url**_ and _**event_url**_ are required to initialize the SDK.
 
-After initialization, the SDK has all the feature flags in the memory and all evaluation is done locally and synchronously, the average evaluation time is < **10** ms.
+The following code demonstrates basic usage of the SDK.
 
-## Installation
-install the sdk in using pip, this version of the SDK is compatible with Python 3.6 through 3.10.
+```python
+from fbclient import get, set_config
+from fbclient.config import Config
 
+env_secret = '<replace-with-your-env-secret>'
+event_url = 'http://localhost:5100'
+streaming_url = '"ws://localhost:5100"'
+
+set_config(Config(env_secret, event_url, streaming_url))
+client = get()
+
+if client.initialize:
+    flag_key = '<replace-with-your-flag-key>'
+    user_key = 'bot-id'
+    user_name = 'bot'
+    user = {'key': user_key, 'name': user_name}
+    detail = client.variation_detail(flag_key, user, default=None)
+    print(f'flag {flag_key} returns {detail.value} for user {user_key}, reason: {detail.reason}')
+
+# ensure that the SDK shuts down cleanly and has a chance to deliver events to FeatBit before the program exits
+client.stop()
 ```
-pip install fb-python-sdk
-```
 
-## SDK
+### Examples
+
+- [Python Demo](https://github.com/featbit/featbit-samples/blob/main/samples/dino-game/demo-python/demo_python.py)
+
+### FBClient
 
-Applications SHOULD instantiate a single instance for the lifetime of the application. In the case where an application
+Applications **SHOULD instantiate a single FBClient instance** for the lifetime of the application. In the case where an application
 needs to evaluate feature flags from different environments, you may create multiple clients, but they should still be
 retained for the lifetime of the application rather than created per request or per thread.
 
-### Bootstrapping
+#### Bootstrapping
 
-The bootstrapping is in fact the call of constructor of `FFCClient`, in which the SDK will be initialized and connect to feature flag center
+The bootstrapping is in fact the call of constructor of `FBClient`, in which the SDK will be initialized and connect to FeatBit.
 
 The constructor will return when it successfully connects, or when the timeout(default: 15 seconds) expires, whichever comes first. If it has not succeeded in connecting when the timeout elapses, you will receive the client in an uninitialized state where feature flags will return default values; it will still continue trying to connect in the background unless there has been a network error or you close the client(using `stop()`). You can detect whether initialization has succeeded by calling `initialize()`.
 
-The best way to use the SDK as a singleton, first make sure you have called `fbclient.set_config()` at startup time. Then `fbclient.get()` will return the same shared `fbclient.client.FFCClient` instance each time. The client will be initialized if it runs first time.
+The best way to use the SDK as a singleton, first make sure you have called `fbclient.set_config()` at startup time. Then `fbclient.get()` will return the same shared `fbclient.client.FBClient` instance each time. The client will be initialized if it runs first time.
 ```python
 from fbclient.config import Config
 from fbclient import get, set_config 
 
 set_config(Config(env_secret, event_url, streaming_url))
 client = get()
 
 if client.initialize:
-    # your code
-
+    # the client is ready
 ```
-You can also manage your `fbclient.client.FBClient`, the SDK will be initialized if you call `fbclient.client.FBClient` constructor.
+You can also manage your `fbclient.client.FBClient`, the SDK will be initialized if you call `fbclient.client.FBClient` constructor. With constructor, you can set the timeout for initialization, the default value is 15 seconds.
 ```python
 from fbclient.config import Config
 from fbclient.client import FBClient
 
 client = FBClient(Config(env_secret, event_url, streaming_url), start_wait=15)
 
 if client.initialize:
-    # your code
-
+    # the client is ready
 ```
 If you prefer to have the constructor return immediately, and then wait for initialization to finish at some other point, you can use `fbclient.client.fbclient.update_status_provider` object, which provides an asynchronous way, as follows:
 
 ``` python
 from fbclient.config import Config
 from fbclient.client import FBClient
 
-client = FFCClient(Config(env_secret), start_wait=0)
-if client._update_status_provider.wait_for_OKState():
-    # your code
-
+client = FBClient(Config(env_secret), start_wait=0)
+if client.update_status_provider.wait_for_OKState():
+    # the client is ready
 ```
 
+It's possible to set a timeout in seconds for the `wait_for_OKState` method. If the timeout is reached, the method will return `False` and the client will still be in an uninitialized state. If you do not specify a timeout, the method will wait indefinitely.
 
-### Evaluation
 
-SDK calculates the value of a feature flag for a given user, and returns a flag vlaue/an object that describes the way that the value was determined.
+> To check if the client is ready is optional. Even if the client is not ready, you can still evaluate feature flags, but the default value will be returned if SDK is not yet initialized.
+
+### FBUser
 
-`User`: A dictionary of attributes that can affect flag evaluation, usually corresponding to a user of your application.
+A dictionary of attributes that can affect flag evaluation, usually corresponding to a user of your application.
 This object contains built-in properties(`key`, `name`). The `key` and `name` are required. The `key` must uniquely identify each user; this could be a username or email address for authenticated users, or a ID for anonymous users. The `name` is used to search your user quickly. You may also define custom properties with arbitrary names and values.
-For instance, the custom key should be a string; the custom value should be a string or a number
+For instance, the custom key should be a string; the custom value should be a string, number or boolean value
+
+```python
+user = {'key': user_key, 'name': user_name, 'age': age}
+```
+
+### Evaluation
+
+SDK calculates the value of a feature flag for a given user, and returns a flag vlaue/an object that describes the way that the value was determined.
 
 ```python
 if client.initialize:
     user = {'key': user_key, 'name': user_name, 'age': age}
+    # evaluate the flag value
     flag_value = client.variation(flag_key, user, default_value)
-    # your if/else code according to flag value
-
+    # evaluate the flag value and get the detail
+    detail = client.variation_detail(flag_key, user, default=None)
 ```
-If evaluation called before SDK client initialized or you set the wrong flag key or user for the evaluation, SDK will return 
-the default value you set. The `fbclient.common_types.FlagState` will explain the details of the last evaluation including error raison.
 
-If you would like to get variations of all feature flags in a special environment, you can use `fbclient.client.FBClient.get_all_latest_flag_variations`, SDK will return `fbclient.common_types.AllFlagStates`, that explain the details of all feature flags
+If you would like to get variations of all feature flags in a special environment, you can use `fbclient.client.FBClient.get_all_latest_flag_variations`, SDK will return `fbclient.common_types.AllFlagStates`, that explain the details of all feature flags. `fbclient.common_types.AllFlagStates.get()` returns the detail of a given feature flag key.
+
 ```python
 if client.initialize:
     user = {'key': user_key, 'name': user_name}
     all_flag_values = client.get_all_latest_flag_variations(user)
-    ed = all_flag_values.get(flag_key)
-    flag_value = ed.variation
-    # your if/else code according to flag value
+    detail = all_flag_values.get(flag_key, default=None)
+```
+
+> Note that if evaluation called before Go SDK client initialized, you set the wrong flag key/user for the evaluation or the related feature flag is not found, SDK will return the default value you set. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error raison.
+
+### Offline Mode
+
+In some situations, you might want to stop making remote calls to FeatBit. Here is how:
 
-    
+```python
+config = Config(env_secret, event_url, streaming_url, offline=True)
+```
+When you put the SDK in offline mode, no insight message is sent to the server and all feature flag evaluations return
+fallback values because there are no feature flags or segments available. If you want to use your own data source,
+SDK allows users to populate feature flags and segments data from a JSON string. Here is an example: [fbclient_test_data.json](tests/fbclient_test_data.json).
+
+The format of the data in flags and segments is defined by FeatBit and is subject to change. Rather than trying to construct these objects yourself, it's simpler to request existing flags directly from the FeatBit server in JSON format and use this output as the starting point for your file. Here's how:
+
+```shell
+# replace http://localhost:5100 with your evaluation server url
+curl -H "Authorization: <your-env-secret>" http://localhost:5100/api/public/sdk/server/latest-all > featbit-bootstrap.json
+```
+
+Then you can use this file to initialize the SDK in offline mode:
+
+```python
+// first load data from file and then
+client.initialize_from_external_json(json)
 ```
 
 ### Experiments (A/B/n Testing)
 We support automatic experiments for pageviews and clicks, you just need to set your experiment on our SaaS platform, then you should be able to see the result in near real time after the experiment is started.
 
 In case you need more control over the experiment data sent to our server, we offer a method to send custom event.
 ```python
 client.track_metric(user, event_name, numeric_value);
 ```
 **numeric_value** is not mandatory, the default value is **1**.
 
 Make sure `track_metric` is called after the related feature flag is evaluated by simply calling `variation` or `variation_detail`
 otherwise, the custom event may not be included into the experiment result.
+
+## Getting support
+
+- If you have a specific question about using this sdk, we encourage you
+  to [ask it in our slack](https://join.slack.com/t/featbit/shared_invite/zt-1ew5e2vbb-x6Apan1xZOaYMnFzqZkGNQ).
+- If you encounter a bug or would like to request a
+  feature, [submit an issue](https://github.com/featbit/featbit-python-sdk/issues/new).
+
+## See Also
+- [Connect To Python Sdk](https://docs.featbit.co/docs/getting-started/4.-connect-an-sdk/server-side-sdks/python-sdk)
```

### Comparing `fb-python-sdk-1.0.1/fb_python_sdk.egg-info/SOURCES.txt` & `fb-python-sdk-1.1.0/fb_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/__init__.py` & `fb-python-sdk-1.1.0/fbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/category.py` & `fb-python-sdk-1.1.0/fbclient/category.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/client.py` & `fb-python-sdk-1.1.0/fbclient/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import threading
-from distutils.util import strtobool
 from typing import Any, Mapping, Optional, Tuple
 
 from fbclient.category import FEATURE_FLAGS, SEGMENTS
-from fbclient.common_types import AllFlagStates, FBUser, FlagState, _EvalResult
+from fbclient.common_types import (AllFlagStates, EvalDetail, FBUser,
+                                   _EvalResult)
 from fbclient.config import Config
 from fbclient.data_storage import NullDataStorage
 from fbclient.evaluator import (REASON_CLIENT_NOT_READY, REASON_ERROR,
                                 REASON_FLAG_NOT_FOUND,
                                 REASON_USER_NOT_SPECIFIED, Evaluator)
 from fbclient.event_processor import DefaultEventProcessor, NullEventProcessor
 from fbclient.event_types import FlagEvent, Metric, MetricEvent, UserEvent
@@ -86,16 +86,16 @@
                                                               update_processor_ready)
         self._update_processor.start()
 
         if start_wait > 0:
             if not isinstance(self._update_processor, NullUpdateProcessor):
                 log.info("FB Python SDK: Waiting for Client initialization in %s seconds" % str(start_wait))
 
-            if isinstance(self._data_storage, NullDataStorage):
-                log.info("FB Python SDK: SDK just returns default variation")
+            if isinstance(self._data_storage, NullDataStorage) or not self._data_storage.initialized:
+                log.warning("FB Python SDK: SDK just returns default variation because of no data found in the given environment")
 
             update_processor_ready.wait(start_wait)
             if self._config.is_offline:
                 log.info("FB Python SDK: SDK is in offline mode")
             elif self._update_processor.initialized:
                 log.info("FB Python SDK: SDK initialization is completed")
             else:
@@ -175,15 +175,15 @@
         else:
             return default_value_type, str(default_value)
 
     def _evaluate_internal(self, key: str, user: dict, default: Any = None) -> _EvalResult:
         default_value_type, default_value = self.__handle_default_value(key, default)
         try:
             if not self.initialize:
-                log.warning('FB Python SDK: Evaluation called before Java SDK client initialized for feature flag, well using the default value')
+                log.warning('FB Python SDK: Evaluation called before SDK is initialized for feature flag, well using the default value')
                 return _EvalResult.error(default_value, REASON_CLIENT_NOT_READY, key, default_value_type)
 
             if not key:
                 log.warning('FB Python SDK: null feature flag key; returning default value')
                 return _EvalResult.error(default_value, REASON_FLAG_NOT_FOUND, key, default_value_type)
 
             flag = self._get_flag_internal(key)
@@ -207,108 +207,96 @@
             return _EvalResult.error(default_value, REASON_ERROR, key, default_value_type)
 
     def variation(self, key: str, user: dict, default: Any = None) -> Any:
         """Return the variation of a feature flag for a given user.
 
         This method will send an event back to feature flag center immediately if no error occurs.
 
+        The default value should be a string, boolean, numeric, or json type.
+
         The result of the flag evaluation will be converted to:
         1: string if the feature flag is a string type
         2: bool if the feature flag is a boolean type
-        3: Python object if the feature flag is a json type
-        4: float/int if the feature flag is a numeric type
+        3: float/int if the feature flag is a numeric type
+        4: Mapping or Iterable of any string, bool, float/int, or Mapping, if the feature flag is a json type
 
         :param key: the unique key for the feature flag
         :param user:  the attributes of the user
         :param default: the default value of the flag, to be used if the return value is not available
-        :return: one of the flag's values in any type in any type of string, bool, json(Python object), and float
+        :return: one of the flag's values in any type in any type of string, bool, float, json
         or the default value if flag evaluation fails
+        :raises: ValueError if the default is not a string, boolean, numeric, or json type
         """
         er = self._evaluate_internal(key, user, default)
         return cast_variation_by_flag_type(er.flag_type, er.value)
 
-    def variation_detail(self, key: str, user: dict, default: Any = None) -> FlagState:
+    def variation_detail(self, key: str, user: dict, default: Any = None) -> EvalDetail:
         """"Return the variation of a feature flag for a given user, but also provides additional information
-         about how this value was calculated, in the property `data` of the :class:`fbclient.common_types.FlagState`.
+         about how this value was calculated, in the property `data` of the :class:`fbclient.common_types.EvalDetail`.
 
         This method will send an event back to feature flag center immediately if no error occurs.
 
-        :param key: the unique key for the feature flag
-        :param user: the attributes of the user
-        :param default: the default value of the flag, to be used if the return value is not available
-        :return: an :class:`fbclient.common_types.FlagState` object
-        """
-        return self._evaluate_internal(key, user, default).to_flag_state
-
-    def is_enabled(self, key: str, user: dict) -> bool:
-        """
-        Return the bool value for a feature flag for a given user. it's strongly recommended to call this method
-        only in a bool feature flag, otherwise the results may not be what you expect
-
-        This method will send an event back to feature flag center immediately if no error occurs.
+        The default value should be a string, boolean, numeric, or json type.
 
         :param key: the unique key for the feature flag
         :param user: the attributes of the user
-        :return: True or False
-
+        :param default: the default value of the flag, to be used if the return value is not available
+        :return: an :class:`fbclient.common_types.EvalDetail` object
+        :raises: ValueError if the default is not a string, boolean, numeric, or json type
         """
-        try:
-            value = self.variation(key, user, False)
-            return bool(strtobool(str(value)))
-        except ValueError:
-            return False
+        return self._evaluate_internal(key, user, default).to_evail_detail
 
     def get_all_latest_flag_variations(self, user: dict) -> AllFlagStates:
         """
         Returns an object that encapsulates the state of all feature flags for a given user
 
         This method does not send events back to feature flag center immediately util calling :func:`fbcclient.common_types.AllFlagStates.get()`
 
         :param user: the attributes of the user
         :return: an :class:`fbcclient.common_types.AllFlagStates` object (will never be None; its `success` property will be False
         if SDK has not been initialized or the user invalid)
         """
         all_flag_details = {}
-        message = ""
+        reason = ""
         success = True
         try:
             if not self.initialize:
                 log.warning('FB Python SDK: Evaluation called before Java SDK client initialized for feature flag')
-                message = REASON_CLIENT_NOT_READY
+                reason = REASON_CLIENT_NOT_READY
                 success = False
             else:
                 try:
                     fb_user = FBUser.from_dict(user)
                     all_flags = self._data_storage.get_all(FEATURE_FLAGS)
                     for flag in all_flags.values():
                         fb_event = FlagEvent(fb_user)
                         er = self._evaluator.evaluate(flag, fb_user, fb_event)
                         all_flag_details[er.to_evail_detail] = fb_event
                 except ValueError as ve:
                     log.warning('FB Python SDK: %s' % str(ve))
-                    message = REASON_USER_NOT_SPECIFIED
+                    reason = REASON_USER_NOT_SPECIFIED
                     success = False
                 except:
                     raise
         except Exception as e:
             log.exception('FB Python SDK: unexpected error in evaluation: %s' % str(e))
-            message = REASON_ERROR
+            reason = REASON_ERROR
             success = False
-        return AllFlagStates(success, message, all_flag_details, self._event_handler)
+        return AllFlagStates(success, reason, all_flag_details, self._event_handler)
 
     def is_flag_known(self, key: str) -> bool:
         """
         Checks if the given flag exists in the your environment
 
         :param key: The key name of the flag to check
         :return: True if the flag exists
         """
         try:
             if not self.initialize:
-                log.warning('FB Python SDK: isFlagKnown called before Java SDK client initialized for feature flag')
+                log.warning('FB Python SDK: isFlagKnown called before SDK is initialized for feature flag')
                 return False
             return self._get_flag_internal(key) is not None
         except Exception as e:
             log.exception('FB Python SDK: unexpected error in is_flag_known: %s' % str(e))
         return False
 
     def flush(self):
```

### Comparing `fb-python-sdk-1.0.1/fbclient/common_types.py` & `fb-python-sdk-1.1.0/fbclient/common_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, Iterable, Mapping, Optional
+from typing import Any, Callable, Dict, Mapping, Optional
 
 from fbclient.utils import cast_variation_by_flag_type, is_numeric
 
 __BUILTINS_MAPING__ = {'key': 'keyid',
                        'name': 'name',
                        'keyid': 'keyid'}
 
 __NO_VARIATION__ = 'NE'
 
+__FLAG_NOT_FOUND__ = 'flag not found'
+
 __FLAG_KEY_UNKNOWN__ = 'flag key unknown'
 
 __FLAG_NAME_UNKNOWN__ = 'flag name unknown'
 
-__FLAG_VALUE_UNKNOWN__ = 'flag value unknown'
-
 
 class Jsonfy(ABC):
 
     @abstractmethod
     def to_json_dict(self) -> dict:
         pass
 
@@ -138,109 +138,108 @@
         return json_dict
 
 
 class BasicFlagState:
     """Abstract class representing flag state after feature flag evaluaion
     """
 
-    def __init__(self, success: bool, message: str):
+    def __init__(self, success: bool, reason: str):
         """Constructs an instance.
 
         :param success: True if successful
-        :param message: the state of last evaluation; the value is OK if successful
+        :param reason: the state of last evaluation; the value is OK if successful
         """
         self._success = success
-        self._message = 'OK' if success else message
+        self._reason = 'OK' if success else reason
 
     @property
     def success(self) -> bool:
         """Returns true if last evaluation was successful
         """
         return self._success
 
     @property
-    def message(self) -> str:
-        """Message representing the state of last evaluation; the value is OK if successful
+    def reason(self) -> str:
+        """reason the state of last evaluation; the value is OK if successful
         """
-        return self._message
+        return self._reason
 
 
 class FlagState(BasicFlagState, Jsonfy):
     """The object representing representing flag state of a given feature flag after feature flag evaluaion
     This object contains the information about how this flag vable was calculated in the property `data`
 
     The result of the flag evaluation should be converted to:
         1: string if the feature flag is a string type
         2: bool if the feature flag is a boolean type
         3: Python object if the feature flag is a json type
         4: float/int if the feature flag is a numeric type
     """
 
-    def __init__(self, success: bool, message: str, data: EvalDetail):
+    def __init__(self, success: bool, reason: str, data: EvalDetail):
         """Constructs an instance.
 
         :param success: True if successful
-        :param message: the state of last evaluation; the value is OK if successful
+        :param reason: the state of last evaluation; the value is OK if successful
         :param data: the result of a flag evaluation with information about how it was calculated
         """
-        super().__init__(success, message)
+        super().__init__(success, reason)
         self._data = data
 
     @property
     def data(self) -> EvalDetail:
         """return the result of a flag evaluation with information about how it was calculated"""
         return self._data
 
     def to_json_dict(self) -> dict:
         return {'success': self.success,
-                'message': self.message,
+                'reason': self.reason,
                 'data': self._data.to_json_dict() if self._data else None}
 
 
 class AllFlagStates(BasicFlagState, Jsonfy):
     """The object that encapsulates the state of all feature flags for a given user after feature flag evaluaion
     :func:`get(key_name)` to get the state for a given feature flag key
     """
 
-    def __init__(self, success: bool, message: str,
+    def __init__(self, success: bool, reason: str,
                  data: Mapping[EvalDetail, "FBEvent"],
                  event_handler: Callable[["FBEvent"], None]):
         """Constructs an instance.
 
         :param success: True if successful
-        :param message: the state of last evaluation; the value is OK if successful
-        :param data: a dictionary containing state of all feature flags and their events
+        :param reason: the state of last evaluation; the value is OK if successful
+        :param data: a dictionary containing latest evaluation of all feature flags and their events
         :event_handler: callback function used to send events to feature flag center
         """
-        super().__init__(success, message)
+        super().__init__(success, reason)
         self._data = dict((ed.key_name, (ed, fb_event)) for ed, fb_event in data.items()) if data else {}
         self._event_handler = event_handler
 
-    @property
-    def key_names(self) -> Iterable[Optional[str]]:
-        """Return key names of all feature flag
-        """
-        return self._data.keys()
-
-    def get(self, key_name: str) -> Optional[EvalDetail]:
+    def get(self, key_name: str, default: Any = None) -> EvalDetail:
         """Return the flag evaluation details of a given feature flag key
 
         This method will send event to back to feature flag center immediately
 
+        The default value should be a string, boolean, numeric, or json type.
+
         :param key_name: key name of the flag
         :return: an :class:`fbclient.common_types.EvalDetail` object
         """
         ed, fb_event = self._data.get(key_name, (None, False))
         if self._event_handler and fb_event:
             self._event_handler(fb_event)
-        return ed
+        return ed if ed is not None else EvalDetail(reason=__FLAG_NOT_FOUND__,
+                                                    variation=default,
+                                                    key_name=key_name,
+                                                    name=__FLAG_NAME_UNKNOWN__)
 
     def to_json_dict(self) -> dict:
         return {'success': self.success,
-                'message': self.message,
+                'message': self.reason,
                 'data': [ed.to_json_dict() for ed, _ in self._data.values()] if self._data else []}
 
 
 class FBEvent(Jsonfy, ABC):
     def __init__(self, user: "FBUser"):
         self._user = user
```

### Comparing `fb-python-sdk-1.0.1/fbclient/config.py` & `fb-python-sdk-1.1.0/fbclient/config.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/data_storage.py` & `fb-python-sdk-1.1.0/fbclient/data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/evaluator.py` & `fb-python-sdk-1.1.0/fbclient/evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/event_processor.py` & `fb-python-sdk-1.1.0/fbclient/event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/event_types.py` & `fb-python-sdk-1.1.0/fbclient/event_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/interfaces.py` & `fb-python-sdk-1.1.0/fbclient/interfaces.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/status.py` & `fb-python-sdk-1.1.0/fbclient/status.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/status_types.py` & `fb-python-sdk-1.1.0/fbclient/status_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/streaming.py` & `fb-python-sdk-1.1.0/fbclient/streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,8 +224,8 @@
             self.__self_closed = _SelfClosed(is_self_close=True, is_reconn=False, state=State.normal_off_state())
             self.__wsapp.close(status=WS_NORMAL_CLOSE)
         if self.__has_network:
             self.__ping_task.stop()
 
     @property
     def initialized(self) -> bool:
-        return self.__ready.is_set() and self.__storage.initialized
+        return self.__ready.is_set()
```

### Comparing `fb-python-sdk-1.0.1/fbclient/utils/__init__.py` & `fb-python-sdk-1.1.0/fbclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/utils/exponential_backoff_jitter_strategy.py` & `fb-python-sdk-1.1.0/fbclient/utils/exponential_backoff_jitter_strategy.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/utils/http_client.py` & `fb-python-sdk-1.1.0/fbclient/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/utils/repeatable_task.py` & `fb-python-sdk-1.1.0/fbclient/utils/repeatable_task.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/utils/rwlock.py` & `fb-python-sdk-1.1.0/fbclient/utils/rwlock.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/fbclient/utils/variation_splitting_algorithm.py` & `fb-python-sdk-1.1.0/fbclient/utils/variation_splitting_algorithm.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/intergration_tests/run_in_start_wait.py` & `fb-python-sdk-1.1.0/intergration_tests/run_in_start_wait.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fbclient.config import Config
 from fbclient.utils import log
 
 logging.basicConfig(level=logging.DEBUG,
                     format='%(asctime)s,%(msecs)d %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
                     datefmt='%m-%d %H:%M')
 
-env_secret = 'aM8NhGoaRUiADNLI-RO8Ug1mDiQeOD_kyUPu9s2DQBuw'
+env_secret = '9T0GABTXokagxhUZ81hUnws9_E2uOpIEyTjScBRr6JKA'
 
 config = Config(env_secret, event_url='http://localhost:5100', streaming_url='ws://localhost:5100')
 
 set_config(config)
 
 client = get()
 
@@ -23,16 +23,16 @@
     while True:
         line = input('input user key and flag key seperated by / \n')
         if 'exit' == line.strip():
             break
         try:
             user_key, flag_key, *_ = tuple(line.split('/'))
             user = {'key': user_key, 'name': user_key, 'country': 'cn'}
-            ffc_user = FBUser.from_dict(user)
-            log.info('FB Python SDK Test: user= %s' % ffc_user.to_json_str())
+            fb_user = FBUser.from_dict(user)
+            log.info('FB Python SDK Test: user= %s' % fb_user.to_json_str())
             t1 = time()
             log.info('FB Python SDK Test: variation= %s' % client.variation_detail(flag_key, user).to_json_str())
             t2 = time()
             log.info('FB Python SDK Test: execution time= %f' % (t2 - t1))
         except:
             log.exception('FB Python SDK Test: unexpected error')
             break
```

### Comparing `fb-python-sdk-1.0.1/setup.py` & `fb-python-sdk-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     extras_require={
         "dev": dev_reqs
     },
     tests_require=dev_reqs,
-    python_requires='>=3.6, <=3.10'
+    python_requires='>=3.6, <=3.11'
 )
```

### Comparing `fb-python-sdk-1.0.1/tests/test_data_storage.py` & `fb-python-sdk-1.1.0/tests/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/tests/test_data_update_status_provider.py` & `fb-python-sdk-1.1.0/tests/test_data_update_status_provider.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/tests/test_evaluator.py` & `fb-python-sdk-1.1.0/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/tests/test_event_processor.py` & `fb-python-sdk-1.1.0/tests/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.0.1/tests/test_fbclient.py` & `fb-python-sdk-1.1.0/tests/test_fbclient.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import base64
+from datetime import datetime
 from pathlib import Path
+from time import sleep
 from unittest.mock import patch
 
 import pytest
 
 from fbclient.client import FBClient
 from fbclient.config import Config
 from fbclient.data_storage import InMemoryDataStorage
@@ -93,105 +95,99 @@
 
 @patch.object(NullUpdateProcessor, "start")
 def test_start_and_nowait(mock_start_method):
     def start():
         pass
     mock_start_method.side_effect = start
     with make_fb_client(NullUpdateProcessor, NullEventProcessor, start_wait=0) as client:
+        assert not client.initialize
+        sleep(0.1)
         assert not client.update_status_provider.wait_for_OKState(timeout=0.1)
 
 
 @patch.object(NullUpdateProcessor, "start")
 def test_variation_when_client_not_initialized(mock_start_method):
     def start():
         pass
     mock_start_method.side_effect = start
     with make_fb_client(NullUpdateProcessor, NullEventProcessor, start_wait=0.1) as client:
         assert not client.initialize
-        flag_state = client.variation_detail("ff-test-bool", USER_1, False)
-        assert not flag_state.success
-        assert not flag_state.data.variation
-        assert flag_state.data.reason == REASON_CLIENT_NOT_READY
+        detail = client.variation_detail("ff-test-bool", USER_1, False)
+        assert detail.variation is False
+        assert detail.reason == REASON_CLIENT_NOT_READY
         all_states = client.get_all_latest_flag_variations(USER_1)  # type: ignore
         assert not all_states.success
-        assert all_states.message == REASON_CLIENT_NOT_READY
+        assert all_states.reason == REASON_CLIENT_NOT_READY
+        detail = all_states.get("ff-test-bool", False)
+        assert detail.variation is False
+        assert detail.reason == REASON_FLAG_NOT_FOUND
 
 
 def test_bool_variation():
     with make_fb_client_offline() as client:
         assert client.initialize
-        assert client.is_enabled("ff-test-bool", USER_1)
-        assert client.variation("ff-test-bool", USER_1, False)
-        flag_state = client.variation_detail("ff-test-bool", USER_2, False)
-        assert flag_state.success
-        assert flag_state.data.variation
-        assert flag_state.data.reason == REASON_TARGET_MATCH
-        assert not client.is_enabled("ff-test-bool", USER_3)
-        flag_state = client.variation_detail("ff-test-bool", USER_4, False)
-        assert flag_state.success
-        assert flag_state.data.variation
-        assert flag_state.data.reason == REASON_FALLTHROUGH
+        assert client.variation("ff-test-bool", USER_1, False) is True
+        detail = client.variation_detail("ff-test-bool", USER_2, False)
+        assert detail.variation is True
+        assert detail.reason == REASON_TARGET_MATCH
+        assert client.variation("ff-test-bool", USER_3, False) is False
+        detail = client.variation_detail("ff-test-bool", USER_4, False)
+        assert detail.variation is True
+        assert detail.reason == REASON_FALLTHROUGH
 
 
 def test_numeric_variation():
     with make_fb_client_offline() as client:
         assert client.initialize
         assert client.variation("ff-test-number", USER_1, -1) == 1
-        flag_state = client.variation_detail("ff-test-number", USER_2, -1)
-        assert flag_state.success
-        assert flag_state.data.variation == 33
-        assert flag_state.data.reason == REASON_RULE_MATCH
+        detail = client.variation_detail("ff-test-number", USER_2, -1)
+        assert detail.variation == 33
+        assert detail.reason == REASON_RULE_MATCH
         assert client.variation("ff-test-number", USER_3, -1) == 86
-        flag_state = client.variation_detail("ff-test-number", USER_4, -1)
-        assert flag_state.success
-        assert flag_state.data.variation == 9999
-        assert flag_state.data.reason == REASON_FALLTHROUGH
+        detail = client.variation_detail("ff-test-number", USER_4, -1)
+        assert detail.variation == 9999
+        assert detail.reason == REASON_FALLTHROUGH
 
 
 def test_string_variation():
     with make_fb_client_offline() as client:
         assert client.initialize
         assert client.variation("ff-test-string", USER_CN_PHONE_NUM, 'error') == 'phone number'
-        flag_state = client.variation_detail("ff-test-string", USER_FR_PHONE_NUM, 'error')
-        assert flag_state.success
-        assert flag_state.data.variation == 'phone number'
-        assert flag_state.data.reason == REASON_RULE_MATCH
+        detail = client.variation_detail("ff-test-string", USER_FR_PHONE_NUM, 'error')
+        assert detail.variation == 'phone number'
+        assert detail.reason == REASON_RULE_MATCH
         assert client.variation("ff-test-string", USER_EMAIL, 'error') == 'email'
-        flag_state = client.variation_detail("ff-test-string", USER_1, 'error')
-        assert flag_state.success
-        assert flag_state.data.variation == 'others'
-        assert flag_state.data.reason == REASON_FALLTHROUGH
+        detail = client.variation_detail("ff-test-string", USER_1, 'error')
+        assert detail.variation == 'others'
+        assert detail.reason == REASON_FALLTHROUGH
 
 
 def test_segment():
     with make_fb_client_offline() as client:
         assert client.initialize
         assert client.variation("ff-test-seg", USER_1, 'error') == 'teamA'
         assert client.variation("ff-test-seg", USER_2, 'error') == 'teamB'
-        flag_state = client.variation_detail("ff-test-seg", USER_3, 'error')
-        assert flag_state.success
-        assert flag_state.data.variation == 'teamA'
-        assert flag_state.data.reason == REASON_RULE_MATCH
-        flag_state = client.variation_detail("ff-test-seg", USER_4, 'error')
-        assert flag_state.success
-        assert flag_state.data.variation == 'teamB'
-        assert flag_state.data.reason == REASON_FALLTHROUGH
+        detail = client.variation_detail("ff-test-seg", USER_3, 'error')
+        assert detail.variation == 'teamA'
+        assert detail.reason == REASON_RULE_MATCH
+        detail = client.variation_detail("ff-test-seg", USER_4, 'error')
+        assert detail.variation == 'teamB'
+        assert detail.reason == REASON_FALLTHROUGH
 
 
 def test_json_variation():
     with make_fb_client_offline() as client:
         assert client.initialize
         json_object = client.variation("ff-test-json", USER_1, {})
         assert json_object["code"] == 200
         assert json_object["reason"] == "you win 100 euros"
-        flag_state = client.variation_detail("ff-test-json", USER_2, {})
-        assert flag_state.success
-        assert flag_state.data.variation["code"] == 404
-        assert flag_state.data.variation["reason"] == "fail to win the lottery"
-        assert flag_state.data.reason == REASON_FALLTHROUGH
+        detail = client.variation_detail("ff-test-json", USER_2, {})
+        assert detail.variation["code"] == 404
+        assert detail.variation["reason"] == "fail to win the lottery"
+        assert detail.reason == REASON_FALLTHROUGH
 
 
 def test_flag_known():
     with make_fb_client_offline() as client:
         assert client.initialize
         assert client.is_flag_known("ff-test-bool")
         assert client.is_flag_known("ff-test-number")
@@ -201,49 +197,56 @@
         assert not client.is_flag_known("ff-not-existed")
 
 
 def test_get_all_latest_flag_variations():
     with make_fb_client_offline() as client:
         assert client.initialize
         all_states = client.get_all_latest_flag_variations(USER_1)
-        ed = all_states.get("ff-test-bool")
-        assert ed is not None and ed.variation
-        ed = all_states.get("ff-test-number")
+        ed = all_states.get("ff-test-bool", False)
+        assert ed is not None and ed.variation is True
+        ed = all_states.get("ff-test-number", -1)
         assert ed is not None and ed.variation == 1
-        ed = all_states.get("ff-test-string")
+        ed = all_states.get("ff-test-string", 'error')
         assert ed is not None and ed.variation == "others"
-        ed = all_states.get("ff-test-seg")
+        ed = all_states.get("ff-test-seg", 'error')
         assert ed is not None and ed.variation == "teamA"
-        ed = all_states.get("ff-test-json")
+        ed = all_states.get("ff-test-json", {})
         assert ed is not None and ed.variation["code"] == 200
 
 
 def test_variation_argument_error():
     with make_fb_client_offline() as client:
         assert client.initialize
-        flag_state = client.variation_detail("ff-not-existed", USER_1, False)
-        assert not flag_state.success
-        assert not flag_state.data.variation
-        assert flag_state.data.reason == REASON_FLAG_NOT_FOUND
-        flag_state = client.variation_detail("ff-test-bool", None, False)  # type: ignore
-        assert not flag_state.success
-        assert not flag_state.data.variation
-        assert flag_state.data.reason == REASON_USER_NOT_SPECIFIED
+        detail = client.variation_detail("ff-not-existed", USER_1, False)
+        assert detail.variation is False
+        assert detail.reason == REASON_FLAG_NOT_FOUND
+        detail = client.variation_detail("ff-test-bool", None, None)  # type: ignore
+        assert detail.variation is None
+        assert detail.reason == REASON_USER_NOT_SPECIFIED
         all_states = client.get_all_latest_flag_variations(None)  # type: ignore
-        assert not all_states.success
-        assert all_states.message == REASON_USER_NOT_SPECIFIED
+        assert all_states.success is False
+        assert all_states.reason == REASON_USER_NOT_SPECIFIED
 
 
 @patch.object(InMemoryDataStorage, "get_all")
 @patch.object(InMemoryDataStorage, "get")
 def test_variation_unexpected_error(mock_get_method, mock_get_all_method):
     mock_get_method.side_effect = RuntimeError('test exception')
     mock_get_all_method.side_effect = RuntimeError('test exception')
     with make_fb_client_offline() as client:
         assert client.initialize
-        flag_state = client.variation_detail("ff-test-bool", USER_1, False)
-        assert not flag_state.success
-        assert not flag_state.data.variation
-        assert flag_state.data.reason == REASON_ERROR
+        detail = client.variation_detail("ff-test-bool", USER_1, False)
+        assert detail.variation is False
+        assert detail.reason == REASON_ERROR
         all_states = client.get_all_latest_flag_variations(USER_1)
         assert not all_states.success
-        assert all_states.message == REASON_ERROR
+        assert all_states.reason == REASON_ERROR
+
+
+def test_variation_error_default_value():
+    now = datetime.utcnow()
+    with make_fb_client_offline() as client:
+        assert client.initialize
+        with pytest.raises(ValueError):
+            client.variation_detail("ff-test-bool", USER_1, now)
+        with pytest.raises(ValueError):
+            client.variation("ff-test-bool", USER_1, now)
```

