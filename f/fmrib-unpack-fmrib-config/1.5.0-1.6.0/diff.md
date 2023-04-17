# Comparing `tmp/fmrib-unpack-fmrib-config-1.5.0.tar.gz` & `tmp/fmrib-unpack-fmrib-config-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmrib-unpack-fmrib-config-1.5.0.tar", last modified: Tue Mar 21 11:13:31 2023, max compression
+gzip compressed data, was "fmrib-unpack-fmrib-config-1.6.0.tar", last modified: Mon Apr 17 11:22:04 2023, max compression
```

## Comparing `fmrib-unpack-fmrib-config-1.5.0.tar` & `fmrib-unpack-fmrib-config-1.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 11:13:31.643835 fmrib-unpack-fmrib-config-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/AUTHOR
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9716 2023-03-21 11:13:31.642835 fmrib-unpack-fmrib-config-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9356 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 11:13:31.633835 fmrib-unpack-fmrib-config-1.5.0/fmrib_unpack_fmrib_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9716 2023-03-21 11:13:31.000000 fmrib-unpack-fmrib-config-1.5.0/fmrib_unpack_fmrib_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      733 2023-03-21 11:13:31.000000 fmrib-unpack-fmrib-config-1.5.0/fmrib_unpack_fmrib_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 11:13:31.000000 fmrib-unpack-fmrib-config-1.5.0/fmrib_unpack_fmrib_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-21 11:13:31.000000 fmrib-unpack-fmrib-config-1.5.0/fmrib_unpack_fmrib_config.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 11:13:31.626835 fmrib-unpack-fmrib-config-1.5.0/funpack/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 11:13:31.637836 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 11:13:31.642835 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/
--rw-rw-rw-   0 root         (0) root         (0)    11590 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/categories.tsv
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-03-21 11:13:18.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/datacodings_navalues.tsv
--rw-rw-rw-   0 root         (0) root         (0)      927 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/datacodings_recoding.tsv
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/datetime_formatting.tsv
--rw-rw-rw-   0 root         (0) root         (0)     3384 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/processing.tsv
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/variables_clean.tsv
--rw-rw-rw-   0 root         (0) root         (0)     5703 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/variables_parentvalues.tsv
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib.cfg
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib_cats.cfg
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib_logs.cfg
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib_new_release.cfg
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib_standard.cfg
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-02-03 09:40:14.000000 fmrib-unpack-fmrib-config-1.5.0/funpack/configs/local.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 11:13:31.643835 fmrib-unpack-fmrib-config-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-03-21 11:13:18.000000 fmrib-unpack-fmrib-config-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:22:04.130812 fmrib-unpack-fmrib-config-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/AUTHOR
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9716 2023-04-17 11:22:04.126812 fmrib-unpack-fmrib-config-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:22:04.126812 fmrib-unpack-fmrib-config-1.6.0/fmrib_unpack_fmrib_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9716 2023-04-17 11:22:04.000000 fmrib-unpack-fmrib-config-1.6.0/fmrib_unpack_fmrib_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      733 2023-04-17 11:22:04.000000 fmrib-unpack-fmrib-config-1.6.0/fmrib_unpack_fmrib_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 11:22:04.000000 fmrib-unpack-fmrib-config-1.6.0/fmrib_unpack_fmrib_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 11:22:04.000000 fmrib-unpack-fmrib-config-1.6.0/fmrib_unpack_fmrib_config.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:22:04.122812 fmrib-unpack-fmrib-config-1.6.0/funpack/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:22:04.126812 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:22:04.126812 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/
+-rw-rw-rw-   0 root         (0) root         (0)    11590 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/categories.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     3568 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/datacodings_navalues.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/datacodings_recoding.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/datetime_formatting.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     3384 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/processing.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/variables_clean.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/variables_parentvalues.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib_cats.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib_logs.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib_new_release.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib_standard.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/funpack/configs/local.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 11:22:04.130812 fmrib-unpack-fmrib-config-1.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-04-17 11:21:57.000000 fmrib-unpack-fmrib-config-1.6.0/setup.py
```

### Comparing `fmrib-unpack-fmrib-config-1.5.0/LICENSE` & `fmrib-unpack-fmrib-config-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/PKG-INFO` & `fmrib-unpack-fmrib-config-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmrib-unpack-fmrib-config
-Version: 1.5.0
+Version: 1.6.0
 Summary: The FUNPACK FMRIB configuration profile
 Home-page: https://git.fmrib.ox.ac.uk/fsl/funpack-fmrib-config
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `fmrib-unpack-fmrib-config-1.5.0/README.md` & `fmrib-unpack-fmrib-config-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/fmrib_unpack_fmrib_config.egg-info/PKG-INFO` & `fmrib-unpack-fmrib-config-1.6.0/fmrib_unpack_fmrib_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmrib-unpack-fmrib-config
-Version: 1.5.0
+Version: 1.6.0
 Summary: The FUNPACK FMRIB configuration profile
 Home-page: https://git.fmrib.ox.ac.uk/fsl/funpack-fmrib-config
 Author: Paul McCarthy
 Author-email: pauldmccarthy@gmail.com
 License: Apache License Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `fmrib-unpack-fmrib-config-1.5.0/fmrib_unpack_fmrib_config.egg-info/SOURCES.txt` & `fmrib-unpack-fmrib-config-1.6.0/fmrib_unpack_fmrib_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/categories.tsv` & `fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/categories.tsv`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/processing.tsv` & `fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/processing.tsv`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib/variables_parentvalues.tsv` & `fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib/variables_parentvalues.tsv`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib.cfg` & `fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # FUNPACK "fmrib.cfg" configuration file
 #
 # Provides FMRIB-recommended processing of UKB tables
 #
 
 # Record config version number in FUNPACK logging
-echo "FUNPACK FMRIB configuration version: 1.3.0"
+echo "FUNPACK FMRIB configuration version: 1.6.0"
 
 # Use local settings
 config_file local
 
 # Contains some FMRIB-specific plugin functions,
 # including date/time normalisation.
 plugin_file fmrib
```

### Comparing `fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib_cats.cfg` & `fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib_cats.cfg`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib_logs.cfg` & `fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib_logs.cfg`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/funpack/configs/fmrib_new_release.cfg` & `fmrib-unpack-fmrib-config-1.6.0/funpack/configs/fmrib_new_release.cfg`

 * *Files identical despite different names*

### Comparing `fmrib-unpack-fmrib-config-1.5.0/setup.py` & `fmrib-unpack-fmrib-config-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import os.path as op
 
 from setuptools import setup
 
-version = '1.5.0'
+version = '1.6.0'
 basedir = op.dirname(__file__)
 
 with open(op.join(basedir, 'README.md'), 'rt') as f:
     readme = f.read()
 
 setup(
     name='fmrib-unpack-fmrib-config',
```

