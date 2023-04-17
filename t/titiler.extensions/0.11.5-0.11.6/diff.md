# Comparing `tmp/titiler.extensions-0.11.5.tar.gz` & `tmp/titiler.extensions-0.11.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.extensions-0.11.5.tar", last modified: Wed Mar 22 16:34:27 2023, max compression
+gzip compressed data, was "titiler.extensions-0.11.6.tar", last modified: Mon Apr 17 11:02:26 2023, max compression
```

## Comparing `titiler.extensions-0.11.5.tar` & `titiler.extensions-0.11.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4700 2023-03-22 16:33:47.419052 titiler.extensions-0.11.5/README.md
--rw-r--r--   0        0        0     1656 2023-03-22 16:33:47.419052 titiler.extensions-0.11.5/pyproject.toml
--rw-r--r--   0        0        0      244 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/__init__.py
--rw-r--r--   0        0        0     1011 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/cogeo.py
--rw-r--r--   0        0        0     5274 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/stac.py
--rw-r--r--   0        0        0    29081 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/templates/cog_index.html
--rw-r--r--   0        0        0    33552 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/templates/stac_index.html
--rw-r--r--   0        0        0     2231 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/templates/wms_1.0.0.xml
--rw-r--r--   0        0        0     2715 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/templates/wms_1.1.1.xml
--rw-r--r--   0        0        0     3452 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/templates/wms_1.3.0.xml
--rw-r--r--   0        0        0     2320 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/viewer.py
--rw-r--r--   0        0        0    20973 2023-03-22 16:33:47.435052 titiler.extensions-0.11.5/titiler/extensions/wms.py
--rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 titiler.extensions-0.11.5/PKG-INFO
+-rw-r--r--   0        0        0     4700 2023-04-17 11:01:43.800545 titiler.extensions-0.11.6/README.md
+-rw-r--r--   0        0        0     1656 2023-04-17 11:01:43.800545 titiler.extensions-0.11.6/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/__init__.py
+-rw-r--r--   0        0        0     1011 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/cogeo.py
+-rw-r--r--   0        0        0     5274 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/stac.py
+-rw-r--r--   0        0        0    29081 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/cog_index.html
+-rw-r--r--   0        0        0    33552 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/stac_index.html
+-rw-r--r--   0        0        0     2231 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.0.0.xml
+-rw-r--r--   0        0        0     2715 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.1.1.xml
+-rw-r--r--   0        0        0     3452 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.3.0.xml
+-rw-r--r--   0        0        0     2320 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/viewer.py
+-rw-r--r--   0        0        0    20973 2023-04-17 11:01:43.816545 titiler.extensions-0.11.6/titiler/extensions/wms.py
+-rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 titiler.extensions-0.11.6/PKG-INFO
```

### Comparing `titiler.extensions-0.11.5/README.md` & `titiler.extensions-0.11.6/README.md`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/pyproject.toml` & `titiler.extensions-0.11.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = []
 dependencies = [
-    "titiler.core==0.11.5",
+    "titiler.core==0.11.6",
 ]
-version = "0.11.5"
+version = "0.11.6"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 test = [
     "pytest",
```

### Comparing `titiler.extensions-0.11.5/titiler/extensions/cogeo.py` & `titiler.extensions-0.11.6/titiler/extensions/cogeo.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/stac.py` & `titiler.extensions-0.11.6/titiler/extensions/stac.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/templates/cog_index.html` & `titiler.extensions-0.11.6/titiler/extensions/templates/cog_index.html`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/templates/stac_index.html` & `titiler.extensions-0.11.6/titiler/extensions/templates/stac_index.html`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/templates/wms_1.0.0.xml` & `titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/templates/wms_1.1.1.xml` & `titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.1.1.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/templates/wms_1.3.0.xml` & `titiler.extensions-0.11.6/titiler/extensions/templates/wms_1.3.0.xml`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/viewer.py` & `titiler.extensions-0.11.6/titiler/extensions/viewer.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/titiler/extensions/wms.py` & `titiler.extensions-0.11.6/titiler/extensions/wms.py`

 * *Files identical despite different names*

### Comparing `titiler.extensions-0.11.5/PKG-INFO` & `titiler.extensions-0.11.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.extensions
-Version: 0.11.5
+Version: 0.11.6
 Summary: Extensions for TiTiler Factories.
 License: MIT
 Keywords: COG,STAC,MosaicJSON,Fastapi,Dynamic tile server,GDAL,Rasterio,OGC
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

