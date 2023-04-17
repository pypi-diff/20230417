# Comparing `tmp/bintropy-1.4.1.tar.gz` & `tmp/bintropy-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bintropy-1.4.1.tar", last modified: Mon Apr 17 15:40:24 2023, max compression
+gzip compressed data, was "bintropy-1.4.2.tar", last modified: Mon Apr 17 15:54:19 2023, max compression
```

## Comparing `bintropy-1.4.1.tar` & `bintropy-1.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.550435 bintropy-1.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-17 15:40:15.000000 bintropy-1.4.1/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-17 15:40:15.000000 bintropy-1.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 15:40:15.000000 bintropy-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:40:24.550435 bintropy-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-17 15:40:15.000000 bintropy-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-17 15:40:15.000000 bintropy-1.4.1/docs/example-not-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-17 15:40:15.000000 bintropy-1.4.1/docs/example-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-17 15:40:15.000000 bintropy-1.4.1/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-17 15:40:15.000000 bintropy-1.4.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       30 2023-04-17 15:40:15.000000 bintropy-1.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:40:24.550435 bintropy-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/src/bintropy/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23896 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-17 15:40:15.000000 bintropy-1.4.1/src/bintropy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:40:24.546435 bintropy-1.4.1/src/bintropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 15:40:24.000000 bintropy-1.4.1/src/bintropy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.549150 bintropy-1.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.541149 bintropy-1.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.541149 bintropy-1.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-17 15:54:09.000000 bintropy-1.4.2/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-17 15:54:09.000000 bintropy-1.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 15:54:09.000000 bintropy-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:54:19.549150 bintropy-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-17 15:54:09.000000 bintropy-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.545150 bintropy-1.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-17 15:54:09.000000 bintropy-1.4.2/docs/example-not-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-17 15:54:09.000000 bintropy-1.4.2/docs/example-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-17 15:54:09.000000 bintropy-1.4.2/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-17 15:54:09.000000 bintropy-1.4.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-17 15:54:09.000000 bintropy-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:54:19.549150 bintropy-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.541149 bintropy-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.545150 bintropy-1.4.2/src/bintropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.549150 bintropy-1.4.2/src/bintropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/top_level.txt
```

### Comparing `bintropy-1.4.1/.github/workflows/python-package.yml` & `bintropy-1.4.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/.gitignore` & `bintropy-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/LICENSE` & `bintropy-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/PKG-INFO` & `bintropy-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.1
+Version: 1.4.2
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bintropy-1.4.1/README.md` & `bintropy-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/docs/example-not-packed.png` & `bintropy-1.4.2/docs/example-not-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/docs/example-packed.png` & `bintropy-1.4.2/docs/example-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/docs/logo.png` & `bintropy-1.4.2/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/pyproject.toml` & `bintropy-1.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Security",
 ]
 dependencies = [
-  "lief",
+  "lief>=0.13.0",
   "matplotlib",
   "numpy>=1.23.0",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
```

### Comparing `bintropy-1.4.1/src/bintropy/__info__.py` & `bintropy-1.4.2/src/bintropy/__info__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/src/bintropy/__init__.py` & `bintropy-1.4.2/src/bintropy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,26 +71,26 @@
 
 
 def _get_ep_and_section(binary):
     """ Helper for computing the entry point and finding its section for each supported format.
     :param binary: LIEF-parsed binary object
     :return:       (ep_file_offset, name_of_ep_section)
     """
-    btype = str(type(binary)).split(".")[1]
+    btype = str(type(binary)).split(".")[2]
     try:
         if btype in ["ELF", "MachO"]:
             ep = binary.virtual_address_to_offset(binary.entrypoint)
             ep_section = binary.section_from_offset(ep)
         elif btype == "PE":
             ep = binary.rva_to_offset(binary.optional_header.addressof_entrypoint)
             ep_section = binary.section_from_rva(binary.optional_header.addressof_entrypoint)
         else:
             raise OSError("Unknown format")
         return ep, ep_section.name
-    except (AttributeError, lief.not_found, lief.conversion_error):
+    except (AttributeError, lief._lief.lief_errors.not_found, lief._lief.lief_errors.conversion_error):
         return None, None
 
 
 def _human_readable_size(size, precision=0):
     """ Convert size in bytes to a more readable form. """
     i, units = 0, ["B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB", "YB"]
     while size > 1024 and i < len(units):
@@ -110,20 +110,16 @@
     :param decide:                    decide if packed or not, otherwise simply return the entropy values
     :param threshold_average_entropy: threshold on average entropy for deciding if packed
     :param threshold_highest_entropy: threshold on highest entropy for deciding if packed
     :param logger:                    logger instance for debug purpose
     :return:                          if decide is True  => bool (whether the input executable is packed or not)
                                                    False => (average_entropy, highest_block_entropy)
     """
-    # try to parse the binary first ; capture the stderr messages from LIEF
-    tmp_fd, null_fd = os.dup(2), os.open(os.devnull, os.O_RDWR)
-    os.dup2(null_fd, 2)
+    # try to parse the binary first
     binary = lief.parse(str(executable))
-    os.dup2(tmp_fd, 2)  # restore stderr
-    os.close(null_fd)
     if binary is None:
         raise OSError("Unknown format")
     # now select the right thresholds
     thresholds = THRESHOLDS.get(binary.format, THRESHOLDS['default'])
     _t1, _t2 = threshold_average_entropy, threshold_highest_entropy
     _t1, _t2 = [_t1, thresholds[0]][_t1 is None], [_t2, thresholds[1]][_t2 is None]
     # FIRST MODE: compute the entropy of the whole executable
```

### Comparing `bintropy-1.4.1/src/bintropy/__main__.py` & `bintropy-1.4.2/src/bintropy/__main__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.1/src/bintropy.egg-info/PKG-INFO` & `bintropy-1.4.2/src/bintropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.1
+Version: 1.4.2
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

