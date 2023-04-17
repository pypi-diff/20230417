# Comparing `tmp/geomapdemo-0.1.2.tar.gz` & `tmp/geomapdemo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapdemo-0.1.2.tar", last modified: Sun Apr 16 22:55:22 2023, max compression
+gzip compressed data, was "geomapdemo-0.1.3.tar", last modified: Mon Apr 17 02:04:53 2023, max compression
```

## Comparing `geomapdemo-0.1.2.tar` & `geomapdemo-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/geomapdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/geomapdemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/geomapdemo/geomapdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/geomapdemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 22:55:22.000000 geomapdemo-0.1.2/geomapdemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 22:55:22.535679 geomapdemo-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-16 22:55:12.000000 geomapdemo-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/geomapdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/geomapdemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/geomapdemo/geomapdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/geomapdemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 02:04:53.000000 geomapdemo-0.1.3/geomapdemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-17 02:04:53.943606 geomapdemo-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-17 02:04:40.000000 geomapdemo-0.1.3/setup.py
```

### Comparing `geomapdemo-0.1.2/LICENSE` & `geomapdemo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.1.2/PKG-INFO` & `geomapdemo-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.1.2/README.md` & `geomapdemo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `geomapdemo-0.1.2/geomapdemo/geomapdemo.py` & `geomapdemo-0.1.3/geomapdemo/geomapdemo.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,29 @@
         if "search_control" not in kwargs:
             """Adds a search control by default"""
             kwargs["search_control"] = True
         
         if kwargs["search_control"]:
             """Adds a search control to the map"""
             self.add_search_control()
+        
+        if "scale_control" not in kwargs:
+            """Adds a scale control by default"""
+            kwargs["scale_control"] = True
+        
+        if kwargs["scale_control"]:
+            """Adds a scale control to the map"""
+            self.add_scale_control()
+        
+        if 'height' in kwargs:
+            """Sets the height of the map"""
+            self.layout.height = kwargs['height']
+        else:
+            """Sets the default height of the map"""
+            kwargs['height'] = '600px'
 
 
     def add_basemap(self, basemap, **kwargs):
         """Adds a basemap to the map
         Args:
             basemap(str): The name of basemap.
             **kwargs: Keyword arguments to be passed to the basemap.
@@ -160,14 +175,37 @@
                     "fillColor": "#fca45d",
                     "color": "#fca45d",
                     "fillOpacity": 1.0
                 }
             }
         self.add_control(draw_control)
     
+    def add_measure_control(self, position = 'bottomleft',  primary_length_unit = 'kilometers', **kwargs):
+        """Adds a measure control to the map
+        Args:
+            position (str, optional): The position of the measure control. Defaults to 'bottomleft'.
+            primary_length_unit (str, optional): The primary length unit of the measure control. Defaults to 'kilometers'.
+            **kwargs: Keyword arguments to be passed to the measure control.
+        """  
+        measure_control = ipyleaflet.MeasureControl(
+            position = position, 
+            primary_length_unit = primary_length_unit,
+            **kwargs
+            )
+        self.add_control(measure_control)
+    
+    def add_scale_control(self, position = 'bottomleft', **kwargs):
+        """Adds a scale control to the map
+        Args:
+            position (str, optional): The position of the scale control. Defaults to 'bottomleft'.
+            **kwargs: Keyword arguments to be passed to the scale control.
+        """  
+        scale_control = ipyleaflet.ScaleControl(position = position, **kwargs)
+        self.add_control(scale_control)
+
     def add_geojson(self, data, name ='GeoJson', **kwargs):
         """Adds a geojson to the map
         Args:
             data (dict): The geojson data.
             name (str, optional): The name of the geojson. Defaults to 'GeoJson'.
             **kwargs: Keyword arguments to be passed to the geojson.
         """
```

### Comparing `geomapdemo-0.1.2/geomapdemo.egg-info/PKG-INFO` & `geomapdemo-0.1.3/geomapdemo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapdemo
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for interactive mapping, testing.
 Home-page: https://github.com/zyang91/geomapdemo
 Author: Zhanchao Yang
 Author-email: zyang91@binghamton.edu
 License: MIT license
 Keywords: geomapdemo
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geomapdemo-0.1.2/setup.py` & `geomapdemo-0.1.3/setup.py`

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
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

