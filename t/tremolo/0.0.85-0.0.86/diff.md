# Comparing `tmp/tremolo-0.0.85.tar.gz` & `tmp/tremolo-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.85.tar", last modified: Mon Apr 17 00:28:38 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.86.tar", last modified: Mon Apr 17 02:09:06 2023, max compression
```

## Comparing `tremolo-0.0.85.tar` & `tremolo-0.0.86.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 00:28:38.000000 tremolo-0.0.85/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.85/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-17 00:28:38.000000 tremolo-0.0.85/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-17 00:21:36.000000 tremolo-0.0.85/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11623 2023-04-16 23:50:01.000000 tremolo-0.0.85/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13717 2023-04-12 23:43:31.000000 tremolo-0.0.85/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     8775 2023-04-16 23:20:22.000000 tremolo-0.0.85/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-14 02:53:02.000000 tremolo-0.0.85/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-04-16 22:37:48.000000 tremolo-0.0.85/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.85/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13668 2023-04-16 23:28:28.000000 tremolo-0.0.85/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-17 00:28:38.000000 tremolo-0.0.85/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 02:09:06.000000 tremolo-0.0.86/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.86/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-17 02:09:06.000000 tremolo-0.0.86/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-17 02:04:05.000000 tremolo-0.0.86/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11623 2023-04-16 23:50:01.000000 tremolo-0.0.86/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/connection_pool.py
+-rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13753 2023-04-17 02:02:16.000000 tremolo-0.0.86/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     8775 2023-04-16 23:20:22.000000 tremolo-0.0.86/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-14 02:53:02.000000 tremolo-0.0.86/tremolo/lib/http_response.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo/lib/parsed/
+-rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/parsed/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-04-16 22:37:48.000000 tremolo-0.0.86/tremolo/lib/parsed/parse.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13668 2023-04-16 23:28:28.000000 tremolo-0.0.86/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.85/PKG-INFO` & `tremolo-0.0.86/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.85
+Version: 0.0.86
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

### Comparing `tremolo-0.0.85/README.md` & `tremolo-0.0.86/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/setup.py` & `tremolo-0.0.86/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.85',
+    version='0.0.86',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.85/tremolo/http_server.py` & `tremolo-0.0.86/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/lib/connection_pool.py` & `tremolo-0.0.86/tremolo/lib/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/lib/http_exception.py` & `tremolo-0.0.86/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/lib/http_protocol.py` & `tremolo-0.0.86/tremolo/lib/http_protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
             self.put_to_queue(data, queue=self._queue[0], transport=self._transport, rate=self._options['upload_rate'])
         )
 
     def eof_received(self):
         self._queue[0].put_nowait(None)
 
     def resume_writing(self):
-        if not self._timeout_waiters['send'].done():
+        if 'send' in self._timeout_waiters and not self._timeout_waiters['send'].done():
             self._timeout_waiters['send'].set_result(None)
 
     def set_watermarks(self, high=65536, low=8192):
         if self._transport is not None:
             self._watermarks['high'] = high
             self._watermarks['low'] = low
```

### Comparing `tremolo-0.0.85/tremolo/lib/http_request.py` & `tremolo-0.0.86/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/lib/http_response.py` & `tremolo-0.0.86/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/lib/parsed/parse.py` & `tremolo-0.0.86/tremolo/lib/parsed/parse.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/lib/request.py` & `tremolo-0.0.86/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/lib/response.py` & `tremolo-0.0.86/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo/tremolo.py` & `tremolo-0.0.86/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.85/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.86/tremolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.85
+Version: 0.0.86
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
```

