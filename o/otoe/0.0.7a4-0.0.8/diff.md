# Comparing `tmp/otoe-0.0.7a4.tar.gz` & `tmp/otoe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.7a4.tar", last modified: Mon Apr 17 14:58:39 2023, max compression
+gzip compressed data, was "otoe-0.0.8.tar", last modified: Mon Apr 17 15:00:23 2023, max compression
```

## Comparing `otoe-0.0.7a4.tar` & `otoe-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 14:58:39.420283 otoe-0.0.7a4/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 14:58:39.420004 otoe-0.0.7a4/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7a4/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 14:58:39.417779 otoe-0.0.7a4/otoe/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      559 2023-04-17 14:58:04.000000 otoe-0.0.7a4/otoe/__init__.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-17 05:25:00.000000 otoe-0.0.7a4/otoe/config.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1153 2023-04-17 05:25:00.000000 otoe-0.0.7a4/otoe/exceptions.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     5034 2023-04-17 05:40:12.000000 otoe-0.0.7a4/otoe/obsidian.py
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 14:58:39.418715 otoe-0.0.7a4/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      962 2023-04-17 14:58:39.000000 otoe-0.0.7a4/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      283 2023-04-17 14:58:39.000000 otoe-0.0.7a4/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 14:58:39.000000 otoe-0.0.7a4/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       35 2023-04-17 14:58:39.000000 otoe-0.0.7a4/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       11 2023-04-17 14:58:39.000000 otoe-0.0.7a4/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 14:58:39.420392 otoe-0.0.7a4/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1291 2023-04-17 14:58:37.000000 otoe-0.0.7a4/setup.py
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 14:58:39.419433 otoe-0.0.7a4/tests/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        0 2023-04-09 15:50:13.000000 otoe-0.0.7a4/tests/__init__.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2260 2023-04-17 05:26:48.000000 otoe-0.0.7a4/tests/test_md.py
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2949 2023-04-17 05:27:00.000000 otoe-0.0.7a4/tests/test_otoe.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.760335 otoe-0.0.8/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-17 15:00:23.760175 otoe-0.0.8/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.8/README.md
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.758354 otoe-0.0.8/otoe/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      559 2023-04-17 14:58:04.000000 otoe-0.0.8/otoe/__init__.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-17 05:25:00.000000 otoe-0.0.8/otoe/config.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1153 2023-04-17 05:25:00.000000 otoe-0.0.8/otoe/exceptions.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     5034 2023-04-17 05:40:12.000000 otoe-0.0.8/otoe/obsidian.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.759281 otoe-0.0.8/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      310 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       35 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        7 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/requires.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       11 2023-04-17 15:00:23.000000 otoe-0.0.8/otoe.egg-info/top_level.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 15:00:23.760377 otoe-0.0.8/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1297 2023-04-17 15:00:20.000000 otoe-0.0.8/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 15:00:23.759785 otoe-0.0.8/tests/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        0 2023-04-09 15:50:13.000000 otoe-0.0.8/tests/__init__.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2260 2023-04-17 05:26:48.000000 otoe-0.0.8/tests/test_md.py
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     2949 2023-04-17 05:27:00.000000 otoe-0.0.8/tests/test_otoe.py
```

### Comparing `otoe-0.0.7a4/PKG-INFO` & `otoe-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7a4
+Version: 0.0.8
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7a4/README.md` & `otoe-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7a4/otoe/__init__.py` & `otoe-0.0.8/otoe/__init__.py`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7a4/otoe/exceptions.py` & `otoe-0.0.8/otoe/exceptions.py`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7a4/otoe/obsidian.py` & `otoe-0.0.8/otoe/obsidian.py`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7a4/otoe.egg-info/PKG-INFO` & `otoe-0.0.8/otoe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7a4
+Version: 0.0.8
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7a4/setup.py` & `otoe-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.7a4",                        # The initial release version
+    version="0.0.8",                        # The initial release version
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
     # py_modules=['obsidian'],             # Name of the python package
     # package_dir={'': 'otoe'},     # Directory of the source code of the package
-    install_requires=[],                     # Install other dependencies if any
+    install_requires=['pyyaml'],                     # Install other dependencies if any
     entry_points={
         'console_scripts': [
             'otoe=otoe:main',
        ],
     }
 )
```

### Comparing `otoe-0.0.7a4/tests/test_md.py` & `otoe-0.0.8/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7a4/tests/test_otoe.py` & `otoe-0.0.8/tests/test_otoe.py`

 * *Files identical despite different names*

