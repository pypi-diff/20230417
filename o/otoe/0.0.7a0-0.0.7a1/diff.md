# Comparing `tmp/otoe-0.0.7a0.tar.gz` & `tmp/otoe-0.0.7a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.7a0.tar", last modified: Mon Apr 17 05:33:25 2023, max compression
+gzip compressed data, was "otoe-0.0.7a1.tar", last modified: Mon Apr 17 05:42:20 2023, max compression
```

## Comparing `otoe-0.0.7a0.tar` & `otoe-0.0.7a1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:33:25.343254 otoe-0.0.7a0/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:33:25.343119 otoe-0.0.7a0/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7a0/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:33:25.341453 otoe-0.0.7a0/otoe/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:33:25.342725 otoe-0.0.7a0/otoe/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:33:25.000000 otoe-0.0.7a0/otoe/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      186 2023-04-17 05:33:25.000000 otoe-0.0.7a0/otoe/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 05:33:25.000000 otoe-0.0.7a0/otoe/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       44 2023-04-17 05:33:25.000000 otoe-0.0.7a0/otoe/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-17 05:33:25.000000 otoe-0.0.7a0/otoe/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 05:33:25.343297 otoe-0.0.7a0/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1292 2023-04-17 05:33:19.000000 otoe-0.0.7a0/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.007036 otoe-0.0.7a1/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:42:20.006905 otoe-0.0.7a1/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7a1/README.md
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 05:42:20.007077 otoe-0.0.7a1/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1287 2023-04-17 05:42:18.000000 otoe-0.0.7a1/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.005704 otoe-0.0.7a1/src/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.005762 otoe-0.0.7a1/src/otoe/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:42:20.006711 otoe-0.0.7a1/src/otoe/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      206 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       35 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-17 05:42:19.000000 otoe-0.0.7a1/src/otoe/otoe.egg-info/top_level.txt
```

### Comparing `otoe-0.0.7a0/PKG-INFO` & `otoe-0.0.7a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7a0
+Version: 0.0.7a1
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7a0/README.md` & `otoe-0.0.7a1/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7a0/otoe/otoe.egg-info/PKG-INFO` & `otoe-0.0.7a1/src/otoe/otoe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7a0
+Version: 0.0.7a1
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7a0/setup.py` & `otoe-0.0.7a1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.7a0",                        # The initial release version
+    version="0.0.7a1",                        # The initial release version
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
-    package_dir={'': 'otoe'},     # Directory of the source code of the package
+    package_dir={'': 'src/otoe'},     # Directory of the source code of the package
     install_requires=[],                     # Install other dependencies if any
     entry_points={
         'console_scripts': [
-            'otoe=otoe.obsidian:main',
+            'otoe=otoe:main',
        ],
     }
 )
```

