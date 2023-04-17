# Comparing `tmp/planet-2.0a5.dev0.tar.gz` & `tmp/planet-2.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/tmp_c1sxce1/planet-2.0a5.dev0.tar", last modified: Thu Oct 20 20:49:42 2022, max compression
+gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/tmp91f072j5/planet-2.0a6.tar", last modified: Thu Nov 10 20:05:21 2022, max compression
```

## Comparing `planet-2.0a5.dev0.tar` & `planet-2.0a6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/
--rw-r--r--   0 runner    (1001) docker     (121)    11324 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8846 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7983 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet/
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7428 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (121)    12452 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    10599 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/orders.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet/clients/
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23897 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/clients/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    17404 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/clients/orders.py
--rw-r--r--   0 runner    (1001) docker     (121)     7974 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/clients/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet/data/
--rw-r--r--   0 runner    (1001) docker     (121)    13778 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/data/Feature.json
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/data/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    22921 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/data/orders_product_bundle_2022_02_02.json
--rw-r--r--   0 runner    (1001) docker     (121)    10951 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/data_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/geojson.py
--rw-r--r--   0 runner    (1001) docker     (121)    15287 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    11413 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    15074 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/order_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     3101 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5065 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/planet/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8846 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 20:49:41.000000 planet-2.0a5.dev0/planet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/planet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-10-20 20:49:42.000000 planet-2.0a5.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-10-20 20:49:11.000000 planet-2.0a5.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:05:21.000000 planet-2.0a6/
+-rw-r--r--   0 runner    (1001) docker     (121)    11324 2022-11-10 20:04:51.000000 planet-2.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     8841 2022-11-10 20:05:21.000000 planet-2.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7983 2022-11-10 20:04:51.000000 planet-2.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:05:21.000000 planet-2.0a6/planet/
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-11-10 20:04:51.000000 planet-2.0a6/planet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-10 20:04:51.000000 planet-2.0a6/planet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7488 2022-11-10 20:04:51.000000 planet-2.0a6/planet/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:05:21.000000 planet-2.0a6/planet/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1764 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12457 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10599 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/orders.py
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-11-10 20:04:51.000000 planet-2.0a6/planet/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:05:21.000000 planet-2.0a6/planet/clients/
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-11-10 20:04:51.000000 planet-2.0a6/planet/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23593 2022-11-10 20:04:51.000000 planet-2.0a6/planet/clients/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17317 2022-11-10 20:04:51.000000 planet-2.0a6/planet/clients/orders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8361 2022-11-10 20:04:51.000000 planet-2.0a6/planet/clients/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-11-10 20:04:51.000000 planet-2.0a6/planet/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:05:21.000000 planet-2.0a6/planet/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    13778 2022-11-10 20:04:51.000000 planet-2.0a6/planet/data/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (121)      684 2022-11-10 20:04:51.000000 planet-2.0a6/planet/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    22921 2022-11-10 20:04:51.000000 planet-2.0a6/planet/data/orders_product_bundle_2022_02_02.json
+-rw-r--r--   0 runner    (1001) docker     (121)    11091 2022-11-10 20:04:51.000000 planet-2.0a6/planet/data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2006 2022-11-10 20:04:51.000000 planet-2.0a6/planet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-11-10 20:04:51.000000 planet-2.0a6/planet/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15485 2022-11-10 20:04:51.000000 planet-2.0a6/planet/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-11-10 20:04:51.000000 planet-2.0a6/planet/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9070 2022-11-10 20:04:51.000000 planet-2.0a6/planet/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15324 2022-11-10 20:04:51.000000 planet-2.0a6/planet/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3199 2022-11-10 20:04:51.000000 planet-2.0a6/planet/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5065 2022-11-10 20:04:51.000000 planet-2.0a6/planet/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8841 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-10 20:05:21.000000 planet-2.0a6/planet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2022-11-10 20:05:21.000000 planet-2.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-11-10 20:04:51.000000 planet-2.0a6/setup.py
```

### Comparing `planet-2.0a5.dev0/LICENSE` & `planet-2.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/PKG-INFO` & `planet-2.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.0a5.dev0
+Version: 2.0a6
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.0a5.dev0/README.md` & `planet-2.0a6/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/__init__.py` & `planet-2.0a6/planet/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/auth.py` & `planet-2.0a6/planet/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 import os
 import pathlib
 import typing
 
 import httpx
 import jwt
 
-from . import http, models
+from . import http
 from .constants import PLANET_BASE_URL, SECRET_FILE_PATH
 from .exceptions import AuthException
+from typing import Optional
 
 LOGGER = logging.getLogger(__name__)
 
 BASE_URL = f'{PLANET_BASE_URL}/v0/auth'
 ENV_API_KEY = 'PL_API_KEY'
 
 AuthType = httpx.Auth
@@ -48,15 +49,16 @@
         '''
         auth = APIKeyAuth(key=key)
         LOGGER.debug('Auth obtained from api key.')
         return auth
 
     @staticmethod
     def from_file(
-            filename: typing.Union[str, pathlib.Path] = None) -> AuthType:
+        filename: Optional[typing.Union[str,
+                                        pathlib.Path]] = None) -> AuthType:
         '''Create authentication from secret file.
 
         The secret file is named `.planet.json` and is stored in the user
         directory. The file has a special format and should have been created
         with `Auth.write()`.
 
         Parameters:
@@ -73,15 +75,15 @@
         except (KeyError, json.decoder.JSONDecodeError):
             raise AuthException(f'File {filename} is not the correct format.')
 
         LOGGER.debug(f'Auth read from secret file {filename}.')
         return auth
 
     @staticmethod
-    def from_env(variable_name: str = None) -> AuthType:
+    def from_env(variable_name: Optional[str] = None) -> AuthType:
         '''Create authentication from environment variable.
 
         Reads the `PL_API_KEY` environment variable
 
         Parameters:
             variable_name: Alternate environment variable.
         '''
@@ -95,15 +97,15 @@
                 f'Environment variable {variable_name} either does not exist '
                 'or is empty.')
         return auth
 
     @staticmethod
     def from_login(email: str,
                    password: str,
-                   base_url: str = None) -> AuthType:
+                   base_url: Optional[str] = None) -> AuthType:
         '''Create authentication from login email and password.
 
         Note: To keep your password secure, the use of `getpass` is
         recommended.
 
         Parameters:
             email: Planet account email address.
@@ -129,28 +131,29 @@
     def value(self):
         pass
 
     @abc.abstractmethod
     def to_dict(self) -> dict:
         pass
 
-    def write(self, filename: typing.Union[str, pathlib.Path] = None):
+    def write(self,
+              filename: Optional[typing.Union[str, pathlib.Path]] = None):
         '''Write authentication information.
 
         Parameters:
             filename: Alternate path for the planet secret file.
         '''
         filename = filename or SECRET_FILE_PATH
         secret_file = _SecretFile(filename)
         secret_file.write(self.to_dict())
 
 
 class AuthClient:
 
-    def __init__(self, base_url: str = None):
+    def __init__(self, base_url: Optional[str] = None):
         """
         Parameters:
             base_url: The base URL to use. Defaults to production
                 authentication API base url.
         """
         self._base_url = base_url or BASE_URL
         if self._base_url.endswith('/'):
@@ -170,18 +173,16 @@
              A JSON object containing an `api_key` property with the user's
         API_KEY.
         '''
         url = f'{self._base_url}/login'
         data = {'email': email, 'password': password}
 
         sess = http.AuthSession()
-        req = models.Request(url, method='POST', json=data)
-        resp = sess.request(req)
-        auth_data = self.decode_response(resp)
-        return auth_data
+        resp = sess.request(url=url, method='POST', json=data)
+        return self.decode_response(resp)
 
     @staticmethod
     def decode_response(response):
         '''Decode the token JWT'''
         token = response.json()['token']
         return jwt.decode(token, options={'verify_signature': False})
