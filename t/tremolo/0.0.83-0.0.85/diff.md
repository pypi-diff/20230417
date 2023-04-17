# Comparing `tmp/tremolo-0.0.83.tar.gz` & `tmp/tremolo-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.83.tar", last modified: Sun Apr 16 13:38:25 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.85.tar", last modified: Mon Apr 17 00:28:38 2023, max compression
```

## Comparing `tremolo-0.0.83.tar` & `tremolo-0.0.85.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-16 13:38:25.000000 tremolo-0.0.83/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.83/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-16 13:38:25.000000 tremolo-0.0.83/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-16 13:32:51.000000 tremolo-0.0.83/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11749 2023-04-14 02:53:18.000000 tremolo-0.0.83/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13717 2023-04-12 23:43:31.000000 tremolo-0.0.83/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     8522 2023-04-16 13:13:40.000000 tremolo-0.0.83/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-14 02:53:02.000000 tremolo-0.0.83/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4962 2023-04-16 13:30:48.000000 tremolo-0.0.83/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13754 2023-04-12 13:07:35.000000 tremolo-0.0.83/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-16 13:38:25.000000 tremolo-0.0.83/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 00:28:38.000000 tremolo-0.0.85/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.85/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-17 00:28:38.000000 tremolo-0.0.85/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-17 00:21:36.000000 tremolo-0.0.85/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11623 2023-04-16 23:50:01.000000 tremolo-0.0.85/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/connection_pool.py
+-rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13717 2023-04-12 23:43:31.000000 tremolo-0.0.85/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     8775 2023-04-16 23:20:22.000000 tremolo-0.0.85/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-14 02:53:02.000000 tremolo-0.0.85/tremolo/lib/http_response.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo/lib/parsed/
+-rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/parsed/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-04-16 22:37:48.000000 tremolo-0.0.85/tremolo/lib/parsed/parse.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13668 2023-04-16 23:28:28.000000 tremolo-0.0.85/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.83/PKG-INFO` & `tremolo-0.0.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.83
+Version: 0.0.85
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

### Comparing `tremolo-0.0.83/README.md` & `tremolo-0.0.85/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.83/setup.py` & `tremolo-0.0.85/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.83',
+    version='0.0.85',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.83/tremolo/http_server.py` & `tremolo-0.0.85/tremolo/http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,63 +256,58 @@
         for middleware in self._middlewares['request']:
             options = await self._handle_middleware(middleware[0], {**middleware[1], **options})
 
             if not isinstance(options, dict):
                 return
 
         if request.is_valid:
-            qs_pos = request.path.find(b'?')
+            if request.query_string != b'':
+                self._server['request'].query = parse_qs(request.query_string.decode(encoding='latin-1'))
 
-            if qs_pos > -1:
-                path = request.path[:qs_pos]
-                self._server['request'].query = parse_qs(request.path[qs_pos + 1:].decode(encoding='latin-1'))
-            else:
-                path = request.path
-
-            p = path.strip(b'/')
+            p = request.path.strip(b'/')
 
             if p == b'':
                 ri = 1
             else:
                 ri = b'%d#%s' % (p.count(b'/') + 2, p[:(p + b'/').find(b'/')])
 
             if ri in self._route_handlers:
                 for (pattern, func, kwargs) in self._route_handlers[ri]:
-                    m = pattern.search(request.path)
+                    m = pattern.search(request.url)
 
                     if m:
                         await self._handle_continue()
 
                         matches = m.groupdict()
 
                         if not matches:
                             matches = m.groups()
 
-                        self._server['request'].params['url'] = matches
+                        self._server['request'].params['path'] = matches
 
                         await self._handle_response(func, {**kwargs, **options})
                         return
             else:
                 for i, (pattern, func, kwargs) in enumerate(self._route_handlers[-1]):
-                    m = pattern.search(request.path)
+                    m = pattern.search(request.url)
 
                     if m:
                         if ri in self._route_handlers:
                             self._route_handlers[ri].append((pattern, func, kwargs))
                         else:
                             self._route_handlers[ri] = [(pattern, func, kwargs)]
 
                         await self._handle_continue()
 
                         matches = m.groupdict()
 
                         if not matches:
                             matches = m.groups()
 
-                        self._server['request'].params['url'] = matches
+                        self._server['request'].params['path'] = matches
 
                         await self._handle_response(func, {**kwargs, **options})
                         del self._route_handlers[-1][i]
                         return
 
             # not found
             await self._handle_response(self._route_handlers[0][1][1], {**self._route_handlers[0][1][2], **options})
