# Comparing `tmp/flask-fd-1.1.0.tar.gz` & `tmp/flask-fd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-fd-1.1.0.tar", last modified: Mon Apr 17 14:07:54 2023, max compression
+gzip compressed data, was "flask-fd-1.1.1.tar", last modified: Mon Apr 17 14:13:00 2023, max compression
```

## Comparing `flask-fd-1.1.0.tar` & `flask-fd-1.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.333872 flask-fd-1.1.0/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1069 2022-09-26 03:49:00.000000 flask-fd-1.1.0/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 14:07:54.333872 flask-fd-1.1.0/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-17 13:33:33.000000 flask-fd-1.1.0/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.317872 flask-fd-1.1.0/flask_fd/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       23 2023-04-17 13:48:31.000000 flask-fd-1.1.0/flask_fd/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/__main__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      738 2023-04-16 19:57:37.000000 flask-fd-1.1.0/flask_fd/cmd.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.321872 flask-fd-1.1.0/flask_fd/gui/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/builder.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/containers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/header_bar.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/helpers.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/indicators.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/menus.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/gui/web.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/helpers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.325873 flask-fd-1.1.0/flask_fd/launchers/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/launchers/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/launchers/launchers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.325873 flask-fd-1.1.0/flask_fd/plop/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/plop/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.325873 flask-fd-1.1.0/flask_fd/plop/flask/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/plop/flask/main_flask_fd_1.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/plop/flask/main_flask_fd_2.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-09-26 03:49:00.000000 flask-fd-1.1.0/flask_fd/plop/flask/main_flask_fd_3.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.325873 flask-fd-1.1.0/flask_fd/plop/flask/starter/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:57:47.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/__init__.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2197 2023-04-12 04:06:05.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flask_for_desktop.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.325873 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-12 03:07:25.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.329872 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      367 2023-04-12 03:09:36.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      333 2022-11-15 17:20:16.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      307 2023-04-12 03:10:18.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/models.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.329872 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:31.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.329872 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/css/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:40.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/css/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.329872 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/img/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-11 23:49:22.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/img/FlaskFdIcon
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:43.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/img/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.329872 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/js/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:46.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/js/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.333872 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:48:08.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/templates/__init__.py
--rw-r--r--   0 byoso     (1000) byoso     (1000)     2918 2023-04-12 02:55:37.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/templates/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      297 2023-04-12 03:12:06.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/templates/index.html
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      256 2023-04-12 03:09:53.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/views.py
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)      106 2023-04-12 03:08:22.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/main.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      282 2023-04-12 03:22:54.000000 flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/shell_context.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1257 2023-04-17 14:04:46.000000 flask-fd-1.1.0/flask_fd/plop/ploppers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:07:54.321872 flask-fd-1.1.0/flask_fd.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 14:07:54.000000 flask-fd-1.1.0/flask_fd.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1673 2023-04-17 14:07:54.000000 flask-fd-1.1.0/flask_fd.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-17 14:07:54.000000 flask-fd-1.1.0/flask_fd.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 14:07:54.000000 flask-fd-1.1.0/flask_fd.egg-info/entry_points.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 14:07:54.000000 flask-fd-1.1.0/flask_fd.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2023-04-17 14:07:54.000000 flask-fd-1.1.0/flask_fd.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-17 14:07:54.333872 flask-fd-1.1.0/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2189 2023-04-17 13:47:33.000000 flask-fd-1.1.0/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.076397 flask-fd-1.1.1/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1069 2022-09-26 03:49:00.000000 flask-fd-1.1.1/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 14:13:00.076397 flask-fd-1.1.1/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-17 13:33:33.000000 flask-fd-1.1.1/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.060397 flask-fd-1.1.1/flask_fd/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       23 2023-04-17 14:12:00.000000 flask-fd-1.1.1/flask_fd/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      988 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/__main__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      738 2023-04-16 19:57:37.000000 flask-fd-1.1.1/flask_fd/cmd.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.064396 flask-fd-1.1.1/flask_fd/gui/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      323 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2822 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/builder.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3976 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/containers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      492 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/header_bar.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      175 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/helpers.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2255 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/indicators.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      574 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/menus.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/gui/web.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      230 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/helpers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.064396 flask-fd-1.1.1/flask_fd/launchers/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       67 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/launchers/__init__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      810 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/launchers/launchers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.068396 flask-fd-1.1.1/flask_fd/plop/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/plop/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.068396 flask-fd-1.1.1/flask_fd/plop/flask/
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1326 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/plop/flask/main_flask_fd_1.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2984 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/plop/flask/main_flask_fd_2.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2656 2022-09-26 03:49:00.000000 flask-fd-1.1.1/flask_fd/plop/flask/main_flask_fd_3.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.068396 flask-fd-1.1.1/flask_fd/plop/flask/starter/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:57:47.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/__init__.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2197 2023-04-12 04:06:05.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flask_for_desktop.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.068396 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-12 03:07:25.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.072397 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      367 2023-04-12 03:09:36.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      333 2022-11-15 17:20:16.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      307 2023-04-12 03:10:18.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/models.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.072397 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:31.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.072397 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/css/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:40.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/css/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.072397 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/img/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4567 2023-04-11 23:49:22.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/img/FlaskFdIcon
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:43.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/img/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.072397 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/js/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:59:46.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/js/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.076397 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-17 13:48:08.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/templates/__init__.py
+-rw-r--r--   0 byoso     (1000) byoso     (1000)     2918 2023-04-12 02:55:37.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/templates/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      297 2023-04-12 03:12:06.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/templates/index.html
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      256 2023-04-12 03:09:53.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/views.py
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)      106 2023-04-12 03:08:22.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/main.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      282 2023-04-12 03:22:54.000000 flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/shell_context.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1296 2023-04-17 14:11:47.000000 flask-fd-1.1.1/flask_fd/plop/ploppers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-17 14:13:00.060397 flask-fd-1.1.1/flask_fd.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1596 2023-04-17 14:12:59.000000 flask-fd-1.1.1/flask_fd.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1673 2023-04-17 14:12:59.000000 flask-fd-1.1.1/flask_fd.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-17 14:12:59.000000 flask-fd-1.1.1/flask_fd.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 14:12:59.000000 flask-fd-1.1.1/flask_fd.egg-info/entry_points.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       47 2023-04-17 14:12:59.000000 flask-fd-1.1.1/flask_fd.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        9 2023-04-17 14:12:59.000000 flask-fd-1.1.1/flask_fd.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-17 14:13:00.076397 flask-fd-1.1.1/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2189 2023-04-17 13:47:33.000000 flask-fd-1.1.1/setup.py
```

### Comparing `flask-fd-1.1.0/LICENSE.md` & `flask-fd-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/PKG-INFO` & `flask-fd-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fd
-Version: 1.1.0
+Version: 1.1.1
 Summary: Use flask to create desktop applications
 Home-page: https://github.com/byoso/flask_for_desktop
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: flask desktop gui
 Platform: UNKNOWN
