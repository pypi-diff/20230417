# Comparing `tmp/customvalidator-0.1.tar.gz` & `tmp/customvalidator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customvalidator-0.1.tar", last modified: Sat Mar 25 03:43:10 2023, max compression
+gzip compressed data, was "customvalidator-0.2.tar", last modified: Mon Apr 17 10:54:52 2023, max compression
```

## Comparing `customvalidator-0.1.tar` & `customvalidator-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 03:43:10.340262 customvalidator-0.1/
--rw-rw-rw-   0        0        0       60 2023-03-25 03:43:10.340262 customvalidator-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-25 03:43:10.315106 customvalidator-0.1/customdbcred/
--rw-rw-rw-   0        0        0     1693 2023-03-25 02:47:42.000000 customvalidator-0.1/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 03:43:10.321105 customvalidator-0.1/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-03-24 14:09:22.000000 customvalidator-0.1/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 03:43:10.322121 customvalidator-0.1/customvalidator/
--rw-rw-rw-   0        0        0      926 2023-03-25 03:37:23.000000 customvalidator-0.1/customvalidator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 03:43:10.338243 customvalidator-0.1/customvalidator.egg-info/
--rw-rw-rw-   0        0        0       60 2023-03-25 03:43:10.000000 customvalidator-0.1/customvalidator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-03-25 03:43:10.000000 customvalidator-0.1/customvalidator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 03:43:10.000000 customvalidator-0.1/customvalidator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-25 03:43:10.000000 customvalidator-0.1/customvalidator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 03:43:10.340262 customvalidator-0.1/setup.cfg
--rw-rw-rw-   0        0        0      204 2023-03-25 03:41:48.000000 customvalidator-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:52.359898 customvalidator-0.2/
+-rw-rw-rw-   0        0        0       60 2023-04-17 10:54:52.358951 customvalidator-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:52.333760 customvalidator-0.2/customdbcred/
+-rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customvalidator-0.2/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:52.334761 customvalidator-0.2/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customvalidator-0.2/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:52.336760 customvalidator-0.2/customvalidator/
+-rw-rw-rw-   0        0        0      926 2023-03-25 03:37:23.000000 customvalidator-0.2/customvalidator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 10:54:52.356890 customvalidator-0.2/customvalidator.egg-info/
+-rw-rw-rw-   0        0        0       60 2023-04-17 10:54:52.000000 customvalidator-0.2/customvalidator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-17 10:54:52.000000 customvalidator-0.2/customvalidator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 10:54:52.000000 customvalidator-0.2/customvalidator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-17 10:54:52.000000 customvalidator-0.2/customvalidator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 10:54:52.359898 customvalidator-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      204 2023-04-17 10:54:34.000000 customvalidator-0.2/setup.py
```

### Comparing `customvalidator-0.1/customdbcred/__init__.py` & `customvalidator-0.2/customdbcred/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 # Custom Module to fetch database credentials
 import logging
 from functools import wraps
 
 from azure.keyvault.secrets import SecretClient
 from azure.identity import ClientSecretCredential
 
+logger_error = logging.getLogger('error_logs')
+
 
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

### Comparing `customvalidator-0.1/customstatuscodes/__init__.py` & `customvalidator-0.2/customstatuscodes/__init__.py`

 * *Files identical despite different names*

### Comparing `customvalidator-0.1/customvalidator/__init__.py` & `customvalidator-0.2/customvalidator/__init__.py`

 * *Files identical despite different names*

