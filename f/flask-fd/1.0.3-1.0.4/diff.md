# Comparing `tmp/flask-fd-1.0.3.tar.gz` & `tmp/flask-fd-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-fd-1.0.3.tar", last modified: Mon Apr 17 13:28:28 2023, max compression
+gzip compressed data, was "flask-fd-1.0.4.tar", last modified: Mon Apr 17 13:36:22 2023, max compression
```

## Comparing `flask-fd-1.0.3.tar` & `flask-fd-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1069 2022-09-26 03:49:00.000000 flask-fd-1.0.3/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1908 2023-04-17 13:28:28.351041 flask-fd-1.0.3/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1297 2022-09-26 03:49:00.000000 flask-fd-1.0.3/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.347041 flask-fd-1.0.3/flask_fd/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       23 2023-04-16 19:57:37.000000 flask-fd-1.0.3/flask_fd/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/__main__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      738 2023-04-16 19:57:37.000000 flask-fd-1.0.3/flask_fd/cmd.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/gui/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/builder.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/containers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/header_bar.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/indicators.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/menus.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/gui/web.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/helpers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/launchers/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/launchers/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/launchers/launchers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/flask/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_1.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_2.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-09-26 03:49:00.000000 flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_3.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/flask/starter/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-12 04:06:05.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/FlaskFdIcon
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2197 2023-04-12 04:06:05.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flask_for_desktop.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.351041 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-12 03:07:25.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      106 2023-04-12 03:08:22.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/main.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      282 2023-04-12 03:22:54.000000 flask-fd-1.0.3/flask_fd/plop/flask/starter/flaskapp/shell_context.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1226 2023-04-16 19:57:37.000000 flask-fd-1.0.3/flask_fd/plop/ploppers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:28:28.347041 flask-fd-1.0.3/flask_fd.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1908 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      966 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/entry_points.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2023-04-17 13:28:28.000000 flask-fd-1.0.3/flask_fd.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-17 13:28:28.351041 flask-fd-1.0.3/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1831 2023-04-16 19:57:37.000000 flask-fd-1.0.3/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.510041 flask-fd-1.0.4/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1069 2022-09-26 03:49:00.000000 flask-fd-1.0.4/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 13:36:22.510041 flask-fd-1.0.4/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-17 13:33:33.000000 flask-fd-1.0.4/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.498041 flask-fd-1.0.4/flask_fd/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       23 2023-04-17 13:33:33.000000 flask-fd-1.0.4/flask_fd/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/__main__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      738 2023-04-16 19:57:37.000000 flask-fd-1.0.4/flask_fd/cmd.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/gui/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/builder.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/containers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/header_bar.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/helpers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/indicators.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/menus.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/gui/web.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/helpers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/launchers/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/launchers/__init__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/launchers/launchers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/plop/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/plop/flask/
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_1.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_2.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-09-26 03:49:00.000000 flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_3.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.506041 flask-fd-1.0.4/flask_fd/plop/flask/starter/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-12 04:06:05.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/FlaskFdIcon
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2197 2023-04-12 04:06:05.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flask_for_desktop.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.510041 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-12 03:07:25.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/__init__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      106 2023-04-12 03:08:22.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/main.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      282 2023-04-12 03:22:54.000000 flask-fd-1.0.4/flask_fd/plop/flask/starter/flaskapp/shell_context.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1226 2023-04-16 19:57:37.000000 flask-fd-1.0.4/flask_fd/plop/ploppers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:36:22.502041 flask-fd-1.0.4/flask_fd.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      966 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/entry_points.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2023-04-17 13:36:22.000000 flask-fd-1.0.4/flask_fd.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-17 13:36:22.510041 flask-fd-1.0.4/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1831 2023-04-17 13:35:53.000000 flask-fd-1.0.4/setup.py
```

### Comparing `flask-fd-1.0.3/LICENSE.md` & `flask-fd-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/PKG-INFO` & `flask-fd-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Use flask to create desktop applications
 Home-page: https://github.com/byoso/flask_for_desktop
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: flask desktop gui
 Platform: UNKNOWN
@@ -39,40 +39,25 @@
 
 ### 2. Installation
 
 ```
 pip install flask-fd
 ```
 
-### 3. get a converter file
-For the simpliest version:
+### 3. get the files
+If you start your app from scratch:
 
+```sh
+flask-fd plop starter
 ```
-flask-fd plop 1
-```
-or for a more customizable and fancy interface, very easy (the best choice)
-```
-flask-fd plop 2
-```
-or just running the app in the default web browser
-```
-flask-fd plop 3
+If you've already done your app and just want to convert it:
+
+```sh
+flask-fd plop converter
 ```
+This one will give you a file that you'll just have to configure following
+the steps in the comments.
 
 The file appear in your current working directory.
 Fill the parameters in the given file.
 
