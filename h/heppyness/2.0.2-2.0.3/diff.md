# Comparing `tmp/heppyness-2.0.2.tar.gz` & `tmp/heppyness-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heppyness-2.0.2.tar", last modified: Mon Feb 27 09:56:51 2023, max compression
+gzip compressed data, was "heppyness-2.0.3.tar", last modified: Mon Apr 17 19:46:01 2023, max compression
```

## Comparing `heppyness-2.0.2.tar` & `heppyness-2.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-02-27 09:56:51.895333 heppyness-2.0.2/
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1071 2022-03-22 10:30:20.000000 heppyness-2.0.2/LICENSE
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1619 2023-02-27 09:56:51.895208 heppyness-2.0.2/PKG-INFO
--rw-r--r--   0 stefanrichter   (501) staff       (20)      965 2023-02-24 10:57:18.000000 heppyness-2.0.2/README.md
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-02-27 09:56:51.893177 heppyness-2.0.2/heppy/
--rw-r--r--   0 stefanrichter   (501) staff       (20)      321 2023-02-24 11:27:11.000000 heppyness-2.0.2/heppy/__init__.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    14124 2022-03-22 10:30:20.000000 heppyness-2.0.2/heppy/heatmap.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    69904 2023-02-24 19:45:46.000000 heppyness-2.0.2/heppy/histogram.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2832 2023-02-20 18:47:17.000000 heppyness-2.0.2/heppy/panel.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    17538 2023-02-24 20:06:45.000000 heppyness-2.0.2/heppy/plot.py
--rwxr-xr-x   0 stefanrichter   (501) staff       (20)     2703 2023-02-24 19:52:53.000000 heppyness-2.0.2/heppy/readroot.py
--rwxr-xr-x   0 stefanrichter   (501) staff       (20)    13157 2023-02-25 10:24:04.000000 heppyness-2.0.2/heppy/readroot_legacy.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2184 2023-02-24 20:20:26.000000 heppyness-2.0.2/heppy/readtrex.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2081 2022-04-21 09:18:03.000000 heppyness-2.0.2/heppy/readyoda.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1478 2022-03-22 10:30:20.000000 heppyness-2.0.2/heppy/scanroot.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    26748 2023-02-24 20:07:11.000000 heppyness-2.0.2/heppy/uncertainty.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     5810 2022-03-22 10:30:20.000000 heppyness-2.0.2/heppy/value.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     6170 2022-03-22 10:30:20.000000 heppyness-2.0.2/heppy/yodarun.py
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-02-27 09:56:51.893909 heppyness-2.0.2/heppyness.egg-info/
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1619 2023-02-27 09:56:51.000000 heppyness-2.0.2/heppyness.egg-info/PKG-INFO
--rw-r--r--   0 stefanrichter   (501) staff       (20)      545 2023-02-27 09:56:51.000000 heppyness-2.0.2/heppyness.egg-info/SOURCES.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)        1 2023-02-27 09:56:51.000000 heppyness-2.0.2/heppyness.egg-info/dependency_links.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)       78 2023-02-27 09:56:51.000000 heppyness-2.0.2/heppyness.egg-info/requires.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)        6 2023-02-27 09:56:51.000000 heppyness-2.0.2/heppyness.egg-info/top_level.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)       38 2023-02-27 09:56:51.895375 heppyness-2.0.2/setup.cfg
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1091 2023-02-24 20:52:32.000000 heppyness-2.0.2/setup.py
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-02-27 09:56:51.894940 heppyness-2.0.2/test/
--rw-r--r--   0 stefanrichter   (501) staff       (20)     3030 2022-03-22 10:30:20.000000 heppyness-2.0.2/test/test_heatmap.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    15789 2022-03-22 10:30:20.000000 heppyness-2.0.2/test/test_histogram1d.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    10062 2022-03-22 10:30:20.000000 heppyness-2.0.2/test/test_histogram2d.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2296 2023-02-24 19:10:25.000000 heppyness-2.0.2/test/test_readroot.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2774 2023-02-24 11:15:00.000000 heppyness-2.0.2/test/test_readroot_legacy.py
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-04-17 19:46:01.589826 heppyness-2.0.3/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1071 2022-03-22 10:30:20.000000 heppyness-2.0.3/LICENSE
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1619 2023-04-17 19:46:01.589673 heppyness-2.0.3/PKG-INFO
+-rw-r--r--   0 stefanrichter   (501) staff       (20)      965 2023-02-24 10:57:18.000000 heppyness-2.0.3/README.md
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-04-17 19:46:01.587285 heppyness-2.0.3/heppy/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)      321 2023-02-24 11:27:11.000000 heppyness-2.0.3/heppy/__init__.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    14124 2022-03-22 10:30:20.000000 heppyness-2.0.3/heppy/heatmap.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    69904 2023-02-24 19:45:46.000000 heppyness-2.0.3/heppy/histogram.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2832 2023-02-20 18:47:17.000000 heppyness-2.0.3/heppy/panel.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    17538 2023-02-24 20:06:45.000000 heppyness-2.0.3/heppy/plot.py
+-rwxr-xr-x   0 stefanrichter   (501) staff       (20)     2761 2023-04-17 19:41:29.000000 heppyness-2.0.3/heppy/readroot.py
+-rwxr-xr-x   0 stefanrichter   (501) staff       (20)    13157 2023-04-17 19:28:50.000000 heppyness-2.0.3/heppy/readroot_legacy.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2184 2023-02-24 20:20:26.000000 heppyness-2.0.3/heppy/readtrex.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2081 2022-04-21 09:18:03.000000 heppyness-2.0.3/heppy/readyoda.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1478 2022-03-22 10:30:20.000000 heppyness-2.0.3/heppy/scanroot.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    26748 2023-02-24 20:07:11.000000 heppyness-2.0.3/heppy/uncertainty.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     5810 2022-03-22 10:30:20.000000 heppyness-2.0.3/heppy/value.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     6170 2022-03-22 10:30:20.000000 heppyness-2.0.3/heppy/yodarun.py
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-04-17 19:46:01.588202 heppyness-2.0.3/heppyness.egg-info/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1619 2023-04-17 19:46:01.000000 heppyness-2.0.3/heppyness.egg-info/PKG-INFO
+-rw-r--r--   0 stefanrichter   (501) staff       (20)      545 2023-04-17 19:46:01.000000 heppyness-2.0.3/heppyness.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)        1 2023-04-17 19:46:01.000000 heppyness-2.0.3/heppyness.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)       78 2023-04-17 19:46:01.000000 heppyness-2.0.3/heppyness.egg-info/requires.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)        6 2023-04-17 19:46:01.000000 heppyness-2.0.3/heppyness.egg-info/top_level.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)       38 2023-04-17 19:46:01.589873 heppyness-2.0.3/setup.cfg
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1091 2023-04-17 19:45:06.000000 heppyness-2.0.3/setup.py
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-04-17 19:46:01.589366 heppyness-2.0.3/test/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     3030 2022-03-22 10:30:20.000000 heppyness-2.0.3/test/test_heatmap.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    15789 2022-03-22 10:30:20.000000 heppyness-2.0.3/test/test_histogram1d.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    10062 2022-03-22 10:30:20.000000 heppyness-2.0.3/test/test_histogram2d.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2949 2023-04-17 19:42:25.000000 heppyness-2.0.3/test/test_readroot.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2774 2023-02-24 11:15:00.000000 heppyness-2.0.3/test/test_readroot_legacy.py
```

### Comparing `heppyness-2.0.2/LICENSE` & `heppyness-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/PKG-INFO` & `heppyness-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heppyness
-Version: 2.0.2
+Version: 2.0.3
 Home-page: https://gitlab.cern.ch/strichte/heppy
 Author: Stefan Richter
 Author-email: stefan.richter@cern.ch
 Maintainer: Stefan Richter
 Maintainer-email: stefan.richter@cern.ch
 License: HEP license, based on MIT license
 Classifier: Programming Language :: Python :: 3
