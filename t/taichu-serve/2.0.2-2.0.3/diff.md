# Comparing `tmp/taichu-serve-2.0.2.tar.gz` & `tmp/taichu-serve-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taichu-serve-2.0.2.tar", last modified: Fri Apr 14 06:11:49 2023, max compression
+gzip compressed data, was "taichu-serve-2.0.3.tar", last modified: Mon Apr 17 06:42:14 2023, max compression
```

## Comparing `taichu-serve-2.0.2.tar` & `taichu-serve-2.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.152250 taichu-serve-2.0.2/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-14 06:11:49.152112 taichu-serve-2.0.2/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-14 06:11:49.152290 taichu-serve-2.0.2/setup.cfg
--rw-r--r--   0 chen       (501) staff       (20)      949 2023-04-14 06:11:45.000000 taichu-serve-2.0.2/setup.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.150879 taichu-serve-2.0.2/taichu_serve/
--rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.2/taichu_serve/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.2/taichu_serve/app.py
--rw-r--r--   0 chen       (501) staff       (20)     2410 2023-04-14 05:13:39.000000 taichu-serve-2.0.2/taichu_serve/command.py
--rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/common.py
--rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.2/taichu_serve/error_code.py
--rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2.py
--rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2_grpc.py
--rw-r--r--   0 chen       (501) staff       (20)     3572 2023-04-14 05:10:28.000000 taichu-serve-2.0.2/taichu_serve/grpc_server.py
--rw-r--r--   0 chen       (501) staff       (20)     2103 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/log.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.151939 taichu-serve-2.0.2/taichu_serve/model_def/
--rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-2.0.2/taichu_serve/model_def/__init__.py
--rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.2/taichu_serve/model_server.py
--rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.2/taichu_serve/ratelimiter.py
--rw-r--r--   0 chen       (501) staff       (20)     1924 2023-04-14 05:14:20.000000 taichu-serve-2.0.2/taichu_serve/settings.py
-drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-14 06:11:49.151798 taichu-serve-2.0.2/taichu_serve.egg-info/
--rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/PKG-INFO
--rw-r--r--   0 chen       (501) staff       (20)      587 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (501) staff       (20)       73 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/entry_points.txt
--rw-r--r--   0 chen       (501) staff       (20)       58 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/requires.txt
--rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-14 06:11:49.000000 taichu-serve-2.0.2/taichu_serve.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-17 06:42:14.740221 taichu-serve-2.0.3/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-17 06:42:14.740024 taichu-serve-2.0.3/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-04-17 06:42:14.740267 taichu-serve-2.0.3/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      940 2023-04-17 05:12:30.000000 taichu-serve-2.0.3/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-17 06:42:14.738696 taichu-serve-2.0.3/taichu_serve/
+-rw-r--r--   0 chen       (501) staff       (20)     3398 2023-04-14 02:56:12.000000 taichu-serve-2.0.3/taichu_serve/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9214 2023-04-14 05:19:23.000000 taichu-serve-2.0.3/taichu_serve/app.py
+-rw-r--r--   0 chen       (501) staff       (20)     2369 2023-04-17 06:39:04.000000 taichu-serve-2.0.3/taichu_serve/command.py
+-rw-r--r--   0 chen       (501) staff       (20)      948 2023-04-13 09:06:46.000000 taichu-serve-2.0.3/taichu_serve/common.py
+-rw-r--r--   0 chen       (501) staff       (20)     1521 2023-04-14 04:52:00.000000 taichu-serve-2.0.3/taichu_serve/error_code.py
+-rw-r--r--   0 chen       (501) staff       (20)     6336 2023-04-12 06:27:59.000000 taichu-serve-2.0.3/taichu_serve/grpc_predict_v2_pb2.py
+-rw-r--r--   0 chen       (501) staff       (20)    13010 2023-04-13 09:06:46.000000 taichu-serve-2.0.3/taichu_serve/grpc_predict_v2_pb2_grpc.py
+-rw-r--r--   0 chen       (501) staff       (20)     4697 2023-04-17 04:31:53.000000 taichu-serve-2.0.3/taichu_serve/grpc_server.py
+-rw-r--r--   0 chen       (501) staff       (20)     2104 2023-04-14 09:24:14.000000 taichu-serve-2.0.3/taichu_serve/log.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-17 06:42:14.739801 taichu-serve-2.0.3/taichu_serve/model_def/
+-rw-r--r--   0 chen       (501) staff       (20)        0 2023-02-07 00:50:51.000000 taichu-serve-2.0.3/taichu_serve/model_def/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     5444 2023-04-14 01:39:52.000000 taichu-serve-2.0.3/taichu_serve/model_server.py
+-rw-r--r--   0 chen       (501) staff       (20)      205 2023-04-13 09:06:46.000000 taichu-serve-2.0.3/taichu_serve/ratelimiter.py
+-rw-r--r--   0 chen       (501) staff       (20)     2081 2023-04-17 04:59:33.000000 taichu-serve-2.0.3/taichu_serve/settings.py
+-rw-r--r--   0 chen       (501) staff       (20)     2841 2023-04-17 06:41:51.000000 taichu-serve-2.0.3/taichu_serve/template.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-04-17 06:42:14.739674 taichu-serve-2.0.3/taichu_serve.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)      235 2023-04-17 06:42:14.000000 taichu-serve-2.0.3/taichu_serve.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      612 2023-04-17 06:42:14.000000 taichu-serve-2.0.3/taichu_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-04-17 06:42:14.000000 taichu-serve-2.0.3/taichu_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)       52 2023-04-17 06:42:14.000000 taichu-serve-2.0.3/taichu_serve.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (501) staff       (20)       53 2023-04-17 06:42:14.000000 taichu-serve-2.0.3/taichu_serve.egg-info/requires.txt
+-rw-r--r--   0 chen       (501) staff       (20)       13 2023-04-17 06:42:14.000000 taichu-serve-2.0.3/taichu_serve.egg-info/top_level.txt
```

### Comparing `taichu-serve-2.0.2/setup.py` & `taichu-serve-2.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 import taichu_serve
 
 pkgs = find_packages()
 
 if __name__ == '__main__':
     name = 'taichu-serve'
 
