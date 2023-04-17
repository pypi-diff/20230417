# Comparing `tmp/nparray2pil-0.0.1.tar.gz` & `tmp/nparray2pil-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nparray2pil-0.0.1.tar", last modified: Mon Apr 17 12:42:11 2023, max compression
+gzip compressed data, was "nparray2pil-0.0.2.tar", last modified: Mon Apr 17 12:38:42 2023, max compression
```

## Comparing `nparray2pil-0.0.1.tar` & `nparray2pil-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:42:11.398545 nparray2pil-0.0.1/
--rw-rw-rw-   0        0        0     1769 2023-04-17 12:42:11.390558 nparray2pil-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-04-17 12:42:01.000000 nparray2pil-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 12:42:11.341138 nparray2pil-0.0.1/nparray2pil/
--rw-rw-rw-   0        0        0       36 2023-04-17 12:08:53.000000 nparray2pil-0.0.1/nparray2pil/__init__.py
--rw-rw-rw-   0        0        0      211 2023-04-17 12:12:04.000000 nparray2pil-0.0.1/nparray2pil/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:42:11.382510 nparray2pil-0.0.1/nparray2pil.egg-info/
--rw-rw-rw-   0        0        0     1769 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-17 12:42:11.000000 nparray2pil-0.0.1/nparray2pil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 12:42:11.398545 nparray2pil-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1496 2023-04-17 12:41:37.000000 nparray2pil-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:38:42.487769 nparray2pil-0.0.2/
+-rw-rw-rw-   0        0        0     1765 2023-04-17 12:38:42.484259 nparray2pil-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1244 2023-04-17 12:38:19.000000 nparray2pil-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 12:38:42.449166 nparray2pil-0.0.2/nparray2pil/
+-rw-rw-rw-   0        0        0       36 2023-04-17 12:08:53.000000 nparray2pil-0.0.2/nparray2pil/__init__.py
+-rw-rw-rw-   0        0        0      211 2023-04-17 12:12:04.000000 nparray2pil-0.0.2/nparray2pil/main.py
+drwxrwxrwx   0        0        0        0 2023-04-17 12:38:42.479740 nparray2pil-0.0.2/nparray2pil.egg-info/
+-rw-rw-rw-   0        0        0     1765 2023-04-17 12:38:42.000000 nparray2pil-0.0.2/nparray2pil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-17 12:38:42.000000 nparray2pil-0.0.2/nparray2pil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 12:38:42.000000 nparray2pil-0.0.2/nparray2pil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-17 12:38:42.000000 nparray2pil-0.0.2/nparray2pil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-17 12:38:42.000000 nparray2pil-0.0.2/nparray2pil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 12:38:42.487769 nparray2pil-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1496 2023-04-17 12:38:32.000000 nparray2pil-0.0.2/setup.py
```

### Comparing `nparray2pil-0.0.1/PKG-INFO` & `nparray2pil-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nparray2pil
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converts numpy arrays into images.
 Home-page: https://github.com/abhinav-gg/nparray2pil/
 Author: Abhinav G, Oliver Gibson
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: np,array,pil,convertion,convert,opencv,array to pil
 Platform: UNKNOWN
@@ -17,15 +17,15 @@
 
 A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
 
 ![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
 
 ## How does it work?
 
-**Use import nparray2pil to get access to the convert functions:**
+Use import nparray2pil to get access to the convert functions:
 ```python
 from nparray2pil import convert
 ```
 and then convert:
 ```python
 convert(myArray)
 ```
```

### Comparing `nparray2pil-0.0.1/README.md` & `nparray2pil-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
 
 ![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
 
 ## How does it work?
 
-**Use import nparray2pil to get access to the convert functions:**
+Use import nparray2pil to get access to the convert functions:
 ```python
 from nparray2pil import convert
 ```
 and then convert:
 ```python
 convert(myArray)
 ```
```

### Comparing `nparray2pil-0.0.1/nparray2pil.egg-info/PKG-INFO` & `nparray2pil-0.0.2/nparray2pil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nparray2pil
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converts numpy arrays into images.
 Home-page: https://github.com/abhinav-gg/nparray2pil/
 Author: Abhinav G, Oliver Gibson
 Author-email: agupta.cam7@gmail.com
 License: MIT
 Keywords: np,array,pil,convertion,convert,opencv,array to pil
 Platform: UNKNOWN
@@ -17,15 +17,15 @@
 
 A PyPi module allowing the users' code to navigate to aliased line number within the Python interpreter
 
 ![Generic badge](https://img.shields.io/badge/version-0.0.1-green.svg)
 
 ## How does it work?
 
-**Use import nparray2pil to get access to the convert functions:**
+Use import nparray2pil to get access to the convert functions:
 ```python
 from nparray2pil import convert
 ```
 and then convert:
 ```python
 convert(myArray)
 ```
```

### Comparing `nparray2pil-0.0.1/setup.py` & `nparray2pil-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
  
 setuptools.setup(
     # Here is the module name.
     name="nparray2pil",
  
     # version of the module
-    version="0.0.1",
+    version="0.0.2",
  
     # Name of Author
     author="Abhinav G, Oliver Gibson",
  
     # your Email address
     author_email="agupta.cam7@gmail.com",
```

