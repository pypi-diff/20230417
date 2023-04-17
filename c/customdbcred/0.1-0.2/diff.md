# Comparing `tmp/customdbcred-0.1.tar.gz` & `tmp/customdbcred-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customdbcred-0.1.tar", last modified: Sat Mar 25 02:49:27 2023, max compression
+gzip compressed data, was "customdbcred-0.2.tar", last modified: Mon Apr 17 10:26:57 2023, max compression
```

## Comparing `customdbcred-0.1.tar` & `customdbcred-0.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 02:49:27.481104 customdbcred-0.1/
--rw-rw-rw-   0        0        0       57 2023-03-25 02:49:27.480103 customdbcred-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-25 02:49:27.459104 customdbcred-0.1/custom_mod/
--rw-rw-rw-   0        0        0     1710 2023-03-24 11:08:28.000000 customdbcred-0.1/custom_mod/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 02:49:27.461104 customdbcred-0.1/customdbcred/
--rw-rw-rw-   0        0        0     1693 2023-03-25 02:47:42.000000 customdbcred-0.1/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 02:49:27.477105 customdbcred-0.1/customdbcred.egg-info/
--rw-rw-rw-   0        0        0       57 2023-03-25 02:49:27.000000 customdbcred-0.1/customdbcred.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-03-25 02:49:27.000000 customdbcred-0.1/customdbcred.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 02:49:27.000000 customdbcred-0.1/customdbcred.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-03-25 02:49:27.000000 customdbcred-0.1/customdbcred.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-25 02:49:27.478104 customdbcred-0.1/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-03-24 14:09:22.000000 customdbcred-0.1/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 02:49:27.480103 customdbcred-0.1/customvalidator/
--rw-rw-rw-   0        0        0        0 2023-03-24 13:05:03.000000 customdbcred-0.1/customvalidator/__init__.py
--rw-rw-rw-   0        0        0       42 2023-03-25 02:49:27.481104 customdbcred-0.1/setup.cfg
--rw-rw-rw-   0        0        0      201 2023-03-25 02:49:24.000000 customdbcred-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.588695 customdbcred-0.2/
+-rw-rw-rw-   0        0        0       57 2023-04-17 10:26:57.588695 customdbcred-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.551450 customdbcred-0.2/customdbcred/
+-rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customdbcred-0.2/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.571060 customdbcred-0.2/customdbcred.egg-info/
+-rw-rw-rw-   0        0        0       57 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 10:26:57.000000 customdbcred-0.2/customdbcred.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.578596 customdbcred-0.2/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customdbcred-0.2/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:26:57.586658 customdbcred-0.2/customvalidator/
+-rw-rw-rw-   0        0        0      926 2023-03-25 03:37:23.000000 customdbcred-0.2/customvalidator/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:26:57.589674 customdbcred-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      201 2023-04-17 10:26:39.000000 customdbcred-0.2/setup.py
```

### Comparing `customdbcred-0.1/custom_mod/__init__.py` & `customdbcred-0.2/customdbcred/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,41 @@
+# Custom Module to fetch database credentials
 import logging
 from functools import wraps
 
 from azure.keyvault.secrets import SecretClient
 from azure.identity import ClientSecretCredential
 
-
-def my_function():
-    print('hello')
-    return 'hello'
+logger_error = logging.getLogger('error_logs')
 
 
 def get_db_cred(func):
     @wraps(func)
     def wrapper_func(req):
-        keyVaultName = "myappkv"
-        KVUri = f"https://{keyVaultName}.vault.azure.net"
-        # credential = DefaultAzureCredential()
-        credential = ClientSecretCredential(tenant_id='26afc1b1-8393-439d-aa1a-483105d77dc3',
-                                            client_id='9d2fe19f-47e6-498f-b384-6f94b0d55500',
-                                            client_secret='lwk8Q~4LbZTagzrC6l0bpwrmraDrEQIalVZnfaf1')
-
-        client = SecretClient(vault_url=KVUri, credential=credential)
-        server = client.get_secret("SERVER").value
-        database = client.get_secret("DATABASE").value
-        username = client.get_secret("USERNAME").value
-        password = client.get_secret("PASSWORD").value
-        driver = '{ODBC Driver 17 for SQL Server}'
-        # Some code to execute before the decorated function is called
-        # payload = [server, database, username, password, driver]
-        output_json = dict(zip(["server", "database", "username", "password", "driver"],
-                               [server, database, username, password, driver]))
-        # output_json = dict(zip(["Status", "Message", "Payload"],["200", "Success", payload]))
-        request_data = req.get_json()
-        request_data.update(output_json)
-
-        result = func(request_data)
-        # Some code to execute after the decorated function is called
-        return result
+        try:
+            if type(req) == dict:
+                result = func(req)
+                return result
+            keyVaultName = "myappkv"
+            KVUri = f"https://{keyVaultName}.vault.azure.net"
+            # credential = DefaultAzureCredential()
+            credential = ClientSecretCredential(tenant_id='26afc1b1-8393-439d-aa1a-483105d77dc3',
+                                                client_id='9d2fe19f-47e6-498f-b384-6f94b0d55500',
+                                                client_secret='lwk8Q~4LbZTagzrC6l0bpwrmraDrEQIalVZnfaf1')
+            client = SecretClient(vault_url=KVUri, credential=credential)
+            server = client.get_secret("SERVER").value
+            database = client.get_secret("DATABASE").value
+            username = client.get_secret("USERNAME").value
+            password = client.get_secret("PASSWORD").value
+            driver = '{ODBC Driver 17 for SQL Server}'
+            output_json = dict(zip(["server", "database", "username", "password", "driver"],
+                                   [server, database, username, password, driver]))
+            request_data = req.get_json()
+            request_data.update(output_json)
+            result = func(request_data)
+            return result
+        except Exception as ex:
+            logger_error.error(f"Exception Encountered Exception is : {ex}", exc_info=1)
+            output_json = dict(zip(['Status', 'Message', 'Payload'], [500, f"Exception encountered: {ex}", None]))
+            result = func(output_json)
+            return func(result)
     return wrapper_func
```

### Comparing `customdbcred-0.1/customstatuscodes/__init__.py` & `customdbcred-0.2/customstatuscodes/__init__.py`

 * *Files identical despite different names*

