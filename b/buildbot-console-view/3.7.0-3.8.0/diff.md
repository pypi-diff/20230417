# Comparing `tmp/buildbot-console-view-3.7.0.tar.gz` & `tmp/buildbot-console-view-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-console-view-3.7.0.tar", last modified: Sun Dec  4 11:52:48 2022, max compression
+gzip compressed data, was "dist/buildbot-console-view-3.8.0.tar", last modified: Mon Apr 17 01:21:14 2023, max compression
```

## Comparing `buildbot-console-view-3.7.0.tar` & `buildbot-console-view-3.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      320 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      860 2022-12-04 11:48:49.000000 buildbot-console-view-3.7.0/buildbot_console_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12053 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    40229 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view/static/scripts.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1161 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view/static/styles.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1660 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view/static/styles.css.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      320 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      478 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       76 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       22 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/buildbot_console_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2022-12-04 11:52:48.000000 buildbot-console-view-3.7.0/setup.cfg
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1544 2022-12-04 11:48:49.000000 buildbot-console-view-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      264 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      860 2023-04-17 01:17:21.000000 buildbot-console-view-3.8.0/buildbot_console_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12053 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    40229 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view/static/scripts.js.map
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1161 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view/static/styles.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1660 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view/static/styles.css.map
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      264 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      478 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       55 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       22 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/buildbot_console_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:21:14.000000 buildbot-console-view-3.8.0/setup.cfg
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1544 2023-04-17 01:17:21.000000 buildbot-console-view-3.8.0/setup.py
```

### Comparing `buildbot-console-view-3.7.0/buildbot_console_view/__init__.py` & `buildbot-console-view-3.8.0/buildbot_console_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.7.0/buildbot_console_view/static/scripts.js` & `buildbot-console-view-3.8.0/buildbot_console_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.7.0/buildbot_console_view/static/scripts.js.map` & `buildbot-console-view-3.8.0/buildbot_console_view/static/scripts.js.map`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.7.0/buildbot_console_view/static/styles.css` & `buildbot-console-view-3.8.0/buildbot_console_view/static/styles.css`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.7.0/buildbot_console_view/static/styles.css.map` & `buildbot-console-view-3.8.0/buildbot_console_view/static/styles.css.map`

 * *Files identical despite different names*

### Comparing `buildbot-console-view-3.7.0/setup.py` & `buildbot-console-view-3.8.0/setup.py`

 * *Files identical despite different names*

