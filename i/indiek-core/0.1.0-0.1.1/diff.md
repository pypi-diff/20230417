# Comparing `tmp/indiek-core-0.1.0.tar.gz` & `tmp/indiek-core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-1ubymxre/indiek-core-0.1.0.tar", last modified: Sat Apr 15 23:36:42 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-or7b6s5q/indiek-core-0.1.1.tar", last modified: Mon Apr 17 01:36:04 2023, max compression
```

## Comparing `indiek-core-0.1.0.tar` & `indiek-core-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-15 23:36:42.402784 indiek-core-0.1.0/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.0/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      269 2023-04-15 23:36:42.402784 indiek-core-0.1.0/PKG-INFO
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-15 23:36:42.398784 indiek-core-0.1.0/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-15 23:36:42.402784 indiek-core-0.1.0/indiek/core/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       13 2023-04-15 23:00:43.000000 indiek-core-0.1.0/indiek/core/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       76 2023-04-15 23:08:05.000000 indiek-core-0.1.0/indiek/core/items.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-15 23:36:42.402784 indiek-core-0.1.0/indiek_core.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      269 2023-04-15 23:36:42.000000 indiek-core-0.1.0/indiek_core.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      265 2023-04-15 23:36:42.000000 indiek-core-0.1.0/indiek_core.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-04-15 23:36:42.000000 indiek-core-0.1.0/indiek_core.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-04-15 23:36:42.000000 indiek-core-0.1.0/indiek_core.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-04-15 23:36:42.000000 indiek-core-0.1.0/indiek_core.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-04-15 23:36:42.402784 indiek-core-0.1.0/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      472 2023-04-15 23:21:33.000000 indiek-core-0.1.0/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-15 23:36:42.402784 indiek-core-0.1.0/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      243 2023-04-15 23:34:13.000000 indiek-core-0.1.0/tests/test_items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.1/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1125 2023-04-17 01:36:04.626090 indiek-core-0.1.1/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      759 2023-04-17 01:35:55.000000 indiek-core-0.1.1/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.622090 indiek-core-0.1.1/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/indiek/core/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       13 2023-04-15 23:00:43.000000 indiek-core-0.1.1/indiek/core/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      420 2023-04-17 00:48:04.000000 indiek-core-0.1.1/indiek/core/items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/indiek_core.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1125 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      276 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-04-17 01:36:04.000000 indiek-core-0.1.1/indiek_core.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-04-17 01:36:04.626090 indiek-core-0.1.1/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      840 2023-04-17 01:24:55.000000 indiek-core-0.1.1/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-04-17 01:36:04.626090 indiek-core-0.1.1/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      689 2023-04-16 01:50:53.000000 indiek-core-0.1.1/tests/test_items.py
```

### Comparing `indiek-core-0.1.0/LICENSE` & `indiek-core-0.1.1/LICENSE`

 * *Files identical despite different names*

