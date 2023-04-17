# Comparing `tmp/titiler.application-0.8.1.tar.gz` & `tmp/titiler.application-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.application-0.8.1.tar", last modified: Thu Dec  1 15:56:05 2022, max compression
+gzip compressed data, was "titiler.application-0.9.0.tar", last modified: Mon Dec  5 17:00:51 2022, max compression
```

## Comparing `titiler.application-0.8.1.tar` & `titiler.application-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:05.598462 titiler.application-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2022-12-01 15:55:48.000000 titiler.application-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2022-12-01 15:56:05.598462 titiler.application-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2022-12-01 15:55:48.000000 titiler.application-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-12-01 15:55:48.000000 titiler.application-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       98 2022-12-01 15:56:05.598462 titiler.application-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2022-12-01 15:55:48.000000 titiler.application-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:05.598462 titiler.application-0.8.1/titiler/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:05.598462 titiler.application-0.8.1/titiler/application/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-01 15:55:48.000000 titiler.application-0.8.1/titiler/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6304 2022-12-01 15:55:48.000000 titiler.application-0.8.1/titiler/application/main.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2022-12-01 15:55:48.000000 titiler.application-0.8.1/titiler/application/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:05.598462 titiler.application-0.8.1/titiler/application/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    27359 2022-12-01 15:55:48.000000 titiler.application-0.8.1/titiler/application/templates/cog_index.html
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2022-12-01 15:55:48.000000 titiler.application-0.8.1/titiler/application/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (122)    31524 2022-12-01 15:55:48.000000 titiler.application-0.8.1/titiler/application/templates/stac_index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:05.598462 titiler.application-0.8.1/titiler.application.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2022-12-01 15:56:05.000000 titiler.application-0.8.1/titiler.application.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      535 2022-12-01 15:56:05.000000 titiler.application-0.8.1/titiler.application.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:05.000000 titiler.application-0.8.1/titiler.application.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:05.000000 titiler.application-0.8.1/titiler.application.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      210 2022-12-01 15:56:05.000000 titiler.application-0.8.1/titiler.application.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-12-01 15:56:05.000000 titiler.application-0.8.1/titiler.application.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:51.482932 titiler.application-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-05 17:00:39.000000 titiler.application-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2022-12-05 17:00:51.482932 titiler.application-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2022-12-05 17:00:39.000000 titiler.application-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-05 17:00:39.000000 titiler.application-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-05 17:00:51.482932 titiler.application-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2022-12-05 17:00:39.000000 titiler.application-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:51.482932 titiler.application-0.9.0/titiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:51.482932 titiler.application-0.9.0/titiler/application/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-05 17:00:39.000000 titiler.application-0.9.0/titiler/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2022-12-05 17:00:39.000000 titiler.application-0.9.0/titiler/application/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-05 17:00:39.000000 titiler.application-0.9.0/titiler/application/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:51.482932 titiler.application-0.9.0/titiler/application/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    27359 2022-12-05 17:00:39.000000 titiler.application-0.9.0/titiler/application/templates/cog_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2022-12-05 17:00:39.000000 titiler.application-0.9.0/titiler/application/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    31524 2022-12-05 17:00:39.000000 titiler.application-0.9.0/titiler/application/templates/stac_index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:51.482932 titiler.application-0.9.0/titiler.application.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2022-12-05 17:00:51.000000 titiler.application-0.9.0/titiler.application.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-05 17:00:51.000000 titiler.application-0.9.0/titiler.application.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:51.000000 titiler.application-0.9.0/titiler.application.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:51.000000 titiler.application-0.9.0/titiler.application.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2022-12-05 17:00:51.000000 titiler.application-0.9.0/titiler.application.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-05 17:00:51.000000 titiler.application-0.9.0/titiler.application.egg-info/top_level.txt
```

### Comparing `titiler.application-0.8.1/PKG-INFO` & `titiler.application-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.application
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC MosaicJSON FastAPI
 Classifier: Intended Audience :: Information Technology
```

### Comparing `titiler.application-0.8.1/README.md` & `titiler.application-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `titiler.application-0.8.1/setup.py` & `titiler.application-0.9.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 inst_reqs = [
     "rio-cogeo>=3.1,<4.0",
-    "titiler.core>=0.8,<0.9",
-    "titiler.mosaic>=0.8,<0.9",
+    "titiler.core>=0.9,<0.10",
+    "titiler.mosaic>=0.9,<0.10",
     "starlette-cramjam>=0.3,<0.4",
     "python-dotenv",
 ]
 extra_reqs = {
     "test": ["pytest", "pytest-cov", "pytest-asyncio", "httpx", "brotlipy"],
     "server": ["uvicorn[standard]>=0.12.0,<0.19.0"],
 }
```

### Comparing `titiler.application-0.8.1/titiler/application/main.py` & `titiler.application-0.9.0/titiler/application/main.py`

 * *Files identical despite different names*

### Comparing `titiler.application-0.8.1/titiler/application/settings.py` & `titiler.application-0.9.0/titiler/application/settings.py`

 * *Files identical despite different names*

### Comparing `titiler.application-0.8.1/titiler/application/templates/cog_index.html` & `titiler.application-0.9.0/titiler/application/templates/cog_index.html`

 * *Files identical despite different names*

### Comparing `titiler.application-0.8.1/titiler/application/templates/index.html` & `titiler.application-0.9.0/titiler/application/templates/index.html`

 * *Files identical despite different names*

### Comparing `titiler.application-0.8.1/titiler/application/templates/stac_index.html` & `titiler.application-0.9.0/titiler/application/templates/stac_index.html`

 * *Files identical despite different names*

### Comparing `titiler.application-0.8.1/titiler.application.egg-info/PKG-INFO` & `titiler.application-0.9.0/titiler.application.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.application
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC MosaicJSON FastAPI
 Classifier: Intended Audience :: Information Technology
```

### Comparing `titiler.application-0.8.1/titiler.application.egg-info/SOURCES.txt` & `titiler.application-0.9.0/titiler.application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

