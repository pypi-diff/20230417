# Comparing `tmp/buildbot-waterfall-view-3.7.0.tar.gz` & `tmp/buildbot-waterfall-view-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-waterfall-view-3.7.0.tar", last modified: Sun Dec  4 11:53:12 2022, max compression
+gzip compressed data, was "dist/buildbot-waterfall-view-3.8.0.tar", last modified: Mon Apr 17 01:21:50 2023, max compression
```

## Comparing `buildbot-waterfall-view-3.7.0.tar` & `buildbot-waterfall-view-3.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      324 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      862 2022-12-04 11:48:49.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    94655 2022-12-04 11:53:11.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   762470 2022-12-04 11:53:11.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/scripts.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3724 2022-12-04 11:53:11.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/styles.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4921 2022-12-04 11:53:11.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/styles.css.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      324 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      500 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       80 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       24 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/buildbot_waterfall_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2022-12-04 11:53:12.000000 buildbot-waterfall-view-3.7.0/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1555 2022-12-04 11:48:49.000000 buildbot-waterfall-view-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      268 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      862 2023-04-17 01:17:21.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    94655 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   762470 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/scripts.js.map
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3724 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/styles.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4921 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/styles.css.map
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      268 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      500 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       59 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       24 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/buildbot_waterfall_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:21:50.000000 buildbot-waterfall-view-3.8.0/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1555 2023-04-17 01:17:21.000000 buildbot-waterfall-view-3.8.0/setup.py
```

### Comparing `buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/__init__.py` & `buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/scripts.js` & `buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/scripts.js.map` & `buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/scripts.js.map`

 * *Files identical despite different names*

### Comparing `buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/styles.css` & `buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/styles.css`

 * *Files identical despite different names*

### Comparing `buildbot-waterfall-view-3.7.0/buildbot_waterfall_view/static/styles.css.map` & `buildbot-waterfall-view-3.8.0/buildbot_waterfall_view/static/styles.css.map`

 * *Files identical despite different names*

### Comparing `buildbot-waterfall-view-3.7.0/setup.py` & `buildbot-waterfall-view-3.8.0/setup.py`

 * *Files identical despite different names*