```

### Comparing `planet-2.0a5.dev0/planet/cli/auth.py` & `planet-2.0a6/planet/cli/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/cli.py` & `planet-2.0a6/planet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/cmds.py` & `planet-2.0a6/planet/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/collect.py` & `planet-2.0a6/planet/cli/collect.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/data.py` & `planet-2.0a6/planet/cli/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     '''Validates the item type by comparing the inputted item type to all
     supported item types.'''
     try:
         for item_type in item_types:
             validate_item_type(item_type)
         return item_types
     except SpecificationException as e:
-        raise click.BadParameter(e)
+        raise click.BadParameter(str(e))
 
 
 def date_range_to_filter(ctx, param, values) -> Optional[List[dict]]:
 
     def _func(obj):
         field, comp, value = obj
         kwargs = {'field_name': field, comp: value}
```

### Comparing `planet-2.0a5.dev0/planet/cli/io.py` & `planet-2.0a6/planet/cli/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/options.py` & `planet-2.0a6/planet/cli/options.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/orders.py` & `planet-2.0a6/planet/cli/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/subscriptions.py` & `planet-2.0a6/planet/cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/cli/types.py` & `planet-2.0a6/planet/cli/types.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/clients/__init__.py` & `planet-2.0a6/planet/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/clients/data.py` & `planet-2.0a6/planet/clients/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 # the License.
 """Functionality for interacting with the data api"""
 import asyncio
 import hashlib
 import logging
 from pathlib import Path
 import time
-import typing
+from typing import Any, AsyncIterator, Callable, Dict, List, Optional
 
 from .. import exceptions
 from ..constants import PLANET_BASE_URL
 from ..http import Session
-from ..models import Paged, Request, Response, StreamingBody
+from ..models import Paged, StreamingBody
 
 BASE_URL = f'{PLANET_BASE_URL}/data/v1/'
 SEARCHES_PATH = '/searches'
 STATS_PATH = '/stats'
 
 # TODO: get these values from the spec directly gh-619
 LIST_SORT_ORDER = ('created desc', 'created asc')
@@ -70,15 +70,15 @@
         ...         # use client here
         ...
         >>> asyncio.run(main())
 
         ```
     """
 
-    def __init__(self, session: Session, base_url: str = None):
+    def __init__(self, session: Session, base_url: Optional[str] = None):
         """
         Parameters:
             session: Open session connected to server.
             base_url: The base URL to use. Defaults to production data API
                 base url.
         """
         self._session = session
@@ -89,31 +89,20 @@
 
     def _searches_url(self):
         return f'{self._base_url}{SEARCHES_PATH}'
 
     def _item_url(self, item_type, item_id):
         return f'{self._base_url}/item-types/{item_type}/items/{item_id}'
 
-    def _request(self, url, method, data=None, params=None, json=None):
-        return Request(url, method=method, data=data, params=params, json=json)
-
-    async def _do_request(self, request: Request) -> Response:
-        """Submit a request and get response.
-
-        Parameters:
-            request: request to submit
-        """
-        return await self._session.request(request)
-
     async def search(self,
-                     item_types: typing.List[str],
+                     item_types: List[str],
                      search_filter: dict,
-                     name: str = None,
-                     sort: str = None,
-                     limit: int = 100) -> typing.AsyncIterator[dict]:
+                     name: Optional[str] = None,
+                     sort: Optional[str] = None,
+                     limit: int = 100) -> AsyncIterator[dict]:
         """Execute a quick search.
 
         Quick searches are saved for a short period of time (~month). The
         `name` parameter of the search defaults to the id of the generated
         search id if `name` is not specified.
 
         To filter to items you have access to download which are of standard
@@ -181,23 +170,23 @@
         if sort and sort != SEARCH_SORT_DEFAULT:
             sort = sort.lower()
             if sort not in SEARCH_SORT:
                 raise exceptions.ClientError(
                     f'{sort} must be one of {SEARCH_SORT}')
             params['_sort'] = sort
 
-        request = self._request(url,
-                                method='POST',
-                                json=request_json,
-                                params=params)
-        return Items(request, self._do_request, limit=limit)
+        response = await self._session.request(method='POST',
+                                               url=url,
+                                               json=request_json,
+                                               params=params)
+        return Items(response, self._session.request, limit=limit)
 
     async def create_search(self,
                             name: str,
-                            item_types: typing.List[str],
+                            item_types: List[str],
                             search_filter: dict,
                             enable_email: bool = False) -> dict:
         """Create a new saved structured item search.
 
         To filter to items you have access to download which are of standard
         (aka not test) quality, use the following:
 
@@ -225,29 +214,30 @@
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         url = self._searches_url()
 
         # TODO: validate item_types
-        request_json = {
+        request = {
             'name': name,
             'filter': search_filter,
             'item_types': item_types,
             '__daily_email_enabled': enable_email
         }
 
-        request = self._request(url, method='POST', json=request_json)
-        response = await self._do_request(request)
+        response = await self._session.request(method='POST',
+                                               url=url,
+                                               json=request)
         return response.json()
 
     async def update_search(self,
                             search_id: str,
                             name: str,
-                            item_types: typing.List[str],
+                            item_types: List[str],
                             search_filter: dict,
                             enable_email: bool = False) -> dict:
         """Update an existing saved search.
 
         Parameters:
             search_id: Saved search identifier.
             name: The name of the saved search.
@@ -256,29 +246,30 @@
             enable_email: Send a daily email when new results are added.
 
         Returns:
             Description of the saved search.
         """
         url = f'{self._searches_url()}/{search_id}'
 
-        request_json = {
+        request = {
             'name': name,
             'filter': search_filter,
             'item_types': item_types,
             '__daily_email_enabled': enable_email
         }
 
-        request = self._request(url, method='PUT', json=request_json)
-        response = await self._do_request(request)
+        response = await self._session.request(method='PUT',
+                                               url=url,
+                                               json=request)
         return response.json()
 
     async def list_searches(self,
                             sort: str = 'created desc',
                             search_type: str = 'any',
-                            limit: int = 100) -> typing.AsyncIterator[dict]:
+                            limit: int = 100) -> AsyncIterator[dict]:
         """List all saved searches available to the authenticated user.
 
         NOTE: the term 'saved' is overloaded here. We want to list saved
         searches that are 'quick' or list saved searches that are 'saved'? Do
         we want to introduce a new term, 'stored' that encompasses 'saved' and
         'quick' searches?
 
@@ -303,51 +294,51 @@
 
         search_type = search_type.lower()
         if search_type not in LIST_SEARCH_TYPE:
             raise exceptions.ClientError(
                 f'{search_type} must be one of {LIST_SEARCH_TYPE}')
 
         url = f'{self._searches_url()}'
-        request = self._request(url, method='GET')
-        return Searches(request, self._do_request, limit=limit)
+
+        response = await self._session.request(method='GET', url=url)
+        return Searches(response, self._session.request, limit=limit)
 
     async def delete_search(self, search_id: str):
         """Delete an existing saved search.
 
         Parameters:
             search_id: Saved search identifier.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         url = f'{self._searches_url()}/{search_id}'
 
-        request = self._request(url, method='DELETE')
-        await self._do_request(request)
+        await self._session.request(method='DELETE', url=url)
 
     async def get_search(self, search_id: str) -> dict:
         """Get a saved search by id.
 
         Parameters:
             search_id: Stored search identifier.
 
         Returns:
             Saved search details.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         url = f'{self._searches_url()}/{search_id}'
-        req = self._request(url, method='GET')
-        resp = await self._do_request(req)
-        return resp.json()
+
+        response = await self._session.request(method='GET', url=url)
+        return response.json()
 
     async def run_search(self,
                          search_id: str,
-                         limit: int = 100) -> typing.AsyncIterator[dict]:
+                         limit: int = 100) -> AsyncIterator[dict]:
         """Execute a saved search.
 
         Parameters:
             search_id: Stored search identifier.
             limit: Maximum number of results to return. When set to 0, no
                 maximum is applied.
 
@@ -355,19 +346,19 @@
             Returns an iterator over all items matching the search.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         url = f'{self._searches_url()}/{search_id}/results'
 
-        request = self._request(url, method='GET')
-        return Items(request, self._do_request, limit=limit)
+        response = await self._session.request(method='GET', url=url)
+        return Items(response, self._session.request, limit=limit)
 
     async def get_stats(self,
-                        item_types: typing.List[str],
+                        item_types: List[str],
                         search_filter: dict,
                         interval: str) -> dict:
         """Get item search statistics.
 
         Parameters:
             item_types: The item types to include in the search.
             search_filter: Structured search criteria.
@@ -384,25 +375,26 @@
         interval = interval.lower()
         if interval not in STATS_INTERVAL:
             raise exceptions.ClientError(
                 f'{interval} must be one of {STATS_INTERVAL}')
 
         url = f'{self._base_url}{STATS_PATH}'
 
-        request_json = {
+        request = {
             'interval': interval,
             'filter': search_filter,
             'item_types': item_types
         }
 
-        request = self._request(url, method='POST', json=request_json)
-        response = await self._do_request(request)
+        response = await self._session.request(method='POST',
+                                               url=url,
+                                               json=request)
         return response.json()
 
-    async def list_asset_types(self) -> typing.List[dict]:
+    async def list_asset_types(self) -> List[dict]:
         """List all asset types available to the authenticated user.
 
         Returns:
             List of asset type details.
 
         Raises:
             planet.exceptions.APIError: On API error.
@@ -423,15 +415,15 @@
             Asset type details.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         raise NotImplementedError
 
-    async def list_item_types(self) -> typing.List[dict]:
+    async def list_item_types(self) -> List[dict]:
         """List all item types available to the authenticated user.
 
         Returns:
             List of item type details.
 
         Raises:
             planet.exceptions.APIError: On API error.
@@ -477,16 +469,15 @@
             Item details.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         raise NotImplementedError
 
-    async def list_item_assets(self, item_type_id: str,
-                               item_id: str) -> typing.List[dict]:
+    async def list_item_assets(self, item_type_id: str, item_id: str) -> dict:
         """List all assets available for an item.
 
         An asset describes a product that can be derived from an item's source
         data, and can be used for various analytic, visual or other purposes.
         These are referred to as asset_types.
 
         Parameters:
@@ -497,16 +488,16 @@
             Descriptions of available assets as a dictionary with asset_type_id
             as keys and asset description as value.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
         url = f'{self._item_url(item_type_id, item_id)}/assets'
-        request = self._request(url, method='GET')
-        response = await self._do_request(request)
+
+        response = await self._session.request(method='GET', url=url)
         return response.json()
 
     async def get_asset(self,
                         item_type_id: str,
                         item_id: str,
                         asset_type_id: str) -> dict:
         """Get an item asset.
@@ -555,25 +546,26 @@
             url = asset['_links']['activate']
         except KeyError:
             raise exceptions.ClientError(
                 'asset missing ["_links"]["activate"] entry')
 
         # lets not try to activate an asset already activating or active
         if status == 'inactive':
-            request = self._request(url, method='GET')
             # no response is returned
-            await self._do_request(request)
+            await self._session.request(method='GET', url=url)
 
         return
 
-    async def wait_asset(self,
-                         asset: dict,
-                         delay: int = WAIT_DELAY,
-                         max_attempts: int = WAIT_MAX_ATTEMPTS,
-                         callback: typing.Callable[[str], None] = None) -> str:
+    async def wait_asset(
+            self,
+            asset: dict,
+            delay: int = WAIT_DELAY,
+            max_attempts: int = WAIT_MAX_ATTEMPTS,
+            callback: Optional[Callable[[str],
+                                        None]] = None) -> Dict[Any, Any]:
         """Wait for an item asset to be active.
 
         Prior to waiting for the asset to be active, be sure to activate the
         asset with activate_asset().
 
         Parameters:
             asset: Description of the asset. Obtained from get_asset().
@@ -618,30 +610,29 @@
 
             try:
                 asset_url = asset['_links']['_self']
             except KeyError:
                 raise exceptions.ClientError(
                     'asset missing ["_links"]["_self"] entry.')
 
-            request = self._request(asset_url, method='GET')
-            response = await self._do_request(request)
+            response = await self._session.request(method='GET', url=asset_url)
             asset = response.json()
 
         if max_attempts and num_attempts >= max_attempts:
             raise exceptions.ClientError(
                 f'Maximum number of attempts ({max_attempts}) reached.')
 
         return asset
 
     async def download_asset(self,
                              asset: dict,
-                             filename: str = None,
+                             filename: Optional[str] = None,
                              directory: Path = Path('.'),
                              overwrite: bool = False,
-                             progress_bar: bool = True) -> str:
+                             progress_bar: bool = True) -> Path:
         """Download an asset.
 
         The asset must be active before it can be downloaded. This can be
         achieved with activate_asset() followed by wait_asset().
 
         If overwrite is False and the file already exists, download will be
         skipped and the file path will be returned as usual.
@@ -664,17 +655,15 @@
         """
         try:
             location = asset['location']
         except KeyError:
             raise exceptions.ClientError(
                 'asset missing ["location"] entry. Is asset active?')
 
-        req = self._request(location, method='GET')
-
-        async with self._session.stream(req) as resp:
+        async with self._session.stream(method='GET', url=location) as resp:
             body = StreamingBody(resp)
             dl_path = Path(directory, filename or body.name)
             dl_path.parent.mkdir(exist_ok=True, parents=True)
             await body.write(dl_path,
                              overwrite=overwrite,
                              progress_bar=progress_bar)
         return dl_path
```

