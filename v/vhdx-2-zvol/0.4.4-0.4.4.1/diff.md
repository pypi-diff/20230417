# Comparing `tmp/vhdx_2_zvol-0.4.4.tar.gz` & `tmp/vhdx_2_zvol-0.4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.4.4.tar", last modified: Mon Apr 17 02:43:43 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.4.1.tar", last modified: Mon Apr 17 02:55:53 2023, max compression
```

## Comparing `vhdx_2_zvol-0.4.4.tar` & `vhdx_2_zvol-0.4.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:43:22.000000 vhdx_2_zvol-0.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/vhdx_2_zvol/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9969 2023-04-17 02:42:49.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-17 02:54:20.000000 vhdx_2_zvol-0.4.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9969 2023-04-17 02:53:07.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/top_level.txt
```

### Comparing `vhdx_2_zvol-0.4.4/vhdx_2_zvol/main.py` & `vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         logging.error(
             f"Failed to convert VHDX to QCOW2: {vhdx_path} -> {qcow2_path}. Error: {e}"
         )
         return False
 
 
 @try_except
-def convert_qcow2_to_zvol(qcow2_path, zpool, zvol):
+def convert_qcow2_to_zvol(qcow2_path, zvol, zpool):
     """
     Convert QCOW2 file to ZVOL dataset in a specified ZFS pool.
 
     Args:
         qcow2_path (str): Path to the QCOW2 file.
         zpool (str): Name of the ZFS pool.
         zvol (str): Name of the ZVOL dataset.
```

