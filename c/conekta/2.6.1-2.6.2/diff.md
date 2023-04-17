# Comparing `tmp/conekta-2.6.1.tar.gz` & `tmp/conekta-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conekta-2.6.1.tar", last modified: Wed Nov 23 21:51:53 2022, max compression
+gzip compressed data, was "conekta-2.6.2.tar", last modified: Mon Apr 17 13:59:08 2023, max compression
```

## Comparing `conekta-2.6.1.tar` & `conekta-2.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 agatto     (501) staff       (20)        0 2022-11-23 21:51:53.430230 conekta-2.6.1/
--rw-r--r--   0 agatto     (501) staff       (20)     2550 2022-11-23 21:49:35.000000 conekta-2.6.1/CHANGELOG.md
--rw-r--r--   0 agatto     (501) staff       (20)     1101 2022-11-23 21:42:55.000000 conekta-2.6.1/LICENSE
--rw-r--r--   0 agatto     (501) staff       (20)       94 2022-11-23 21:42:55.000000 conekta-2.6.1/MANIFEST.in
--rw-r--r--   0 agatto     (501) staff       (20)      754 2022-11-23 21:51:53.429757 conekta-2.6.1/PKG-INFO
--rw-r--r--   0 agatto     (501) staff       (20)     8812 2022-11-23 21:48:21.000000 conekta-2.6.1/README.md
--rw-r--r--   0 agatto     (501) staff       (20)       81 2022-11-23 21:42:55.000000 conekta-2.6.1/README.txt
-drwxr-xr-x   0 agatto     (501) staff       (20)        0 2022-11-23 21:51:53.412127 conekta-2.6.1/conekta/
--rw-r--r--   0 agatto     (501) staff       (20)    24051 2022-11-23 21:48:21.000000 conekta-2.6.1/conekta/__init__.py
-drwxr-xr-x   0 agatto     (501) staff       (20)        0 2022-11-23 21:51:53.417255 conekta-2.6.1/conekta/ssl_data/
--rw-r--r--   0 agatto     (501) staff       (20)   261053 2022-11-23 21:42:55.000000 conekta-2.6.1/conekta/ssl_data/ca_bundle.crt
-drwxr-xr-x   0 agatto     (501) staff       (20)        0 2022-11-23 21:51:53.415992 conekta-2.6.1/conekta.egg-info/
--rw-r--r--   0 agatto     (501) staff       (20)      754 2022-11-23 21:51:53.000000 conekta-2.6.1/conekta.egg-info/PKG-INFO
--rw-r--r--   0 agatto     (501) staff       (20)      467 2022-11-23 21:51:53.000000 conekta-2.6.1/conekta.egg-info/SOURCES.txt
--rw-r--r--   0 agatto     (501) staff       (20)        1 2022-11-23 21:51:53.000000 conekta-2.6.1/conekta.egg-info/dependency_links.txt
--rw-r--r--   0 agatto     (501) staff       (20)       25 2022-11-23 21:51:53.000000 conekta-2.6.1/conekta.egg-info/requires.txt
--rw-r--r--   0 agatto     (501) staff       (20)       14 2022-11-23 21:51:53.000000 conekta-2.6.1/conekta.egg-info/top_level.txt
--rw-r--r--   0 agatto     (501) staff       (20)        1 2022-11-23 21:43:53.000000 conekta-2.6.1/conekta.egg-info/zip-safe
--rw-r--r--   0 agatto     (501) staff       (20)       38 2022-11-23 21:51:53.430366 conekta-2.6.1/setup.cfg
--rw-r--r--   0 agatto     (501) staff       (20)     1081 2022-11-23 21:48:21.000000 conekta-2.6.1/setup.py
-drwxr-xr-x   0 agatto     (501) staff       (20)        0 2022-11-23 21:51:53.428587 conekta-2.6.1/tests/
--rw-r--r--   0 agatto     (501) staff       (20)    14591 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/__init__.py
--rw-r--r--   0 agatto     (501) staff       (20)     3722 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/test_checkouts.py
--rw-r--r--   0 agatto     (501) staff       (20)     3598 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/test_customer.py
--rw-r--r--   0 agatto     (501) staff       (20)     3742 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/test_events.py
--rw-r--r--   0 agatto     (501) staff       (20)      506 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/test_logs.py
--rw-r--r--   0 agatto     (501) staff       (20)    12890 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/test_orders.py
--rw-r--r--   0 agatto     (501) staff       (20)     3125 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/test_pagination.py
--rw-r--r--   0 agatto     (501) staff       (20)      569 2022-11-23 21:42:55.000000 conekta-2.6.1/tests/test_webhooks.py
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.256983 conekta-2.6.2/
+-rw-r--r--   0 franklin   (501) staff       (20)     2716 2023-04-17 13:51:55.000000 conekta-2.6.2/CHANGELOG.md
+-rw-r--r--   0 franklin   (501) staff       (20)     1101 2023-01-06 15:45:22.000000 conekta-2.6.2/LICENSE
+-rw-r--r--   0 franklin   (501) staff       (20)       94 2023-01-06 15:45:22.000000 conekta-2.6.2/MANIFEST.in
+-rw-r--r--   0 franklin   (501) staff       (20)      754 2023-04-17 13:59:08.256794 conekta-2.6.2/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)     8812 2023-04-17 13:51:55.000000 conekta-2.6.2/README.md
+-rw-r--r--   0 franklin   (501) staff       (20)       81 2023-01-06 15:45:22.000000 conekta-2.6.2/README.txt
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.249375 conekta-2.6.2/conekta/
+-rw-r--r--   0 franklin   (501) staff       (20)    24237 2023-04-17 13:51:55.000000 conekta-2.6.2/conekta/__init__.py
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.252667 conekta-2.6.2/conekta/ssl_data/
+-rw-r--r--   0 franklin   (501) staff       (20)   261053 2023-01-06 15:45:22.000000 conekta-2.6.2/conekta/ssl_data/ca_bundle.crt
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.252333 conekta-2.6.2/conekta.egg-info/
+-rw-r--r--   0 franklin   (501) staff       (20)      754 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)      467 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/SOURCES.txt
+-rw-r--r--   0 franklin   (501) staff       (20)        1 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/dependency_links.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       25 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/requires.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       14 2023-04-17 13:59:08.000000 conekta-2.6.2/conekta.egg-info/top_level.txt
+-rw-r--r--   0 franklin   (501) staff       (20)        1 2023-01-06 17:12:23.000000 conekta-2.6.2/conekta.egg-info/zip-safe
+-rw-r--r--   0 franklin   (501) staff       (20)       38 2023-04-17 13:59:08.257079 conekta-2.6.2/setup.cfg
+-rw-r--r--   0 franklin   (501) staff       (20)     1081 2023-04-17 13:51:55.000000 conekta-2.6.2/setup.py
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-04-17 13:59:08.256315 conekta-2.6.2/tests/
+-rw-r--r--   0 franklin   (501) staff       (20)    15559 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/__init__.py
+-rw-r--r--   0 franklin   (501) staff       (20)     3510 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_checkouts.py
+-rw-r--r--   0 franklin   (501) staff       (20)     3593 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_customer.py
+-rw-r--r--   0 franklin   (501) staff       (20)     3745 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_events.py
+-rw-r--r--   0 franklin   (501) staff       (20)      508 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_logs.py
+-rw-r--r--   0 franklin   (501) staff       (20)    12832 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_orders.py
+-rw-r--r--   0 franklin   (501) staff       (20)     3113 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_pagination.py
+-rw-r--r--   0 franklin   (501) staff       (20)      575 2023-04-17 13:51:55.000000 conekta-2.6.2/tests/test_webhooks.py
```

### Comparing `conekta-2.6.1/CHANGELOG.md` & `conekta-2.6.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## [2.6.2](https://github.com/conekta/conekta-python/releases/tag/v2.6.2) - 2023-04-17
+### Change
+- Fix checkout errors
+- Fix checkout tests
+- Delete unused methods
+
 ## [2.6.1](https://github.com/conekta/conekta-python/releases/tag/v2.6.1) - 2020-12-30
 ### Change
 - Fix indentation error
 
 ## [2.6.0](https://github.com/conekta/conekta-python/releases/tag/v2.6.0) - 2020-12-30
 ### Change
 - Support creation of a payment link in the SDK.
```

### Comparing `conekta-2.6.1/LICENSE` & `conekta-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conekta-2.6.1/PKG-INFO` & `conekta-2.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conekta
-Version: 2.6.1
+Version: 2.6.2
 Summary: Easy Conekta python wrapper
 Home-page: https://github.com/conekta/conekta-python
 Download-URL: https://github.com/conekta/conekta-python/tarball/master
 Author: Conekta
 Author-email: soporte@conekta.io
 License: MIT License
 Keywords: conekta wrapper
```

### Comparing `conekta-2.6.1/README.md` & `conekta-2.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <div align="center">
 
 ![banner](readme_files/banner.png)
 
-# Conekta Python v2.6.1
+# Conekta Python v2.6.2
 
 ![python badge](readme_files/python-badge.png)
 ![conekta badge](readme_files/conekta-badge.png)
 
 </div>
 
 Wrapper for api.conekta.io
```

### Comparing `conekta-2.6.1/conekta/__init__.py` & `conekta-2.6.2/conekta/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
-#coding: utf-8
-#(c) 2013 Julian Ceballos <@jceb>
+# coding: utf-8
+# (c) 2013 Julian Ceballos <@jceb>
 
 import os
 import base64
 import inspect
 import requests
 import urllib
 import time
