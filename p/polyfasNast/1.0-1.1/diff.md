# Comparing `tmp/polyfasNast-1.0.tar.gz` & `tmp/polyfasNast-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfasNast-1.0.tar", last modified: Mon Apr 17 16:40:23 2023, max compression
+gzip compressed data, was "polyfasNast-1.1.tar", last modified: Mon Apr 17 17:36:08 2023, max compression
```

## Comparing `polyfasNast-1.0.tar` & `polyfasNast-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:23.796766 polyfasNast-1.0/
--rw-rw-rw-   0        0        0      152 2023-04-17 16:40:23.796766 polyfasNast-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:23.773258 polyfasNast-1.0/polyfasNast/
--rw-rw-rw-   0        0        0       38 2023-04-17 16:39:01.000000 polyfasNast-1.0/polyfasNast/_init_.py
-drwxrwxrwx   0        0        0        0 2023-04-17 16:40:23.792703 polyfasNast-1.0/polyfasNast.egg-info/
--rw-rw-rw-   0        0        0      152 2023-04-17 16:40:23.000000 polyfasNast-1.0/polyfasNast.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-04-17 16:40:23.000000 polyfasNast-1.0/polyfasNast.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 16:40:23.000000 polyfasNast-1.0/polyfasNast.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 16:40:23.000000 polyfasNast-1.0/polyfasNast.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-04-17 16:40:23.000000 polyfasNast-1.0/polyfasNast.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 16:40:23.799189 polyfasNast-1.0/setup.cfg
--rw-rw-rw-   0        0        0      251 2023-04-17 16:27:57.000000 polyfasNast-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:36:08.389733 polyfasNast-1.1/
+-rw-rw-rw-   0        0        0      152 2023-04-17 17:36:08.391033 polyfasNast-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-17 17:36:08.367409 polyfasNast-1.1/polyfasNast/
+-rw-rw-rw-   0        0        0       29 2023-04-17 17:33:19.000000 polyfasNast-1.1/polyfasNast/_init_.py
+-rw-rw-rw-   0        0        0       23 2023-04-17 17:31:10.000000 polyfasNast-1.1/polyfasNast/class_file.py
+drwxrwxrwx   0        0        0        0 2023-04-17 17:36:08.389733 polyfasNast-1.1/polyfasNast.egg-info/
+-rw-rw-rw-   0        0        0      152 2023-04-17 17:36:08.000000 polyfasNast-1.1/polyfasNast.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-04-17 17:36:08.000000 polyfasNast-1.1/polyfasNast.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 17:36:08.000000 polyfasNast-1.1/polyfasNast.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 16:40:23.000000 polyfasNast-1.1/polyfasNast.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-04-17 17:36:08.000000 polyfasNast-1.1/polyfasNast.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 17:36:08.391033 polyfasNast-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      251 2023-04-17 17:35:16.000000 polyfasNast-1.1/setup.py
```

