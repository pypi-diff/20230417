# Comparing `tmp/netsuite_python-1.3.8.tar.gz` & `tmp/netsuite_python-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.3.8.tar", last modified: Wed Apr 12 21:53:31 2023, max compression
+gzip compressed data, was "netsuite_python-1.4.0.tar", last modified: Mon Apr 17 18:32:26 2023, max compression
```

## Comparing `netsuite_python-1.3.8.tar` & `netsuite_python-1.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.836536 netsuite_python-1.3.8/
--rw-rw-rw-   0        0        0    12699 2023-04-12 21:53:31.836536 netsuite_python-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    12368 2023-04-12 21:14:15.000000 netsuite_python-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.821083 netsuite_python-1.3.8/netsuite/
--rw-rw-rw-   0        0        0    11858 2023-04-12 21:38:42.000000 netsuite_python-1.3.8/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.823526 netsuite_python-1.3.8/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.3.8/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.826535 netsuite_python-1.3.8/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.3.8/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.3.8/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.3.8/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.3.8/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.3.8/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.3.8/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.827535 netsuite_python-1.3.8/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0     8422 2023-04-12 21:53:28.000000 netsuite_python-1.3.8/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6306 2023-04-12 21:38:42.000000 netsuite_python-1.3.8/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.830535 netsuite_python-1.3.8/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.3.8/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:53:31.835536 netsuite_python-1.3.8/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0    12699 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 21:53:31.000000 netsuite_python-1.3.8/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 21:53:31.836536 netsuite_python-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-04-12 21:53:28.000000 netsuite_python-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.306775 netsuite_python-1.4.0/
+-rw-rw-rw-   0        0        0    12699 2023-04-17 18:32:26.306775 netsuite_python-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    12368 2023-04-12 21:14:15.000000 netsuite_python-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.278992 netsuite_python-1.4.0/netsuite/
+-rw-rw-rw-   0        0        0    13726 2023-04-17 18:30:10.000000 netsuite_python-1.4.0/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.286775 netsuite_python-1.4.0/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.4.0/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.291774 netsuite_python-1.4.0/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.4.0/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.4.0/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.4.0/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.4.0/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.4.0/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.4.0/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.293778 netsuite_python-1.4.0/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0     8422 2023-04-12 21:53:28.000000 netsuite_python-1.4.0/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.4.0/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.300775 netsuite_python-1.4.0/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.4.0/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:32:26.305775 netsuite_python-1.4.0/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0    12699 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 18:32:26.000000 netsuite_python-1.4.0/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 18:32:26.306775 netsuite_python-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-04-17 18:32:00.000000 netsuite_python-1.4.0/setup.py
```

### Comparing `netsuite_python-1.3.8/PKG-INFO` & `netsuite_python-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite_python
-Version: 1.3.8
+Version: 1.4.0
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.8/README.md` & `netsuite_python-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/Netsuite.py` & `netsuite_python-1.4.0/netsuite/Netsuite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 import json
+import os.path
 import pathlib
 import jwt
 from datetime import datetime, timedelta
 from pathlib import Path
+import importlib
+
+import importlib.util
+import netsuite.settings
 import requests
 from netsuite.NetsuiteToken import NetsuiteToken
 # from netsuite.swagger_client.restlet_client import RestletClient
 from netsuite.settings import APISettings
 from netsuite.storages import BaseStorage, JSONStorage
 from netsuite import api_clients
 
 
-client_exists = False
-try:
-    import netsuite_rest_client
-    from netsuite_rest_client.api import *
-    client_exists = True
-except ModuleNotFoundError or ImportError as err:
-    print('Rest Client needs to be generated')
+# client_exists = False
+# try:
+#     # base_dir = str(netsuite.settings.NETSUITE_CLIENT_DIR)
+#     api_client  = importlib.util.find_spec('netsuite_rest_client', str(netsuite.settings.NETSUITE_CLIENT_DIR))
+#     if api_client is None:
+#         print("Run 'netsuite generate-rest-client' after getting a token")
+#     else:
+#         netsuite_rest_client = api_client.loader.load_module()
+#     # apis = importlib.import_module('netsuite_rest_client.apis')
+#     # print(apis)
+#
+#     # print(my_module.loader.load_module())
+#     # from base_dir import *
+#     # import netsuite.netsuite_rest_client
+#     # from netsuite.netsuite_rest_client import *
+#     client_exists = True
+# except ModuleNotFoundError or ImportError as err:
+#     print(err)
+#     print('Rest Client needs to be generated')
+
 
 
 class Netsuite:
     app_name: str = None
     storage: BaseStorage = None
     api_settings: APISettings
-    rest_client = None
     query_client = None
     restlet_client = None
 
     def __init__(self, config: dict = None, config_file: Path = None):
         if config and config_file:
             raise ValueError("You can only load settings from one source")
         if config_file:
