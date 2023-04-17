# Comparing `tmp/otoe-0.0.7a1.tar.gz` & `tmp/otoe-0.0.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.7a1.tar", last modified: Mon Apr 17 05:42:20 2023, max compression
+gzip compressed data, was "otoe-0.0.7a2.tar", last modified: Mon Apr 17 05:45:00 2023, max compression
```

## Comparing `otoe-0.0.7a1.tar` & `otoe-0.0.7a2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.007036 otoe-0.0.7a1/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:42:20.006905 otoe-0.0.7a1/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7a1/README.md
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 05:42:20.007077 otoe-0.0.7a1/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1287 2023-04-17 05:42:18.000000 otoe-0.0.7a1/setup.py
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.005704 otoe-0.0.7a1/src/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.005762 otoe-0.0.7a1/src/otoe/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.006711 otoe-0.0.7a1/src/otoe/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      206 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       35 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/top_level.txt
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:45:00.483004 otoe-0.0.7a2/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:45:00.482876 otoe-0.0.7a2/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7a2/README.md
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 05:45:00.483054 otoe-0.0.7a2/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1282 2023-04-17 05:44:25.000000 otoe-0.0.7a2/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:45:00.481617 otoe-0.0.7a2/src/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:45:00.482553 otoe-0.0.7a2/src/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:45:00.000000 otoe-0.0.7a2/src/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      181 2023-04-17 05:45:00.000000 otoe-0.0.7a2/src/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 05:45:00.000000 otoe-0.0.7a2/src/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       35 2023-04-17 05:45:00.000000 otoe-0.0.7a2/src/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-17 05:45:00.000000 otoe-0.0.7a2/src/otoe.egg-info/top_level.txt
```

### Comparing `otoe-0.0.7a1/PKG-INFO` & `otoe-0.0.7a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7a1
+Version: 0.0.7a2
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7a1/README.md` & `otoe-0.0.7a2/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7a1/setup.py` & `otoe-0.0.7a2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.7a1",                        # The initial release version
+    version="0.0.7a2",                        # The initial release version
     author="Yakov Varnaev",                     # Full name of the author
     description="Sort of a UI for espanso configs.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.7',                # Minimum version requirement of the package
     py_modules=['otoe'],             # Name of the python package
-    package_dir={'': 'src/otoe'},     # Directory of the source code of the package
+    package_dir={'': 'src'},     # Directory of the source code of the package
     install_requires=[],                     # Install other dependencies if any
     entry_points={
         'console_scripts': [
             'otoe=otoe:main',
        ],
     }
 )
```

### Comparing `otoe-0.0.7a1/src/otoe/otoe.egg-info/PKG-INFO` & `otoe-0.0.7a2/src/otoe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7a1
+Version: 0.0.7a2
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

