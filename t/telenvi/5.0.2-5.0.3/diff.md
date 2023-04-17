# Comparing `tmp/telenvi-5.0.2.tar.gz` & `tmp/telenvi-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telenvi-5.0.2.tar", last modified: Wed Apr  5 15:39:13 2023, max compression
+gzip compressed data, was "telenvi-5.0.3.tar", last modified: Mon Apr 17 10:40:07 2023, max compression
```

## Comparing `telenvi-5.0.2.tar` & `telenvi-5.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-05 15:39:13.910000 telenvi-5.0.2/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-05 15:39:08.000000 telenvi-5.0.2/LICENSE
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-05 15:39:13.910000 telenvi-5.0.2/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-05 15:39:08.000000 telenvi-5.0.2/README.md
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-05 15:39:08.000000 telenvi-5.0.2/pyproject.toml
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-05 15:39:13.910000 telenvi-5.0.2/setup.cfg
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-05 15:39:13.910000 telenvi-5.0.2/src/
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-05 15:39:13.910000 telenvi-5.0.2/src/telenvi/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22405 2023-04-05 15:39:08.000000 telenvi-5.0.2/src/telenvi/GeoIm.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-05 15:39:08.000000 telenvi-5.0.2/src/telenvi/__init__.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-05 15:39:08.000000 telenvi-5.0.2/src/telenvi/associations.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    24416 2023-04-05 15:39:08.000000 telenvi-5.0.2/src/telenvi/raster_tools.py
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-05 15:39:08.000000 telenvi-5.0.2/src/telenvi/vector_tools.py
-drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-05 15:39:13.910000 telenvi-5.0.2/src/telenvi.egg-info/
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-05 15:39:13.000000 telenvi-5.0.2/src/telenvi.egg-info/PKG-INFO
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-05 15:39:13.000000 telenvi-5.0.2/src/telenvi.egg-info/SOURCES.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-05 15:39:13.000000 telenvi-5.0.2/src/telenvi.egg-info/dependency_links.txt
--rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-05 15:39:13.000000 telenvi-5.0.2/src/telenvi.egg-info/top_level.txt
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    35823 2023-04-17 10:40:01.000000 telenvi-5.0.3/LICENSE
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-17 10:40:07.640000 telenvi-5.0.3/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      620 2023-04-17 10:40:01.000000 telenvi-5.0.3/README.md
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)       84 2023-04-17 10:40:01.000000 telenvi-5.0.3/pyproject.toml
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      673 2023-04-17 10:40:07.640000 telenvi-5.0.3/setup.cfg
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/src/
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/src/telenvi/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    22386 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/GeoIm.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      133 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/__init__.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      478 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/associations.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)    24416 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/raster_tools.py
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     2859 2023-04-17 10:40:01.000000 telenvi-5.0.3/src/telenvi/vector_tools.py
+drwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        0 2023-04-17 10:40:07.640000 telenvi-5.0.3/src/telenvi.egg-info/
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)     1145 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/PKG-INFO
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)      311 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/SOURCES.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        1 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/dependency_links.txt
+-rwxr-xr-x   0 duvanelt  (1000) duvanelt  (1000)        8 2023-04-17 10:40:07.000000 telenvi-5.0.3/src/telenvi.egg-info/top_level.txt
```

### Comparing `telenvi-5.0.2/LICENSE` & `telenvi-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.2/PKG-INFO` & `telenvi-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.2
+Version: 5.0.3
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `telenvi-5.0.2/README.md` & `telenvi-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.2/setup.cfg` & `telenvi-5.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telenvi
-version = 5.0.2
+version = 5.0.3
 author = Thibaut Duvanel, Julien Pellen
 author_email = thibaut.duvanel@univ-savoie.fr
 description = Some remote sensing tricks from telenvi master students
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pyzak117/telenvi
 project_urls =
```

### Comparing `telenvi-5.0.2/src/telenvi/GeoIm.py` & `telenvi-5.0.3/src/telenvi/GeoIm.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         return target
 
     def cropFromVector(self, vector, polygon = 0, verbose = False, inplace=False):
         """
         vector : shapely.geometry.polygon.Polygon or str - path to a shapefile
         polygon : id of the feature, if vector is a shapefile
         """
-        print(type(vector))
+        
         # We get the polygon geo extent
         if type(vector) == str:
             layer = gpd.read_file(vector)
             bounds = layer["geometry"][polygon].bounds
 
         if type(vector) == gpd.GeoDataFrame:
             bounds = vector.iloc[0]["geometry"].bounds
```

### Comparing `telenvi-5.0.2/src/telenvi/raster_tools.py` & `telenvi-5.0.3/src/telenvi/raster_tools.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.2/src/telenvi/vector_tools.py` & `telenvi-5.0.3/src/telenvi/vector_tools.py`

 * *Files identical despite different names*

### Comparing `telenvi-5.0.2/src/telenvi.egg-info/PKG-INFO` & `telenvi-5.0.3/src/telenvi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telenvi
-Version: 5.0.2
+Version: 5.0.3
 Summary: Some remote sensing tricks from telenvi master students
 Home-page: https://github.com/pyzak117/telenvi
 Author: Thibaut Duvanel, Julien Pellen
 Author-email: thibaut.duvanel@univ-savoie.fr
 Project-URL: Bug Tracker, https://github.com/pyzak117/telenvi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

