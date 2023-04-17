# Comparing `tmp/HTTP-PyServer-0.0.3.tar.gz` & `tmp/HTTP-PyServer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.0.3.tar", last modified: Thu Apr 13 03:22:47 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.0.4.tar", last modified: Mon Apr 17 15:25:24 2023, max compression
```

## Comparing `HTTP-PyServer-0.0.3.tar` & `HTTP-PyServer-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:22:47.413127 HTTP-PyServer-0.0.3/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2024 2023-04-13 03:22:47.411127 HTTP-PyServer-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1473 2023-04-13 03:09:58.000000 HTTP-PyServer-0.0.3/README.md
--rw-rw-rw-   0        0        0      629 2023-04-13 03:22:24.000000 HTTP-PyServer-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 03:22:47.413127 HTTP-PyServer-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-13 03:22:47.355276 HTTP-PyServer-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 03:22:47.381207 HTTP-PyServer-0.0.3/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2024 2023-04-13 03:22:47.000000 HTTP-PyServer-0.0.3/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-04-13 03:22:47.000000 HTTP-PyServer-0.0.3/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:22:47.000000 HTTP-PyServer-0.0.3/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 03:22:47.000000 HTTP-PyServer-0.0.3/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 03:22:47.409132 HTTP-PyServer-0.0.3/src/server/
--rw-rw-rw-   0        0        0      191 2023-04-13 02:01:27.000000 HTTP-PyServer-0.0.3/src/server/__init__.py
--rw-rw-rw-   0        0        0     5364 2023-04-13 03:02:53.000000 HTTP-PyServer-0.0.3/src/server/render.py
--rw-rw-rw-   0        0        0     2150 2023-04-12 04:52:51.000000 HTTP-PyServer-0.0.3/src/server/request.py
--rw-rw-rw-   0        0        0     3930 2023-04-13 01:37:40.000000 HTTP-PyServer-0.0.3/src/server/responses.py
--rw-rw-rw-   0        0        0     3656 2023-04-13 02:47:16.000000 HTTP-PyServer-0.0.3/src/server/routes.py
--rw-rw-rw-   0        0        0     4229 2023-04-12 19:38:44.000000 HTTP-PyServer-0.0.3/src/server/server.py
+drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.243085 HTTP-PyServer-0.0.4/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2036 2023-04-17 15:25:24.242087 HTTP-PyServer-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1473 2023-04-13 03:09:58.000000 HTTP-PyServer-0.0.4/README.md
+-rw-rw-rw-   0        0        0      641 2023-04-17 15:21:34.000000 HTTP-PyServer-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 15:25:24.244083 HTTP-PyServer-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.165295 HTTP-PyServer-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.219152 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2036 2023-04-17 15:25:23.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-04-17 15:25:24.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 15:25:23.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 15:25:23.000000 HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 15:25:24.239095 HTTP-PyServer-0.0.4/src/server/
+-rw-rw-rw-   0        0        0      191 2023-04-13 02:01:27.000000 HTTP-PyServer-0.0.4/src/server/__init__.py
+-rw-rw-rw-   0        0        0     5364 2023-04-13 03:02:53.000000 HTTP-PyServer-0.0.4/src/server/render.py
+-rw-rw-rw-   0        0        0     2347 2023-04-17 15:20:32.000000 HTTP-PyServer-0.0.4/src/server/request.py
+-rw-rw-rw-   0        0        0     3930 2023-04-13 01:37:40.000000 HTTP-PyServer-0.0.4/src/server/responses.py
+-rw-rw-rw-   0        0        0     3656 2023-04-13 02:47:16.000000 HTTP-PyServer-0.0.4/src/server/routes.py
+-rw-rw-rw-   0        0        0     4387 2023-04-17 15:21:28.000000 HTTP-PyServer-0.0.4/src/server/server.py
```

### Comparing `HTTP-PyServer-0.0.3/LICENSE` & `HTTP-PyServer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.0.3/PKG-INFO` & `HTTP-PyServer-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.0.3
-Summary: Simple way to make complex http servers
+Version: 0.0.4
+Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HTTP-PyServer-0.0.3/README.md` & `HTTP-PyServer-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.0.3/pyproject.toml` & `HTTP-PyServer-0.0.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
-description = "Simple way to make complex http servers"
+description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `HTTP-PyServer-0.0.3/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.0.4/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.0.3
-Summary: Simple way to make complex http servers
+Version: 0.0.4
+Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HTTP-PyServer-0.0.3/src/server/render.py` & `HTTP-PyServer-0.0.4/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.0.3/src/server/request.py` & `HTTP-PyServer-0.0.4/src/server/request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import urllib
 
 class Request:
 
     def __init__(self,
                  *args,
+                 address: tuple = (),
                  method: str = '',
                  path: str = '',
                  version: str = '',
                  headers: dict = {},
                  body: str = '',
                  query: dict = {},
                  values: dict = {}):
         '''Initializes the request class.'''
 
+        self.address = address
+
         self.method = method
 
         self.path = path
 
         self.version = version
 
         self.headers = headers
@@ -26,14 +29,15 @@
         self.query = query
 
         self.values = values
 
     @classmethod
     def from_string(cls,
                     *args,
+                    address: tuple = (),
                     request: str):
         '''Creates a request object from an HTTP request string.'''
 
         lines = request.split('\r\n')
 
         method, path, version = lines[0].split(' ')
 
@@ -73,21 +77,23 @@
 
             values = dict()
 
             for key, value in urllib.parse.parse_qs(body).items():
 
                 values[key] = value[0]
 
-            return cls(method = method,
+            return cls(address = address,
+                       method = method,
                        path = path,
                        version = version,
                        headers = headers,
                        body = body,
                        query = query,
                        values = values)
 
-        return cls(method = method,
+        return cls(address = address,
+                   method = method,
                    path = path,
                    version = version,
                    headers = headers,
                    body = body,
                    query = query)
```

### Comparing `HTTP-PyServer-0.0.3/src/server/responses.py` & `HTTP-PyServer-0.0.4/src/server/responses.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.0.3/src/server/routes.py` & `HTTP-PyServer-0.0.4/src/server/routes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.0.3/src/server/server.py` & `HTTP-PyServer-0.0.4/src/server/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
                 connection.close()
 
                 return None
 
         try:
 
-            parsed_request = request.Request.from_string(request = raw_request)
+            parsed_request = request.Request.from_string(address = address,
+                                                         request = raw_request)
 
         except:
 
             logging.error(f'Invalid request from {address[0]}:{address[1]}, closing connection.')
 
             connection.close()
 
@@ -47,15 +48,16 @@
         if content_length:=parsed_request.headers.get('Content-Length'):
 
             if length_recieved:=len(raw_request.split('\r\n\r\n')[1]) < (length_to_recieve:=int(content_length)):
 
                 raw_request += connection.recv(length_to_recieve - length_recieved).decode(encoding = 'utf-8',
                                                                                            errors = 'ignore')
 
-                parsed_request = request.Request.from_string(request = raw_request)
+                parsed_request = request.Request.from_string(address = address,
+                                                             request = raw_request)
 
         logging.debug(f'Recieved {parsed_request.method.title()} request from {address[0]}:{address[1]} for {parsed_request.path if parsed_request.path else "/"}')
 
         connection.send(routes.Routes.get_route(path = parsed_request.path,
                                                 request = parsed_request))
 
         logging.debug(f'Sent {parsed_request.method} response to {address[0]}:{address[1]} for {parsed_request.path if parsed_request.path else "/"}')
```

