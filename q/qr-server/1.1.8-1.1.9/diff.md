# Comparing `tmp/qr_server-1.1.8.tar.gz` & `tmp/qr_server-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qr_server-1.1.8.tar", last modified: Thu Oct 20 18:56:21 2022, max compression
+gzip compressed data, was "qr_server-1.1.9.tar", last modified: Thu Oct 20 19:05:14 2022, max compression
```

## Comparing `qr_server-1.1.8.tar` & `qr_server-1.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 18:56:21.049976 qr_server-1.1.8/
--rw-rw-r--   0 kurush    (1000) kurush    (1000)       73 2021-11-04 14:37:28.000000 qr_server-1.1.8/.gitignore
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     1075 2021-09-19 20:05:55.000000 qr_server-1.1.8/LICENSE
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     2570 2022-10-20 18:56:21.049976 qr_server-1.1.8/PKG-INFO
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     2080 2021-11-04 15:10:28.000000 qr_server-1.1.8/README.md
-drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 18:56:21.049976 qr_server-1.1.8/qr_server/
--rw-r--r--   0 kurush    (1000) kurush    (1000)     1935 2022-03-31 08:56:30.000000 qr_server-1.1.8/qr_server/Config.py
--rw-r--r--   0 kurush    (1000) kurush    (1000)      718 2021-11-17 14:46:14.000000 qr_server-1.1.8/qr_server/FileManager.py
--rw-r--r--   0 kurush    (1000) kurush    (1000)     2894 2022-09-18 13:36:45.000000 qr_server-1.1.8/qr_server/FlaskServer.py
--rw-r--r--   0 kurush    (1000) kurush    (1000)     2831 2021-11-04 15:07:44.000000 qr_server-1.1.8/qr_server/Logger.py
--rw-r--r--   0 kurush    (1000) kurush    (1000)     1527 2021-11-04 15:07:44.000000 qr_server-1.1.8/qr_server/Repository.py
--rw-r--r--   0 kurush    (1000) kurush    (1000)      472 2021-11-04 15:07:44.000000 qr_server-1.1.8/qr_server/RoleManager.py
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     2880 2022-10-20 18:56:11.000000 qr_server-1.1.8/qr_server/Server.py
--rw-r--r--   0 kurush    (1000) kurush    (1000)     3546 2021-11-04 15:07:44.000000 qr_server-1.1.8/qr_server/TokenManager.py
--rw-r--r--   0 kurush    (1000) kurush    (1000)      422 2021-11-04 15:07:44.000000 qr_server-1.1.8/qr_server/__init__.py
--rw-rw-r--   0 kurush    (1000) kurush    (1000)      867 2021-10-16 09:43:36.000000 qr_server-1.1.8/qr_server/dict_parsing.py
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     2403 2021-10-16 10:14:18.000000 qr_server-1.1.8/qr_server/dto_converter.py
-drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 18:56:21.049976 qr_server-1.1.8/qr_server/example/
--rw-rw-r--   0 kurush    (1000) kurush    (1000)      631 2021-11-04 15:10:22.000000 qr_server-1.1.8/qr_server/example/AuthRepository.py
--rw-rw-r--   0 kurush    (1000) kurush    (1000)      297 2021-11-04 14:07:07.000000 qr_server-1.1.8/qr_server/example/auth_dtos.py
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     1555 2021-11-04 15:10:22.000000 qr_server-1.1.8/qr_server/example/auth_service.py
--rw-rw-r--   0 kurush    (1000) kurush    (1000)      297 2021-11-04 14:07:07.000000 qr_server-1.1.8/qr_server/example/config.yaml
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     1325 2022-10-20 18:52:37.000000 qr_server-1.1.8/qr_server/request_sending.py
-drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 18:56:21.049976 qr_server-1.1.8/qr_server.egg-info/
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     2570 2022-10-20 18:56:20.000000 qr_server-1.1.8/qr_server.egg-info/PKG-INFO
--rw-rw-r--   0 kurush    (1000) kurush    (1000)      638 2022-10-20 18:56:20.000000 qr_server-1.1.8/qr_server.egg-info/SOURCES.txt
--rw-rw-r--   0 kurush    (1000) kurush    (1000)        1 2022-10-20 18:56:20.000000 qr_server-1.1.8/qr_server.egg-info/dependency_links.txt
--rw-rw-r--   0 kurush    (1000) kurush    (1000)      136 2022-10-20 18:56:20.000000 qr_server-1.1.8/qr_server.egg-info/requires.txt
--rw-rw-r--   0 kurush    (1000) kurush    (1000)       10 2022-10-20 18:56:20.000000 qr_server-1.1.8/qr_server.egg-info/top_level.txt
--rw-rw-r--   0 kurush    (1000) kurush    (1000)      121 2022-09-18 11:17:44.000000 qr_server-1.1.8/requirements.txt
--rw-rw-r--   0 kurush    (1000) kurush    (1000)       38 2022-10-20 18:56:21.049976 qr_server-1.1.8/setup.cfg
--rw-rw-r--   0 kurush    (1000) kurush    (1000)     2937 2022-10-20 18:56:15.000000 qr_server-1.1.8/setup.py
+drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 19:05:14.449108 qr_server-1.1.9/
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)       73 2021-11-04 14:37:28.000000 qr_server-1.1.9/.gitignore
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     1075 2021-09-19 20:05:55.000000 qr_server-1.1.9/LICENSE
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     2570 2022-10-20 19:05:14.449108 qr_server-1.1.9/PKG-INFO
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     2080 2021-11-04 15:10:28.000000 qr_server-1.1.9/README.md
+drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 19:05:14.449108 qr_server-1.1.9/qr_server/
+-rw-r--r--   0 kurush    (1000) kurush    (1000)     1935 2022-03-31 08:56:30.000000 qr_server-1.1.9/qr_server/Config.py
+-rw-r--r--   0 kurush    (1000) kurush    (1000)      718 2021-11-17 14:46:14.000000 qr_server-1.1.9/qr_server/FileManager.py
+-rw-r--r--   0 kurush    (1000) kurush    (1000)     3016 2022-10-20 19:05:10.000000 qr_server-1.1.9/qr_server/FlaskServer.py
+-rw-r--r--   0 kurush    (1000) kurush    (1000)     2831 2021-11-04 15:07:44.000000 qr_server-1.1.9/qr_server/Logger.py
+-rw-r--r--   0 kurush    (1000) kurush    (1000)     1527 2021-11-04 15:07:44.000000 qr_server-1.1.9/qr_server/Repository.py
+-rw-r--r--   0 kurush    (1000) kurush    (1000)      472 2021-11-04 15:07:44.000000 qr_server-1.1.9/qr_server/RoleManager.py
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     2880 2022-10-20 18:56:11.000000 qr_server-1.1.9/qr_server/Server.py
+-rw-r--r--   0 kurush    (1000) kurush    (1000)     3546 2021-11-04 15:07:44.000000 qr_server-1.1.9/qr_server/TokenManager.py
+-rw-r--r--   0 kurush    (1000) kurush    (1000)      422 2021-11-04 15:07:44.000000 qr_server-1.1.9/qr_server/__init__.py
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)      867 2021-10-16 09:43:36.000000 qr_server-1.1.9/qr_server/dict_parsing.py
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     2403 2021-10-16 10:14:18.000000 qr_server-1.1.9/qr_server/dto_converter.py
+drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 19:05:14.449108 qr_server-1.1.9/qr_server/example/
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)      631 2021-11-04 15:10:22.000000 qr_server-1.1.9/qr_server/example/AuthRepository.py
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)      297 2021-11-04 14:07:07.000000 qr_server-1.1.9/qr_server/example/auth_dtos.py
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     1555 2021-11-04 15:10:22.000000 qr_server-1.1.9/qr_server/example/auth_service.py
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)      297 2021-11-04 14:07:07.000000 qr_server-1.1.9/qr_server/example/config.yaml
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     1325 2022-10-20 18:52:37.000000 qr_server-1.1.9/qr_server/request_sending.py
+drwxrwxr-x   0 kurush    (1000) kurush    (1000)        0 2022-10-20 19:05:14.449108 qr_server-1.1.9/qr_server.egg-info/
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     2570 2022-10-20 19:05:14.000000 qr_server-1.1.9/qr_server.egg-info/PKG-INFO
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)      638 2022-10-20 19:05:14.000000 qr_server-1.1.9/qr_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)        1 2022-10-20 19:05:14.000000 qr_server-1.1.9/qr_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)      136 2022-10-20 19:05:14.000000 qr_server-1.1.9/qr_server.egg-info/requires.txt
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)       10 2022-10-20 19:05:14.000000 qr_server-1.1.9/qr_server.egg-info/top_level.txt
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)      121 2022-09-18 11:17:44.000000 qr_server-1.1.9/requirements.txt
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)       38 2022-10-20 19:05:14.449108 qr_server-1.1.9/setup.cfg
+-rw-rw-r--   0 kurush    (1000) kurush    (1000)     2937 2022-10-20 19:05:10.000000 qr_server-1.1.9/setup.py
```

### Comparing `qr_server-1.1.8/LICENSE` & `qr_server-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/PKG-INFO` & `qr_server-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qr_server
-Version: 1.1.8
+Version: 1.1.9
 Summary: console app builder
 Home-page: https://github.com/Kurush7/qr_server
 Author: Kurush
 Author-email: ze17@ya.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `qr_server-1.1.8/README.md` & `qr_server-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/Config.py` & `qr_server-1.1.9/qr_server/Config.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/FileManager.py` & `qr_server-1.1.9/qr_server/FileManager.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/FlaskServer.py` & `qr_server-1.1.9/qr_server/FlaskServer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 import time
 import gevent.pywsgi
 
 from .Server import *
 
 
 class FlaskContextCreator(IQRContextCreator):
-    def create_context(self, request, rep: IQRRepository) -> QRContext:
+    def create_context(self, request, rep: IQRRepository, meta: dict) -> QRContext:
         json = request.get_json(silent=True)
         if json is None:
             json = dict()
-        return QRContext(json, request.args, request.headers, request.form, request.files, rep)
+        return QRContext(json, request.args, request.headers, request.form, request.files, rep, meta)
 
 
 class FlaskServer(IQRServer, FlaskContextCreator, QRLogger):
     def __init__(self, default_err_code=500, default_err_msg='Internal server error'):
         FlaskContextCreator.__init__(self)
         QRLogger.__init__(self)
         self.app = None
         self.debug = None
         self.methods = {}
         self.managers = dict()
+        self.meta = dict()
 
         self.default_err_code = default_err_code
         self.default_err_msg = default_err_msg
 
     def init_server(self, config: IQRConfig):
         app_name = config['app_name']
         if app_name is None: app_name = 'app'
@@ -48,15 +49,15 @@
         """register method"""
         func = lambda *args, **kwargs: self.__method(f, *args, **kwargs)
         func.__name__ = f.__name__
         self.methods[f.__name__] = \
             self.app.route(route, methods=[method_type])(func)
 
     def __method(self, f, *args, **kwargs):
-        ctx = super().create_context(request, self)
+        ctx = super().create_context(request, self, meta=self.meta)
         ctx.set_managers(self.managers)
         in_msg = '[' + request.method + '] ' + request.url + '/' + request.query_string.decode()
         try:
             start = time.time()
             result = f(ctx, *args, **kwargs)
             end = time.time()
             msecs = int((end - start) * 1000)
@@ -76,7 +77,10 @@
         except Exception as e:
             super().info(in_msg)
             super().exception(e)
             return self.default_err_msg, self.default_err_code
 
     def register_manager(self, manager: IQRManager):
         self.managers[manager.get_name()] = manager
+
+    def set_meta(self, meta: dict):
+        self.meta = meta
```