### Comparing `planet-2.0a5.dev0/planet/clients/orders.py` & `planet-2.0a6/planet/clients/orders.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """Functionality for interacting with the orders api"""
 import asyncio
 import logging
 import time
-import typing
+from typing import AsyncIterator, Callable, List, Optional
 import uuid
 import json
 import hashlib
 
 from pathlib import Path
 from .. import exceptions
 from ..constants import PLANET_BASE_URL
 from ..http import Session
-from ..models import Paged, Request, Response, StreamingBody
+from ..models import Paged, StreamingBody
 
 BASE_URL = f'{PLANET_BASE_URL}/compute/ops'
 STATS_PATH = '/stats/orders/v2'
 ORDERS_PATH = '/orders/v2'
 BULK_PATH = '/bulk/orders/v2'
 
 # Order states https://developers.planet.com/docs/orders/ordering/#order-states
@@ -80,15 +80,15 @@
         ...         # use client here
         ...
         >>> asyncio.run(main())
 
         ```
     """
 
-    def __init__(self, session: Session, base_url: str = None):
+    def __init__(self, session: Session, base_url: Optional[str] = None):
         """
         Parameters:
             session: Open session connected to server.
             base_url: The base URL to use. Defaults to production orders API
                 base url.
         """
         self._session = session
@@ -108,25 +108,14 @@
 
     def _orders_url(self):
         return f'{self._base_url}{ORDERS_PATH}'
 
     def _stats_url(self):
         return f'{self._base_url}{STATS_PATH}'
 
-    def _request(self, url, method, data=None, params=None, json=None):
-        return Request(url, method=method, data=data, params=params, json=json)
-
-    async def _do_request(self, request: Request) -> Response:
-        '''Submit a request and get response.
-
-        Parameters:
-            request: request to submit
-        '''
-        return await self._session.request(request)
-
     async def create_order(self, request: dict) -> dict:
         '''Create an order request.
 
         Example:
 
         ```python
         >>> import asyncio
@@ -152,18 +141,18 @@
         Returns:
             JSON description of the created order
 
         Raises:
             planet.exceptions.APIError: On API error.
         '''
         url = self._orders_url()
-
-        req = self._request(url, method='POST', json=request)
-        resp = await self._do_request(req)
-        return resp.json()
+        response = await self._session.request(method='POST',
+                                               url=url,
+                                               json=request)
+        return response.json()
 
     async def get_order(self, order_id: str) -> dict:
         '''Get order details by Order ID.
 
         Parameters:
             order_id: The ID of the order
 