```

### Comparing `flask-fd-1.1.0/README.md` & `flask-fd-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/__main__.py` & `flask-fd-1.1.1/flask_fd/__main__.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/cmd.py` & `flask-fd-1.1.1/flask_fd/cmd.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/gui/builder.py` & `flask-fd-1.1.1/flask_fd/gui/builder.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/gui/containers.py` & `flask-fd-1.1.1/flask_fd/gui/containers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/gui/indicators.py` & `flask-fd-1.1.1/flask_fd/gui/indicators.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/gui/menus.py` & `flask-fd-1.1.1/flask_fd/gui/menus.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/launchers/launchers.py` & `flask-fd-1.1.1/flask_fd/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/plop/flask/main_flask_fd_1.py` & `flask-fd-1.1.1/flask_fd/plop/flask/main_flask_fd_1.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/plop/flask/main_flask_fd_2.py` & `flask-fd-1.1.1/flask_fd/plop/flask/main_flask_fd_2.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/plop/flask/main_flask_fd_3.py` & `flask-fd-1.1.1/flask_fd/plop/flask/main_flask_fd_3.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/plop/flask/starter/flask_for_desktop.py` & `flask-fd-1.1.1/flask_fd/plop/flask/starter/flask_for_desktop.py`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/static/img/FlaskFdIcon` & `flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/static/img/FlaskFdIcon`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/plop/flask/starter/flaskapp/app/templates/_base.html` & `flask-fd-1.1.1/flask_fd/plop/flask/starter/flaskapp/app/templates/_base.html`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/flask_fd/plop/ploppers.py` & `flask-fd-1.1.1/flask_fd/plop/ploppers.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,10 +31,12 @@
 def plop_starter():
     cwd = os.getcwd()
     # copy starter folders
     folder = os.path.join(BASE_DIR, "flask/starter")
     if os.path.exists(os.path.join(cwd, "flask_fd_app")):
         print("Aborted: flask_fd_app already exists in the current directory")
     else:
+        # icon
+        _plop_icon(cwd)
         shutil.copytree(folder, os.path.join(cwd, "flask_fd_app"))
         set_executable(os.path.join(cwd, 'flask_fd_app/flask_for_desktop.py'))
         print("Flask-fd starter kit ploped !")
```

### Comparing `flask-fd-1.1.0/flask_fd.egg-info/PKG-INFO` & `flask-fd-1.1.1/flask_fd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-fd
-Version: 1.1.0
+Version: 1.1.1
 Summary: Use flask to create desktop applications
 Home-page: https://github.com/byoso/flask_for_desktop
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: flask desktop gui
 Platform: UNKNOWN
```

### Comparing `flask-fd-1.1.0/flask_fd.egg-info/SOURCES.txt` & `flask-fd-1.1.1/flask_fd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-fd-1.1.0/setup.py` & `flask-fd-1.1.1/setup.py`

 * *Files identical despite different names*

