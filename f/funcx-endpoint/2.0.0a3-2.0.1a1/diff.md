# Comparing `tmp/funcx-endpoint-2.0.0a3.tar.gz` & `tmp/funcx-endpoint-2.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-endpoint-2.0.0a3.tar", last modified: Mon Apr  3 22:38:32 2023, max compression
+gzip compressed data, was "funcx-endpoint-2.0.1a1.tar", last modified: Mon Apr 17 19:13:52 2023, max compression
```

## Comparing `funcx-endpoint-2.0.0a3.tar` & `funcx-endpoint-2.0.1a1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:38:32.663210 funcx-endpoint-2.0.0a3/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-03 17:17:07.000000 funcx-endpoint-2.0.0a3/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      686 2023-04-03 22:38:32.663254 funcx-endpoint-2.0.0a3/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      419 2023-04-03 17:17:07.000000 funcx-endpoint-2.0.0a3/README.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:38:32.662217 funcx-endpoint-2.0.0a3/funcx_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      244 2023-04-03 20:00:27.000000 funcx-endpoint-2.0.0a3/funcx_endpoint/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:38:32.663101 funcx-endpoint-2.0.0a3/funcx_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      238 2023-04-03 22:03:08.000000 funcx-endpoint-2.0.0a3/funcx_endpoint/executors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      245 2023-04-03 22:38:18.000000 funcx-endpoint-2.0.0a3/funcx_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:38:32.662960 funcx-endpoint-2.0.0a3/funcx_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      686 2023-04-03 22:38:32.000000 funcx-endpoint-2.0.0a3/funcx_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      356 2023-04-03 22:38:32.000000 funcx-endpoint-2.0.0a3/funcx_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-03 22:38:32.000000 funcx-endpoint-2.0.0a3/funcx_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      329 2023-04-03 22:38:32.000000 funcx-endpoint-2.0.0a3/funcx_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)       33 2023-04-03 22:38:32.000000 funcx-endpoint-2.0.0a3/funcx_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       15 2023-04-03 22:38:32.000000 funcx-endpoint-2.0.0a3/funcx_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-03 22:38:32.663470 funcx-endpoint-2.0.0a3/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     1639 2023-04-03 22:37:53.000000 funcx-endpoint-2.0.0a3/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.117795 funcx-endpoint-2.0.1a1/
+-rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 19:06:42.000000 funcx-endpoint-2.0.1a1/MANIFEST.in
+-rw-r--r--   0 chris      (501) staff       (20)     1842 2023-04-17 19:13:52.117871 funcx-endpoint-2.0.1a1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     1115 2023-04-17 18:38:33.000000 funcx-endpoint-2.0.1a1/PyPI.md
+-rw-r--r--   0 chris      (501) staff       (20)      430 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.116448 funcx-endpoint-2.0.1a1/funcx_endpoint/
+-rw-r--r--   0 chris      (501) staff       (20)      122 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/funcx_endpoint/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.117581 funcx-endpoint-2.0.1a1/funcx_endpoint/executors/
+-rw-r--r--   0 chris      (501) staff       (20)      107 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/funcx_endpoint/executors/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      245 2023-04-17 19:06:42.000000 funcx-endpoint-2.0.1a1/funcx_endpoint/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.117431 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     1842 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      376 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      329 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)       31 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       15 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      305 2023-04-17 19:13:52.118203 funcx-endpoint-2.0.1a1/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     1776 2023-04-17 18:38:33.000000 funcx-endpoint-2.0.1a1/setup.py
```

### Comparing `funcx-endpoint-2.0.0a3/LICENSE` & `funcx-endpoint-2.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.0a3/setup.py` & `funcx-endpoint-2.0.1a1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import os
+from pathlib import Path
 
 from setuptools import find_packages, setup
 
-compute_endpoint_path = "/Users/lei/glob/funcX/compute_endpoint"
-
 REQUIRES = [
-    "globus-compute-endpoint>=2.0.0a1",
+    "globus-compute-endpoint>=2.0.0",
 ]
 
 version_ns = {}
 with open(os.path.join("funcx_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
 
+directory = Path(__file__).parent
+long_description = (directory / "PyPI.md").read_text()
+
 setup(
     name="funcx-endpoint",
     version=version,
     packages=find_packages(),
     description="funcX: High Performance Function Serving for Science",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     install_requires=REQUIRES,
     extras_require={},
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
```

