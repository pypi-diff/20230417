# Comparing `tmp/foyou-http-0.0.8.tar.gz` & `tmp/foyou-http-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foyou-http-0.0.8.tar", last modified: Thu Sep  1 12:21:17 2022, max compression
+gzip compressed data, was "foyou-http-0.0.9.tar", last modified: Thu Sep  1 12:35:47 2022, max compression
```

## Comparing `foyou-http-0.0.8.tar` & `foyou-http-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:21:17.008118 foyou-http-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-01 12:21:11.000000 foyou-http-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-01 12:21:11.000000 foyou-http-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-09-01 12:21:17.008118 foyou-http-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-09-01 12:21:11.000000 foyou-http-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-01 12:21:11.000000 foyou-http-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-01 12:21:17.008118 foyou-http-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:21:17.008118 foyou-http-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:21:17.008118 foyou-http-0.0.8/src/foyou_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-09-01 12:21:16.000000 foyou-http-0.0.8/src/foyou_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-01 12:21:16.000000 foyou-http-0.0.8/src/foyou_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 12:21:16.000000 foyou-http-0.0.8/src/foyou_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-01 12:21:16.000000 foyou-http-0.0.8/src/foyou_http.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-01 12:21:16.000000 foyou-http-0.0.8/src/foyou_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-01 12:21:16.000000 foyou-http-0.0.8/src/foyou_http.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:21:17.008118 foyou-http-0.0.8/src/simplehttp/
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-09-01 12:21:15.000000 foyou-http-0.0.8/src/simplehttp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:21:17.008118 foyou-http-0.0.8/src/simplehttp/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-01 12:21:11.000000 foyou-http-0.0.8/src/simplehttp/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-01 12:21:11.000000 foyou-http-0.0.8/src/simplehttp/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:35:47.924234 foyou-http-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-01 12:35:43.000000 foyou-http-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-01 12:35:43.000000 foyou-http-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-09-01 12:35:47.924234 foyou-http-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-09-01 12:35:43.000000 foyou-http-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-01 12:35:43.000000 foyou-http-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-01 12:35:47.924234 foyou-http-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:35:47.924234 foyou-http-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:35:47.924234 foyou-http-0.0.9/src/foyou_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-09-01 12:35:47.000000 foyou-http-0.0.9/src/foyou_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-01 12:35:47.000000 foyou-http-0.0.9/src/foyou_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 12:35:47.000000 foyou-http-0.0.9/src/foyou_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-01 12:35:47.000000 foyou-http-0.0.9/src/foyou_http.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-01 12:35:47.000000 foyou-http-0.0.9/src/foyou_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-01 12:35:47.000000 foyou-http-0.0.9/src/foyou_http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:35:47.924234 foyou-http-0.0.9/src/simplehttp/
+-rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-09-01 12:35:47.000000 foyou-http-0.0.9/src/simplehttp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:35:47.924234 foyou-http-0.0.9/src/simplehttp/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-01 12:35:43.000000 foyou-http-0.0.9/src/simplehttp/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-01 12:35:43.000000 foyou-http-0.0.9/src/simplehttp/templates/index.html
```

### Comparing `foyou-http-0.0.8/LICENSE` & `foyou-http-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `foyou-http-0.0.8/PKG-INFO` & `foyou-http-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foyou-http
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple http server for share files.
 Home-page: https://github.com/foyoux/foyou-http
 Author: foyou
 Author-email: yimi.0822@qq.com
 License: GPL-3.0
 Project-URL: Source, https://github.com/foyoux/foyou-http
 Project-URL: Bug Tracker, https://github.com/foyoux/foyou-http/issues
```

### Comparing `foyou-http-0.0.8/README.md` & `foyou-http-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `foyou-http-0.0.8/setup.cfg` & `foyou-http-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `foyou-http-0.0.8/src/foyou_http.egg-info/PKG-INFO` & `foyou-http-0.0.9/src/foyou_http.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foyou-http
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple http server for share files.
 Home-page: https://github.com/foyoux/foyou-http
 Author: foyou
 Author-email: yimi.0822@qq.com
 License: GPL-3.0
 Project-URL: Source, https://github.com/foyoux/foyou-http
 Project-URL: Bug Tracker, https://github.com/foyoux/foyou-http/issues
```

### Comparing `foyou-http-0.0.8/src/simplehttp/__init__.py` & `foyou-http-0.0.9/src/simplehttp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
+import os
+from datetime import datetime
 
-def start_server(host, port, dir_):
-    import os
-    from datetime import datetime
+from flask import Flask, render_template, request
+from werkzeug.security import safe_join
 
-    from flask import Flask, render_template, request
-    from werkzeug.security import safe_join
+app = Flask(__name__, static_url_path='/')
+
+
+def index(e):
+    path = safe_join(app.static_folder, request.path.strip('/'))
+    if not os.path.exists(path):
+        return render_template('404.html'), 400
+    body = []
+    f: os.DirEntry
+    for f in os.scandir(path):
+        if f.name.startswith('.'):
+            continue
+        f_stat = f.stat()
+        body.append({
+            'path': f.name + ('/' if f.is_dir() else ''),
+            'time': datetime.strftime(datetime.fromtimestamp(f_stat.st_mtime), '%Y-%m-%d %H:%M:%S'),
+            'size': f_stat.st_size if f.is_file() else '-'
+        })
+    body.sort(key=lambda x: x['path'])
+    body.sort(key=lambda x: not x['path'].endswith('/'))
+    return render_template('index.html', title=request.path, body=body)
 
-    app = Flask(__name__, static_url_path='/')
-    app._static_folder = os.path.abspath(dir_)
 
-    def index(e):
-        path = safe_join(app.static_folder, request.path.strip('/'))
-        if not os.path.exists(path):
-            return render_template('404.html'), 400
-        body = []
-        f: os.DirEntry
-        for f in os.scandir(path):
-            if f.name.startswith('.'):
-                continue
-            f_stat = f.stat()
-            body.append({
-                'path': f.name + ('/' if f.is_dir() else ''),
-                'time': datetime.strftime(datetime.fromtimestamp(f_stat.st_mtime), '%Y-%m-%d %H:%M:%S'),
-                'size': f_stat.st_size if f.is_file() else '-'
-            })
-        body.sort(key=lambda x: x['path'])
-        body.sort(key=lambda x: not x['path'].endswith('/'))
-        return render_template('index.html', title=request.path, body=body)
+app.register_error_handler(404, index)
 
-    app.register_error_handler(404, index)
 
+def start_server(host, port, dir_):
+    app._static_folder = os.path.abspath(dir_)
     app.run(host=host, port=port)
 
 
 def main():
     import argparse
     parser = argparse.ArgumentParser(
         description='simple http server for share files.',
```

