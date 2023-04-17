# Comparing `tmp/tutti-client-0.3.7.tar.gz` & `tmp/tutti-client-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutti-client-0.3.7.tar", last modified: Mon Apr 17 03:09:42 2023, max compression
+gzip compressed data, was "tutti-client-0.3.8.tar", last modified: Mon Apr 17 06:22:44 2023, max compression
```

## Comparing `tutti-client-0.3.7.tar` & `tutti-client-0.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kenshiroueda   (501) staff       (20)        0 2023-04-17 03:09:42.108179 tutti-client-0.3.7/
--rw-r--r--   0 kenshiroueda   (501) staff       (20)    11357 2022-10-20 05:46:51.000000 tutti-client-0.3.7/LICENSE.txt
--rw-r--r--   0 kenshiroueda   (501) staff       (20)      133 2022-10-20 05:46:51.000000 tutti-client-0.3.7/MANIFEST.in
--rw-r--r--   0 kenshiroueda   (501) staff       (20)     5884 2023-04-17 03:09:42.108386 tutti-client-0.3.7/PKG-INFO
--rw-r--r--   0 kenshiroueda   (501) staff       (20)     5115 2022-10-20 05:46:51.000000 tutti-client-0.3.7/README.md
--rw-r--r--   0 kenshiroueda   (501) staff       (20)      320 2022-10-31 13:24:59.000000 tutti-client-0.3.7/pyproject.toml
--rw-r--r--   0 kenshiroueda   (501) staff       (20)      107 2023-04-17 03:09:42.109049 tutti-client-0.3.7/setup.cfg
--rw-r--r--   0 kenshiroueda   (501) staff       (20)     8764 2023-04-14 11:49:15.000000 tutti-client-0.3.7/setup.py
-drwxr-xr-x   0 kenshiroueda   (501) staff       (20)        0 2023-04-17 03:09:42.104900 tutti-client-0.3.7/tutti_client/
--rw-r--r--   0 kenshiroueda   (501) staff       (20)       21 2022-10-20 05:46:51.000000 tutti-client-0.3.7/tutti_client/__init__.py
--rw-r--r--   0 kenshiroueda   (501) staff       (20)    32392 2023-04-14 11:48:52.000000 tutti-client-0.3.7/tutti_client/controller.py
--rw-r--r--   0 kenshiroueda   (501) staff       (20)      154 2022-10-20 05:46:51.000000 tutti-client-0.3.7/tutti_client/error.py
--rw-r--r--   0 kenshiroueda   (501) staff       (20)    10707 2022-10-20 05:46:51.000000 tutti-client-0.3.7/tutti_client/listener.py
--rw-r--r--   0 kenshiroueda   (501) staff       (20)     3672 2022-10-20 05:46:51.000000 tutti-client-0.3.7/tutti_client/tutti.py
-drwxr-xr-x   0 kenshiroueda   (501) staff       (20)        0 2023-04-17 03:09:42.107803 tutti-client-0.3.7/tutti_client.egg-info/
--rw-r--r--   0 kenshiroueda   (501) staff       (20)     5884 2023-04-17 03:09:42.000000 tutti-client-0.3.7/tutti_client.egg-info/PKG-INFO
--rw-r--r--   0 kenshiroueda   (501) staff       (20)      367 2023-04-17 03:09:42.000000 tutti-client-0.3.7/tutti_client.egg-info/SOURCES.txt
--rw-r--r--   0 kenshiroueda   (501) staff       (20)        1 2023-04-17 03:09:42.000000 tutti-client-0.3.7/tutti_client.egg-info/dependency_links.txt
--rw-r--r--   0 kenshiroueda   (501) staff       (20)       20 2023-04-17 03:09:42.000000 tutti-client-0.3.7/tutti_client.egg-info/requires.txt
--rw-r--r--   0 kenshiroueda   (501) staff       (20)       13 2023-04-17 03:09:42.000000 tutti-client-0.3.7/tutti_client.egg-info/top_level.txt
+drwxr-xr-x   0 kenshiroueda   (501) staff       (20)        0 2023-04-17 06:22:44.693932 tutti-client-0.3.8/
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)    11357 2022-10-20 05:46:51.000000 tutti-client-0.3.8/LICENSE.txt
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)      133 2022-10-20 05:46:51.000000 tutti-client-0.3.8/MANIFEST.in
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)     5884 2023-04-17 06:22:44.694189 tutti-client-0.3.8/PKG-INFO
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)     5115 2022-10-20 05:46:51.000000 tutti-client-0.3.8/README.md
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)      320 2022-10-31 13:24:59.000000 tutti-client-0.3.8/pyproject.toml
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)      107 2023-04-17 06:22:44.694799 tutti-client-0.3.8/setup.cfg
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)     8764 2023-04-17 06:22:27.000000 tutti-client-0.3.8/setup.py
+drwxr-xr-x   0 kenshiroueda   (501) staff       (20)        0 2023-04-17 06:22:44.691252 tutti-client-0.3.8/tutti_client/
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)       21 2022-10-20 05:46:51.000000 tutti-client-0.3.8/tutti_client/__init__.py
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)    32300 2023-04-17 06:21:59.000000 tutti-client-0.3.8/tutti_client/controller.py
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)      154 2022-10-20 05:46:51.000000 tutti-client-0.3.8/tutti_client/error.py
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)    10707 2022-10-20 05:46:51.000000 tutti-client-0.3.8/tutti_client/listener.py
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)     3672 2022-10-20 05:46:51.000000 tutti-client-0.3.8/tutti_client/tutti.py
+drwxr-xr-x   0 kenshiroueda   (501) staff       (20)        0 2023-04-17 06:22:44.693504 tutti-client-0.3.8/tutti_client.egg-info/
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)     5884 2023-04-17 06:22:44.000000 tutti-client-0.3.8/tutti_client.egg-info/PKG-INFO
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)      367 2023-04-17 06:22:44.000000 tutti-client-0.3.8/tutti_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)        1 2023-04-17 06:22:44.000000 tutti-client-0.3.8/tutti_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)       20 2023-04-17 06:22:44.000000 tutti-client-0.3.8/tutti_client.egg-info/requires.txt
+-rw-r--r--   0 kenshiroueda   (501) staff       (20)       13 2023-04-17 06:22:44.000000 tutti-client-0.3.8/tutti_client.egg-info/top_level.txt
```

### Comparing `tutti-client-0.3.7/LICENSE.txt` & `tutti-client-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutti-client-0.3.7/PKG-INFO` & `tutti-client-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutti-client
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python client library for Tutti.ai
 Home-page: https://github.com/iflb/tutti-client-python
 Author: Intelligent Framework Lab
 Author-email: saito@iflab.tokyo
 Project-URL: Project Owner, http://www.pcl.cs.waseda.ac.jp/
 Project-URL: Funding, https://www.waseda.jp/inst/gcs/news/2019/11/29/870/
 Keywords: crowdsourcing annotation framework asyncio
