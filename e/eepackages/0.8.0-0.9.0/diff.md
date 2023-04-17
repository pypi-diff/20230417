# Comparing `tmp/eepackages-0.8.0.tar.gz` & `tmp/eepackages-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eepackages-0.8.0.tar", last modified: Thu Nov 18 08:57:59 2021, max compression
+gzip compressed data, was "eepackages-0.9.0.tar", last modified: Thu Nov 25 17:36:08 2021, max compression
```

## Comparing `eepackages-0.8.0.tar` & `eepackages-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 08:57:59.564179 eepackages-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-11-18 08:57:41.000000 eepackages-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-11-18 08:57:59.564179 eepackages-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-11-18 08:57:41.000000 eepackages-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 08:57:59.564179 eepackages-0.8.0/eepackages/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 08:57:59.564179 eepackages-0.8.0/eepackages/applications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15616 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/applications/bathymetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     4668 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/applications/waterbody_area.py
--rw-r--r--   0 runner    (1001) docker     (121)    17250 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/assets.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/gl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/tiler.py
--rw-r--r--   0 runner    (1001) docker     (121)    11074 2021-11-18 08:57:41.000000 eepackages-0.8.0/eepackages/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 08:57:59.564179 eepackages-0.8.0/eepackages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-11-18 08:57:59.000000 eepackages-0.8.0/eepackages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      412 2021-11-18 08:57:59.000000 eepackages-0.8.0/eepackages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 08:57:59.000000 eepackages-0.8.0/eepackages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 08:57:59.000000 eepackages-0.8.0/eepackages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-18 08:57:59.000000 eepackages-0.8.0/eepackages.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 08:57:59.564179 eepackages-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-11-18 08:57:50.000000 eepackages-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 17:36:08.272266 eepackages-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2021-11-25 17:35:57.000000 eepackages-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-11-25 17:36:08.272266 eepackages-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-11-25 17:35:57.000000 eepackages-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 17:36:08.272266 eepackages-0.9.0/eepackages/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 17:36:08.272266 eepackages-0.9.0/eepackages/applications/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15616 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/applications/bathymetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4675 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/applications/waterbody_area.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17250 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/assets.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/gl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/tiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11074 2021-11-25 17:35:57.000000 eepackages-0.9.0/eepackages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 17:36:08.272266 eepackages-0.9.0/eepackages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-11-25 17:36:08.000000 eepackages-0.9.0/eepackages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2021-11-25 17:36:08.000000 eepackages-0.9.0/eepackages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-25 17:36:08.000000 eepackages-0.9.0/eepackages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-25 17:36:08.000000 eepackages-0.9.0/eepackages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-25 17:36:08.000000 eepackages-0.9.0/eepackages.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-25 17:36:08.272266 eepackages-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-11-25 17:36:00.000000 eepackages-0.9.0/setup.py
```

### Comparing `eepackages-0.8.0/LICENSE` & `eepackages-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eepackages-0.8.0/PKG-INFO` & `eepackages-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eepackages
-Version: 0.8.0
+Version: 0.9.0
 Summary: A set of utilities built on top of Google Earth Engine (migrated from JavaScript)
 Home-page: https://github.com/gee-community/ee-packages-py
 Author: Gennadii Donchyts
 Author-email: gennadiy.donchyts@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `eepackages-0.8.0/README.md` & `eepackages-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `eepackages-0.8.0/eepackages/applications/bathymetry.py` & `eepackages-0.9.0/eepackages/applications/bathymetry.py`

 * *Files identical despite different names*

### Comparing `eepackages-0.8.0/eepackages/applications/waterbody_area.py` & `eepackages-0.9.0/eepackages/applications/waterbody_area.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     
   p = ee.Algorithms.If(ee.Algorithms.IsEqual(p, None), 101, p)
 
   waterFill = (waterOccurrence.gt(ee.Image.constant(p))
     .updateMask(water.unmask(0, False).Not()))
     
   # exclude false-positive, where we're sure in a non-water
-  nonWater = ndwi.lt(-0.15).unmask(0)
+  nonWater = ndwi.lt(-0.15).unmask(0, False)
   waterFill = waterFill.updateMask(nonWater.Not())
   
   fill = (ee.Image.pixelArea().mask(waterFill)
     .reduceRegion(**{
       'reducer': ee.Reducer.sum(),
       'geometry': geom,
       'scale': scale
```

### Comparing `eepackages-0.8.0/eepackages/assets.py` & `eepackages-0.9.0/eepackages/assets.py`

 * *Files identical despite different names*

### Comparing `eepackages-0.8.0/eepackages/tiler.py` & `eepackages-0.9.0/eepackages/tiler.py`

 * *Files identical despite different names*

### Comparing `eepackages-0.8.0/eepackages/utils.py` & `eepackages-0.9.0/eepackages/utils.py`

 * *Files identical despite different names*

### Comparing `eepackages-0.8.0/eepackages.egg-info/PKG-INFO` & `eepackages-0.9.0/eepackages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eepackages
-Version: 0.8.0
+Version: 0.9.0
 Summary: A set of utilities built on top of Google Earth Engine (migrated from JavaScript)
 Home-page: https://github.com/gee-community/ee-packages-py
 Author: Gennadii Donchyts
 Author-email: gennadiy.donchyts@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `eepackages-0.8.0/setup.py` & `eepackages-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import os
 import re
 
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 def read(filename):
     filename = os.path.join(os.path.dirname(__file__), filename)
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
```

