# Comparing `tmp/flask-fd-1.0.4.tar.gz` & `tmp/flask-fd-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-fd-1.0.4.tar", last modified: Mon Apr 17 13:36:22 2023, max compression
+gzip compressed data, was "flask-fd-1.0.5.tar", last modified: Mon Apr 17 13:44:00 2023, max compression
```

## Comparing `flask-fd-1.0.4.tar` & `flask-fd-1.0.5.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.510041 flask-fd-1.0.4/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1069 2022-09-26 03:49:00.000000 flask-fd-1.0.4/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 13:36:22.510041 flask-fd-1.0.4/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-17 13:33:33.000000 flask-fd-1.0.4/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.498041 flask-fd-1.0.4/flask_fd/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       23 2023-04-17 13:33:33.000000 flask-fd-1.0.4/flask_fd/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/__main__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      738 2023-04-16 19:57:37.000000 flask-fd-1.0.4/flask_fd/cmd.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/gui/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/builder.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/containers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/header_bar.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/indicators.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/menus.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/web.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/helpers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/launchers/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/launchers/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/launchers/launchers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/plop/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/plop/flask/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_1.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_2.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_3.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/plop/flask/starter/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-12 04:06:05.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/FlaskFdIcon
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2197 2023-04-12 04:06:05.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flask_for_desktop.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.510041 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-12 03:07:25.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      106 2023-04-12 03:08:22.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/main.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      282 2023-04-12 03:22:54.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/shell_context.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1226 2023-04-16 19:57:37.000000 flask-fd-1.0.4/flask_fd/plop/ploppers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.502041 flask-fd-1.0.4/flask_fd.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      966 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/entry_points.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-17 13:36:22.510041 flask-fd-1.0.4/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1831 2023-04-17 13:35:53.000000 flask-fd-1.0.4/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.494384 flask-fd-1.0.5/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1069 2022-09-26 03:49:00.000000 flask-fd-1.0.5/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 13:44:00.494384 flask-fd-1.0.5/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-17 13:33:33.000000 flask-fd-1.0.5/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.470383 flask-fd-1.0.5/flask_fd/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       23 2023-04-17 13:43:19.000000 flask-fd-1.0.5/flask_fd/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/__main__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      738 2023-04-16 19:57:37.000000 flask-fd-1.0.5/flask_fd/cmd.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.482384 flask-fd-1.0.5/flask_fd/gui/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/builder.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/containers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/header_bar.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/helpers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/indicators.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/menus.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/gui/web.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/helpers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.486384 flask-fd-1.0.5/flask_fd/launchers/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/launchers/__init__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/launchers/launchers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.486384 flask-fd-1.0.5/flask_fd/plop/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/plop/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.486384 flask-fd-1.0.5/flask_fd/plop/flask/
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/plop/flask/main_flask_fd_1.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/plop/flask/main_flask_fd_2.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-09-26 03:49:00.000000 flask-fd-1.0.5/flask_fd/plop/flask/main_flask_fd_3.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.490384 flask-fd-1.0.5/flask_fd/plop/flask/starter/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-12 04:06:05.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/FlaskFdIcon
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2197 2023-04-12 04:06:05.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flask_for_desktop.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.490384 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-12 03:07:25.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.494384 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      367 2023-04-12 03:09:36.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      333 2022-11-15 17:20:16.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      307 2023-04-12 03:10:18.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/models.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.466383 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/static/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.494384 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/static/img/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-11 23:49:22.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/static/img/FlaskFdIcon
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      256 2023-04-12 03:09:53.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/app/views.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      106 2023-04-12 03:08:22.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/main.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      282 2023-04-12 03:22:54.000000 flask-fd-1.0.5/flask_fd/plop/flask/starter/flaskapp/shell_context.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1226 2023-04-16 19:57:37.000000 flask-fd-1.0.5/flask_fd/plop/ploppers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:44:00.474383 flask-fd-1.0.5/flask_fd.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 13:44:00.000000 flask-fd-1.0.5/flask_fd.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1235 2023-04-17 13:44:00.000000 flask-fd-1.0.5/flask_fd.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-17 13:44:00.000000 flask-fd-1.0.5/flask_fd.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:44:00.000000 flask-fd-1.0.5/flask_fd.egg-info/entry_points.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:44:00.000000 flask-fd-1.0.5/flask_fd.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2023-04-17 13:44:00.000000 flask-fd-1.0.5/flask_fd.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-17 13:44:00.494384 flask-fd-1.0.5/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2192 2023-04-17 13:43:19.000000 flask-fd-1.0.5/setup.py
```

### Comparing `flask-fd-1.0.4/LICENSE.md` & `flask-fd-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/PKG-INFO` & `flask-fd-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fd
-Version: 1.0.4
+Version: 1.0.5
 Summary: Use flask to create desktop applications
 Home-page: https://github.com/byoso/flask_for_desktop
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: flask desktop gui
 Platform: UNKNOWN
