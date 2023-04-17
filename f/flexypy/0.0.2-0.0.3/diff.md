# Comparing `tmp/flexypy-0.0.2.tar.gz` & `tmp/flexypy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexypy-0.0.2.tar", last modified: Mon Apr 17 08:36:21 2023, max compression
+gzip compressed data, was "flexypy-0.0.3.tar", last modified: Mon Apr 17 10:42:08 2023, max compression
```

## Comparing `flexypy-0.0.2.tar` & `flexypy-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.848876 flexypy-0.0.2/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 08:36:21.848876 flexypy-0.0.2/PKG-INFO
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.840876 flexypy-0.0.2/flexypy/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.2/flexypy/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.2/flexypy/cli.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/exceptions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.2/flexypy/exceptions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.2/flexypy/exceptions/baseexceptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.2/flexypy/exceptions/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.2/flexypy/exceptions/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/exceptions/web/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.2/flexypy/exceptions/web/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.2/flexypy/exceptions/web/baseexseptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.2/flexypy/exceptions/web/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/generate_templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.2/flexypy/generate_templates/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.2/flexypy/generate_templates/generator.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/generate_templates/templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.2/flexypy/generate_templates/templates/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/generate_templates/templates/config/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.2/flexypy/generate_templates/templates/config/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       24 2023-04-15 14:55:12.000000 flexypy-0.0.2/flexypy/generate_templates/templates/config/apps.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.2/flexypy/generate_templates/templates/config/dirs.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      254 2023-04-17 08:31:23.000000 flexypy-0.0.2/flexypy/generate_templates/templates/main.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/http/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.2/flexypy/http/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1168 2023-04-14 14:37:12.000000 flexypy-0.0.2/flexypy/http/request.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2634 2023-04-15 08:50:25.000000 flexypy-0.0.2/flexypy/http/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     8359 2023-04-16 08:44:00.000000 flexypy-0.0.2/flexypy/http/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy/http/template/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.2/flexypy/http/template/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.848876 flexypy-0.0.2/flexypy/http/template/extensions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.2/flexypy/http/template/extensions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.2/flexypy/http/template/extensions/base_extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      431 2023-04-16 08:43:50.000000 flexypy-0.0.2/flexypy/http/template/extensions/template_ext.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     3248 2023-04-16 08:44:00.000000 flexypy-0.0.2/flexypy/http/template/render.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.848876 flexypy-0.0.2/flexypy/middlewares/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.2/flexypy/middlewares/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.2/flexypy/middlewares/mddl.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 08:36:21.844876 flexypy-0.0.2/flexypy.egg-info/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/PKG-INFO
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1139 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/SOURCES.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/dependency_links.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       21 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/requires.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-17 08:36:21.000000 flexypy-0.0.2/flexypy.egg-info/top_level.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      385 2023-04-17 08:36:14.000000 flexypy-0.0.2/pyproject.toml
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-17 08:36:21.848876 flexypy-0.0.2/setup.cfg
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 10:42:08.284719 flexypy-0.0.3/PKG-INFO
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.280719 flexypy-0.0.3/flexypy/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.0.3/flexypy/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.0.3/flexypy/cli.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/exceptions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.0.3/flexypy/exceptions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.0.3/flexypy/exceptions/baseexceptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.0.3/flexypy/exceptions/extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.0.3/flexypy/exceptions/render.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.0.3/flexypy/exceptions/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.0.3/flexypy/exceptions/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/exceptions/web/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.0.3/flexypy/exceptions/web/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.0.3/flexypy/exceptions/web/baseexseptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.0.3/flexypy/exceptions/web/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/generate_templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.0.3/flexypy/generate_templates/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1036 2023-04-16 08:47:03.000000 flexypy-0.0.3/flexypy/generate_templates/generator.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/generate_templates/templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.0.3/flexypy/generate_templates/templates/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/generate_templates/templates/config/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.0.3/flexypy/generate_templates/templates/config/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       24 2023-04-15 14:55:12.000000 flexypy-0.0.3/flexypy/generate_templates/templates/config/apps.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.0.3/flexypy/generate_templates/templates/config/dirs.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      254 2023-04-17 08:31:23.000000 flexypy-0.0.3/flexypy/generate_templates/templates/main.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/http/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.0.3/flexypy/http/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1168 2023-04-14 14:37:12.000000 flexypy-0.0.3/flexypy/http/request.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2635 2023-04-17 09:53:46.000000 flexypy-0.0.3/flexypy/http/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     8822 2023-04-17 10:35:15.000000 flexypy-0.0.3/flexypy/http/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/http/template/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.0.3/flexypy/http/template/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/http/template/extensions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.0.3/flexypy/http/template/extensions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      763 2023-04-14 16:19:59.000000 flexypy-0.0.3/flexypy/http/template/extensions/base_extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.0.3/flexypy/http/template/extensions/template_ext.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.0.3/flexypy/http/template/render.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.284719 flexypy-0.0.3/flexypy/middlewares/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.0.3/flexypy/middlewares/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.0.3/flexypy/middlewares/mddl.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-04-17 10:42:08.280719 flexypy-0.0.3/flexypy.egg-info/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-04-17 10:42:08.000000 flexypy-0.0.3/flexypy.egg-info/PKG-INFO
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1200 2023-04-17 10:42:08.000000 flexypy-0.0.3/flexypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-04-17 10:42:08.000000 flexypy-0.0.3/flexypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       21 2023-04-17 10:42:08.000000 flexypy-0.0.3/flexypy.egg-info/requires.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-04-17 10:42:08.000000 flexypy-0.0.3/flexypy.egg-info/top_level.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      385 2023-04-17 10:41:51.000000 flexypy-0.0.3/pyproject.toml
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-04-17 10:42:08.284719 flexypy-0.0.3/setup.cfg
```

### Comparing `flexypy-0.0.2/flexypy/exceptions/web/server.py` & `flexypy-0.0.3/flexypy/exceptions/web/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.2/flexypy/generate_templates/generator.py` & `flexypy-0.0.3/flexypy/generate_templates/generator.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.2/flexypy/http/request.py` & `flexypy-0.0.3/flexypy/http/request.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.2/flexypy/http/routing.py` & `flexypy-0.0.3/flexypy/http/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.parent_route = parent_route
         p = self._modify_path(path)
         self.slug_data = self.parse_slug(p)
         super().__init__(p, template_path)
 
     def _modify_path(self, path) -> str:
         if self.parent_route:
-            return self.parent_route().path.strip('/') + '/' + path.strip('/')
+            return self.parent_route().path.strip('/') + '/' + path.lstrip('/')
         else:
             return path
 
     def post(self):
         pass
```

### Comparing `flexypy-0.0.2/flexypy/http/server.py` & `flexypy-0.0.3/flexypy/http/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from flexypy.http.routing import UserRoute
 from typing import Type
 import os
 from flexypy.exceptions.web.server import PathNotFound
 from urllib import parse
 from cgi import FieldStorage
 from flexypy.middlewares.mddl import Middleware
+import re
 
 
 @dataclass
 class HtmlResponse:
     code: str
     header: list[tuple[str, str]]
     html: bytes
@@ -59,15 +60,14 @@
                     app.request = self.request
 
                     mddl_app, mddl_redirect = self._run_middlewares(app)
                     if mddl_redirect.from_path and mddl_redirect.to_path:
                         if self.full_url == mddl_redirect.from_path:
                             return self.render.render_redirect(mddl_redirect.to_path)
                     return self._method_get(mddl_app)
-
                 if self.router.check_static_file():
                     return self._method_get_static_files(self.router.check_static_file())
 
                 # If path not found
                 if not path_found:
                     t = PathNotFound(self.full_url, [self.server_address + i().get_path() for i in self.routes])
                     return self.render.render_traceback(t.code, t.html)
