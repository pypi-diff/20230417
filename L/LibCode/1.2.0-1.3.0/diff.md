# Comparing `tmp/LibCode-1.2.0.tar.gz` & `tmp/LibCode-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibCode-1.2.0.tar", last modified: Mon Apr 17 05:28:05 2023, max compression
+gzip compressed data, was "LibCode-1.3.0.tar", last modified: Mon Apr 17 05:42:52 2023, max compression
```

## Comparing `LibCode-1.2.0.tar` & `LibCode-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:28:05.141228 LibCode-1.2.0/
--rw-r--r--   0 axelsanchez   (501) staff       (20)     1070 2023-04-04 05:26:09.000000 LibCode-1.2.0/LICENSE
-drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:28:05.140390 LibCode-1.2.0/LibCode.egg-info/
--rw-r--r--   0 axelsanchez   (501) staff       (20)    23223 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/PKG-INFO
--rw-r--r--   0 axelsanchez   (501) staff       (20)      198 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/SOURCES.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)        1 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/dependency_links.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)        7 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/requires.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)        6 2023-04-17 05:28:05.000000 LibCode-1.2.0/LibCode.egg-info/top_level.txt
--rw-r--r--   0 axelsanchez   (501) staff       (20)    23223 2023-04-17 05:28:05.141062 LibCode-1.2.0/PKG-INFO
--rw-r--r--   0 axelsanchez   (501) staff       (20)    22760 2023-04-17 05:24:23.000000 LibCode-1.2.0/README.md
-drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:28:05.140539 LibCode-1.2.0/myLib/
--rw-r--r--   0 axelsanchez   (501) staff       (20)      241 2023-04-11 03:18:19.000000 LibCode-1.2.0/myLib/__init__.py
--rw-r--r--   0 axelsanchez   (501) staff       (20)       38 2023-04-17 05:28:05.141291 LibCode-1.2.0/setup.cfg
--rw-r--r--   0 axelsanchez   (501) staff       (20)      718 2023-04-17 05:27:03.000000 LibCode-1.2.0/setup.py
+drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:42:52.362365 LibCode-1.3.0/
+-rw-r--r--   0 axelsanchez   (501) staff       (20)     1070 2023-04-04 05:26:09.000000 LibCode-1.3.0/LICENSE
+drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:42:52.361757 LibCode-1.3.0/LibCode.egg-info/
+-rw-r--r--   0 axelsanchez   (501) staff       (20)    23230 2023-04-17 05:42:52.000000 LibCode-1.3.0/LibCode.egg-info/PKG-INFO
+-rw-r--r--   0 axelsanchez   (501) staff       (20)      198 2023-04-17 05:42:52.000000 LibCode-1.3.0/LibCode.egg-info/SOURCES.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)        1 2023-04-17 05:42:52.000000 LibCode-1.3.0/LibCode.egg-info/dependency_links.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)        7 2023-04-17 05:42:52.000000 LibCode-1.3.0/LibCode.egg-info/requires.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)        6 2023-04-17 05:42:52.000000 LibCode-1.3.0/LibCode.egg-info/top_level.txt
+-rw-r--r--   0 axelsanchez   (501) staff       (20)    23230 2023-04-17 05:42:52.362240 LibCode-1.3.0/PKG-INFO
+-rw-r--r--   0 axelsanchez   (501) staff       (20)    22767 2023-04-17 05:35:50.000000 LibCode-1.3.0/README.md
+drwxr-xr-x   0 axelsanchez   (501) staff       (20)        0 2023-04-17 05:42:52.361871 LibCode-1.3.0/myLib/
+-rw-r--r--   0 axelsanchez   (501) staff       (20)      241 2023-04-11 03:18:19.000000 LibCode-1.3.0/myLib/__init__.py
+-rw-r--r--   0 axelsanchez   (501) staff       (20)       38 2023-04-17 05:42:52.362403 LibCode-1.3.0/setup.cfg
+-rw-r--r--   0 axelsanchez   (501) staff       (20)      718 2023-04-17 05:35:35.000000 LibCode-1.3.0/setup.py
```

### Comparing `LibCode-1.2.0/LICENSE` & `LibCode-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LibCode-1.2.0/LibCode.egg-info/PKG-INFO` & `LibCode-1.3.0/LibCode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibCode
-Version: 1.2.0
+Version: 1.3.0
 Summary: A data structures and algorithms library implemented with Python and tested with Pytest!
 Home-page: https://github.com/Axeloooo/LibCode
 Author: Axel Sanchez and  Mariia Podgaietska
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 # LibCode
 
 ![](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white) ![](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=for-the-badge&logo=Pytest&logoColor=white) ![](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=for-the-badge&logo=GitHub-Actions&logoColor=white) ![](https://img.shields.io/badge/Git-F05032.svg?style=for-the-badge&logo=Git&logoColor=white) ![](https://img.shields.io/badge/macOS-000000.svg?style=for-the-badge&logo=macOS&logoColor=white)
 
 ### PyPi Package URL
 
 ```bash
-https://pypi.org/project/LibCode/1.1.0/
+https://pypi.org/project/LibCode/1.3.0/
 ```
 
 ### Collaborators
 
 - Axel Sanchez
 - Mariia Podgaietska
 
@@ -40,15 +40,15 @@
 - Circular Doubly Linked List
 - Binary Search Tree
 - AVL Tree
 
 ## Installation
 
 ```bash
-pip install LibCode
+pip install LibCode==1.3.0
 ```
 
 ## Overview
 
 The library contains the following modules:
 
 - `myLib.src.data_structures.linear`
```

### Comparing `LibCode-1.2.0/PKG-INFO` & `LibCode-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibCode
-Version: 1.2.0
+Version: 1.3.0
 Summary: A data structures and algorithms library implemented with Python and tested with Pytest!
 Home-page: https://github.com/Axeloooo/LibCode
 Author: Axel Sanchez and  Mariia Podgaietska
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 # LibCode
 
 ![](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white) ![](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=for-the-badge&logo=Pytest&logoColor=white) ![](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=for-the-badge&logo=GitHub-Actions&logoColor=white) ![](https://img.shields.io/badge/Git-F05032.svg?style=for-the-badge&logo=Git&logoColor=white) ![](https://img.shields.io/badge/macOS-000000.svg?style=for-the-badge&logo=macOS&logoColor=white)
 
 ### PyPi Package URL
 
 ```bash
-https://pypi.org/project/LibCode/1.1.0/
+https://pypi.org/project/LibCode/1.3.0/
 ```
 
 ### Collaborators
 
 - Axel Sanchez
 - Mariia Podgaietska
 
@@ -40,15 +40,15 @@
 - Circular Doubly Linked List
 - Binary Search Tree
 - AVL Tree
 
 ## Installation
 
 ```bash
-pip install LibCode
+pip install LibCode==1.3.0
 ```
 
 ## Overview
 
 The library contains the following modules:
 
 - `myLib.src.data_structures.linear`
```

### Comparing `LibCode-1.2.0/README.md` & `LibCode-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # LibCode
 
 ![](https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white) ![](https://img.shields.io/badge/Pytest-0A9EDC.svg?style=for-the-badge&logo=Pytest&logoColor=white) ![](https://img.shields.io/badge/GitHub%20Actions-2088FF.svg?style=for-the-badge&logo=GitHub-Actions&logoColor=white) ![](https://img.shields.io/badge/Git-F05032.svg?style=for-the-badge&logo=Git&logoColor=white) ![](https://img.shields.io/badge/macOS-000000.svg?style=for-the-badge&logo=macOS&logoColor=white)
 
 ### PyPi Package URL
 
 ```bash
-https://pypi.org/project/LibCode/1.1.0/
+https://pypi.org/project/LibCode/1.3.0/
 ```
 
 ### Collaborators
 
 - Axel Sanchez
 - Mariia Podgaietska
 
@@ -27,15 +27,15 @@
 - Circular Doubly Linked List
 - Binary Search Tree
 - AVL Tree
 
 ## Installation
 
 ```bash
-pip install LibCode
+pip install LibCode==1.3.0
 ```
 
 ## Overview
 
 The library contains the following modules:
 
 - `myLib.src.data_structures.linear`
```

### Comparing `LibCode-1.2.0/setup.py` & `LibCode-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="LibCode",
-    version="1.2.0",
+    version="1.3.0",
     description="A data structures and algorithms library implemented with Python and tested with Pytest!",
     author="Axel Sanchez and  Mariia Podgaietska",
     packages=[
         "myLib",
     ],
     install_requires=[
         "pytest",
```

