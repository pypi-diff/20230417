# Comparing `tmp/vhdx_2_zvol-0.4.1.tar.gz` & `tmp/vhdx_2_zvol-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.4.1.tar", last modified: Mon Apr 17 02:05:11 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.2.tar", last modified: Mon Apr 17 02:20:34 2023, max compression
```

## Comparing `vhdx_2_zvol-0.4.1.tar` & `vhdx_2_zvol-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:03:57.000000 vhdx_2_zvol-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/vhdx_2_zvol/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9839 2023-04-17 02:03:01.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:19:54.000000 vhdx_2_zvol-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9899 2023-04-17 02:19:27.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/top_level.txt
```

### Comparing `vhdx_2_zvol-0.4.1/vhdx_2_zvol/main.py` & `vhdx_2_zvol-0.4.2/vhdx_2_zvol/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         try:
             return func(*args, **kwargs)
         except Exception as e:
             logging.error(f"An error occurred: {e}")
             return False
 
     return wrapper
+
+
 def get_qcow_size(qcow_path):
     """Get size of QCOW2 file using qemu-img"""
     try:
         # Run qemu-img info command to get size
         output = subprocess.check_output(['qemu-img', 'info', qcow_path])
         output = output.decode('utf-8')
 
@@ -45,15 +47,17 @@
             size_value *= 1024 * 1024 * 1024
         elif size_unit == 'TiB':
             size_value *= 1024 * 1024 * 1024 * 1024
 
         return size_value
 
     except Exception as e:
-        print(f'Error getting QCOW2 size: {e}')
+        
+        logger.error(f'Error getting QCOW2 size: {e}')
+        logger.error(f'Output: {output}')
         return None
 
 
 def parse_args():
     import sys
 
     script_name = sys.argv[0]
```

