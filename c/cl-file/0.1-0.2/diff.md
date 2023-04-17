# Comparing `tmp/cl_file-0.1.tar.gz` & `tmp/cl_file-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cl_file-0.1.tar", last modified: Mon Apr 17 16:40:25 2023, max compression
+gzip compressed data, was "cl_file-0.2.tar", last modified: Mon Apr 17 17:39:13 2023, max compression
```

## Comparing `cl_file-0.1.tar` & `cl_file-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:25.074711 cl_file-0.1/
--rw-rw-rw-   0        0        0      148 2023-04-17 16:40:25.077717 cl_file-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:25.047306 cl_file-0.1/cl_file/
--rw-rw-rw-   0        0        0       23 2023-04-17 16:39:00.000000 cl_file-0.1/cl_file/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:25.070511 cl_file-0.1/cl_file.egg-info/
--rw-rw-rw-   0        0        0      148 2023-04-17 16:40:24.000000 cl_file-0.1/cl_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-04-17 16:40:24.000000 cl_file-0.1/cl_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:40:24.000000 cl_file-0.1/cl_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:40:24.000000 cl_file-0.1/cl_file.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-04-17 16:40:24.000000 cl_file-0.1/cl_file.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 16:40:25.080757 cl_file-0.1/setup.cfg
--rw-rw-rw-   0        0        0      243 2023-04-17 16:29:44.000000 cl_file-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:13.842006 cl_file-0.2/
+-rw-rw-rw-   0        0        0      148 2023-04-17 17:39:13.843003 cl_file-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:13.806083 cl_file-0.2/cl_file/
+-rw-rw-rw-   0        0        0       35 2023-04-17 17:35:41.000000 cl_file-0.2/cl_file/_init_.py
+-rw-rw-rw-   0        0        0       23 2023-04-17 17:35:41.000000 cl_file-0.2/cl_file/class_file.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:39:13.835025 cl_file-0.2/cl_file.egg-info/
+-rw-rw-rw-   0        0        0      148 2023-04-17 17:39:13.000000 cl_file-0.2/cl_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-17 17:39:13.000000 cl_file-0.2/cl_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:39:13.000000 cl_file-0.2/cl_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 16:40:24.000000 cl_file-0.2/cl_file.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-04-17 17:39:13.000000 cl_file-0.2/cl_file.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:39:13.850501 cl_file-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      245 2023-04-17 17:35:41.000000 cl_file-0.2/setup.py
```