```

### Comparing `tremolo-0.0.83/tremolo/lib/connection_pool.py` & `tremolo-0.0.85/tremolo/lib/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.83/tremolo/lib/http_exception.py` & `tremolo-0.0.85/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.83/tremolo/lib/http_protocol.py` & `tremolo-0.0.85/tremolo/lib/http_protocol.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.83/tremolo/lib/http_request.py` & `tremolo-0.0.85/tremolo/lib/http_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,24 @@
         self.headers = protocol.header.headers
         self.host = protocol.header.gethost()
 
         if isinstance(self.host, list):
             self.host = self.host[0]
 
         self.method = protocol.header.getmethod().upper()
-        self.path = protocol.header.getpath()
+        self.url = protocol.header.geturl()
+        path_size = self.url.find(b'?')
+
+        if path_size == -1:
+            self.path = self.url
+            self.query_string = b''
+        else:
+            self.path = self.url[:path_size]
+            self.query_string = self.url[path_size + 1:]
+
         self.version = protocol.header.getversion()
 
         if self.version != b'1.0':
             self.version = b'1.1'
 
         self._content_length = -1
         self._content_type = b'application/octet-stream'
```

### Comparing `tremolo-0.0.83/tremolo/lib/http_response.py` & `tremolo-0.0.85/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.83/tremolo/lib/parsed/parse.py` & `tremolo-0.0.85/tremolo/lib/parsed/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,26 +85,26 @@
                         self.headers[b'_status'] = int(_status)
                         self.is_valid_response = True
                     except ValueError:
                         self.headers[b'_version'] = b''
                         self.headers[b'_status'] = 0
                         self.headers[b'_message'] = b''
                 else:
-                    path_end_pos = line.find(b' HTTP/')
+                    url_end_pos = line.find(b' HTTP/')
 
-                    if path_end_pos > 0:
+                    if url_end_pos > 0:
                         self.is_request = True
 
                         try:
-                            self.headers[b'_method'], self.headers[b'_path'] = line[:path_end_pos].split(b' ', 1)
-                            self.headers[b'_version'] = line[path_end_pos + len(' HTTP/'):]
+                            self.headers[b'_method'], self.headers[b'_url'] = line[:url_end_pos].split(b' ', 1)
+                            self.headers[b'_version'] = line[url_end_pos + len(' HTTP/'):]
                             self.is_valid_request = True
                         except ValueError:
                             self.headers[b'_method'] = b''
-                            self.headers[b'_path'] = b''
+                            self.headers[b'_url'] = b''
                             self.headers[b'_version'] = b''
 
                 self.headers[b'_line'] = line
             else:
                 self.is_valid_request = False
                 self.is_valid_response = False
 
@@ -140,16 +140,16 @@
 
     def gethost(self):
         return self.headers.get(b'x-forwarded-host', self.headers.get(b'host'))
 
     def getmethod(self):
         return self.headers.get(b'_method')
 
-    def getpath(self):
-        return self.headers.get(b'_path')
+    def geturl(self):
+        return self.headers.get(b'_url')
 
     def getversion(self):
         return self.headers.get(b'_version')
 
     def getstatus(self):
         return self.headers.get(b'_status')
```

### Comparing `tremolo-0.0.83/tremolo/lib/request.py` & `tremolo-0.0.85/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.83/tremolo/lib/response.py` & `tremolo-0.0.85/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.83/tremolo/tremolo.py` & `tremolo-0.0.85/tremolo/tremolo.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,20 +128,15 @@
         return options
 
     def _add_handler(self, path='/', func=None, kwargs={}):
         if path.startswith('^') or path.endswith('$'):
             pattern = path.encode(encoding='latin-1')
             self._route_handlers[-1].append((pattern, func, kwargs))
         else:
-            qs_pos = path.find('?')
-
-            if qs_pos > -1:
-                path = path[:qs_pos]
-
-            p = path.strip('/')
+            p = path.split('?', 1)[0].strip('/')
 
             if p == '':
                 ri = 1
                 pattern = self._route_handlers[1][0][0]
                 self._route_handlers[ri] = [(pattern, func, kwargs)]
             else:
                 ri = '{:d}#{:s}'.format(p.count('/') + 2, p[:(p + '/').find('/')]).encode(encoding='latin-1')
```

### Comparing `tremolo-0.0.83/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.85/tremolo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.83
+Version: 0.0.85
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

