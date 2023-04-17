# Comparing `tmp/rollbar-0.9.8.tar.gz` & `tmp/rollbar-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rollbar-0.9.8.tar", last modified: Fri Mar 13 17:54:37 2015, max compression
+gzip compressed data, was "dist/rollbar-0.9.9.tar", last modified: Fri Apr 10 22:59:13 2015, max compression
```

## Comparing `rollbar-0.9.8.tar` & `rollbar-0.9.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/
--rw-r--r--   0 coryvirok   (501) staff       (20)    16847 2015-03-13 17:54:37.000000 rollbar-0.9.8/PKG-INFO
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar/
--rw-r--r--   0 coryvirok   (501) staff       (20)    37670 2015-03-13 17:51:28.000000 rollbar-0.9.8/rollbar/__init__.py
--rw-r--r--   0 coryvirok   (501) staff       (20)     3018 2015-02-02 20:01:37.000000 rollbar-0.9.8/rollbar/cli.py
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar/contrib/
--rw-r--r--   0 coryvirok   (501) staff       (20)        0 2014-12-18 23:50:09.000000 rollbar-0.9.8/rollbar/contrib/__init__.py
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar/contrib/bottle/
--rw-r--r--   0 coryvirok   (501) staff       (20)     1096 2015-02-02 20:01:37.000000 rollbar-0.9.8/rollbar/contrib/bottle/__init__.py
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar/contrib/django/
--rw-r--r--   0 coryvirok   (501) staff       (20)      204 2015-02-02 20:01:37.000000 rollbar-0.9.8/rollbar/contrib/django/__init__.py
--rw-r--r--   0 coryvirok   (501) staff       (20)      696 2014-12-18 23:50:09.000000 rollbar-0.9.8/rollbar/contrib/django/context_processors.py
--rw-r--r--   0 coryvirok   (501) staff       (20)     4854 2015-02-02 20:01:37.000000 rollbar-0.9.8/rollbar/contrib/django/middleware.py
--rw-r--r--   0 coryvirok   (501) staff       (20)      106 2014-12-18 23:50:09.000000 rollbar-0.9.8/rollbar/contrib/django/models.py
--rw-r--r--   0 coryvirok   (501) staff       (20)      460 2014-12-18 23:50:09.000000 rollbar-0.9.8/rollbar/contrib/django/tests.py
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar/contrib/flask/
--rw-r--r--   0 coryvirok   (501) staff       (20)      315 2014-12-18 23:50:09.000000 rollbar-0.9.8/rollbar/contrib/flask/__init__.py
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar/contrib/pyramid/
--rw-r--r--   0 coryvirok   (501) staff       (20)     5054 2015-02-02 20:01:37.000000 rollbar-0.9.8/rollbar/contrib/pyramid/__init__.py
--rw-r--r--   0 coryvirok   (501) staff       (20)     5187 2015-02-02 20:01:37.000000 rollbar-0.9.8/rollbar/logger.py
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar/test/
--rw-r--r--   0 coryvirok   (501) staff       (20)     2270 2014-12-18 23:50:09.000000 rollbar-0.9.8/rollbar/test/__init__.py
--rw-r--r--   0 coryvirok   (501) staff       (20)     1303 2015-03-10 23:00:26.000000 rollbar-0.9.8/rollbar/test/test_loghandler.py
--rw-r--r--   0 coryvirok   (501) staff       (20)    30370 2015-03-13 17:48:12.000000 rollbar-0.9.8/rollbar/test/test_rollbar.py
-drwxr-xr-x   0 coryvirok   (501) staff       (20)        0 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar.egg-info/
--rw-r--r--   0 coryvirok   (501) staff       (20)        1 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar.egg-info/dependency_links.txt
--rw-r--r--   0 coryvirok   (501) staff       (20)      134 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar.egg-info/entry_points.txt
--rw-r--r--   0 coryvirok   (501) staff       (20)    16847 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar.egg-info/PKG-INFO
--rw-r--r--   0 coryvirok   (501) staff       (20)        8 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar.egg-info/requires.txt
--rw-r--r--   0 coryvirok   (501) staff       (20)      650 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar.egg-info/SOURCES.txt
--rw-r--r--   0 coryvirok   (501) staff       (20)        8 2015-03-13 17:54:37.000000 rollbar-0.9.8/rollbar.egg-info/top_level.txt
--rw-r--r--   0 coryvirok   (501) staff       (20)       59 2015-03-13 17:54:37.000000 rollbar-0.9.8/setup.cfg
--rw-r--r--   0 coryvirok   (501) staff       (20)     1808 2015-02-02 20:01:37.000000 rollbar-0.9.8/setup.py
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/
+-rw-rw-r--   0 brian     (1002) brian     (1002)     5187 2015-01-05 23:38:09.000000 rollbar-0.9.9/rollbar/logger.py
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/test/
+-rw-rw-r--   0 brian     (1002) brian     (1002)     1303 2014-08-20 23:30:13.000000 rollbar-0.9.9/rollbar/test/test_loghandler.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)     2270 2014-03-15 00:02:36.000000 rollbar-0.9.9/rollbar/test/__init__.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)    30370 2015-04-10 20:41:30.000000 rollbar-0.9.9/rollbar/test/test_rollbar.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)    37796 2015-04-10 22:54:23.000000 rollbar-0.9.9/rollbar/__init__.py
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/contrib/
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/contrib/bottle/
+-rw-rw-r--   0 brian     (1002) brian     (1002)     1096 2014-03-15 00:02:36.000000 rollbar-0.9.9/rollbar/contrib/bottle/__init__.py
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/contrib/flask/
+-rw-rw-r--   0 brian     (1002) brian     (1002)      315 2014-03-15 00:02:36.000000 rollbar-0.9.9/rollbar/contrib/flask/__init__.py
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/contrib/rq/
+-rw-rw-r--   0 brian     (1002) brian     (1002)     1668 2015-04-10 22:53:56.000000 rollbar-0.9.9/rollbar/contrib/rq/__init__.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)        0 2013-02-23 01:29:59.000000 rollbar-0.9.9/rollbar/contrib/__init__.py
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/contrib/pyramid/
+-rw-rw-r--   0 brian     (1002) brian     (1002)     5054 2014-03-15 00:02:36.000000 rollbar-0.9.9/rollbar/contrib/pyramid/__init__.py
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar/contrib/django/
+-rw-rw-r--   0 brian     (1002) brian     (1002)      460 2013-02-23 01:29:59.000000 rollbar-0.9.9/rollbar/contrib/django/tests.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)      204 2014-08-19 03:23:11.000000 rollbar-0.9.9/rollbar/contrib/django/__init__.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)      106 2013-02-23 01:29:59.000000 rollbar-0.9.9/rollbar/contrib/django/models.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)     4854 2014-03-15 00:02:36.000000 rollbar-0.9.9/rollbar/contrib/django/middleware.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)      696 2013-02-23 01:29:59.000000 rollbar-0.9.9/rollbar/contrib/django/context_processors.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)     3018 2014-03-15 00:02:36.000000 rollbar-0.9.9/rollbar/cli.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)     1808 2014-11-26 22:02:36.000000 rollbar-0.9.9/setup.py
+-rw-rw-r--   0 brian     (1002) brian     (1002)       59 2015-04-10 22:59:12.000000 rollbar-0.9.9/setup.cfg
+drwxrwxr-x   0 brian     (1002) brian     (1002)        0 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar.egg-info/
+-rw-rw-r--   0 brian     (1002) brian     (1002)      134 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar.egg-info/entry_points.txt
+-rw-rw-r--   0 brian     (1002) brian     (1002)        1 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1002) brian     (1002)      681 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1002) brian     (1002)        8 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1002) brian     (1002)        8 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar.egg-info/top_level.txt
+-rw-rw-r--   0 brian     (1002) brian     (1002)    16847 2015-04-10 22:59:12.000000 rollbar-0.9.9/rollbar.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1002) brian     (1002)    16847 2015-04-10 22:59:12.000000 rollbar-0.9.9/PKG-INFO
```

### Comparing `rollbar-0.9.8/PKG-INFO` & `rollbar-0.9.9/rollbar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: rollbar
-Version: 0.9.8
+Version: 0.9.9
 Summary: Logs exceptions and other data to Rollbar. Provides a generic interface, as well as a Django middleware and a Pyramid tween.
 Home-page: http://github.com/rollbar/pyrollbar
 Author: Rollbar, Inc.
 Author-email: support@rollbar.com
 License: UNKNOWN
