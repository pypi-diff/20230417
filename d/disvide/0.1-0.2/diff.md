# Comparing `tmp/disvide-0.1.tar.gz` & `tmp/disvide-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disvide-0.1.tar", last modified: Mon Apr 17 14:20:48 2023, max compression
+gzip compressed data, was "disvide-0.2.tar", last modified: Mon Apr 17 14:30:05 2023, max compression
```

## Comparing `disvide-0.1.tar` & `disvide-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:20:48.187965 disvide-0.1/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.1/LICENSE
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      365 2023-04-17 14:20:48.187965 disvide-0.1/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2674 2023-04-17 12:38:38.000000 disvide-0.1/README.md
-drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:20:48.187965 disvide-0.1/disvide.egg-info/
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      365 2023-04-17 14:20:48.000000 disvide-0.1/disvide.egg-info/PKG-INFO
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      160 2023-04-17 14:20:48.000000 disvide-0.1/disvide.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:20:48.000000 disvide-0.1/disvide.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:20:48.000000 disvide-0.1/disvide.egg-info/top_level.txt
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      103 2023-04-17 14:20:48.197965 disvide-0.1/setup.cfg
--rw-r--r--   0 mohammed  (1000) mohammed  (1000)      475 2023-04-17 14:20:46.000000 disvide-0.1/setup.py
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:30:05.637980 disvide-0.2/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     1062 2023-04-17 12:14:03.000000 disvide-0.2/LICENSE
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      365 2023-04-17 14:30:05.637980 disvide-0.2/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)     2674 2023-04-17 12:38:38.000000 disvide-0.2/README.rst
+drwxr-xr-x   0 mohammed  (1000) mohammed  (1000)        0 2023-04-17 14:30:05.637980 disvide-0.2/disvide.egg-info/
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      365 2023-04-17 14:30:05.000000 disvide-0.2/disvide.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      161 2023-04-17 14:30:05.000000 disvide-0.2/disvide.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:30:05.000000 disvide-0.2/disvide.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)        1 2023-04-17 14:30:05.000000 disvide-0.2/disvide.egg-info/top_level.txt
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      104 2023-04-17 14:30:05.637980 disvide-0.2/setup.cfg
+-rw-r--r--   0 mohammed  (1000) mohammed  (1000)      475 2023-04-17 14:29:36.000000 disvide-0.2/setup.py
```

### Comparing `disvide-0.1/LICENSE` & `disvide-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `disvide-0.1/README.md` & `disvide-0.2/README.rst`

 * *Files identical despite different names*