```

### Comparing `tutti-client-0.3.7/README.md` & `tutti-client-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `tutti-client-0.3.7/setup.py` & `tutti-client-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.3.7',  # Required
+    version='0.3.8',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     #description='Ingenious Framework for Configuration',  # Optional
     description='Python client library for Tutti.ai',  # Optional
```

### Comparing `tutti-client-0.3.7/tutti_client/controller.py` & `tutti-client-0.3.8/tutti_client/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,20 +91,18 @@
                     'user_name': user_name,
                     'password_hash': password_hash,
                     'access_token': access_token
                 },
                 called = called
             )
 
-    async def sign_out(self, access_token: str = None, called = True):
+    async def sign_out(self, called = True):
         return await self._call_or_send(
                 self._duct.EVENT['AUTHENTICATION_SIGN_OUT'],
-                {
-                    'access_token': access_token
-                },
+                {},
                 called = called
             )
 
     async def get_user_ids(self, called = True):
         """Requests a list of available internal user IDs.
         """
         return await self._call_or_send(
```

### Comparing `tutti-client-0.3.7/tutti_client/listener.py` & `tutti-client-0.3.8/tutti_client/listener.py`

 * *Files identical despite different names*

### Comparing `tutti-client-0.3.7/tutti_client/tutti.py` & `tutti-client-0.3.8/tutti_client/tutti.py`

 * *Files identical despite different names*

### Comparing `tutti-client-0.3.7/tutti_client.egg-info/PKG-INFO` & `tutti-client-0.3.8/tutti_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutti-client
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python client library for Tutti.ai
 Home-page: https://github.com/iflb/tutti-client-python
 Author: Intelligent Framework Lab
 Author-email: saito@iflab.tokyo
 Project-URL: Project Owner, http://www.pcl.cs.waseda.ac.jp/
 Project-URL: Funding, https://www.waseda.jp/inst/gcs/news/2019/11/29/870/
 Keywords: crowdsourcing annotation framework asyncio
```

