# Comparing `tmp/vhdx_2_zvol-0.4.3.tar.gz` & `tmp/vhdx_2_zvol-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.4.3.tar", last modified: Mon Apr 17 02:37:17 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.4.tar", last modified: Mon Apr 17 02:43:43 2023, max compression
```

## Comparing `vhdx_2_zvol-0.4.3.tar` & `vhdx_2_zvol-0.4.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:37:17.335898 vhdx_2_zvol-0.4.3/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:37:17.335898 vhdx_2_zvol-0.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:37:17.335898 vhdx_2_zvol-0.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:37:12.000000 vhdx_2_zvol-0.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:37:17.331897 vhdx_2_zvol-0.4.3/vhdx_2_zvol/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9969 2023-04-17 02:36:39.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:37:17.331897 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:43:22.000000 vhdx_2_zvol-0.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9969 2023-04-17 02:42:49.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:43:43.284625 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:43:43.000000 vhdx_2_zvol-0.4.4/vhdx_2_zvol.egg-info/top_level.txt
```

### Comparing `vhdx_2_zvol-0.4.3/vhdx_2_zvol/main.py` & `vhdx_2_zvol-0.4.4/vhdx_2_zvol/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,23 +203,23 @@
     # Check if zvol command is present in the os PATH
     if not shutil.which("zfs"):
         logging.error(
             "zvol command not found in os PATH. Please ensure that the zvol"
             + " command is installed and available in the PATH."
         )
         return False
-    if zvol_size is not None:
+    if qcow_size is not None:
     # Create ZFS zvol with the obtained size
         try:
             output = subprocess.check_output(['zfs', 'list', '-t', 'volume', '-o', 'name'])
             zvol_list = output.decode('utf-8').split()
             if zvol_name in zvol_list:
                 logger.info(f'ZFS zvol "{zvol_name}" already exists. Skipping creation.')
             else:
-                subprocess.run(['zfs', 'create', '-V', str(zvol_size), zvol_name])
+                subprocess.run(['zfs', 'create', '-V', str(qcow_size), zvol_name])
                 logging.info("ZVOL conversion successful.")
         except subprocess.CalledProcessError as e:
             logging.error(f"Failed to create ZVOL: {e}")
             return False
     else:
         logger.error('Failed to get QCOW2 size.')
```

