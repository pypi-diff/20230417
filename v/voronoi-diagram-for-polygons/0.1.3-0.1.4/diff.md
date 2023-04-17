# Comparing `tmp/voronoi-diagram-for-polygons-0.1.3.tar.gz` & `tmp/voronoi-diagram-for-polygons-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voronoi-diagram-for-polygons-0.1.3.tar", last modified: Thu Nov 17 03:37:40 2022, max compression
+gzip compressed data, was "voronoi-diagram-for-polygons-0.1.4.tar", last modified: Mon Apr 17 02:13:00 2023, max compression
```

## Comparing `voronoi-diagram-for-polygons-0.1.3.tar` & `voronoi-diagram-for-polygons-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2022-11-17 03:37:40.057662 voronoi-diagram-for-polygons-0.1.3/
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     1091 2020-07-31 21:47:37.000000 voronoi-diagram-for-polygons-0.1.3/LICENSE
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     7157 2022-11-17 03:37:40.057662 voronoi-diagram-for-polygons-0.1.3/PKG-INFO
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     6780 2022-11-17 03:34:11.000000 voronoi-diagram-for-polygons-0.1.3/README.md
-drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2022-11-17 03:37:39.988653 voronoi-diagram-for-polygons-0.1.3/longsgis/
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)      152 2022-11-17 02:22:59.000000 voronoi-diagram-for-polygons-0.1.3/longsgis/__init__.py
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     6049 2022-11-17 03:28:31.000000 voronoi-diagram-for-polygons-0.1.3/longsgis/longsgis.py
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)       38 2022-11-17 03:37:40.057662 voronoi-diagram-for-polygons-0.1.3/setup.cfg
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)      828 2022-11-17 02:23:36.000000 voronoi-diagram-for-polygons-0.1.3/setup.py
-drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2022-11-17 03:37:40.035532 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)     7157 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/PKG-INFO
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)      327 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/SOURCES.txt
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)        1 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/dependency_links.txt
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)       34 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/requires.txt
--rwxrwxrwx   0 bruce     (1000) bruce     (1000)        9 2022-11-17 03:37:39.000000 voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/top_level.txt
+drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2023-04-17 02:13:00.583721 voronoi-diagram-for-polygons-0.1.4/
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)     1091 2020-07-31 21:47:37.000000 voronoi-diagram-for-polygons-0.1.4/LICENSE
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)     7258 2023-04-17 02:13:00.583721 voronoi-diagram-for-polygons-0.1.4/PKG-INFO
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)     6885 2023-04-17 01:51:45.000000 voronoi-diagram-for-polygons-0.1.4/README.md
+drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2023-04-17 02:13:00.505586 voronoi-diagram-for-polygons-0.1.4/longsgis/
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)      152 2022-11-17 02:22:59.000000 voronoi-diagram-for-polygons-0.1.4/longsgis/__init__.py
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)     6174 2023-04-17 01:47:57.000000 voronoi-diagram-for-polygons-0.1.4/longsgis/longsgis.py
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)       38 2023-04-17 02:13:00.583721 voronoi-diagram-for-polygons-0.1.4/setup.cfg
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)      828 2023-04-17 01:48:18.000000 voronoi-diagram-for-polygons-0.1.4/setup.py
+drwxrwxrwx   0 bruce     (1000) bruce     (1000)        0 2023-04-17 02:13:00.568096 voronoi-diagram-for-polygons-0.1.4/voronoi_diagram_for_polygons.egg-info/
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)     7258 2023-04-17 02:13:00.000000 voronoi-diagram-for-polygons-0.1.4/voronoi_diagram_for_polygons.egg-info/PKG-INFO
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)      327 2023-04-17 02:13:00.000000 voronoi-diagram-for-polygons-0.1.4/voronoi_diagram_for_polygons.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)        1 2023-04-17 02:13:00.000000 voronoi-diagram-for-polygons-0.1.4/voronoi_diagram_for_polygons.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)       34 2023-04-17 02:13:00.000000 voronoi-diagram-for-polygons-0.1.4/voronoi_diagram_for_polygons.egg-info/requires.txt
+-rwxrwxrwx   0 bruce     (1000) bruce     (1000)        9 2023-04-17 02:13:00.000000 voronoi-diagram-for-polygons-0.1.4/voronoi_diagram_for_polygons.egg-info/top_level.txt
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/LICENSE` & `voronoi-diagram-for-polygons-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voronoi-diagram-for-polygons-0.1.3/PKG-INFO` & `voronoi-diagram-for-polygons-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voronoi-diagram-for-polygons
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to create Voronoi diagram for polygons.
 Home-page: https://github.com/longavailable/voronoi-diagram-for-polygons
 Author: Xiaolong "Bruce" Liu, Meixiu Yu
 Author-email: liuxiaolong125@gmail.com, meixiuyu@hhu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -150,14 +150,18 @@
 - Fix a [FutureWarning](https://pandas.pydata.org/docs/whatsnew/v1.4.0.html#whatsnew-140-deprecations-frame-series-append).
 
 ### v0.1.3
 
 - Make it more robust for the less-vertice-geometry inputs. [#4](https://github.com/longavailable/voronoi-diagram-for-polygons/issues/4#issue-1378217062).
 - Fix a few ***FutureWarnings***.
 
+### v0.1.4
+
+- Change as [Shapely] goes. `MultiPolygon` is not iterable any more from [Shapely] 2.0.
+
 [Voronoi diagram for polygons]: https://github.com/longavailable/voronoi-diagram-for-polygons
 [Voronoi diagram]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Thiessen polygons]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Shapely]: https://shapely.readthedocs.io/en/latest/
 [GeoPandas]: https://geopandas.org/index.html
 [Create Thiessen Polygons (Analysis)]: https://pro.arcgis.com/en/pro-app/tool-reference/analysis/create-thiessen-polygons.htm
 [ArcGIS Pro]: https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/README.md` & `voronoi-diagram-for-polygons-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 - Fix a [FutureWarning](https://pandas.pydata.org/docs/whatsnew/v1.4.0.html#whatsnew-140-deprecations-frame-series-append).
 
 ### v0.1.3
 
 - Make it more robust for the less-vertice-geometry inputs. [#4](https://github.com/longavailable/voronoi-diagram-for-polygons/issues/4#issue-1378217062).
 - Fix a few ***FutureWarnings***.
 
+### v0.1.4
+
+- Change as [Shapely] goes. `MultiPolygon` is not iterable any more from [Shapely] 2.0.
+
 [Voronoi diagram for polygons]: https://github.com/longavailable/voronoi-diagram-for-polygons
 [Voronoi diagram]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Thiessen polygons]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Shapely]: https://shapely.readthedocs.io/en/latest/
 [GeoPandas]: https://geopandas.org/index.html
 [Create Thiessen Polygons (Analysis)]: https://pro.arcgis.com/en/pro-app/tool-reference/analysis/create-thiessen-polygons.htm
 [ArcGIS Pro]: https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/longsgis/longsgis.py` & `voronoi-diagram-for-polygons-0.1.4/longsgis/longsgis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 """
-* Updated on 2022/11/17
+* Updated on 2023/04/17
 * python3
 **
 * Geoprocessing in Python
 """
 import pandas as pd
 import geopandas as gpd
 import numpy as np
