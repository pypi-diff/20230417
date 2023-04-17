# Comparing `tmp/mythic-0.1.0rc3.tar.gz` & `tmp/mythic-0.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.0rc3.tar", last modified: Thu Apr  6 15:01:43 2023, max compression
+gzip compressed data, was "mythic-0.1.0rc4.tar", last modified: Mon Apr 17 15:37:19 2023, max compression
```

## Comparing `mythic-0.1.0rc3.tar` & `mythic-0.1.0rc4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-06 15:01:43.364386 mythic-0.1.0rc3/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-06 15:01:43.364003 mythic-0.1.0rc3/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc3/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-06 15:01:43.361692 mythic-0.1.0rc3/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc3/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc3/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    94328 2023-04-06 14:43:47.000000 mythic-0.1.0rc3/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3623 2023-04-06 15:00:49.000000 mythic-0.1.0rc3/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc3/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc3/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-06 15:01:43.363529 mythic-0.1.0rc3/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-06 15:01:43.000000 mythic-0.1.0rc3/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-06 15:01:43.000000 mythic-0.1.0rc3/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-06 15:01:43.000000 mythic-0.1.0rc3/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-06 15:01:43.000000 mythic-0.1.0rc3/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-06 15:01:43.000000 mythic-0.1.0rc3/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-06 15:01:43.364503 mythic-0.1.0rc3/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-06 14:47:24.000000 mythic-0.1.0rc3/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-17 15:37:19.307404 mythic-0.1.0rc4/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-17 15:37:19.306962 mythic-0.1.0rc4/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc4/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-17 15:37:19.303799 mythic-0.1.0rc4/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc4/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc4/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    94328 2023-04-06 14:43:47.000000 mythic-0.1.0rc4/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3623 2023-04-17 15:37:03.000000 mythic-0.1.0rc4/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc4/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc4/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-17 15:37:19.306357 mythic-0.1.0rc4/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-17 15:37:19.000000 mythic-0.1.0rc4/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-17 15:37:19.000000 mythic-0.1.0rc4/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-17 15:37:19.000000 mythic-0.1.0rc4/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-17 15:37:19.000000 mythic-0.1.0rc4/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-17 15:37:19.000000 mythic-0.1.0rc4/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-17 15:37:19.307577 mythic-0.1.0rc4/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-17 15:35:51.000000 mythic-0.1.0rc4/setup.py
```

### Comparing `mythic-0.1.0rc3/PKG-INFO` & `mythic-0.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc3/README.md` & `mythic-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc3/mythic/graphql_queries.py` & `mythic-0.1.0rc4/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc3/mythic/mythic.py` & `mythic-0.1.0rc4/mythic/mythic.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc3/mythic/mythic_classes.py` & `mythic-0.1.0rc4/mythic/mythic_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.server_ip = server_ip
         self.server_port = server_port
         self.server_api_version = server_api_version
         self.ssl = ssl
         self.http = "http://" if not ssl else "https://"
         self.ws = "ws://" if not ssl else "wss://"
         self.global_timeout = global_timeout if global_timeout is not None else -1
-        self.scripting_version = "0.1.0rc3"
+        self.scripting_version = "0.1.0rc4"
         self.current_operation_id = 0
         self.operator_id = None
         self.operator = None
         self.schema = schema
 
     def __str__(self):
         return json.dumps(
```

### Comparing `mythic-0.1.0rc3/mythic/mythic_utilities.py` & `mythic-0.1.0rc4/mythic/mythic_utilities.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc3/mythic.egg-info/PKG-INFO` & `mythic-0.1.0rc4/mythic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc3/setup.py` & `mythic-0.1.0rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.0rc3",
+    version="0.1.0rc4",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

