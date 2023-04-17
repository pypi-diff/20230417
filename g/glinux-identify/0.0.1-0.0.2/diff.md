# Comparing `tmp/glinux-identify-0.0.1.tar.gz` & `tmp/glinux-identify-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glinux-identify-0.0.1.tar", last modified: Mon Apr 17 00:29:19 2023, max compression
+gzip compressed data, was "glinux-identify-0.0.2.tar", last modified: Mon Apr 17 01:43:38 2023, max compression
```

## Comparing `glinux-identify-0.0.1.tar` & `glinux-identify-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 00:29:19.864642 glinux-identify-0.0.1/
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      742 2023-04-17 00:29:19.864642 glinux-identify-0.0.1/PKG-INFO
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       63 2023-04-17 00:20:24.973022 glinux-identify-0.0.1/setup.cfg
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1570 2023-04-17 00:29:00.616327 glinux-identify-0.0.1/setup.py
+drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 01:43:38.653060 glinux-identify-0.0.2/
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      524 2023-04-17 01:43:38.653060 glinux-identify-0.0.2/PKG-INFO
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       33 2023-04-17 01:41:00.442723 glinux-identify-0.0.2/setup.cfg
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1085 2023-04-17 01:43:34.577000 glinux-identify-0.0.2/setup.py
```

