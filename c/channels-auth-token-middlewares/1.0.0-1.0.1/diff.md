# Comparing `tmp/channels_auth_token_middlewares-1.0.0.tar.gz` & `tmp/channels_auth_token_middlewares-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "channels_auth_token_middlewares-1.0.0.tar", last modified: Mon Mar 14 17:44:22 2022, max compression
+gzip compressed data, was "channels_auth_token_middlewares-1.0.1.tar", last modified: Mon Apr 17 19:25:11 2023, max compression
```

## Comparing `channels_auth_token_middlewares-1.0.0.tar` & `channels_auth_token_middlewares-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 17:44:22.104106 channels_auth_token_middlewares-1.0.0/
--rw-rw-r--   0 root         (0) root         (0)    11358 2022-02-24 20:17:02.000000 channels_auth_token_middlewares-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1760 2022-03-14 17:44:22.104106 channels_auth_token_middlewares-1.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      774 2022-03-11 20:27:31.000000 channels_auth_token_middlewares-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 17:44:22.100106 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-02-27 19:09:51.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      764 2022-02-24 20:19:56.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 17:44:22.104106 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/middleware/
--rw-rw-r--   0 root         (0) root         (0)      788 2022-02-24 20:20:08.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/middleware/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5438 2022-02-24 20:20:17.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/middleware/base.py
--rw-rw-r--   0 root         (0) root         (0)     2291 2022-02-27 18:53:12.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/middleware/drf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-14 17:44:22.104106 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1760 2022-03-14 17:44:21.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2022-03-14 17:44:22.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-14 17:44:21.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-03-14 17:44:21.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-03-14 17:44:22.000000 channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-14 17:44:22.104106 channels_auth_token_middlewares-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1240 2022-02-26 20:28:41.000000 channels_auth_token_middlewares-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1038 2023-04-17 18:28:46.000000 channels_auth_token_middlewares-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.456685 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      764 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/
+-rw-rw-r--   0 root         (0) root         (0)      788 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5746 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/base.py
+-rw-rw-r--   0 root         (0) root         (0)     2291 2023-04-17 14:50:45.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/drf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 19:25:11.456685 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-17 19:25:11.000000 channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 19:25:11.460685 channels_auth_token_middlewares-1.0.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1290 2023-04-17 19:08:37.000000 channels_auth_token_middlewares-1.0.1/setup.py
```

### Comparing `channels_auth_token_middlewares-1.0.0/LICENSE` & `channels_auth_token_middlewares-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.0/PKG-INFO` & `channels_auth_token_middlewares-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: channels_auth_token_middlewares
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Channels auth token middlewares
 Home-page: https://github.com/YegorDB/django-channels-auth-token-middlewares
 Author: Yegor Bitensky
-License: UNKNOWN
 Keywords: django channels middleware
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Channels auth token middlewares
 
@@ -30,16 +29,24 @@
 
 ## Requirements
 - Python>=3.6
 - Channels>=3
 
 
 ## Install
-`$ pip install channels_auth_token_middlewares`
-
+1. `$ pip install channels-auth-token-middlewares`
+2. Add app name to `INSTALLED_APPS`
+```python
+INSTALLED_APPS = [
+    # base django apps (django.contrib.auth is required)
+    # other apps this one depends on (like rest_framework if it's necessary)
+    'channels_auth_token_middlewares',
+    # custom apps
+]
+```
 
 ## Tutorial
 [Explore](tutorial)
 
 
 ## Docs
 [Explore](docs)
@@ -54,9 +61,7 @@
 ### Usage
 
 #### Run
 `$ docker-compose -f docker-compose.tests.yml up`
 
 #### Clean
 `$ docker-compose -f docker-compose.tests.yml down`
