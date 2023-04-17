# Comparing `tmp/vhdx_2_zvol-0.4.4.2.tar.gz` & `tmp/vhdx_2_zvol-0.4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.4.4.2.tar", last modified: Mon Apr 17 03:09:55 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.4.3.tar", last modified: Mon Apr 17 03:20:45 2023, max compression
```

## Comparing `vhdx_2_zvol-0.4.4.2.tar` & `vhdx_2_zvol-0.4.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-17 03:09:51.000000 vhdx_2_zvol-0.4.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10795 2023-04-17 03:09:43.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:20:45.940074 vhdx_2_zvol-0.4.4.3/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 03:20:45.940074 vhdx_2_zvol-0.4.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 03:20:45.940074 vhdx_2_zvol-0.4.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-17 03:20:41.000000 vhdx_2_zvol-0.4.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:20:45.936074 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10719 2023-04-17 03:20:28.000000 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:20:45.936074 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 03:20:45.000000 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 03:20:45.000000 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 03:20:45.000000 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 03:20:45.000000 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 03:20:45.000000 vhdx_2_zvol-0.4.4.3/vhdx_2_zvol.egg-info/top_level.txt
```

### Comparing `vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/main.py` & `vhdx_2_zvol-0.4.4.3/vhdx_2_zvol/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import argparse
 import logging
 import os
 import shutil
 import subprocess
 
 # Logging configuration
+
 logging.basicConfig(
     format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
 )
 logger = logging.getLogger(__name__)
 
-
 def try_except(func):
     def wrapper(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
             logging.error(f"An error occurred: {e}")
             return False
@@ -232,23 +232,19 @@
                 subprocess.run(['zfs', 'create', '-V', str(qcow_size), zvol_name])
                 logging.info("ZVOL conversion successful.")
         except subprocess.CalledProcessError as e:
             logging.error(f"Failed to create ZVOL: {e}")
             return False
     else:
         logger.error('Failed to get QCOW2 size.')
-    
-    # dd data from QCOW2 to ZVOL
-    
-    # Example usage:
-    mountpoint = get_zfs_mountpoint(zvol_name)
-    
+
+    mountpoint = get_zfs_mountpoint(zpool)
     if mountpoint:
         mountpoint = mountpoint + f"/{zvol}"
-        logger.debug(f'The mountpoint for dataset {zvol_name} is: {mountpoint}')
+        logger.debug(f'The mountpoint for dataset {zpool} is: {mountpoint}')
     else:
         logger.error(f'Failed to get mountpoint for dataset {zvol_name}.')
         return
 
     try:
         output = subprocess.check_output(
             ['dd', f'if={qcow2_path}', f'of={mountpoint}'],
```