-Description: # Rollbar notifier for Python [![Build Status](https://travis-ci.org/rollbar/pyrollbar.png?branch=v0.9.6)](https://travis-ci.org/rollbar/pyrollbar) [![codecov.io](https://codecov.io/github/rollbar/pyrollbar/coverage.svg?branch=master)](https://codecov.io/github/rollbar/pyrollbar?branch=master)
+Description: # Rollbar notifier for Python [![Build Status](https://travis-ci.org/rollbar/pyrollbar.png?branch=v0.9.9)](https://travis-ci.org/rollbar/pyrollbar) [![codecov.io](https://codecov.io/github/rollbar/pyrollbar/coverage.svg?branch=master)](https://codecov.io/github/rollbar/pyrollbar?branch=master)
         
         <!-- RemoveNext -->
         Python notifier for reporting exceptions, errors, and log messages to [Rollbar](https://rollbar.com).
         
         <!-- Sub:[TOC] -->
         
         ## Quick start
```

### Comparing `rollbar-0.9.8/rollbar/__init__.py` & `rollbar-0.9.9/rollbar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Plugin for Pyramid apps to submit errors to Rollbar
 """
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 
 import copy
 import inspect
 import json
 import logging
+import os
 import socket
 import sys
 import threading
 import time
 import traceback
 import types
 import urllib
@@ -500,14 +501,15 @@
                 'class': cls.__name__,
                 'message': _to_str(exc),
             }
         }
     }
 
     if extra_data:
+        extra_data = _scrub_obj(extra_data)
         if isinstance(extra_data, dict):
             data['custom'] = extra_data
         else:
             data['custom'] = {'value': extra_data}
 
     _add_locals_data(data, exc_info)
     _add_request_data(data, request)
@@ -536,14 +538,15 @@
     data['body'] = {
         'message': {
             'body': message
         }
     }
 
     if extra_data:
+        extra_data = _scrub_obj(extra_data)
         data['body']['message'].update(extra_data)
 
     _add_request_data(data, request)
     _add_person_data(data, request)
     data['server'] = _build_server_data()
 
     if payload_data:
@@ -1045,15 +1048,16 @@
 def _build_server_data():
     """
     Returns a dictionary containing information about the server environment.
     """
     # server environment
     server_data = {
         'host': socket.gethostname(),
-        'argv': sys.argv
+        'argv': sys.argv,
+        'pid': os.getpid()
     }
 
     for key in ['branch', 'root']:
         if SETTINGS.get(key):
             server_data[key] = SETTINGS[key]
 
     return server_data
```

### Comparing `rollbar-0.9.8/rollbar/cli.py` & `rollbar-0.9.9/rollbar/cli.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/contrib/bottle/__init__.py` & `rollbar-0.9.9/rollbar/contrib/bottle/__init__.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/contrib/django/context_processors.py` & `rollbar-0.9.9/rollbar/contrib/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/contrib/django/middleware.py` & `rollbar-0.9.9/rollbar/contrib/django/middleware.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/contrib/pyramid/__init__.py` & `rollbar-0.9.9/rollbar/contrib/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/logger.py` & `rollbar-0.9.9/rollbar/logger.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/test/__init__.py` & `rollbar-0.9.9/rollbar/test/__init__.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/test/test_loghandler.py` & `rollbar-0.9.9/rollbar/test/test_loghandler.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar/test/test_rollbar.py` & `rollbar-0.9.9/rollbar/test/test_rollbar.py`

 * *Files identical despite different names*

### Comparing `rollbar-0.9.8/rollbar.egg-info/PKG-INFO` & `rollbar-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: rollbar
-Version: 0.9.8
+Version: 0.9.9
 Summary: Logs exceptions and other data to Rollbar. Provides a generic interface, as well as a Django middleware and a Pyramid tween.
 Home-page: http://github.com/rollbar/pyrollbar
 Author: Rollbar, Inc.
 Author-email: support@rollbar.com
 License: UNKNOWN
-Description: # Rollbar notifier for Python [![Build Status](https://travis-ci.org/rollbar/pyrollbar.png?branch=v0.9.6)](https://travis-ci.org/rollbar/pyrollbar) [![codecov.io](https://codecov.io/github/rollbar/pyrollbar/coverage.svg?branch=master)](https://codecov.io/github/rollbar/pyrollbar?branch=master)
+Description: # Rollbar notifier for Python [![Build Status](https://travis-ci.org/rollbar/pyrollbar.png?branch=v0.9.9)](https://travis-ci.org/rollbar/pyrollbar) [![codecov.io](https://codecov.io/github/rollbar/pyrollbar/coverage.svg?branch=master)](https://codecov.io/github/rollbar/pyrollbar?branch=master)
         
         <!-- RemoveNext -->
         Python notifier for reporting exceptions, errors, and log messages to [Rollbar](https://rollbar.com).
         
         <!-- Sub:[TOC] -->
         
         ## Quick start
```

### Comparing `rollbar-0.9.8/rollbar.egg-info/SOURCES.txt` & `rollbar-0.9.9/rollbar.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 rollbar/contrib/django/__init__.py
 rollbar/contrib/django/context_processors.py
 rollbar/contrib/django/middleware.py
 rollbar/contrib/django/models.py
 rollbar/contrib/django/tests.py
 rollbar/contrib/flask/__init__.py
 rollbar/contrib/pyramid/__init__.py
+rollbar/contrib/rq/__init__.py
 rollbar/test/__init__.py
 rollbar/test/test_loghandler.py
 rollbar/test/test_rollbar.py
```

### Comparing `rollbar-0.9.8/setup.py` & `rollbar-0.9.9/setup.py`

 * *Files identical despite different names*

