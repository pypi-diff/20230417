# Comparing `tmp/blue_engine-0.1.tar.gz` & `tmp/blue_engine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_engine-0.1.tar", last modified: Mon Apr 17 12:49:32 2023, max compression
+gzip compressed data, was "blue_engine-0.1.1.tar", last modified: Mon Apr 17 13:54:29 2023, max compression
```

## Comparing `blue_engine-0.1.tar` & `blue_engine-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:49:32.150585 blue_engine-0.1/
--rw-rw-rw-   0        0        0     1072 2023-04-17 12:40:47.000000 blue_engine-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      217 2023-04-17 12:49:32.151585 blue_engine-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-17 12:26:22.000000 blue_engine-0.1/README.rst
--rw-rw-rw-   0        0        0      115 2023-04-17 12:49:32.161588 blue_engine-0.1/setup.cfg
--rw-rw-rw-   0        0        0      248 2023-04-17 12:39:01.000000 blue_engine-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:49:32.092570 blue_engine-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 12:49:32.148587 blue_engine-0.1/src/blue_engine.egg-info/
--rw-rw-rw-   0        0        0      217 2023-04-17 12:49:31.000000 blue_engine-0.1/src/blue_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-17 12:49:31.000000 blue_engine-0.1/src/blue_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:49:31.000000 blue_engine-0.1/src/blue_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:49:31.000000 blue_engine-0.1/src/blue_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 13:54:29.409892 blue_engine-0.1.1/
+-rw-rw-rw-   0        0        0     1072 2023-04-17 12:40:47.000000 blue_engine-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      219 2023-04-17 13:54:29.409892 blue_engine-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:26:22.000000 blue_engine-0.1.1/README.rst
+-rw-rw-rw-   0        0        0      115 2023-04-17 13:54:29.423898 blue_engine-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      329 2023-04-17 13:54:13.000000 blue_engine-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 13:54:29.324870 blue_engine-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 13:54:29.404892 blue_engine-0.1.1/src/blue_engine.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-04-17 13:54:29.000000 blue_engine-0.1.1/src/blue_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-17 13:54:29.000000 blue_engine-0.1.1/src/blue_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:54:29.000000 blue_engine-0.1.1/src/blue_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 13:54:29.000000 blue_engine-0.1.1/src/blue_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 13:54:29.000000 blue_engine-0.1.1/src/blue_engine.egg-info/top_level.txt
```

### Comparing `blue_engine-0.1/LICENSE.txt` & `blue_engine-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