-### 4. launch the app
-
-Execute the provided file, you'll see you flask app wrapped in a pretty
-Gtk interface
-
-### 5. get an installer (for linux)
-This if you want to integrate your app in the system.
-The installer uses [Geninstaller](https://github.com/byoso/geninstaller)
-
-```
-flask-fd plop installer
-```
-Fill the parameters in the installer.
-
```

### Comparing `flask-fd-1.0.3/README.md` & `flask-fd-1.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -20,38 +20,23 @@
 
 ### 2. Installation
 
 ```
 pip install flask-fd
 ```
 
-### 3. get a converter file
-For the simpliest version:
+### 3. get the files
+If you start your app from scratch:
 
+```sh
+flask-fd plop starter
 ```
-flask-fd plop 1
-```
-or for a more customizable and fancy interface, very easy (the best choice)
-```
-flask-fd plop 2
-```
-or just running the app in the default web browser
-```
-flask-fd plop 3
+If you've already done your app and just want to convert it:
+
+```sh
+flask-fd plop converter
 ```
+This one will give you a file that you'll just have to configure following
+the steps in the comments.
 
 The file appear in your current working directory.
 Fill the parameters in the given file.
-
-### 4. launch the app
-
-Execute the provided file, you'll see you flask app wrapped in a pretty
-Gtk interface
-
-### 5. get an installer (for linux)
-This if you want to integrate your app in the system.
-The installer uses [Geninstaller](https://github.com/byoso/geninstaller)
-
-```
-flask-fd plop installer
-```
-Fill the parameters in the installer.
```

### Comparing `flask-fd-1.0.3/flask_fd/__main__.py` & `flask-fd-1.0.4/flask_fd/__main__.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/cmd.py` & `flask-fd-1.0.4/flask_fd/cmd.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/gui/builder.py` & `flask-fd-1.0.4/flask_fd/gui/builder.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/gui/containers.py` & `flask-fd-1.0.4/flask_fd/gui/containers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/gui/indicators.py` & `flask-fd-1.0.4/flask_fd/gui/indicators.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/gui/menus.py` & `flask-fd-1.0.4/flask_fd/gui/menus.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/launchers/launchers.py` & `flask-fd-1.0.4/flask_fd/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_1.py` & `flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_1.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_2.py` & `flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_2.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/plop/flask/main_flask_fd_3.py` & `flask-fd-1.0.4/flask_fd/plop/flask/main_flask_fd_3.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/plop/flask/starter/FlaskFdIcon` & `flask-fd-1.0.4/flask_fd/plop/flask/starter/FlaskFdIcon`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/plop/flask/starter/flask_for_desktop.py` & `flask-fd-1.0.4/flask_fd/plop/flask/starter/flask_for_desktop.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd/plop/ploppers.py` & `flask-fd-1.0.4/flask_fd/plop/ploppers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/flask_fd.egg-info/PKG-INFO` & `flask-fd-1.0.4/flask_fd.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fd
-Version: 1.0.3
+Version: 1.0.4
 Summary: Use flask to create desktop applications
 Home-page: https://github.com/byoso/flask_for_desktop
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: flask desktop gui
 Platform: UNKNOWN
@@ -39,40 +39,25 @@
 
 ### 2. Installation
 
 ```
 pip install flask-fd
 ```
 
-### 3. get a converter file
-For the simpliest version:
+### 3. get the files
+If you start your app from scratch:
 
+```sh
+flask-fd plop starter
 ```
-flask-fd plop 1
-```
-or for a more customizable and fancy interface, very easy (the best choice)
-```
-flask-fd plop 2
-```
-or just running the app in the default web browser
-```
-flask-fd plop 3
+If you've already done your app and just want to convert it:
+
+```sh
+flask-fd plop converter
 ```
+This one will give you a file that you'll just have to configure following
+the steps in the comments.
 
 The file appear in your current working directory.
 Fill the parameters in the given file.
 
-### 4. launch the app
-
-Execute the provided file, you'll see you flask app wrapped in a pretty
-Gtk interface
-
-### 5. get an installer (for linux)
-This if you want to integrate your app in the system.
-The installer uses [Geninstaller](https://github.com/byoso/geninstaller)
-
-```
-flask-fd plop installer
-```
-Fill the parameters in the installer.
-
```

### Comparing `flask-fd-1.0.3/flask_fd.egg-info/SOURCES.txt` & `flask-fd-1.0.4/flask_fd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-fd-1.0.3/setup.py` & `flask-fd-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         "flask_fd.plop.flask.starter",
         "flask_fd.plop.flask.starter.flaskapp",
         ],
     # include_package_data=True,
     package_data={'': ['FlaskFdIcon', 'installer']},
     python_requires='>=3.6',
     install_requires=[
-        "flamewok >= 1.0.8",
+        "flamewok >= 1.2.1",
         "flask-sqlalchemy",
         "flask-migrate",
     ],
     keywords='flask desktop gui',
     entry_points={
         "console_scripts": [
             "flask-fd=flask_fd.cmd:cmd",
```

