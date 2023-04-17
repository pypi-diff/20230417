# Comparing `tmp/geomapdemo-0.1.3.tar.gz` & `tmp/geomapdemo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.1.3.tar", last modified: Mon Apr 17 02:04:53 2023, max compression
+gzip compressed data, was "geomapdemo-0.1.4.tar", last modified: Mon Apr 17 03:13:06 2023, max compression
```

## Comparing `geomapdemo-0.1.3.tar` & `geomapdemo-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 03:13:06.000000 geomapdemo-0.1.4/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-17 03:13:06.588604 geomapdemo-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-17 03:12:56.000000 geomapdemo-0.1.4/setup.py
```

### Comparing `geomapdemo-0.1.3/LICENSE` & `geomapdemo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.1.3/PKG-INFO` & `geomapdemo-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.1.3/README.md` & `geomapdemo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.1.3/geomapdemo/geomapdemo.py` & `geomapdemo-0.1.4/geomapdemo/geomapdemo.py`

 * *Files 14% similar despite different names*

```diff
@@ -225,14 +225,24 @@
             name (str, optional): The name of the shapefile. Defaults to 'Shapefile'.
             **kwargs: Keyword arguments to be passed to the shapefile.
         """        
         import geopandas as gpd
         gdf = gpd.read_file(path)
         geojson = gdf.__geo_interface__
         self.add_geojson(geojson, name=name, **kwargs)
+    
+    def add_markers(self, center, draggable = False, **kwargs):
+        """Adds markers to the map
+        Args:
+            center (tuple): The center of the markers.
+            draggable (bool, optional): Whether the markers are draggable. Defaults to False.
+            **kwargs: Keyword arguments to be passed to the markers.
+        """        
+        marker = ipyleaflet.Marker(location=center, draggable= draggable, **kwargs)
+        self.add_layer(marker)
 
 
 
 
 
 def generate_random_string(length=10, upper=False, punctuations=False, digits=False):
     """Generates a random string of fixed length
```

### Comparing `geomapdemo-0.1.3/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.1.4/geomapdemo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.1.3/setup.py` & `geomapdemo-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='geomapdemo',
     name='geomapdemo',
     packages=find_packages(include=['geomapdemo', 'geomapdemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zyang91/geomapdemo',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

