# Comparing `tmp/astropalmerio-0.1.0.tar.gz` & `tmp/astropalmerio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astropalmerio-0.1.0.tar", last modified: Thu Mar 23 16:18:19 2023, max compression
+gzip compressed data, was "astropalmerio-0.1.1.tar", last modified: Mon Apr 17 14:06:36 2023, max compression
```

## Comparing `astropalmerio-0.1.0.tar` & `astropalmerio-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.676436 astropalmerio-0.1.0/
--rw-r--r--   0 palmerio   (501) staff       (20)    35142 2022-11-04 09:41:03.000000 astropalmerio-0.1.0/LICENSE.md
--rw-r--r--   0 palmerio   (501) staff       (20)     1410 2023-03-23 16:18:19.676856 astropalmerio-0.1.0/PKG-INFO
--rw-r--r--   0 palmerio   (501) staff       (20)      577 2022-12-20 10:39:38.000000 astropalmerio-0.1.0/README.rst
--rw-r--r--   0 palmerio   (501) staff       (20)      143 2023-03-09 16:11:59.000000 astropalmerio-0.1.0/pyproject.toml
--rw-r--r--   0 palmerio   (501) staff       (20)     1135 2023-03-23 16:18:19.678098 astropalmerio-0.1.0/setup.cfg
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.645025 astropalmerio-0.1.0/src/
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.648553 astropalmerio-0.1.0/src/astropalmerio/
--rw-r--r--   0 palmerio   (501) staff       (20)      225 2023-03-23 16:10:54.000000 astropalmerio-0.1.0/src/astropalmerio/__init__.py
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.654635 astropalmerio-0.1.0/src/astropalmerio/galaxies/
--rw-r--r--   0 palmerio   (501) staff       (20)    22021 2023-03-10 10:01:21.000000 astropalmerio-0.1.0/src/astropalmerio/galaxies/M08.py
--rw-r--r--   0 palmerio   (501) staff       (20)     1525 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/galaxies/__init__.py
--rw-r--r--   0 palmerio   (501) staff       (20)     6083 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/galaxies/extinction.py
--rw-r--r--   0 palmerio   (501) staff       (20)     6250 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/galaxies/properties.py
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.657458 astropalmerio-0.1.0/src/astropalmerio/io/
--rw-r--r--   0 palmerio   (501) staff       (20)      211 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/io/__init__.py
--rw-r--r--   0 palmerio   (501) staff       (20)     9410 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/io/ascii.py
--rw-r--r--   0 palmerio   (501) staff       (20)     5150 2023-03-10 10:00:29.000000 astropalmerio-0.1.0/src/astropalmerio/io/fits.py
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.666787 astropalmerio-0.1.0/src/astropalmerio/mc/
--rw-r--r--   0 palmerio   (501) staff       (20)    10420 2023-03-23 15:44:45.000000 astropalmerio-0.1.0/src/astropalmerio/mc/MC_var.py
--rw-r--r--   0 palmerio   (501) staff       (20)     9507 2023-03-23 15:44:45.000000 astropalmerio-0.1.0/src/astropalmerio/mc/__arithmetic_MC_var.py
--rw-r--r--   0 palmerio   (501) staff       (20)     1227 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/mc/__init__.py
--rw-r--r--   0 palmerio   (501) staff       (20)     5621 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/mc/distributions.py
--rw-r--r--   0 palmerio   (501) staff       (20)     8494 2023-03-10 09:55:57.000000 astropalmerio-0.1.0/src/astropalmerio/mc/realizations.py
--rw-r--r--   0 palmerio   (501) staff       (20)     4166 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/mc/sampling.py
--rw-r--r--   0 palmerio   (501) staff       (20)     9585 2023-03-10 09:57:59.000000 astropalmerio-0.1.0/src/astropalmerio/mc/utils.py
--rw-r--r--   0 palmerio   (501) staff       (20)     5855 2023-03-09 16:01:04.000000 astropalmerio-0.1.0/src/astropalmerio/mc/visualization.py
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.675611 astropalmerio-0.1.0/src/astropalmerio/spectra/
--rw-r--r--   0 palmerio   (501) staff       (20)     1361 2023-03-23 09:51:16.000000 astropalmerio-0.1.0/src/astropalmerio/spectra/__init__.py
--rw-r--r--   0 palmerio   (501) staff       (20)     4179 2023-03-23 14:52:33.000000 astropalmerio-0.1.0/src/astropalmerio/spectra/conversions.py
--rw-r--r--   0 palmerio   (501) staff       (20)    18951 2023-03-23 15:45:39.000000 astropalmerio-0.1.0/src/astropalmerio/spectra/emission_lines.py
--rw-r--r--   0 palmerio   (501) staff       (20)     1998 2023-03-23 15:44:45.000000 astropalmerio-0.1.0/src/astropalmerio/spectra/reduction.py
--rw-r--r--   0 palmerio   (501) staff       (20)     5172 2023-03-23 15:44:45.000000 astropalmerio-0.1.0/src/astropalmerio/spectra/utils.py
--rw-r--r--   0 palmerio   (501) staff       (20)     8347 2023-03-10 10:03:12.000000 astropalmerio-0.1.0/src/astropalmerio/spectra/visualization.py
-drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-03-23 16:18:19.651036 astropalmerio-0.1.0/src/astropalmerio.egg-info/
--rw-r--r--   0 palmerio   (501) staff       (20)     1410 2023-03-23 16:18:19.000000 astropalmerio-0.1.0/src/astropalmerio.egg-info/PKG-INFO
--rw-r--r--   0 palmerio   (501) staff       (20)     1091 2023-03-23 16:18:19.000000 astropalmerio-0.1.0/src/astropalmerio.egg-info/SOURCES.txt
--rw-r--r--   0 palmerio   (501) staff       (20)        1 2023-03-23 16:18:19.000000 astropalmerio-0.1.0/src/astropalmerio.egg-info/dependency_links.txt
--rw-r--r--   0 palmerio   (501) staff       (20)        1 2022-11-04 10:36:15.000000 astropalmerio-0.1.0/src/astropalmerio.egg-info/not-zip-safe
--rw-r--r--   0 palmerio   (501) staff       (20)       37 2023-03-23 16:18:19.000000 astropalmerio-0.1.0/src/astropalmerio.egg-info/requires.txt
--rw-r--r--   0 palmerio   (501) staff       (20)       14 2023-03-23 16:18:19.000000 astropalmerio-0.1.0/src/astropalmerio.egg-info/top_level.txt
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.976589 astropalmerio-0.1.1/
+-rw-r--r--   0 palmerio   (501) staff       (20)    35142 2022-11-04 09:41:03.000000 astropalmerio-0.1.1/LICENSE.md
+-rw-r--r--   0 palmerio   (501) staff       (20)       73 2023-04-17 14:04:25.000000 astropalmerio-0.1.1/MANIFEST.in
+-rw-r--r--   0 palmerio   (501) staff       (20)     1410 2023-04-17 14:06:36.976783 astropalmerio-0.1.1/PKG-INFO
+-rw-r--r--   0 palmerio   (501) staff       (20)      577 2022-12-20 10:39:38.000000 astropalmerio-0.1.1/README.rst
+-rw-r--r--   0 palmerio   (501) staff       (20)      143 2023-03-09 16:11:59.000000 astropalmerio-0.1.1/pyproject.toml
+-rw-r--r--   0 palmerio   (501) staff       (20)     1189 2023-04-17 14:06:36.977798 astropalmerio-0.1.1/setup.cfg
+-rw-r--r--   0 palmerio   (501) staff       (20)      148 2023-04-17 14:02:34.000000 astropalmerio-0.1.1/setup.py
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.961571 astropalmerio-0.1.1/src/
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.964405 astropalmerio-0.1.1/src/astropalmerio/
+-rw-r--r--   0 palmerio   (501) staff       (20)      225 2023-04-17 14:06:27.000000 astropalmerio-0.1.1/src/astropalmerio/__init__.py
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.966945 astropalmerio-0.1.1/src/astropalmerio/data/
+-rw-r--r--   0 palmerio   (501) staff       (20)      989 2023-02-10 16:39:24.000000 astropalmerio-0.1.1/src/astropalmerio/data/emission_lines.tsv
+-rw-r--r--   0 palmerio   (501) staff       (20)    24279 2023-02-07 17:21:37.000000 astropalmerio-0.1.1/src/astropalmerio/data/met_cal_for_M08_method.txt
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.968518 astropalmerio-0.1.1/src/astropalmerio/galaxies/
+-rw-r--r--   0 palmerio   (501) staff       (20)    21996 2023-04-12 14:12:30.000000 astropalmerio-0.1.1/src/astropalmerio/galaxies/M08.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     1525 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/galaxies/__init__.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     6083 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/galaxies/extinction.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     6250 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/galaxies/properties.py
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.969875 astropalmerio-0.1.1/src/astropalmerio/io/
+-rw-r--r--   0 palmerio   (501) staff       (20)      211 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/io/__init__.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     9410 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/io/ascii.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     5150 2023-03-10 10:00:29.000000 astropalmerio-0.1.1/src/astropalmerio/io/fits.py
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.973433 astropalmerio-0.1.1/src/astropalmerio/mc/
+-rw-r--r--   0 palmerio   (501) staff       (20)    10420 2023-03-23 15:44:45.000000 astropalmerio-0.1.1/src/astropalmerio/mc/MC_var.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     9507 2023-03-23 15:44:45.000000 astropalmerio-0.1.1/src/astropalmerio/mc/__arithmetic_MC_var.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     1227 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/mc/__init__.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     5621 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/mc/distributions.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     8494 2023-03-10 09:55:57.000000 astropalmerio-0.1.1/src/astropalmerio/mc/realizations.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     4166 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/mc/sampling.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     9585 2023-03-10 09:57:59.000000 astropalmerio-0.1.1/src/astropalmerio/mc/utils.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     5855 2023-03-09 16:01:04.000000 astropalmerio-0.1.1/src/astropalmerio/mc/visualization.py
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.976227 astropalmerio-0.1.1/src/astropalmerio/spectra/
+-rw-r--r--   0 palmerio   (501) staff       (20)     1361 2023-03-23 09:51:16.000000 astropalmerio-0.1.1/src/astropalmerio/spectra/__init__.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     4179 2023-03-23 14:52:33.000000 astropalmerio-0.1.1/src/astropalmerio/spectra/conversions.py
+-rw-r--r--   0 palmerio   (501) staff       (20)    18951 2023-03-23 15:45:39.000000 astropalmerio-0.1.1/src/astropalmerio/spectra/emission_lines.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     1998 2023-03-23 15:44:45.000000 astropalmerio-0.1.1/src/astropalmerio/spectra/reduction.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     5172 2023-03-23 15:44:45.000000 astropalmerio-0.1.1/src/astropalmerio/spectra/utils.py
+-rw-r--r--   0 palmerio   (501) staff       (20)     8347 2023-03-10 10:03:12.000000 astropalmerio-0.1.1/src/astropalmerio/spectra/visualization.py
+drwxr-xr-x   0 palmerio   (501) staff       (20)        0 2023-04-17 14:06:36.966158 astropalmerio-0.1.1/src/astropalmerio.egg-info/
+-rw-r--r--   0 palmerio   (501) staff       (20)     1410 2023-04-17 14:06:36.000000 astropalmerio-0.1.1/src/astropalmerio.egg-info/PKG-INFO
+-rw-r--r--   0 palmerio   (501) staff       (20)     1204 2023-04-17 14:06:36.000000 astropalmerio-0.1.1/src/astropalmerio.egg-info/SOURCES.txt
+-rw-r--r--   0 palmerio   (501) staff       (20)        1 2023-04-17 14:06:36.000000 astropalmerio-0.1.1/src/astropalmerio.egg-info/dependency_links.txt
+-rw-r--r--   0 palmerio   (501) staff       (20)        1 2022-11-04 10:36:15.000000 astropalmerio-0.1.1/src/astropalmerio.egg-info/not-zip-safe
+-rw-r--r--   0 palmerio   (501) staff       (20)       37 2023-04-17 14:06:36.000000 astropalmerio-0.1.1/src/astropalmerio.egg-info/requires.txt
+-rw-r--r--   0 palmerio   (501) staff       (20)       14 2023-04-17 14:06:36.000000 astropalmerio-0.1.1/src/astropalmerio.egg-info/top_level.txt
```

### Comparing `astropalmerio-0.1.0/LICENSE.md` & `astropalmerio-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/PKG-INFO` & `astropalmerio-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropalmerio
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for scientific data analysis and visualization.
 Home-page: https://github.com/JPalmerio/astropalmerio
 Author: Jesse Palmerio
 Author-email: jesse.palmerio@obspm.fr
 Project-URL: Bug Tracker, https://github.com/JPalmerio/astropalmerio/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `astropalmerio-0.1.0/README.rst` & `astropalmerio-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/setup.cfg` & `astropalmerio-0.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 	scipy>=1.10
 	astropy>=5.2
 
 [options.packages.find]
 where = src
 include = astropalmerio*
 