```

### Comparing `heppyness-2.0.2/README.md` & `heppyness-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/heatmap.py` & `heppyness-2.0.3/heppy/heatmap.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/histogram.py` & `heppyness-2.0.3/heppy/histogram.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/panel.py` & `heppyness-2.0.3/heppy/panel.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/plot.py` & `heppyness-2.0.3/heppy/plot.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/readroot.py` & `heppyness-2.0.3/heppy/readroot.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     urhist = file[histpath]
 
     if not any(['TH1' in urhist.classname, 'TH2' in urhist.classname]):
         raise TypeError('Can only read ROOT.TH1 and ROOT.TH2 objects, but '
             f'found {urhist.classname} object in {rootfile} at {histpath}')
 
     binedges = tuple([axis.edges() for axis in urhist.axes])
+    if len(binedges) == 1:
+        binedges = binedges[0]
     corr_variations = {}
     for name, path in variation_paths.items():
         try:
             corr_variations[name] = file[path].values()
         except ReferenceError:
             if not ignore_missing_variations:
                 raise ValueError('While reading variation histograms, could '
```

### Comparing `heppyness-2.0.2/heppy/readroot_legacy.py` & `heppyness-2.0.3/heppy/readroot_legacy.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/readtrex.py` & `heppyness-2.0.3/heppy/readtrex.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/readyoda.py` & `heppyness-2.0.3/heppy/readyoda.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/scanroot.py` & `heppyness-2.0.3/heppy/scanroot.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/uncertainty.py` & `heppyness-2.0.3/heppy/uncertainty.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/value.py` & `heppyness-2.0.3/heppy/value.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppy/yodarun.py` & `heppyness-2.0.3/heppy/yodarun.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/heppyness.egg-info/PKG-INFO` & `heppyness-2.0.3/heppyness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heppyness
-Version: 2.0.2
+Version: 2.0.3
 Home-page: https://gitlab.cern.ch/strichte/heppy
 Author: Stefan Richter
 Author-email: stefan.richter@cern.ch
 Maintainer: Stefan Richter
 Maintainer-email: stefan.richter@cern.ch
 License: HEP license, based on MIT license
 Classifier: Programming Language :: Python :: 3
```

### Comparing `heppyness-2.0.2/heppyness.egg-info/SOURCES.txt` & `heppyness-2.0.3/heppyness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/setup.py` & `heppyness-2.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='heppyness',
     license='HEP license, based on MIT license',
-    version='2.0.2',
+    version='2.0.3',
     author='Stefan Richter',
     author_email='stefan.richter@cern.ch',
     maintainer='Stefan Richter',
     maintainer_email='stefan.richter@cern.ch',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `heppyness-2.0.2/test/test_heatmap.py` & `heppyness-2.0.3/test/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/test/test_histogram1d.py` & `heppyness-2.0.3/test/test_histogram1d.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/test/test_histogram2d.py` & `heppyness-2.0.3/test/test_histogram2d.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.2/test/test_readroot_legacy.py` & `heppyness-2.0.3/test/test_readroot_legacy.py`

 * *Files identical despite different names*

