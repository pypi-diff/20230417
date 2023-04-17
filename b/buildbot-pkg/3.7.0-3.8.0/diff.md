# Comparing `tmp/buildbot-pkg-3.7.0.tar.gz` & `tmp/buildbot-pkg-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-pkg-3.7.0.tar", last modified: Sun Dec  4 11:50:51 2022, max compression
+gzip compressed data, was "dist/buildbot-pkg-3.8.0.tar", last modified: Mon Apr 17 01:20:00 2023, max compression
```

## Comparing `buildbot-pkg-3.7.0.tar` & `buildbot-pkg-3.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      307 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1292 2022-12-04 11:48:49.000000 buildbot-pkg-3.7.0/README
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/buildbot_pkg.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      307 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/buildbot_pkg.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      220 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/buildbot_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/buildbot_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/buildbot_pkg.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       13 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/buildbot_pkg.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8509 2022-12-04 11:48:49.000000 buildbot-pkg-3.7.0/buildbot_pkg.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2022-12-04 11:50:50.000000 buildbot-pkg-3.7.0/setup.cfg
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1194 2022-12-04 11:48:49.000000 buildbot-pkg-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:20:00.000000 buildbot-pkg-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      251 2023-04-17 01:20:00.000000 buildbot-pkg-3.8.0/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1292 2023-04-17 01:17:21.000000 buildbot-pkg-3.8.0/README
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:20:00.000000 buildbot-pkg-3.8.0/buildbot_pkg.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      251 2023-04-17 01:19:59.000000 buildbot-pkg-3.8.0/buildbot_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      220 2023-04-17 01:19:59.000000 buildbot-pkg-3.8.0/buildbot_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:19:59.000000 buildbot-pkg-3.8.0/buildbot_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       19 2023-04-17 01:19:59.000000 buildbot-pkg-3.8.0/buildbot_pkg.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       13 2023-04-17 01:19:59.000000 buildbot-pkg-3.8.0/buildbot_pkg.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8509 2023-04-17 01:17:21.000000 buildbot-pkg-3.8.0/buildbot_pkg.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:20:00.000000 buildbot-pkg-3.8.0/setup.cfg
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)     1194 2023-04-17 01:17:21.000000 buildbot-pkg-3.8.0/setup.py
```

### Comparing `buildbot-pkg-3.7.0/README` & `buildbot-pkg-3.8.0/README`

 * *Files identical despite different names*

### Comparing `buildbot-pkg-3.7.0/buildbot_pkg.py` & `buildbot-pkg-3.8.0/buildbot_pkg.py`

 * *Files identical despite different names*

### Comparing `buildbot-pkg-3.7.0/setup.py` & `buildbot-pkg-3.8.0/setup.py`

 * *Files identical despite different names*

