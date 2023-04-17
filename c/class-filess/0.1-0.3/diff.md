# Comparing `tmp/class_filess-0.1.tar.gz` & `tmp/class_filess-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "class_filess-0.1.tar", last modified: Mon Apr 17 16:46:46 2023, max compression
+gzip compressed data, was "class_filess-0.3.tar", last modified: Mon Apr 17 17:59:21 2023, max compression
```

## Comparing `class_filess-0.1.tar` & `class_filess-0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:46:46.224506 class_filess-0.1/
--rw-rw-rw-   0        0        0      237 2023-04-17 16:46:46.224506 class_filess-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 16:46:46.172519 class_filess-0.1/class_filess/
--rw-rw-rw-   0        0        0       31 2023-04-17 16:38:27.000000 class_filess-0.1/class_filess/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:46:46.221507 class_filess-0.1/class_filess.egg-info/
--rw-rw-rw-   0        0        0      237 2023-04-17 16:46:45.000000 class_filess-0.1/class_filess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-17 16:46:46.000000 class_filess-0.1/class_filess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:46:46.000000 class_filess-0.1/class_filess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:46:46.000000 class_filess-0.1/class_filess.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-04-17 16:46:46.000000 class_filess-0.1/class_filess.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 16:46:46.228505 class_filess-0.1/setup.cfg
--rw-rw-rw-   0        0        0      267 2023-04-17 16:44:31.000000 class_filess-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:59:21.146935 class_filess-0.3/
+-rw-rw-rw-   0        0        0      167 2023-04-17 17:59:21.146935 class_filess-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 17:59:21.078951 class_filess-0.3/class_filess/
+-rw-rw-rw-   0        0        0       35 2023-04-17 17:59:08.000000 class_filess-0.3/class_filess/_init_.py
+-rw-rw-rw-   0        0        0       23 2023-04-17 17:31:29.000000 class_filess-0.3/class_filess/class_files.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:59:21.143935 class_filess-0.3/class_filess.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-04-17 17:59:20.000000 class_filess-0.3/class_filess.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-04-17 17:59:20.000000 class_filess-0.3/class_filess.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:59:20.000000 class_filess-0.3/class_filess.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 17:53:17.000000 class_filess-0.3/class_filess.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-04-17 17:59:20.000000 class_filess-0.3/class_filess.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:59:21.161933 class_filess-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      267 2023-04-17 17:59:08.000000 class_filess-0.3/setup.py
```