-    requirements = ['grpcio', 'grpcio-tools', 'protobuf', 'Flask', 'gunicorn', 'Jinja2', 'Pillow']
+    requirements = ['grpcio', 'grpcio-tools', 'protobuf',
+                    'Flask', 'gunicorn', 'requests']
 
     setup(
         name=name,
-        version='2.0.2',
+        version='2.0.3',
         description='taichu serve is a tool for serving deep learning inference',
         # long_description='',
         author='taichu platform team',
         # author_email='noreply@noreply.com',
         python_requires=">=3.6.0",
         url='',
         keywords='Serving Deep Learning Inference AI',
         packages=pkgs,
         install_requires=requirements,
         entry_points={
-            'console_scripts': ['taichu_serve = taichu_serve.command:infer_server_start']
+            'console_scripts': ['taichu = taichu_serve.command:cli']
         },
         include_package_data=True,
         # license='Apache License Version 2.0'
     )
```

### Comparing `taichu-serve-2.0.2/taichu_serve/__init__.py` & `taichu-serve-2.0.3/taichu_serve/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.2/taichu_serve/app.py` & `taichu-serve-2.0.3/taichu_serve/app.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.2/taichu_serve/common.py` & `taichu-serve-2.0.3/taichu_serve/common.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.2/taichu_serve/error_code.py` & `taichu-serve-2.0.3/taichu_serve/error_code.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2.py` & `taichu-serve-2.0.3/taichu_serve/grpc_predict_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.2/taichu_serve/grpc_predict_v2_pb2_grpc.py` & `taichu-serve-2.0.3/taichu_serve/grpc_predict_v2_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.2/taichu_serve/log.py` & `taichu-serve-2.0.3/taichu_serve/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import sys
 from typing import Optional
 
 from flask import request, g
 from taichu_serve.common import Local
 
+
 class JsonFormatter(logging.Formatter):
 
     def __init__(
             self,
             fmt: Optional[str] = "%(asctime)s",
             datefmt: Optional[str] = None,
             style: Optional[str] = "%",
```

### Comparing `taichu-serve-2.0.2/taichu_serve/model_server.py` & `taichu-serve-2.0.3/taichu_serve/model_server.py`

 * *Files identical despite different names*

### Comparing `taichu-serve-2.0.2/taichu_serve/settings.py` & `taichu-serve-2.0.3/taichu_serve/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 DEFAULT_TF_SERVER_PORT = 8500
 
 logger = logging.getLogger(__name__)
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Taichu Model Server')
+    parser.add_argument('action', action="store", choices=['init', 'serve'])
+    # parser.add_argument('name', action="store", default='default', type=str)
+
     parser.add_argument('--grpc_port', action="store", default=8889, type=int)
     parser.add_argument('--http_port', action="store", default=8888, type=int)
     parser.add_argument('--grpc_only', action="store", default=False, type=bool)
     parser.add_argument('--model_path', action="store", default='./', type=str)
     parser.add_argument('--service_file', action="store", default='customize_service.py', type=str)
     parser.add_argument('--max_concurrent_requests', action="store", default=1, type=int)
     parser.add_argument('--instances_num', action="store", default=1, type=int)
```

### Comparing `taichu-serve-2.0.2/taichu_serve.egg-info/SOURCES.txt` & `taichu-serve-2.0.3/taichu_serve.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 taichu_serve/grpc_predict_v2_pb2.py
 taichu_serve/grpc_predict_v2_pb2_grpc.py
 taichu_serve/grpc_server.py
 taichu_serve/log.py
 taichu_serve/model_server.py
 taichu_serve/ratelimiter.py
 taichu_serve/settings.py
+taichu_serve/template.py
 taichu_serve.egg-info/PKG-INFO
 taichu_serve.egg-info/SOURCES.txt
 taichu_serve.egg-info/dependency_links.txt
 taichu_serve.egg-info/entry_points.txt
 taichu_serve.egg-info/requires.txt
 taichu_serve.egg-info/top_level.txt
 taichu_serve/model_def/__init__.py
```

