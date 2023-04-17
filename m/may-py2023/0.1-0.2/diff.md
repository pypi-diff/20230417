# Comparing `tmp/may_py2023-0.1.tar.gz` & `tmp/may_py2023-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "may_py2023-0.1.tar", last modified: Mon Apr 17 16:40:06 2023, max compression
+gzip compressed data, was "may_py2023-0.2.tar", last modified: Mon Apr 17 17:39:35 2023, max compression
```

## Comparing `may_py2023-0.1.tar` & `may_py2023-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:06.527857 may_py2023-0.1/
--rw-rw-rw-   0        0        0      167 2023-04-17 16:40:06.527857 may_py2023-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:06.501128 may_py2023-0.1/may_py2023/
--rw-rw-rw-   0        0        0       23 2023-04-17 16:36:55.000000 may_py2023-0.1/may_py2023/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:06.525135 may_py2023-0.1/may_py2023.egg-info/
--rw-rw-rw-   0        0        0      167 2023-04-17 16:40:06.000000 may_py2023-0.1/may_py2023.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-04-17 16:40:06.000000 may_py2023-0.1/may_py2023.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:40:06.000000 may_py2023-0.1/may_py2023.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:40:06.000000 may_py2023-0.1/may_py2023.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-04-17 16:40:06.000000 may_py2023-0.1/may_py2023.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 16:40:06.531872 may_py2023-0.1/setup.cfg
--rw-rw-rw-   0        0        0      265 2023-04-17 16:28:42.000000 may_py2023-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:35.020476 may_py2023-0.2/
+-rw-rw-rw-   0        0        0      167 2023-04-17 17:39:35.020476 may_py2023-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:34.985020 may_py2023-0.2/may_py2023/
+-rw-rw-rw-   0        0        0       32 2023-04-17 17:33:48.000000 may_py2023-0.2/may_py2023/_init_.py
+-rw-rw-rw-   0        0        0       23 2023-04-17 17:33:48.000000 may_py2023-0.2/may_py2023/may_py2023.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:35.018485 may_py2023-0.2/may_py2023.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-04-17 17:39:34.000000 may_py2023-0.2/may_py2023.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-17 17:39:34.000000 may_py2023-0.2/may_py2023.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:39:34.000000 may_py2023-0.2/may_py2023.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 16:40:06.000000 may_py2023-0.2/may_py2023.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-04-17 17:39:34.000000 may_py2023-0.2/may_py2023.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:39:35.030475 may_py2023-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      265 2023-04-17 17:36:08.000000 may_py2023-0.2/setup.py
```

