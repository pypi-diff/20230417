# Comparing `tmp/titiler.core-0.8.1.tar.gz` & `tmp/titiler.core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.core-0.8.1.tar", last modified: Thu Dec  1 15:56:00 2022, max compression
+gzip compressed data, was "titiler.core-0.9.0.tar", last modified: Mon Dec  5 17:00:47 2022, max compression
```

## Comparing `titiler.core-0.8.1.tar` & `titiler.core-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.882477 titiler.core-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2022-12-01 15:55:48.000000 titiler.core-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2022-12-01 15:56:00.882477 titiler.core-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2022-12-01 15:55:48.000000 titiler.core-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-12-01 15:55:48.000000 titiler.core-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       91 2022-12-01 15:56:00.882477 titiler.core-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2022-12-01 15:55:48.000000 titiler.core-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.874477 titiler.core-0.8.1/titiler/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.878477 titiler.core-0.8.1/titiler/core/
--rw-r--r--   0 runner    (1001) docker     (122)      231 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.878477 titiler.core-0.8.1/titiler/core/algorithm/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      837 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/algorithm/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5044 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/algorithm/dem.py
--rw-r--r--   0 runner    (1001) docker     (122)      994 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/algorithm/index.py
--rw-r--r--   0 runner    (1001) docker     (122)    13538 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1879 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    65245 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     3726 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.878477 titiler.core-0.8.1/titiler/core/models/
--rw-r--r--   0 runner    (1001) docker     (122)      838 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/models/OGC.py
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/models/mapbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/models/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.882477 titiler.core-0.8.1/titiler/core/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/resources/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/resources/responses.py
--rw-r--r--   0 runner    (1001) docker     (122)     3564 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.882477 titiler.core-0.8.1/titiler/core/templates/
--rw-r--r--   0 runner    (1001) docker     (122)     3358 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     2956 2022-12-01 15:55:48.000000 titiler.core-0.8.1/titiler/core/templates/wmts.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:00.878477 titiler.core-0.8.1/titiler.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2022-12-01 15:56:00.000000 titiler.core-0.8.1/titiler.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      840 2022-12-01 15:56:00.000000 titiler.core-0.8.1/titiler.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:00.000000 titiler.core-0.8.1/titiler.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:00.000000 titiler.core-0.8.1/titiler.core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      256 2022-12-01 15:56:00.000000 titiler.core-0.8.1/titiler.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-12-01 15:56:00.000000 titiler.core-0.8.1/titiler.core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-05 17:00:39.000000 titiler.core-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2022-12-05 17:00:47.102960 titiler.core-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2022-12-05 17:00:39.000000 titiler.core-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-05 17:00:39.000000 titiler.core-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-05 17:00:47.106960 titiler.core-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2022-12-05 17:00:39.000000 titiler.core-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/titiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/titiler/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/titiler/core/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/algorithm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/algorithm/dem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/algorithm/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13538 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65307 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/titiler/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/models/OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/models/mapbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/models/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/titiler/core/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/resources/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/resources/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/titiler/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2022-12-05 17:00:39.000000 titiler.core-0.9.0/titiler/core/templates/wmts.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:47.102960 titiler.core-0.9.0/titiler.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2022-12-05 17:00:47.000000 titiler.core-0.9.0/titiler.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2022-12-05 17:00:47.000000 titiler.core-0.9.0/titiler.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:47.000000 titiler.core-0.9.0/titiler.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:47.000000 titiler.core-0.9.0/titiler.core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2022-12-05 17:00:47.000000 titiler.core-0.9.0/titiler.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-05 17:00:47.000000 titiler.core-0.9.0/titiler.core.egg-info/top_level.txt
```

### Comparing `titiler.core-0.8.1/PKG-INFO` & `titiler.core-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.core
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC FastAPI
 Classifier: Intended Audience :: Information Technology
```

### Comparing `titiler.core-0.8.1/README.md` & `titiler.core-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/setup.py` & `titiler.core-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/algorithm/__init__.py` & `titiler.core-0.9.0/titiler/core/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/algorithm/base.py` & `titiler.core-0.9.0/titiler/core/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/algorithm/dem.py` & `titiler.core-0.9.0/titiler/core/algorithm/dem.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/algorithm/index.py` & `titiler.core-0.9.0/titiler/core/algorithm/index.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/dependencies.py` & `titiler.core-0.9.0/titiler/core/dependencies.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/errors.py` & `titiler.core-0.9.0/titiler/core/errors.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/factory.py` & `titiler.core-0.9.0/titiler/core/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Type, Union
 from urllib.parse import urlencode
 
 import rasterio
 from geojson_pydantic.features import Feature, FeatureCollection
 from geojson_pydantic.geometries import Polygon
 from morecantile import TileMatrixSet
