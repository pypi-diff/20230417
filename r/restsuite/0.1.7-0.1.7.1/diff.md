# Comparing `tmp/restsuite-0.1.7.tar.gz` & `tmp/restsuite-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restsuite-0.1.7.tar", last modified: Wed Mar 29 23:03:41 2023, max compression
+gzip compressed data, was "restsuite-0.1.7.1.tar", last modified: Mon Apr 17 21:14:03 2023, max compression
```

## Comparing `restsuite-0.1.7.tar` & `restsuite-0.1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-03-29 23:03:41.903967 restsuite-0.1.7/
--rw-r--r--   0 peterwilliams   (501) staff       (20)     1070 2023-01-10 22:48:18.000000 restsuite-0.1.7/LICENSE
--rw-r--r--   0 peterwilliams   (501) staff       (20)     9435 2023-03-29 23:03:41.903685 restsuite-0.1.7/PKG-INFO
--rw-r--r--   0 peterwilliams   (501) staff       (20)     7583 2023-01-18 21:17:16.000000 restsuite-0.1.7/README.md
--rw-r--r--   0 peterwilliams   (501) staff       (20)      801 2023-03-29 23:01:26.000000 restsuite-0.1.7/pyproject.toml
-drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-03-29 23:03:41.902703 restsuite-0.1.7/restsuite/
--rw-r--r--   0 peterwilliams   (501) staff       (20)       86 2023-01-10 17:43:57.000000 restsuite-0.1.7/restsuite/__init__.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)    13271 2023-02-02 14:13:32.000000 restsuite-0.1.7/restsuite/auth.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     7978 2023-01-18 21:38:29.000000 restsuite-0.1.7/restsuite/base_rest.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     2527 2023-01-10 21:32:14.000000 restsuite-0.1.7/restsuite/rest.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     6626 2023-01-13 20:33:33.000000 restsuite-0.1.7/restsuite/restlet.py
--rw-r--r--   0 peterwilliams   (501) staff       (20)     4442 2023-03-29 23:02:43.000000 restsuite-0.1.7/restsuite/suiteql.py
-drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-03-29 23:03:41.903519 restsuite-0.1.7/restsuite.egg-info/
--rw-r--r--   0 peterwilliams   (501) staff       (20)     9435 2023-03-29 23:03:41.000000 restsuite-0.1.7/restsuite.egg-info/PKG-INFO
--rw-r--r--   0 peterwilliams   (501) staff       (20)      319 2023-03-29 23:03:41.000000 restsuite-0.1.7/restsuite.egg-info/SOURCES.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)        1 2023-03-29 23:03:41.000000 restsuite-0.1.7/restsuite.egg-info/dependency_links.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)        9 2023-03-29 23:03:41.000000 restsuite-0.1.7/restsuite.egg-info/requires.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)       10 2023-03-29 23:03:41.000000 restsuite-0.1.7/restsuite.egg-info/top_level.txt
--rw-r--r--   0 peterwilliams   (501) staff       (20)       38 2023-03-29 23:03:41.904003 restsuite-0.1.7/setup.cfg
+drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-04-17 21:14:03.067467 restsuite-0.1.7.1/
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     1070 2023-01-10 22:48:18.000000 restsuite-0.1.7.1/LICENSE
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     9437 2023-04-17 21:14:03.067279 restsuite-0.1.7.1/PKG-INFO
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     7583 2023-01-18 21:17:16.000000 restsuite-0.1.7.1/README.md
+-rw-r--r--   0 peterwilliams   (501) staff       (20)      803 2023-04-17 21:13:56.000000 restsuite-0.1.7.1/pyproject.toml
+drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-04-17 21:14:03.066306 restsuite-0.1.7.1/restsuite/
+-rw-r--r--   0 peterwilliams   (501) staff       (20)       86 2023-01-10 17:43:57.000000 restsuite-0.1.7.1/restsuite/__init__.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)    13271 2023-02-02 14:13:32.000000 restsuite-0.1.7.1/restsuite/auth.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     7978 2023-01-18 21:38:29.000000 restsuite-0.1.7.1/restsuite/base_rest.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     2527 2023-01-10 21:32:14.000000 restsuite-0.1.7.1/restsuite/rest.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     6626 2023-01-13 20:33:33.000000 restsuite-0.1.7.1/restsuite/restlet.py
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     4455 2023-04-17 21:12:25.000000 restsuite-0.1.7.1/restsuite/suiteql.py
+drwxr-xr-x   0 peterwilliams   (501) staff       (20)        0 2023-04-17 21:14:03.067104 restsuite-0.1.7.1/restsuite.egg-info/
+-rw-r--r--   0 peterwilliams   (501) staff       (20)     9437 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/PKG-INFO
+-rw-r--r--   0 peterwilliams   (501) staff       (20)      319 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/SOURCES.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)        1 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/dependency_links.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)        9 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/requires.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)       10 2023-04-17 21:14:03.000000 restsuite-0.1.7.1/restsuite.egg-info/top_level.txt
+-rw-r--r--   0 peterwilliams   (501) staff       (20)       38 2023-04-17 21:14:03.067516 restsuite-0.1.7.1/setup.cfg
```

### Comparing `restsuite-0.1.7/LICENSE` & `restsuite-0.1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7/PKG-INFO` & `restsuite-0.1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsuite
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Easily work with Netsuite's REST API
 Author: Peter Williams, Richard Demke, Andy Gannaway
 Author-email: Peter Williams <petercw94@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Williams
```

### Comparing `restsuite-0.1.7/README.md` & `restsuite-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7/pyproject.toml` & `restsuite-0.1.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "restsuite"
-version = "0.1.7"
+version = "0.1.7.1"
 description = "Easily work with Netsuite's REST API"
 readme = "README.md"
 authors = [
     {name="Peter Williams", email="petercw94@gmail.com"},
     {name="Peter Williams"},
     {name="Richard Demke"},
     {name="Andy Gannaway"}
```

### Comparing `restsuite-0.1.7/restsuite/auth.py` & `restsuite-0.1.7.1/restsuite/auth.py`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7/restsuite/base_rest.py` & `restsuite-0.1.7.1/restsuite/base_rest.py`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7/restsuite/rest.py` & `restsuite-0.1.7.1/restsuite/rest.py`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7/restsuite/restlet.py` & `restsuite-0.1.7.1/restsuite/restlet.py`

 * *Files identical despite different names*

### Comparing `restsuite-0.1.7/restsuite/suiteql.py` & `restsuite-0.1.7.1/restsuite/suiteql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Module for making SuiteQL queries
 """
 
+import json
+
 from .auth import NetsuiteOAuth
 import requests
 
 
 class NetSuiteQL:
     """
     """
@@ -34,15 +36,15 @@
 
         Returns:
         -------
         - response (obj) -> requests.response object from POST request.
 
         """
 
-        body = '{"q": "' + query_string + '"}'
+        body = json.dumps({"q": query_string})
 
         headers = self.auth.generate_auth_header("POST", url)
 
         response = requests.post(url, headers=headers, data=body, cookies={
                                  'NS_ROUTING_VERSION': 'LAGGING'})
 
         return response
```

### Comparing `restsuite-0.1.7/restsuite.egg-info/PKG-INFO` & `restsuite-0.1.7.1/restsuite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restsuite
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: Easily work with Netsuite's REST API
 Author: Peter Williams, Richard Demke, Andy Gannaway
 Author-email: Peter Williams <petercw94@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Williams
```