+[options.package_data]
+zhunter.data = 
+	*.tsv
+	*.txt
+
 [flake8]
 ignore = E231, E226, W503
 max-line-length = 88
 extend-ignore = E203
 
 [egg_info]
 tag_build =
```

### Comparing `astropalmerio-0.1.0/src/astropalmerio/galaxies/M08.py` & `astropalmerio-0.1.1/src/astropalmerio/galaxies/M08.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,14 @@
     "OIIIb_NII_scatter_rec",
     "plot_relations",
 ]
 
 import numpy as np
 import matplotlib.pyplot as plt
 
-plt.style.use("ggplot")
-
 
 Maio_file = "./data/met_cal_for_M08_method.txt"
 Z_sun = 8.69
 font = {"size": 15}
 
 
 def read_column(
```

### Comparing `astropalmerio-0.1.0/src/astropalmerio/galaxies/__init__.py` & `astropalmerio-0.1.1/src/astropalmerio/galaxies/__init__.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/galaxies/extinction.py` & `astropalmerio-0.1.1/src/astropalmerio/galaxies/extinction.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/galaxies/properties.py` & `astropalmerio-0.1.1/src/astropalmerio/galaxies/properties.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/io/ascii.py` & `astropalmerio-0.1.1/src/astropalmerio/io/ascii.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/io/fits.py` & `astropalmerio-0.1.1/src/astropalmerio/io/fits.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/MC_var.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/MC_var.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/__arithmetic_MC_var.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/__arithmetic_MC_var.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/__init__.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/distributions.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/distributions.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/realizations.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/realizations.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/sampling.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/sampling.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/utils.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/utils.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/mc/visualization.py` & `astropalmerio-0.1.1/src/astropalmerio/mc/visualization.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/spectra/__init__.py` & `astropalmerio-0.1.1/src/astropalmerio/spectra/__init__.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/spectra/conversions.py` & `astropalmerio-0.1.1/src/astropalmerio/spectra/conversions.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/spectra/emission_lines.py` & `astropalmerio-0.1.1/src/astropalmerio/spectra/emission_lines.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/spectra/reduction.py` & `astropalmerio-0.1.1/src/astropalmerio/spectra/reduction.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/spectra/utils.py` & `astropalmerio-0.1.1/src/astropalmerio/spectra/utils.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio/spectra/visualization.py` & `astropalmerio-0.1.1/src/astropalmerio/spectra/visualization.py`

 * *Files identical despite different names*

### Comparing `astropalmerio-0.1.0/src/astropalmerio.egg-info/PKG-INFO` & `astropalmerio-0.1.1/src/astropalmerio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astropalmerio
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for scientific data analysis and visualization.
 Home-page: https://github.com/JPalmerio/astropalmerio
 Author: Jesse Palmerio
 Author-email: jesse.palmerio@obspm.fr
 Project-URL: Bug Tracker, https://github.com/JPalmerio/astropalmerio/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `astropalmerio-0.1.0/src/astropalmerio.egg-info/SOURCES.txt` & `astropalmerio-0.1.1/src/astropalmerio.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 LICENSE.md
+MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
+setup.py
 src/astropalmerio/__init__.py
 src/astropalmerio.egg-info/PKG-INFO
 src/astropalmerio.egg-info/SOURCES.txt
 src/astropalmerio.egg-info/dependency_links.txt
 src/astropalmerio.egg-info/not-zip-safe
 src/astropalmerio.egg-info/requires.txt
 src/astropalmerio.egg-info/top_level.txt
+src/astropalmerio/data/emission_lines.tsv
+src/astropalmerio/data/met_cal_for_M08_method.txt
 src/astropalmerio/galaxies/M08.py
 src/astropalmerio/galaxies/__init__.py
 src/astropalmerio/galaxies/extinction.py
 src/astropalmerio/galaxies/properties.py
 src/astropalmerio/io/__init__.py
 src/astropalmerio/io/ascii.py
 src/astropalmerio/io/fits.py
```

