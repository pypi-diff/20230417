# Comparing `tmp/EMPOL_GUI-2.2.0.tar.gz` & `tmp/EMPOL_GUI-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EMPOL_GUI-2.2.0.tar", last modified: Mon Apr 17 08:05:04 2023, max compression
+gzip compressed data, was "EMPOL_GUI-2.2.1.tar", last modified: Mon Apr 17 08:13:59 2023, max compression
```

## Comparing `EMPOL_GUI-2.2.0.tar` & `EMPOL_GUI-2.2.1.tar`

### file list

```diff
@@ -1,11 +1,25 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-17 05:51:31.000000 EMPOL_GUI-2.2.0/LICENCE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2023-04-17 05:48:57.000000 EMPOL_GUI-2.2.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-04-17 08:03:59.000000 EMPOL_GUI-2.2.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 08:13:59.562820 EMPOL_GUI-2.2.1/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 08:13:59.558820 EMPOL_GUI-2.2.1/EMPOL_GUI/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1067 2023-03-27 09:54:20.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/Bias.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2052 2023-03-27 09:54:20.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/Flat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15568 2023-04-10 09:34:15.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/GUI_merge_astid.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       18 2023-04-17 08:10:52.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8441 2023-03-29 06:18:04.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/empol_astrometry.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    20693 2023-03-27 09:54:20.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/empol_center_finding.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     9976 2023-03-29 05:44:18.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/empol_photometry.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10543 2023-03-29 06:22:31.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/empol_pol.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6658 2023-03-29 05:45:28.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/empol_pol_single_obj.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2758 2023-03-27 09:54:20.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/extcatalog.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4435 2023-03-27 09:54:20.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/recenter.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8968 2023-04-07 18:57:50.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/single_obj_stack.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     9263 2023-03-29 06:01:01.000000 EMPOL_GUI-2.2.1/EMPOL_GUI/single_phot.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 08:13:59.562820 EMPOL_GUI-2.2.1/EMPOL_GUI.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 08:13:59.000000 EMPOL_GUI-2.2.1/EMPOL_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      497 2023-04-17 08:13:59.000000 EMPOL_GUI-2.2.1/EMPOL_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 08:13:59.000000 EMPOL_GUI-2.2.1/EMPOL_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-04-17 08:13:59.000000 EMPOL_GUI-2.2.1/EMPOL_GUI.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-17 05:51:31.000000 EMPOL_GUI-2.2.1/LICENCE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 08:13:59.562820 EMPOL_GUI-2.2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2023-04-17 05:48:57.000000 EMPOL_GUI-2.2.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 08:13:59.562820 EMPOL_GUI-2.2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-04-17 08:12:27.000000 EMPOL_GUI-2.2.1/setup.py
```

### Comparing `EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/PKG-INFO` & `EMPOL_GUI-2.2.1/EMPOL_GUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EMPOL-GUI
-Version: 2.2.0
+Version: 2.2.1
 Summary: Astronomial Large Data Reduction GUI - EMPOL
 Home-page: https://github.com/aasthagupta128/EMPOL_GUI
 Author: Aastha Gupta
 Author-email: aastha.gupta1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EMPOL_GUI-2.2.0/LICENCE` & `EMPOL_GUI-2.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `EMPOL_GUI-2.2.0/PKG-INFO` & `EMPOL_GUI-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EMPOL_GUI
-Version: 2.2.0
+Version: 2.2.1
 Summary: Astronomial Large Data Reduction GUI - EMPOL
 Home-page: https://github.com/aasthagupta128/EMPOL_GUI
 Author: Aastha Gupta
 Author-email: aastha.gupta1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EMPOL_GUI-2.2.0/README.md` & `EMPOL_GUI-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `EMPOL_GUI-2.2.0/setup.py` & `EMPOL_GUI-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EMPOL_GUI",
-    version="2.2.0",
+    version="2.2.1",
     author="Aastha Gupta",
     author_email="aastha.gupta1208@gmail.com",
     description="Astronomial Large Data Reduction GUI - EMPOL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aasthagupta128/EMPOL_GUI",
     packages=setuptools.find_packages(),
```