+import shapely
 from shapely.ops import voronoi_diagram as svd
 from shapely.geometry import Polygon, MultiPolygon
 import itertools, math
 
 def minimum_distance(gdf):
 	'''Calculate the minimum distance of all vertices of input geometries.
 	
@@ -135,15 +136,18 @@
 	Parameters:
 		plg: plg who has holes / empties
 			Type: shapely.geometry.MultiPolygon or shapely.geometry.Polygon
 	Returns:
 		a shapely.geometry.MultiPolygon or shapely.geometry.Polygon object
 	'''
 	if isinstance(plg, MultiPolygon):
-		return MultiPolygon(Polygon(p.exterior) for p in plg)
+		if shapely.__version__ < '2.0':
+			return MultiPolygon(Polygon(p.exterior) for p in plg)
+		else:
+			return MultiPolygon(Polygon(p.exterior) for p in plg.geoms)
 	elif isinstance(plg, Polygon):
 		return Polygon(plg.exterior)
 
 def dropHoles(gdf):
 	'''Remove / drop / fill the holes / empties for iterms in GeoDataFrame.
 	
 	Parameters:
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/setup.py` & `voronoi-diagram-for-polygons-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
 	long_description = fh.read()
 
 setup(
```

### Comparing `voronoi-diagram-for-polygons-0.1.3/voronoi_diagram_for_polygons.egg-info/PKG-INFO` & `voronoi-diagram-for-polygons-0.1.4/voronoi_diagram_for_polygons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voronoi-diagram-for-polygons
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to create Voronoi diagram for polygons.
 Home-page: https://github.com/longavailable/voronoi-diagram-for-polygons
 Author: Xiaolong "Bruce" Liu, Meixiu Yu
 Author-email: liuxiaolong125@gmail.com, meixiuyu@hhu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -150,14 +150,18 @@
 - Fix a [FutureWarning](https://pandas.pydata.org/docs/whatsnew/v1.4.0.html#whatsnew-140-deprecations-frame-series-append).
 
 ### v0.1.3
 
 - Make it more robust for the less-vertice-geometry inputs. [#4](https://github.com/longavailable/voronoi-diagram-for-polygons/issues/4#issue-1378217062).
 - Fix a few ***FutureWarnings***.
 
+### v0.1.4
+
+- Change as [Shapely] goes. `MultiPolygon` is not iterable any more from [Shapely] 2.0.
+
 [Voronoi diagram for polygons]: https://github.com/longavailable/voronoi-diagram-for-polygons
 [Voronoi diagram]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Thiessen polygons]: https://en.wikipedia.org/wiki/Voronoi_diagram
 [Shapely]: https://shapely.readthedocs.io/en/latest/
 [GeoPandas]: https://geopandas.org/index.html
 [Create Thiessen Polygons (Analysis)]: https://pro.arcgis.com/en/pro-app/tool-reference/analysis/create-thiessen-polygons.htm
 [ArcGIS Pro]: https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview
```