```

### Comparing `flask-fd-1.0.4/README.md` & `flask-fd-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/__main__.py` & `flask-fd-1.0.5/flask_fd/__main__.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/cmd.py` & `flask-fd-1.0.5/flask_fd/cmd.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/gui/builder.py` & `flask-fd-1.0.5/flask_fd/gui/builder.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/gui/containers.py` & `flask-fd-1.0.5/flask_fd/gui/containers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/gui/indicators.py` & `flask-fd-1.0.5/flask_fd/gui/indicators.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/gui/menus.py` & `flask-fd-1.0.5/flask_fd/gui/menus.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/launchers/launchers.py` & `flask-fd-1.0.5/flask_fd/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_1.py` & `flask-fd-1.0.5/flask_fd/plop/flask/main_flask_fd_1.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_2.py` & `flask-fd-1.0.5/flask_fd/plop/flask/main_flask_fd_2.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_3.py` & `flask-fd-1.0.5/flask_fd/plop/flask/main_flask_fd_3.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/plop/flask/starter/FlaskFdIcon` & `flask-fd-1.0.5/flask_fd/plop/flask/starter/FlaskFdIcon`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/plop/flask/starter/flask_for_desktop.py` & `flask-fd-1.0.5/flask_fd/plop/flask/starter/flask_for_desktop.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd/plop/ploppers.py` & `flask-fd-1.0.5/flask_fd/plop/ploppers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.4/flask_fd.egg-info/PKG-INFO` & `flask-fd-1.0.5/flask_fd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fd
-Version: 1.0.4
+Version: 1.0.5
 Summary: Use flask to create desktop applications
 Home-page: https://github.com/byoso/flask_for_desktop
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: flask desktop gui
 Platform: UNKNOWN
```

### Comparing `flask-fd-1.0.4/flask_fd.egg-info/SOURCES.txt` & `flask-fd-1.0.5/flask_fd.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,13 @@
 flask_fd/plop/flask/main_flask_fd_1.py
 flask_fd/plop/flask/main_flask_fd_2.py
 flask_fd/plop/flask/main_flask_fd_3.py
 flask_fd/plop/flask/starter/FlaskFdIcon
 flask_fd/plop/flask/starter/flask_for_desktop.py
 flask_fd/plop/flask/starter/flaskapp/__init__.py
 flask_fd/plop/flask/starter/flaskapp/main.py
-flask_fd/plop/flask/starter/flaskapp/shell_context.py
+flask_fd/plop/flask/starter/flaskapp/shell_context.py
+flask_fd/plop/flask/starter/flaskapp/app/__init__.py
+flask_fd/plop/flask/starter/flaskapp/app/config.py
+flask_fd/plop/flask/starter/flaskapp/app/models.py
+flask_fd/plop/flask/starter/flaskapp/app/views.py
+flask_fd/plop/flask/starter/flaskapp/app/static/img/FlaskFdIcon
```