@@ -13,103 +13,129 @@
 try:
     import json
 except ImportError:
     import simplejson as json
 
 API_VERSION = '2.0.0'
 
-__version__ = '2.6.1'
+__version__ = '2.6.2'
 __author__ = 'Leo Fischer'
 
 API_BASE = 'https://api.conekta.io/'
 
 data = {
-    'lang' : 'python',
-    'lang_version' : platform.python_version(),
-    'publisher' : 'conekta',
-    'bindings_version' : __version__,
-    'uname' : platform.uname()
+    'lang': 'python',
+    'lang_version': platform.python_version(),
+    'publisher': 'conekta',
+    'bindings_version': __version__,
+    'uname': platform.uname()
 }
 
 HEADERS = {
     'Accept': 'application/vnd.conekta-v%s+json' % (API_VERSION),
     'Content-type': 'application/json',
-    'X-Conekta-Client-User-Agent' : json.dumps(data)
+    'X-Conekta-Client-User-Agent': json.dumps(data)
 }
 
 api_key = ''
 locale = 'en'
 
+
 class ConektaError(Exception):
-  def __init__(self, error_json):
-      super(ConektaError, self).__init__(error_json)
-      self.error_json = error_json
-      try:
-        self.details = self.error_json['details']
-        self.message = self.details[0]['message']
-        self.debug_message = self.details[0]['debug_message']
-        self.code = self.details[0]['code']
-      except Exception:
-        self.details = [
-            {
-                "message": "Hubo un error de comunicación Por favor intenta más tarde.",
-                "debug_message": "Error message was unparsable",
-                "code": "conekta.error.unparsable_error"
-            }
-        ]
-        self.message = "Hubo un error de comunicación Por favor intenta más tarde."
-        self.debug_message = "Error message was unparsable"
-        self.code = "conekta.error.unparsable_error"
-
-  def __str__(self):
-      str(self.message)
-
-class MalformedRequestError(ConektaError): pass
-class AuthenticationError(ConektaError): pass
-class ProcessingError(ConektaError): pass
-class ResourceNotFoundError(ConektaError): pass
-class ParameterValidationError(ConektaError): pass
-class ApiError(ConektaError): pass
+    def __init__(self, error_json):
+        super(ConektaError, self).__init__(error_json)
+        self.error_json = error_json
+        try:
+            self.details = self.error_json['details']
+            self.message = self.details[0]['message']
+            self.debug_message = self.details[0]['debug_message']
+            self.code = self.details[0]['code']
+        except Exception:
+            self.details = [
+                {
+                    "message": "Hubo un error de comunicación Por favor intenta más tarde.",
+                    "debug_message": "Error message was unparsable",
+                    "code": "conekta.error.unparsable_error"
+                }
+            ]
+            self.message = "Hubo un error de comunicación Por favor intenta más tarde."
+            self.debug_message = "Error message was unparsable"
+            self.code = "conekta.error.unparsable_error"
+
+    def __str__(self):
+        str(self.message)
+
+
+class MalformedRequestError(ConektaError):
+    pass
+
+
+class AuthenticationError(ConektaError):
+    pass
+
+
+class ProcessingError(ConektaError):
+    pass
+
+
+class ResourceNotFoundError(ConektaError):
+    pass
+
+
+class ParameterValidationError(ConektaError):
+    pass
+
+
+class ApiError(ConektaError):
+    pass
+
 
 class _Resource(object):
     def __init__(self, attributes):
         self.initialize_instance(attributes)
 
     def __getitem__(self, key):
         return self.__dict__[key]
 
     def __setitem__(self, key, value):
         self.__dict__[key] = value
 
     @classmethod
     def build_http_request(cls, method, path, params, _api_key=None):
         if _api_key is None:
-            HEADERS['Authorization'] = 'Basic %s' % (base64.b64encode((api_key + ':').encode('utf-8'))).decode('ascii')
+            HEADERS['Authorization'] = 'Basic %s' % (base64.b64encode(
+                (api_key + ':').encode('utf-8'))).decode('ascii')
         else:
-            HEADERS['Authorization'] = 'Basic %s' % (base64.b64encode((_api_key + ':').encode("utf-8"))).decode('ascii')
+            HEADERS['Authorization'] = 'Basic %s' % (base64.b64encode(
+                (_api_key + ':').encode("utf-8"))).decode('ascii')
 
         if not locale is None:
             HEADERS['Accept-Language'] = locale
 
         absolute_url = API_BASE + path
-        CA_PATH = os.path.join(os.path.dirname(__file__), 'ssl_data/ca_bundle.crt')
+        CA_PATH = os.path.join(os.path.dirname(
+            __file__), 'ssl_data/ca_bundle.crt')
         if method == 'GET':
             if params is None:
                 url = absolute_url
             else:
                 try:
-                    url = "%s?%s" % (absolute_url, urllib.parse.urlencode(params, True))
+                    url = "%s?%s" % (
+                        absolute_url, urllib.parse.urlencode(params, True))
                 except AttributeError:
-                    url = "%s?%s" % (absolute_url, urllib.urlencode(params, True))
-            body = requests.request(method, url, headers=HEADERS, verify=CA_PATH)
+                    url = "%s?%s" % (
+                        absolute_url, urllib.urlencode(params, True))
+            body = requests.request(
+                method, url, headers=HEADERS, verify=CA_PATH)
         else:
             if params is None:
                 params = ''
-            body = requests.request(method, absolute_url, headers=HEADERS, verify=CA_PATH, data=json.dumps(params))
-            
+            body = requests.request(
+                method, absolute_url, headers=HEADERS, verify=CA_PATH, data=json.dumps(params))
+
         headers = body.headers
         headers['status'] = str(body.status_code)
         body = body._content
         try:
             body = str(body, 'utf-8')
         except TypeError:
             body = str(body)
@@ -131,15 +157,16 @@
         elif headers['status'] == '500' or headers['status'] == '500':
             raise ApiError(json.loads(body))
         else:
             raise ConektaError(json.loads(body))
 
     @classmethod
     def load_url(cls, path, method='GET', params=None, api_key=None):
-        response = cls.build_http_request(method, path, params, _api_key = api_key)
+        response = cls.build_http_request(
+            method, path, params, _api_key=api_key)
         return response
 
     @classmethod
     def class_name(cls):
         try:
             return "%s" % urllib.parse.quote_plus(cls.__name__.lower())
         except AttributeError:
@@ -162,80 +189,85 @@
         old_keys = (set(existing_keys) - set(['parent'])) - set(new_keys)
         for key in old_keys:
             self.__dict__[key] = None
 
         for key in new_keys:
             self.__dict__[key] = attributes[key]
 
-
     def load_via_http_request(self, url=None, method='POST', params=None, api_key=None):
         if url is None:
             url = self.instance_url()
             method = 'GET'
 
-        response = self.load_url(url, method=method, params=params, api_key=api_key)
+        response = self.load_url(
+            url, method=method, params=params, api_key=api_key)
 
         self.initialize_instance(response)
 
         return self
 
+
 class _EventableResource(_Resource):
 
     def events(self, params={}, api_key=None):
         uri = self.instance_url()
         if hasattr(self, 'parent'):
             uri = "%s/%s" % (self.instance_url(), self.id)
 
-        event = Event.load_url("%s/events" % uri, 'GET', params, api_key=api_key)
+        event = Event.load_url("%s/events" % uri, 'GET',
+                               params, api_key=api_key)
         return Event(event)
 
+
 class _DeletableResource(_Resource):
 
     def delete(self, params={}, list_to_remove=None, uri=None, api_key=None):
         if uri is None:
             uri = self.instance_url()
 
             if hasattr(self, 'parent'):
                 uri = "%s/%s" % (self.instance_url(), self.id)
 
-
-
-        object_reponse = self.load_via_http_request(uri, 'DELETE', {}, api_key=api_key)
+        object_reponse = self.load_via_http_request(
+            uri, 'DELETE', {}, api_key=api_key)
 
         if list_to_remove != None:
             for remove_object in list_to_remove:
                 if remove_object.id == self.id:
                     list_to_remove.remove(remove_object)
                     break
 
         return object_reponse
 
+
 class _UpdatableResource(_Resource):
 
     def update(self, params={}, api_key=None):
         uri = self.instance_url()
 
         if hasattr(self, 'parent') and not isinstance(self, Subscription):
             uri = "%s/%s" % (self.instance_url(), self.id)
 
         return self.load_via_http_request(uri, 'PUT', params, api_key=api_key)
 
+
 class _CreatableResource(_Resource):
 
     @classmethod
     def create(cls, params, api_key=None):
         endpoint = cls.class_url()
         return cls(cls.load_url(endpoint, method='POST', params=params, api_key=api_key))
 
+
 class _FindableResource(_Resource):
 
     @classmethod
     def find(cls, _id, api_key=None):
         endpoint = cls.class_url()
-        return cls(cls.load_url("%s/%s" % (endpoint, _id), api_key=api_key ))
+        return cls(cls.load_url("%s/%s" % (endpoint, _id), api_key=api_key))
 
     @classmethod
     def where(cls, query={}, limit=10, offset=0, sort=[], api_key=None):
         endpoint = cls.class_url()
         query['limit'] = limit
 
         response = cls.load_url(endpoint, 'GET', query, api_key=api_key)
@@ -255,55 +287,57 @@
 
             elif obj["object"] == "log":
                 new_obj = Log(obj)
                 pag.class_name = Log
 
             pag.data.append(new_obj)
 
-
         return pag
 
-    #DEPRECATED aliased method, will be removed in next major release
+    # DEPRECATED aliased method, will be removed in next major release
     @classmethod
     def get(cls, _id, api_key=None):
         cls.find(_id, api_key)
 
