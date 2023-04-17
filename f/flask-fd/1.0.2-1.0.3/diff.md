# Comparing `tmp/flask-fd-1.0.2.tar.gz` & `tmp/flask-fd-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-fd-1.0.2.tar", last modified: Fri Aug  5 23:51:58 2022, max compression
+gzip compressed data, was "flask-fd-1.0.3.tar", last modified: Mon Apr 17 13:28:28 2023, max compression
```

## Comparing `flask-fd-1.0.2.tar` & `flask-fd-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1749 2022-08-05 15:37:38.000000 flask-fd-1.0.2/setup.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-08-05 23:35:52.000000 flask-fd-1.0.2/flask_fd/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       63 2022-08-05 23:51:07.000000 flask-fd-1.0.2/flask_fd/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1825 2022-08-05 21:13:00.000000 flask-fd-1.0.2/flask_fd/cmd.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-08-05 15:25:37.000000 flask-fd-1.0.2/flask_fd/__main__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd/launchers/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-08-05 15:25:37.000000 flask-fd-1.0.2/flask_fd/launchers/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-08-05 16:17:42.000000 flask-fd-1.0.2/flask_fd/launchers/launchers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd/gui/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-08-05 15:25:37.000000 flask-fd-1.0.2/flask_fd/gui/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-08-05 21:13:00.000000 flask-fd-1.0.2/flask_fd/gui/header_bar.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-08-05 21:13:00.000000 flask-fd-1.0.2/flask_fd/gui/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-08-05 16:17:42.000000 flask-fd-1.0.2/flask_fd/gui/menus.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-08-05 21:13:00.000000 flask-fd-1.0.2/flask_fd/gui/web.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-08-05 16:17:42.000000 flask-fd-1.0.2/flask_fd/gui/indicators.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-08-05 23:09:03.000000 flask-fd-1.0.2/flask_fd/gui/builder.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-08-05 23:09:03.000000 flask-fd-1.0.2/flask_fd/gui/containers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd/plop/
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd/plop/flask/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-08-05 21:13:00.000000 flask-fd-1.0.2/flask_fd/plop/flask/main_flask_fd_1.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-08-05 23:09:03.000000 flask-fd-1.0.2/flask_fd/plop/flask/main_flask_fd_2.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-08-05 21:13:00.000000 flask-fd-1.0.2/flask_fd/plop/flask/main_flask_fd_3.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd/plop/installer/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     5291 2022-08-05 23:51:07.000000 flask-fd-1.0.2/flask_fd/plop/installer/installer
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-08-05 15:25:37.000000 flask-fd-1.0.2/flask_fd/plop/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd/plop/icon/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-08-05 15:25:37.000000 flask-fd-1.0.2/flask_fd/plop/icon/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2022-08-05 15:25:37.000000 flask-fd-1.0.2/flask_fd/plop/icon/FlaskFdIcon
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1642 2022-08-05 23:31:45.000000 flask-fd-1.0.2/flask_fd/plop/ploppers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2022-08-05 23:51:57.000000 flask-fd-1.0.2/flask_fd.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2022-08-05 23:51:57.000000 flask-fd-1.0.2/flask_fd.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2022-08-05 23:51:57.000000 flask-fd-1.0.2/flask_fd.egg-info/entry_points.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       16 2022-08-05 23:51:57.000000 flask-fd-1.0.2/flask_fd.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      814 2022-08-05 23:51:58.000000 flask-fd-1.0.2/flask_fd.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2316 2022-08-05 23:51:57.000000 flask-fd-1.0.2/flask_fd.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1270 2022-08-05 23:09:03.000000 flask-fd-1.0.2/README.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2022-08-05 23:51:58.000000 flask-fd-1.0.2/setup.cfg
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2316 2022-08-05 23:51:58.000000 flask-fd-1.0.2/PKG-INFO
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1069 2022-09-26 03:49:00.000000 flask-fd-1.0.3/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1908 2023-04-17 13:28:28.351041 flask-fd-1.0.3/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1297 2022-09-26 03:49:00.000000 flask-fd-1.0.3/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.347041 flask-fd-1.0.3/flask_fd/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       23 2023-04-16 19:57:37.000000 flask-fd-1.0.3/flask_fd/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/__main__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      738 2023-04-16 19:57:37.000000 flask-fd-1.0.3/flask_fd/cmd.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/gui/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/builder.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/containers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/header_bar.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/helpers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/indicators.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/menus.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/web.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/helpers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/launchers/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/launchers/__init__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/launchers/launchers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/flask/
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_1.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_2.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_3.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/flask/starter/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-12 04:06:05.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/FlaskFdIcon
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2197 2023-04-12 04:06:05.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flask_for_desktop.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-12 03:07:25.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/__init__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      106 2023-04-12 03:08:22.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/main.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      282 2023-04-12 03:22:54.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/shell_context.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1226 2023-04-16 19:57:37.000000 flask-fd-1.0.3/flask_fd/plop/ploppers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.347041 flask-fd-1.0.3/flask_fd.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1908 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      966 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/entry_points.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-17 13:28:28.351041 flask-fd-1.0.3/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1831 2023-04-16 19:57:37.000000 flask-fd-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flask-fd-1.0.2/setup.py` & `flask-fd-1.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="flask-fd",
     version=f"{__version__}",
     description=(
-        "Use flask to create a desktop GUI"
+        "Use flask to create desktop applications"
         ),
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/byoso/flask_for_desktop",
     author="Vincent Fabre",
     author_email="peigne.plume@gmail.com",
     license="MIT",
