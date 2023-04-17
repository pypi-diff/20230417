# Comparing `tmp/wozoxutils-0.1.tar.gz` & `tmp/wozoxutils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wozoxutils-0.1.tar", last modified: Mon Apr 17 12:16:29 2023, max compression
+gzip compressed data, was "wozoxutils-0.2.tar", last modified: Mon Apr 17 12:33:29 2023, max compression
```

## Comparing `wozoxutils-0.1.tar` & `wozoxutils-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:16:29.558903 wozoxutils-0.1/
--rw-rw-rw-   0        0        0     1062 2023-04-17 11:13:35.000000 wozoxutils-0.1/LICENSE
--rw-rw-rw-   0        0        0      277 2023-04-17 12:16:29.558903 wozoxutils-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-04-17 11:13:35.000000 wozoxutils-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 12:16:29.559904 wozoxutils-0.1/setup.cfg
--rw-rw-rw-   0        0        0      387 2023-04-17 11:54:40.000000 wozoxutils-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:16:29.556138 wozoxutils-0.1/wozoxutils/
--rw-rw-rw-   0        0        0        0 2023-04-17 11:56:26.000000 wozoxutils-0.1/wozoxutils/__init__.py
--rw-rw-rw-   0        0        0     1344 2023-04-17 12:12:35.000000 wozoxutils-0.1/wozoxutils/file.py
--rw-rw-rw-   0        0        0      895 2023-04-17 12:15:03.000000 wozoxutils-0.1/wozoxutils/hash.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:16:29.557899 wozoxutils-0.1/wozoxutils.egg-info/
--rw-rw-rw-   0        0        0      277 2023-04-17 12:16:29.000000 wozoxutils-0.1/wozoxutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-17 12:16:29.000000 wozoxutils-0.1/wozoxutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:16:29.000000 wozoxutils-0.1/wozoxutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 12:16:29.000000 wozoxutils-0.1/wozoxutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:33:29.285669 wozoxutils-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 12:33:14.000000 wozoxutils-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 12:33:29.285669 wozoxutils-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-17 12:33:14.000000 wozoxutils-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:33:29.285669 wozoxutils-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-17 12:33:14.000000 wozoxutils-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:33:29.285669 wozoxutils-0.2/wozoxutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:33:14.000000 wozoxutils-0.2/wozoxutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 12:33:14.000000 wozoxutils-0.2/wozoxutils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-17 12:33:14.000000 wozoxutils-0.2/wozoxutils/hash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:33:29.285669 wozoxutils-0.2/wozoxutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 12:33:29.000000 wozoxutils-0.2/wozoxutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-17 12:33:29.000000 wozoxutils-0.2/wozoxutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:33:29.000000 wozoxutils-0.2/wozoxutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 12:33:29.000000 wozoxutils-0.2/wozoxutils.egg-info/top_level.txt
```

### Comparing `wozoxutils-0.1/LICENSE` & `wozoxutils-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.1/wozoxutils/file.py` & `wozoxutils-0.2/wozoxutils/file.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.1/wozoxutils/hash.py` & `wozoxutils-0.2/wozoxutils/hash.py`

 * *Files identical despite different names*

