# Comparing `tmp/happydomain-0.0.6.tar.gz` & `tmp/happydomain-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happydomain-0.0.6.tar", last modified: Thu Apr 13 15:19:58 2023, max compression
+gzip compressed data, was "happydomain-0.0.7.tar", last modified: Mon Apr 17 10:32:07 2023, max compression
```

## Comparing `happydomain-0.0.6.tar` & `happydomain-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:19:58.805650 happydomain-0.0.6/
--rw-r--r--   0 root         (0) root         (0)    21781 2023-04-13 15:19:50.000000 happydomain-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 15:19:58.805650 happydomain-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-13 15:19:50.000000 happydomain-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:19:58.793651 happydomain-0.0.6/happydomain/
--rw-r--r--   0 root         (0) root         (0)     1667 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/admin.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/api.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/authuser.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/domain.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/error.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/provider.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/service.py
--rw-r--r--   0 root         (0) root         (0)     3699 2023-04-13 15:19:50.000000 happydomain-0.0.6/happydomain/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 15:19:58.801650 happydomain-0.0.6/happydomain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1042 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      413 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 15:19:58.000000 happydomain-0.0.6/happydomain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-13 15:19:50.000000 happydomain-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 15:19:58.805650 happydomain-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 15:19:50.000000 happydomain-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:32:07.138746 happydomain-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)    21781 2023-04-17 10:31:18.000000 happydomain-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-17 10:32:07.134746 happydomain-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-17 10:31:18.000000 happydomain-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:32:07.122747 happydomain-0.0.7/happydomain/
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/admin.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/api.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/authuser.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/domain.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/error.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/provider.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/service.py
+-rw-r--r--   0 root         (0) root         (0)     3699 2023-04-17 10:31:18.000000 happydomain-0.0.7/happydomain/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 10:32:07.134746 happydomain-0.0.7/happydomain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 10:32:06.000000 happydomain-0.0.7/happydomain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-17 10:31:18.000000 happydomain-0.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 10:32:07.138746 happydomain-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-17 10:31:18.000000 happydomain-0.0.7/setup.py
```

### Comparing `happydomain-0.0.6/LICENSE` & `happydomain-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/PKG-INFO` & `happydomain-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.6/happydomain/__init__.py` & `happydomain-0.0.7/happydomain/__init__.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/happydomain/admin.py` & `happydomain-0.0.7/happydomain/admin.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/happydomain/api.py` & `happydomain-0.0.7/happydomain/api.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/happydomain/authuser.py` & `happydomain-0.0.7/happydomain/authuser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 from urllib.parse import quote
 
+from .api import HappyError
+
 class AuthUser:
 
     def __init__(self, _session, Id, Email, EmailVerification, Password, CreatedAt, LastLoggedIn, AllowCommercials):
         self._session = _session
 
         self.Id = Id
         self.Email = Email
```

### Comparing `happydomain-0.0.6/happydomain/domain.py` & `happydomain-0.0.7/happydomain/domain.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/happydomain/provider.py` & `happydomain-0.0.7/happydomain/provider.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/happydomain/service.py` & `happydomain-0.0.7/happydomain/service.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/happydomain/zone.py` & `happydomain-0.0.7/happydomain/zone.py`

 * *Files identical despite different names*

### Comparing `happydomain-0.0.6/happydomain.egg-info/PKG-INFO` & `happydomain-0.0.7/happydomain.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happydomain
-Version: 0.0.6
+Version: 0.0.7
 Summary: Finally a simple interface for domain names.
 Home-page: https://git.happydomain.org/python-sdk
 Author: happyDomain's team
 Author-email: happyDomain's team <contact+pypi@happydomain.org>
 License: CECILL-2.1
 Project-URL: Homepage, https://git.happydomain.org/python-sdk
 Project-URL: Bug Tracker, https://git.happydomain.org/python-sdk/issues
```

### Comparing `happydomain-0.0.6/pyproject.toml` & `happydomain-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "happydomain"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="happyDomain's team", email="contact+pypi@happydomain.org" },
 ]
 description = "Finally a simple interface for domain names."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `happydomain-0.0.6/setup.py` & `happydomain-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from glob import glob
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.0.6"
+version = "0.0.7"
 
 setup(
     name = "happydomain",
     version = version,
     description = "Finally a simple interface for domain names.",
     long_description = open('README.md').read(),
```