@@ -173,17 +162,16 @@
         Raises:
             planet.exceptions.ClientError: If order_id is not a valid UUID.
             planet.exceptions.APIError: On API error.
         '''
         self._check_order_id(order_id)
         url = f'{self._orders_url()}/{order_id}'
 
-        req = self._request(url, method='GET')
-        resp = await self._do_request(req)
-        return resp.json()
+        response = await self._session.request(method='GET', url=url)
+        return response.json()
 
     async def cancel_order(self, order_id: str) -> dict:
         '''Cancel a queued order.
 
         Parameters:
             order_id: The ID of the order
 
@@ -193,19 +181,19 @@
         Raises:
             planet.exceptions.ClientError: If order_id is not a valid UUID.
             planet.exceptions.APIError: On API error.
         '''
         self._check_order_id(order_id)
         url = f'{self._orders_url()}/{order_id}'
 
-        req = self._request(url, method='PUT')
-        resp = await self._do_request(req)
-        return resp.json()
+        response = await self._session.request(method='PUT', url=url)
+        return response.json()
 
-    async def cancel_orders(self, order_ids: typing.List[str] = None) -> dict:
+    async def cancel_orders(self,
+                            order_ids: Optional[List[str]] = None) -> dict:
         '''Cancel queued orders in bulk.
 
         Parameters:
             order_ids: The IDs of the orders. If empty or None, all orders in a
                 pre-running state will be cancelled.
 
         Returns:
@@ -219,35 +207,36 @@
         url = f'{self._base_url}{BULK_PATH}/cancel'
         cancel_body = {}
         if order_ids:
             for oid in order_ids:
                 self._check_order_id(oid)
             cancel_body['order_ids'] = order_ids
 
-        req = self._request(url, method='POST', json=cancel_body)
-        resp = await self._do_request(req)
-        return resp.json()
+        response = await self._session.request(method='POST',
+                                               url=url,
+                                               json=cancel_body)
+
+        return response.json()
 
     async def aggregated_order_stats(self) -> dict:
         '''Get aggregated counts of active orders.
 
         Returns:
             Aggregated order counts
 
         Raises:
             planet.exceptions.APIError: On API error.
         '''
         url = self._stats_url()
-        req = self._request(url, method='GET')
-        resp = await self._do_request(req)
-        return resp.json()
+        response = await self._session.request(method='GET', url=url)
+        return response.json()
 
     async def download_asset(self,
                              location: str,
-                             filename: str = None,
+                             filename: Optional[str] = None,
                              directory: Path = Path('.'),
                              overwrite: bool = False,
                              progress_bar: bool = True) -> Path:
         """Download ordered asset.
 
         Parameters:
             location: Download location url including download token.
@@ -259,31 +248,29 @@
 
         Returns:
             Path to downloaded file.
 
         Raises:
             planet.exceptions.APIError: On API error.
         """
-        req = self._request(location, method='GET')
-
-        async with self._session.stream(req) as resp:
+        async with self._session.stream(method='GET', url=location) as resp:
             body = StreamingBody(resp)
             dl_path = Path(directory, filename or body.name)
             dl_path.parent.mkdir(exist_ok=True, parents=True)
             await body.write(dl_path,
                              overwrite=overwrite,
                              progress_bar=progress_bar)
         return dl_path
 
     async def download_order(self,
                              order_id: str,
                              directory: Path = Path('.'),
                              overwrite: bool = False,
                              progress_bar: bool = False,
-                             checksum: str = None) -> typing.List[Path]:
+                             checksum: Optional[str] = None) -> List[Path]:
         """Download all assets in an order.
 
         Parameters:
             order_id: The ID of the order.
             directory: Base directory for file download. This directory must
                 already exist.
             overwrite: Overwrite files if they already exist.
@@ -389,18 +376,18 @@
 
             if origin_hash != returned_hash:
                 raise exceptions.ClientError(
                     f'File ({filename}) checksums do not match.')
 
     async def wait(self,
                    order_id: str,
-                   state: str = None,
+                   state: Optional[str] = None,
                    delay: int = 5,
                    max_attempts: int = 200,
-                   callback: typing.Callable[[str], None] = None) -> str:
+                   callback: Optional[Callable[[str], None]] = None) -> str:
         """Wait until order reaches desired state.
 
         Returns the state of the order on the last poll.
 
         This function polls the Orders API to determine the order state, with
         the specified delay between each polling attempt, until the
         order reaches a final state, or earlier state, if specified.
@@ -473,16 +460,16 @@
         if max_attempts and num_attempts >= max_attempts:
             raise exceptions.ClientError(
                 f'Maximum number of attempts ({max_attempts}) reached.')
 
         return current_state
 
     async def list_orders(self,
-                          state: str = None,
-                          limit: int = 100) -> typing.AsyncIterator[dict]:
+                          state: Optional[str] = None,
+                          limit: int = 100) -> AsyncIterator[dict]:
         """Get all order requests.
 
         Parameters:
             state: Filter orders to given state.
             limit: Maximum number of results to return. When set to 0, no
                 maximum is applied.
 
@@ -500,9 +487,11 @@
                 raise exceptions.ClientError(
                     f'Order state ({state}) is not a valid state. '
                     f'Valid states are {ORDER_STATE_SEQUENCE}')
             params = {"state": state}
         else:
             params = None
 
-        request = self._request(url, 'GET', params=params)
-        return Orders(request, self._do_request, limit=limit)
+        response = await self._session.request(method='GET',
+                                               url=url,
+                                               params=params)
+        return Orders(response, self._session.request, limit=limit)
```

### Comparing `planet-2.0a5.dev0/planet/clients/subscriptions.py` & `planet-2.0a6/planet/clients/subscriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Planet Subscriptions API Python client."""
 
 import logging
 from typing import AsyncIterator, Optional, Set
 
 from planet.exceptions import APIError, ClientError
 from planet.http import Session
-from planet.models import Paged, Request
+from planet.models import Paged
 
 LOGGER = logging.getLogger()
 
 
 class SubscriptionsClient:
     """A Planet Subscriptions Service API 1.0.0 client.
 
@@ -25,15 +25,15 @@
 
     Attributes:
         session (Session): an authenticated session which wraps the
             low-level HTTP client.
     """
 
     def __init__(self, session: Session) -> None:
-        self.session = session
+        self._session = session
 
     async def list_subscriptions(self,
                                  status: Optional[Set[str]] = None,
                                  limit: int = 100) -> AsyncIterator[dict]:
         """Get account subscriptions with optional filtering.
 
         Note:
@@ -59,19 +59,21 @@
 
         class _SubscriptionsPager(Paged):
             """Navigates pages of messages about subscriptions."""
             ITEMS_KEY = 'subscriptions'
 
         params = {'status': [val for val in status or {}]}
         url = 'https://api.planet.com/subscriptions/v1'
-        req = Request(url, params=params)
 
         try:
-            async for sub in _SubscriptionsPager(req,
-                                                 self.session.request,
+            response = await self._session.request(method='GET',
+                                                   url=url,
+                                                   params=params)
+            async for sub in _SubscriptionsPager(response,
+                                                 self._session.request,
                                                  limit=limit):
                 yield sub
         # Forward APIError. We don't strictly need this clause, but it
         # makes our intent clear.
         except APIError:
             raise
         except ClientError:  # pragma: no cover
@@ -88,18 +90,19 @@
 
         Raises:
             APIError: on an API server error.
             ClientError: on a client error.
         """
 
         url = 'https://api.planet.com/subscriptions/v1'
-        req = Request(url, method='POST', json=request)
 
         try:
-            resp = await self.session.request(req)
+            resp = await self._session.request(method='POST',
+                                               url=url,
+                                               json=request)
         # Forward APIError. We don't strictly need this clause, but it
         # makes our intent clear.
         except APIError:
             raise
         except ClientError:  # pragma: no cover
             raise
         else:
@@ -117,18 +120,17 @@
 
         Raises:
             APIError: on an API server error.
             ClientError: on a client error.
         """
         root_url = 'https://api.planet.com/subscriptions/v1'
         url = f'{root_url}/{subscription_id}/cancel'
-        req = Request(url, method='POST')
 
         try:
-            _ = await self.session.request(req)
+            _ = await self._session.request(method='POST', url=url)
         # Forward APIError. We don't strictly need this clause, but it
         # makes our intent clear.
         except APIError:
             raise
         except ClientError:  # pragma: no cover
             raise
 
@@ -144,18 +146,19 @@
             dict: description of the updated subscription.
 
         Raises:
             APIError: on an API server error.
             ClientError: on a client error.
         """
         url = f'https://api.planet.com/subscriptions/v1/{subscription_id}'
-        req = Request(url, method='PUT', json=request)
 
         try:
-            resp = await self.session.request(req)
+            resp = await self._session.request(method='PUT',
+                                               url=url,
+                                               json=request)
         # Forward APIError. We don't strictly need this clause, but it
         # makes our intent clear.
         except APIError:
             raise
         except ClientError:  # pragma: no cover
             raise
         else:
@@ -172,18 +175,17 @@
             dict: description of the subscription.
 
         Raises:
             APIError: on an API server error.
             ClientError: on a client error.
         """
         url = f'https://api.planet.com/subscriptions/v1/{subscription_id}'
-        req = Request(url, method='GET')
 
         try:
-            resp = await self.session.request(req)
+            resp = await self._session.request(method='GET', url=url)
         # Forward APIError. We don't strictly need this clause, but it
         # makes our intent clear.
         except APIError:
             raise
         except ClientError:  # pragma: no cover
             raise
         else:
@@ -221,19 +223,22 @@
             """Navigates pages of messages about subscription results."""
             NEXT_KEY = '_next'
             ITEMS_KEY = 'results'
 
         params = {'status': [val for val in status or {}]}
         root_url = 'https://api.planet.com/subscriptions/v1'
         url = f'{root_url}/{subscription_id}/results'
-        req = Request(url, params=params)
 
         try:
-            async for sub in _ResultsPager(req,
-                                           self.session.request,
+            resp = await self._session.request(method='GET',
+                                               url=url,
+                                               params=params)
+
+            async for sub in _ResultsPager(resp,
+                                           self._session.request,
                                            limit=limit):
                 yield sub
         # Forward APIError. We don't strictly need this clause, but it
         # makes our intent clear.
         except APIError:
             raise
         except ClientError:  # pragma: no cover
```

### Comparing `planet-2.0a5.dev0/planet/constants.py` & `planet-2.0a6/planet/constants.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/data/Feature.json` & `planet-2.0a6/planet/data/Feature.json`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/data/README.md` & `planet-2.0a6/planet/data/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/data/orders_product_bundle_2022_02_02.json` & `planet-2.0a6/planet/data/orders_product_bundle_2022_02_02.json`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/data_filter.py` & `planet-2.0a6/planet/data_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """Functionality for preparing a data search filter"""
 from datetime import datetime
 import logging
-from typing import Any, Callable, List, Union
+from typing import Optional, Any, Callable, List, Union
 
 from planet import exceptions, geojson
 
 LOGGER = logging.getLogger(__name__)
 
 
 def and_filter(nested_filters: List[dict]) -> dict:
@@ -72,15 +72,15 @@
 def _range_filter(
     ftype: str,
     field_name: str,
     gt: Any,
     lt: Any,
     gte: Any,
     lte: Any,
-    callback: Callable = None,
+    callback: Optional[Callable] = None,
 ) -> dict:
     """Base for creating range filters.
 
     Parameters:
         ftype: Type of the filter
         field_name: Name of field to filter on.
         gt: Greater than conditional value.
@@ -105,18 +105,18 @@
     if not config:
         raise exceptions.PlanetError("No conditional parameters specified.")
 
     return _field_filter(ftype, field_name=field_name, config=config)
 
 
 def date_range_filter(field_name: str,
-                      gt: datetime = None,
-                      lt: datetime = None,
-                      gte: datetime = None,
-                      lte: datetime = None) -> dict:
+                      gt: Optional[datetime] = None,
+                      lt: Optional[datetime] = None,
+                      gte: Optional[datetime] = None,
+                      lte: Optional[datetime] = None) -> dict:
     """Create a DateRangeFilter
 
     The DateRangeFilter can be used to search on any property with a timestamp
     such as acquired or published.
 
     One or more of the conditional parameters `gt`, `lt`, `gte`, `lte` must be
     specified. Conditionals are combined in a logical AND, so only items that
@@ -147,18 +147,18 @@
     if not value.utcoffset():
         # rfc3339 needs a Z if there is no timezone offset
         iso += 'Z'
     return iso
 
 
 def range_filter(field_name: str,
-                 gt: float = None,
-                 lt: float = None,
-                 gte: float = None,
-                 lte: float = None) -> dict:
+                 gt: Optional[float] = None,
+                 lt: Optional[float] = None,
+                 gte: Optional[float] = None,
+                 lte: Optional[float] = None) -> dict:
     """Create a RangeFilter
 
     The RangeFilter can be used to search for items with numerical properties.
     It is useful for matching fields that have a continuous range of values
     such as cloud_cover or view_angle.
 
     One or more of the conditional parameters `gt`, `lt`, `gte`, `lte` must be
@@ -175,18 +175,18 @@
     Raises:
         exceptions.PlanetError: If no conditional parameter is specified.
     """
     return _range_filter('RangeFilter', field_name, gt, lt, gte, lte)
 
 
 def update_filter(field_name: str,
-                  gt: float = None,
-                  lt: float = None,
-                  gte: float = None,
-                  lte: float = None) -> dict:
+                  gt: Optional[float] = None,
+                  lt: Optional[float] = None,
+                  gte: Optional[float] = None,
+                  lte: Optional[float] = None) -> dict:
     """Create an UpdateFilter
 
     The UpdateFilter can be used to filter items by changes to a specified
     metadata field value made after a specified date, due to a republishing
     event. This feature allows you identify items which may have been
     republished with improvements or fixes, enabling you to keep your internal
     catalogs up-to-date and make more informed redownload decisions. The filter
```

### Comparing `planet-2.0a5.dev0/planet/exceptions.py` & `planet-2.0a6/planet/exceptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/geojson.py` & `planet-2.0a6/planet/geojson.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/http.py` & `planet-2.0a6/planet/http.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """Functionality to perform HTTP requests"""
 from __future__ import annotations  # https://stackoverflow.com/a/33533514
 import asyncio
 from collections import Counter
+from contextlib import asynccontextmanager
 from http import HTTPStatus
 import logging
 import random
 import time
-
+from typing import AsyncGenerator, Optional
 import httpx
 
 from .auth import Auth, AuthType
 from . import exceptions, models
 from .__version__ import __version__
 
 # NOTE: configuration of the session was performed using the data API quick
