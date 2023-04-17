# Comparing `tmp/cf_wesgrh-0.1.tar.gz` & `tmp/cf_wesgrh-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_wesgrh-0.1.tar", last modified: Mon Apr 17 17:08:48 2023, max compression
+gzip compressed data, was "cf_wesgrh-0.2.tar", last modified: Mon Apr 17 17:38:59 2023, max compression
```

## Comparing `cf_wesgrh-0.1.tar` & `cf_wesgrh-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 17:08:48.603659 cf_wesgrh-0.1/
--rw-rw-rw-   0        0        0      138 2023-04-17 17:08:48.603659 cf_wesgrh-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 17:08:48.556841 cf_wesgrh-0.1/cf_wesgrh/
--rw-rw-rw-   0        0        0       23 2023-04-17 16:46:50.000000 cf_wesgrh-0.1/cf_wesgrh/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 17:08:48.603659 cf_wesgrh-0.1/cf_wesgrh.egg-info/
--rw-rw-rw-   0        0        0      138 2023-04-17 17:08:48.000000 cf_wesgrh-0.1/cf_wesgrh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-17 17:08:48.000000 cf_wesgrh-0.1/cf_wesgrh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 17:08:48.000000 cf_wesgrh-0.1/cf_wesgrh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 17:08:48.000000 cf_wesgrh-0.1/cf_wesgrh.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-17 17:08:48.000000 cf_wesgrh-0.1/cf_wesgrh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 17:08:48.603659 cf_wesgrh-0.1/setup.cfg
--rw-rw-rw-   0        0        0      235 2023-04-17 17:07:48.000000 cf_wesgrh-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:38:59.193602 cf_wesgrh-0.2/
+-rw-rw-rw-   0        0        0      138 2023-04-17 17:38:59.193602 cf_wesgrh-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 17:38:59.162348 cf_wesgrh-0.2/cf_wesgrh/
+-rw-rw-rw-   0        0        0       36 2023-04-17 17:36:55.000000 cf_wesgrh-0.2/cf_wesgrh/_init_.py
+-rw-rw-rw-   0        0        0       23 2023-04-17 17:36:55.000000 cf_wesgrh-0.2/cf_wesgrh/cf_wesgrh.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:38:59.193602 cf_wesgrh-0.2/cf_wesgrh.egg-info/
+-rw-rw-rw-   0        0        0      138 2023-04-17 17:38:58.000000 cf_wesgrh-0.2/cf_wesgrh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-04-17 17:38:59.000000 cf_wesgrh-0.2/cf_wesgrh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:38:58.000000 cf_wesgrh-0.2/cf_wesgrh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 17:08:48.000000 cf_wesgrh-0.2/cf_wesgrh.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-04-17 17:38:59.000000 cf_wesgrh-0.2/cf_wesgrh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:38:59.193602 cf_wesgrh-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      235 2023-04-17 17:36:55.000000 cf_wesgrh-0.2/setup.py
```