@@ -66,26 +83,31 @@
             if not self.api_settings.JSON_STORAGE_PATH:
                 raise Exception("JSON_STORAGE_PATH must be defined for JSONStorage")
             self.storage.storage_path = self.api_settings.JSON_STORAGE_PATH
         self.rest_url = f"https://{self.api_settings.NETSUITE_APP_NAME}.suitetalk.api.netsuite.com/services/rest" \
                         f"/record/v1/ "
         self.access_token_url = f"https://{self.api_settings.NETSUITE_APP_NAME}.suitetalk.api.netsuite.com/services/rest/auth/oauth2/v1/token",
 
-    @property
-    def REST_CLIENT(self):
-        try:
-            if not self.rest_client:
-                if client_exists:
-                    self.rest_client = self.get_rest_client()
-
-                    return self.rest_client
-            else:
-                print('Client needs to be generated.')
-        except Exception as e:
-            print(e)
+    # @property
+    # def REST_CLIENT(self):
+    #     print('ah')
+    #     if not self.rest_client:
+    #         self.rest_client = self.RestClient(self).api_client
+    #     return self.rest_client
+    #     # try:
+    #     #     if not self.rest_client:
+    #     #         if client_exists:
+    #     #             self.rest_client = self.RestClient(self).api_client
+    #     #
+    #     #             self.customer_api = apis.CustomerApi(self.rest_client)
+    #     #             return self.rest_client
+    #     #     else:
+    #     #         print('Client needs to be generated.')
+    #     # except Exception as e:
+    #     #     print(e)
 
 
     @property
     def QUERY_CLIENT(self):
         if not self.query_client:
             self.query_client = self.QueryClient(self)
             # if self.token.access_token is not None:
@@ -165,15 +187,15 @@
             'Authorization': f'Bearer {token.access_token}'
         }
         response = requests.get(url, headers=headers, params=params)
         # print(token.access_token)
         # print(response.json())
         data = {
             'options': {
-                'packageName': 'netsuite_client'
+                'packageName': 'netsuite_rest_client'
             },
             'generateSourceCodeOnly': 'True',
             'spec': response.json()
         }
         headers2 = {
             'Content-Type': 'application/json'
         }
@@ -190,42 +212,66 @@
         req = requests.get(url)
         print('Downloading Completed')
 
         # extracting the zip file contents
         file = zipfile.ZipFile(BytesIO(req.content))
         file.extractall(path=self.api_settings.NETSUITE_CLIENT_PATH)
 
-        src = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client/netsuite_client')
-        dst = Path(self.api_settings.NETSUITE_CLIENT_PATH)
-        shutil.copytree(src, dst, symlinks=False, ignore=None, ignore_dangling_symlinks=False,
+
+        client_src = Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), f'python-client/netsuite_rest_client')
+        class_src = Path.joinpath(Path(netsuite.settings.PACKAGE_DIR), f'netsuite_rest_client/rest_api_client.py')
+        dst = Path(f'{self.api_settings.NETSUITE_CLIENT_PATH}')
+
+        shutil.copytree(client_src, dst, symlinks=True, ignore=None, ignore_dangling_symlinks=False,
                         dirs_exist_ok=True)
+
+        shutil.copy(class_src, dst)
+
         print('Netsuite Rest Client Created')
-        # shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
-        # print('temp folder removed.')
+        shutil.rmtree(Path.joinpath(Path(self.api_settings.NETSUITE_CLIENT_PATH), 'python-client'))
+        print('temp folder removed.')
 
-        # with open("./client_schema.json", "w") as outfile:
-        #     outfile.write(json.dumps(response.json()))
+        print('\n Netsuite is Ready To Go!')
+        print('Usage Example')
+        print('\n ----------------------')
+        print('\nfrom netsuite import Netsuite'
+              '\nfrom netsuite_rest_client import apis, rest_api_client'
+              '\nnetsuite = Netsuite()'
+              '\nrest_client = rest_api_client.RestApiClient(netsuite)'
+              '\ncustomer_api = apis.CustomerApi(rest_client)')
 
     def get_token(self):
         if not self.token.is_expired:
             return self.token
         else:
             return self.request_access_token()
 
 
-    def get_rest_client(self):
-        configuration = netsuite_rest_client.configuration.Configuration(
-            host=f"https://{self.netsuite_app_name}.suitetalk.api.netsuite.com/services/rest/record/v1"
-        )
-
-        configuration.api_key['OAuth_1.0_authorization'] = self.get_token().access_token
-        configuration.api_key_prefix['OAuth_1.0_authorization'] = 'Bearer'
-        rest_client.api_client = netsuite_rest_client.api_client.ApiClient(configuration=configuration)
-        rest_client.customer_api = netsuite_rest_client.api.customer_api.CustomerApi(api_client)
-        return rest_client
+    # def get_rest_client(self):
+    #     configuration = netsuite_rest_client.configuration.Configuration(
+    #         host=f"https://{self.netsuite_app_name}.suitetalk.api.netsuite.com/services/rest/record/v1"
+    #     )
+    #
+    #     configuration.api_key['OAuth_1.0_authorization'] = self.get_token().access_token
+    #     configuration.api_key_prefix['OAuth_1.0_authorization'] = 'Bearer'
+    #     rest_client.api_client = netsuite_rest_client.api_client.ApiClient(configuration=configuration)
+    #     rest_client.customer_api = netsuite_rest_client.api.customer_api.CustomerApi(api_client)
+    #     return rest_client
+    #
+    # class RestClient:
+    #     def __init__(self, netsuite):
+    #         print('ah2')
+    #         self.netsuite = netsuite
+    #         self.configuration = netsuite_rest_client.configuration.Configuration()
+    #         self.configuration.host = f"https://{netsuite.netsuite_app_name}.suitetalk.api.netsuite.com/services/rest/record/v1"
+    #         self.configuration.api_key['OAuth_1.0_authorization'] = self.netsuite.get_token().access_token
+    #         self.configuration.api_key_prefix['OAuth_1.0_authorization'] = 'Bearer'
+    #         self.api_client = netsuite_rest_client.api_client.ApiClient(configuration=self.configuration)
+
+
 
 
     class QueryClient:
         def __init__(self, netsuite):
             self.netsuite = netsuite
             self.configuration = api_clients.Configuration()
             self.configuration.token = netsuite.storage.get_token(netsuite.app_name)
