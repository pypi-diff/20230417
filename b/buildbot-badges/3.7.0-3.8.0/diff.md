# Comparing `tmp/buildbot-badges-3.7.0.tar.gz` & `tmp/buildbot-badges-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-badges-3.7.0.tar", last modified: Sun Dec  4 11:53:18 2022, max compression
+gzip compressed data, was "dist/buildbot-badges-3.8.0.tar", last modified: Mon Apr 17 01:21:57 2023, max compression
```

## Comparing `buildbot-badges-3.7.0.tar` & `buildbot-badges-3.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      312 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/PKG-INFO
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5167 2022-12-04 11:48:49.000000 buildbot-badges-3.7.0/buildbot_badges/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges/static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-badges-3.7.0/buildbot_badges/static/.placeholder
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges/templates/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1212 2022-12-04 11:48:49.000000 buildbot-badges-3.7.0/buildbot_badges/templates/badgeio.svg.j2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      714 2022-12-04 11:48:49.000000 buildbot-badges-3.7.0/buildbot_badges/templates/flat-square.svg.j2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1480 2022-12-04 11:48:49.000000 buildbot-badges-3.7.0/buildbot_badges/templates/flat.svg.j2
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1574 2022-12-04 11:48:49.000000 buildbot-badges-3.7.0/buildbot_badges/templates/plastic.svg.j2
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges.egg-info/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      312 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges.egg-info/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      507 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges.egg-info/SOURCES.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges.egg-info/dependency_links.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       64 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges.egg-info/entry_points.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       32 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges.egg-info/requires.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/buildbot_badges.egg-info/top_level.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2022-12-04 11:53:18.000000 buildbot-badges-3.7.0/setup.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1684 2022-12-04 11:48:49.000000 buildbot-badges-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      256 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/PKG-INFO
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5167 2023-04-17 01:17:21.000000 buildbot-badges-3.8.0/buildbot_badges/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges/static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-badges-3.8.0/buildbot_badges/static/.placeholder
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges/templates/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1212 2023-04-17 01:17:21.000000 buildbot-badges-3.8.0/buildbot_badges/templates/badgeio.svg.j2
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      714 2023-04-17 01:17:21.000000 buildbot-badges-3.8.0/buildbot_badges/templates/flat-square.svg.j2
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1480 2023-04-17 01:17:21.000000 buildbot-badges-3.8.0/buildbot_badges/templates/flat.svg.j2
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1574 2023-04-17 01:17:21.000000 buildbot-badges-3.8.0/buildbot_badges/templates/plastic.svg.j2
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges.egg-info/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      256 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges.egg-info/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      507 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges.egg-info/SOURCES.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        1 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges.egg-info/dependency_links.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       43 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges.egg-info/entry_points.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       32 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges.egg-info/requires.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       16 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/buildbot_badges.egg-info/top_level.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       38 2023-04-17 01:21:57.000000 buildbot-badges-3.8.0/setup.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1684 2023-04-17 01:17:21.000000 buildbot-badges-3.8.0/setup.py
```

### Comparing `buildbot-badges-3.7.0/buildbot_badges/__init__.py` & `buildbot-badges-3.8.0/buildbot_badges/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.7.0/buildbot_badges/templates/badgeio.svg.j2` & `buildbot-badges-3.8.0/buildbot_badges/templates/badgeio.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.7.0/buildbot_badges/templates/flat-square.svg.j2` & `buildbot-badges-3.8.0/buildbot_badges/templates/flat-square.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.7.0/buildbot_badges/templates/flat.svg.j2` & `buildbot-badges-3.8.0/buildbot_badges/templates/flat.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.7.0/buildbot_badges/templates/plastic.svg.j2` & `buildbot-badges-3.8.0/buildbot_badges/templates/plastic.svg.j2`

 * *Files identical despite different names*

### Comparing `buildbot-badges-3.7.0/setup.py` & `buildbot-badges-3.8.0/setup.py`

 * *Files identical despite different names*

