# Comparing `tmp/buildbot-grid-view-3.7.0.tar.gz` & `tmp/buildbot-grid-view-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-grid-view-3.7.0.tar", last modified: Sun Dec  4 11:53:00 2022, max compression
+gzip compressed data, was "dist/buildbot-grid-view-3.8.0.tar", last modified: Mon Apr 17 01:21:31 2023, max compression
```

## Comparing `buildbot-grid-view-3.7.0.tar` & `buildbot-grid-view-3.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      318 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      861 2022-12-04 11:48:49.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9944 2022-12-04 11:52:59.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31122 2022-12-04 11:52:59.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/static/scripts.js.map
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      545 2022-12-04 11:52:59.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/static/styles.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      837 2022-12-04 11:52:59.000000 buildbot-grid-view-3.7.0/buildbot_grid_view/static/styles.css.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      318 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      445 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       70 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/buildbot_grid_view.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2022-12-04 11:53:00.000000 buildbot-grid-view-3.7.0/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1533 2022-12-04 11:48:49.000000 buildbot-grid-view-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      262 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      861 2023-04-17 01:17:21.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9944 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31122 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/static/scripts.js.map
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      545 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/static/styles.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      837 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view/static/styles.css.map
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      262 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      445 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       49 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/buildbot_grid_view.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:21:31.000000 buildbot-grid-view-3.8.0/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1533 2023-04-17 01:17:21.000000 buildbot-grid-view-3.8.0/setup.py
```

### Comparing `buildbot-grid-view-3.7.0/buildbot_grid_view/__init__.py` & `buildbot-grid-view-3.8.0/buildbot_grid_view/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.7.0/buildbot_grid_view/static/scripts.js` & `buildbot-grid-view-3.8.0/buildbot_grid_view/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.7.0/buildbot_grid_view/static/scripts.js.map` & `buildbot-grid-view-3.8.0/buildbot_grid_view/static/scripts.js.map`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.7.0/buildbot_grid_view/static/styles.css` & `buildbot-grid-view-3.8.0/buildbot_grid_view/static/styles.css`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.7.0/buildbot_grid_view/static/styles.css.map` & `buildbot-grid-view-3.8.0/buildbot_grid_view/static/styles.css.map`

 * *Files identical despite different names*

### Comparing `buildbot-grid-view-3.7.0/setup.py` & `buildbot-grid-view-3.8.0/setup.py`

 * *Files identical despite different names*

