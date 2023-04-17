# Comparing `tmp/EMPOL_GUI-2.1.0.tar.gz` & `tmp/EMPOL_GUI-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EMPOL_GUI-2.1.0.tar", last modified: Mon Apr 17 07:53:06 2023, max compression
+gzip compressed data, was "EMPOL_GUI-2.2.0.tar", last modified: Mon Apr 17 08:05:04 2023, max compression
```

## Comparing `EMPOL_GUI-2.1.0.tar` & `EMPOL_GUI-2.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 07:53:06.889598 EMPOL_GUI-2.1.0/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 07:53:06.889598 EMPOL_GUI-2.1.0/EMPOL_GUI.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 07:53:06.000000 EMPOL_GUI-2.1.0/EMPOL_GUI.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-17 07:53:06.000000 EMPOL_GUI-2.1.0/EMPOL_GUI.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 07:53:06.000000 EMPOL_GUI-2.1.0/EMPOL_GUI.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 07:53:06.000000 EMPOL_GUI-2.1.0/EMPOL_GUI.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-17 05:51:31.000000 EMPOL_GUI-2.1.0/LICENCE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 07:53:06.889598 EMPOL_GUI-2.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2023-04-17 05:48:57.000000 EMPOL_GUI-2.1.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 07:53:06.889598 EMPOL_GUI-2.1.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-04-17 07:10:04.000000 EMPOL_GUI-2.1.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 08:05:04.000000 EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-04-17 05:51:31.000000 EMPOL_GUI-2.2.0/LICENCE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2142 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1708 2023-04-17 05:48:57.000000 EMPOL_GUI-2.2.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 08:05:04.476984 EMPOL_GUI-2.2.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      644 2023-04-17 08:03:59.000000 EMPOL_GUI-2.2.0/setup.py
```

### Comparing `EMPOL_GUI-2.1.0/EMPOL_GUI.egg-info/PKG-INFO` & `EMPOL_GUI-2.2.0/EMPOL_GUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: EMPOL-GUI
-Version: 2.1.0
+Version: 2.2.0
 Summary: Astronomial Large Data Reduction GUI - EMPOL
 Home-page: https://github.com/aasthagupta128/EMPOL_GUI
 Author: Aastha Gupta
-Author-email: aastha.gupta1208@email.com
+Author-email: aastha.gupta1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 Note: The file is only for Linux - Ubuntu Users
```

### Comparing `EMPOL_GUI-2.1.0/LICENCE` & `EMPOL_GUI-2.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `EMPOL_GUI-2.1.0/PKG-INFO` & `EMPOL_GUI-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: EMPOL_GUI
-Version: 2.1.0
+Version: 2.2.0
 Summary: Astronomial Large Data Reduction GUI - EMPOL
 Home-page: https://github.com/aasthagupta128/EMPOL_GUI
 Author: Aastha Gupta
-Author-email: aastha.gupta1208@email.com
+Author-email: aastha.gupta1208@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 Note: The file is only for Linux - Ubuntu Users
```

### Comparing `EMPOL_GUI-2.1.0/README.md` & `EMPOL_GUI-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `EMPOL_GUI-2.1.0/setup.py` & `EMPOL_GUI-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EMPOL_GUI",
-    version="2.1.0",
+    version="2.2.0",
     author="Aastha Gupta",
-    author_email="aastha.gupta1208@email.com",
+    author_email="aastha.gupta1208@gmail.com",
     description="Astronomial Large Data Reduction GUI - EMPOL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aasthagupta128/EMPOL_GUI",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