### Comparing `qr_server-1.1.8/qr_server/Logger.py` & `qr_server-1.1.9/qr_server/Logger.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/Repository.py` & `qr_server-1.1.9/qr_server/Repository.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/Server.py` & `qr_server-1.1.9/qr_server/Server.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/TokenManager.py` & `qr_server-1.1.9/qr_server/TokenManager.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/dict_parsing.py` & `qr_server-1.1.9/qr_server/dict_parsing.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/dto_converter.py` & `qr_server-1.1.9/qr_server/dto_converter.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/example/AuthRepository.py` & `qr_server-1.1.9/qr_server/example/AuthRepository.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/example/auth_service.py` & `qr_server-1.1.9/qr_server/example/auth_service.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server/request_sending.py` & `qr_server-1.1.9/qr_server/request_sending.py`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/qr_server.egg-info/PKG-INFO` & `qr_server-1.1.9/qr_server.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qr-server
-Version: 1.1.8
+Version: 1.1.9
 Summary: console app builder
 Home-page: https://github.com/Kurush7/qr_server
 Author: Kurush
 Author-email: ze17@ya.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `qr_server-1.1.8/qr_server.egg-info/SOURCES.txt` & `qr_server-1.1.9/qr_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qr_server-1.1.8/setup.py` & `qr_server-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     'Inject',
     'requests',
     'gevent',
 ]
 
 setuptools.setup(
     name="qr_server",
-    version="1.1.8",
+    version="1.1.9",
     author="Kurush",
     author_email="ze17@ya.ru",
     description="console app builder",
     long_description_content_type="text/markdown",
     url="https://github.com/Kurush7/qr_server",
     packages=setuptools.find_packages(),
     install_requires=required,
```