+
 class Card(_UpdatableResource, _DeletableResource):
 
     def instance_url(self):
         return "customers/%s/cards/%s" % (self.parent.id, self.id)
 
+
 class Charge(_CreatableResource, _FindableResource):
 
     def instance_url(self):
         return "orders/%s/charges" % (self.parent.id)
 
     def refund(self, amount=None, api_key=None):
         if amount is None:
             return self.load_via_http_request("%s/refund" % self.instance_url(), api_key=api_key)
         else:
-            return self.load_via_http_request("%s/refund" % self.instance_url(), 'POST', {'amount':amount}, api_key=api_key)
+            return self.load_via_http_request("%s/refund" % self.instance_url(), 'POST', {'amount': amount}, api_key=api_key)
 
     def capture(self, api_key=None):
         return self.load_via_http_request("%s/capture" % self.instance_url(), api_key=api_key)
 
+
 class Order(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource, _EventableResource):
     def __init__(self, *args, **kwargs):
         super(Order, self).__init__(*args, **kwargs)
         attributes = args[0]
         self.currency = attributes['currency']
         self.line_items = []
         self.tax_lines = []
         self.shipping_lines = []
         self.discount_lines = []
         self.charges = []
         query = {}
         if 'line_items' in attributes.keys():
             endpoint = 'orders/{}/line_items'.format(attributes['id'])
-            response = self.load_url(endpoint,'GET',query,api_key=api_key)
+            response = self.load_url(endpoint, 'GET', query, api_key=api_key)
             for line_item in response["data"]:
                 new_line_item = LineItem(line_item)
                 new_line_item.parent = self
                 self.line_items.append(new_line_item)
 
         if 'tax_lines' in attributes.keys():
             for tax_line in attributes['tax_lines']["data"]:
@@ -323,197 +357,222 @@
                 new_discount_line.parent = self
                 self.discount_lines.append(new_discount_line)
 
         if 'customer_info' in attributes.keys():
             self.customer_info = CustomerInfo(attributes['customer_info'])
 
         if 'shipping_contact' in attributes.keys():
-            self.shipping_contact = ShippingContact(attributes['shipping_contact'])
+            self.shipping_contact = ShippingContact(
+                attributes['shipping_contact'])
 
         if 'charges' in attributes.keys():
             for charge in attributes['charges']["data"]:
                 payment_method = None
                 if charge['payment_method'] is not None:
                     payment_method = PaymentMethod(charge['payment_method'])
                 charge = Charge(charge)
                 charge.payment_method = payment_method
                 self.charges.append(charge)
 
         if 'checkout' in attributes.keys():
             self.checkout = CheckoutOrder(attributes['checkout'])
 
     def capture(self, params={}, api_key=None):
-        order = Order.load_url("%s/capture" % (self.instance_url()), 'PUT', params, api_key=api_key)
+        order = Order.load_url(
+            "%s/capture" % (self.instance_url()), 'PUT', params, api_key=api_key)
         time.sleep(2)
         new_order = Order.find(self.id)
         self.charges = new_order.charges
         self.payment_status = new_order.payment_status
         return new_order
 
     def refund(self, params={}, api_key=None):
-        order_refund = Order.load_url("%s/refund" % (self.instance_url()), 'POST', params, api_key=api_key)
+        order_refund = Order.load_url(
+            "%s/refund" % (self.instance_url()), 'POST', params, api_key=api_key)
         time.sleep(2)
         new_order = Order.find(self.id)
         self.charges = new_order.charges
         self.payment_status = new_order.payment_status
         return new_order
 
     def void(self, params={}, api_key=None):
-        order_refund = Order.load_url("%s/void" % (self.instance_url()), 'POST', params, api_key=api_key)
+        order_refund = Order.load_url(
+            "%s/void" % (self.instance_url()), 'POST', params, api_key=api_key)
         time.sleep(2)
         new_order = Order.find(self.id)
         self.charges = new_order.charges
         self.payment_status = new_order.payment_status
         return new_order
 
     def charge(self, params, api_key=None):
-        charge = Charge(Charge.load_url("%s/charges" % self.instance_url(), 'POST', params, api_key=api_key))
+        charge = Charge(Charge.load_url("%s/charges" %
+                        self.instance_url(), 'POST', params, api_key=api_key))
         self.charges.append(charge)
         return charge
 
     def createShippingContact(self, params, api_key=None):
-        orders = self.update(params)
+        orders = self.update(params, api_key=api_key)
         self.shipping_contact = ShippingContact(orders['shipping_contact'])
         return self.shipping_contact
 
     def createLineItem(self, params, api_key=None):
-        line_item = LineItem(LineItem.load_url("%s/line_items" % self.instance_url(), 'POST', params, api_key=api_key))
+        line_item = LineItem(LineItem.load_url(
+            "%s/line_items" % self.instance_url(), 'POST', params, api_key=api_key))
         self.line_items.append(line_item)
         return line_item
 
     def createTaxLine(self, params, api_key=None):
-        tax_line = TaxLine(TaxLine.load_url("%s/tax_lines" % self.instance_url(), 'POST', params, api_key=api_key))
+        tax_line = TaxLine(TaxLine.load_url("%s/tax_lines" %
+                           self.instance_url(), 'POST', params, api_key=api_key))
         self.tax_lines.append(tax_line)
         return tax_line
 
     def createShippingLine(self, params, api_key=None):
-        shipping_line = ShippingLine(ShippingLine.load_url("%s/shipping_lines" % self.instance_url(), 'POST', params, api_key=api_key))
+        shipping_line = ShippingLine(ShippingLine.load_url(
+            "%s/shipping_lines" % self.instance_url(), 'POST', params, api_key=api_key))
         self.shipping_lines.append(shipping_line)
         return shipping_line
 
     def createDiscountLine(self, params, api_key=None):
-        discount_line = DiscountLine(DiscountLine.load_url("%s/discount_lines" % self.instance_url(), 'POST', params, api_key=api_key))
+        discount_line = DiscountLine(DiscountLine.load_url(
+            "%s/discount_lines" % self.instance_url(), 'POST', params, api_key=api_key))
         self.discount_lines.append(discount_line)
         return discount_line
 
-    def createCheckout(self, params, api_key=None):
-        checkout = CheckoutOrder(DiscountLine.load_url("%s/orders" % self.instance_url(), 'POST', params, api_key=api_key))
-        self.checkout.append(checkout)
-        return checkout
 
-class CustomerInfo(_UpdatableResource): pass
+class CustomerInfo(_UpdatableResource):
+    pass
+
+
+class OrderReturns(_UpdatableResource):
+    pass
+
+
+class PaymentMethod(_UpdatableResource):
+    pass
 
-class OrderReturns(_UpdatableResource): pass
 
-class PaymentMethod(_UpdatableResource): pass
+class Address(_FindableResource):
+    pass
 
-class Address(_FindableResource): pass
 
 class Customer(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource, _EventableResource):
 
     def __init__(self, *args, **kwargs):
         super(Customer, self).__init__(*args, **kwargs)
 
         attributes = args[0]
-        self.payment_sources   = []
+        self.payment_sources = []
         self.shipping_contacts = []
         if 'payment_sources' in attributes.keys():
             for payment_source in attributes['payment_sources']['data']:
                 new_payment_source = PaymentSource(payment_source)
                 new_payment_source.parent = self
                 self.payment_sources.append(new_payment_source)
 
         if 'shipping_contacts' in attributes.keys():
             for shipping_contact in attributes['shipping_contacts']['data']:
                 new_shipping_contact = ShippingContact(shipping_contact)
-                new_shipping_contact.address = Address(shipping_contact["address"])
+                new_shipping_contact.address = Address(
+                    shipping_contact["address"])
                 new_shipping_contact.parent = self
                 self.shipping_contacts.append(new_shipping_contact)
 
         if 'subscription' in attributes.keys() and isinstance(attributes['subscription'], dict):
             attributes['subscription']['parent'] = self
             self.subscription = Subscription(attributes['subscription'])
         else:
             self.subscription = None
 
     def createPaymentSource(self, params, api_key=None):
-        pay_src = PaymentSource.load_url("%s/payment_sources" % self.instance_url(), 'POST', params, api_key=api_key)
+        pay_src = PaymentSource.load_url(
+            "%s/payment_sources" % self.instance_url(), 'POST', params, api_key=api_key)
         payment_source = PaymentSource(pay_src)
         payment_source.parent = self
         self.payment_sources.append(payment_source)
         return payment_source
 
     def createShippingContact(self, params, api_key=None):
-        shipping = PaymentSource.load_url("%s/shipping_contacts" % self.instance_url(), 'POST', params, api_key=api_key)
+        shipping = PaymentSource.load_url(
+            "%s/shipping_contacts" % self.instance_url(), 'POST', params, api_key=api_key)
         shipping_contact = ShippingContact(shipping)
         shipping_contact.parent = self
         self.shipping_contacts.append(shipping_contact)
         return shipping_contact
 
     def createSubscription(self, params, api_key=None):
-        subscription = Subscription(Subscription.load_url("%s/subscription" % self.instance_url(), 'POST', params, api_key=api_key))
+        subscription = Subscription(Subscription.load_url(
+            "%s/subscription" % self.instance_url(), 'POST', params, api_key=api_key))
         subscription.parent = self
         self.subscription = subscription
         return subscription
 
     @property
     def default_card(self):
         if self.default_card_id:
             return [card for card in self.cards if card.id == self.default_card_id][0]
         else:
             return None
 
+
 class Checkout(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource):
 
     def __init__(self, *args, **kwargs):
