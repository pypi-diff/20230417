# Comparing `tmp/SmartsheetFunctions-0.0.5.2.tar.gz` & `tmp/SmartsheetFunctions-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartsheetFunctions-0.0.5.2.tar", last modified: Mon Apr 17 15:39:36 2023, max compression
+gzip compressed data, was "SmartsheetFunctions-0.0.5.3.tar", last modified: Mon Apr 17 21:03:50 2023, max compression
```

## Comparing `SmartsheetFunctions-0.0.5.2.tar` & `SmartsheetFunctions-0.0.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:39:36.001331 SmartsheetFunctions-0.0.5.2/
--rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.2/LICENSE
--rw-rw-rw-   0        0        0     5064 2023-04-17 15:39:35.999330 SmartsheetFunctions-0.0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 15:39:35.979329 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions/
--rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions/__init__.py
--rw-rw-rw-   0        0        0     9284 2023-04-17 15:36:32.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions/smartsheet.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:39:35.996333 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/
--rw-rw-rw-   0        0        0     5064 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 15:39:35.000000 SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:39:36.001331 SmartsheetFunctions-0.0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-04-17 15:36:30.000000 SmartsheetFunctions-0.0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:03:50.228917 SmartsheetFunctions-0.0.5.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-06 14:51:56.000000 SmartsheetFunctions-0.0.5.3/LICENSE
+-rw-rw-rw-   0        0        0     5064 2023-04-17 21:03:50.227919 SmartsheetFunctions-0.0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4659 2023-04-06 16:20:52.000000 SmartsheetFunctions-0.0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 21:03:50.207917 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions/
+-rw-rw-rw-   0        0        0        0 2023-03-08 20:38:06.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions/__init__.py
+-rw-rw-rw-   0        0        0    23338 2023-04-17 21:02:30.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions/smartsheet.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:03:50.224921 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/
+-rw-rw-rw-   0        0        0     5064 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-17 21:03:50.000000 SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:03:50.229916 SmartsheetFunctions-0.0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      763 2023-04-17 21:03:08.000000 SmartsheetFunctions-0.0.5.3/setup.py
```

### Comparing `SmartsheetFunctions-0.0.5.2/LICENSE` & `SmartsheetFunctions-0.0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.2/PKG-INFO` & `SmartsheetFunctions-0.0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.2/README.md` & `SmartsheetFunctions-0.0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `SmartsheetFunctions-0.0.5.2/SmartsheetFunctions.egg-info/PKG-INFO` & `SmartsheetFunctions-0.0.5.3/SmartsheetFunctions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartsheetFunctions
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: SmartSheet Functions for development
 Author: Derek Bantel
 Author-email: derekbantel@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SmartsheetFunctions-0.0.5.2/setup.py` & `SmartsheetFunctions-0.0.5.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="SmartsheetFunctions",
-    version="0.0.5.2",
+    version="0.0.5.3",
     author="Derek Bantel",
     author_email="derekbantel@outlook.com",
     description="SmartSheet Functions for development",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     packages=["SmartsheetFunctions"],
```

