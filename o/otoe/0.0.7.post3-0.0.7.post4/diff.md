# Comparing `tmp/otoe-0.0.7.post3.tar.gz` & `tmp/otoe-0.0.7.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.7.post3.tar", last modified: Mon Apr 17 05:12:17 2023, max compression
+gzip compressed data, was "otoe-0.0.7.post4.tar", last modified: Mon Apr 17 05:15:37 2023, max compression
```

## Comparing `otoe-0.0.7.post3.tar` & `otoe-0.0.7.post4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:12:17.131286 otoe-0.0.7.post3/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-17 05:12:17.131162 otoe-0.0.7.post3/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7.post3/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:12:17.130015 otoe-0.0.7.post3/otoe/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:12:17.130073 otoe-0.0.7.post3/otoe/src/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:12:17.130978 otoe-0.0.7.post3/otoe/src/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-17 05:12:17.000000 otoe-0.0.7.post3/otoe/src/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      206 2023-04-17 05:12:17.000000 otoe-0.0.7.post3/otoe/src/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 05:12:17.000000 otoe-0.0.7.post3/otoe/src/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       44 2023-04-17 05:12:17.000000 otoe-0.0.7.post3/otoe/src/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-17 05:12:17.000000 otoe-0.0.7.post3/otoe/src/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 05:12:17.131335 otoe-0.0.7.post3/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1383 2023-04-17 05:12:14.000000 otoe-0.0.7.post3/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:15:37.922169 otoe-0.0.7.post4/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-17 05:15:37.922028 otoe-0.0.7.post4/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7.post4/README.md
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:15:37.920777 otoe-0.0.7.post4/otoe/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:15:37.920832 otoe-0.0.7.post4/otoe/src/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:15:37.920889 otoe-0.0.7.post4/otoe/src/otoe/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:15:37.921832 otoe-0.0.7.post4/otoe/src/otoe/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-17 05:15:37.000000 otoe-0.0.7.post4/otoe/src/otoe/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      231 2023-04-17 05:15:37.000000 otoe-0.0.7.post4/otoe/src/otoe/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 05:15:37.000000 otoe-0.0.7.post4/otoe/src/otoe/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       53 2023-04-17 05:15:37.000000 otoe-0.0.7.post4/otoe/src/otoe/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-17 05:15:37.000000 otoe-0.0.7.post4/otoe/src/otoe/otoe.egg-info/top_level.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 05:15:37.922209 otoe-0.0.7.post4/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1398 2023-04-17 05:15:01.000000 otoe-0.0.7.post4/setup.py
```

### Comparing `otoe-0.0.7.post3/PKG-INFO` & `otoe-0.0.7.post4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7.post3
+Version: 0.0.7.post4
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7.post3/README.md` & `otoe-0.0.7.post4/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7.post3/otoe/src/otoe.egg-info/PKG-INFO` & `otoe-0.0.7.post4/otoe/src/otoe/otoe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7.post3
+Version: 0.0.7.post4
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7.post3/setup.py` & `otoe-0.0.7.post4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 srcpath = str(Path(__file__).parent / 'src' / 'otoe_epicker')
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.7_3",                        # The initial release version
+    version="0.0.7_4",                        # The initial release version
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
     py_modules=["otoe"],             # Name of the python package
-    package_dir={'': 'otoe/src'},     # Directory of the source code of the package
+    package_dir={'': 'otoe/src/otoe/'},     # Directory of the source code of the package
     install_requires=[],                     # Install other dependencies if any
     entry_points={
         'console_scripts': [
-            'otoe=otoe.obsidian:main',
+            'otoe=otoe.src.otoe.obsidian:main',
        ],
     }
 )
```

