# Comparing `tmp/vhdx_2_zvol-0.4.4.1.tar.gz` & `tmp/vhdx_2_zvol-0.4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.4.4.1.tar", last modified: Mon Apr 17 02:55:53 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.4.2.tar", last modified: Mon Apr 17 03:09:55 2023, max compression
```

## Comparing `vhdx_2_zvol-0.4.4.1.tar` & `vhdx_2_zvol-0.4.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-17 02:54:20.000000 vhdx_2_zvol-0.4.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9969 2023-04-17 02:53:07.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:55:53.297984 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:55:53.000000 vhdx_2_zvol-0.4.4.1/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      284 2023-04-17 03:09:51.000000 vhdx_2_zvol-0.4.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10795 2023-04-17 03:09:43.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:09:55.699544 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 03:09:55.000000 vhdx_2_zvol-0.4.4.2/vhdx_2_zvol.egg-info/top_level.txt
```

### Comparing `vhdx_2_zvol-0.4.4.1/vhdx_2_zvol/main.py` & `vhdx_2_zvol-0.4.4.2/vhdx_2_zvol/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,14 +54,28 @@
 
     except Exception as e:
         
         logger.error(f'Error getting QCOW2 size: {e}')
         logger.error(f'Output: {output}')
         return None
 
+import subprocess
+
+def get_zfs_mountpoint(dataset):
+    try:
+        # Execute the zfs command and capture the output
+        output = subprocess.check_output(['zfs', 'get', '-H', '-o', 'value', 'mountpoint', dataset], universal_newlines=True)
+        # Extract the mountpoint from the output
+        mountpoint = output.strip()
+        return mountpoint
+    except subprocess.CalledProcessError as e:
+        logger.error(f'Error getting mountpoint for dataset {dataset}: {e}')
+        return None
+
+
 
 def parse_args():
     import sys
 
     script_name = sys.argv[0]
     parser = argparse.ArgumentParser(
         description="Convert Hyper-V VHDX files to QCOW2 format and further convert"
@@ -220,17 +234,28 @@
         except subprocess.CalledProcessError as e:
             logging.error(f"Failed to create ZVOL: {e}")
             return False
     else:
         logger.error('Failed to get QCOW2 size.')
     
     # dd data from QCOW2 to ZVOL
+    
+    # Example usage:
+    mountpoint = get_zfs_mountpoint(zvol_name)
+    
+    if mountpoint:
+        mountpoint = mountpoint + f"/{zvol}"
+        logger.debug(f'The mountpoint for dataset {zvol_name} is: {mountpoint}')
+    else:
+        logger.error(f'Failed to get mountpoint for dataset {zvol_name}.')
+        return
+
     try:
         output = subprocess.check_output(
-            ['dd', f'if={qcow2_path}', f'of={zvol_name}'],
+            ['dd', f'if={qcow2_path}', f'of={mountpoint}'],
             stderr=subprocess.STDOUT,
             universal_newlines=True,
         )
         logging.info(
             f"Successfully converted QCOW2 file '{qcow2_path}' to ZVOL dataset '{zvol_name}'"
         )
         return True
```