@@ -46,22 +46,24 @@
     ],
     packages=[
         "flask_fd",
         "flask_fd.gui",
         "flask_fd.launchers",
         "flask_fd.plop",
         "flask_fd.plop.flask",
-        "flask_fd.plop.installer",
-        "flask_fd.plop.icon",
+        "flask_fd.plop.flask.starter",
+        "flask_fd.plop.flask.starter.flaskapp",
         ],
     # include_package_data=True,
     package_data={'': ['FlaskFdIcon', 'installer']},
     python_requires='>=3.6',
     install_requires=[
         "flamewok >= 1.0.8",
+        "flask-sqlalchemy",
+        "flask-migrate",
     ],
     keywords='flask desktop gui',
     entry_points={
         "console_scripts": [
             "flask-fd=flask_fd.cmd:cmd",
         ]
     },
```

### Comparing `flask-fd-1.0.2/flask_fd/__main__.py` & `flask-fd-1.0.3/flask_fd/__main__.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/launchers/launchers.py` & `flask-fd-1.0.3/flask_fd/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/gui/menus.py` & `flask-fd-1.0.3/flask_fd/gui/menus.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/gui/indicators.py` & `flask-fd-1.0.3/flask_fd/gui/indicators.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/gui/builder.py` & `flask-fd-1.0.3/flask_fd/gui/builder.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/gui/containers.py` & `flask-fd-1.0.3/flask_fd/gui/containers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/plop/flask/main_flask_fd_1.py` & `flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_1.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/plop/flask/main_flask_fd_2.py` & `flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_2.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/plop/flask/main_flask_fd_3.py` & `flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_3.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd/plop/icon/FlaskFdIcon` & `flask-fd-1.0.3/flask_fd/plop/flask/starter/FlaskFdIcon`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.2/flask_fd.egg-info/SOURCES.txt` & `flask-fd-1.0.3/flask_fd.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 README.md
 setup.py
 flask_fd/__init__.py
 flask_fd/__main__.py
 flask_fd/cmd.py
 flask_fd/helpers.py
 flask_fd.egg-info/PKG-INFO
@@ -21,10 +22,12 @@
 flask_fd/launchers/__init__.py
 flask_fd/launchers/launchers.py
 flask_fd/plop/__init__.py
 flask_fd/plop/ploppers.py
 flask_fd/plop/flask/main_flask_fd_1.py
 flask_fd/plop/flask/main_flask_fd_2.py
 flask_fd/plop/flask/main_flask_fd_3.py
-flask_fd/plop/icon/FlaskFdIcon
-flask_fd/plop/icon/__init__.py
-flask_fd/plop/installer/installer
+flask_fd/plop/flask/starter/FlaskFdIcon
+flask_fd/plop/flask/starter/flask_for_desktop.py
+flask_fd/plop/flask/starter/flaskapp/__init__.py
+flask_fd/plop/flask/starter/flaskapp/main.py
+flask_fd/plop/flask/starter/flaskapp/shell_context.py
```

### Comparing `flask-fd-1.0.2/README.md` & `flask-fd-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ![silly-gui-icon](https://i.goopics.net/tou3jl.png)
 
 # Flask for desktop
 
 _Build a desktop application with flask._
-_All you need is to add the provided file, and Silly gui in your dependencies_
+_All you need is to add the provided file, and Flask for desktop in your dependencies_
 
 
 
 ## How it works in a few words
 
-Basicaly, when the app is launched, silly-gui runs the flask server alongside a desktop window and/or the main browser of the user's system.
+Basicaly, when the app is launched, Flask for desktop runs the flask server alongside a desktop window and/or the main browser of the user's system.
 
 The user's experience is similar with an 'electron' application, but there, it is python inside instead of JS.
 
 ## How to do it
 
 ### 1. Code your flask app as usual
 
@@ -26,15 +26,15 @@
 
 ### 3. get a converter file
 For the simpliest version:
 
 ```
 flask-fd plop 1
 ```
-or for a more customizable and fancy interface (the best choice)
+or for a more customizable and fancy interface, very easy (the best choice)
 ```
 flask-fd plop 2
 ```
 or just running the app in the default web browser
 ```
 flask-fd plop 3
 ```
```

