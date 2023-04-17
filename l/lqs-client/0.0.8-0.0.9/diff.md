# Comparing `tmp/lqs-client-0.0.8.tar.gz` & `tmp/lqs-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqs-client-0.0.8.tar", last modified: Tue Nov  1 17:37:23 2022, max compression
+gzip compressed data, was "lqs-client-0.0.9.tar", last modified: Wed Nov  2 14:53:18 2022, max compression
```

## Comparing `lqs-client-0.0.8.tar` & `lqs-client-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-01 17:37:23.982845 lqs-client-0.0.8/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3215 2022-11-01 17:37:23.982845 lqs-client-0.0.8/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2716 2022-11-01 17:35:01.000000 lqs-client-0.0.8/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-01 17:37:23.974845 lqs-client-0.0.8/lqs_client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1846 2022-11-01 17:35:32.000000 lqs-client-0.0.8/lqs_client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2022-11-01 15:39:56.000000 lqs-client-0.0.8/lqs_client/__main__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-01 17:37:23.978845 lqs-client-0.0.8/lqs_client/interface/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2022-10-04 18:08:06.000000 lqs-client-0.0.8/lqs_client/interface/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2022-11-01 15:43:34.000000 lqs-client-0.0.8/lqs_client/interface/common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5855 2022-11-01 15:43:34.000000 lqs-client-0.0.8/lqs_client/interface/creator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2022-11-01 15:43:34.000000 lqs-client-0.0.8/lqs_client/interface/deleter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2022-11-01 15:43:34.000000 lqs-client-0.0.8/lqs_client/interface/getter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16405 2022-11-01 17:32:17.000000 lqs-client-0.0.8/lqs_client/interface/lister.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16849 2022-10-04 19:16:48.000000 lqs-client-0.0.8/lqs_client/interface/s3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2221 2022-11-01 15:43:34.000000 lqs-client-0.0.8/lqs_client/interface/updater.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-01 17:37:23.974845 lqs-client-0.0.8/lqs_client.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3215 2022-11-01 17:37:23.000000 lqs-client-0.0.8/lqs_client.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2022-11-01 17:37:23.000000 lqs-client-0.0.8/lqs_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-01 17:37:23.000000 lqs-client-0.0.8/lqs_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2022-11-01 17:37:23.000000 lqs-client-0.0.8/lqs_client.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-01 17:37:23.000000 lqs-client-0.0.8/lqs_client.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-09-29 18:21:02.000000 lqs-client-0.0.8/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-11-01 17:37:23.982845 lqs-client-0.0.8/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2022-11-01 13:59:11.000000 lqs-client-0.0.8/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.956888 lqs-client-0.0.9/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3215 2022-11-02 14:53:18.956888 lqs-client-0.0.9/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2716 2022-11-01 17:35:01.000000 lqs-client-0.0.9/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.948888 lqs-client-0.0.9/lqs_client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1846 2022-11-01 17:35:32.000000 lqs-client-0.0.9/lqs_client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2022-11-01 15:39:56.000000 lqs-client-0.0.9/lqs_client/__main__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.956888 lqs-client-0.0.9/lqs_client/interface/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2022-10-04 18:08:06.000000 lqs-client-0.0.9/lqs_client/interface/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3191 2022-11-02 14:52:48.000000 lqs-client-0.0.9/lqs_client/interface/common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5855 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/creator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/deleter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1959 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/getter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16405 2022-11-01 17:32:17.000000 lqs-client-0.0.9/lqs_client/interface/lister.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16849 2022-10-04 19:16:48.000000 lqs-client-0.0.9/lqs_client/interface/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2221 2022-11-01 15:43:34.000000 lqs-client-0.0.9/lqs_client/interface/updater.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-02 14:53:18.952888 lqs-client-0.0.9/lqs_client.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3215 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-11-02 14:53:18.000000 lqs-client-0.0.9/lqs_client.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      206 2022-09-29 18:21:02.000000 lqs-client-0.0.9/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-11-02 14:53:18.956888 lqs-client-0.0.9/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2022-11-02 14:52:26.000000 lqs-client-0.0.9/setup.py
```

### Comparing `lqs-client-0.0.8/PKG-INFO` & `lqs-client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.0.8/README.md` & `lqs-client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client/__init__.py` & `lqs-client-0.0.9/lqs_client/__init__.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client/interface/common.py` & `lqs-client-0.0.9/lqs_client/interface/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,34 +64,47 @@
     def _get_payload_data(self, args, exclude=[]):
         payload = {}
         for key, value in args.items():
             if value is not None and key not in ["self"] + exclude:
                 payload[key] = value
         return payload
 
+    def _handle_response_data(self, response):
+        try:
+            response_data = response.json()
+        except json.decoder.JSONDecodeError:
+            raise Exception(f"Error: {response.text}")
+        if response.ok:
+            return response_data
+        else:
+            raise Exception(response_data)
+
     def _get_resource(self, resource_path):
         r = requests.get(f"{self._api_url}/{resource_path}", headers=self._headers)
-        results = r.json()
-        return results
+        try:
+            response_data = r.json()
+        except json.decoder.JSONDecodeError:
+            raise Exception(f"Error: {r.text}")
+        if r.ok:
+            return response_data
+        else:
+            raise Exception(response_data)
 
     def _create_resource(self, resource_path, data):
         r = requests.post(
             f"{self._api_url}/{resource_path}",
             data=json.dumps(data),
             headers=self._headers,
         )
-        response_data = r.json()
-        return response_data
+        return self._handle_response_data(r)
 
     def _update_resource(self, resource_path, data):
         r = requests.patch(
             f"{self._api_url}/{resource_path}",
             data=json.dumps(data),
             headers=self._headers,
         )
-        response_data = r.json()
-        return response_data
+        return self._handle_response_data(r)
 
     def _delete_resource(self, resource_path):
         r = requests.delete(f"{self._api_url}/{resource_path}", headers=self._headers)
-        results = r.json()
-        return results
+        return self._handle_response_data(r)
```

### Comparing `lqs-client-0.0.8/lqs_client/interface/creator.py` & `lqs-client-0.0.9/lqs_client/interface/creator.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client/interface/deleter.py` & `lqs-client-0.0.9/lqs_client/interface/deleter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client/interface/getter.py` & `lqs-client-0.0.9/lqs_client/interface/getter.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client/interface/lister.py` & `lqs-client-0.0.9/lqs_client/interface/lister.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client/interface/s3.py` & `lqs-client-0.0.9/lqs_client/interface/s3.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client/interface/updater.py` & `lqs-client-0.0.9/lqs_client/interface/updater.py`

 * *Files identical despite different names*

### Comparing `lqs-client-0.0.8/lqs_client.egg-info/PKG-INFO` & `lqs-client-0.0.9/lqs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqs-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: LogQS Client
 Home-page: https://github.com/carnegierobotics/LogQS-Client
 Author: Nathan Margaglio
 Author-email: nmargaglio@carnegierobotics.com
 Project-URL: Bug Tracker, https://github.com/carnegierobotics/LogQS-Client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lqs-client-0.0.8/setup.py` & `lqs-client-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lqs-client",
-    version="0.0.8",
+    version="0.0.9",
     author="Nathan Margaglio",
     author_email="nmargaglio@carnegierobotics.com",
     description="LogQS Client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/carnegierobotics/LogQS-Client",
     project_urls={
```

