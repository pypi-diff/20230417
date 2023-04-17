# Comparing `tmp/vhdx_2_zvol-0.4.tar.gz` & `tmp/vhdx_2_zvol-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.4.tar", last modified: Sun Apr 16 18:28:07 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.1.tar", last modified: Mon Apr 17 02:05:11 2023, max compression
```

## Comparing `vhdx_2_zvol-0.4.tar` & `vhdx_2_zvol-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      280 2023-04-16 18:28:02.000000 vhdx_2_zvol-0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/vhdx_2_zvol/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4/vhdx_2_zvol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7631 2023-04-14 00:22:46.000000 vhdx_2_zvol-0.4/vhdx_2_zvol/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-17 02:03:57.000000 vhdx_2_zvol-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9839 2023-04-17 02:03:01.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 02:05:11.883578 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-17 02:05:11.000000 vhdx_2_zvol-0.4.1/vhdx_2_zvol.egg-info/top_level.txt
```

### Comparing `vhdx_2_zvol-0.4/vhdx_2_zvol/main.py` & `vhdx_2_zvol-0.4.1/vhdx_2_zvol/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,45 @@
         try:
             return func(*args, **kwargs)
         except Exception as e:
             logging.error(f"An error occurred: {e}")
             return False
 
     return wrapper
+def get_qcow_size(qcow_path):
+    """Get size of QCOW2 file using qemu-img"""
+    try:
+        # Run qemu-img info command to get size
+        output = subprocess.check_output(['qemu-img', 'info', qcow_path])
+        output = output.decode('utf-8')
+
+        # Extract the virtual size from the output
+        size_line = next(line for line in output.split('\n') if 'virtual size' in line)
+        size_parts = size_line.split(':')
+        size = size_parts[1].strip()
+
+        # Extract the size value and unit
+        size_value, size_unit = size.split()
+        size_value = int(size_value)
+
+        # Convert size to bytes based on the unit
+        if size_unit == 'KiB':
+            size_value *= 1024
+        elif size_unit == 'MiB':
+            size_value *= 1024 * 1024
+        elif size_unit == 'GiB':
+            size_value *= 1024 * 1024 * 1024
+        elif size_unit == 'TiB':
+            size_value *= 1024 * 1024 * 1024 * 1024
+
+        return size_value
+
+    except Exception as e:
+        print(f'Error getting QCOW2 size: {e}')
+        return None
 
 
 def parse_args():
     import sys
 
     script_name = sys.argv[0]
     parser = argparse.ArgumentParser(
@@ -146,39 +177,67 @@
     Args:
         qcow2_path (str): Path to the QCOW2 file.
         zpool (str): Name of the ZFS pool.
         zvol (str): Name of the ZVOL dataset.
 
     Returns:
         bool: True if conversion is successful, False otherwise.
+
     """
+    logger.debug("Get QCOW file size")
+    qcow_size = get_qcow_size(qcow2_path)
+    zvol_name = f"{zpool}/{zvol}"
+    if qcow_size is None:
+        logging.error(f"Failed to get QCOW file size: {qcow2_path}")
+        return False
+
     logging.info(
-        f"Converting QCOW2 file '{qcow2_path}' to ZVOL dataset '{zpool}/{zvol}'"
+        f"Converting QCOW2 file '{qcow2_path}' to ZVOL dataset '{zvol_name}'"
     )
 
     # Check if zvol command is present in the os PATH
     if not shutil.which("zfs"):
         logging.error(
             "zvol command not found in os PATH. Please ensure that the zvol"
             + " command is installed and available in the PATH."
         )
         return False
-
-    # Construct the zvol command
-    zvol_cmd = f"zfs create {zpool}/{zvol} {qcow2_path}"
-
-    # Run the zvol command
+    if zvol_size is not None:
+    # Create ZFS zvol with the obtained size
+        try:
+            output = subprocess.check_output(['zfs', 'list', '-t', 'volume', '-o', 'name'])
+            zvol_list = output.decode('utf-8').split()
+            if zvol_name in zvol_list:
+                logger.info(f'ZFS zvol "{zvol_name}" already exists. Skipping creation.')
+            else:
+                subprocess.run(['zfs', 'create', '-V', str(zvol_size), zvol_name])
+                logging.info("ZVOL conversion successful.")
+        except subprocess.CalledProcessError as e:
+            logging.error(f"Failed to create ZVOL: {e}")
+            return False
+    else:
+        logger.error('Failed to get QCOW2 size.')
+    
+    # dd data from QCOW2 to ZVOL
     try:
-        subprocess.run(zvol_cmd, shell=True, check=True)
-        logging.info("ZVOL conversion successful.")
+        output = subprocess.check_output(
+            ['dd', f'if={qcow2_path}', f'of={zvol_name}'],
+            stderr=subprocess.STDOUT,
+            universal_newlines=True,
+        )
+        logging.info(
+            f"Successfully converted QCOW2 file '{qcow2_path}' to ZVOL dataset '{zvol_name}'"
+        )
         return True
     except subprocess.CalledProcessError as e:
-        logging.error(f"Failed to convert QCOW2 to ZVOL: {e}")
+        logging.error(
+            f"Failed to convert QCOW2 file '{qcow2_path}' to ZVOL dataset '{zvol_name}'. Error: {e}"
+        )
         return False
-
+    
 
 @try_except
 def remove_file(file_path):
     """
     Removes a file from the file system.
 
     Args:
```

