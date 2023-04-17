# Comparing `tmp/class_files-0.1.tar.gz` & `tmp/class_files-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_files-0.1.tar", last modified: Mon Apr 17 16:40:12 2023, max compression
+gzip compressed data, was "class_files-0.2.tar", last modified: Mon Apr 17 17:39:02 2023, max compression
```

## Comparing `class_files-0.1.tar` & `class_files-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:12.400806 class_files-0.1/
--rw-rw-rw-   0        0        0      170 2023-04-17 16:40:12.400806 class_files-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:12.362820 class_files-0.1/class_files/
--rw-rw-rw-   0        0        0       90 2023-04-17 16:36:38.000000 class_files-0.1/class_files/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:12.398808 class_files-0.1/class_files.egg-info/
--rw-rw-rw-   0        0        0      170 2023-04-17 16:40:12.000000 class_files-0.1/class_files.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-04-17 16:40:12.000000 class_files-0.1/class_files.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:40:12.000000 class_files-0.1/class_files.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:40:12.000000 class_files-0.1/class_files.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-04-17 16:40:12.000000 class_files-0.1/class_files.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 16:40:12.403806 class_files-0.1/setup.cfg
--rw-rw-rw-   0        0        0      271 2023-04-17 16:28:12.000000 class_files-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:02.967002 class_files-0.2/
+-rw-rw-rw-   0        0        0      170 2023-04-17 17:39:02.967002 class_files-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:02.938011 class_files-0.2/class_files/
+-rw-rw-rw-   0        0        0       51 2023-04-17 17:30:55.000000 class_files-0.2/class_files/_init_.py
+-rw-rw-rw-   0        0        0       44 2023-04-17 17:30:55.000000 class_files-0.2/class_files/class_file.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:02.966002 class_files-0.2/class_files.egg-info/
+-rw-rw-rw-   0        0        0      170 2023-04-17 17:39:02.000000 class_files-0.2/class_files.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-17 17:39:02.000000 class_files-0.2/class_files.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:39:02.000000 class_files-0.2/class_files.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 16:40:12.000000 class_files-0.2/class_files.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-04-17 17:39:02.000000 class_files-0.2/class_files.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:39:02.974000 class_files-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      269 2023-04-17 17:35:07.000000 class_files-0.2/setup.py
```

