# Comparing `tmp/titiler.mosaic-0.8.1.tar.gz` & `tmp/titiler.mosaic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titiler.mosaic-0.8.1.tar", last modified: Thu Dec  1 15:56:03 2022, max compression
+gzip compressed data, was "titiler.mosaic-0.9.0.tar", last modified: Mon Dec  5 17:00:49 2022, max compression
```

## Comparing `titiler.mosaic-0.8.1.tar` & `titiler.mosaic-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       56 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/titiler/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/titiler/mosaic/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/titiler/mosaic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      509 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/titiler/mosaic/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    30070 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/titiler/mosaic/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/titiler/mosaic/models/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/titiler/mosaic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      288 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/titiler/mosaic/models/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/titiler/mosaic/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/titiler/mosaic/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      533 2022-12-01 15:55:48.000000 titiler.mosaic-0.8.1/titiler/mosaic/resources/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 15:56:03.234470 titiler.mosaic-0.8.1/titiler.mosaic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1913 2022-12-01 15:56:03.000000 titiler.mosaic-0.8.1/titiler.mosaic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      499 2022-12-01 15:56:03.000000 titiler.mosaic-0.8.1/titiler.mosaic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:03.000000 titiler.mosaic-0.8.1/titiler.mosaic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 15:56:03.000000 titiler.mosaic-0.8.1/titiler.mosaic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-12-01 15:56:03.000000 titiler.mosaic-0.8.1/titiler.mosaic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-12-01 15:56:03.000000 titiler.mosaic-0.8.1/titiler.mosaic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:49.146947 titiler.mosaic-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2022-12-05 17:00:49.146947 titiler.mosaic-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-05 17:00:49.150947 titiler.mosaic-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:49.146947 titiler.mosaic-0.9.0/titiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:49.146947 titiler.mosaic-0.9.0/titiler/mosaic/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/titiler/mosaic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/titiler/mosaic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30118 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/titiler/mosaic/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:49.146947 titiler.mosaic-0.9.0/titiler/mosaic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/titiler/mosaic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/titiler/mosaic/models/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:49.146947 titiler.mosaic-0.9.0/titiler/mosaic/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/titiler/mosaic/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-05 17:00:39.000000 titiler.mosaic-0.9.0/titiler/mosaic/resources/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 17:00:49.146947 titiler.mosaic-0.9.0/titiler.mosaic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2022-12-05 17:00:49.000000 titiler.mosaic-0.9.0/titiler.mosaic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2022-12-05 17:00:49.000000 titiler.mosaic-0.9.0/titiler.mosaic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:49.000000 titiler.mosaic-0.9.0/titiler.mosaic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 17:00:49.000000 titiler.mosaic-0.9.0/titiler.mosaic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-05 17:00:49.000000 titiler.mosaic-0.9.0/titiler.mosaic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-05 17:00:49.000000 titiler.mosaic-0.9.0/titiler.mosaic.egg-info/top_level.txt
```

### Comparing `titiler.mosaic-0.8.1/PKG-INFO` & `titiler.mosaic-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.mosaic
-Version: 0.8.1
+Version: 0.9.0
 Summary: MosaicJSON plugin for TiTiler.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: MosaicJSON
 Classifier: Intended Audience :: Information Technology
```

### Comparing `titiler.mosaic-0.8.1/README.md` & `titiler.mosaic-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `titiler.mosaic-0.8.1/setup.py` & `titiler.mosaic-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup titiler.mosaic."""
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
-inst_reqs = ["titiler.core>=0.8,<0.9", "cogeo-mosaic>=5.0,<5.1"]
+inst_reqs = ["titiler.core>=0.9,<0.10", "cogeo-mosaic>=5.0,<5.1"]
 extra_reqs = {
     "test": ["pytest", "pytest-cov", "pytest-asyncio", "httpx"],
 }
 
 
 setup(
     name="titiler.mosaic",
```

### Comparing `titiler.mosaic-0.8.1/titiler/mosaic/factory.py` & `titiler.mosaic-0.9.0/titiler/mosaic/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from fastapi import Depends, Path, Query
 
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, Response
 
 # BaseBackend does not support other TMS than WebMercator
-default_tms = TileMatrixSets({"WebMercatorQuad": tms.get("WebMercatorQuad")})
+mosaic_tms = TileMatrixSets({"WebMercatorQuad": tms.get("WebMercatorQuad")})
 
 
 def PixelSelectionParams(
     pixel_selection: PixelSelectionMethod = Query(
         PixelSelectionMethod.first,
         description="Pixel selection method.",
     )
@@ -63,15 +63,16 @@
         Type[MultiBandReader],
     ] = Reader
 
     backend_dependency: Type[DefaultDependency] = DefaultDependency
 
     pixel_selection_dependency: Callable[..., MosaicMethodBase] = PixelSelectionParams
 
-    supported_tms: TileMatrixSets = default_tms
+    supported_tms: TileMatrixSets = mosaic_tms
+    default_tms: str = "WebMercatorQuad"
 
     # Add/Remove some endpoints
     add_viewer: bool = True
 
     def register_routes(self):
         """
         This Method register routes to the router.
@@ -238,16 +239,16 @@
             **img_endpoint_params,
         )
         def tile(
             z: int = Path(..., ge=0, le=30, description="Mercator tiles's zoom level"),
             x: int = Path(..., description="Mercator tiles's column"),
             y: int = Path(..., description="Mercator tiles's row"),
             TileMatrixSetId: Literal[tuple(self.supported_tms.list())] = Query(
-                "WebMercatorQuad",
-                description="TileMatrixSet Name (default: 'WebMercatorQuad')",
+                self.default_tms,
+                description=f"TileMatrixSet Name (default: '{self.default_tms}')",
             ),  # noqa
             scale: int = Query(
                 1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
             ),
             format: ImageType = Query(
                 None, description="Output image type. Default is auto."
             ),
@@ -335,16 +336,16 @@
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
             ),  # noqa
             src_path=Depends(self.path_dependency),
             tile_format: Optional[ImageType] = Query(
                 None, description="Output image type. Default is auto."
             ),
             tile_scale: int = Query(
                 1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
@@ -491,16 +492,16 @@
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
             ),  # noqa
             src_path=Depends(self.path_dependency),
             tile_format: ImageType = Query(
                 ImageType.png, description="Output image type. Default is png."
             ),
             tile_scale: int = Query(
                 1, gt=0, lt=4, description="Tile size scale. 1=256x256, 2=512x512..."
```

### Comparing `titiler.mosaic-0.8.1/titiler/mosaic/resources/enums.py` & `titiler.mosaic-0.9.0/titiler/mosaic/resources/enums.py`

 * *Files identical despite different names*

### Comparing `titiler.mosaic-0.8.1/titiler.mosaic.egg-info/PKG-INFO` & `titiler.mosaic-0.9.0/titiler.mosaic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titiler.mosaic
-Version: 0.8.1
+Version: 0.9.0
 Summary: MosaicJSON plugin for TiTiler.
 Home-page: https://github.com/developmentseed/titiler
 Author: Vincent Sarago
 Author-email: vincent@developmentseed.org
 License: MIT
 Keywords: MosaicJSON
 Classifier: Intended Audience :: Information Technology
```

