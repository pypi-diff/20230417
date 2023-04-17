# Comparing `tmp/libds-0.1.tar.gz` & `tmp/libds-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libds-0.1.tar", last modified: Mon Apr 17 12:40:04 2023, max compression
+gzip compressed data, was "libds-0.2.tar", last modified: Mon Apr 17 12:57:04 2023, max compression
```

## Comparing `libds-0.1.tar` & `libds-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:40:04.305005 libds-0.1/
--rw-rw-rw-   0        0        0      373 2023-04-17 12:40:04.305005 libds-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 12:40:04.304008 libds-0.1/libds.egg-info/
--rw-rw-rw-   0        0        0      373 2023-04-17 12:40:04.000000 libds-0.1/libds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-04-17 12:40:04.000000 libds-0.1/libds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:40:04.000000 libds-0.1/libds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:40:04.000000 libds-0.1/libds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 12:40:04.306001 libds-0.1/setup.cfg
--rw-rw-rw-   0        0        0      497 2023-04-17 12:39:15.000000 libds-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:57:04.636716 libds-0.2/
+-rw-rw-rw-   0        0        0      373 2023-04-17 12:57:04.635718 libds-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 12:57:04.634721 libds-0.2/libds.egg-info/
+-rw-rw-rw-   0        0        0      373 2023-04-17 12:57:04.000000 libds-0.2/libds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-04-17 12:57:04.000000 libds-0.2/libds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 12:57:04.000000 libds-0.2/libds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 12:57:04.000000 libds-0.2/libds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 12:57:04.636716 libds-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-04-17 12:56:41.000000 libds-0.2/setup.py
```

