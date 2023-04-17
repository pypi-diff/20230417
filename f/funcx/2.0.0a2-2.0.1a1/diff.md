# Comparing `tmp/funcx-2.0.0a2.tar.gz` & `tmp/funcx-2.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-2.0.0a2.tar", last modified: Mon Apr  3 22:17:32 2023, max compression
+gzip compressed data, was "funcx-2.0.1a1.tar", last modified: Mon Apr 17 19:13:34 2023, max compression
```

## Comparing `funcx-2.0.0a2.tar` & `funcx-2.0.1a1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:17:32.808566 funcx-2.0.0a2/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-03 17:17:07.000000 funcx-2.0.0a2/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      665 2023-04-03 22:17:32.808616 funcx-2.0.0a2/PKG-INFO
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:17:32.807763 funcx-2.0.0a2/funcx/
--rw-r--r--   0 lei        (501) staff       (20)      467 2023-04-03 20:00:27.000000 funcx-2.0.0a2/funcx/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:17:32.808458 funcx-2.0.0a2/funcx/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-04-03 20:00:27.000000 funcx-2.0.0a2/funcx/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1146 2023-04-03 22:17:20.000000 funcx-2.0.0a2/funcx/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:17:32.808337 funcx-2.0.0a2/funcx.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      665 2023-04-03 22:17:32.000000 funcx-2.0.0a2/funcx.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      233 2023-04-03 22:17:32.000000 funcx-2.0.0a2/funcx.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-03 22:17:32.000000 funcx-2.0.0a2/funcx.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)       28 2023-04-03 22:17:32.000000 funcx-2.0.0a2/funcx.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)        6 2023-04-03 22:17:32.000000 funcx-2.0.0a2/funcx.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-03 22:17:32.808845 funcx-2.0.0a2/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     1468 2023-04-03 22:13:58.000000 funcx-2.0.0a2/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.854456 funcx-2.0.1a1/
+-rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 funcx-2.0.1a1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 19:06:42.000000 funcx-2.0.1a1/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     1797 2023-04-17 19:13:34.854534 funcx-2.0.1a1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     1051 2023-04-17 18:38:33.000000 funcx-2.0.1a1/PyPI.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.853217 funcx-2.0.1a1/funcx/
+-rw-r--r--   0 chris      (501) staff       (20)      467 2023-04-12 14:51:48.000000 funcx-2.0.1a1/funcx/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.854240 funcx-2.0.1a1/funcx/serialize/
+-rw-r--r--   0 chris      (501) staff       (20)      110 2023-04-12 14:51:48.000000 funcx-2.0.1a1/funcx/serialize/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1146 2023-04-17 19:06:42.000000 funcx-2.0.1a1/funcx/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:34.854082 funcx-2.0.1a1/funcx.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     1797 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      253 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       26 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)        6 2023-04-17 19:13:34.000000 funcx-2.0.1a1/funcx.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      305 2023-04-17 19:13:34.854866 funcx-2.0.1a1/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     1659 2023-04-17 18:38:33.000000 funcx-2.0.1a1/setup.py
```

### Comparing `funcx-2.0.0a2/LICENSE` & `funcx-2.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-2.0.0a2/funcx/version.py` & `funcx-2.0.1a1/funcx/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.0a2"
+__version__ = "2.0.1a1"
 
 DEPRECATION_FUNCX = """
 The funcX SDK has been renamed to Globus Compute SDK and the new package is
 available on PyPI:
     https://pypi.org/project/globus-compute-sdk/
 
 Please consider upgrading to Globus Compute.  More information can be found at:
```

### Comparing `funcx-2.0.0a2/setup.py` & `funcx-2.0.1a1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import re
+from pathlib import Path
 
 from setuptools import find_packages, setup
 
-compute_sdk_path = "/Users/lei/glob/funcX/compute_sdk"
-
 REQUIRES = [
-    "globus-compute-sdk>=2.0.0a1",
+    "globus-compute-sdk>=2.0.0",
 ]
 
 
 def parse_version():
     # single source of truth for package version
     version_string = ""
     version_pattern = re.compile(r'__version__ = "([^"]*)"')
@@ -21,30 +20,36 @@
                 version_string = match.group(1)
                 break
     if not version_string:
         raise RuntimeError("Failed to parse version information")
     return version_string
 
 
+directory = Path(__file__).parent
+long_description = (directory / "PyPI.md").read_text()
+
+
 setup(
     name="funcx",
     version=parse_version(),
     packages=find_packages(),
-    description="funcX: High Performance Function Serving for Science",
+    description="Globus Compute: High Performance Function Serving for Science",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=REQUIRES,
     extras_require={},
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
     ],
-    keywords=["funcX", "FaaS", "Function Serving"],
-    author="funcX team",
-    author_email="labs@globus.org",
+    keywords=["funcX", "FaaS", "Function Serving", "Globus Compute"],
+    author="The Globus Compute Team",
+    author_email="support@globus.org",
     license="Apache License, Version 2.0",
     url="https://github.com/funcx-faas/funcx",
 )
```

