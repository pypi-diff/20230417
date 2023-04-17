# Comparing `tmp/EMPOL_GUI-1.0.0.tar.gz` & `tmp/EMPOL_GUI-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EMPOL_GUI-1.0.0.tar", last modified: Mon Apr 17 05:59:43 2023, max compression
+gzip compressed data, was "EMPOL_GUI-1.1.0.tar", last modified: Mon Apr 17 06:25:18 2023, max compression
```

## Comparing `EMPOL_GUI-1.0.0.tar` & `EMPOL_GUI-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 05:59:43.764614 EMPOL_GUI-1.0.0/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 05:59:43.764614 EMPOL_GUI-1.0.0/EMPOL_GUI.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-04-17 05:59:43.000000 EMPOL_GUI-1.0.0/EMPOL_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-17 05:59:43.000000 EMPOL_GUI-1.0.0/EMPOL_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 05:59:43.000000 EMPOL_GUI-1.0.0/EMPOL_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 05:59:43.000000 EMPOL_GUI-1.0.0/EMPOL_GUI.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-17 05:51:31.000000 EMPOL_GUI-1.0.0/LICENCE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-04-17 05:59:43.764614 EMPOL_GUI-1.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2023-04-17 05:48:57.000000 EMPOL_GUI-1.0.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 05:59:43.764614 EMPOL_GUI-1.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      646 2023-04-17 05:57:38.000000 EMPOL_GUI-1.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 06:25:18.048211 EMPOL_GUI-1.1.0/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 06:25:18.048211 EMPOL_GUI-1.1.0/EMPOL_GUI.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-04-17 06:25:18.000000 EMPOL_GUI-1.1.0/EMPOL_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-17 06:25:18.000000 EMPOL_GUI-1.1.0/EMPOL_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 06:25:18.000000 EMPOL_GUI-1.1.0/EMPOL_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 06:25:18.000000 EMPOL_GUI-1.1.0/EMPOL_GUI.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-17 05:51:31.000000 EMPOL_GUI-1.1.0/LICENCE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2144 2023-04-17 06:25:18.048211 EMPOL_GUI-1.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2023-04-17 05:48:57.000000 EMPOL_GUI-1.1.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 06:25:18.048211 EMPOL_GUI-1.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      646 2023-04-17 06:25:10.000000 EMPOL_GUI-1.1.0/setup.py
```

### Comparing `EMPOL_GUI-1.0.0/EMPOL_GUI.egg-info/PKG-INFO` & `EMPOL_GUI-1.1.0/EMPOL_GUI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EMPOL-GUI
-Version: 1.0.0
+Version: 1.1.0
 Summary: Astronomial Large Data Reduction GUI - EMPOL
 Home-page: https://github.com/aasthagupta128/Merged_Code
 Author: Aastha Gupta
 Author-email: aastha.gupta1208@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EMPOL_GUI-1.0.0/LICENCE` & `EMPOL_GUI-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `EMPOL_GUI-1.0.0/PKG-INFO` & `EMPOL_GUI-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EMPOL_GUI
-Version: 1.0.0
+Version: 1.1.0
 Summary: Astronomial Large Data Reduction GUI - EMPOL
 Home-page: https://github.com/aasthagupta128/Merged_Code
 Author: Aastha Gupta
 Author-email: aastha.gupta1208@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EMPOL_GUI-1.0.0/README.md` & `EMPOL_GUI-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `EMPOL_GUI-1.0.0/setup.py` & `EMPOL_GUI-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EMPOL_GUI",
-    version="1.0.0",
+    version="1.1.0",
     author="Aastha Gupta",
     author_email="aastha.gupta1208@email.com",
     description="Astronomial Large Data Reduction GUI - EMPOL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aasthagupta128/Merged_Code",
     packages=setuptools.find_packages(),
```

