# Comparing `tmp/vhdx_2_zvol-0.4.2.tar.gz` & `tmp/vhdx_2_zvol-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.4.2.tar", last modified: Mon Apr 17 02:20:34 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.3.tar", last modified: Mon Apr 17 02:37:17 2023, max compression
```

## Comparing `vhdx_2_zvol-0.4.2.tar` & `vhdx_2_zvol-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:19:54.000000 vhdx_2_zvol-0.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/vhdx_2_zvol/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9899 2023-04-17 02:19:27.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:20:34.537881 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:20:34.000000 vhdx_2_zvol-0.4.2/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:37:17.335898 vhdx_2_zvol-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:37:17.335898 vhdx_2_zvol-0.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:37:17.335898 vhdx_2_zvol-0.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:37:12.000000 vhdx_2_zvol-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:37:17.331897 vhdx_2_zvol-0.4.3/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9969 2023-04-17 02:36:39.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:37:17.331897 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:37:17.000000 vhdx_2_zvol-0.4.3/vhdx_2_zvol.egg-info/top_level.txt
```

### Comparing `vhdx_2_zvol-0.4.2/vhdx_2_zvol/main.py` & `vhdx_2_zvol-0.4.3/vhdx_2_zvol/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         output = subprocess.check_output(['qemu-img', 'info', qcow_path])
         output = output.decode('utf-8')
 
         # Extract the virtual size from the output
         size_line = next(line for line in output.split('\n') if 'virtual size' in line)
         size_parts = size_line.split(':')
         size = size_parts[1].strip()
+        if "(" in size:
+            size = size.split("(")[0].strip()
 
         # Extract the size value and unit
         size_value, size_unit = size.split()
         size_value = int(size_value)
 
         # Convert size to bytes based on the unit
         if size_unit == 'KiB':
```