-
-
```

### Comparing `channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/apps.py` & `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/apps.py`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/middleware/__init__.py` & `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/middleware/base.py` & `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,35 +89,42 @@
         Must be implemented by subclass to get user instance by token key.
         Implementation need to returns user instance or None.
         """
         raise NotImplementedError(
             "subclasses of BaseAuthTokenMiddleware "
             "must provide a get_user_instance(token_key) method")
 
+    def get_scope_header_value(self, scope, header_name):
+        if isinstance(header_name, str):
+            header_name = header_name.encode()
+        elif not isinstance(header_name, bytes):
+            raise ValueError("Header name must be string or bytes")
+
+        headers = dict(scope["headers"])
+        value = headers.get(header_name, headers.get(header_name.lower()))
+
+        if not value:
+            return None
+        return value.decode()
+
 
 class HeaderAuthTokenMiddleware(BaseAuthTokenMiddleware):
     """Base middleware which parses token key from request header."""
 
     header_name = None
     keyword = None
 
     def __init__(self, *args, header_name=None, keyword=None, **kwargs):
         self.header_name = str(header_name or self.header_name)
-        self.header_name = self.header_name.lower().encode()
-
         self.keyword = str(keyword or self.keyword)
 
         super().__init__(*args, **kwargs)
 
     def get_token_key_string(self, scope):
-        headers = dict(scope["headers"])
-        value = headers.get(self.header_name)
-        if not value:
-            return None
-        return value.decode()
+        return self.get_scope_header_value(scope, self.header_name)
 
     @property
     def token_key_string_regex(self):
         """
         Regex to parse token key from token key string.
         Token key need to be in first group.
         """
@@ -132,16 +139,16 @@
 
     def __init__(self, *args, cookie_name=None, **kwargs):
         self.cookie_name = str(cookie_name or self.cookie_name)
 
         super().__init__(*args, **kwargs)
 
     def get_token_key_string(self, scope):
-        headers = dict(scope["headers"])
-        cookie_raw_data = headers.get(b"cookie", b"").decode()
+        header_name = "Cookie"
+        cookie_raw_data = self.get_scope_header_value(scope, header_name) or ''
         cookie = BaseCookie()
         cookie.load(cookie_raw_data)
         cookie_item = cookie.get(self.cookie_name)
         if not cookie_item:
             return None
         return cookie_item.value
```

### Comparing `channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares/middleware/drf.py` & `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares/middleware/drf.py`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/PKG-INFO` & `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: channels-auth-token-middlewares
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Channels auth token middlewares
 Home-page: https://github.com/YegorDB/django-channels-auth-token-middlewares
 Author: Yegor Bitensky
-License: UNKNOWN
 Keywords: django channels middleware
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Channels auth token middlewares
 
@@ -30,16 +29,24 @@
 
 ## Requirements
 - Python>=3.6
 - Channels>=3
 
 
 ## Install
-`$ pip install channels_auth_token_middlewares`
-
+1. `$ pip install channels-auth-token-middlewares`
+2. Add app name to `INSTALLED_APPS`
+```python
+INSTALLED_APPS = [
+    # base django apps (django.contrib.auth is required)
+    # other apps this one depends on (like rest_framework if it's necessary)
+    'channels_auth_token_middlewares',
+    # custom apps
+]
+```
 
 ## Tutorial
 [Explore](tutorial)
 
 
 ## Docs
 [Explore](docs)
@@ -54,9 +61,7 @@
 ### Usage
 
 #### Run
 `$ docker-compose -f docker-compose.tests.yml up`
 
 #### Clean
 `$ docker-compose -f docker-compose.tests.yml down`
-
-
```

### Comparing `channels_auth_token_middlewares-1.0.0/channels_auth_token_middlewares.egg-info/SOURCES.txt` & `channels_auth_token_middlewares-1.0.1/channels_auth_token_middlewares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `channels_auth_token_middlewares-1.0.0/setup.py` & `channels_auth_token_middlewares-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="channels_auth_token_middlewares",
-    version="1.0.0",
+    version="1.0.1",
     description="Django Channels auth token middlewares",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/YegorDB/django-channels-auth-token-middlewares",
     author="Yegor Bitensky",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -21,14 +21,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="django channels middleware",
     packages=find_packages(exclude=["docs*", "tests*", "tutorial*"]),
     python_requires=">=3.6",
     install_requires=["channels>=3"],
 )
```

