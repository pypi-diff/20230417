# Comparing `tmp/y_class_files-0.3.tar.gz` & `tmp/y_class_files-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y_class_files-0.3.tar", last modified: Mon Apr 17 17:57:45 2023, max compression
+gzip compressed data, was "y_class_files-0.4.tar", last modified: Mon Apr 17 18:12:29 2023, max compression
```

## Comparing `y_class_files-0.3.tar` & `y_class_files-0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 17:57:45.437966 y_class_files-0.3/
--rw-rw-rw-   0        0        0      131 2023-04-17 17:57:45.437966 y_class_files-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-17 17:57:45.437966 y_class_files-0.3/setup.cfg
--rw-rw-rw-   0        0        0      232 2023-04-17 17:57:34.000000 y_class_files-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:57:45.422343 y_class_files-0.3/y_class_files/
--rw-rw-rw-   0        0        0       31 2023-04-17 17:57:34.000000 y_class_files-0.3/y_class_files/_init_.py
--rw-rw-rw-   0        0        0     5442 2023-03-29 18:03:52.000000 y_class_files-0.3/y_class_files/class_files.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:57:45.437966 y_class_files-0.3/y_class_files.egg-info/
--rw-rw-rw-   0        0        0      131 2023-04-17 17:57:45.000000 y_class_files-0.3/y_class_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-17 17:57:45.000000 y_class_files-0.3/y_class_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 17:57:45.000000 y_class_files-0.3/y_class_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:40:27.000000 y_class_files-0.3/y_class_files.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-04-17 17:57:45.000000 y_class_files-0.3/y_class_files.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 18:12:29.347730 y_class_files-0.4/
+-rw-rw-rw-   0        0        0      131 2023-04-17 18:12:29.347730 y_class_files-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-17 18:12:29.347730 y_class_files-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      232 2023-04-17 18:09:19.000000 y_class_files-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:12:29.347730 y_class_files-0.4/y_class_files/
+-rw-rw-rw-   0        0        0       31 2023-04-17 17:57:34.000000 y_class_files-0.4/y_class_files/_init_.py
+-rw-rw-rw-   0        0        0     5442 2023-03-29 18:03:52.000000 y_class_files-0.4/y_class_files/class_files.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:12:29.347730 y_class_files-0.4/y_class_files.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-04-17 18:12:29.000000 y_class_files-0.4/y_class_files.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-17 18:12:29.000000 y_class_files-0.4/y_class_files.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:12:29.000000 y_class_files-0.4/y_class_files.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 16:40:27.000000 y_class_files-0.4/y_class_files.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-17 18:12:29.000000 y_class_files-0.4/y_class_files.egg-info/top_level.txt
```

### Comparing `y_class_files-0.3/y_class_files/class_files.py` & `y_class_files-0.4/y_class_files/class_files.py`

 * *Files identical despite different names*

