# Comparing `tmp/buildbot-wsgi-dashboards-3.7.0.tar.gz` & `tmp/buildbot-wsgi-dashboards-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-wsgi-dashboards-3.7.0.tar", last modified: Sun Dec  4 11:53:18 2022, max compression
+gzip compressed data, was "dist/buildbot-wsgi-dashboards-3.8.0.tar", last modified: Mon Apr 17 01:21:56 2023, max compression
```

## Comparing `buildbot-wsgi-dashboards-3.7.0.tar` & `buildbot-wsgi-dashboards-3.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      375 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2022-12-04 11:48:49.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2025 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/static/scripts.js
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8307 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/static/scripts.js.map
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      375 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      421 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       82 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       25 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2022-12-04 11:53:18.000000 buildbot-wsgi-dashboards-3.7.0/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1609 2022-12-04 11:48:49.000000 buildbot-wsgi-dashboards-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      319 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2023-04-17 01:17:21.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2025 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/static/scripts.js
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8307 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/static/scripts.js.map
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      319 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      421 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       61 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       25 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:21:56.000000 buildbot-wsgi-dashboards-3.8.0/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1609 2023-04-17 01:17:21.000000 buildbot-wsgi-dashboards-3.8.0/setup.py
```

### Comparing `buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/__init__.py` & `buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/static/scripts.js` & `buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/static/scripts.js`

 * *Files identical despite different names*

### Comparing `buildbot-wsgi-dashboards-3.7.0/buildbot_wsgi_dashboards/static/scripts.js.map` & `buildbot-wsgi-dashboards-3.8.0/buildbot_wsgi_dashboards/static/scripts.js.map`

 * *Files identical despite different names*

### Comparing `buildbot-wsgi-dashboards-3.7.0/setup.py` & `buildbot-wsgi-dashboards-3.8.0/setup.py`

 * *Files identical despite different names*