-        super(Checkouts, self).__init__(*args, **kwargs)
-        
-    def create(self, params, api_key=None):
-        return self.load_via_http_request("%s/checkouts" % self.instance_url(), 'POST', params, api_key=api_key)
+        super(Checkout, self).__init__(*args, **kwargs)
 
     def cancel(self, params, api_key=None):
-        return self.load_via_http_request("%s/checkouts/cancel/%s" % (self.instance_url(), self.id), 'PUT', None, api_key=api_key)
+        return self.load_via_http_request("%s/cancel" % (self.instance_url()), 'PUT', None, api_key=api_key)
 
     def sendEmail(self, params, api_key=None):
-        return self.load_via_http_request("%s/checkouts/email" % self.instance_url(), 'POST', params, api_key=api_key)
+        return self.load_via_http_request("%s/email" % self.instance_url(), 'POST', params, api_key=api_key)
 
     def sendSms(self, params, api_key=None):
-        return self.load_via_http_request("%s/checkouts/sms" % self.instance_url(), 'POST', params, api_key=api_key)
+        return self.load_via_http_request("%s/sms" % self.instance_url(), 'POST', params, api_key=api_key)
+
+
+class Event(_FindableResource):
+    pass
 
-class Event(_FindableResource): pass
 
-class Log(_FindableResource): pass
+class Log(_FindableResource):
+    pass
+
 
 class Payee(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource):
 
     def __init__(self, *args, **kwargs):
         super(Payee, self).__init__(*args, **kwargs)
 
         attributes = args[0]
         self.payout_methods = []
         if 'payout_methods' in attributes.keys():
             for payout_method in attributes['payout_methods']:
                 payout_method['parent'] = self
                 self.payout_methods.append(PayoutMethod(payout_method))
 
     def createPayoutMethod(self, params, api_key=None):
-        payout_method = PayoutMethod(PayoutMethod.load_url("%s/payout_methods" % self.instance_url(), 'POST', params, api_key=api_key))
+        payout_method = PayoutMethod(PayoutMethod.load_url(
+            "%s/payout_methods" % self.instance_url(), 'POST', params, api_key=api_key))
         payout_method.parent = self
         self.payout_methods.append(payout_method)
         return payout_method
 
     @property
     def default_payout_method(self):
         if self.default_payout_method_id:
             return [payout_method for payout_method in self.payout_methods if payout_method.id == self.default_payout_method_id][0]
         else:
             return None
 
-class Payout(_CreatableResource, _FindableResource): pass
-class Pagination(_CreatableResource):
+
+class Payout(_CreatableResource, _FindableResource):
+    pass
+
+
+class Pagination(_CreatableResource, _FindableResource):
     def next(self):
         if not hasattr(self, 'next_page_url'):
             return None
 
         raw_params = self.next_page_url.split("?")[1]
         query = {}
         for elemet_params in raw_params.split("&"):
@@ -527,20 +586,24 @@
         raw_params = self.previous_page_url.split("?")[1]
         query = {}
         for elemet_params in raw_params.split("&"):
             key_and_param = elemet_params.split("=")
             query[key_and_param[0]] = key_and_param[1]
         return self.class_name.where(query)
 
+
 class PayoutMethod(_UpdatableResource, _DeletableResource):
 
     def instance_url(self):
         return "payees/%s/payout_methods/%s" % (self.parent.id, self.id)
 
-class Plan(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource): pass
+
+class Plan(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource):
+    pass
+
 
 class Subscription(_UpdatableResource):
 
     def instance_url(self):
         return "customers/%s/subscription" % (self.parent.id)
 
     def pause(self, finish_billing_cycle=False, until=None, api_key=None):
@@ -556,74 +619,85 @@
     def card(self):
         return [card for card in self.parent.cards if card.id == self.card_id][0]
 
     @property
     def plan(self):
         return Plan.retrieve(self.plan_id)
 
-class Webhook(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource): pass
+
+class Webhook(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource):
+    pass
+
 
 class LineItem(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource, _EventableResource):
 
     def instance_url(self):
         return "orders/%s/line_items" % (self.parent.id)
 
     def delete(self, params={}, api_key=None):
         return super(LineItem, self).delete(params, self.parent.line_items)
 
+
 class TaxLine(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource, _EventableResource):
 
     def instance_url(self):
         return "orders/%s/tax_lines" % (self.parent.id)
 
     def delete(self, params={}, api_key=None):
         return super(TaxLine, self).delete(params, self.parent.tax_lines)
 
+
 class ShippingLine(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource, _EventableResource):
 
     def instance_url(self):
         return "orders/%s/shipping_lines" % (self.parent.id)
 
     def delete(self, params={}, api_key=None):
         return super(ShippingLine, self).delete(params, self.parent.shipping_lines)
 
+
 class DiscountLine(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource, _EventableResource):
 
     def instance_url(self):
         return "orders/%s/discount_lines" % (self.parent.id)
 
     def delete(self, params={}, api_key=None):
         return super(DiscountLine, self).delete(params, self.parent.discount_lines)
 
+
 class PaymentSource(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource):
     def instance_url(self):
         return "customers/%s/payment_sources" % (self.parent.id)
 
     def delete(self, params={}, api_key=None):
         return super(PaymentSource, self).delete(params, self.parent.payment_sources)
 
     def events(self, params={}, api_key=None):
-        uri = "%s/payment_sources/%s/events" % (self.parent.instance_url(), self.id)
+        uri = "%s/payment_sources/%s/events" % (
+            self.parent.instance_url(), self.id)
         event = Event.load_url(uri, 'GET', params, api_key=api_key)
         return Event(event)
 
+
 class ShippingContact(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource):
 
     def instance_url(self):
         return "customers/%s/shipping_contacts" % (self.parent.id)
 
     def update(self, params={}, api_key=None):
         uri = "%s/shipping_contacts/%s" % (self.parent.instance_url(), self.id)
         return self.load_via_http_request(uri, 'PUT', params, api_key=api_key)
 
     def delete(self, params={}, api_key=None):
         uri = "%s/shipping_contacts/%s" % (self.parent.instance_url(), self.id)
         return super(ShippingContact, self).delete(params, self.parent.shipping_contacts, uri)
 
     def events(self, params={}, api_key=None):
-        uri = "%s/shipping_contacts/%s/events" % (self.parent.instance_url(), self.id)
+        uri = "%s/shipping_contacts/%s/events" % (
+            self.parent.instance_url(), self.id)
         return Event(Event.load_url(uri, 'GET', params, api_key=api_key))
 
+
 class CheckoutOrder(_CreatableResource, _UpdatableResource, _DeletableResource, _FindableResource):
 
     def instance_url(self):
-        return "orders" 
+        return "orders"
```

### Comparing `conekta-2.6.1/conekta/ssl_data/ca_bundle.crt` & `conekta-2.6.2/conekta/ssl_data/ca_bundle.crt`

 * *Files identical despite different names*

### Comparing `conekta-2.6.1/conekta.egg-info/PKG-INFO` & `conekta-2.6.2/conekta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conekta
-Version: 2.6.1
+Version: 2.6.2
 Summary: Easy Conekta python wrapper
 Home-page: https://github.com/conekta/conekta-python
 Download-URL: https://github.com/conekta/conekta-python/tarball/master
 Author: Conekta
 Author-email: soporte@conekta.io
 License: MIT License
 Keywords: conekta wrapper
```

### Comparing `conekta-2.6.1/setup.py` & `conekta-2.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 #coding: utf-8
 #(c) 2013 Julian Ceballos <@jceb>
 
 from setuptools import setup, find_packages
 
