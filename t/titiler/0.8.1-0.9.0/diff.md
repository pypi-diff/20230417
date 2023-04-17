# Comparing `tmp/titiler-0.8.1.tar.gz` & `tmp/titiler-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler-0.8.1.tar", last modified: Thu Dec  1 15:56:07 2022, max compression
+gzip compressed data, was "titiler-0.9.0.tar", last modified: Mon Dec  5 17:00:53 2022, max compression
```

## Comparing `titiler-0.8.1.tar` & `titiler-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:07.950455 titiler-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2022-12-01 15:55:48.000000 titiler-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-12-01 15:55:48.000000 titiler-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6707 2022-12-01 15:56:07.950455 titiler-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5940 2022-12-01 15:55:48.000000 titiler-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 15:56:07.950455 titiler-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2022-12-01 15:55:48.000000 titiler-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:07.950455 titiler-0.8.1/titiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6707 2022-12-01 15:56:07.000000 titiler-0.8.1/titiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      222 2022-12-01 15:56:07.000000 titiler-0.8.1/titiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:07.000000 titiler-0.8.1/titiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:07.000000 titiler-0.8.1/titiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       69 2022-12-01 15:56:07.000000 titiler-0.8.1/titiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:07.000000 titiler-0.8.1/titiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:53.898921 titiler-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2022-12-05 17:00:39.000000 titiler-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-05 17:00:39.000000 titiler-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2022-12-05 17:00:53.898921 titiler-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2022-12-05 17:00:39.000000 titiler-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-05 17:00:53.898921 titiler-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2022-12-05 17:00:39.000000 titiler-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:53.898921 titiler-0.9.0/titiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2022-12-05 17:00:53.000000 titiler-0.9.0/titiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-05 17:00:53.000000 titiler-0.9.0/titiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:53.000000 titiler-0.9.0/titiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:53.000000 titiler-0.9.0/titiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-05 17:00:53.000000 titiler-0.9.0/titiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:53.000000 titiler-0.9.0/titiler.egg-info/top_level.txt
```

### Comparing `titiler-0.8.1/LICENSE` & `titiler-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `titiler-0.8.1/PKG-INFO` & `titiler-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC MosaicJSON FastAPI Tile Server Dynamic
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler Version: 0.8.1 Summary: A modern dynamic
+Metadata-Version: 2.1 Name: titiler Version: 0.9.0 Summary: A modern dynamic
 tile server built on top of FastAPI and Rasterio/GDAL. Home-page: https://
 github.com/developmentseed/titiler Author: Vincent Sarago Author-email:
 vincent@developmentseed.org License: MIT Keywords: COG STAC MosaicJSON FastAPI
 Tile Server Dynamic Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `titiler-0.8.1/README.md` & `titiler-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `titiler-0.8.1/setup.py` & `titiler-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup titiler metapackage."""
 
 from setuptools import setup
 
 with open("README.md") as f:
     long_description = f.read()
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 inst_reqs = [
     f"titiler.core=={__version__}",
     f"titiler.mosaic=={__version__}",
     f"titiler.application=={__version__}",
 ]
```

### Comparing `titiler-0.8.1/titiler.egg-info/PKG-INFO` & `titiler-0.9.0/titiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC MosaicJSON FastAPI Tile Server Dynamic
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: titiler Version: 0.8.1 Summary: A modern dynamic
+Metadata-Version: 2.1 Name: titiler Version: 0.9.0 Summary: A modern dynamic
 tile server built on top of FastAPI and Rasterio/GDAL. Home-page: https://
 github.com/developmentseed/titiler Author: Vincent Sarago Author-email:
 vincent@developmentseed.org License: MIT Keywords: COG STAC MosaicJSON FastAPI
 Tile Server Dynamic Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