@@ -246,17 +292,14 @@
             self.configuration.token = netsuite.storage.get_token(netsuite.app_name)
             self.configuration.token_refresh_hook = self.refresh_token
             self.configuration.app_name = netsuite.netsuite_app_name
             self.configuration.host = f"https://{self.configuration.app_name}.restlets.api.netsuite.com/app/site/hosting/restlet.nl"
             self.api_client = api_clients.ApiClient(configuration=self.configuration)
             self.restlet_api = api_clients.RestletApi(api_client=self.api_client)
 
-            # self.contact_api = swagger_client.ContactApi(api_client=self.api_client)
-            # self.customer_api = swagger_client.CustomerApi(api_client=self.api_client)
-            # self.message_api = swagger_client.MessageApi(api_client=self.api_client)
 
         def refresh_token(self):
             self.configuration.token = self.netsuite.get_token()
             return self.configuration.token
 
     # def get_status_dict(self):
     #     if self.token.access_token is None:
```

### Comparing `netsuite_python-1.3.8/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.4.0/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.4.0/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/api_clients/api_client.py` & `netsuite_python-1.4.0/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/api_clients/configuration.py` & `netsuite_python-1.4.0/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/api_clients/rest.py` & `netsuite_python-1.4.0/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/module_loading.py` & `netsuite_python-1.4.0/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/scripts/cli.py` & `netsuite_python-1.4.0/netsuite/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/settings.py` & `netsuite_python-1.4.0/netsuite/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     settings = None
 
 BASE_DIR = Path(__file__).parent.parent.parent.parent.parent.parent.resolve()
 BASE_CONFIG_DIR = Path.joinpath(BASE_DIR, 'config')
 NETSUITE_CONFIG_DIR = Path.joinpath(BASE_CONFIG_DIR, 'netsuite')
 NETSUITE_TOKENS_DIR = Path.joinpath(BASE_CONFIG_DIR, 'tokens')
 PACKAGE_DIR = Path(__file__).parent.resolve()
-NETSUITE_CLIENT_DIR = Path.joinpath(PACKAGE_DIR, 'netsuite_rest_client')
+NETSUITE_CLIENT_DIR = Path.joinpath(BASE_DIR, 'netsuite_rest_client')
 
 if not os.path.exists(NETSUITE_CONFIG_DIR):
     os.makedirs(NETSUITE_CONFIG_DIR)
 if not os.path.exists(NETSUITE_TOKENS_DIR):
     os.makedirs(NETSUITE_TOKENS_DIR)
 if not os.path.exists(NETSUITE_CLIENT_DIR):
     os.makedirs(NETSUITE_CLIENT_DIR)
@@ -69,15 +69,15 @@
 
 
     'STORAGE_CLASS': 'netsuite.storages.JSONStorage',
     'CREDENTIALS_PATH': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_credentials.json')),
     'JSON_STORAGE_PATH': str(Path.joinpath(NETSUITE_TOKENS_DIR, 'netsuite_tokens.json')),
     'NETSUITE_CERTIFICATE_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_certificate.pem')),
     'NETSUITE_KEY_FILE': str(Path.joinpath(NETSUITE_CONFIG_DIR, 'netsuite_key.pem')),
-    'NETSUITE_CLIENT_PATH': str(Path.joinpath(PACKAGE_DIR, 'netsuite_rest_client')),
+    'NETSUITE_CLIENT_PATH': str(Path.joinpath(BASE_DIR, 'netsuite_rest_client')),
     'APP_NAME': 'default',
 }
 
 # List of settings that may be in string import notation.
 IMPORT_STRINGS = [
     'DEFAULT_STORAGE_CLASSES',
     'STORAGE_CLASS',
```

### Comparing `netsuite_python-1.3.8/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.4.0/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite/storages/JSONStorage.py` & `netsuite_python-1.4.0/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.4.0/netsuite_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.3.8
+Version: 1.4.0
 Summary: Python SDK for Netsuite API with Django Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `netsuite_python-1.3.8/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.4.0/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.3.8/setup.py` & `netsuite_python-1.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.3.8',
+    version='1.4.0',
     description='Python SDK for Netsuite API with Django Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