@@ -221,15 +222,15 @@
     ...         pass
     ...
     >>> asyncio.run(main())
 
     ```
     '''
 
-    def __init__(self, auth: AuthType = None):
+    def __init__(self, auth: Optional[AuthType] = None):
         """Initialize a Session.
 
         Parameters:
             auth: Planet server authentication.
         """
         if auth is None:
             # Try getting credentials from environment before checking
@@ -238,21 +239,24 @@
             try:
                 auth = Auth.from_env()
             except exceptions.PlanetError:
                 auth = Auth.from_file()
 
         LOGGER.info(f'Session read timeout set to {READ_TIMEOUT}.')
         timeout = httpx.Timeout(10.0, read=READ_TIMEOUT)
+
+        headers = {
+            'User-Agent': self._get_user_agent(), 'X-Planet-App': 'python-sdk'
+        }
+
         self._client = httpx.AsyncClient(auth=auth,
+                                         headers=headers,
                                          timeout=timeout,
                                          follow_redirects=True)
 
-        self._client.headers.update({'User-Agent': self._get_user_agent()})
-        self._client.headers.update({'X-Planet-App': 'python-sdk'})
-
         async def alog_request(*args, **kwargs):
             return self._log_request(*args, **kwargs)
 
         async def alog_response(*args, **kwargs):
             return self._log_response(*args, **kwargs)
 
         self._client.event_hooks['request'] = [alog_request]
@@ -344,54 +348,74 @@
         * https://cloud.google.com/iot/docs/how-tos/exponential-backoff
         """
         random_number_milliseconds = random.randint(0, 1000) / 1000.0
         calc_wait = 2**num_tries + random_number_milliseconds
         return min(calc_wait, max_retry_backoff)
 
     async def request(self,
-                      request: models.Request,
-                      stream: bool = False) -> models.Response:
-        """Submit a request with retry.
+                      method: str,
+                      url: str,
+                      json: Optional[dict] = None,
+                      params: Optional[dict] = None) -> models.Response:
+        """Build a request and submit it with retry and limiting.
 
         Parameters:
-            request: Request to submit.
-            stream: Get the body as a stream.
+            method: HTTP request method.
+            url: Location of the API endpoint.
+            json: JSON to send.
+            params: Values to send in the query string.
 
         Returns:
             Server response.
 
         Raises:
             planet.exceptions.APIException: On API error.
             planet.exceptions.ClientError: When retry limit is exceeded.
         """
-        # TODO: retry will be provided in httpx v1 [1] with usage [2]
-        # 1. https://github.com/encode/httpcore/pull/221
-        # 2. https://github.com/encode/httpx/blob/
-        # 89fb0cbc69ea07b123dd7b36dc1ed9151c5d398f/docs/async.md#explicit-transport-instances # noqa
-        # TODO: if throttling is necessary, check out [1] once v1
-        # 1. https://github.com/encode/httpx/issues/984
-        return await self._retry(self._request, request, stream=stream)
+        if json:
+            headers = {'Content-Type': 'application/json'}
+        else:
+            headers = None
 
-    async def _request(self, request, stream=False):
-        """Submit a request with rate/worker limiting."""
+        request = self._client.build_request(method=method,
+                                             url=url,
+                                             json=json,
+                                             params=params,
+                                             headers=headers)
+
+        http_response = await self._retry(self._send, request, stream=False)
+        return models.Response(http_response)
+
+    async def _send(self, request, stream=False) -> httpx.Response:
+        """Send request with with rate/worker limiting."""
         async with self._limiter:
-            http_resp = await self._client.send(request.http_request,
-                                                stream=stream)
-        return models.Response(request, http_resp)
+            http_resp = await self._client.send(request, stream=stream)
+
+        return http_resp
 
-    def stream(self, request: models.Request) -> Stream:
+    @asynccontextmanager
+    async def stream(
+            self, method: str,
+            url: str) -> AsyncGenerator[models.StreamingResponse, None]:
         """Submit a request and get the response as a stream context manager.
 
         Parameters:
-            request: Request to submit
+            method: HTTP request method.
+            url: Location of the API endpoint.
 
         Returns:
-            Context manager providing the body as a stream.
+            Context manager providing the streaming response.
         """
-        return Stream(session=self, request=request)
+        request = self._client.build_request(method=method, url=url)
+        http_response = await self._retry(self._send, request, stream=True)
+        response = models.StreamingResponse(http_response)
+        try:
+            yield response
+        finally:
+            await response.aclose()
 
 
 class AuthSession(BaseSession):
     """Synchronous connection to the Planet Auth service."""
 
     def __init__(self):
         """Initialize an AuthSession.
@@ -399,54 +423,33 @@
         self._client = httpx.Client(timeout=None)
         self._client.headers.update({'User-Agent': self._get_user_agent()})
         self._client.event_hooks['request'] = [self._log_request]
         self._client.event_hooks['response'] = [
             self._log_response, self._raise_for_status
         ]
 
-    def request(self, request):
+    def request(self, method: str, url: str, json: dict):
         """Submit a request
 
         Parameters:
-            request: Request to submit.
+            method: HTTP request method.
+            url: Location of the API endpoint.
+            json: JSON to send.
 
         Returns:
             Server response.
 
         Raises:
             planet.exceptions.APIException: On API error.
         """
-
-        http_resp = self._client.send(request.http_request)
-        return models.Response(request, http_resp)
+        request = self._client.build_request(method=method, url=url, json=json)
+        http_resp = self._client.send(request)
+        return models.Response(http_resp)
 
     @classmethod
     def _raise_for_status(cls, response):
         try:
             super()._raise_for_status(response)
         except exceptions.BadQuery:
             raise exceptions.APIError('Not a valid email address.')
         except exceptions.InvalidAPIKey:
             raise exceptions.APIError('Incorrect email or password.')
-
-
-class Stream:
-    '''Context manager for asynchronous response stream from Planet server.'''
-
-    def __init__(self, session: Session, request: models.Request):
-        """
-        Parameters:
-            session: Open session to Planet server.
-            request:  Request to submit.
-        """
-        self.session = session
-        self.request = request
-
-    async def __aenter__(self):
-        self.response = await self.session.request(
-            request=self.request,
-            stream=True,
-        )
-        return self.response
-
-    async def __aexit__(self, exc_type=None, exc_value=None, traceback=None):
-        await self.response.aclose()
```

### Comparing `planet-2.0a5.dev0/planet/io.py` & `planet-2.0a6/planet/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet/models.py` & `planet-2.0a6/planet/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,181 +9,111 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Manage data for requests and responses."""
-from datetime import datetime
 import logging
 import mimetypes
 from pathlib import Path
 import random
 import re
 import string
-import typing
+from typing import AsyncGenerator, Callable, List
 
 import httpx
 from tqdm.asyncio import tqdm
 
 from .exceptions import PagingError
 
 LOGGER = logging.getLogger(__name__)
 
 
-class RequestException(Exception):
-    """Exceptions thrown by RequestException"""
-    pass
-
-
-class Request:
-    '''Handles a HTTP request for the Planet server.
-
-    :param url: URL of API endpoint
-    :type url: str
-    :param params: Values to send in the query string. Defaults to None.
-    :type params: dict, list of tuples, or bytes, optional
-    :param data: Object to send in the body. Defaults to None.
-    :type data: dict, list of tuples, bytes, or file-like object, optional
-    :param json: JSON to send. Defaults to None.
-    :type json: dict, optional
-    :param method: HTTP request method. Defaults to 'GET'
-    :type method: str, optional
-    :raises RequestException: When provided `body_type` is not a subclass of
-        :py:class:`planet.api.models.Body`
-    '''
-
-    def __init__(self, url, params=None, data=None, json=None, method='GET'):
-        if data or json:
-            headers = {'Content-Type': 'application/json'}
-        else:
-            headers = None
-
-        self.http_request = httpx.Request(method,
-                                          url,
-                                          params=params,
-                                          data=data,
-                                          json=json,
-                                          headers=headers)
+class Response:
+    """Handles the Planet server's response to a HTTP request."""
+
+    def __init__(self, http_response: httpx.Response):
+        """Initialize object.
+
+        Parameters:
+            http_response: Response that was received from the server.
+        """
+        self._http_response = http_response
+
+    def __repr__(self):
+        return f'<models.Response [{self.status_code}]>'
 
     @property
-    def url(self):
-        return self.http_request.url
+    def status_code(self) -> int:
+        """HTTP status code"""
+        return self._http_response.status_code
 
