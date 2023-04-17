# Comparing `tmp/y_class_files-0.1.tar.gz` & `tmp/y_class_files-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y_class_files-0.1.tar", last modified: Mon Apr 17 16:43:43 2023, max compression
+gzip compressed data, was "y_class_files-0.2.tar", last modified: Mon Apr 17 17:39:10 2023, max compression
```

## Comparing `y_class_files-0.1.tar` & `y_class_files-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:43:43.757028 y_class_files-0.1/
--rw-rw-rw-   0        0        0      131 2023-04-17 16:43:43.757028 y_class_files-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-17 16:43:43.757028 y_class_files-0.1/setup.cfg
--rw-rw-rw-   0        0        0      232 2023-04-17 16:29:43.000000 y_class_files-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:43:43.757028 y_class_files-0.1/y_class_files/
--rw-rw-rw-   0        0        0       25 2023-04-17 16:39:01.000000 y_class_files-0.1/y_class_files/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:43:43.757028 y_class_files-0.1/y_class_files.egg-info/
--rw-rw-rw-   0        0        0      131 2023-04-17 16:43:43.000000 y_class_files-0.1/y_class_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-04-17 16:43:43.000000 y_class_files-0.1/y_class_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:43:43.000000 y_class_files-0.1/y_class_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:40:27.000000 y_class_files-0.1/y_class_files.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-04-17 16:43:43.000000 y_class_files-0.1/y_class_files.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:10.489217 y_class_files-0.2/
+-rw-rw-rw-   0        0        0      131 2023-04-17 17:39:10.489217 y_class_files-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:39:10.489217 y_class_files-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      232 2023-04-17 17:35:26.000000 y_class_files-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:10.473593 y_class_files-0.2/y_class_files/
+-rw-rw-rw-   0        0        0       34 2023-04-17 17:35:26.000000 y_class_files-0.2/y_class_files/_init_.py
+-rw-rw-rw-   0        0        0       23 2023-04-17 17:35:26.000000 y_class_files-0.2/y_class_files/y_class_file.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:10.489217 y_class_files-0.2/y_class_files.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-04-17 17:39:10.000000 y_class_files-0.2/y_class_files.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-17 17:39:10.000000 y_class_files-0.2/y_class_files.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:39:10.000000 y_class_files-0.2/y_class_files.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 16:40:27.000000 y_class_files-0.2/y_class_files.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-04-17 17:39:10.000000 y_class_files-0.2/y_class_files.egg-info/top_level.txt
```

