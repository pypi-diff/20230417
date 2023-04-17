# Comparing `tmp/otoe-0.0.7.post1.tar.gz` & `tmp/otoe-0.0.7.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.7.post1.tar", last modified: Sun Apr 16 20:53:03 2023, max compression
+gzip compressed data, was "otoe-0.0.7.post2.tar", last modified: Mon Apr 17 05:05:54 2023, max compression
```

## Comparing `otoe-0.0.7.post1.tar` & `otoe-0.0.7.post2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.792889 otoe-0.0.7.post1/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-16 20:53:03.792756 otoe-0.0.7.post1/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7.post1/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.791309 otoe-0.0.7.post1/otoe/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.791369 otoe-0.0.7.post1/otoe/src/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.791425 otoe-0.0.7.post1/otoe/src/otoe_epicker/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.792549 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      835 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-16 20:53:03.792934 otoe-0.0.7.post1/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1391 2023-04-16 20:51:08.000000 otoe-0.0.7.post1/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:05:54.231212 otoe-0.0.7.post2/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-17 05:05:54.231044 otoe-0.0.7.post2/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7.post2/README.md
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:05:54.229745 otoe-0.0.7.post2/otoe/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:05:54.229803 otoe-0.0.7.post2/otoe/src/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:05:54.229857 otoe-0.0.7.post2/otoe/src/otoe_epicker/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-17 05:05:54.230827 otoe-0.0.7.post2/otoe/src/otoe_epicker/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-17 05:05:54.000000 otoe-0.0.7.post2/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      271 2023-04-17 05:05:54.000000 otoe-0.0.7.post2/otoe/src/otoe_epicker/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-17 05:05:54.000000 otoe-0.0.7.post2/otoe/src/otoe_epicker/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-17 05:05:54.000000 otoe-0.0.7.post2/otoe/src/otoe_epicker/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-17 05:05:54.000000 otoe-0.0.7.post2/otoe/src/otoe_epicker/otoe.egg-info/top_level.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-17 05:05:54.231257 otoe-0.0.7.post2/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1391 2023-04-17 05:05:50.000000 otoe-0.0.7.post2/setup.py
```

### Comparing `otoe-0.0.7.post1/PKG-INFO` & `otoe-0.0.7.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7.post1
+Version: 0.0.7.post2
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7.post1/README.md` & `otoe-0.0.7.post2/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO` & `otoe-0.0.7.post2/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7.post1
+Version: 0.0.7.post2
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7.post1/setup.py` & `otoe-0.0.7.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 srcpath = str(Path(__file__).parent / 'src' / 'otoe_epicker')
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.7_1",                        # The initial release version
+    version="0.0.7_2",                        # The initial release version
     author="Yakov Varnaev",                     # Full name of the author
     description="Sort of a UI for espanso configs.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