-    @url.setter
-    def url(self, url):
-        '''Set the url.
-
-        :param url: URL of API endpoint
-        :type url: str
-        '''
-        self.http_request.url = httpx.URL(url)
+    def json(self) -> dict:
+        """Response json"""
+        return self._http_response.json()
 
 
-class Response:
-    '''Handles the Planet server's response to a HTTP request.
+class StreamingResponse(Response):
 
-    :param request: Request that was submitted to the server
-    :type request: :py:Class:`Request`
-    :param http_response: Response that was received from the server
-    :type http_response: :py:Class:`requests.models.Response`
-    '''
-
-    def __init__(self, request, http_response):
-        self.request = request
-        self.http_response = http_response
+    @property
+    def headers(self) -> httpx.Headers:
+        return self._http_response.headers
 
-    def __repr__(self):
-        return f'<models.Response [{self.status_code}]>'
+    @property
+    def url(self) -> str:
+        return str(self._http_response.url)
 
     @property
-    def status_code(self):
-        '''HTTP status code.
+    def num_bytes_downloaded(self) -> int:
+        return self._http_response.num_bytes_downloaded
 
-        :returns: status code
-        :rtype: int
-        '''
-        return self.http_response.status_code
-
-    def json(self):
-        '''Get response json.
-
-        :returns:response json
-        :rtype: dict
-        '''
-        return self.http_response.json()
+    async def aiter_bytes(self):
+        async for c in self._http_response.aiter_bytes():
+            yield c
 
     async def aclose(self):
-        await self.http_response.aclose()
+        await self._http_response.aclose()
 
 
 class StreamingBody:
-    '''A representation of a streaming resource from the API.
+    """A representation of a streaming resource from the API."""
 
-    :param response: Response that was received from the server
-    :type response: :py:Class:`requests.models.Response`
-        '''
-
-    def __init__(self, response):
-        self.response = response.http_response
-        self.url = response.request.url
+    def __init__(self, response: StreamingResponse):
+        """Initialize the object.
+
+        Parameters:
+            response: Response that was received from the server.
+        """
+        self._response = response
 
     @property
-    def name(self):
-        '''The name of this resource.
+    def name(self) -> str:
+        """The name of this resource.
+
         The default is to use the content-disposition header value from the
         response. If not found, falls back to resolving the name from the url
         or generating a random name with the type from the response.
-
-        :returns: name of this resource
-        :rtype: str
-        '''
-        name = (_get_filename_from_headers(self.response.headers)
-                or _get_filename_from_url(self.url) or _get_random_filename(
-                    self.response.headers.get('content-type')))
+        """
+        name = (_get_filename_from_headers(self._response.headers)
+                or _get_filename_from_url(self._response.url)
+                or _get_random_filename(
+                    self._response.headers.get('content-type')))
         return name
 
     @property
-    def size(self):
-        '''The size of the body.
-
-        :returns: size of the body
-        :rtype: int
-        '''
-        return int(self.response.headers['Content-Length'])
-
-    @property
-    def num_bytes_downloaded(self):
-        '''The number of bytes downloaded.
-
-        :returns: number of bytes downloaded
-        :rtype: int
-        '''
-        return self.response.num_bytes_downloaded
-
-    def last_modified(self):
-        '''Read the last-modified header as a datetime, if present.
-
-        :returns: last-modified header
-        :rtype: datatime or None
-        '''
-        lm = self.response.headers.get('last-modified', None)
-        return datetime.strptime(lm, '%a, %d %b %Y %H:%M:%S GMT') if lm \
-            else None
-
-    async def aiter_bytes(self):
-        async for c in self.response.aiter_bytes():
-            yield c
+    def size(self) -> int:
+        """The size of the body."""
+        return int(self._response.headers['Content-Length'])
 
     async def write(self,
                     filename: Path,
                     overwrite: bool = True,
                     progress_bar: bool = True):
         """Write the body to a file.
-
         Parameters:
             filename: Name to assign to downloaded file.
             overwrite: Overwrite any existing files.
             progress_bar: Show progress bar during download.
         """
 
         class _LOG:
@@ -217,18 +147,18 @@
                             disable=progress_bar)
                 with tqdm(total=self.size,
                           unit_scale=True,
                           unit_divisor=unit,
                           unit='B',
                           desc=str(filename),
                           disable=not progress_bar) as progress:
-                    previous = self.num_bytes_downloaded
-                    async for chunk in self.aiter_bytes():
+                    previous = self._response.num_bytes_downloaded
+                    async for chunk in self._response.aiter_bytes():
                         fp.write(chunk)
-                        new = self.num_bytes_downloaded
+                        new = self._response.num_bytes_downloaded
                         _log.update(new)
                         progress.update(new - previous)
                         previous = new
         except FileExistsError:
             LOGGER.info(f'File {filename} exists, not overwriting')
 
 
@@ -274,39 +204,34 @@
     Each returned result is a JSON dict.
     """
     LINKS_KEY = '_links'
     NEXT_KEY = 'next'
     ITEMS_KEY = 'items'
 
     def __init__(self,
-                 request: Request,
-                 do_request_fcn: typing.Callable,
+                 response: Response,
+                 request_fcn: Callable,
                  limit: int = 0):
         """
         Parameters:
             request: Request to send to server for first page.
-            do_request_fcn: Function for submitting a request. Must take in
-                Request object and return Response.
+            request_fcn: Function for submitting a request and retrieving a
+            result. Must take in url and method parameters.
             limit: Maximum number of results to return. When set to 0, no
                 maximum is applied.
         """
-        self.request = request
-        self._do_request = do_request_fcn
+        self._request_fcn = request_fcn
 
-        self._pages = self._get_pages()
+        self._pages = self._get_pages(response)
 
-        self._items: typing.List[dict] = []
+        self._items: List[dict] = []
 
         self.i = 0
         self.limit = limit
 
-    @staticmethod
-    def _next_page_request(url):
-        return Request(url, 'GET')
-
     def __aiter__(self):
         return self
 
     async def __anext__(self) -> dict:
         # This was implemented because traversing _get_pages()
         # in an async generator was resulting in retrieving all the
         # pages, when the goal is to stop retrieval when the limit
@@ -324,39 +249,37 @@
                 item = self._items.pop(0)
                 self.i += 1
             except IndexError:
                 raise StopAsyncIteration
 
         return item
 
-    async def _get_pages(self) -> typing.AsyncGenerator:
-        LOGGER.debug('getting first page')
-        resp = await self._do_request(self.request)
-        page = resp.json()
+    async def _get_pages(self, response) -> AsyncGenerator:
+        page = response.json()
         yield page
 
         next_url = self._next_link(page)
         while (next_url):
             LOGGER.debug('getting next page')
-            request = self._next_page_request(next_url)
-            resp = await self._do_request(request)
-            page = resp.json()
-            yield page
+            response = await self._request_fcn(url=next_url, method='GET')
+            page = response.json()
 
             # If the next URL is the same as the previous URL we will
             # get the same response and be stuck in a page cycle. This
             # has happened in development and could happen in the case
             # of a bug in the production API.
             prev_url = next_url
             next_url = self._next_link(page)
 
             if next_url == prev_url:
                 raise PagingError(
                     "Page cycle detected at {!r}".format(next_url))
 
+            yield page
+
     def _next_link(self, page):
         try:
             next_link = page[self.LINKS_KEY][self.NEXT_KEY]
             LOGGER.debug(f'next: {next_link}')
         except KeyError:
             LOGGER.debug('end of the pages')
             next_link = False
```

### Comparing `planet-2.0a5.dev0/planet/order_request.py` & `planet-2.0a6/planet/order_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """Functionality for preparing order details for use in creating an order"""
 from __future__ import annotations  # https://stackoverflow.com/a/33533514
 import logging