-version = "2.6.1"
+version = "2.6.2"
 author = "Conekta"
 
 setup(
     name='conekta',
     version=version,
     author=author,
     author_email='soporte@conekta.io',
```

### Comparing `conekta-2.6.1/tests/__init__.py` & `conekta-2.6.2/tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python
 # coding: utf-8
-#(c) 2013 Julian Ceballos <@jceb>
+# (c) 2013 Julian Ceballos <@jceb>
 
 import unittest
 import random
 import conekta
+from datetime import datetime, timedelta
 
 
 class BaseEndpointTestCase(unittest.TestCase):
     random.seed()
 
     client = conekta
 
@@ -19,21 +20,21 @@
         "reference_id": "9893-cohib_s1_wolf_pack",
         "card": "tok_test_visa_4242",
         "details": {
             "name": "Wolverine",
             "email": "logan.thomas@xmen.org",
             "phone": "403-342-0642",
             "line_items": [{
-              "name": "Shades",
-              "description": "Imported From Mex.",
-              "unit_price": 20000,
-              "quantity": 1,
-              "sku": "cohb_s1",
-              "category": "eyewear"
-           }]
+                "name": "Shades",
+                "description": "Imported From Mex.",
+                "unit_price": 20000,
+                "quantity": 1,
+                "sku": "cohb_s1",
+                "category": "eyewear"
+            }]
         }
     }
 
     cash_charge_object = {
         "currency": "MXN",
         "amount": 20000,
         "description": "Grad Stogies: Second Class",
@@ -42,21 +43,21 @@
             "type": "oxxo"
         },
         "details": {
             "name": "Wolverine",
             "email": "logan.thomas@xmen.org",
             "phone": "403-342-0642",
             "line_items": [{
-              "name": "Shades",
-              "description": "Imported From Mex.",
-              "unit_price": 20000,
-              "quantity": 1,
-              "sku": "cohb_s1",
-              "category": "eyewear"
-           }]
+                "name": "Shades",
+                "description": "Imported From Mex.",
+                "unit_price": 20000,
+                "quantity": 1,
+                "sku": "cohb_s1",
+                "category": "eyewear"
+            }]
         }
     }
 
     bank_charge_object = {
         "currency": "MXN",
         "amount": 20000,
         "description": "Grad Stogies: Second Class",
@@ -65,21 +66,21 @@
             "type": "banorte"
         },
         "details": {
             "name": "Wolverine",
             "email": "logan.thomas@xmen.org",
             "phone": "403-342-0642",
             "line_items": [{
-              "name": "Shades",
-              "description": "Imported From Mex.",
-              "unit_price": 20000,
-              "quantity": 1,
-              "sku": "cohb_s1",
-              "category": "eyewear"
-           }]
+                "name": "Shades",
+                "description": "Imported From Mex.",
+                "unit_price": 20000,
+                "quantity": 1,
+                "sku": "cohb_s1",
+                "category": "eyewear"
+            }]
         }
     }
 
     spei_charge_object = {
         "currency": "MXN",
         "amount": 20000,
         "description": "Grad Stogies: Second Class",
@@ -88,56 +89,56 @@
             "type": "spei"
         },
         "details": {
             "name": "Wolverine",
             "email": "logan.thomas@xmen.org",
             "phone": "403-342-0642",
             "line_items": [{
-              "name": "Shades",
-              "description": "Imported From Mex.",
-              "unit_price": 20000,
-              "quantity": 1,
-              "sku": "cohb_s1",
-              "category": "eyewear"
-           }]
+                "name": "Shades",
+                "description": "Imported From Mex.",
+                "unit_price": 20000,
+                "quantity": 1,
+                "sku": "cohb_s1",
+                "category": "eyewear"
+            }]
         }
     }
 
     plan_object = {
-        'id':'py_test_plan_' + str(random.randint(1, 1000000)),
+        'id': 'py_test_plan_' + str(random.randint(1, 1000000)),
         'name': 'Python Test Subscription',
         'amount': 10000,
         'currency': 'MXN',
         'interval': 'week',
         'frequency': 3
     }
 
     customer_object = {
-        'name':'James Howlett',
-        'email':'logan@x-men.org',
-        'phone':'+525511223344',
-        'payment_sources':[
-          { 'token_id': 'tok_test_visa_4242',
-            'type': 'card'},
-          { 'token_id': 'tok_test_mastercard_5100',
-            'type': 'card'}
+        'name': 'James Howlett',
+        'email': 'logan@x-men.org',
+        'phone': '+525511223344',
+        'payment_sources': [
+            {'token_id': 'tok_test_visa_4242',
+             'type': 'card'},
+            {'token_id': 'tok_test_mastercard_5100',
+             'type': 'card'}
         ],
-    "shipping_contacts": [{
-        "phone": "+525511223344",
-        "receiver": "Marvin Fuller",
-        "between_streets": "Ackerman Crescent",
-        "address": {
-            "street1": "250 Alexis St",
-            "city": "Red Deer",
-            "state": "Alberta",
-            "country": "CA",
-            "postal_code": "T4N 0B8"
-        }
+        "shipping_contacts": [{
+            "phone": "+525511223344",
+            "receiver": "Marvin Fuller",
+            "between_streets": "Ackerman Crescent",
+            "address": {
+                "street1": "250 Alexis St",
+                "city": "Red Deer",
+                "state": "Alberta",
+                "country": "CA",
+                "postal_code": "T4N 0B8"
+            }
 
-    }]
+        }]
     }
 
     payee_object = {
         'name': 'Graydon Creed',
         'email': 'graydon@friendsofhumanity.com',
         'phone': '5555555555',
         'bank': {
@@ -149,143 +150,143 @@
     payout_method_object = {
         'type': 'bank_transfer_payout_method',
         'account_number': '123456789012345673',
         'account_holder': 'Friends of Humanity'
     }
 
     order_object = {
-      "line_items": [
-          {
-              "name": "Box of Cohiba S1s",
-              "description": "Imported From Mex.",
-              "unit_price": 20000,
-              "quantity": 1,
-              "sku": "cohb_s1",
-              "category": "food",
-              "type" : "physical",
-              "tags" : ["food", "mexican food"]
-          }
-      ],
-      "tax_lines":[
-        {
-          "description": "IVA",
-          "amount": 600,
-          "metadata": {
-            "random_key": "random_value"
-          }
-        }],
-      "shipping_lines":[
-        {
-          "amount": 0,
-          "tracking_number": "TRACK123",
-          "carrier": "USPS",
-          "method": "Train",
-          "metadata": {
-             "random_key": "random_value"
-          }
-        }],
-      "discount_lines":[
-        {
-          "code": "descuento",
-          "type": "loyalty",
-          "amount": 600
+        "line_items": [
+            {
+                "name": "Box of Cohiba S1s",
+                "description": "Imported From Mex.",
+                "unit_price": 20000,
+                "quantity": 1,
+                "sku": "cohb_s1",
+                "category": "food",
+                "type": "physical",
+                "tags": ["food", "mexican food"]
+            }
+        ],
+        "tax_lines": [
+            {
+                "description": "IVA",
+                "amount": 600,
+                "metadata": {
+                    "random_key": "random_value"
+                }
+            }],
+        "shipping_lines": [
+            {
+                "amount": 0,
+                "tracking_number": "TRACK123",
+                "carrier": "USPS",
+                "method": "Train",
+                "metadata": {
+                    "random_key": "random_value"
+                }
+            }],
+        "discount_lines": [
+            {
+                "code": "descuento",
+                "type": "loyalty",
+                "amount": 600
+            }],
+        "customer_info": {
+            "name": "John Constantine",
+            "phone": "+525533445566",
+            "email": "john@meh.com",
+            "corporate": False,
+            "vertical_info": {}
+        },
+        "shipping_contact": {
+            "phone": "5544332211",
+            "receiver": "Marvin Fuller",
+            "between_streets": "Ackerman Crescent",
+            "address": {
+                "street1": "250 Alexis St",
+                "state": "Alberta",
+                "country": "MX",
+                "postal_code": "23455",
+                "metadata": {"soft_validations": True}
+            }
+        },
+        "charges": [{
+            "payment_method": {
+                "type": "oxxo_cash"
+            },
+            "amount": 20000
         }],
-      "customer_info":{
-          "name": "John Constantine",
-          "phone": "+525533445566",
-          "email": "john@meh.com",
-          "corporate": False,
-          "vertical_info": {}
-        },
-      "shipping_contact":{
-          "phone" : "5544332211",
-          "receiver": "Marvin Fuller",
-          "between_streets": "Ackerman Crescent",
-          "address": {
-              "street1": "250 Alexis St",
-              "state": "Alberta",
-              "country": "MX",
-              "postal_code": "23455",
-              "metadata":{ "soft_validations": True}
-          }
-      },
-      "charges": [{
-        "payment_method":{
-          "type":"oxxo_cash"
-        },
-        "amount": 20000
-      }],
-      "currency" : "mxn",
-      "metadata" : {"test" : "extra info"}
+        "currency": "mxn",
+        "metadata": {"test": "extra info"}
     }
     line_item_object = {
         "name": "test line item",
         "description": "Imported From Mex.",
         "unit_price": 10000,
         "quantity": 2,
         "sku": "noSKU",
         "category": "food",
-        "type" : "physical",
-        "tags" : ["food", "mexican food"]
+        "type": "physical",
+        "tags": ["food", "mexican food"]
     }
     tax_line_object = {
         "description": "IVA2",
         "amount": 600,
         "metadata": {
-        "random_key": "random_value"
+            "random_key": "random_value"
         }
     }
 
     shipping_lines_object = {
         "amount": 0,
         "tracking_number": "TRACK123",
         "carrier": "USPS",
         "method": "Train",
         "metadata": {
-           "random_key": "random_value"
+            "random_key": "random_value"
         }
     }
 
     discount_line_object = {
         "code": "descuento",
         "type": "loyalty",
         "amount": 100
     }
 
     order_shipping_contact_object = {
-      "shipping_contact": {
-        "phone" : "+525511223399",
-        "receiver": "Marvin Fuller",
-        "between_streets": "Ackerman Crescent",
-        "address": {
-            "street1": "250 Alexis St",
-            "state": "Alberta",
-            "country": "MX",
-            "postal_code": "23455",
-            "metadata":{ "soft_validations": True}
-          }
-      }
+        "shipping_contact": {
+            "phone": "+525511223399",
+            "receiver": "Marvin Fuller",
+            "between_streets": "Ackerman Crescent",
+            "address": {
+                "street1": "250 Alexis St",
+                "state": "Alberta",
+                "country": "MX",
+                "postal_code": "23455",
+                "metadata": {"soft_validations": True}
+            }
+        }
     }
 
     charge_object = {
-      "payment_method":{
-        "type":"oxxo_cash"
-      },
-      "amount": 20000
+        "payment_method": {
+            "type": "oxxo_cash"
+        },
+        "amount": 20000
     }
 
     payment_source_object = {
-      'token_id': 'tok_test_visa_4242',
-      'type': 'card'
+        'token_id': 'tok_test_visa_4242',
+        'type': 'card'
     }
 
     update_payment_source_object = {
         "name": "Emiliano Cabrera",
         "exp_month": "12",
-        "exp_year": "20",
+        "exp_year": "29",
         "address": {
             "street1": "Nuevo leon",
             "city": "Monterrey",
             "state": "Nuevo Leon",
             "country": "MX",
             "postal_code": "64700"
         }
@@ -304,80 +305,82 @@
         }
     }
 
     checkout_object = {
         "name": "Payment Link Name",
         "type": "PaymentLink",
         "recurrent": False,
-        "expired_at": 1590882634,
+        "expired_at": int((datetime.today() + timedelta(days=1)).timestamp()),
         "allowed_payment_methods": ["cash", "card", "bank_transfer"],
         "needs_shipping_contact": True,
         "monthly_installments_enabled": False,
         "monthly_installments_options": [3, 6, 9, 12],
         "order_template": {
             "line_items": [{
                 "name": "Red Wine",
                 "unit_price": 1000,
                 "quantity": 10
             }],
-        "currency": "MXN",
-        "customer_info": {
-              "name": "Juan Perez",
-              "email": "test@conekta.com",
-              "phone": "5566982090"
+            "currency": "MXN",
+            "customer_info": {
+                "name": "Juan Perez",
+                "email": "test@conekta.com",
+                "phone": "5566982090"
+            }
         }
-      }
     }
 
     checkout_object_multiple = {
+        "payments_limit_count": 2,
         "name": "Payment Link Name",
         "type": "PaymentLink",
         "recurrent": True,
-        "expired_at": 1590882634,
+        "expired_at": int((datetime.today() + timedelta(days=1)).timestamp()),
         "allowed_payment_methods": ["cash", "card", "bank_transfer"],
         "needs_shipping_contact": True,
         "monthly_installments_enabled": False,
         "monthly_installments_options": [3, 6, 9, 12],
         "order_template": {
             "line_items": [{
                 "name": "Red Wine",
                 "unit_price": 1000,
                 "quantity": 10
             }],
-        "currency": "MXN",
-        "customer_info": {
-              "name": "Juan Perez",
-              "email": "test@conekta.com",
-              "phone": "5566982090"
+            "currency": "MXN",
+            "customer_info": {
+                "name": "Juan Perez",
+                "email": "test@conekta.com",
+                "phone": "5566982090"
+            }
         }
-      }
     }
 
     checkout_object_msi = {
+        "payments_limit_count" : 2,
         "name": "Payment Link Name",
         "type": "PaymentLink",
         "recurrent": True,
-        "expired_at": 1590882634,
+        "expired_at": int((datetime.today() + timedelta(days=1)).timestamp()),
         "allowed_payment_methods": ["cash", "card", "bank_transfer"],
         "needs_shipping_contact": True,
         "monthly_installments_enabled": True,
         "monthly_installments_options": [3, 6, 9, 12],
         "order_template": {
             "line_items": [{
                 "name": "Red Wine",
                 "unit_price": 1000,
                 "quantity": 10
             }],
-        "currency": "MXN",
-        "customer_info": {
-              "name": "Juan Perez",
-              "email": "test@conekta.com",
-              "phone": "5566982090"
+            "currency": "MXN",
+            "customer_info": {
+                "name": "Juan Perez",
+                "email": "test@conekta.com",
+                "phone": "5566982090"
+            }
         }
-      }
     }
 
     checkout_object_type_checkout = {
         "name": "Payment Link Name",
         "type": "checkout",
         "recurrent": True,
         "expired_at": 1590882634,
@@ -387,136 +390,136 @@
         "monthly_installments_options": [3, 6, 9, 12],
         "order_template": {
             "line_items": [{
                 "name": "Red Wine",
                 "unit_price": 1000,
                 "quantity": 10
             }],
-        "currency": "MXN",
-        "customer_info": {
-              "name": "Juan Perez",
-              "email": "test@conekta.com",
-              "phone": "5566982090"
+            "currency": "MXN",
+            "customer_info": {
+                "name": "Juan Perez",
+                "email": "test@conekta.com",
+                "phone": "5566982090"
+            }
         }
-      }
     }
 
-        checkout_object_send = {
-        "id": "05b25724-df59-4925-8762-105d627875fd"
+    checkout_object_send = {
+        "id": "05b25724-df59-4925-8762-105d627875fd",
         "name": "Payment Link Name",
         "type": "checkout",
         "recurrent": True,
         "expired_at": 1590882634,
         "allowed_payment_methods": ["cash", "card", "bank_transfer"],
         "needs_shipping_contact": True,
         "monthly_installments_enabled": True,
         "monthly_installments_options": [3, 6, 9, 12],
         "order_template": {
             "line_items": [{
                 "name": "Red Wine",
                 "unit_price": 1000,
                 "quantity": 10
             }],
-        "currency": "MXN",
-        "customer_info": {
-              "name": "Juan Perez",
-              "email": "test@conekta.com",
-              "phone": "5566982090"
+            "currency": "MXN",
+            "customer_info": {
+                "name": "Juan Perez",
+                "email": "test@conekta.com",
+                "phone": "5566982090"
+            }
         }
-      }
     }
 
-
-    checkout_order_object = 
+    checkout_order_object = {
         "currency": "MXN",
         "customer_info": {
-           "customer_id": "cus_2o3FvMEBiKitVK1vQ"
+            "customer_id": "cus_2tgwCPgJZR56HvkKK"
         },
-       "line_items": [{
-           "name": "Box of Cohiba S1s",
-           "unit_price": 300000,
-           "quantity": 1
-       }],
-       "shipping_lines": [{
-           "amount": 0
-       }],
-       "checkout": {
-           "allowed_payment_methods": ["cash", "card", "bank_transfer"],
-           "multifactor_authentication": False,
-           "monthly_installments_enabled": False,
-           "monthly_installments_options": [3,6,9,12,18],
-           "expires_at": 1609891200
-        },
-       "shipping_contact": {
-          "phone": "+5215555555555",
-          "receiver": "Marvin Fuller",
-          "address": {
-            "street1": "Nuevo Leon 4",
-            "country": "MX",
-            "postal_code": "06100"
-          }
-       }
+        "line_items": [{
+            "name": "Box of Cohiba S1s",
+            "unit_price": 300000,
+            "quantity": 1
+        }],
+        "shipping_lines": [{
+            "amount": 0
+        }],
+        "checkout": {
+            "allowed_payment_methods": ["cash", "card", "bank_transfer"],
+            "multifactor_authentication": False,
+            "monthly_installments_enabled": False,
+            "monthly_installments_options": [3, 6, 9, 12, 18],
+            "expired_at": int((datetime.today() + timedelta(days=1)).timestamp())
+        },
+        "shipping_contact": {
+            "phone": "+5215555555555",
+            "receiver": "Marvin Fuller",
+            "address": {
+                "street1": "Nuevo Leon 4",
+                "country": "MX",
+                "postal_code": "06100"
+            }
+        }}
 
-    checkout_msi_order__object = 
+    checkout_msi_order__object = {
         "currency": "MXN",
         "customer_info": {
-           "customer_id": "cus_2o3FvMEBiKitVK1vQ"
+            "customer_id": "cus_2tgwCPgJZR56HvkKK"
         },
-       "line_items": [{
-           "name": "Box of Cohiba S1s",
-           "unit_price": 300000,
-           "quantity": 1
-       }],
-       "shipping_lines": [{
-           "amount": 0
-       }],
-       "checkout": {
-           "type":"Integration",
-           "allowed_payment_methods": ["cash", "card", "bank_transfer"],
-           "multifactor_authentication": False,
-           "monthly_installments_enabled": True,
-           "monthly_installments_options": [3,6,9,12,18],
-           "expires_at": 1609891200
-        },
-       "shipping_contact": {
-          "phone": "+5215555555555",
-          "receiver": "Marvin Fuller",
-          "address": {
-            "street1": "Nuevo Leon 4",
-            "country": "MX",
-            "postal_code": "06100"
-          }
-       }
-
+        "line_items": [{
+            "name": "Box of Cohiba S1s",
+            "unit_price": 300000,
+            "quantity": 1
+        }],
+        "shipping_lines": [{
+            "amount": 0
+        }],
+        "checkout": {
+            "type": "Integration",
+            "allowed_payment_methods": ["cash", "card", "bank_transfer"],
+            "multifactor_authentication": False,
+            "monthly_installments_enabled": True,
+            "monthly_installments_options": [3, 6, 9, 12, 18],
+            "expires_at": 1609891200
+        },
+        "shipping_contact": {
+            "phone": "+5215555555555",
+            "receiver": "Marvin Fuller",
+            "address": {
+                "street1": "Nuevo Leon 4",
+                "country": "MX",
+                "postal_code": "06100"
+            }
+        }
+    }
 
-          checkout_order__redirect_object = 
+    checkout_order__redirect_object = {
         "currency": "MXN",
         "customer_info": {
-           "customer_id": "cus_2o3FvMEBiKitVK1vQ"
+            "customer_id": "cus_2tgwCPgJZR56HvkKK"
         },
-       "line_items": [{
-           "name": "Box of Cohiba S1s",
-           "unit_price": 300000,
-           "quantity": 1
-       }],
-       "shipping_lines": [{
-           "amount": 0
-       }],
-       "checkout": {
-           "type":"HostedPayment",
-           "success_url": "testredirect.com",
-           "failure_url": "testredirect.com",
-           "allowed_payment_methods": ["cash", "card", "bank_transfer"],
-           "multifactor_authentication": False,
-           "monthly_installments_enabled": False,
-           "monthly_installments_options": [3,6,9,12,18],
-           "expires_at": 1609891200
-        },
-       "shipping_contact": {
-          "phone": "+5215555555555",
-          "receiver": "Marvin Fuller",
-          "address": {
-            "street1": "Nuevo Leon 4",
-            "country": "MX",
-            "postal_code": "06100"
-          }
-       }
+        "line_items": [{
+            "name": "Box of Cohiba S1s",
+            "unit_price": 300000,
+            "quantity": 1
+        }],
+        "shipping_lines": [{
+            "amount": 0
+        }],
+        "checkout": {
+            "type": "HostedPayment",
+            "success_url": "https://testredirect.com",
+            "failure_url": "https://testredirect.com",
+            "allowed_payment_methods": ["cash", "card", "bank_transfer"],
+            "multifactor_authentication": False,
+            "monthly_installments_enabled": False,
+            "monthly_installments_options": [3, 6, 9, 12, 18],
+            "expired_at": int((datetime.today() + timedelta(days=1)).timestamp())
+        },
+        "shipping_contact": {
+            "phone": "+5215555555555",
+            "receiver": "Marvin Fuller",
+            "address": {
+                "street1": "Nuevo Leon 4",
+                "country": "MX",
+                "postal_code": "06100"
+            }
+        }
+    }
```

### Comparing `conekta-2.6.1/tests/test_checkouts.py` & `conekta-2.6.2/tests/test_checkouts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,88 @@
 #!/usr/bin/python
-#coding: utf-8
-#(c) 2020 Erick Colin <@erickcolin>
+# coding: utf-8
+# (c) 2020 Erick Colin <@erickcolin>
 
 from . import BaseEndpointTestCase
 
+
 class CheckoutsEndpointTestCase(BaseEndpointTestCase):
 
     def test_01_create_checkout(self):
-        
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         checkout = self.client.Checkout.create(self.checkout_object.copy())
 
         assert checkout.type == "PaymentLink"
         assert checkout.object == "checkout"
-        assert checkout.status != "Issued"
-        assert checkout.url.startswith("https:\\pay.conekta")
-        assert checkout.id.len() == 36
-    
-    def test_02_create_checkout_recurrent(self):
+        assert checkout.status == "Issued"
+        assert checkout.url.startswith("https://pay.conekta")
+        assert len(checkout.id) == 36
 
+    def test_02_create_checkout_recurrent(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         checkout = self.client.Checkout.create(self.checkout_object_multiple.copy())
 
         assert checkout.recurrent == True
         assert checkout.type == "PaymentLink"
         assert checkout.object == "checkout"
-        assert checkout.url.startswith("https:\\pay.conekta")
-        assert checkout.id.len() == 36
+        assert checkout.url.startswith("https://pay.conekta")
+        assert len(checkout.id) == 36
 
-    
     def test_03_create_checkout_msi(self):
-
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         checkout = self.client.Checkout.create(self.checkout_object_msi.copy())
 
         assert checkout.monthly_installments_enabled == True
         assert checkout.type == "PaymentLink"
         assert checkout.object == "checkout"
-        assert checkout.url.startswith("https:\\pay.conekta")
-        assert checkout.id.len() == 36
+        assert checkout.url.startswith("https://pay.conekta")
+        assert len(checkout.id) == 36
 
     def test_04_checkout_sendmail(self):
-
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
-        checkout = self.client.Checkout.sendEmail(self.checkout_object_send.copy())
+        checkout = self.client.Checkout.create(self.checkout_object.copy())
+        response = checkout.sendEmail(self.checkout_object_send.copy())
 
-        assert isinstance(checkout,self.checkout_object_send.copy())
+        assert response.emails_sent == 1
 
     def test_05_checkout_sendsms(self):
-
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
-        checkout = self.client.Checkout.sendSms(self.checkout_object_send.copy())
-
-        assert isinstance(checkout,self.checkout_object_send.copy())
+        checkout = self.client.Checkout.create(self.checkout_object.copy())
+        response = checkout.sendSms(self.checkout_object_send.copy())
 
-    def test_06_checkout_cancel():
+        assert response.sms_sent == 1
 
+    def test_06_checkout_cancel(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
-        checkout = self.client.Checkout.cancel(self.checkout_object_send.copy())
+        checkout = self.client.Checkout.create(self.checkout_object.copy())
+        canceled_checkout = checkout.cancel(self.checkout_object_send.copy())
 
-        assert checkout.status == "Cancelled"
+        assert canceled_checkout.status == "Cancelled"
 
-    def test_07_orders_checkout_create(self)
+    def test_07_orders_checkout_create(self):
+        self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
+        order = self.client.Order.create(self.checkout_order_object.copy())
 
-       self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
-        order = self.checkout_order_object.copy()
-        order = self.client.Order.create(order)
-        checkout = order.createCheckout(self.checkout_order_object.copy())
-        
+        checkout = order.checkout
         assert checkout.type == "Integration"
-        assert checkout.status != "Issued"
-        assert checkout.url.startswith("https:\\pay.conekta")
-        assert checkout.id.len() == 36
+        assert checkout.status == "Issued"
+        assert len(checkout.id) == 36
 
+    def test_08_orders_checkout_create_redirection(self):
+        self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
+        order = self.client.Order.create(self.checkout_order__redirect_object.copy())
 
-    def test_08_orders_checkout_create_redireccion(self)
-
-       self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
-        order = self.checkout_order__redirect_object.copy()
-        order = self.client.Order.create(order)
-        checkout = order.createCheckout(self.checkout_order__redirect_object.copy())
-        
+        checkout = order.checkout
         assert checkout.type == "HostedPayment"
-        assert checkout.status != "Issued"
-        assert checkout.url.startswith("https:\\pay.conekta")
-        assert checkout.id.len() == 36
-
-    def test_09_orders_checkout__msi_create(self)
-
-       self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
-        order = self.checkout_order_object.copy()
-        order = self.client.Order.create(order)
-        checkout = order.createCheckout(self.checkout_order_object.copy())
-        
-        assert checkout.monthly_installments_enabled = True,
+        assert checkout.status == "Issued"
+        assert checkout.url.startswith("https://pay.conekta")
+        assert len(checkout.id) == 36
+
+    def test_09_orders_checkout__msi_create(self):
+        self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
+        order = self.client.Order.create(self.checkout_order_object.copy())
+
+        checkout = order.checkout
+        self.assertFalse(checkout.monthly_installments_enabled)
         assert checkout.type == "Integration"
-        assert checkout.status != "Issued"
-        assert checkout.url.startswith("https:\\pay.conekta")
-        assert checkout.id.len() == 36
+        assert checkout.status == "Issued"
+        assert len(checkout.id) == 36
```

### Comparing `conekta-2.6.1/tests/test_customer.py` & `conekta-2.6.2/tests/test_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/usr/bin/python
-#coding: utf-8
-#(c) 2017 Ramses Carbajal <@RamsesCarbajal>
+# coding: utf-8
+# (c) 2017 Ramses Carbajal <@RamsesCarbajal>
 from . import BaseEndpointTestCase
 
-class OrdersEndpointTestCase(BaseEndpointTestCase):
+
+class CustomersEndpointTestCase(BaseEndpointTestCase):
 
     def test_01_customer_create(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer = self.client.Customer.create(self.customer_object.copy())
         payment_source = customer.payment_sources[0]
         shipping_contact = customer.shipping_contacts[0]
 
-        assert customer.name  == 'James Howlett'
+        assert customer.name == 'James Howlett'
         assert customer.email == 'logan@x-men.org'
         assert customer.phone == '+525511223344'
-        assert payment_source.brand.lower() == 'visa' or payment_source.brand.lower() == 'mc'
+        assert payment_source.brand.lower() == 'visa' or payment_source.brand.lower() == 'mastercard'
         assert payment_source.last4 == '4242' or payment_source.last4 == '5100'
-        assert payment_source.type  == 'card'
+        assert payment_source.type == 'card'
 
-        assert shipping_contact.receiver        == "Marvin Fuller"
+        assert shipping_contact.receiver == "Marvin Fuller"
         assert shipping_contact.between_streets == "Ackerman Crescent"
-        assert shipping_contact.address.city    == "Red Deer"
+        assert shipping_contact.address.city == "Red Deer"
 
     def test_02_customer_add_token(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer_params = self.customer_object.copy()
         del customer_params["payment_sources"]
         customer = self.client.Customer.create(customer_params)
         payment_source = customer.createPaymentSource(self.payment_source_object.copy())
@@ -34,15 +35,15 @@
 
     def test_03_customer_update_payment_source(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer = self.client.Customer.create(self.customer_object.copy())
         payment_source = customer.payment_sources[0]
         payment_source.update(self.update_payment_source_object.copy())
         payment_source = customer.payment_sources[0]
-        assert payment_source.brand.lower() == 'visa' or payment_source.brand.lower() == 'mc'
+        assert payment_source.brand.lower() == 'visa' or payment_source.brand.lower() == 'mastercard'
         assert payment_source.last4 == '4242' or payment_source.last4 == '5100'
 
     def test_04_customer_delete_payment_source(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer = self.client.Customer.create(self.customer_object.copy())
         payment_source = customer.payment_sources[0]
 
@@ -58,19 +59,19 @@
     def test_08_customer_add_shipping_contact(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer_params = self.customer_object.copy()
         del customer_params["shipping_contacts"]
         customer = self.client.Customer.create(customer_params)
         shipping_contact = customer.createShippingContact(self.shipping_contact_object.copy())
 
-        assert shipping_contact.phone           == "+525511008811"
-        assert shipping_contact.receiver        == "Dr. Manhatan"
+        assert shipping_contact.phone == "+525511008811"
+        assert shipping_contact.receiver == "Dr. Manhatan"
         assert shipping_contact.between_streets == "some streets"
 
     def test_09_customer_update_plan(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer = self.client.Customer.create(self.customer_object.copy())
-        customer.createSubscription({"plan":"gold-plan"})
-        customer.subscription.update({"plan":"opal-plan"})
+        customer.createSubscription({"plan": "gold-plan"})
+        customer.subscription.update({"plan": "opal-plan"})
         customer2 = self.client.Customer.find(customer.id)
 
         assert customer2.subscription.plan_id == "opal-plan"
```

### Comparing `conekta-2.6.1/tests/test_events.py` & `conekta-2.6.2/tests/test_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/python
-#coding: utf-8
-#(c) 2013 Julian Ceballos <@jceb>
-#(c) 2014- Leo Fischer / Conekta <@leofischer/@conektaio>
+# coding: utf-8
+# (c) 2013 Julian Ceballos <@jceb>
+# (c) 2014- Leo Fischer / Conekta <@leofischer/@conektaio>
 
 from . import BaseEndpointTestCase
 
-class OrdersEndpointTestCase(BaseEndpointTestCase):
+
+class EventsEndpointTestCase(BaseEndpointTestCase):
 
     def test_01_order_event(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         order = self.client.Order.create(self.order_object.copy())
         event = order.events()
 
         assert event.data
 
-
     def test_02_line_item_event(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         raw_order = self.order_object.copy()
         raw_order["charges"] = None
         order = self.client.Order.create(raw_order)
 
         line_item = order.line_items[0]
```

### Comparing `conekta-2.6.1/tests/test_orders.py` & `conekta-2.6.2/tests/test_orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/python
-#coding: utf-8
-#(c) 2017 Ramses Carbajal <@RamsesCarbajal>
+# coding: utf-8
+# (c) 2017 Ramses Carbajal <@RamsesCarbajal>
 
 from . import BaseEndpointTestCase
 from nose.tools import assert_raises
 
+
 class OrdersEndpointTestCase(BaseEndpointTestCase):
 
     def test_01_order_create(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         order = self.client.Order.create(self.order_object.copy())
         assert order.currency
         line_item = order.line_items[0]
@@ -93,19 +94,19 @@
         line_item = order.line_items[0]
         assert line_item.unit_price == 30000
         assert line_item.description == "some description"
 
     def test_09_order_get_all_line_items(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
 
-        large_order_by_find  = self.client.Order.find('ord_2h9umNjHAzx8ZMtPA')
-        large_order_by_where = self.client.Order.where({'id':'ord_2h9umNjHAzx8ZMtPA'})
+        large_order_by_find = self.client.Order.find('ord_2ti8wMTYM7UnpS8Gd')
+        large_order_by_where = self.client.Order.where({'search': 'ord_2ti8wMTYM7UnpS8Gd'})
 
-        assert len(large_order_by_where.data[0].line_items) == 15
-        assert len(large_order_by_find.line_items) == 15
+        assert len(large_order_by_where.data[0].line_items) == 1
+        assert len(large_order_by_find.line_items) == 1
 
     def test_10_order_update_tax_line(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         raw_order = self.order_object.copy()
         del raw_order["charges"]
         order = self.client.Order.create(raw_order)
         tax_line = order.tax_lines[0]
@@ -141,30 +142,28 @@
         discount_line.update(raw_discount_line)
         discount_line = order.discount_lines[0]
         assert discount_line.code == "promocion"
 
     def test_13_order_with_token_id(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         raw_order = self.order_object.copy()
-        charge = {}
-        charge["payment_method"] = {}
+        charge = {"payment_method": {}}
         charge["payment_method"]["type"] = "card"
         charge["payment_method"]["token_id"] = "tok_test_visa_4242"
         raw_order["charges"] = [charge]
 
         order = self.client.Order.create(raw_order)
         charge = order.charges[0]
         assert charge.status == "paid"
         assert charge.amount == 20000
 
     def test_14_order_capture(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         raw_order = self.order_object.copy()
-        charge = {}
-        charge["payment_method"] = {}
+        charge = {"payment_method": {}}
         charge["payment_method"]["type"] = "card"
         charge["payment_method"]["token_id"] = "tok_test_visa_4242"
         raw_order["charges"] = [charge]
         raw_order["pre_authorize"] = True
         order = self.client.Order.create(raw_order)
 
         assert order.charges[0].amount == 20000
@@ -197,28 +196,27 @@
         refunded_order = order.refund(order_refund_params)
 
         assert refunded_order.payment_status == "refunded"
 
     def test_15_order_void(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         raw_order = self.order_object.copy()
-        charge = {}
-        charge["payment_method"] = {}
+        charge = {"payment_method": {}}
         charge["payment_method"]["type"] = "card"
         charge["payment_method"]["token_id"] = "tok_test_visa_4242"
         raw_order["charges"] = [charge]
         raw_order["pre_authorize"] = True
         order = self.client.Order.create(raw_order)
 
         assert order.charges[0].amount == 20000
         assert order.charges[0].status == "pre_authorized"
         assert order.payment_status == "pre_authorized"
 
         refunded_order = order.void()
-        
+
         assert refunded_order.payment_status == "voided"
 
     def test_16_order_delete_line_item(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         raw_order = self.order_object.copy()
         del raw_order["charges"]
         order = self.client.Order.create(raw_order)
@@ -273,15 +271,14 @@
 
         assert discount_line_deleted.deleted == True
 
         discount_line = order.discount_lines[0]
         assert discount_line.code == "descuento"
         assert discount_line.type == "loyalty"
 
-
     def test_19_order_create_with_customer_id(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer = self.client.Customer.create(self.customer_object.copy())
         order_params = self.order_object.copy()
         del order_params["customer_info"]
         order_params["customer_info"] = {}
         order_params["customer_info"]["customer_id"] = customer.id
```

### Comparing `conekta-2.6.1/tests/test_pagination.py` & `conekta-2.6.2/tests/test_pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 #!/usr/bin/python
-#coding: utf-8
-#(c) 2017 Ramses Carbajal <@RamsesCarbajal>
+# coding: utf-8
+# (c) 2017 Ramses Carbajal <@RamsesCarbajal>
+import unittest
 
 from . import BaseEndpointTestCase
 
-class OrdersEndpointTestCase(BaseEndpointTestCase):
+
+class PaginationEndpointTestCase(BaseEndpointTestCase):
 
     def test_01_customer_all(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer1 = self.client.Customer.create(self.customer_object.copy())
         customer2 = self.client.Customer.create(self.customer_object.copy())
         customer3 = self.client.Customer.create(self.customer_object.copy())
-        
+
         customers = self.client.Customer.where()
-        assert customers.data[0].id    
+        assert customers.data[0].id
 
     def test_02_customer_pagination_next(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer1 = self.client.Customer.create(self.customer_object.copy())
         customer2 = self.client.Customer.create(self.customer_object.copy())
         customer3 = self.client.Customer.create(self.customer_object.copy())
         query = {}
         query["next"] = customer1.id
         customers = self.client.Customer.where(query)
         new_search = customers.next()
 
         custs = new_search.data
-        assert new_search.data[0].id     
+        assert new_search.data[0].id
 
     def test_03_customer_pagination_before(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         customer1 = self.client.Customer.create(self.customer_object.copy())
         customer2 = self.client.Customer.create(self.customer_object.copy())
         customer3 = self.client.Customer.create(self.customer_object.copy())
         query = {}
         query["previous"] = customer1.id
         customers = self.client.Customer.where(query)
         new_search = customers.next()
-        
+
         custs = new_search.data
         assert custs[0].id
 
     def test_04_order_all(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         self.client.Order.create(self.order_object.copy())
         self.client.Order.create(self.order_object.copy())
         self.client.Order.create(self.order_object.copy())
-        
+
         orders = self.client.Order.where()
         assert orders.data[0].id
 
     def test_05_order_pagination_next(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         order1 = self.client.Order.create(self.order_object.copy())
         order2 = self.client.Order.create(self.order_object.copy())
         order3 = self.client.Order.create(self.order_object.copy())
         query = {}
         query["next"] = order1.id
         orders = self.client.Order.where(query)
         new_search = orders.next()
 
         orders = new_search.data
-        assert new_search.data[0].id     
+        assert new_search.data[0].id
 
+    @unittest.skip("reason for skipping")
     def test_05_order_pagination_before(self):
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
         order1 = self.client.Order.create(self.order_object.copy())
         order2 = self.client.Order.create(self.order_object.copy())
         order3 = self.client.Order.create(self.order_object.copy())
-        query = {}
-        query["previous"] = order1.id
+        query = {"previous": order1.id}
         orders = self.client.Order.where(query)
         new_search = orders.next()
 
         orders = new_search.data
-        assert new_search.data[0].id    
-
-        
+        assert orders[0].id
```

### Comparing `conekta-2.6.1/tests/test_webhooks.py` & `conekta-2.6.2/tests/test_webhooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/python
-#coding: utf-8
-#(c) 2016- Leo Fischer / Conekta <@leofischer/@conektaio>
+# coding: utf-8
+# (c) 2016- Leo Fischer / Conekta <@leofischer/@conektaio>
 
 from . import BaseEndpointTestCase
 
-class OrdersEndpointTestCase(BaseEndpointTestCase):
+
+class WebhooksEndpointTestCase(BaseEndpointTestCase):
     def test_1_webhooks(self):
         url = 'https://www.example.com'
-        url2 = url + '/new_endpoint' 
+        url2 = url + '/new_endpoint'
 
         self.client.api_key = 'key_ZLy4aP2szht1HqzkCezDEA'
-        webhook = self.client.Webhook.create({'url':url})
+        webhook = self.client.Webhook.create({'url': url})
         assert webhook.url == url
-        webhook.update({'url':url2})
+        webhook.update({'url': url2})
         assert webhook.url == url2
         webhook.delete()
         assert webhook.deleted
```

