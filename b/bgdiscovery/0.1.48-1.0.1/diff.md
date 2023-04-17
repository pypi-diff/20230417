# Comparing `tmp/bgdiscovery-0.1.48.tar.gz` & `tmp/bgdiscovery-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgdiscovery-0.1.48.tar", last modified: Mon Apr 17 06:15:47 2023, max compression
+gzip compressed data, was "bgdiscovery-1.0.1.tar", last modified: Mon Apr 17 06:16:23 2023, max compression
```

## Comparing `bgdiscovery-0.1.48.tar` & `bgdiscovery-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-17 06:15:47.800747 bgdiscovery-0.1.48/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2240 2023-04-17 06:15:47.800747 bgdiscovery-0.1.48/PKG-INFO
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-17 06:15:47.800747 bgdiscovery-0.1.48/bgdiscovery.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2240 2023-04-17 06:15:47.000000 bgdiscovery-0.1.48/bgdiscovery.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2023-04-17 06:15:47.000000 bgdiscovery-0.1.48/bgdiscovery.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-17 06:15:47.000000 bgdiscovery-0.1.48/bgdiscovery.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-04-17 06:15:47.000000 bgdiscovery-0.1.48/bgdiscovery.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2023-04-17 06:15:47.000000 bgdiscovery-0.1.48/bgdiscovery.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2023-04-17 06:15:47.000000 bgdiscovery-0.1.48/bgdiscovery.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-17 06:15:47.800747 bgdiscovery-0.1.48/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3340 2023-04-17 06:03:30.000000 bgdiscovery-0.1.48/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-17 06:16:23.089274 bgdiscovery-1.0.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2239 2023-04-17 06:16:23.089274 bgdiscovery-1.0.1/PKG-INFO
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-17 06:16:23.085274 bgdiscovery-1.0.1/bgdiscovery.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2239 2023-04-17 06:16:23.000000 bgdiscovery-1.0.1/bgdiscovery.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2023-04-17 06:16:23.000000 bgdiscovery-1.0.1/bgdiscovery.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-17 06:16:23.000000 bgdiscovery-1.0.1/bgdiscovery.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-04-17 06:16:23.000000 bgdiscovery-1.0.1/bgdiscovery.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2023-04-17 06:16:23.000000 bgdiscovery-1.0.1/bgdiscovery.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       12 2023-04-17 06:16:23.000000 bgdiscovery-1.0.1/bgdiscovery.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-17 06:16:23.089274 bgdiscovery-1.0.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3340 2023-04-17 06:03:30.000000 bgdiscovery-1.0.1/setup.py
```

### Comparing `bgdiscovery-0.1.48/PKG-INFO` & `bgdiscovery-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgdiscovery
-Version: 0.1.48
+Version: 1.0.1
 Summary: biGENIUS Discovery App.
 Home-page: https://www.bigenius.info/
 Author: biGENIUS AG
 Author-email: gergely.szecsenyi@bigenius.info
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bgdiscovery-0.1.48/bgdiscovery.egg-info/PKG-INFO` & `bgdiscovery-1.0.1/bgdiscovery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgdiscovery
-Version: 0.1.48
+Version: 1.0.1
 Summary: biGENIUS Discovery App.
 Home-page: https://www.bigenius.info/
 Author: biGENIUS AG
 Author-email: gergely.szecsenyi@bigenius.info
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bgdiscovery-0.1.48/setup.py` & `bgdiscovery-1.0.1/setup.py`

 * *Files identical despite different names*