-from typing import Any, Dict, List
+from typing import Optional, Any, Dict, List
 
 from . import geojson, specs
 
 LOGGER = logging.getLogger(__name__)
 
 
 def build_request(name: str,
                   products: List[dict],
                   subscription_id: int = 0,
-                  delivery: dict = None,
-                  notifications: dict = None,
-                  order_type: str = None,
-                  tools: List[dict] = None,
-                  stac: dict = None) -> dict:
+                  delivery: Optional[dict] = None,
+                  notifications: Optional[dict] = None,
+                  order_type: Optional[str] = None,
+                  tools: Optional[List[dict]] = None,
+                  stac: Optional[dict] = None) -> dict:
     '''Prepare an order request.
 
     ```python
     >>> from planet.api.order_details import (
     ...     build_request, product, toar_tool, reproject_tool, tile_tool)
     ...
     >>> products = [
@@ -92,15 +92,15 @@
 
     return details
 
 
 def product(item_ids: List[str],
             product_bundle: str,
             item_type: str,
-            fallback_bundle: str = None) -> dict:
+            fallback_bundle: Optional[str] = None) -> dict:
     '''Product description for an order detail.
 
     Parameters:
         item_ids: IDs of the catalog items to include in the order.
         product_bundle: Set of asset types for the catalog items.
         item_type: The class of spacecraft and processing characteristics
             for the catalog items.
@@ -127,32 +127,32 @@
         'item_ids': item_ids,
         'item_type': item_type,
         'product_bundle': validated_product_bundle
     }
     return product_dict
 
 
-def notifications(email: bool = None,
-                  webhook_url: str = None,
-                  webhook_per_order: bool = None) -> dict:
+def notifications(email: Optional[bool] = None,
+                  webhook_url: Optional[str] = None,
+                  webhook_per_order: Optional[bool] = None) -> dict:
     '''Notifications description for an order detail.
 
     Parameters:
         email: Enable email notifications for an order.
         webhook_url: URL for notification when the order is ready.
         webhook_per_order: Request a single webhook call per order instead
             of one call per each delivered item.
     '''
     return dict((k, v) for k, v in locals().items() if v)
 
 
-def delivery(archive_type: str = None,
+def delivery(archive_type: Optional[str] = None,
              single_archive: bool = False,
-             archive_filename: str = None,
-             cloud_config: dict = None) -> dict:
+             archive_filename: Optional[str] = None,
+             cloud_config: Optional[dict] = None) -> dict:
     '''Order delivery configuration.
 
     Example:
         ```python
         amazon_s3_config = amazon_s3(
             'access_key',
             'secret_access_key',
@@ -192,15 +192,15 @@
     return config
 
 
 def amazon_s3(aws_access_key_id: str,
               aws_secret_access_key: str,
               bucket: str,
               aws_region: str,
-              path_prefix: str = None) -> dict:
+              path_prefix: Optional[str] = None) -> dict:
     '''Amazon S3 Cloud configuration.
 
     Parameters:
         aws_access_key_id: S3 account access key.
         aws_secret_access_key: S3 account secret key.
         bucket: The name of the bucket that will receive the order output.
         aws_region: The region where the bucket lives in AWS.
@@ -220,16 +220,16 @@
 
     return {'amazon_s3': cloud_details}
 
 
 def azure_blob_storage(account: str,
                        container: str,
                        sas_token: str,
-                       storage_endpoint_suffix: str = None,
-                       path_prefix: str = None) -> dict:
+                       storage_endpoint_suffix: Optional[str] = None,
+                       path_prefix: Optional[str] = None) -> dict:
     '''Azure Blob Storage configuration.
 
     Parameters:
         account: Azure account.
         container: ABS container name.
         sas_token: Shared-Access Signature token. Token should be specified
             without a leading '?'.
@@ -251,15 +251,15 @@
         cloud_details['path_prefix'] = path_prefix
 
     return {'azure_blob_storage': cloud_details}
 
 
 def google_cloud_storage(bucket: str,
                          credentials: str,
-                         path_prefix: str = None) -> dict:
+                         path_prefix: Optional[str] = None) -> dict:
     '''Google Cloud Storage configuration.
 
     Parameters:
         bucket: GCS bucket name.
         credentials: JSON-string of service account for bucket.
         path_prefix: Custom string to prepend to the files delivered to the
             bucket. A slash (/) character will be treated as a "folder".
@@ -364,16 +364,16 @@
             'COG' or 'PL_NITF'
     '''
     file_format = specs.validate_file_format(file_format)
     return _tool('file_format', {'format': file_format})
 
 
 def reproject_tool(projection: str,
-                   resolution: float = None,
-                   kernel: str = None) -> dict:
+                   resolution: Optional[float] = None,
+                   kernel: Optional[str] = None) -> dict:
     '''Create the API spec representation of a reproject tool.
 
     Parameters:
         projection: A coordinate system in the form EPSG:n. (ex. EPSG:4326 for
             WGS84, EPSG:32611 for UTM 11 North (WGS84), or EPSG:3857 for Web
             Mercator).
         resolution: The pixel width and height in the output file. The API
@@ -385,19 +385,19 @@
             "lanczos", "average" and "mode".
     '''
     parameters = dict((k, v) for k, v in locals().items() if v)
     return _tool('reproject', parameters)
 
 
 def tile_tool(tile_size: int,
-              origin_x: float = None,
-              origin_y: float = None,
-              pixel_size: float = None,
-              name_template: str = None,
-              conformal_x_scaling: bool = None) -> dict:
+              origin_x: Optional[float] = None,
+              origin_y: Optional[float] = None,
+              pixel_size: Optional[float] = None,
+              name_template: Optional[str] = None,
+              conformal_x_scaling: Optional[bool] = None) -> dict:
     '''Create the API spec representation of a reproject tool.
 
     Parameters:
         tile_size: Height and width of output tiles in pixels and lines
             (always square).
         origin_x: Tiling system x origin in projected coordinates. The API
             default is zero.
@@ -410,15 +410,15 @@
             like 128_200.tif. The {tilex} and {tiley} parameters can be of the
             form {tilex:06d} to produce a fixed width field with leading zeros.
     '''
     parameters = dict((k, v) for k, v in locals().items() if v)
     return _tool('tile', parameters)
 
 
-def toar_tool(scale_factor: int = None, ) -> dict:
+def toar_tool(scale_factor: Optional[int] = None, ) -> dict:
     '''Create the API spec representation of a TOAR tool.
 
     Parameters:
         scale_factor: Scale factor applied to convert 0.0 to 1.0 reflectance
             floating point values to a value that fits in 16bit integer pixels.
             The API default is 10000. Values over 65535 could result in high
             reflectances not fitting in 16bit integers.
```

### Comparing `planet-2.0a5.dev0/planet/reporting.py` & `planet-2.0a6/planet/reporting.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 """Functionality for reporting progress."""
 import logging
+from typing import Optional
 
 from tqdm.asyncio import tqdm
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ProgressBar:
@@ -53,16 +54,16 @@
             bar.update(state='created', order_id='oid')
             ...
         ```
     """
 
     def __init__(
         self,
-        order_id: str = None,
-        state: str = None,
+        order_id: Optional[str] = None,
+        state: Optional[str] = None,
         disable: bool = False,
     ):
         """Initialize the object.
 
         Parameters:
             order_id: Id of the order.
             state: State of the order.
@@ -84,15 +85,17 @@
     def desc(self):
         return f'order {self.order_id}'
 
     def update_state(self, state: str):
         """Simple function to be used as a callback for state reporting"""
         self.update(state=state)
 
-    def update(self, state: str = None, order_id: str = None):
+    def update(self,
+               state: Optional[str] = None,
+               order_id: Optional[str] = None):
         if state:
             self.state = state
             if self.bar is not None:
                 try:
                     self.bar.postfix[1] = self.state
                 except AttributeError:
                     # If the bar is disabled, attempting to access
```

### Comparing `planet-2.0a5.dev0/planet/specs.py` & `planet-2.0a6/planet/specs.py`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/planet.egg-info/PKG-INFO` & `planet-2.0a6/planet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.0a5.dev0
+Version: 2.0a6
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.0a5.dev0/planet.egg-info/SOURCES.txt` & `planet-2.0a6/planet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planet-2.0a5.dev0/setup.py` & `planet-2.0a6/setup.py`

 * *Files identical despite different names*

