# Comparing `tmp/bintropy-1.4.2.tar.gz` & `tmp/bintropy-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bintropy-1.4.2.tar", last modified: Mon Apr 17 15:54:19 2023, max compression
+gzip compressed data, was "bintropy-1.4.3.tar", last modified: Mon Apr 17 20:33:42 2023, max compression
```

## Comparing `bintropy-1.4.2.tar` & `bintropy-1.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.549150 bintropy-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.541149 bintropy-1.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.541149 bintropy-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-17 15:54:09.000000 bintropy-1.4.2/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-17 15:54:09.000000 bintropy-1.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 15:54:09.000000 bintropy-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:54:19.549150 bintropy-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-17 15:54:09.000000 bintropy-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.545150 bintropy-1.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-17 15:54:09.000000 bintropy-1.4.2/docs/example-not-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-17 15:54:09.000000 bintropy-1.4.2/docs/example-packed.png
--rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-17 15:54:09.000000 bintropy-1.4.2/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-17 15:54:09.000000 bintropy-1.4.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-17 15:54:09.000000 bintropy-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:54:19.549150 bintropy-1.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.541149 bintropy-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.545150 bintropy-1.4.2/src/bintropy/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-17 15:54:09.000000 bintropy-1.4.2/src/bintropy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:54:19.549150 bintropy-1.4.2/src/bintropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 15:54:19.000000 bintropy-1.4.2/src/bintropy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-17 20:33:34.000000 bintropy-1.4.3/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-17 20:33:34.000000 bintropy-1.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 20:33:34.000000 bintropy-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 20:33:42.403380 bintropy-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-17 20:33:34.000000 bintropy-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    65270 2023-04-17 20:33:34.000000 bintropy-1.4.3/docs/example-not-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56052 2023-04-17 20:33:34.000000 bintropy-1.4.3/docs/example-packed.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2023-04-17 20:33:34.000000 bintropy-1.4.3/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-17 20:33:34.000000 bintropy-1.4.3/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-17 20:33:34.000000 bintropy-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:33:42.403380 bintropy-1.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/src/bintropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23759 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-17 20:33:34.000000 bintropy-1.4.3/src/bintropy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:33:42.403380 bintropy-1.4.3/src/bintropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46750 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 20:33:42.000000 bintropy-1.4.3/src/bintropy.egg-info/top_level.txt
```

### Comparing `bintropy-1.4.2/.github/workflows/python-package.yml` & `bintropy-1.4.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/.gitignore` & `bintropy-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/LICENSE` & `bintropy-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/PKG-INFO` & `bintropy-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.2
+Version: 1.4.3
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bintropy-1.4.2/README.md` & `bintropy-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/docs/example-not-packed.png` & `bintropy-1.4.3/docs/example-not-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/docs/example-packed.png` & `bintropy-1.4.3/docs/example-packed.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/docs/logo.png` & `bintropy-1.4.3/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/pyproject.toml` & `bintropy-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/src/bintropy/__info__.py` & `bintropy-1.4.3/src/bintropy/__info__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/src/bintropy/__init__.py` & `bintropy-1.4.3/src/bintropy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: UTF-8 -*-
 import lief
 import math
-import matplotlib.pyplot as plt
 import os
 import statistics
 
 
 __all__ = ["bintropy", "characteristics", "entropy", "is_packed", "plot", "THRESHOLDS"]
 
 
+__btype = lambda b: str(type(b)).split(".")[2]
 __log = lambda l, m, lvl="debug": getattr(l, lvl)(m) if l else None
 __secname = lambda s: s.strip("\x00") or s or "<empty>"
 
 # https://matplotlib.org/2.0.2/examples/color/named_colors.html
 COLORS = {
     None:       ["salmon", "gold", "plum", "darkkhaki", "orchid", "sandybrown", "purple", "khaki", "peru", "thistle"],
     'headers':  "black",
@@ -63,23 +63,21 @@
 THRESHOLDS = {
     'default':           (6.677, 7.199),  # average entropy, highest entropy
     lief.EXE_FORMATS.PE: (6.677, 7.199),
     #TODO: get average and highest entropy values for lief.EXE_FORMATS.ELF
     #TODO: get average and highest entropy values for lief.EXE_FORMATS.MACHO
 }
 
-plt.rcParams['font.family'] = "serif"
-
 
 def _get_ep_and_section(binary):
     """ Helper for computing the entry point and finding its section for each supported format.
     :param binary: LIEF-parsed binary object
     :return:       (ep_file_offset, name_of_ep_section)
     """
-    btype = str(type(binary)).split(".")[2]
+    btype = __btype(binary)
     try:
         if btype in ["ELF", "MachO"]:
             ep = binary.virtual_address_to_offset(binary.entrypoint)
             ep_section = binary.section_from_offset(ep)
         elif btype == "PE":
             ep = binary.rva_to_offset(binary.optional_header.addressof_entrypoint)
             ep_section = binary.section_from_rva(binary.optional_header.addressof_entrypoint)
@@ -221,15 +219,15 @@
     tmp_fd, null_fd = os.dup(2), os.open(os.devnull, os.O_RDWR)
     os.dup2(null_fd, 2)
     binary = lief.parse(str(executable))
     os.dup2(tmp_fd, 2)  # restore stderr
     os.close(null_fd)
     if binary is None:
         raise TypeError("Not an executable")
-    data['type'] = str(type(binary)).split(".")[1]
+    data['type'] = __btype(binary)
     # entry point (EP)
     ep, ep_section = _get_ep_and_section(binary)
     # convert to 3-tuple (EP offset on plot, EP file offset, section name containing EP)
     data['entrypoint'] = None if ep is None else (int(ep // data['chunksize']), ep, __secname(ep_section))
     # sections
     __d = lambda s, e, n: (int(s), int(e), n, statistics.mean(data['entropy'][int(s):int(e)+1]))
     data['sections'] = [__d(0, int(max(MIN_ZONE_WIDTH, binary.sections[0].offset // chunksize)), "Headers")] \
@@ -339,14 +337,16 @@
     :param filenames:  list of paths of the binaries to be included in the figure
     :param img_format: format of the created figure
     :param dpi:        resolution of the created figure
     :param labels:     list of custom labels to be used for the binaries (can be lambda-based)
     :param sublabel:   static or lambda-based sublabel for display under the label
     :param kwargs:     keyword-arguments for characteristics(...) ; n_samples and window_size
     """
+    import matplotlib.pyplot as plt
+    plt.rcParams['font.family'] = "serif"
     if len(filenames) == 0:
         raise ValueError("No executable to plot")
     lloc, title = kwargs.get('legend_location', "lower center"), not kwargs.get('no_title', False)
     lloc_side = lloc.split()[1] in ["left", "right"]
     nf, N_TOP, N_TOP2, N_BOT, N_BOT2 = len(filenames), 1.15, 1.37, -.15, -.37
     fig, objs = plt.subplots(nf+[0, 1][title], sharex=True)
     fig.set_size_inches(10, nf+[0, 1][title])
```

### Comparing `bintropy-1.4.2/src/bintropy/__main__.py` & `bintropy-1.4.3/src/bintropy/__main__.py`

 * *Files identical despite different names*

### Comparing `bintropy-1.4.2/src/bintropy.egg-info/PKG-INFO` & `bintropy-1.4.3/src/bintropy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bintropy
-Version: 1.4.2
+Version: 1.4.3
 Summary: Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