@@ -81,17 +81,18 @@
                                              keep_blank_values=True)
                     self.request.POST.set_data(form_data)
 
                     # Set app request
                     app.request = self.request
 
                     mddl_app, mddl_redirect = self._run_middlewares(app)
-                    if mddl_redirect.from_path and mddl_redirect.to_path:
-                        if self.full_url == mddl_redirect.from_path:
-                            return self.render.render_redirect(mddl_redirect.to_path)
+                    if mddl_redirect:
+                        if mddl_redirect.from_path and mddl_redirect.to_path:
+                            if self.full_url == mddl_redirect.from_path:
+                                return self.render.render_redirect(mddl_redirect.to_path)
 
                     return self._method_post(app)
 
     def _method_get(self, app: UserRoute) -> HtmlResponse:
         mime_type = mimetypes.guess_type(app.template_path)[0]
         resp = self.render.render_html('200 OK', [('Content-type', mime_type)], app.get())
         return resp
@@ -109,15 +110,25 @@
             elif not current_url:
                 p = filepath
             else:
                 if current_url.rfind('/') != -1:
                     converted_path = current_url[:current_url.rfind('/')+1:]
                 else:
                     converted_path = current_url
-                p = filepath.split(converted_path)[-1].strip('/')
+
+                p = filepath
+
+                if filepath.startswith(converted_path):
+                    p = filepath.split(converted_path)[-1].strip('/')
+
+                    # If names are duplicated in the path. For example test/test/path/to/file
+                    for i in re.finditer(converted_path, filepath):
+                        if os.path.exists(filepath[i.end()::]):
+                            p = filepath[i.end()::]
+                            break
 
             if os.path.exists(p):
                 with open(p, 'rb') as f:
                     mime_type = mimetypes.guess_type(p)[0]
                     resp = self.render.render_html('200 OK', [('Content-type', mime_type)], f.read())
                     return resp
```

### Comparing `flexypy-0.0.2/flexypy/http/template/extensions/base_extension.py` & `flexypy-0.0.3/flexypy/http/template/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.0.2/flexypy/http/template/render.py` & `flexypy-0.0.3/flexypy/http/template/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import jinja2
 from config.dirs import TEMPLATES_PATH, EXTENSIONS_PATH, GLOBAL_TEMPLATE_OBJECTS_PATH, GLOBAL_TEMPLATE_FUNCTIONS_PATH
 import os
 from typing import Callable, Type
 from flexypy.http.template.extensions.base_extension import BaseExtension
 import importlib
+from flexypy.exceptions.render import TemplateNotFound
 
 
 class RenderTemplate:
     def __init__(self, template_path):
         self.template_path = template_path
         self._template_source: str = ''
         self._methods = []
@@ -19,14 +20,15 @@
 
     def render(self, **kwargs) -> str:
         try:
             for templ in TEMPLATES_PATH:
                 filepath = os.path.join(templ, self.template_path)
                 if os.path.exists(filepath):
                     return _JinjaInit(filepath).template_methods(self._methods).jinit(**kwargs)
+            raise TemplateNotFound('render', self.template_path)
         except Exception as e:
             raise e
 
 
 class _JinjaInit:
     def __init__(self, filepath: str):
         self._path = filepath.split('templates')[-1]
```

### Comparing `flexypy-0.0.2/flexypy.egg-info/SOURCES.txt` & `flexypy-0.0.3/flexypy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 flexypy.egg-info/PKG-INFO
 flexypy.egg-info/SOURCES.txt
 flexypy.egg-info/dependency_links.txt
 flexypy.egg-info/requires.txt
 flexypy.egg-info/top_level.txt
 flexypy/exceptions/__init__.py
 flexypy/exceptions/baseexceptions.py
+flexypy/exceptions/extension.py
+flexypy/exceptions/render.py
 flexypy/exceptions/routing.py
 flexypy/exceptions/server.py
 flexypy/exceptions/web/__init__.py
 flexypy/exceptions/web/baseexseptions.py
 flexypy/exceptions/web/server.py
 flexypy/generate_templates/__init__.py
 flexypy/generate_templates/generator.py
```

