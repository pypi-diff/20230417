# Comparing `tmp/glinux-boot-image-kthresher-0.0.1.tar.gz` & `tmp/glinux-boot-image-kthresher-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glinux-boot-image-kthresher-0.0.1.tar", last modified: Mon Apr 17 00:26:38 2023, max compression
+gzip compressed data, was "glinux-boot-image-kthresher-0.0.2.tar", last modified: Mon Apr 17 01:45:50 2023, max compression
```

## Comparing `glinux-boot-image-kthresher-0.0.1.tar` & `glinux-boot-image-kthresher-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 00:26:38.605697 glinux-boot-image-kthresher-0.0.1/
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      754 2023-04-17 00:26:38.605697 glinux-boot-image-kthresher-0.0.1/PKG-INFO
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       63 2023-04-17 00:20:24.973022 glinux-boot-image-kthresher-0.0.1/setup.cfg
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1594 2023-04-17 00:25:54.996750 glinux-boot-image-kthresher-0.0.1/setup.py
+drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 01:45:50.662993 glinux-boot-image-kthresher-0.0.2/
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      536 2023-04-17 01:45:50.662993 glinux-boot-image-kthresher-0.0.2/PKG-INFO
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       33 2023-04-17 01:41:00.442723 glinux-boot-image-kthresher-0.0.2/setup.cfg
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1109 2023-04-17 01:45:49.206972 glinux-boot-image-kthresher-0.0.2/setup.py
```