-from morecantile import tms as default_tms
+from morecantile import tms as morecantile_tms
 from morecantile.defaults import TileMatrixSets
 from rio_tiler.io import BaseReader, MultiBandReader, MultiBaseReader, Reader
 from rio_tiler.models import BandStatistics, Bounds, Info
 from rio_tiler.types import ColorMapType
 from rio_tiler.utils import get_array_statistics
 
 from titiler.core.algorithm import AlgorithmMetadata, Algorithms, BaseAlgorithm
@@ -139,15 +139,16 @@
     # Reader dependency
     reader_dependency: Type[DefaultDependency] = DefaultDependency
 
     # GDAL ENV dependency
     environment_dependency: Callable[..., Dict] = lambda: dict()
 
     # TileMatrixSet dependency
-    supported_tms: TileMatrixSets = default_tms
+    supported_tms: TileMatrixSets = morecantile_tms
+    default_tms: str = "WebMercatorQuad"
 
     # Router Prefix is needed to find the path for /tile if the TilerFactory.router is mounted
     # with other router (multiple `.../tile` routes).
     # e.g if you mount the route with `/cog` prefix, set router_prefix to cog and
     router_prefix: str = ""
 
     # add additional headers in response
@@ -461,16 +462,16 @@
             **img_endpoint_params,
         )
         def tile(
             z: int = Path(..., ge=0, le=30, description="TMS tiles's zoom level"),
             x: int = Path(..., description="TMS tiles's column"),
             y: int = Path(..., description="TMS tiles's row"),
             TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(
-                "WebMercatorQuad",
-                description="TileMatrixSet Name (default: 'WebMercatorQuad')",
+                self.default_tms,
+                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
             ),
             scale: int = Query(
                 1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
             ),
             format: ImageType = Query(
                 None, description="Output image type. Default is auto."
             ),
@@ -545,16 +546,16 @@
             response_model=TileJSON,
             responses={200: {"description": "Return a tilejson"}},
             response_model_exclude_none=True,
         )
         def tilejson(
             request: Request,
             TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(
-                "WebMercatorQuad",
-                description="TileMatrixSet Name (default: 'WebMercatorQuad')",
+                self.default_tms,
+                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
             ),
             src_path=Depends(self.path_dependency),
             tile_format: Optional[ImageType] = Query(
                 None, description="Output image type. Default is auto."
             ),
             tile_scale: int = Query(
                 1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
@@ -690,16 +691,16 @@
         @self.router.get("/WMTSCapabilities.xml", response_class=XMLResponse)
         @self.router.get(
             "/{TileMatrixSetId}/WMTSCapabilities.xml", response_class=XMLResponse
         )
         def wmts(
             request: Request,
             TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(
-                "WebMercatorQuad",
-                description="TileMatrixSet Name (default: 'WebMercatorQuad')",
+                self.default_tms,
+                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
             ),
             src_path=Depends(self.path_dependency),
             tile_format: ImageType = Query(
                 ImageType.png, description="Output image type. Default is png."
             ),
             tile_scale: int = Query(
                 1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
@@ -1453,15 +1454,15 @@
             return fc.features[0] if isinstance(geojson, Feature) else fc
 
 
 @dataclass
 class TMSFactory:
     """TileMatrixSet endpoints Factory."""
 
-    supported_tms: TileMatrixSets = default_tms
+    supported_tms: TileMatrixSets = morecantile_tms
 
     # FastAPI router
     router: APIRouter = field(default_factory=APIRouter)
 
     # Router Prefix is needed to find the path for /tile if the TilerFactory.router is mounted
     # with other router (multiple `.../tile` routes).
     # e.g if you mount the route with `/cog` prefix, set router_prefix to cog and
```

### Comparing `titiler.core-0.8.1/titiler/core/middleware.py` & `titiler.core-0.9.0/titiler/core/middleware.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/models/OGC.py` & `titiler.core-0.9.0/titiler/core/models/OGC.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/models/mapbox.py` & `titiler.core-0.9.0/titiler/core/models/mapbox.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/models/responses.py` & `titiler.core-0.9.0/titiler/core/models/responses.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/resources/enums.py` & `titiler.core-0.9.0/titiler/core/resources/enums.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/resources/responses.py` & `titiler.core-0.9.0/titiler/core/resources/responses.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/routing.py` & `titiler.core-0.9.0/titiler/core/routing.py`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/templates/index.html` & `titiler.core-0.9.0/titiler/core/templates/index.html`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler/core/templates/wmts.xml` & `titiler.core-0.9.0/titiler/core/templates/wmts.xml`

 * *Files identical despite different names*

### Comparing `titiler.core-0.8.1/titiler.core.egg-info/PKG-INFO` & `titiler.core-0.9.0/titiler.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.core
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern dynamic tile server built on top of FastAPI and Rasterio/GDAL.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: COG STAC FastAPI
 Classifier: Intended Audience :: Information Technology
```

### Comparing `titiler.core-0.8.1/titiler.core.egg-info/SOURCES.txt` & `titiler.core-0.9.0/titiler.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

