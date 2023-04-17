# Comparing `tmp/hydromt_sfincs-0.2.1.tar.gz` & `tmp/hydromt_sfincs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromt_sfincs-0.2.1.tar", last modified: Wed Feb 23 13:16:34 2022, max compression
+gzip compressed data, was "hydromt_sfincs-1.0.0.tar", last modified: Mon Apr 17 16:01:50 2023, max compression
```

## Comparing `hydromt_sfincs-0.2.1.tar` & `hydromt_sfincs-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,27 @@
--rw-r--r--   0        0        0     1364 2022-02-23 10:18:36.776775 hydromt_sfincs-0.2.1/.gitignore
--rw-r--r--   0        0        0      614 2022-02-23 10:18:36.776775 hydromt_sfincs-0.2.1/.zenodo.json
--rw-r--r--   0        0        0    35148 2022-02-23 10:18:36.776775 hydromt_sfincs-0.2.1/LICENSE
--rw-r--r--   0        0        0     2796 2022-02-23 10:18:36.776775 hydromt_sfincs-0.2.1/README.rst
--rw-r--r--   0        0        0      204 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/__init__.py
--rw-r--r--   0        0        0      197 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/data/lulc/README
--rw-r--r--   0        0        0     2680 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/data/lulc/corine_mapping.csv
--rw-r--r--   0        0        0     2497 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/data/lulc/globcover_mapping.csv
--rw-r--r--   0        0        0     1845 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/data/lulc/globcover_mapping_sediment.csv
--rw-r--r--   0        0        0     1764 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/data/lulc/vito_mapping.csv
--rw-r--r--   0        0        0      658 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/data/sfincs/sfincs.inp
--rw-r--r--   0        0        0    10121 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/plots.py
--rw-r--r--   0        0        0   103493 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/sfincs.py
--rw-r--r--   0        0        0    28960 2022-02-23 13:08:13.926665 hydromt_sfincs-0.2.1/hydromt_sfincs/utils.py
--rw-r--r--   0        0        0      127 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/workflows/__init__.py
--rw-r--r--   0        0        0    19598 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/workflows/bathymetry.py
--rw-r--r--   0        0        0     2894 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/workflows/discharge.py
--rw-r--r--   0        0        0     3238 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/workflows/flwdir.py
--rw-r--r--   0        0        0     2973 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/hydromt_sfincs/workflows/landuse.py
--rw-r--r--   0        0        0     1638 2022-02-23 10:18:36.846776 hydromt_sfincs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 hydromt_sfincs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1380 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/.gitignore
+-rw-r--r--   0        0        0      819 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/.zenodo.json
+-rw-r--r--   0        0        0    35148 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5339 2023-04-17 16:01:40.052248 hydromt_sfincs-1.0.0/README.rst
+-rw-r--r--   0        0        0      535 2023-04-17 16:01:40.056248 hydromt_sfincs-1.0.0/environment.yml
+-rw-r--r--   0        0        0      215 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/README
+-rw-r--r--   0        0        0     1151 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/corine_mapping.csv
+-rw-r--r--   0        0        0      335 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/esa_worldcover_mapping.csv
+-rw-r--r--   0        0        0     1702 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/globcover_mapping.csv
+-rw-r--r--   0        0        0      874 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/vito_mapping.csv
+-rw-r--r--   0        0        0      658 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/data/sfincs/sfincs.inp
+-rw-r--r--   0        0        0    10523 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/plots.py
+-rw-r--r--   0        0        0    21886 2023-04-17 16:01:40.188256 hydromt_sfincs-1.0.0/hydromt_sfincs/regulargrid.py
+-rw-r--r--   0        0        0   120821 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/sfincs.py
+-rw-r--r--   0        0        0     6414 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/sfincs_input.py
+-rw-r--r--   0        0        0    29380 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/subgrid.py
+-rw-r--r--   0        0        0    25856 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/utils.py
+-rw-r--r--   0        0        0      171 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/__init__.py
+-rw-r--r--   0        0        0    15096 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/bathymetry.py
+-rw-r--r--   0        0        0     3444 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/discharge.py
+-rw-r--r--   0        0        0     5285 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/flwdir.py
+-rw-r--r--   0        0        0      630 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/landuse.py
+-rw-r--r--   0        0        0    10030 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/merge.py
+-rw-r--r--   0        0        0    12754 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/tiling.py
+-rw-r--r--   0        0        0     1911 2023-04-17 16:01:40.192256 hydromt_sfincs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7038 1970-01-01 00:00:00.000000 hydromt_sfincs-1.0.0/PKG-INFO
```

### Comparing `hydromt_sfincs-0.2.1/.gitignore` & `hydromt_sfincs-1.0.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -65,22 +65,23 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
-docs/generated/
+docs/_generated/
 docs/_examples/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook /  examples
 .ipynb_checkpoints
+examples/tmp*
 
 # pyenv
 .python-version
 
 # celery beat schedule file
 celerybeat-schedule
 
@@ -112,8 +113,8 @@
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
 # dask
-dask-worker-space/
+dask-worker-space/
```

### Comparing `hydromt_sfincs-0.2.1/.zenodo.json` & `hydromt_sfincs-1.0.0/.zenodo.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7166666666666667%*

 * *Differences: {"'creators'": "{insert: [(0, OrderedDict([('affiliation', 'Deltares'), ('name', 'de Goede, "*

 * *               "Roel')])), (4, OrderedDict([('affiliation', 'Deltares-USA'), ('name', 'van "*

 * *               "Ormondt, Maarten')]))]}",*

 * * "'description'": "'SFINCS plugin for HydroMT.'",*

 * * "'license'": "'GPLv3'",*

 * * "'title'": "'HydroMT-SFINCS'"}*

```diff
@@ -1,24 +1,32 @@
 {
     "access_right": "open",
     "creators": [
         {
             "affiliation": "Deltares",
+            "name": "de Goede, Roel"
+        },
+        {
+            "affiliation": "Deltares",
             "name": "Eilander, Dirk",
             "orcid": "0000-0002-0951-8418"
         },
         {
             "affiliation": "Deltares",
             "name": "Leijnse, Tim",
             "orcid": "0000-0003-1873-3387"
         },
         {
             "affiliation": "Deltares",
             "name": "Winsemius, Hessel C.",
             "orcid": "0000-0001-5471-172X"
+        },
+        {
+            "affiliation": "Deltares-USA",
+            "name": "van Ormondt, Maarten"
         }
     ],
-    "description": "SFINCS plugin for hydroMT.",
-    "license": "MIT",
-    "title": "hydroMT-sfincs",
+    "description": "SFINCS plugin for HydroMT.",
+    "license": "GPLv3",
+    "title": "HydroMT-SFINCS",
     "upload_type": "software"
 }
```

### Comparing `hydromt_sfincs-0.2.1/LICENSE` & `hydromt_sfincs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-0.2.1/hydromt_sfincs/data/lulc/globcover_mapping.csv` & `hydromt_sfincs-1.0.0/hydromt_sfincs/data/lulc/globcover_mapping.csv`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-globcover,description,landuse,Kext,N,PathFrac,RootingDepth,Sl,Swood,WaterFrac,USLE_C,Cov_River
-11,Post-flooding or irrigated croplands (or aquatic),11,0.6,0.2,0,390,0.127,0.01,0,0.2,0.97
-14,Rainfed croplands,14,0.6,0.2,0,390,0.127,0,0,0.35,1.97
-20,Mosaic cropland (50-70%) / vegetation (grassland/shrubland/forest) (20-50%),20,0.6,0.44,0,397,0.127,0.01,0,0.27,1.97
-30,Mosaic vegetation (grassland/shrubland/forest) (50-70%) / cropland (20-50%) ,30,0.6,0.56,0,400,0.127,0.01,0,0.25,1.97
-40,Closed to open (>15%) broadleaved evergreen or semi-deciduous forest (>5m),40,0.6,0.3,0,308,0.039,0.5,0,0.0065,5.40
-50,Closed (>40%) broadleaved deciduous forest (>5m),50,0.8,0.8,0,430,0.036,0.5,0,0.001,19.20
-60,Open (15-40%) broadleaved deciduous forest/woodland (>5m),60,0.8,0.4,0,430,0.036,0.5,0,0.01,5.40
-70,Closed (>40%) needleleaved evergreen forest (>5m),70,0.8,0.1,0,382,0.045,0.5,0,0.001,19.20
-90,Open (15-40%) needleleaved deciduous or evergreen forest (>5m),90,0.8,0.4,0,382,0.045,0.5,0,0.01,5.40
-100,Mosaic forest or shrubland (50-70%) / grassland (20-50%),100,0.8,0.3,0,406,0.039,0.5,0,0.02,5.40
-110,Mosaic forest or shrubland (50-70%) / grassland (20-50%),110,0.6,0.456,0,286,0.07,0.2,0,0.015,5.40
-120,Mosaic grassland (50-70%) / forest or shrubland (20-50%) ,120,0.6,0.5,0,179,0.127,0.05,0,0.03,1.97
-130,Closed to open (>15%) (broadleaved or needleleaved evergreen or deciduous) shrubland (<5m),130,0.6,0.5,0,432,0.07,0.1,0,0.035,1.97
-140,Closed to open (>15%) herbaceous vegetation (grassland savannas or lichens/mosses),140,0.6,0.24,0,457,0.09,0,0,0.05,1.97
-150,Closed to open (>15%) herbaceous vegetation (grassland savannas or lichens/mosses),150,0.6,0.02,0,137,0.04,0.04,0,0.35,1.97
-160,Closed to open (>15%) broadleaved forest regularly flooded (semi-permanently or temporarily) - Fresh or brackish water,160,0.6,0.3,0,308,0.04,0.1,0,0.001,5.40
-170,Closed (>40%) broadleaved forest or shrubland permanently flooded - Saline or brackish water,170,0.8,0.8,0,308,0.036,0.2,0,0.0005,19.20
-180,Closed to open (>15%) grassland or woody vegetation on regularly flooded or waterlogged soil -  Fresh brackish or saline water,180,0.6,0.15,0,107,0.127,0.01,0,0.04,1.97
-190,Artificial surfaces and associated areas (Urban areas >50%),190,0.6,0.011,0.75,179,0.04,0.01,0,0.0,1.0
-200,Bare areas,200,0.6,0.01,0,0,0.04,0,0,0.0,1.0
-210,Water bodies,210,0.7,0.08,0,0,0.04,0,1,0.0,1.0
-220,Permanent snow and ice,220,0.6,0.01,0,0,0.04,0,0,0.0,1.0
-230,No Data,230,-999,-999,-999,-999,-999,-999,-999,-999,-999
+globcover,description,landuse,N
+11,Post-flooding or irrigated croplands (or aquatic),11,0.2
+14,Rainfed croplands,14,0.2
+20,Mosaic cropland (50-70%) / vegetation (grassland/shrubland/forest) (20-50%),20,0.44
+30,Mosaic vegetation (grassland/shrubland/forest) (50-70%) / cropland (20-50%) ,30,0.56
+40,Closed to open (>15%) broadleaved evergreen or semi-deciduous forest (>5m),40,0.3
+50,Closed (>40%) broadleaved deciduous forest (>5m),50,0.8
+60,Open (15-40%) broadleaved deciduous forest/woodland (>5m),60,0.4
+70,Closed (>40%) needleleaved evergreen forest (>5m),70,0.1
+90,Open (15-40%) needleleaved deciduous or evergreen forest (>5m),90,0.4
+100,Mosaic forest or shrubland (50-70%) / grassland (20-50%),100,0.3
+110,Mosaic forest or shrubland (50-70%) / grassland (20-50%),110,0.456
+120,Mosaic grassland (50-70%) / forest or shrubland (20-50%) ,120,0.5
+130,Closed to open (>15%) (broadleaved or needleleaved evergreen or deciduous) shrubland (<5m),130,0.5
+140,Closed to open (>15%) herbaceous vegetation (grassland savannas or lichens/mosses),140,0.24
+150,Closed to open (>15%) herbaceous vegetation (grassland savannas or lichens/mosses),150,0.02
+160,Closed to open (>15%) broadleaved forest regularly flooded (semi-permanently or temporarily) - Fresh or brackish water,160,0.3
+170,Closed (>40%) broadleaved forest or shrubland permanently flooded - Saline or brackish water,170,0.8
+180,Closed to open (>15%) grassland or woody vegetation on regularly flooded or waterlogged soil -  Fresh brackish or saline water,180,0.15
+190,Artificial surfaces and associated areas (Urban areas >50%),190,0.011
+200,Bare areas,200,0.01
+210,Water bodies,210,0.08
+220,Permanent snow and ice,220,0.01
+230,No Data,230,-999
```

### Comparing `hydromt_sfincs-0.2.1/hydromt_sfincs/data/sfincs/sfincs.inp` & `hydromt_sfincs-1.0.0/hydromt_sfincs/data/sfincs/sfincs.inp`

 * *Files identical despite different names*

### Comparing `hydromt_sfincs-0.2.1/hydromt_sfincs/plots.py` & `hydromt_sfincs-1.0.0/hydromt_sfincs/plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-import geopandas as gpd
-import pandas as pd
+"""Plotting functions for SFINCS model data."""
+from typing import Dict, List, Tuple
+
 import numpy as np
+import pandas as pd
 import xarray as xr
-from typing import Dict, Tuple, List
+
+from .utils import get_bounds_vector
 
 __all__ = ["plot_forcing", "plot_basemap"]
 
 geom_style = {
     "rivers": dict(linestyle="-", linewidth=1.0, color="darkblue"),
     "rivers_out": dict(linestyle="-", linewidth=1.0, color="darkgreen"),
     "msk2": dict(linestyle="-", linewidth=1.5, color="r"),
     "msk3": dict(linestyle="-", linewidth=1.5, color="m"),
-    "thd": dict(linestyle="-", linewidth=1.0, color="k", annotate=True),
-    "weir": dict(linestyle="--", linewidth=1.0, color="k", annotate=True),
+    "thd": dict(linestyle="-", linewidth=1.0, color="k", annotate=False),
+    "weir": dict(linestyle="--", linewidth=1.0, color="k", annotate=False),
     "bnd": dict(marker="^", markersize=75, c="w", edgecolor="k", annotate=True),
     "src": dict(marker=">", markersize=75, c="w", edgecolor="k", annotate=True),
     "obs": dict(marker="d", markersize=75, c="w", edgecolor="r", annotate=True),
+    "region": dict(ls="--", linewidth=1, color="r"),
 }
 
 
 def plot_forcing(forcing: Dict, **kwargs):
     """Plot model timeseries forcing.
 
     For distributed forcing a spatial avarage is plotted.
@@ -30,160 +34,172 @@
         Model forcing
 
     Returns
     -------
     fig, axes
         Model fig and ax objects
     """
-    import matplotlib.pyplot as plt
     import matplotlib.dates as mdates
+    import matplotlib.pyplot as plt
 
     n = len(forcing.keys())
     kwargs0 = dict(sharex=True, figsize=(6, n * 3))
     kwargs0.update(**kwargs)
     fig, axes = plt.subplots(n, 1, **kwargs0)
     axes = [axes] if n == 1 else axes
     for i, name in enumerate(forcing):
-        da = forcing[name]
+        da = forcing[name].transpose("time", ...)
         longname = da.attrs.get("standard_name", "")
         unit = da.attrs.get("unit", "")
         prefix = ""
         if da.ndim == 3:
             da = da.mean(dim=[da.raster.x_dim, da.raster.y_dim])
             prefix = "mean "
         # convert to Single index dataframe (bar plots don't work with xarray)
-        df = da.squeeze().to_series()
+        df = da.to_pandas()
         if isinstance(df.index, pd.MultiIndex):
             df = df.unstack(0)
         # convert dates a-priori as automatic conversion doesn't always work
         df.index = mdates.date2num(df.index)
-        if longname == "precipitation":
+        if name.startswith("precip"):
             axes[i].bar(df.index, df.values, facecolor="darkblue")
         else:
             df.plot.line(ax=axes[i]).legend(
                 title="index",
                 bbox_to_anchor=(1.05, 1),
                 loc="upper left",
-                ncol=2,
+                ncol=df.columns.size // 5 + 1,
+                prop={"size": 8},
             )
         axes[i].set_ylabel(f"{prefix}{longname}\n[{unit}]")
         axes[i].set_title(f"SFINCS {longname} forcing ({name})")
 
     # use a concise date formatter for format date axis ticks
     locator = mdates.AutoDateLocator()
     formatter = mdates.ConciseDateFormatter(locator)
     axes[-1].xaxis.set_major_locator(locator)
     axes[-1].xaxis.set_major_formatter(formatter)
 
     return fig, axes
 
 
 def plot_basemap(
-    staticmaps: xr.Dataset,
-    staticgeoms: Dict,
+    ds: xr.Dataset,
+    geoms: Dict,
     variable: str = "dep",
-    shaded: bool = True,
+    shaded: bool = False,
     plot_bounds: bool = True,
     plot_region: bool = False,
     plot_geoms: bool = True,
-    bmap: str = "sat",
+    bmap: str = None,
     zoomlevel: int = 11,
     figsize: Tuple[int] = None,
-    geoms: List[str] = None,
+    geom_names: List[str] = None,
     geom_kwargs: Dict = {},
     legend_kwargs: Dict = {},
     bmap_kwargs: Dict = {},
     **kwargs,
 ):
     """Create basemap plot.
 
     Parameters
     ----------
-    staticmaps : xr.Dataset
+    ds : xr.Dataset
         Dataset with model maps
-    staticgeoms : Dict of geopandas.GeoDataFrame
+    geoms : Dict of geopandas.GeoDataFrame
         Model geometries
     variable : str, optional
-        Map name to plot, by default 'dep'
+        Map of variable in ds to plot, by default 'dep'
     shaded : bool, optional
-        Add shade to variable (only for variable = 'dep'), by default True
+        Add shade to variable (only for variable = 'dep'), by default False
     plot_bounds : bool, optional
         Add waterlevel (msk=2) and open (msk=3) boundary conditions to plot.
     plot_region : bool, optional
         If True, plot region outline.
     plot_geoms : bool, optional
         If True, plot available geoms.
     bmap : {'sat', 'osm'}
         background map, by default "sat"
     zoomlevel : int, optional
         zoomlevel, by default 11
     figsize : Tuple[int], optional
         figure size, by default None
-    geoms : List[str], optional
+    geom_names : List[str], optional
         list of model geometries to plot, by default all model geometries
     geom_kwargs : Dict of Dict, optional
         Model geometry styling per geometry, passed to geopandas.GeoDataFrame.plot method.
         For instance: {'src': {'markersize': 30}}.
     legend_kwargs : Dict, optional
         Legend kwargs, passed to ax.legend method.
+
     Returns
     -------
     fig, axes
         Model fig and ax objects
     """
+    import cartopy.crs as ccrs
+    import cartopy.io.img_tiles as cimgt
     import matplotlib.pyplot as plt
     from matplotlib import colors, patheffects
-    import cartopy.io.img_tiles as cimgt
-    import cartopy.crs as ccrs
 
     # read crs and utm zone > convert to cartopy
-    wkt = staticmaps.raster.crs.to_wkt()
+    wkt = ds.raster.crs.to_wkt()
     if "UTM zone " not in wkt:
         raise ValueError("Model CRS UTM zone not found.")
-    utm_zone = staticmaps.raster.crs.to_wkt().split("UTM zone ")[1][:3]
+    utm_zone = ds.raster.crs.to_wkt().split("UTM zone ")[1][:3]
     utm = ccrs.UTM(int(utm_zone[:2]), "S" in utm_zone)
-    extent = np.array(staticmaps.raster.box.buffer(2e3).total_bounds)[[0, 2, 1, 3]]
+    extent = np.array(ds.raster.box.buffer(1e2).total_bounds)[[0, 2, 1, 3]]
 
     # create fig with geo-axis and set background
     if figsize is None:
-        ratio = staticmaps.raster.ycoords.size / (staticmaps.raster.xcoords.size * 1.2)
-        figsize = (10, 10 * ratio)
+        ratio = ds.raster.ycoords.size / (ds.raster.xcoords.size * 1.4)
+        figsize = (8, 8 * ratio)
     fig = plt.figure(figsize=figsize)
     ax = plt.subplot(projection=utm)
     ax.set_extent(extent, crs=utm)
     if bmap == "sat":
         ax.add_image(cimgt.QuadtreeTiles(**bmap_kwargs), zoomlevel)
     elif bmap == "osm":
         ax.add_image(cimgt.OSM(**bmap_kwargs), zoomlevel)
-    elif hasattr(cimgt, bmap):
+    elif bmap is not None and hasattr(cimgt, bmap):
         ax.add_image(getattr(cimgt, bmap)(**bmap_kwargs), zoomlevel)
 
+    # by default colorbar on lower right & legend upper right
+    kwargs0 = {"cbar_kwargs": {"shrink": 0.5, "anchor": (0, 0)}}
+    kwargs0.update(kwargs)
     # make nice cmap
     if "cmap" not in kwargs or "norm" not in kwargs:
-        if variable == "dep":
-            vmin, vmax = (
-                staticmaps["dep"].raster.mask_nodata().quantile([0.0, 0.98]).values
-            )
+        if variable == "dep" and "dep" in ds:
+            vmin, vmax = ds["dep"].raster.mask_nodata().quantile([0.0, 0.98]).values
             vmin, vmax = int(kwargs.pop("vmin", vmin)), int(kwargs.pop("vmax", vmax))
             c_dem = plt.cm.terrain(np.linspace(0.25, 1, vmax))
             if vmin < 0:
                 c_bat = plt.cm.terrain(np.linspace(0, 0.17, max(1, abs(vmin))))
                 c_dem = np.vstack((c_bat, c_dem))
             cmap = colors.LinearSegmentedColormap.from_list("dem", c_dem)
             norm = colors.Normalize(vmin=vmin, vmax=vmax)
             cmap, norm = kwargs.pop("cmap", cmap), kwargs.pop("norm", norm)
-            kwargs.update(norm=norm, cmap=cmap)
-
-    if variable in staticmaps:
-        da = staticmaps[variable].raster.mask_nodata()
-        # by default colorbar on lower right & legend upper right
-        kwargs0 = {"cbar_kwargs": {"shrink": 0.6, "anchor": (0, 0)}}
-        kwargs0.update(kwargs)
-        da.plot(transform=utm, ax=ax, zorder=1, **kwargs0)
-        if shaded and variable == "dep":
+            kwargs0.update(norm=norm, cmap=cmap)
+        elif variable == "msk" and "msk" in ds:
+            cmap = colors.LinearSegmentedColormap.from_list(
+                "Set1", ["grey", "r", "m"], N=4
+            )
+            norm = colors.BoundaryNorm([0.5, 1.5, 2.5, 3.5], 3)
+            kwargs0.update(norm=norm, cmap=cmap)
+            kwargs0["cbar_kwargs"].update(ticks=[1, 2, 3])
+
+    if variable in ds:
+        da = ds[variable].raster.mask_nodata()
+        if np.any(ds["msk"] > 0):
+            da = da.where(ds["msk"] > 0)
+        if da.raster.rotation != 0 and "xc" in da.coords and "yc" in da.coords:
+            da.plot(transform=utm, x="xc", y="yc", ax=ax, zorder=1, **kwargs0)
+        else:
+            da.plot.imshow(transform=utm, ax=ax, zorder=1, **kwargs0)
+        if shaded and variable == "dep" and da.raster.rotation == 0:
             ls = colors.LightSource(azdeg=315, altdeg=45)
             dx, dy = da.raster.res
             _rgb = ls.shade(
                 da.fillna(0).values,
                 norm=kwargs["norm"],
                 cmap=kwargs["cmap"],
                 blend_mode="soft",
@@ -206,68 +222,58 @@
         zorder=4,
         path_effects=[
             patheffects.Stroke(linewidth=3, foreground="w"),
             patheffects.Normal(),
         ],
     )
     # plot mask boundaries
-    if plot_bounds:
-        gdf_msk = staticmaps["msk"].raster.vectorize()
-        region = (
-            (staticmaps["msk"] >= 1)
-            .astype("int16")
-            .raster.vectorize()
-            .drop(columns="value")
-        )
-        gdf_msk = gdf_msk[gdf_msk["value"] != 1]
-        gdf_msk["geometry"] = gdf_msk.boundary
-        region["geometry"] = region.boundary
-        gdf_msk = gpd.overlay(
-            gdf_msk, region, "intersection", keep_geom_type=False
-        ).explode()
-        gdf_msk = gdf_msk[gdf_msk.length > 0]
+    if plot_bounds and (ds["msk"] >= 1).any():
+        gdf_msk = get_bounds_vector(ds["msk"])
         gdf_msk2 = gdf_msk[gdf_msk["value"] == 2]
         gdf_msk3 = gdf_msk[gdf_msk["value"] == 3]
         if gdf_msk2.index.size > 0:
             gdf_msk2.plot(ax=ax, zorder=3, label="waterlevel bnd", **geom_style["msk2"])
         if gdf_msk3.index.size > 0:
             gdf_msk3.plot(ax=ax, zorder=3, label="outflow bnd", **geom_style["msk3"])
 
     # plot static geoms
     if plot_geoms:
-        geoms = geoms if isinstance(geoms, list) else list(staticgeoms.keys())
-        for name in geoms:
-            gdf = staticgeoms.get(name, None)
+        geom_names = geom_names if isinstance(geom_names, list) else list(geoms.keys())
+        for name in geom_names:
+            gdf = geoms.get(name, None)
             if gdf is None or name in ["region", "bbox"]:
                 continue
             # copy is important to keep annotate working if repeated
             kwargs = geom_style.get(name, {}).copy()
             annotate = kwargs.pop("annotate", False)
             gdf.plot(ax=ax, zorder=3, label=name, **kwargs)
-            if annotate:
+            if annotate and np.all(gdf.geometry.type == "Point"):
                 for label, row in gdf.iterrows():
                     x, y = row.geometry.x, row.geometry.y
                     ax.annotate(label, xy=(x, y), **ann_kwargs)
 
-    if "region" in staticgeoms and plot_region:
-        staticgeoms["region"].boundary.plot(ax=ax, ls="-", lw=0.5, color="k", zorder=2)
+    if "region" in geoms and plot_region:
+        geoms["region"].boundary.plot(
+            ax=ax, zorder=2, label="region", **geom_style["region"]
+        )
 
     # title, legend and labels
     ax.xaxis.set_visible(True)
     ax.yaxis.set_visible(True)
     ax.set_ylabel(f"y coordinate UTM zone {utm_zone} [m]")
     ax.set_xlabel(f"x coordinate UTM zone {utm_zone} [m]")
     variable = "base" if variable is None else variable
     ax.set_title(f"SFINCS {variable} map")
     # NOTE without defined loc it takes forever to find a 'best' location
     # by default outside plot
-    if geoms or plot_bounds:
+    if geom_names or plot_bounds:
         legend_kwargs0 = dict(
             bbox_to_anchor=(1.05, 1),
             title="Legend",
             loc="upper left",
             frameon=True,
+            prop=dict(size=8),
         )
         legend_kwargs0.update(**legend_kwargs)
         ax.legend(**legend_kwargs0)
 
     return fig, ax
```

### Comparing `hydromt_sfincs-0.2.1/hydromt_sfincs/sfincs.py` & `hydromt_sfincs-1.0.0/hydromt_sfincs/sfincs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,95 @@
-# -*- coding: utf-8 -*-
-import os
-from os.path import join, isfile, abspath, dirname, basename, isabs
+"""
+SfincsModel class
+"""
+from __future__ import annotations
+
 import glob
-import numpy as np
 import logging
-import pyflwdir
+import os
+from os.path import abspath, basename, dirname, isabs, isfile, join
+from pathlib import Path
+from typing import Any, Dict, List, Tuple, Union
+
 import geopandas as gpd
-from rasterio.warp import transform_bounds
-from shapely.geometry import box
+import hydromt
+import numpy as np
 import pandas as pd
 import xarray as xr
-from typing import Dict, Tuple, List
-from scipy import ndimage
-
-import hydromt
-from hydromt.models.model_api import Model
-from hydromt.vector import GeoDataArray
-from hydromt.raster import RasterDataset, RasterDataArray
+from hydromt.models.model_grid import GridModel
+from hydromt.raster import RasterDataArray
+from hydromt.vector import GeoDataArray, GeoDataset
+from pyproj import CRS
+from shapely.geometry import box
 
-from . import workflows, utils, plots, DATADIR
+from . import DATADIR, plots, utils, workflows
+from .regulargrid import RegularGrid
+from .sfincs_input import SfincsInput
 
 __all__ = ["SfincsModel"]
 
 logger = logging.getLogger(__name__)
 
 
-class SfincsModel(Model):
+class SfincsModel(GridModel):
+    # GLOBAL Static class variables that can be used by all methods within
+    # SfincsModel class. Typically list of variables (e.g. _MAPS) or
+    # dict with varname - filename pairs (e.g. thin_dams : thd)
     _NAME = "sfincs"
     _GEOMS = {
-        "gauges": "obs",
+        "observation_points": "obs",
         "weirs": "weir",
         "thin_dams": "thd",
     }  # parsed to dict of geopandas.GeoDataFrame
-    _FORCING = {
-        "waterlevel": ("bzs", "bnd"),  #  timeseries, locations tuple
-        "discharge": ("dis", "src"),
-        "precip": ("precip", None),
-        "precip2D": ("netampr", None),
-    }  # parsed to dict of hydromt.GeoDataArray if locations else xarray.DataArray
-    _MAPS = {
-        "elevtn": "dep",
-        "mask": "msk",
-        "curve_number": "scs",
-        "manning": "manning",
-        "infiltration": "qinf",
-    }  # parsed to hydromt.RasterDataset
+    _FORCING_1D = {
+        # timeseries (can be multiple), locations tuple
+        "waterlevel": (["bzs"], "bnd"),
+        "waves": (["bzi"], "bnd"),
+        "discharge": (["dis"], "src"),
+        "precip": (["precip"], None),
+        "wavespectra": (["bhs", "btp", "bwd", "bds"], "bwv"),
+        "wavemaker": (["whi", "wti", "wst"], "wvp"),  # TODO check names and test
+    }
+    _FORCING_NET = {
+        # 2D forcing sfincs name, rename tuple
+        "waterlevel": ("netbndbzsbzi", {"zs": "bzs", "zi": "bzi"}),
+        "discharge": ("netsrcdis", {"discharge": "dis"}),
+        "precip": ("netampr", {"Precipitation": "precip"}),
+        "press": ("netamp", {"barometric_pressure": "press"}),
+        "wind": ("netamuamv", {"eastward_wind": "wind_u", "northward_wind": "wind_v"}),
+    }
+    _FORCING_SPW = {"spiderweb": "spw"}  # TODO add read and write functions
+    _MAPS = ["msk", "dep", "scs", "manning", "qinf"]
+    _STATES = ["rst", "ini"]
     _FOLDERS = []
-    _CLI_ARGS = {"region": "setup_region", "res": "setup_topobathy"}
+    _CLI_ARGS = {"region": "setup_grid_from_region", "res": "setup_grid_from_region"}
     _CONF = "sfincs.inp"
     _DATADIR = DATADIR
     _ATTRS = {
         "dep": {"standard_name": "elevation", "unit": "m+ref"},
         "msk": {"standard_name": "mask", "unit": "-"},
         "scs": {
             "standard_name": "potential maximum soil moisture retention",
             "unit": "in",
         },
         "qinf": {"standard_name": "infiltration rate", "unit": "mm.hr-1"},
         "manning": {"standard_name": "manning roughness", "unit": "s.m-1/3"},
         "bzs": {"standard_name": "waterlevel", "unit": "m+ref"},
+        "bzi": {"standard_name": "wave height", "unit": "m"},
         "dis": {"standard_name": "discharge", "unit": "m3.s-1"},
-        "netampr": {"standard_name": "precipitation", "unit": "mm.hr-1"},
         "precip": {"standard_name": "precipitation", "unit": "mm.hr-1"},
     }
 
     def __init__(
         self,
-        root=None,
-        mode="w",
-        config_fn="sfincs.inp",
-        write_gis=True,
-        data_libs=None,
-        deltares_data=None,
-        artifact_data=None,
+        root: str = None,
+        mode: str = "w",
+        config_fn: str = "sfincs.inp",
+        write_gis: bool = True,
+        data_libs: Union[List[str], str] = None,
         logger=logger,
     ):
         """
         The SFINCS model class (SfincsModel) contains methods to read, write, setup and edit
         `SFINCS <https://sfincs.readthedocs.io/en/latest/>`_ models.
 
         Parameters
@@ -85,368 +98,401 @@
             Path to model folder
         mode: {'w', 'r+', 'r'}
             Open model in write, append or reading mode, by default 'w'
         config_fn: str, Path, optional
             Filename of model config file, by default "sfincs.inp"
         write_gis: bool
             Write model files additionally to geotiff and geojson, by default True
-        opt: dict
-            Values for model setup options, used when called from CLI
-        sources: dict
-            Library with references to data sources
+        data_libs: List, str
+            List of data catalog yaml files, by default None
+
         """
-        # model paths
+        # model folders
         self._write_gis = write_gis
         if write_gis and "gis" not in self._FOLDERS:
             self._FOLDERS.append("gis")
 
         super().__init__(
             root=root,
             mode=mode,
             config_fn=config_fn,
             data_libs=data_libs,
-            deltares_data=deltares_data,
-            artifact_data=artifact_data,
             logger=logger,
         )
 
+        # placeholder grid classes
+        self.grid_type = None
+        self.reggrid = None
+        self.quadtree = None
+        self.subgrid = xr.Dataset()
+
+    @property
+    def mask(self) -> xr.DataArray | None:
+        """Returns model mask"""
+        if self.grid_type == "regular":
+            if "msk" in self.grid:
+                return self.grid["msk"]
+            elif self.reggrid is not None:
+                return self.reggrid.empty_mask
+
     @property
-    def mask(self):
-        """Returns model mask map."""
-        name = self._MAPS["mask"]
-        da_mask = None
-        if name not in self._staticmaps and self._MAPS["elevtn"] in self._staticmaps:
-            da_elv = self.staticmaps[self._MAPS["elevtn"]]
-            da_mask = (da_elv != da_elv.raster.nodata).astype(np.uint8)
-            da_mask.raster.set_nodata(0)
-            self.set_staticmaps(da_mask, name)
-        elif name in self._staticmaps:
-            da_mask = self.staticmaps[name]
-        return da_mask
+    def region(self) -> gpd.GeoDataFrame:
+        """Returns the geometry of the active model cells."""
+        # NOTE overwrites property in GridModel
+        region = gpd.GeoDataFrame()
+        if "region" in self.geoms:
+            region = self.geoms["region"]
+        elif "msk" in self.grid and np.any(self.grid["msk"] > 0):
+            da = xr.where(self.mask > 0, 1, 0).astype(np.int16)
+            da.raster.set_nodata(0)
+            region = da.raster.vectorize().dissolve()
+        elif self.reggrid is not None:
+            region = self.reggrid.empty_mask.raster.box
+        return region
 
-    def setup_basemaps(
-        self, basemaps_fn, res=100, crs="utm", reproj_method="bilinear", **kwargs
+    @property
+    def crs(self) -> CRS | None:
+        """Returns the model crs"""
+        if self.grid_type == "regular":
+            return self.reggrid.crs
+        elif self.grid_type == "quadtree":
+            return self.quadtree.crs
+
+    def set_crs(self, crs: Any) -> None:
+        """Sets the model crs"""
+        if self.grid_type == "regular":
+            self.reggrid.crs = CRS.from_user_input(crs)
+            self.grid.raster.set_crs(self.reggrid.crs)
+        elif self.grid_type == "quadtree":
+            self.quadtree.crs = CRS.from_user_input(crs)
+
+    def setup_grid(
+        self,
+        x0: float,
+        y0: float,
+        dx: float,
+        dy: float,
+        nmax: int,
+        mmax: int,
+        rotation: float,
+        epsg: int,
     ):
-        self.logger.warning(
-            "'setup_basemaps' is deprecated use 'setup_topobathy instead'"
-        )
-        if kwargs:
-            self.logger.warning(f"{list(kwargs.keys())} arguments ignored")
-        self.setup_topobathy(
-            topobathy_fn=basemaps_fn, res=res, crs=crs, reproj_method=reproj_method
+        """Setup a regular or quadtree grid.
+
+        Parameters
+        ----------
+        x0, y0 : float
+            x,y coordinates of the origin of the grid
+        dx, dy : float
+            grid cell size in x and y direction
+        mmax, nmax : int
+            number of grid cells in x and y direction
+        rotation : float, optional
+            rotation of grid [degree angle], by default None
+        epsg : int, optional
+            epsg-code of the coordinate reference system, by default None
+        """
+        # TODO gdf_refinement for quadtree
+
+        self.config.update(
+            x0=x0,
+            y0=y0,
+            dx=dx,
+            dy=dy,
+            nmax=nmax,
+            mmax=mmax,
+            rotation=rotation,
+            epsg=epsg,
         )
+        self.update_grid_from_config()
 
-    def setup_topobathy(
+    def setup_grid_from_region(
         self,
-        topobathy_fn,
-        res=100,
-        crs="utm",
-        reproj_method="bilinear",
+        region: dict,
+        res: float = 100,
+        crs: Union[str, int] = "utm",
+        rotated: bool = False,
+        hydrography_fn: str = None,
+        basin_index_fn: str = None,
+        dec_origin: int = 0,
+        dec_rotation: int = 3,
     ):
-        """Setup model grid and interpolate topobathy (dep) data to this grid.
+        """Setup a regular or quadtree grid from a region.
 
-        NOTE: This method should be called after `setup_region` but before any other model component.
+        Parameters
+        ----------
+        region : dict
+            Dictionary describing region of interest, e.g.:
 
-        The input topobathy dataset is reprojected to the model projected `crs` and
-        resolution `res` using `reproj_method` interpolation.
+            * {'bbox': [xmin, ymin, xmax, ymax]}
+            * {'geom': 'path/to/polygon_geometry'}
+
+            For a complete overview of all region options,
+            see :py:function:~hydromt.workflows.basin_mask.parse_region
+        res : float, optional
+            grid resolution, by default 100 m
+        crs : Union[str, int], optional
+            coordinate reference system of the grid
+            if "utm" (default) the best UTM zone is selected
+            else a pyproj crs string or epsg code (int) can be provided
+        grid_type : str, optional
+            grid type, "regular" (default) or "quadtree"
+        rotated : bool, optional
+            if True, a minimum rotated rectangular grid is fitted around the region, by default False
+        hydrography_fn : str
+            Name of data source for hydrography data.
+        basin_index_fn : str
+            Name of data source with basin (bounding box) geometries associated with
+            the 'basins' layer of `hydrography_fn`. Only required if the `region` is
+            based on a (sub)(inter)basins without a 'bounds' argument.
+        dec_origin : int, optional
+            number of decimals to round the origin coordinates, by default 0
+        dec_rotation : int, optional
+            number of decimals to round the rotation angle, by default 3
+
+        See Also
+        --------
+        hydromt.workflows.basin_mask.parse_region
+        """
+        # setup `region` of interest of the model.
+        self.setup_region(
+            region=region,
+            hydrography_fn=hydrography_fn,
+            basin_index_fn=basin_index_fn,
+        )
+        # get pyproj crs of best UTM zone if crs=utm
+        pyproj_crs = hydromt.gis_utils.parse_crs(
+            crs, self.region.to_crs(4326).total_bounds
+        )
+        if self.geoms["region"].crs != pyproj_crs:
+            self.geoms["region"] = self.geoms["region"].to_crs(pyproj_crs)
+
+        # create grid from region
+        # NOTE keyword rotated is added to still have the possibility to create unrotated grids if needed (e.g. for FEWS?)
+        if rotated:
+            geom = self.geoms["region"].unary_union
+            x0, y0, mmax, nmax, rot = utils.rotated_grid(
+                geom, res, dec_origin=dec_origin, dec_rotation=dec_rotation
+            )
+        else:
+            x0, y0, x1, y1 = self.geoms["region"].total_bounds
+            x0, y0 = round(x0, dec_origin), round(y0, dec_origin)
+            mmax = int(np.ceil((x1 - x0) / res))
+            nmax = int(np.ceil((y1 - y0) / res))
+            rot = 0
+        self.setup_grid(
+            x0=x0,
+            y0=y0,
+            dx=res,
+            dy=res,
+            nmax=nmax,
+            mmax=mmax,
+            rotation=rot,
+            epsg=pyproj_crs.to_epsg(),
+        )
 
-        Adds model layers:
+    def setup_dep(
+        self,
+        datasets_dep: List[dict],
+        buffer_cells: int = 0,  # not in list
+        interp_method: str = "linear",  # used for buffer cells only
+    ):
+        """Interpolate topobathy (dep) data to the model grid.
+
+        Adds model grid layers:
 
-        * **dep** map: combined elevation/bathymetry [m+ref]
+        * **dep**: combined elevation/bathymetry [m+ref]
 
         Parameters
         ----------
-        topobathy_fn : str
-            Path or data source name for topobathy raster data.
-        res : float
-            Model resolution [m], by default 100 m.
-            If None, the basemaps res is used.
-        crs : str, int, optional
-            Model Coordinate Reference System (CRS) as epsg code.
-            By default 'utm' in which case the region centroid UTM zone is used.
-            If None, the basemaps CRS is used. This must be a projected CRS.
-        reproj_method: str, optional
-            Method used to reproject topobathy data, by default 'bilinear'
-        """
-        if self.region is None:
-            raise ValueError("Model region not found, run `setup_region` first.")
-        geom = self.region.dissolve()
-
-        # parse crs. if 'utm' the utm zone is calculated based the region
-        if crs is not None:
-            crs = hydromt.gis_utils.parse_crs(crs, geom.to_crs(4326).total_bounds)
-        if crs is not None and crs.is_geographic:
-            raise ValueError("A projected CRS is required.")
-        if crs is not None and geom.crs != crs:
-            # if geom is a rectangular bbox, transform it to a rect bbox in crs
-            poly = geom.geometry[0]
-            if np.isclose(poly.minimum_rotated_rectangle.area, poly.area):
-                dst_bbox = transform_bounds(geom.crs, crs, *geom.total_bounds)
-                geom = gpd.GeoDataFrame(geometry=[box(*dst_bbox)], crs=crs)
-            else:
-                geom = geom.to_crs(crs.to_epsg())
+        datasets_dep : List[dict]
+            List of dictionaries with topobathy data, each containing a dataset name or Path (elevtn) and optional merge arguments e.g.:
+            [{'elevtn': merit_hydro, 'zmin': 0.01}, {'elevtn': gebco, 'offset': 0, 'merge_method': 'first', reproj_method: 'bilinear'}]
+            For a complete overview of all merge options, see :py:function:~hydromt.workflows.merge_multi_dataarrays
+        buffer_cells : int, optional
+            Number of cells between datasets to ensure smooth transition of bed levels, by default 0
+        interp_method : str, optional
+            Interpolation method used to fill the buffer cells , by default "linear"
+        """
 
-        # read global data (lazy!)
-        da_elv = self.data_catalog.get_rasterdataset(
-            topobathy_fn, geom=geom, buffer=20, variables=["elevtn"]
-        )
+        # retrieve model resolution to determine zoom level for xyz-datasets
+        # TODO fix for quadtree
+        if not self.mask.raster.crs.is_geographic:
+            res = np.abs(self.mask.raster.res[0])
+        else:
+            res = np.abs(self.mask.raster.res[0]) * 111111.0
 
-        # reproject to destination CRS
-        check_crs = crs is not None and da_elv.raster.crs != crs
-        check_res = abs(da_elv.raster.res[0]) != res
-        if check_crs or check_res:
-            da_elv = da_elv.raster.reproject(
-                dst_res=res, dst_crs=crs, align=True, method=reproj_method
-            )
-        # clip & mask
-        da_elv = (
-            da_elv.raster.clip_geom(geom, mask=True)
-            .raster.mask_nodata()
-            .fillna(-9999)  # force nodata value to be -9999
-            .round(2)  # cm precision
-        )
-        da_elv.raster.set_nodata(-9999)
+        datasets_dep = self._parse_datasets_dep(datasets_dep, res=res)
 
-        # set staticmaps
-        name = self._MAPS["elevtn"]
-        da_elv.attrs.update(**self._ATTRS.get(name, {}))
-        self.set_staticmaps(data=da_elv, name=name)
-        # update config
-        self.update_spatial_attrs()
-
-    def setup_merge_topobathy(
-        self,
-        topobathy_fn,
-        elv_min=None,
-        elv_max=None,
-        mask_fn=None,
-        max_width=0,
-        offset_fn=None,
-        offset_constant=0,
-        merge_buffer=0,
-        merge_method="first",
-        reproj_method="bilinear",
-        interp_method="linear",
-    ):
-        """Updates the existing model topobathy data (dep file) with a new topobathy
-        source within the current model extent.
-
-        By default (`merge_method="first"`) invalid (nodata) cells in the current topobathy
-        data are replaced with values from the new topobathy source.
-
-        Use `offset_fn` for a spatially varying, or `offset_constant` for a spatially uniform
-        offset to convert the vertical datum of the new source before merging.
-
-        Gaps in the data (i.e. areas with nodata cells surrounded areas with valid elevation)
-        are interpolated based on `interp_method`, by deafult 'linear'. Gaps are not
-        interpolated if `interp_method = None`
-
-        Updates model layer:
-
-        * **dep** map: combined elevation/bathymetry [m+ref]
-
-        Parameters
-        ----------
-        topobathy_fn : str, optional
-            Path or data source name for topobathy raster data.
-
-            * Required variables: ['elevtn']
-        mask_fn : str, optional
-            Path or data source name of polygon with valid new topobathy cells.
-        max_width: int, optional
-            Maximum width (number of cells) to append to valid dep cells if larger than
-            zero. By default 0.
-        elv_min, elv_max : float, optional
-            Minimum and maximum elevation caps for new topobathy cells, cells outside
-            this range are linearly interpolated. Note: applied after offset!
-        offset_fn : str, optional
-            Path or data source name for Spatially varying map with difference between
-            the vertical reference of the current model topobathy and the new data source [m].
-            The offset is added to the new source before merging.
-        offset_fn : float, optional
-            Same as `offset_fn` but spatially uniform value [m].
-        merge_buffer : int, optional
-            Buffer (number of cells) around the original (`merge_method = 'first'`)
-            or new (`merge_method = 'last'`) data source where values are interpolated
-            using `interp_method`.
-            Not recommended to use in combination with merge_methods 'min' or 'max'
-        merge_method: {'first','last','min','max'}, optional
-            merge method, by default 'first':
-
-            * first: use valid new where existing invalid
-            * last: use valid new
-            * min: pixel-wise min of existing and new
-            * max: pixel-wise max of existing and new
-        reproj_method: {'bilinear', 'cubic', 'nearest'}
-            Method used to reproject the offset and second dataset to the grid of the
-            new topobathy dataset, by default 'bilinear'
-        interp_method, {'linear', 'nearest', 'rio_idw'}, optional
-            Method used to interpolate holes of nodata in the merged dataset,
-            by default 'linear'. If None holes are not interpolated.
-        """
-        name = self._MAPS["elevtn"]
-        assert name in self.staticmaps
-        da_elv = self.staticmaps[name]
-        geom = self.staticmaps.raster.box
-        da_elv2 = self.data_catalog.get_rasterdataset(
-            topobathy_fn, geom=geom, buffer=10, variables=["elevtn"]
-        )
-        kwargs = dict(
-            reproj_method=reproj_method,
-            interp_method=interp_method,
-            merge_buffer=merge_buffer,
-            merge_method=merge_method,
-            max_width=max_width,
-        )
-        # mask
-        if mask_fn is not None:
-            gdf_mask = self.data_catalog.get_geodataframe(mask_fn)
-            da_elv2 = da_elv2.raster.clip_geom(gdf_mask, mask=True)
-        # offset
-        if offset_fn is not None:
-            # variable name not important, but must be single variable
-            da_offset = self.data_catalog.get_rasterdataset(
-                offset_fn, geom=geom, buffer=10
-            )
-            assert isinstance(da_offset, xr.DataArray)
-            kwargs.update(da_offset=da_offset)
-        elif offset_constant > 0:
-            kwargs.update(da_offset=offset_constant)
-        # merge
-        da_dep_merged = workflows.merge_topobathy(
-            da_elv,
-            da_elv2,
-            elv_min=elv_min,
-            elv_max=elv_max,
-            logger=self.logger,
-            **kwargs,
-        )
-        self.set_staticmaps(data=da_dep_merged.round(2), name=name)
+        if self.grid_type == "regular":
+            da_dep = workflows.merge_multi_dataarrays(
+                da_list=datasets_dep,
+                da_like=self.mask,
+                buffer_cells=buffer_cells,
+                interp_method=interp_method,
+                logger=self.logger,
+            )
+
+            # check if no nan data is present in the bed levels
+            if not np.isnan(da_dep).any():
+                self.logger.warning(
+                    f"Interpolate data at {int(np.sum(np.isnan(da_dep.values)))} cells"
+                )
+                da_dep = da_dep.raster.interpolate_na(method="rio_idw")
+
+            self.set_grid(da_dep, name="dep")
+            # FIXME this shouldn't be necessary, since da_dep should already have the crs
+            if self.crs is not None and self.grid.raster.crs is None:
+                self.grid.set_crs(self.crs)
 
-    def setup_mask(
+            if "depfile" not in self.config:
+                self.config.update({"depfile": "sfincs.dep"})
+        elif self.grid_type == "quadtree":
+            raise NotImplementedError(
+                "Create dep not yet implemented for quadtree grids."
+            )
+
+    def setup_mask_active(
         self,
-        mask_fn=None,
-        include_mask_fn=None,
-        exclude_mask_fn=None,
-        elv_min=None,
-        elv_max=None,
-        fill_area=10,
-        drop_area=0,
-        connectivity=8,
-        all_touched=True,
-        reset_mask=False,
-        **kwargs,  # to catch deprecated args
-    ):
-        """Creates mask of active model cells.
-
-        The SFINCS model mask defines 0) Inactive, 1) active, and 2) waterlevel boundary
-        and 3) outflow boundary cells. This method sets the active cells set using,
-        while boundary cells are set in the `setup_bounds` method.
+        mask: Union[str, Path, gpd.GeoDataFrame] = None,
+        include_mask: Union[str, Path, gpd.GeoDataFrame] = None,
+        exclude_mask: Union[str, Path, gpd.GeoDataFrame] = None,
+        mask_buffer: int = 0,
+        zmin: float = None,
+        zmax: float = None,
+        fill_area: float = 10.0,
+        drop_area: float = 0.0,
+        connectivity: int = 8,
+        all_touched: bool = True,
+        reset_mask: bool = False,
+    ):
+        """Setup active model cells.
 
-        Active model cells are based on cells with valid elevation (i.e. not nodata),
+        The SFINCS model mask defines inactive (msk=0), active (msk=1), and waterlevel boundary (msk=2)
+        and outflow boundary (msk=3) cells. This method sets the active and inactive cells.
+
+        Active model cells are based on a region and cells with valid elevation (i.e. not nodata),
         optionally bounded by areas inside the include geomtries, outside the exclude geomtries,
         larger or equal than a minimum elevation threshhold and smaller or equal than a
         maximum elevation threshhold.
         All conditions are combined using a logical AND operation.
 
-        NOTE: Inactive cells are set to nodata values in all staticmaps which cannot be undone!
-
         Sets model layers:
 
         * **msk** map: model mask [-]
 
         Parameters
         ----------
-        mask_fn: str, optional
-            Path or data source name of polygons describing the initial region with active model cells.
-            If not given, the initial active model cells are based on valid elevation cells.
-        include_mask_fn, exclude_mask_fn: str, optional
+        mask: str, Path, gpd.GeoDataFrame, optional
+            Path or data source name of polygons to initiliaze active mask with; proceding arguments can be used to include/exclude cells
+            If not given, existing mask (if present) used, else mask is initialized empty.
+        include_mask, exclude_mask: str, Path, gpd.GeoDataFrame, optional
             Path or data source name of polygons to include/exclude from the active model domain.
-            Note that exclude (second last) and include (last) areas are processed after other critera,
-            i.e. `elv_min`, `elv_max` and `drop_area`, and thus overrule these criteria for active model cells.
-        elv_min, elv_max : float, optional
+            Note that include (second last) and exclude (last) areas are processed after other critera,
+            i.e. `zmin`, `zmax` and `drop_area`, and thus overrule these criteria for active model cells.
+        mask_buffer: float, optional
+            If larger than zero, extend the `include_mask` geometry with a buffer [m],
+            by default 0.
+        zmin, zmax : float, optional
             Minimum and maximum elevation thresholds for active model cells.
         fill_area : float, optional
-            Maximum area [km2] of contiguous cells below `elv_min` or above `elv_max` but surrounded
+            Maximum area [km2] of contiguous cells below `zmin` or above `zmax` but surrounded
             by cells within the valid elevation range to be kept as active cells, by default 10 km2.
         drop_area : float, optional
             Maximum area [km2] of contiguous cells to be set as inactive cells, by default 0 km2.
         connectivity, {4, 8}:
             The connectivity used to define contiguous cells, if 4 only horizontal and vertical
             connections are used, if 8 (default) also diagonal connections.
         all_touched: bool, optional
             if True (default) include (or exclude) a cell in the mask if it touches any of the
             include (or exclude) geometries. If False, include a cell only if its center is
             within one of the shapes, or if it is selected by Bresenham's line algorithm.
         reset_mask: bool, optional
             If True, reset existing mask layer. If False (default) updating existing mask.
-            Note that previously set inactive cells can not be reset to active cells.
         """
-        if "active_mask_fn" in kwargs:
-            self.logger.warning("'active_mask_fn' is deprecated use 'mask_fn' instead.")
-            mask_fn = kwargs.pop("active_mask_fn")
-
-        if reset_mask and self._MAPS["mask"] in self.staticmaps:  # reset
-            self._staticmaps = self._staticmaps.drop_vars(self._MAPS["mask"])
-
         # read geometries
-        gdf0, gdf1, gdf2 = None, None, None
+        gdf_mask, gdf_include, gdf_exclude = None, None, None
         bbox = self.region.to_crs(4326).total_bounds
-        if mask_fn is not None:
-            gdf0 = self.data_catalog.get_geodataframe(mask_fn, bbox=bbox)
-        if include_mask_fn is not None:
-            gdf1 = self.data_catalog.get_geodataframe(include_mask_fn, bbox=bbox)
-        if exclude_mask_fn is not None:
-            gdf2 = self.data_catalog.get_geodataframe(exclude_mask_fn, bbox=bbox)
+        if mask is not None:
+            if not isinstance(mask, gpd.GeoDataFrame) and str(mask).endswith(".pol"):
+                # NOTE polygons should be in same CRS as model
+                gdf_mask = utils.polygon2gdf(
+                    feats=utils.read_geoms(fn=mask), crs=self.region.crs
+                )
+            else:
+                gdf_mask = self.data_catalog.get_geodataframe(mask, bbox=bbox)
+            if mask_buffer > 0:  # NOTE assumes model in projected CRS!
+                gdf_mask["geometry"] = gdf_mask.to_crs(self.crs).buffer(mask_buffer)
+        if include_mask is not None:
+            if not isinstance(include_mask, gpd.GeoDataFrame) and str(
+                include_mask
+            ).endswith(".pol"):
+                # NOTE polygons should be in same CRS as model
+                gdf_include = utils.polygon2gdf(
+                    feats=utils.read_geoms(fn=include_mask), crs=self.region.crs
+                )
+            else:
+                gdf_include = self.data_catalog.get_geodataframe(
+                    include_mask, bbox=bbox
+                )
+        if exclude_mask is not None:
+            if not isinstance(exclude_mask, gpd.GeoDataFrame) and str(
+                exclude_mask
+            ).endswith(".pol"):
+                gdf_exclude = utils.polygon2gdf(
+                    feats=utils.read_geoms(fn=exclude_mask), crs=self.region.crs
+                )
+            else:
+                gdf_exclude = self.data_catalog.get_geodataframe(
+                    exclude_mask, bbox=bbox
+                )
 
         # get mask
-        da_mask = utils.mask_topobathy(
-            da_elv=self.staticmaps[self._MAPS["elevtn"]],
-            gdf_mask=gdf0,
-            gdf_include=gdf1,
-            gdf_exclude=gdf2,
-            elv_min=elv_min,
-            elv_max=elv_max,
-            fill_area=fill_area,
-            drop_area=drop_area,
-            connectivity=connectivity,
-            all_touched=all_touched,
-            logger=self.logger,
-        )
+        if self.grid_type == "regular":
+            da_mask = self.reggrid.create_mask_active(
+                da_mask=self.grid["msk"] if "msk" in self.grid else None,
+                da_dep=self.grid["dep"] if "dep" in self.grid else None,
+                gdf_mask=gdf_mask,
+                gdf_include=gdf_include,
+                gdf_exclude=gdf_exclude,
+                zmin=zmin,
+                zmax=zmax,
+                fill_area=fill_area,
+                drop_area=drop_area,
+                connectivity=connectivity,
+                all_touched=all_touched,
+                reset_mask=reset_mask,
+                logger=self.logger,
+            )
+            self.set_grid(da_mask, name="msk")
+            # update config
+            if "mskfile" not in self.config:
+                self.config.update({"mskfile": "sfincs.msk"})
+            if "indexfile" not in self.config:
+                self.config.update({"indexfile": "sfincs.ind"})
+            # update region
+            self.logger.info("Derive region geometry based on active cells.")
+            region = da_mask.where(da_mask <= 1, 1).raster.vectorize()
+            self.set_geoms(region, "region")
 
-        n = np.count_nonzero(da_mask.values)
-        self.logger.debug(f"Mask with {n:d} active cells set; updating staticmaps ...")
-        # update all staticmaps
-        for name in self._staticmaps.raster.vars:
-            da = self._staticmaps[name]
-            self._staticmaps[name] = da.where(da_mask, da.raster.nodata)
-        # update sfincs mask with boolean mask to conserve mask values
-        da_mask = self.mask.where(da_mask, np.uint8(0))  # unint8 dtype!
-        self.set_staticmaps(da_mask, self._MAPS["mask"])
-
-        self.logger.debug(f"Derive region geometry based on active cells.")
-        region = da_mask.where(da_mask <= 1, 1).raster.vectorize()
-        self.set_staticgeoms(region, "region")
-
-    def setup_bounds(
-        self,
-        btype="waterlevel",
-        mask_fn=None,
-        include_mask_fn=None,
-        exclude_mask_fn=None,
-        elv_min=None,
-        elv_max=None,
-        mask_buffer=0,
-        connectivity=8,
-        reset_bounds=False,
+    def setup_mask_bounds(
+        self,
+        btype: str = "waterlevel",
+        include_mask: Union[str, Path, gpd.GeoDataFrame] = None,
+        exclude_mask: Union[str, Path, gpd.GeoDataFrame] = None,
+        zmin: float = None,
+        zmax: float = None,
+        connectivity: int = 8,
+        all_touched: bool = False,
+        reset_bounds: bool = False,
     ):
         """Set boundary cells in the model mask.
 
-        The SFINCS model mask defines 0) Inactive, 1) active, and 2) waterlevel boundary
-        and 3) outflow boundary cells. Active cells set using the `setup_mask` method,
+        The SFINCS model mask defines inactive (msk=0), active (msk=1), and waterlevel boundary (msk=2)
+        and outflow boundary (msk=3) cells. Active cells set using the `setup_mask` method,
         while this method sets both types of boundary cells, see `btype` argument.
 
         Boundary cells at the edge of the active model domain,
         optionally bounded by areas inside the include geomtries, outside the exclude geomtries,
         larger or equal than a minimum elevation threshhold and smaller or equal than a
         maximum elevation threshhold.
         All conditions are combined using a logical AND operation.
@@ -455,1102 +501,1131 @@
 
         * **msk** map: model mask [-]
 
         Parameters
         ----------
         btype: {'waterlevel', 'outflow'}
             Boundary type
-        mask_fn: str, optional
-            Path or data source name of polygons describing the initial region constraining model boundary cells.
-        include_mask_fn, exclude_mask_fn: str, optional
+        include_mask, exclude_mask: str, Path, gpd.GeoDataFrame, optional
             Path or data source name for geometries with areas to include/exclude from the model boundary.
-            Note that exclude (second last) and include (last) areas are processed after other critera,
-            i.e. `elv_min`, `elv_max`, and thus overrule these criteria for model boundary cells.
-        elv_min, elv_max : float, optional
+        zmin, zmax : float, optional
             Minimum and maximum elevation thresholds for boundary cells.
-        mask_buffer: float, optional
-            If larger than zero, extend the `mask_fn` geometry with a buffer [m],
-            by default 0.
+            Note that when include and exclude areas are used, the elevation range is only applied
+            on cells within the include area and outside the exclude area.
         reset_bounds: bool, optional
             If True, reset existing boundary cells of the selected boundary
             type (`btype`) before setting new boundary cells, by default False.
+        all_touched: bool, optional
+            if True (default) include (or exclude) a cell in the mask if it touches any of the
+            include (or exclude) geometries. If False, include a cell only if its center is
+            within one of the shapes, or if it is selected by Bresenham's line algorithm.
         connectivity, {4, 8}:
             The connectivity used to detect the model edge, if 4 only horizontal and vertical
             connections are used, if 8 (default) also diagonal connections.
         """
-        btype = btype.lower()
-        bvalues = {"waterlevel": 2, "outflow": 3}
-        if btype not in bvalues:
-            raise ValueError('btype must be one of "waterlevel", "outflow"')
-        bvalue = bvalues[btype]
 
-        # get mask / include / exclude geometries
-        gdf0, gdf_include, gdf_exclude = None, None, None
+        # get include / exclude geometries
+        gdf_include, gdf_exclude = None, None
         bbox = self.region.to_crs(4326).total_bounds
-        if mask_fn:
-            gdf0 = self.data_catalog.get_geodataframe(mask_fn, bbox=bbox)
-            if mask_buffer > 0:  # NOTE assumes model in projected CRS!
-                gdf0["geometry"] = gdf0.to_crs(self.crs).buffer(mask_buffer)
-        if include_mask_fn:
-            gdf_include = self.data_catalog.get_geodataframe(include_mask_fn, bbox=bbox)
-        if exclude_mask_fn:
-            gdf_exclude = self.data_catalog.get_geodataframe(exclude_mask_fn, bbox=bbox)
+        if include_mask is not None:
+            if not isinstance(include_mask, gpd.GeoDataFrame) and str(
+                include_mask
+            ).endswith(".pol"):
+                # NOTE polygons should be in same CRS as model
+                gdf_include = utils.polygon2gdf(
+                    feats=utils.read_geoms(fn=include_mask), crs=self.region.crs
+                )
+            else:
+                gdf_include = self.data_catalog.get_geodataframe(
+                    include_mask, bbox=bbox
+                )
+        if exclude_mask is not None:
+            if not isinstance(exclude_mask, gpd.GeoDataFrame) and str(
+                exclude_mask
+            ).endswith(".pol"):
+                gdf_exclude = utils.polygon2gdf(
+                    feats=utils.read_geoms(fn=exclude_mask), crs=self.region.crs
+                )
+            else:
+                gdf_exclude = self.data_catalog.get_geodataframe(
+                    exclude_mask, bbox=bbox
+                )
 
         # mask values
-        bounds = utils.mask_bounds(
-            da_msk=self.mask,
-            da_elv=self.staticmaps[self._MAPS["elevtn"]],
-            gdf_mask=gdf0,
-            gdf_include=gdf_include,
-            gdf_exclude=gdf_exclude,
-            elv_min=elv_min,
-            elv_max=elv_max,
-            connectivity=connectivity,
-        )
-
-        # update model mask
-        da_mask = self.mask
-        if reset_bounds:  # reset existing boundary cells
-            self.logger.debug(f"{btype} (mask={bvalue:d}) boundary cells reset.")
-            da_mask = da_mask.where(da_mask != np.uint8(bvalue), np.uint8(1))
-        # avoid any msk3 cells neighboring msk2 cells
-        if bvalue == 3 and np.any(da_mask == 2):
-            msk2_dilated = ndimage.binary_dilation(
-                (da_mask == 2).values,
-                structure=np.ones((3, 3)),
-                iterations=1,  # minimal one cell distance between msk2 and msk3 cells
-            )
-            bounds = bounds.where(~msk2_dilated, False)
-        ncells = np.count_nonzero(bounds.values)
-        if ncells > 0:
-            da_mask = da_mask.where(~bounds, np.uint8(bvalue))
-            self.set_staticmaps(da_mask, self._MAPS["mask"])
-            self.logger.debug(
-                f"{ncells:d} {btype} (mask={bvalue:d}) boundary cells set."
+        if self.grid_type == "regular":
+            da_mask = self.reggrid.create_mask_bounds(
+                da_mask=self.grid["msk"],
+                btype=btype,
+                gdf_include=gdf_include,
+                gdf_exclude=gdf_exclude,
+                da_dep=self.grid["dep"] if "dep" in self.grid else None,
+                zmin=zmin,
+                zmax=zmax,
+                connectivity=connectivity,
+                all_touched=all_touched,
+                reset_bounds=reset_bounds,
+                logger=self.logger,
             )
+            self.set_grid(da_mask, name="msk")
 
-    def setup_river_hydrography(self, hydrography_fn=None, adjust_dem=False, **kwargs):
-        """Setup hydrography layers for flow directions ("flwdir") and upstream area
-        ("uparea") which are required to setup the setup_river* model components.
-
-        If no hydrography data is provided (`hydrography_fn=None`) flow directions are
-        derived from the model elevation data.
-        Note that in that case the upstream area map will miss the contribution from area
-        upstream of the model domain and incoming rivers in the `setup_river_inflow`
-        cannot be detected.
-
-        If the model crs or resolution is different from the input hydrography data,
-        it is reprojected to the model grid. Note that this works best if the destination
-        resolution is roughly the same or higher (i.e. smaller cells).
-
-        Adds model layers (both not used by SFINCS!):
-
-        * **uparea** map: upstream area [km2]
-        * **flwdir** map: local D8 flow directions [-]
-
-        Updates model layer (if `adjust_dem=True`):
+    def setup_subgrid(
+        self,
+        datasets_dep: List[dict],
+        datasets_rgh: List[dict] = [],
+        buffer_cells: int = 0,
+        nbins: int = 10,
+        nr_subgrid_pixels: int = 20,
+        nrmax: int = 2000,  # blocksize
+        max_gradient: float = 5.0,
+        z_minimum: float = -99999.0,
+        manning_land: float = 0.04,
+        manning_sea: float = 0.02,
+        rgh_lev_land: float = 0.0,
+        write_dep_tif: bool = False,
+        write_man_tif: bool = False,
+    ):
+        """Setup method for subgrid tables based on a list of
+        elevation and Manning's roughness datasets.
 
-        * **dep** map: combined elevation/bathymetry [m+ref]
+        These datasets are used to derive relations between the water level
+        and the volume in a cell to do the continuity update,
+        and a representative water depth used to calculate momentum fluxes.
+
+        This allows that one can compute on a coarser computational grid,
+        while still accounting for the local topography and roughness.
 
         Parameters
         ----------
-        hydrography_fn : str
-            Path or data source name for hydrography raster data, by default None
-            and derived from model elevation data.
+        datasets_dep : List[dict]
+            List of dictionaries with topobathy data.
+            Each should minimally contain a data catalog source name, data file path, or xarray raster object ('elevtn')
+            Optional merge arguments include 'zmin', 'zmax', 'mask', 'offset', 'reproj_method', and 'merge_method'.
+            e.g.: [{'elevtn': merit_hydro, 'zmin': 0.01}, {'elevtn': gebco, 'offset': 0, 'merge_method': 'first', reproj_method: 'bilinear'}]
+            For a complete overview of all merge options, see :py:function:~hydromt.workflows.merge_multi_dataarrays
+        datasets_rgh : List[dict], optional
+            List of dictionaries with Manning's n datasets. Each dictionary should at least contain one of the following:
+            * (1) manning: filename (or Path) of gridded data with manning values
+            * (2) lulc (and reclass_table) :a combination of a filename of gridded landuse/landcover and a mapping table.
+            In additon, optional merge arguments can be provided e.g.: merge_method, gdf_valid_fn
+        buffer_cells : int, optional
+            Number of cells between datasets to ensure smooth transition of bed levels, by default 0
+        nbins : int, optional
+            Number of bins in the subgrid tables, by default 10
+        nr_subgrid_pixels : int, optional
+            Number of subgrid pixels per computational cell, by default 20
+        nrmax : int, optional
+            Maximum number of cells per subgrid-block, by default 2000
+            These blocks are used to prevent memory issues while working with large datasets
+        max_gradient : float, optional
+            Maximum gradient in the subgrid tables, by default 5.0
+        z_minimum : float, optional
+            Minimum depth in the subgrid tables, by default -99999.0
+        manning_land, manning_sea : float, optional
+            Constant manning roughness values for land and sea, by default 0.04 and 0.02 s.m-1/3
+            Note that these values are only used when no Manning's n datasets are provided, or to fill the nodata values
+        rgh_lev_land : float, optional
+            Elevation level to distinguish land and sea roughness (when using manning_land and manning_sea), by default 0.0
+        write_dep_tif : bool, optional
+            Create geotiff of the merged topobathy on the subgrid resolution, by default False
+        write_man_tif : bool, optional
+            Create geotiff of the merged roughness on the subgrid resolution, by default False
+        """
+
+        # retrieve model resolution
+        # TODO fix for quadtree
+        if not self.mask.raster.crs.is_geographic:
+            res = np.abs(self.mask.raster.res[0]) / nr_subgrid_pixels
+        else:
+            res = np.abs(self.mask.raster.res[0]) * 111111.0 / nr_subgrid_pixels
 
-            * Required variable: ['uparea']
-            * Optional variable: ['flwdir']
-        adjust_dem: bool, optional
-            Adjust the model elevation such that each downstream cell is at the
-            same or lower elevation. By default True.
-        """
-        name = self._MAPS["elevtn"]
-        assert name in self.staticmaps
-        da_elv = self.staticmaps[name]
-        if hydrography_fn is not None:
-            ds_hydro = self.data_catalog.get_rasterdataset(
-                hydrography_fn, geom=self.region, buffer=20, single_var_as_array=False
-            )
-            assert "uparea" in ds_hydro
-            warp = ~da_elv.raster.aligned_grid(ds_hydro)
-            if warp or "flwdir" not in ds_hydro:
-                self.logger.info("Reprojecting hydrography data to destination grid.")
-                ds_out = hydromt.flw.reproject_hydrography_like(
-                    ds_hydro, da_elv, logger=self.logger, **kwargs
-                )
-            else:
-                ds_out = ds_hydro[["uparea", "flwdir"]].raster.clip_bbox(
-                    da_elv.raster.bounds
-                )
-            ds_out = ds_out.raster.mask(da_elv != da_elv.raster.nodata)
+        datasets_dep = self._parse_datasets_dep(datasets_dep, res=res)
+
+        if len(datasets_rgh) > 0:
+            # NOTE conversion from landuse/landcover to manning happens here
+            datasets_rgh = self._parse_datasets_rgh(datasets_rgh)
+
+        # folder where high-resolution topobathy and manning geotiffs are stored
+        if write_dep_tif or write_man_tif:
+            highres_dir = os.path.join(self.root, "subgrid")
+            if not os.path.isdir(highres_dir):
+                os.makedirs(highres_dir)
         else:
-            self.logger.info("Getting hydrography data from model grid.")
-            da_flw = hydromt.flw.d8_from_dem(da_elv, **kwargs)
-            flwdir = hydromt.flw.flwdir_from_da(da_flw, ftype="d8")
-            da_upa = xr.DataArray(
-                dims=da_elv.raster.dims,
-                coords=da_elv.raster.coords,
-                data=flwdir.upstream_area(unit="km2"),
-                name="uparea",
-            )
-            da_upa.raster.set_nodata(-9999)
-            ds_out = xr.merge([da_upa, da_flw])
-
-        self.logger.info("Saving hydrography data to staticmaps.")
-        self.set_staticmaps(ds_out["uparea"])
-        self.set_staticmaps(ds_out["flwdir"])
-
-        if adjust_dem:
-            self.logger.info(f"Hydrologically adjusting {name} map.")
-            flwdir = hydromt.flw.flwdir_from_da(ds_out["flwdir"], ftype="d8")
-            da_elv.data = flwdir.dem_adjust(da_elv.values)
-            self.set_staticmaps(da_elv.round(2), name)
-
-    def setup_river_bathymetry(
-        self,
-        river_geom_fn=None,
-        river_mask_fn=None,
-        qbankfull_fn=None,
-        rivdph_method="gvf",
-        rivwth_method="geom",
-        river_upa=25.0,
-        river_len=1000,
-        min_rivwth=50.0,
-        min_rivdph=1.0,
-        rivbank=True,
-        rivbankq=25,
-        segment_length=3e3,
-        smooth_length=10e3,
-        constrain_rivbed=True,
-        constrain_estuary=True,
-        dig_river_d4=True,
-        plot_riv_profiles=0,
-        **kwargs,  # for workflows.get_river_bathymetry method
-    ):
-        """Burn rivers into the model elevation (dep) file.
-
-        NOTE: this method is experimental and may change in the near future.
-
-        River cells are based on the `river_mask_fn` raster file if `rivwth_method='mask'`,
-        or if `rivwth_method='geom'` the rasterized segments buffered with half a river width
-        ("rivwth" [m]) if that attribute is found in `river_geom_fn`.
-
-        If a river segment geometry file `river_geom_fn` with bedlevel column ("zb" [m+REF]) or
-        a river depth ("rivdph" [m]) in combination with `rivdph_method='geom'` is provided,
-        this attribute is used directly.
-
-        Otherwise, a river depth is estimated based on bankfull discharge ("qbankfull" [m3/s])
-        attribute taken from the nearest river segment in `river_geom_fn` or `qbankfull_fn`
-        upstream river boundary points if provided.
-
-        The river depth is relative to the bankfull elevation profile if `rivbank=True` (default),
-        which is estimated as the `rivbankq` elevation percentile [0-100] of cells neighboring river cells.
-        This option requires the flow direction ("flwdir") and upstream area ("uparea") maps to be set
-        using the "setup_river_hydrography" method. If `rivbank=False` the depth is simply subtracted
-        from the elevation of river cells.
-
-        Missing river width and river depth values are filled by propagating valid values downstream and
-        using the constant minimum values `min_rivwth` and `min_rivdph` for the remaining missing values.
-
-        Updates model layer:
-
-        * **dep** map: combined elevation/bathymetry [m+ref]
-
-        Adds model layers
-
-        * **rivmsk** map: map of river cells (not used by SFINCS)
-        * **rivers** geom: geometry of rivers (not used by SFINCS)
-
-        Parameters
-        ----------
-        river_geom_fn : str, optional
-            Line geometry with river attribute data.
-
-            * Required variable for direct bed level burning: ['zb']
-            * Required variable for direct river depth burning: ['rivdph'] (only in combination with rivdph_method='geom')
-            * Variables used for river depth estimates: ['qbankfull', 'rivwth']
-
-        river_mask_fn : str, optional
-            River mask raster used to define river cells
-        qbankfull_fn: str, optional
-            Point geometry with bankfull discharge estimates
-
-            * Required variable: ['qbankfull']
-
-        rivdph_method : {'gvf', 'manning', 'powlaw'}
-            River depth estimate method, by default 'gvf'
-        rivwth_method : {'geom', 'mask'}
-            Derive the river with from either the `river_geom_fn` (geom) or
-            `river_mask_fn` (mask; default) data.
-        river_upa : float, optional
-            Minimum upstream area threshold for rivers [km2], by default 25.0
-        river_len: float, optional
-            Mimimum river length within the model domain threshhold [m], by default 1000 m.
-        min_rivwth, min_rivdph: float, optional
-            Minimum river width [m] (by default 50.0) and depth [m] (by default 1.0)
-        rivbank: bool, optional
-            If True (default), approximate the reference elevation for the river depth based
-            on the river bankfull elevation at cells neighboring river cells. Otherwise
-            use the elevation of the local river cell as reference level.
-        rivbankq : float, optional
-            quantile [1-100] for river bank estimation, by default 25
-        segment_length : float, optional
-            Approximate river segment length [m], by default 5e3
-        smooth_length : float, optional
-            Approximate smoothing length [m], by default 10e3
-        constrain_estuary : bool, optional
-            If True (default) fix the river depth in estuaries based on the upstream river depth.
-        constrain_rivbed : bool, optional
-            If True (default) correct the river bed level to be hydrologically correct,
-            i.e. sloping downward in downstream direction.
-        dig_river_d4: bool, optional
-            If True (default), dig the river out to be hydrologically connected in D4.
-        """
-        if river_mask_fn is None and rivwth_method == "mask":
-            raise ValueError(
-                '"river_mask_fn" should be provided if rivwth_method="mask".'
-            )
-        # get basemap river flwdir
-        self.mask  # make sure msk is staticmaps
-        ds = self.staticmaps
-        flwdir = None
-        if "flwdir" in ds:
-            flwdir = hydromt.flw.flwdir_from_da(ds["flwdir"], mask=False)
-
-        # read river line geometry data
-        gdf_riv = None
-        if river_geom_fn is not None:
-            gdf_riv = self.data_catalog.get_geodataframe(
-                river_geom_fn, geom=self.region
-            ).to_crs(self.crs)
-        # read river bankfull point data
-        gdf_qbf = None
-        if qbankfull_fn is not None:
-            gdf_qbf = self.data_catalog.get_geodataframe(
-                qbankfull_fn,
-                geom=self.region,
-            ).to_crs(self.crs)
-        # read river mask raster data
-        da_rivmask = None
-        if river_mask_fn is not None:
-            da_rivmask = self.data_catalog.get_rasterdataset(
-                river_mask_fn, geom=self.region
-            ).raster.reproject_like(ds, "max")
-            ds["rivmsk"] = da_rivmask.where(self.mask != 0, 0) != 0
-        elif "rivmsk" in ds:
-            self.logger.info(
-                'River mask based on internal "rivmsk" layer. If this is unwanted '
-                "delete the gis/rivmsk.tif file or drop the rivmsk staticmaps variable."
-            )
-
-        # estimate elevation bed level based on qbankfull (and other parameters)
-        if not (gdf_riv is not None and "zb" in gdf_riv):
-            if flwdir is None:
-                msg = '"flwdir" staticmap layer missing, run "setup_river_hydrography".'
-                raise ValueError(msg)
-            gdf_riv, ds["rivmsk"] = workflows.get_river_bathymetry(
-                ds,
-                flwdir=flwdir,
-                gdf_riv=gdf_riv,
-                gdf_qbf=gdf_qbf,
-                rivdph_method=rivdph_method,
-                rivwth_method=rivwth_method,
-                river_upa=river_upa,
-                river_len=river_len,
-                min_rivdph=min_rivdph,
-                min_rivwth=min_rivwth,
-                rivbank=rivbank,
-                rivbankq=rivbankq,
-                segment_length=segment_length,
-                smooth_length=smooth_length,
-                elevtn_name=self._MAPS["elevtn"],
-                constrain_estuary=constrain_estuary,
-                constrain_rivbed=constrain_rivbed,
+            highres_dir = None
+
+        if self.grid_type == "regular":
+            self.reggrid.subgrid.build(
+                da_mask=self.mask,
+                datasets_dep=datasets_dep,
+                datasets_rgh=datasets_rgh,
+                buffer_cells=buffer_cells,
+                nbins=nbins,
+                nr_subgrid_pixels=nr_subgrid_pixels,
+                nrmax=nrmax,
+                max_gradient=max_gradient,
+                z_minimum=z_minimum,
+                manning_land=manning_land,
+                manning_sea=manning_sea,
+                rgh_lev_land=rgh_lev_land,
+                write_dep_tif=write_dep_tif,
+                write_man_tif=write_man_tif,
+                highres_dir=highres_dir,
                 logger=self.logger,
-                **kwargs,
             )
-        elif "rivmsk" not in ds:
-            buffer = gdf_riv["rivwth"].values if "rivwth" in gdf_riv else 0
-            gdf_riv_buf = gdf_riv.buffer(buffer)
-            ds["rivmsk"] = ds.raster.geometry_mask(gdf_riv_buf, all_touched=True)
-
-        # set elevation bed level
-        da_elv1, ds["rivmsk"] = workflows.burn_river_zb(
-            gdf_riv=gdf_riv,
-            da_elv=ds[self._MAPS["elevtn"]],
-            da_msk=ds["rivmsk"],
-            flwdir=flwdir,
-            river_d4=dig_river_d4,
-            logger=self.logger,
-        )
+            self.subgrid = self.reggrid.subgrid.to_xarray(
+                dims=self.mask.raster.dims, coords=self.mask.raster.coords
+            )
+        elif self.grid_type == "quadtree":
+            pass
 
-        if plot_riv_profiles > 0:
-            # TODO move to plots
-            import matplotlib.pyplot as plt
-
-            flw = pyflwdir.from_dataframe(gdf_riv.set_index("idx"))
-            upa_pit = gdf_riv.loc[flw.idxs_pit, "uparea"]
-            n = int(plot_riv_profiles)
-            idxs = flw.idxs_pit[np.argsort(upa_pit).values[::-1]][:n]
-            paths, _ = flw.path(idxs=idxs, direction="up")
-            _, axes = plt.subplots(n, 1, figsize=(7, n * 4))
-            for path, ax in zip(paths, axes):
-                g0 = gdf_riv.loc[path, :]
-                x = g0["rivdst"].values
-                ax.plot(x, g0["zs"], "--k", label="bankfull")
-                ax.plot(x, g0["elevtn"], ":k", label="original zb")
-                ax.plot(x, g0["zb"], "--g", label=f"{rivdph_method} zb (corrected)")
-                mask = da_elv1.raster.geometry_mask(g0).values
-                x1 = flwdir.distnc[mask]
-                y1 = da_elv1.data[mask]
-                s1 = np.argsort(x1)
-                ax.plot(x1[s1], y1[s1], ".b", ms=2, label="zb (burned)")
-            ax.legend()
-            if not os.path.isdir(join(self.root, "figs")):
-                os.makedirs(join(self.root, "figs"))
-            fn_fig = join(self.root, "figs", "river_bathymetry.png")
-            plt.savefig(fn_fig, dpi=225, bbox_inches="tight")
-
-        # update dep
-        self.set_staticmaps(da_elv1.round(2), name=self._MAPS["elevtn"])
-        # keep river geom and rivmsk for postprocessing
-        self.set_staticgeoms(gdf_riv, name="rivers")
-        # save rivmask as int8 map (geotif does not support bool maps)
-        da_rivmask = ds["rivmsk"].astype(np.int8).where(ds[self._MAPS["mask"]] > 0, 255)
-        da_rivmask.raster.set_nodata(255)
-        self.set_staticmaps(da_rivmask, name="rivmsk")
+        if "sbgfile" not in self.config:  # only add sbgfile if not already present
+            self.config.update({"sbgfile": "sfincs.sbg"})
+        # subgrid is used so no depfile or manningfile needed
+        if "depfile" in self.config:
+            self.config.pop("depfile")  # remove depfile from config
+        if "manningfile" in self.config:
+            self.config.pop("manningfile")  # remove manningfile from config
 
     def setup_river_inflow(
         self,
-        hydrography_fn=None,
-        river_upa=25.0,
-        river_len=1e3,
-        river_width=2e3,
-        keep_rivers_geom=False,
-        buffer=10,
-        **kwargs,  # catch deprecated args
+        rivers: Union[str, Path, gpd.GeoDataFrame] = None,
+        hydrography: Union[str, Path, xr.Dataset] = None,
+        river_upa: float = 10.0,
+        river_len: float = 1e3,
+        river_width: float = 500,
+        merge: bool = False,
+        first_index: int = 1,
+        keep_rivers_geom: bool = False,
     ):
-        """Setup river inflow (source) points where a river enters the model domain.
+        """Setup discharge (src) points where a river enters the model domain.
+
+        If `rivers` is not provided, river centerlines are extracted from the
+        `hydrography` dataset based on the `river_upa` threshold.
+
+        Waterlevel or outflow boundary cells intersecting with the river
+        are removed from the model mask.
 
-        NOTE: this method requires the either `hydrography_fn` or `setup_river_hydrography` to be run first.
-        NOTE: best to run after `setup_mask`
+        Discharge is set to zero at these points, but can be updated
+        using the `setup_discharge_forcing` or `setup_discharge_forcing_from_grid` methods.
+
+        Note: this method assumes the rivers are directed from up- to downstream.
 
         Adds model layers:
 
-        * **src** geoms: discharge boundary point locations
-        * **dis** forcing: dummy discharge timeseries
+        * **dis** forcing: discharge forcing
         * **mask** map: SFINCS mask layer (only if `river_width` > 0)
-        * **rivers_in** geoms: river centerline (if `keep_rivers_geom`; not used by SFINCS)
+        * **rivers_inflow** geoms: river centerline (if `keep_rivers_geom`; not used by SFINCS)
 
         Parameters
         ----------
-        hydrography_fn: str, Path, optional
-            Path or data source name for hydrography raster data, by default 'merit_hydro'.
+        rivers : str, Path, gpd.GeoDataFrame, optional
+            Path, data source name, or geopandas object for river centerline data.
+            If present, the 'uparea' and 'rivlen' attributes are used.
+        hydrography: str, Path, xr.Dataset optional
+            Path, data source name, or a xarray raster object for hydrography data.
 
             * Required layers: ['uparea', 'flwdir'].
         river_upa : float, optional
-            Minimum upstream area threshold for rivers [km2], by default 25.0
+            Minimum upstream area threshold for rivers [km2], by default 10.0
         river_len: float, optional
             Mimimum river length within the model domain threshhold [m], by default 1 km.
         river_width: float, optional
             Estimated constant width [m] of the inflowing river. Boundary cells within
             half the width are forced to be closed (mask = 1) to avoid instabilities with
-            nearby open or waterlevel boundary cells, by default 1 km.
+            nearby open or waterlevel boundary cells, by default 500 m.
+        merge: bool, optional
+            If True, merge rivers source points with existing points, by default False.
+        first_index: int, optional
+            First index for the river source points, by default 1.
         keep_rivers_geom: bool, optional
-            If True, keep a geometry of the rivers "rivers_in" in staticgeoms. By default False.
+            If True, keep a geometry of the rivers "rivers_inflow" in geoms. By default False.
         buffer: int, optional
             Buffer [no. of cells] around model domain, by default 10.
-        """
-        if "basemaps_fn" in kwargs:
-            self.logger.warning(
-                "'basemaps_fn' is deprecated use 'hydrography_fn' instead."
-            )
-            hydrography_fn = kwargs.pop("basemaps_fn")
 
-        if hydrography_fn is not None:
+        See Also
+        --------
+        setup_discharge_forcing
+        setup_discharge_forcing_from_grid
+        """
+        da_flwdir, da_uparea, gdf_riv = None, None, None
+        if hydrography is not None:
             ds = self.data_catalog.get_rasterdataset(
-                hydrography_fn,
+                hydrography,
                 geom=self.region,
                 variables=["uparea", "flwdir"],
-                buffer=buffer,
+                buffer=5,
             )
+            da_flwdir = ds["flwdir"]
+            da_uparea = ds["uparea"]
+        elif rivers == "rivers_outflow" and rivers in self.geoms:
+            # reuse rivers from setup_river_in/outflow
+            gdf_riv = self.geoms[rivers]
+        elif rivers is not None:
+            gdf_riv = self.data_catalog.get_geodataframe(
+                rivers, geom=self.region
+            ).to_crs(self.crs)
         else:
-            ds = self.staticmaps
-            if "uparea" not in ds or "flwdir" not in ds:
-                raise ValueError(
-                    '"uparea" and/or "flwdir" layers missing. '
-                    "Run setup_river_hydrography first or provide hydrography_fn dataset."
-                )
+            raise ValueError("Either hydrography or rivers must be provided.")
 
-        # (re)calculate region to make sure it's accurate
-        region = self.mask.where(self.mask <= 1, 1).raster.vectorize()
         gdf_src, gdf_riv = workflows.river_boundary_points(
-            da_flwdir=ds["flwdir"],
-            da_uparea=ds["uparea"],
-            region=region,
+            region=self.region,
+            res=self.reggrid.dx,
+            gdf_riv=gdf_riv,
+            da_flwdir=da_flwdir,
+            da_uparea=da_uparea,
             river_len=river_len,
             river_upa=river_upa,
-            btype="inflow",
-            return_river=keep_rivers_geom,
-            logger=self.logger,
+            inflow=True,
         )
-        if len(gdf_src.index) == 0:
+        n = len(gdf_src.index)
+        self.logger.info(f"Found {n} river inflow points.")
+        if n == 0:
             return
 
-        # set forcing with dummy timeseries to keep valid sfincs model
-        gdf_src = gdf_src.to_crs(self.crs.to_epsg())
-        self.set_forcing_1d(xy=gdf_src, name="discharge")
+        # set forcing src pnts
+        gdf_src.index = gdf_src.index + first_index
+        self.set_forcing_1d(gdf_locs=gdf_src.copy(), name="dis", merge=merge)
+
         # set river
-        if keep_rivers_geom and gdf_riv is not None:
-            gdf_riv = gdf_riv.to_crs(self.crs.to_epsg())
-            gdf_riv.index = gdf_riv.index.values + 1  # one based index
-            self.set_staticgeoms(gdf_riv, name="rivers_in")
+        if keep_rivers_geom:
+            self.set_geoms(gdf_riv, name="rivers_inflow")
 
-        # update mask if closed_bounds_buffer > 0
-        if river_width > 0:
+        # update mask if river_width > 0
+        if "rivwth" in gdf_src.columns:
+            river_width = gdf_src["rivwth"].fillna(river_width)
+        if np.any(river_width > 0) and np.any(self.mask > 1):
             # apply buffer
-            gdf_src_buf = gpd.GeoDataFrame(
-                geometry=gdf_src.buffer(river_width / 2), crs=gdf_src.crs
-            )
+            gdf_src["geometry"] = gdf_src.buffer(river_width / 2)
             # find intersect of buffer and model grid
-            bounds = utils.mask_bounds(self.mask, gdf_mask=gdf_src_buf)
+            tmp_msk = self.reggrid.create_mask_bounds(
+                xr.where(self.mask > 0, 1, 0).astype(np.uint8), gdf_include=gdf_src
+            )
+            reset_msk = np.logical_and(tmp_msk > 1, self.mask > 1)
             # update model mask
-            n = np.count_nonzero(bounds.values)
+            n = int(np.sum(reset_msk))
             if n > 0:
-                da_mask = self.mask.where(~bounds, np.uint8(1))
-                self.set_staticmaps(da_mask, self._MAPS["mask"])
-                self.logger.debug(
-                    f"{n:d} closed (mask=1) boundary cells set around src points."
-                )
+                da_mask = self.mask.where(~reset_msk, np.uint8(1))
+                self.set_grid(da_mask, "msk")
+                self.logger.info(f"Boundary cells (n={n}) updated around src points.")
 
     def setup_river_outflow(
         self,
-        hydrography_fn=None,
-        river_upa=25.0,
-        river_len=1e3,
-        river_width=2e3,
-        append_bounds=False,
-        keep_rivers_geom=False,
-        **kwargs,  # catch deprecated arguments
+        rivers: Union[str, Path, gpd.GeoDataFrame] = None,
+        hydrography: Union[str, Path, xr.Dataset] = None,
+        river_upa: float = 10.0,
+        river_len: float = 1e3,
+        river_width: float = 500,
+        keep_rivers_geom: bool = False,
+        reset_bounds: bool = False,
+        btype: str = "outflow",
     ):
-        """Setup open boundary cells (mask=3) where a river flows out of the model domain.
+        """Setup open boundary cells (mask=3) where a river flows
+        out of the model domain.
+
+        If `rivers` is not provided, river centerlines are extracted from the
+        `hydrography` dataset based on the `river_upa` threshold.
 
-        Outflow locations are based on a minimal upstream area threshold. Locations within
-        half `river_width` of a discharge source point or waterlevel boundary cells are omitted.
+        River outflows that intersect with discharge source point or waterlevel
+        boundary cells are omitted.
 
-        NOTE: this method requires the either `hydrography_fn` input or `setup_river_hydrography` to be run first.
-        NOTE: best to run after `setup_mask`, `setup_bounds` and `setup_river_inflow`
+        Note: this method assumes the rivers are directed from up- to downstream.
 
         Adds / edits model layers:
 
         * **msk** map: edited by adding outflow points (msk=3)
-        * **river_out** geoms: river centerline (if `keep_rivers_geom`; not used by SFINCS)
+        * **rivers_outflow** geoms: river centerline (if `keep_rivers_geom`; not used by SFINCS)
 
         Parameters
         ----------
-        hydrography_fn: str, Path, optional
-            Path or data source name for hydrography raster data, by default 'merit_hydro'.
+        rivers : str, Path, gpd.GeoDataFrame, optional
+            Path, data source name, or geopandas object for river centerline data.
+            If present, the 'uparea' and 'rivlen' attributes are used.
+        hydrography: str, Path, xr.Dataset optional
+            Path, data source name, or a xarray raster object for hydrography data.
+
             * Required layers: ['uparea', 'flwdir'].
-        river_width: int, optional
-            The width [m] of the open boundary cells in the SFINCS msk file.
-            By default 2km, i.e.: 1km to each side of the outflow location.
         river_upa : float, optional
-            Minimum upstream area threshold for rivers [km2], by default 25.0
+            Minimum upstream area threshold for rivers [km2], by default 10.0
         river_len: float, optional
             Mimimum river length within the model domain threshhold [m], by default 1000 m.
+        river_width: int, optional
+            The width [m] of the open boundary cells in the SFINCS msk file.
+            By default 500m, i.e.: 250m to each side of the outflow location.
         append_bounds: bool, optional
             If True, write new outflow boundary cells on top of existing. If False (default),
             first reset existing outflow boundary cells to normal active cells.
         keep_rivers_geom: bool, optional
-            If True, keep a geometry of the rivers "rivers_out" in staticgeoms. By default False.
-        """
-        if "outflow_width" in kwargs:
-            self.logger.warning(
-                "'outflow_width' is deprecated use 'river_width' instead."
-            )
-            river_width = kwargs.pop("outflow_width")
-        if "basemaps_fn" in kwargs:
-            self.logger.warning(
-                "'basemaps_fn' is deprecated use 'hydrography_fn' instead."
-            )
-            hydrography_fn = kwargs.pop("basemaps_fn")
+            If True, keep a geometry of the rivers "rivers_outflow" in geoms. By default False.
+        reset_bounds: bool, optional
+            If True, reset existing outlfow boundary cells before setting new boundary cells,
+            by default False.
+        btype: {'waterlevel', 'outflow'}
+            Boundary type
 
-        if hydrography_fn is not None:
+        See Also
+        --------
+        setup_mask_bounds
+        """
+        da_flwdir, da_uparea, gdf_riv = None, None, None
+        if hydrography is not None:
             ds = self.data_catalog.get_rasterdataset(
-                hydrography_fn,
+                hydrography,
                 geom=self.region,
                 variables=["uparea", "flwdir"],
-                buffer=10,
+                buffer=5,
             )
+            da_flwdir = ds["flwdir"]
+            da_uparea = ds["uparea"]
+        elif rivers == "rivers_inflow" and rivers in self.geoms:
+            # reuse rivers from setup_river_in/outflow
+            gdf_riv = self.geoms[rivers]
+        elif rivers is not None:
+            gdf_riv = self.data_catalog.get_geodataframe(
+                rivers, geom=self.region
+            ).to_crs(self.crs)
         else:
-            ds = self.staticmaps
-            if "uparea" not in ds or "flwdir" not in ds:
-                raise ValueError(
-                    '"uparea" and/or "flwdir" layers missing. '
-                    "Run setup_river_hydrography first or provide hydrography_fn dataset."
-                )
+            raise ValueError("Either hydrography or rivers must be provided.")
 
-        # (re)calculate region to make sure it's accurate
-        region = self.mask.where(self.mask <= 1, 1).raster.vectorize()
+        # TODO reproject region and gdf_riv to utm zone if model crs is geographic
         gdf_out, gdf_riv = workflows.river_boundary_points(
-            da_flwdir=ds["flwdir"],
-            da_uparea=ds["uparea"],
-            region=region,
+            region=self.region,
+            res=self.reggrid.dx,
+            gdf_riv=gdf_riv,
+            da_flwdir=da_flwdir,
+            da_uparea=da_uparea,
             river_len=river_len,
             river_upa=river_upa,
-            btype="outflow",
-            return_river=keep_rivers_geom,
-            logger=self.logger,
+            inflow=False,
         )
-        if len(gdf_out.index) == 0:
-            return
 
-        # apply buffer
-        gdf_out = gdf_out.to_crs(self.crs.to_epsg())  # assumes projected CRS
-        gdf_out_buf = gpd.GeoDataFrame(
-            geometry=gdf_out.buffer(river_width / 2.0), crs=gdf_out.crs
-        )
-        # remove points near waterlevel boundary cells
-        da_mask = self.mask
-        msk2 = (da_mask == 2).astype(np.int8)
-        msk_wdw = msk2.raster.zonal_stats(gdf_out_buf, stats="max")
-        bool_drop = (msk_wdw[f"{da_mask.name}_max"] == 1).values
-        if np.any(bool_drop):
-            self.logger.debug(
-                f"{int(sum(bool_drop)):d} outflow (mask=3) boundary cells near water level (mask=2) boundary cells dropped."
-            )
-            gdf_out = gdf_out[~bool_drop]
-        if len(gdf_out.index) == 0:
-            self.logger.debug(f"0 outflow (mask=3) boundary cells set.")
-            return
-        # remove outflow points near source points
-        fname = self._FORCING["discharge"][0]
-        if fname in self.forcing:
-            gdf_src = self.forcing[fname].vector.to_gdf()
-            idx_drop = gpd.sjoin(gdf_out_buf, gdf_src, how="inner").index.values
-            if idx_drop.size > 0:
-                gdf_out_buf = gdf_out_buf.drop(idx_drop)
-                self.logger.debug(
-                    f"{idx_drop.size:d} outflow (mask=3) boundary cells near src points dropped."
-                )
-
-        # find intersect of buffer and model grid
-        bounds = utils.mask_bounds(da_mask, gdf_mask=gdf_out_buf)
-        # update model mask
-        if not append_bounds:  # reset existing outflow boundary cells
-            da_mask = da_mask.where(da_mask != 3, np.uint8(1))
-        bounds = np.logical_and(bounds, da_mask == 1)  # make sure not to overwrite
-        n = np.count_nonzero(bounds.values)
+        if len(gdf_out) > 0:
+            if "rivwth" in gdf_out.columns:
+                river_width = gdf_out["rivwth"].fillna(river_width)
+            gdf_out["geometry"] = gdf_out.buffer(river_width / 2)
+            # remove points near waterlevel boundary cells
+            if np.any(self.mask == 2) and btype == "outflow":
+                gdf_msk2 = utils.get_bounds_vector(self.mask)
+                # NOTE: this should be a single geom
+                geom = gdf_msk2[gdf_msk2["value"] == 2].unary_union
+                gdf_out = gdf_out[~gdf_out.intersects(geom)]
+            # remove outflow points near source points
+            if "dis" in self.forcing and len(gdf_out) > 0:
+                geom = self.forcing["dis"].vector.to_gdf().unary_union
+                gdf_out = gdf_out[~gdf_out.intersects(geom)]
+
+        # update mask
+        n = len(gdf_out.index)
+        self.logger.info(f"Found {n} valid river outflow points.")
         if n > 0:
-            da_mask = da_mask.where(~bounds, np.uint8(3))
-            self.set_staticmaps(da_mask, self._MAPS["mask"])
-            self.logger.debug(f"{n:d} outflow (mask=3) boundary cells set.")
-        if keep_rivers_geom and gdf_riv is not None:
-            gdf_riv = gdf_riv.to_crs(self.crs.to_epsg())
-            gdf_riv.index = gdf_riv.index.values + 1  # one based index
-            self.set_staticgeoms(gdf_riv, name="rivers_out")
+            self.setup_mask_bounds(
+                btype=btype, include_mask=gdf_out, reset_bounds=reset_bounds
+            )
+        elif reset_bounds:
+            self.setup_mask_bounds(btype=btype, reset_bounds=reset_bounds)
 
-    def setup_cn_infiltration(self, cn_fn="gcn250", antecedent_runoff_conditions="avg"):
+        # keep river centerlines
+        if keep_rivers_geom and len(gdf_riv) > 0:
+            self.set_geoms(gdf_riv, name="rivers_outflow")
+
+    def setup_constant_infiltration(self, qinf, reproj_method="average"):
+        """Setup spatially varying constant infiltration rate (qinffile).
+
+        Adds model layers:
+
+        * **qinf** map: constant infiltration rate [mm/hr]
+
+        Parameters
+        ----------
+        qinf : str, Path, or RasterDataset
+            Spatially varying infiltration rates [mm/hr]
+        reproj_method : str, optional
+            Resampling method for reprojecting the infiltration data to the model grid.
+            By default 'average'. For more information see, :py:meth:`hydromt.raster.RasterDataArray.reproject_like`
+        """
+
+        # get infiltration data
+        da_inf = self.data_catalog.get_rasterdataset(qinf, geom=self.region, buffer=10)
+        da_inf = da_inf.raster.mask_nodata()  # set nodata to nan
+
+        # reproject infiltration data to model grid
+        da_inf = da_inf.raster.reproject_like(self.mask, method=reproj_method)
+
+        # check on nan values
+        if np.logical_and(np.isnan(da_inf), self.mask >= 1).any():
+            self.logger.warning("NaN values found in infiltration data; filled with 0")
+            da_inf = da_inf.fillna(0)
+        da_inf.raster.set_nodata(-9999.0)
+
+        # set grid
+        mname = "qinf"
+        da_inf.attrs.update(**self._ATTRS.get(mname, {}))
+        self.set_grid(da_inf, name=mname)
+
+        # update config: remove default inf and set qinf map
+        self.set_config(f"{mname}file", f"sfincs.{mname}")
+        self.config.pop("qinf", None)
+
+    def setup_cn_infiltration(self, cn, antecedent_moisture="avg", reproj_method="med"):
         """Setup model potential maximum soil moisture retention map (scsfile)
         from gridded curve number map.
 
         Adds model layers:
 
         * **scs** map: potential maximum soil moisture retention [inch]
 
         Parameters
         ---------
-        cn_fn: str, optional
+        cn: str, Path, or RasterDataset
             Name of gridded curve number map.
 
             * Required layers without antecedent runoff conditions: ['cn']
             * Required layers with antecedent runoff conditions: ['cn_dry', 'cn_avg', 'cn_wet']
-        antecedent_runoff_conditions: {'dry', 'avg', 'wet'}, optional
+        antecedent_moisture: {'dry', 'avg', 'wet'}, optional
             Antecedent runoff conditions.
             None if data has no antecedent runoff conditions.
             By default `avg`
+        reproj_method : str, optional
+            Resampling method for reprojecting the curve number data to the model grid.
+            By default 'med'. For more information see, :py:meth:`hydromt.raster.RasterDataArray.reproject_like`
         """
         # get data
+        da_org = self.data_catalog.get_rasterdataset(cn, geom=self.region, buffer=10)
+        # read variable
         v = "cn"
-        if antecedent_runoff_conditions:
-            v = f"cn_{antecedent_runoff_conditions}"
-        da_org = self.data_catalog.get_rasterdataset(
-            cn_fn, geom=self.region, buffer=10, variables=[v]
-        )
+        if antecedent_moisture:
+            v = f"cn_{antecedent_moisture}"
+        if isinstance(da_org, xr.Dataset) and v in da_org.data_vars:
+            da_org = da_org[v]
+        elif not isinstance(da_org, xr.DataArray):
+            raise ValueError(f"Could not find variable {v} in {cn}")
+
         # reproject using median
-        da_cn = da_org.raster.reproject_like(self.staticmaps, method="med")
-        # CN=100 based on water mask
-        if "rivmsk" in self.staticmaps:
-            self.logger.info(
-                'Updating CN map based on "rivmsk" from setup_river_hydrography method.'
-            )
-            da_cn = da_cn.where(self.staticmaps["rivmsk"] == 0, 100)
+        da_cn = da_org.raster.reproject_like(self.grid, method=reproj_method)
+
         # convert to potential maximum soil moisture retention S (1000/CN - 10) [inch]
         da_scs = workflows.cn_to_s(da_cn, self.mask > 0).round(3)
-        # set staticmaps
-        mname = self._MAPS["curve_number"]
+
+        # set grid
+        mname = "scs"
         da_scs.attrs.update(**self._ATTRS.get(mname, {}))
-        self.set_staticmaps(da_scs, name=mname)
+        self.set_grid(da_scs, name=mname)
         # update config: remove default infiltration values and set scs map
         self.config.pop("qinf", None)
         self.set_config(f"{mname}file", f"sfincs.{mname}")
 
     def setup_manning_roughness(
         self,
-        lulc_fn=None,
-        map_fn=None,
-        riv_man=0.03,
-        lnd_man=0.1,
-        sea_man=None,
+        datasets_rgh: List[dict] = [],
+        manning_land=0.04,
+        manning_sea=0.02,
+        rgh_lev_land=0,
     ):
-        """Setup model manning roughness map (manningfile) from gridded
+        """Setup model manning roughness map (manningfile) from gridded manning data or a combinataion of gridded
         land-use/land-cover map and manning roughness mapping table.
 
         Adds model layers:
 
         * **man** map: manning roughness coefficient [s.m-1/3]
 
         Parameters
         ---------
-        lulc_fn: str, optional
-            Name of landuse-landcover map.
+        datasets_rgh : List[dict], optional
+            List of dictionaries with Manning's n datasets. Each dictionary should at least contain one of the following:
+            * (1) manning: filename (or Path) of gridded data with manning values
+            * (2) lulc (and reclass_table) :a combination of a filename of gridded landuse/landcover and a mapping table.
+            In additon, optional merge arguments can be provided e.g.: merge_method, gdf_valid_fn
+        manning_land, manning_sea : float, optional
+            Constant manning roughness values for land and sea, by default 0.04 and 0.02 s.m-1/3
+            Note that these values are only used when no Manning's n datasets are provided, or to fill the nodata values
+        rgh_lev_land : float, optional
+            Elevation level to distinguish land and sea roughness (when using manning_land and manning_sea), by default 0.0
+        """
 
-            * Required layers: ['lulc']
-        map_fn: path-like, optional
-            CSV mapping file with lulc classes in the index column and manning values
-            in another column with 'N' as header.
-        lnd_man, riv_man, sea_man: float, optional
-            Constant manning roughness values for land (by default 0.1 s.m-1/3)
-            river (by default 0.03 s.m-1/3) and sea (by default None and skipped).
-            River cells are based on the river mask ('rivmsk') staticmaps layer
-            from the `setup_river_hydrography` component. Sea cells are based on elevation
-            values smaller than zero.
-            Manning roughness for land cells are superseeded by the landuse-landcover
-            map based values if `lulc_fn` is not None.
-        """
-        da_msk = self.mask > 0
-        da_man = xr.full_like(da_msk, lnd_man, dtype=np.float32)
-        da_man.raster.set_nodata(-9999.0)
-        if lulc_fn is not None:
-            if map_fn is None:
-                map_fn = join(DATADIR, "lulc", f"{lulc_fn}_mapping.csv")
-            if not os.path.isfile(map_fn):
-                raise IOError(f"Manning roughness mapping file not found: {map_fn}")
-            da_org = self.data_catalog.get_rasterdataset(
-                lulc_fn, geom=self.region, buffer=10, variables=["lulc"]
-            )
-            # reproject and reclassify
-            # TODO use generic names for parameters
-            # FIXME use hydromt general version!!
-            da_man = workflows.landuse(
-                da_org, da_msk, map_fn, logger=self.logger, params=["N"]
-            )["N"]
-        if "rivmsk" in self.staticmaps and riv_man is not None:
-            self.logger.info("Setting constant manning roughness for river cells.")
-            da_man = da_man.where(self.staticmaps["rivmsk"] != 1, riv_man)
-        elif lulc_fn is None:
-            self.logger.warning(
-                'Skipping spatial variable manning roughness map as no river mask ("rivmsk" staticmaps layer)'
-                ' or landuse-landcover map ("lulc_fn" argument) was provided. Set constant manning roughness'
-                ' using the "manning", "manning_land" and/or "manning_sea" parameters in the sfincs.inp file.'
-            )
-            return
-        if sea_man is not None:
-            self.logger.info("Setting constant manning roughness for sea cells.")
-            da_man = da_man.where(self.staticmaps[self._MAPS["elevtn"]] >= 0, sea_man)
-        # mask and set precision
-        da_man = da_man.where(da_msk, da_man.raster.nodata).round(3)
-        # set staticmaps
-        mname = self._MAPS["manning"]
-        da_man.attrs.update(**self._ATTRS.get(mname, {}))
-        self.set_staticmaps(da_man, name=mname)
-        # update config: remove default manning values and set maning map
-        for v in ["manning_land", "manning_sea", "rgh_lev_land"]:
-            self.config.pop(v, None)
-        self.set_config(f"{mname}file", f"sfincs.{mname[:3]}")
+        if len(datasets_rgh) > 0:
+            datasets_rgh = self._parse_datasets_rgh(datasets_rgh)
+        else:
+            datasets_rgh = []
+
+        # fromdep keeps track of whether any manning values should be based on the depth or not
+        fromdep = len(datasets_rgh) == 0
+        if self.grid_type == "regular":
+            if len(datasets_rgh) > 0:
+                da_man = workflows.merge_multi_dataarrays(
+                    da_list=datasets_rgh,
+                    da_like=self.mask,
+                    interp_method="linear",
+                    logger=self.logger,
+                )
+                fromdep = np.isnan(da_man).where(self.mask > 0, False).any()
+            if "dep" in self.grid and fromdep:
+                da_man0 = xr.where(
+                    self.grid["dep"] >= rgh_lev_land, manning_land, manning_sea
+                )
+            elif fromdep:
+                da_man0 = xr.full_like(self.mask, manning_land, dtype=np.float32)
 
-    def setup_gauges(self, gauges_fn, overwrite=False, **kwargs):
+            if len(datasets_rgh) > 0 and fromdep:
+                self.logger.warning("nan values in manning roughness array")
+                da_man = da_man.where(~np.isnan(da_man), da_man0)
+            elif fromdep:
+                da_man = da_man0
+            da_man.raster.set_nodata(-9999.0)
+
+            # set grid
+            mname = "manning"
+            da_man.attrs.update(**self._ATTRS.get(mname, {}))
+            self.set_grid(da_man, name=mname)
+            # update config: remove default manning values and set maning map
+            for v in ["manning_land", "manning_sea", "rgh_lev_land"]:
+                self.config.pop(v, None)
+            self.set_config(f"{mname}file", f"sfincs.{mname[:3]}")
+
+    def setup_observation_points(
+        self,
+        locations: Union[str, Path, gpd.GeoDataFrame],
+        merge: bool = True,
+        **kwargs,
+    ):
         """Setup model observation point locations.
 
         Adds model layers:
 
         * **obs** geom: observation point locations
 
         Parameters
         ---------
-        gauges_fn: str
-            Path to observation points geometry file.
-            See :py:meth:`hydromt.open_vector`, for accepted files.
-        overwrite: bool, optional
-            If True, overwrite existing gauges instead of appending the new gauges.
+        locations: str, Path, gpd.GeoDataFrame, optional
+            Path, data source name, or geopandas object for observation point locations.
+        merge: bool, optional
+            If True, merge the new observation points with the existing ones. By default True.
         """
-        name = self._GEOMS["gauges"]
-        # ensure the catalog is loaded before adding any new entries
+        name = self._GEOMS["observation_points"]
+
+        # FIXME ensure the catalog is loaded before adding any new entries
         self.data_catalog.sources
-        gdf = self.data_catalog.get_geodataframe(
-            gauges_fn, geom=self.region, assert_gtype="Point", **kwargs
+
+        gdf_obs = self.data_catalog.get_geodataframe(
+            locations, geom=self.region, assert_gtype="Point", **kwargs
         ).to_crs(self.crs)
-        if not overwrite and name in self.staticgeoms:
-            gdf0 = self._staticgeoms.pop(name)
-            gdf = gpd.GeoDataFrame(pd.concat([gdf, gdf0], ignore_index=True))
-            self.logger.info(f"Adding new gauges to existing gauges.")
-        self.set_staticgeoms(gdf, name)
+
+        if not gdf_obs.geometry.type.isin(["Point"]).all():
+            raise ValueError("Observation points must be of type Point.")
+
+        if merge and name in self.geoms:
+            gdf0 = self._geoms.pop(name)
+            gdf_obs = gpd.GeoDataFrame(pd.concat([gdf_obs, gdf0], ignore_index=True))
+            self.logger.info(f"Adding new observation points to existing ones.")
+
+        self.set_geoms(gdf_obs, name)
         self.set_config(f"{name}file", f"sfincs.{name}")
-        self.logger.info(f"{name} set based on {gauges_fn}")
 
     def setup_structures(
-        self, structures_fn, stype, dz=None, overwrite=False, **kwargs
+        self,
+        structures: Union[str, Path, gpd.GeoDataFrame],
+        stype: str,
+        dz: float = None,
+        merge: bool = True,
+        **kwargs,
     ):
         """Setup thin dam or weir structures.
 
         Adds model layer (depending on `stype`):
 
         * **thd** geom: thin dam
         * **weir** geom: weir / levee
 
         Parameters
         ----------
-        structures_fn : str, Path
-            Path to structure line geometry file.
-            The "name" (for thd and weir), "z" and "par1" (for weir only) are optional.
-            For weirs: `dz` must be provided if gdf has no "z" column or Z LineString;
+        structures : str, Path
+            Path, data source name, or geopandas object to structure line geometry file.
+            The "name" (for thd and weir), "z" and "par1" (for weir only) variables are optional.
+            For weirs: `dz` must be provided if gdf has no "z" column or ZLineString;
             "par1" defaults to 0.6 if gdf has no "par1" column.
         stype : {'thd', 'weir'}
             Structure type.
-        overwrite: bool, optional
-            If True, overwrite existing 'stype' structures instead of appending the
-            new structures.
+        merge : bool, optional
+            If True, merge with existing'stype' structures, by default True.
         dz: float, optional
             If provided, for weir structures the z value is calculated from
             the model elevation (dep) plus dz.
         """
+
+        # read, clip and reproject
+        gdf_structures = self.data_catalog.get_geodataframe(
+            structures, geom=self.region, **kwargs
+        ).to_crs(self.crs)
+
         cols = {
             "thd": ["name", "geometry"],
             "weir": ["name", "z", "par1", "geometry"],
         }
         assert stype in cols
-        # read, clip and reproject
-        gdf = self.data_catalog.get_geodataframe(
-            structures_fn, geom=self.region, **kwargs
-        ).to_crs(self.crs)
-        gdf = gdf[[c for c in cols[stype] if c in gdf.columns]]  # keep relevant cols
-        structs = utils.gdf2structures(gdf)  # check if it parsed correct
+        gdf = gdf_structures[
+            [c for c in cols[stype] if c in gdf_structures.columns]
+        ]  # keep relevant cols
+
+        structs = utils.gdf2linestring(gdf)  # check if it parsed correct
         # sample zb values from dep file and set z = zb + dz
         if stype == "weir" and dz is not None:
-            elv = self.staticmaps[self._MAPS["elevtn"]]
+            elv = self.grid["dep"]
             structs_out = []
             for s in structs:
                 pnts = gpd.points_from_xy(x=s["x"], y=s["y"])
                 zb = elv.raster.sample(gpd.GeoDataFrame(geometry=pnts, crs=self.crs))
                 s["z"] = zb.values + float(dz)
                 structs_out.append(s)
-            gdf = utils.structures2gdf(structs_out, crs=self.crs)
+            gdf = utils.linestring2gdf(structs_out, crs=self.crs)
+        # Else function if you define elevation of weir
         elif stype == "weir" and np.any(["z" not in s for s in structs]):
             raise ValueError("Weir structure requires z values.")
         # combine with existing structures if present
-        if not overwrite and stype in self.staticgeoms:
-            gdf0 = self._staticgeoms.pop(stype)
+        if merge and stype in self.geoms:
+            gdf0 = self._geoms.pop(stype)
             gdf = gpd.GeoDataFrame(pd.concat([gdf, gdf0], ignore_index=True))
             self.logger.info(f"Adding {stype} structures to existing structures.")
+
         # set structures
-        self.set_staticgeoms(gdf, stype)
+        self.set_geoms(gdf, stype)
         self.set_config(f"{stype}file", f"sfincs.{stype}")
-        self.logger.info(f"{stype} structure set based on {structures_fn}")
 
     ### FORCING
-    def setup_h_forcing(
+    def set_forcing_1d(
         self,
-        geodataset_fn=None,
-        timeseries_fn=None,
-        offset_fn=None,
-        buffer=5e3,
-        **kwargs,
+        df_ts: pd.DataFrame = None,
+        gdf_locs: gpd.GeoDataFrame = None,
+        name: str = "bzs",
+        merge: bool = True,
     ):
-        """Setup waterlevel boundary point locations (bnd) and time series (bzs).
+        """Set 1D forcing time series for 'bzs' or 'dis' boundary conditions.
 
-        Use `geodataset_fn` to set the waterlevel boundary from a dataset of point location
-        timeseries. The dataset is clipped to the model region plus `buffer` [m], and
-        model time based on the model config tstart and tstop entries.
-
-        Use `timeseries_fn` in combination with `geodataset_fn=None` to set a spatially
-        uniform waterlevel for all waterlevel boundary cells (msk==2),
-
-        If `timeseries_fn` and `geodataset_fn` are both not provided a dummy (h=0) waterlevel
-        boundary is set.
-
-        The vertical reference of the waterlevel data can be corrected to match
-        the vertical reference of the model elevation (dep) layer by adding
-        a local offset value derived from the `offset_fn` map to the waterlevels,
-        e.g. mean dynamic topography for difference between EGM and MSL levels.
+        1D forcing exists of point location `gdf_locs` and associated timeseries `df_ts`.
+        If `gdf_locs` is None, the currently set locations are used.
 
-        Adds model layers:
+        If merge is True, time series in `df_ts` with the same index will
+        overwrite existing data. Time series with new indices are added to
+        the existing forcing.
+
+        In case the forcing time series have a numeric index, the index is converted to
+        a datetime index assuming the index is in seconds since `tref`.
+
+        Parameters
+        ----------
+        df_ts : pd.DataFrame, optional
+            1D forcing time series data. If None, dummy forcing data is added.
+        gdf_locs : gpd.GeoDataFrame, optional
+            Location of waterlevel boundary points. If None, the currently set locations are used.
+        name : str, optional
+            Name of the waterlevel boundary time series file, by default 'bzs'.
+        merge : bool, optional
+            If True, merge with existing forcing data, by default True.
+        """
+        # check dtypes
+        if gdf_locs is not None:
+            if not isinstance(gdf_locs, gpd.GeoDataFrame):
+                raise ValueError("gdf_locs must be a gpd.GeoDataFrame")
+            if not gdf_locs.index.is_integer() and gdf_locs.index.is_unique:
+                raise ValueError("gdf_locs index must be unique integer values")
+            if not gdf_locs.geometry.type.isin(["Point"]).all():
+                raise ValueError("gdf_locs geometry must be Point")
+            if gdf_locs.crs != self.crs:
+                gdf_locs = gdf_locs.to_crs(self.crs)
+        elif name in self.forcing:
+            gdf_locs = self.forcing[name].vector.to_gdf()
+        if df_ts is not None:
+            if not isinstance(df_ts, pd.DataFrame):
+                raise ValueError("df_ts must be a pd.DataFrame")
+            if not df_ts.columns.is_integer() and df_ts.columns.is_unique:
+                raise ValueError("df_ts column names must be unique integer values")
+        # parse datetime index
+        if df_ts is not None and df_ts.index.is_numeric():
+            if "tref" not in self.config:
+                raise ValueError(
+                    "tref must be set in config to convert numeric index to datetime index"
+                )
+            tref = utils.parse_datetime(self.config["tref"])
+            df_ts.index = tref + pd.to_timedelta(df_ts.index, unit="sec")
+        # parse location index
+        if (
+            gdf_locs is not None
+            and df_ts is not None
+            and gdf_locs.index.size == df_ts.columns.size
+            and not set(gdf_locs.index) == set(df_ts.columns)
+        ):
+            # loop over integer columns and find matching index
+            for col in gdf_locs.select_dtypes(include=np.integer).columns:
+                if set(gdf_locs[col]) == set(df_ts.columns):
+                    gdf_locs = gdf_locs.set_index(col)
+                    self.logger.info(f"Setting gdf_locs index to {col}")
+                    break
+            if not (gdf_locs.index) == set(df_ts.columns):
+                gdf_locs = gdf_locs.set_index(df_ts.columns)
+                self.logger.info(
+                    f"No matching index column found in gdf_locs; assuming the order is correct"
+                )
+        # merge with existing data
+        if name in self.forcing and merge:
+            # read existing data
+            da = self.forcing[name]
+            gdf0 = da.vector.to_gdf()
+            df0 = da.transpose(..., da.vector.index_dim).to_pandas()
+            if set(gdf0.index) != set(gdf_locs.index):
+                # merge locations; overwrite existing locations with the same name
+                gdf0 = gdf0.drop(gdf_locs.index, errors="ignore")
+                gdf_locs = pd.concat([gdf0, gdf_locs], axis=0).sort_index()
+                # gdf_locs = gpd.GeoDataFrame(gdf_locs, crs=gdf0.crs)
+                df0 = df0.reindex(gdf_locs.index, axis=1, fill_value=0)
+            if df_ts is None:
+                df_ts = df0
+            elif set(df0.columns) != set(df_ts.columns):
+                # merge timeseries; overwrite existing timeseries with the same name
+                df0 = df0.drop(columns=df_ts.columns, errors="ignore")
+                df_ts = pd.concat([df0, df_ts], axis=1).sort_index()
+                # use linear interpolation and backfill to fill in missing values
+                df_ts = df_ts.sort_index()
+                df_ts = df_ts.interpolate(method="linear").bfill().fillna(0)
+        # location data is required
+        if gdf_locs is None:
+            raise ValueError(
+                f"gdf_locs must be provided if not merged with existing {name} forcing data"
+            )
+        # fill in missing timeseries
+        if df_ts is None:
+            df_ts = pd.DataFrame(
+                index=pd.date_range(*self.get_model_time(), periods=2),
+                data=0,
+                columns=gdf_locs.index,
+            )
+        # set forcing with consistent names
+        if not set(gdf_locs.index) == set(df_ts.columns):
+            raise ValueError("The gdf_locs index and df_ts columns must be the same")
+        gdf_locs.index.name = "index"
+        df_ts.columns.name = "index"
+        df_ts.index.name = "time"
+        da = GeoDataArray.from_gdf(gdf_locs.to_crs(self.crs), data=df_ts, name=name)
+        self.set_forcing(da.transpose("time", "index"))
+
+    def setup_waterlevel_forcing(
+        self,
+        geodataset: Union[str, Path, xr.Dataset] = None,
+        timeseries: Union[str, Path, pd.DataFrame] = None,
+        locations: Union[str, Path, gpd.GeoDataFrame] = None,
+        offset: Union[str, Path, xr.Dataset] = None,
+        buffer: float = 5e3,
+        merge: bool = True,
+    ):
+        """Setup waterlevel forcing.
+
+        Waterlevel boundary conditions are read from a `geodataset` (geospatial point timeseries)
+        or a tabular `timeseries` dataframe. At least one of these must be provided.
+
+        The tabular timeseries data is combined with `locations` if provided,
+        or with existing 'bnd' locations if previously set.
+
+        Adds model forcing layers:
 
-        * **bnd** geom: waterlevel gauge point locations
         * **bzs** forcing: waterlevel time series [m+ref]
 
         Parameters
         ----------
-        geodataset_fn: str, Path
-            Path or data source name for geospatial point timeseries file.
-            This can either be a netcdf file with geospatial coordinates
-            or a combined point location file with a `timeseries_fn` data csv file.
-
-            * Required variables if netcdf: ['waterlevel']
-            * Required coordinates if netcdf: ['time', 'index', 'y', 'x']
-        timeseries_fn: str, Path
-            Path to spatially uniform timeseries csv file with time index in first column
-            and waterlevels in the second column. The first row is interpreted as header,
-            see :py:meth:`hydromt.open_timeseries_from_table`, for details.
-            NOTE: tabulated timeseries files can only in combination with point location
-            coordinates be set as a geodataset in the data_catalog yml file.
-        offset_fn: str, optional
-            Path or data source name for gridded offset between vertical reference of elevation and waterlevel data,
-            Adds to the waterlevel data before merging.
-
-            * Required variables: ['mdt']
+        geodataset: str, Path, xr.Dataset, optional
+            Path, data source name, or xarray data object for geospatial point timeseries.
+        timeseries: str, Path, pd.DataFrame, optional
+            Path, data source name, or pandas data object for tabular timeseries.
+        locations: str, Path, gpd.GeoDataFrame, optional
+            Path, data source name, or geopandas object for bnd point locations.
+        offset: str, Path, xr.Dataset, float, optional
+            Path, data source name, constant value or xarray raster data for gridded offset
+            between vertical reference of elevation and waterlevel data,
+            The offset is added to the waterlevel data.
         buffer: float, optional
             Buffer [m] around model water level boundary cells to select waterlevel gauges,
             by default 5 km.
+        merge : bool, optional
+            If True, merge with existing forcing data, by default True.
 
+        See Also
+        --------
+        set_forcing_1d
         """
-        name = "waterlevel"
-        msk2 = self.mask == 2
-        if not np.any(msk2):
-            # No waterlevel boundary remove bnd/bzs from sfincs.inp
-            self.logger.warning(
-                "No waterlevel boundary cells (msk==2) in model mask. "
-                "Update the mask layer first before setting waterlevel timeseries."
-            )
-            return
-
+        gdf_locs, df_ts = None, None
         tstart, tstop = self.get_model_time()  # model time
-        if geodataset_fn is not None:
-            if timeseries_fn is not None:
-                kwargs.update(fn_data=str(timeseries_fn))
-            # read and clip data in time & space
-            # buffer around msk==2 values
+        # buffer around msk==2 values
+        if np.any(self.mask == 2):
             region = self.mask.where(self.mask == 2, 0).raster.vectorize()
+        else:
+            region = self.region
+        # read waterlevel data from geodataset or geodataframe
+        if geodataset is not None:
+            # read and clip data in time & space
             da = self.data_catalog.get_geodataset(
-                geodataset_fn,
+                geodataset,
                 geom=region,
                 buffer=buffer,
-                variables=[name],
+                variables=["waterlevel"],
                 time_tuple=(tstart, tstop),
-                crs=self.crs.to_epsg(),  # assume model crs if no explicit crs defined
-                **kwargs,
+                crs=self.crs,
+            )
+            df_ts = da.transpose(..., da.vector.index_dim).to_pandas()
+            gdf_locs = da.vector.to_gdf()
+        elif timeseries is not None:
+            df_ts = self.data_catalog.get_dataframe(
+                timeseries,
+                time_tuple=(tstart, tstop),
+                # kwargs below only applied if timeseries not in data catalog
+                parse_dates=True,
+                index_col=0,
             )
+            df_ts.columns = df_ts.columns.map(int)  # parse column names to integers
         else:
-            # create bnd point on single waterlevel boundary cell
-            x, y = self.staticmaps.raster.xy(*np.where(msk2))
-            gdf = gpd.GeoDataFrame(
-                index=[1], geometry=gpd.points_from_xy(x[[0]], y[[0]]), crs=self.crs
-            )
-            if timeseries_fn is not None:
-                da_ts = hydromt.open_timeseries(timeseries_fn, name=name).sel(
-                    time=slice(tstart, tstop)
-                )
-                assert (
-                    da_ts["index"].size == 1
-                ), "Uniform waterlevel should contain single time series."
-                da = GeoDataArray.from_gdf(gdf, da_ts, index_dim="index")
+            raise ValueError("Either geodataset or timeseries must be provided")
+
+        # optionally read location data (if not already read from geodataset)
+        if gdf_locs is None and locations is not None:
+            gdf_locs = self.data_catalog.get_geodataframe(
+                locations, geom=region, buffer=buffer, crs=self.crs
+            ).to_crs(self.crs)
+        elif gdf_locs is None and "bzs" in self.forcing:
+            gdf_locs = self.forcing["bzs"].vector.to_gdf()
+        elif gdf_locs is None:
+            raise ValueError("No waterlevel boundary (bnd) points provided.")
+
+        # optionally read offset data and correct df_ts
+        if offset is not None and gdf_locs is not None:
+            if isinstance(offset, (float, int)):
+                df_ts += offset
             else:
-                self.set_forcing_1d(xy=gdf, name=name)  # dummy timeseries
-                return
-        # correct for MDT
-        if offset_fn is not None and isfile(offset_fn):
-            da_mdt = self.data_catalog.get_rasterdataset(
-                offset_fn, geom=self.region, buffer=buffer, variables=["mdt"]
-            )
-            mdt_pnts = da_mdt.raster.sample(da.vector.to_gdf()).fillna(0)
-            da = da + mdt_pnts
-            mdt_avg = mdt_pnts.mean().values
-            self.logger.debug(f"{name} forcing: applied MDT (avg: {mdt_avg:+.2f})")
-        self.set_forcing_1d(ts=da, name=name)
-
-    def setup_q_forcing(self, geodataset_fn=None, timeseries_fn=None, **kwargs):
-        """Setup discharge boundary point locations (src) and time series (dis).
+                da_offset = self.data_catalog.get_rasterdataset(
+                    offset, geom=self.region, buffer=5
+                )
+                offset_pnts = da_offset.raster.sample(gdf_locs)
+                df_offset = offset_pnts.to_pandas().reindex(df_ts.columns).fillna(0)
+                df_ts = df_ts + df_offset
+                offset = offset_pnts.mean().values
+            self.logger.debug(
+                f"waterlevel forcing: applied offset (avg: {offset:+.2f})"
+            )
 
-        Use `geodataset_fn` to set the discharge boundary from a dataset of point location
-        timeseries. Only locations within the model domain are selected.
+        # set/ update forcing
+        self.set_forcing_1d(df_ts, gdf_locs, name="bzs", merge=merge)
 
-        Use `timeseries_fn` to set discharge boundary conditions to pre-set (src) locations,
-        e.g. after the :py:meth:`~hydromt_sfincs.SfincsModel.setup_river_inflow` method.
+    def setup_waterlevel_bnd_from_mask(
+        self,
+        distance: float = 1e4,
+        merge: bool = True,
+    ):
+        """Setup waterlevel boundary (bnd) points along model waterlevel boundary (msk=2).
 
-        The dataset/timeseries are clipped to the model time based on the model config
-        tstart and tstop entries.
+        The waterlevel boundary (msk=2) should be set before calling this method,
+        e.g.: with `setup_mask_bounds`
+
+        Waterlevels (bzs) are set to zero at these points, but can be updated
+        with `setup_waterlevel_forcing`.
+
+        Parameters
+        ----------
+        distance: float, optional
+            Distance [m] between waterlevel boundary points,
+            by default 10 km.
+        merge : bool, optional
+            If True, merge with existing forcing data, by default True.
+
+        See Also
+        --------
+        setup_waterlevel_forcing
+        setup_mask_bounds
+        """
+        # get waterlevel boundary vector based on mask
+        gdf_msk = utils.get_bounds_vector(self.mask)
+        gdf_msk2 = gdf_msk[gdf_msk["value"] == 2]
+
+        # create points along boundary
+        points = []
+        for _, row in gdf_msk2.iterrows():
+            distances = np.arange(0, row.geometry.length, distance)
+            for d in distances:
+                point = row.geometry.interpolate(d)
+                points.append((point.x, point.y))
+
+        # create geodataframe with points
+        gdf = gpd.GeoDataFrame(geometry=gpd.points_from_xy(*zip(*points)), crs=self.crs)
+
+        # set waterlevel boundary
+        self.set_forcing_1d(gdf_locs=gdf, name="bzs", merge=merge)
+
+    def setup_discharge_forcing(
+        self, geodataset=None, timeseries=None, locations=None, merge=True
+    ):
+        """Setup discharge forcing.
+
+        Discharge timeseries are read from a `geodataset` (geospatial point timeseries)
+        or a tabular `timeseries` dataframe. At least one of these must be provided.
+
+        The tabular timeseries data is combined with `locations` if provided,
+        or with existing 'src' locations if previously set, e.g., with the
+        `setup_river_inflow` method.
 
         Adds model layers:
 
-        * **src** geom: discharge gauge point locations
         * **dis** forcing: discharge time series [m3/s]
 
         Parameters
         ----------
-        geodataset_fn: str, Path
-            Path or data source name for geospatial point timeseries file.
-            This can either be a netcdf file with geospatial coordinates
-            or a combined point location file with a timeseries data csv file
-            which can be setup through the data_catalog yml file.
-
-            * Required variables if netcdf: ['discharge']
-            * Required coordinates if netcdf: ['time', 'index', 'y', 'x']
-        timeseries_fn: str, Path
-            Path to tabulated timeseries csv file with time index in first column
-            and location IDs in the first row,
-            see :py:meth:`hydromt.open_timeseries_from_table`, for details.
-            NOTE: tabulated timeseries files can only in combination with point location
-            coordinates be set as a geodataset in the data_catalog yml file.
-
+        geodataset: str, Path, xr.Dataset, optional
+            Path, data source name, or xarray data object for geospatial point timeseries.
+        timeseries: str, Path, pd.DataFrame, optional
+            Path, data source name, or pandas data object for tabular timeseries.
+        locations: str, Path, gpd.GeoDataFrame, optional
+            Path, data source name, or geopandas object for bnd point locations.
+        merge : bool, optional
+            If True, merge with existing forcing data, by default True.
+
+        See Also
+        --------
+        setup_river_inflow
         """
-        name = "discharge"
-        fname = self._FORCING[name][0]
-        tstart, tstop = self.get_model_time()  # time slice
-        if geodataset_fn is None and fname not in self.forcing:
-            self.logger.warning(
-                "No discharge inflow (src) points set: "
-                "Run ``setup_river_inflow()`` method first or provide locations."
+        gdf_locs, df_ts = None, None
+        tstart, tstop = self.get_model_time()  # model time
+        # read waterlevel data from geodataset or geodataframe
+        if geodataset is not None:
+            # read and clip data in time & space
+            da = self.data_catalog.get_geodataset(
+                geodataset,
+                geom=self.region,
+                variables=["discharge"],
+                time_tuple=(tstart, tstop),
+                crs=self.crs,
             )
-            return
-        elif geodataset_fn is not None:
-            if timeseries_fn is not None:
-                kwargs.update(fn_data=str(timeseries_fn))
-            # read and clip data
-            da = (
-                self.data_catalog.get_geodataset(
-                    geodataset_fn,
-                    geom=self.region,
-                    variables=[name],
-                    time_tuple=(tstart, tstop),
-                    crs=self.crs.to_epsg(),  # assume model crs if none defined
-                    **kwargs,
-                )
-                .fillna(0.0)
-                .rename(fname)
+            df_ts = da.transpose(..., da.vector.index_dim).to_pandas()
+            gdf_locs = da.vector.to_gdf()
+        elif timeseries is not None:
+            df_ts = self.data_catalog.get_dataframe(
+                timeseries,
+                time_tuple=(tstart, tstop),
+                # kwargs below only applied if timeseries not in data catalog
+                parse_dates=True,
+                index_col=0,
             )
-            self.set_forcing_1d(ts=da, name=name)
-        elif timeseries_fn is not None:
-            # read timeseries data and match with existing gdf
-            gdf = self.forcing[fname].vector.to_gdf()
-            da_ts = hydromt.open_timeseries_from_table(timeseries_fn, name=name)
-            da_ts = da_ts.sel(time=slice(tstart, tstop)).fillna(0.0)
-            self.set_forcing_1d(ts=da_ts, xy=gdf, name=name)
+            df_ts.columns = df_ts.columns.map(int)  # parse column names to integers
         else:
-            raise ValueError(
-                'Either "geodataset_fn" or "timeseries_fn" must be provided.'
-            )
+            raise ValueError("Either geodataset or timeseries must be provided")
+
+        # optionally read location data (if not already read from geodataset)
+        if gdf_locs is None and locations is not None:
+            gdf_locs = self.data_catalog.get_geodataframe(
+                locations, geom=self.region, crs=self.crs
+            ).to_crs(self.crs)
+        elif gdf_locs is None and "dis" in self.forcing:
+            gdf_locs = self.forcing["dis"].vector.to_gdf()
+        elif gdf_locs is None:
+            raise ValueError("No discharge boundary (src) points provided.")
 
-    def setup_q_forcing_from_grid(
+        # set/ update forcing
+        self.set_forcing_1d(df_ts, gdf_locs, name="dis", merge=merge)
+
+    def setup_discharge_forcing_from_grid(
         self,
-        discharge_fn,
-        locs_fn=None,
-        uparea_fn=None,
+        discharge,
+        locations=None,
+        uparea=None,
         wdw=1,
         rel_error=0.05,
         abs_error=50,
-        **kwargs,  # catch deprecated args
     ):
-        """Setup discharge boundary location (src) and timeseries (dis) based on a
-        gridded discharge dataset.
+        """Setup discharge forcing based on a gridded discharge dataset.
 
-        If `locs_fn` is not provided, the discharge source locations are expected to be
-        pre-set, e.g. using the :py:meth:`~hydromt_sfincs.SfincsModel.setup_river_inflow` method.
+        Discharge boundary timesereis are read from the `discharge` dataset
+        with gridded discharge time series data.
 
-        If an upstream area grid is provided the discharge boundary condition is
-        snapped to the best fitting grid cell within a `wdw` neighboring cells.
-        The best fit is dermined based on the minimal relative upstream area error if
-        an upstream area value is available for the discharge boundary locations;
-        otherwise it is based on maximum upstream area.
+        The `locations` are snapped to the `uparea` grid if provided based their
+        uparea attribute. If not provided, the nearest grid cell is used.
 
         Adds model layers:
 
-        * **src** geom: discharge gauge point locations
         * **dis** forcing: discharge time series [m3/s]
 
+        Adds meta layer (not used by SFINCS):
+
+        * **src_snapped** geom: snapped gauge location on discharge grid
+
         Parameters
         ----------
-        discharge_fn: str, Path, optional
-            Path or data source name for gridded discharge timeseries dataset.
+        discharge: str, Path, xr.DataArray optional
+            Path,  data source name or xarray data object for gridded discharge timeseries dataset.
 
             * Required variables: ['discharge' (m3/s)]
             * Required coordinates: ['time', 'y', 'x']
-        locs_fn: str, Path, optional
-            Path or data source name for point location dataset. Not required if
-            point location have previously been set with :py:meth:`~hydromt_sfincs.SfincsModel.setup_river_inflow`
-            See :py:meth:`hydromt.open_vector`, for accepted files.
+        locations: str, Path, gpd.GeoDataFrame, optional
+            Path, data source name, or geopandas data object for point location dataset.
+            Not required if point location have previously been set, e.g. using the
+            :py:meth:`~hydromt_sfincs.SfincsModel.setup_river_inflow` method.
 
-        uparea_fn: str, Path, optional
-            Path to upstream area grid in gdal (e.g. geotiff) or netcdf format.
+            * Required variables: ['uparea' (km2)]
+        uparea: str, Path, optional
+            Path, data source name, or xarray data object for upstream area grid.
 
             * Required variables: ['uparea' (km2)]
         wdw: int, optional
             Window size in number of cells around discharge boundary locations
-            to snap to, only used if ``uparea_fn`` is provided. By default 1.
+            to snap to, only used if ``uparea`` is provided. By default 1.
         rel_error, abs_error: float, optional
             Maximum relative error (default 0.05) and absolute error (default 50 km2)
             between the discharge boundary location upstream area and the upstream area of
-            the best fit grid cell, only used if "discharge" staticgeoms has a "uparea" column.
+            the best fit grid cell, only used if "discharge" geoms has a "uparea" column.
+
+        See Also
+        --------
+        setup_river_inflow
         """
-        if "max_error" in kwargs:
-            self.logger.warning(
-                "'max_error' is deprecated use 'rel_error' and 'abs_error' instead."
-            )
-            rel_error = kwargs.pop("max_error")
-            abs_error = 0  # mimic old behaviour
-
-        name = "discharge"
-        fname = self._FORCING[name][0]
-        if locs_fn is not None:
+        if locations is not None:
             gdf = self.data_catalog.get_geodataframe(
-                locs_fn, geom=self.region, assert_gtype="Point"
+                locations, geom=self.region, assert_gtype="Point"
             ).to_crs(self.crs)
-        elif fname in self.forcing:
-            da = self.forcing[fname]
-            gdf = da.vector.to_gdf()
+        elif "dis" in self.forcing:
+            gdf = self.forcing["dis"].vector.to_gdf()
         else:
-            self.logger.warning(
-                'No discharge inflow points in staticgeoms. Provide locations using "locs_fn" or '
-                'run "setup_river_inflow()" method first to determine inflow locations.'
-            )
-            return
+            raise ValueError("No discharge boundary (src) points provided.")
+
         # read data
         ds = self.data_catalog.get_rasterdataset(
-            discharge_fn,
+            discharge,
             geom=self.region,
             buffer=2,
             time_tuple=self.get_model_time(),  # model time
-            variables=[name],
+            variables=["discharge"],
             single_var_as_array=False,
         )
-        if uparea_fn is not None and "uparea" in gdf.columns:
+        if uparea is not None and "uparea" in gdf.columns:
             da_upa = self.data_catalog.get_rasterdataset(
-                uparea_fn, geom=self.region, buffer=2, variables=["uparea"]
+                uparea, geom=self.region, buffer=2, variables=["uparea"]
             )
             # make sure ds and da_upa align
             ds["uparea"] = da_upa.raster.reproject_like(ds, method="nearest")
         elif "uparea" not in gdf.columns:
             self.logger.warning('No "uparea" column found in location data.')
 
-        da_q = workflows.snap_discharge(
+        # TODO use hydromt core method
+        ds_snapped = workflows.snap_discharge(
             ds=ds,
             gdf=gdf,
             wdw=wdw,
             rel_error=rel_error,
             abs_error=abs_error,
             uparea_name="uparea",
-            discharge_name=name,
+            discharge_name="discharge",
             logger=self.logger,
         )
         # set zeros for src points without matching discharge
-        da_q = da_q.reindex(index=gdf.index, fill_value=0).fillna(0)
-
+        da_q = ds_snapped["discharge"].reindex(index=gdf.index, fill_value=0).fillna(0)
+        df_q = da_q.transpose("time", ...).to_pandas()
         # update forcing
-        self.set_forcing_1d(name=name, ts=da_q, xy=gdf)
+        self.set_forcing_1d(df_ts=df_q, gdf_locs=gdf, name="dis")
+        # keep snapped locations
+        self.set_geoms(ds_snapped.vector.to_gdf(), "src_snapped")
 
-    def setup_p_forcing_from_grid(
-        self, precip_fn=None, dst_res=None, aggregate=False, **kwargs
+    def setup_precip_forcing_from_grid(
+        self, precip=None, dst_res=None, aggregate=False, **kwargs
     ):
         """Setup precipitation forcing from a gridded spatially varying data source.
 
         If aggregate is True, spatially uniform precipitation forcing is added to
         the model based on the mean precipitation over the model domain.
         If aggregate is False, distributed precipitation is added to the model as netcdf file.
         The data is reprojected to the model CRS (and destination resolution `dst_res` if provided).
@@ -1558,111 +1633,209 @@
         Adds one of these model layer:
 
         * **netamprfile** forcing: distributed precipitation [mm/hr]
         * **precipfile** forcing: uniform precipitation [mm/hr]
 
         Parameters
         ----------
-        precip_fn, str, Path
+        precip, str, Path
             Path to precipitation rasterdataset netcdf file.
 
             * Required variables: ['precip' (mm)]
             * Required coordinates: ['time', 'y', 'x']
 
         dst_res: float
             output resolution (m), by default None and computed from source data.
             Only used in combination with aggregate=False
         aggregate: bool, {'mean', 'median'}, optional
             Method to aggregate distributed input precipitation data. If True, mean
             aggregation is used, if False (default) the data is not aggregated and
             spatially distributed precipitation is returned.
         """
-        variable = "precip"
         # get data for model domain and config time range
         precip = self.data_catalog.get_rasterdataset(
-            precip_fn,
+            precip,
             geom=self.region,
             buffer=2,
             time_tuple=self.get_model_time(),
-            variables=[variable],
+            variables=["precip"],
         )
 
         # aggregate or reproject in space
         if aggregate:
             stat = aggregate if isinstance(aggregate, str) else "mean"
-            self.logger.debug(f"Aggregate {variable} using {stat}.")
+            self.logger.debug(f"Aggregate precip using {stat}.")
             zone = self.region.dissolve()  # make sure we have a single (multi)polygon
             precip_out = precip.raster.zonal_stats(zone, stats=stat)[f"precip_{stat}"]
-            precip_out = precip_out.where(precip_out >= 0, 0).fillna(0).squeeze()
+            df_ts = precip_out.where(precip_out >= 0, 0).fillna(0).squeeze().to_pandas()
+            self.setup_precip_forcing(df_ts.to_frame())
         else:
             # reproject to model utm crs
             # NOTE: currently SFINCS errors (stack overflow) on large files,
             # downscaling to model grid is not recommended
             kwargs0 = dict(align=dst_res is not None, method="nearest_index")
             kwargs0.update(kwargs)
             meth = kwargs0["method"]
-            self.logger.debug(f"Resample {variable} using {meth}.")
+            self.logger.debug(f"Resample precip using {meth}.")
             precip_out = precip.raster.reproject(
                 dst_crs=self.crs, dst_res=dst_res, **kwargs
             ).fillna(0)
 
-        # resample in time
-        precip_out = hydromt.workflows.resample_time(
-            precip_out,
-            freq=pd.to_timedelta("1H"),
-            conserve_mass=True,
-            upsampling="bfill",
-            downsampling="sum",
-            logger=self.logger,
-        )
-        precip_out.name = "Precipitation"  # capital is important for netamprfile
+            # resample in time
+            precip_out = hydromt.workflows.resample_time(
+                precip_out,
+                freq=pd.to_timedelta("1H"),
+                conserve_mass=True,
+                upsampling="bfill",
+                downsampling="sum",
+                logger=self.logger,
+            ).rename("precip")
 
-        # set correct names and attrs and add forcing
-        fname = self._FORCING[variable][0]
-        fname2 = self._FORCING[f"{variable}2D"][0]
-        if aggregate:
-            # remove netamprfile
-            self._forcing.pop(fname2, None)
-            self._config.pop(f"{fname2}file", None)
-            # precipfile = sfincs.precip
-            fn_out = f"sfincs.{fname}"
-        else:
-            # remove precipfile
-            self._forcing.pop(fname, None)
-            self._config.pop(f"{fname}file", None)
-            # netamprfile = precip.nc
-            fn_out = f"{variable}.nc"
-            fname = fname2
-        precip_out.attrs.update(**self._ATTRS.get(fname, {}))
-        self.set_config(f"{fname}file", fn_out)
-        self.set_forcing(precip_out, name=fname)
+            # add to forcing
+            self.set_forcing(precip_out, name="precip")
 
-    def setup_p_forcing(self, precip_fn=None, **kwargs):
+    def setup_precip_forcing(self, timeseries):
         """Setup spatially uniform precipitation forcing (precip).
 
         Adds model layers:
 
         * **precipfile** forcing: uniform precipitation [mm/hr]
 
         Parameters
         ----------
-        precip_fn, str, Path
+        timeseries, str, Path
             Path to tabulated timeseries csv file with time index in first column
             and location IDs in the first row,
             see :py:meth:`hydromt.open_timeseries_from_table`, for details.
             Note: tabulated timeseries files cannot yet be set through the data_catalog yml file.
         """
-        ts = hydromt.open_timeseries_from_table(precip_fn, **kwargs)
-        self.set_forcing_1d(name="precip", ts=ts.squeeze())
-        # remove netamprfile
-        fname2 = self._FORCING["precip2D"][0]
-        self._forcing.pop(fname2, None)
-        self._config.pop(f"{fname2}file", None)
+        tstart, tstop = self.get_model_time()
+        df_ts = self.data_catalog.get_dataframe(
+            timeseries,
+            time_tuple=(tstart, tstop),
+            # kwargs below only applied if timeseries not in data catalog
+            parse_dates=True,
+            index_col=0,
+        )
+        if isinstance(df_ts, pd.DataFrame):
+            df_ts = df_ts.squeeze()
+        if not isinstance(df_ts, pd.Series):
+            raise ValueError("df_ts must be a pandas.Series")
+        df_ts.name = "precip"
+        df_ts.index.name = "time"
+        self.set_forcing(df_ts.to_xarray(), name="precip")
 
-    def plot_forcing(self, fn_out="forcing.png", **kwargs):
+    def setup_tiles(
+        self,
+        path: Union[str, Path] = None,
+        region: dict = None,
+        datasets_dep: List[dict] = [],
+        zoom_range: Union[int, List[int]] = [0, 13],
+        z_range: List[int] = [-20000.0, 20000.0],
+        create_index_tiles: bool = True,
+        create_topobathy_tiles: bool = True,
+        fmt: str = "bin",
+    ):
+        """Create both index and topobathy tiles in webmercator format.
+
+        Parameters
+        ----------
+        path : Union[str, Path]
+            Directory in which to store the index tiles, if None, the model root + tiles is used.
+        region : dict
+            Dictionary describing region of interest, e.g.:
+            * {'bbox': [xmin, ymin, xmax, ymax]}. Note bbox should be provided in WGS 84
+            * {'geom': 'path/to/polygon_geometry'}
+            If None, the model region is used.
+        datasets_dep : List[dict]
+            List of dictionaries with topobathy data, each containing a dataset name or Path (elevtn) and optional merge arguments e.g.:
+            [{'elevtn': merit_hydro, 'zmin': 0.01}, {'elevtn': gebco, 'offset': 0, 'merge_method': 'first', reproj_method: 'bilinear'}]
+            For a complete overview of all merge options, see :py:function:~hydromt.workflows.merge_multi_dataarrays
+            Note that subgrid/dep_subgrid.tif is automatically used if present and datasets_dep is left empty.
+        zoom_range : Union[int, List[int]], optional
+            Range of zoom levels for which tiles are created, by default [0,13]
+        z_range : List[int], optional
+            Range of valid elevations that are included in the topobathy tiles, by default [-20000.0, 20000.0]
+        create_index_tiles : bool, optional
+            If True, index tiles are created, by default True
+        create_topobathy_tiles : bool, optional
+            If True, topobathy tiles are created, by default True.
+        fmt : str, optional
+            Format of the tiles: "bin" (binary, default), or "png".
+        """
+        # use model root if path not provided
+        if path is None:
+            path = os.path.join(self.root, "tiles")
+
+        # use model region if region not provided
+        if region is None:
+            region = self.region
+        else:
+            _kind, _region = hydromt.workflows.parse_region(region=region)
+            if "bbox" in _region:
+                bbox = _region["bbox"]
+                region = gpd.GeoDataFrame(geometry=[box(*bbox)], crs=4326)
+            elif "geom" in _region:
+                region = _region["geom"]
+                if region.crs is None:
+                    raise ValueError('Model region "geom" has no CRS')
+
+        # if only one zoom level is specified, create tiles up to that zoom level (inclusive)
+        if isinstance(zoom_range, int):
+            zoom_range = [0, zoom_range]
+
+        # create index tiles
+        if create_index_tiles:
+            # only binary and png are supported for index tiles so set to binary if tif
+            fmt_ind = "bin" if fmt == "tif" else fmt
+
+            if self.grid_type == "regular":
+                self.reggrid.create_index_tiles(
+                    region=region,
+                    root=path,
+                    zoom_range=zoom_range,
+                    fmt=fmt_ind,
+                    logger=self.logger,
+                )
+            elif self.grid_type == "quadtree":
+                raise NotImplementedError(
+                    "Index tiles not yet implemented for quadtree grids."
+                )
+
+        # create topobathy tiles
+        if create_topobathy_tiles:
+            # compute resolution of highest zoom level
+            # resolution of zoom level 0  on equator: 156543.03392804097
+            res = 156543.03392804097 / 2 ** zoom_range[1]
+            datasets_dep = self._parse_datasets_dep(datasets_dep, res=res)
+
+            # if no datasets provided, check if high-res subgrid geotiff is there
+            if len(datasets_dep) == 0:
+                if os.path.exists(os.path.join(self.root, "subgrid")):
+                    # check if there is a dep_subgrid.tif
+                    dep = os.path.join(self.root, "subgrid", "dep_subgrid.tif")
+                    if os.path.exists(dep):
+                        da = self.data_catalog.get_rasterdataset(dep)
+                        datasets_dep.append({"da": da})
+                    else:
+                        raise ValueError("No topobathy datasets provided.")
+
+            # create topobathy tiles
+            workflows.tiling.create_topobathy_tiles(
+                root=path,
+                region=region,
+                datasets_dep=datasets_dep,
+                index_path=os.path.join(path, "index"),
+                zoom_range=zoom_range,
+                z_range=z_range,
+                fmt=fmt,
+            )
+
+    # Plotting
+    def plot_forcing(self, fn_out=None, **kwargs):
         """Plot model timeseries forcing.
 
         For distributed forcing a spatial avarage is plotted.
 
         Parameters
         ----------
         fn_out: str
@@ -1673,118 +1846,130 @@
             Model forcing
 
         Returns
         -------
         fig, axes
             Model fig and ax objects
         """
-        import matplotlib.pyplot as plt
         import matplotlib.dates as mdates
+        import matplotlib.pyplot as plt
 
         if self.forcing:
-            # update missing attributes for plot labels
+            forcing = {}
             for name in self.forcing:
-                attrs = self._ATTRS.get(name, {})
-                self.forcing[name].attrs.update(**attrs)
-            fig, axes = plots.plot_forcing(self.forcing, **kwargs)
-
-            # set xlim to model tstart - tend
-            tstart, tstop = self.get_model_time()
-            axes[-1].set_xlim(mdates.date2num([tstart, tstop]))
-
-            # save figure
-            if fn_out is not None:
-                if not os.path.isabs(fn_out):
-                    fn_out = join(self.root, "figs", fn_out)
-                if not os.path.isdir(dirname(fn_out)):
-                    os.makedirs(dirname(fn_out))
-                plt.savefig(fn_out, dpi=225, bbox_inches="tight")
-            return fig, axes
+                if isinstance(self.forcing[name], xr.Dataset):
+                    continue  # plot only dataarrays
+                forcing[name] = self.forcing[name]
+                # update missing attributes for plot labels
+                forcing[name].attrs.update(**self._ATTRS.get(name, {}))
+            if len(forcing) > 0:
+                fig, axes = plots.plot_forcing(forcing, **kwargs)
+                # set xlim to model tstart - tend
+                tstart, tstop = self.get_model_time()
+                axes[-1].set_xlim(mdates.date2num([tstart, tstop]))
+
+                # save figure
+                if fn_out is not None:
+                    if not os.path.isabs(fn_out):
+                        fn_out = join(self.root, "figs", fn_out)
+                    if not os.path.isdir(dirname(fn_out)):
+                        os.makedirs(dirname(fn_out))
+                    plt.savefig(fn_out, dpi=225, bbox_inches="tight")
+                return fig, axes
+        else:
+            raise ValueError("No forcing found in model.")
 
     def plot_basemap(
         self,
-        fn_out: str = "basemap.png",
+        fn_out: str = None,
         variable: str = "dep",
-        shaded: bool = True,
+        shaded: bool = False,
         plot_bounds: bool = True,
         plot_region: bool = False,
         plot_geoms: bool = True,
-        bmap: str = "sat",
+        bmap: str = None,
         zoomlevel: int = 11,
         figsize: Tuple[int] = None,
-        geoms: List[str] = None,
+        geom_names: List[str] = None,
         geom_kwargs: Dict = {},
         legend_kwargs: Dict = {},
         **kwargs,
     ):
         """Create basemap plot.
 
         Parameters
         ----------
-        fn_out: str
-            Path to output figure file.
+        fn_out: str, optional
+            Path to output figure file, by default None.
             If a basename is given it is saved to <model_root>/figs/<fn_out>
             If None, no file is saved.
-        staticmaps : xr.Dataset
-            Dataset with model maps
-        staticgeoms : Dict of geopandas.GeoDataFrame
-            Model geometries
         variable : str, optional
-            Map name to plot, by default 'dep'
+            Map of variable in ds to plot, by default 'dep'
         shaded : bool, optional
-            Add shade to variable (only for variable = 'dep'), by default True
+            Add shade to variable (only for variable = 'dep' and non-rotated grids),
+            by default False
         plot_bounds : bool, optional
             Add waterlevel (msk=2) and open (msk=3) boundary conditions to plot.
         plot_region : bool, optional
             If True, plot region outline.
         plot_geoms : bool, optional
             If True, plot available geoms.
-        bmap : {'sat', ''}
-            background map, by default "sat"
+        bmap : {'sat', 'osm'}, optional
+            background map, by default None
         zoomlevel : int, optional
             zoomlevel, by default 11
         figsize : Tuple[int], optional
             figure size, by default None
-        geoms : List[str], optional
+        geom_names : List[str], optional
             list of model geometries to plot, by default all model geometries.
         geom_kwargs : Dict of Dict, optional
             Model geometry styling per geometry, passed to geopandas.GeoDataFrame.plot method.
             For instance: {'src': {'markersize': 30}}.
         legend_kwargs : Dict, optional
             Legend kwargs, passed to ax.legend method.
 
         Returns
         -------
         fig, axes
             Model fig and ax objects
         """
         import matplotlib.pyplot as plt
 
-        # combine staticgeoms and forcing locations
-        sg = self.staticgeoms.copy()
-        for fname, gname in self._FORCING.values():
-            if fname in self.forcing and gname is not None:
-                sg.update({gname: self._forcing[fname].vector.to_gdf()})
-
-        # make sure staticmaps are set
-        if self._MAPS["mask"] not in self.staticmaps:
-            self.set_staticmaps(self.mask, self._MAPS["mask"])
+        # combine geoms and forcing locations
+        sg = self.geoms.copy()
+        for fname, gname in self._FORCING_1D.values():
+            if fname[0] in self.forcing and gname is not None:
+                try:
+                    sg.update({gname: self._forcing[fname[0]].vector.to_gdf()})
+                except ValueError:
+                    self.logger.debug(f'unable to plot forcing location: "{fname}"')
+        if plot_region and "region" not in self.geoms:
+            sg.update({"region": self.region})
+
+        # make sure grid are set
+        if variable.startswith("subgrid.") and self.subgrid:
+            ds = self.subgrid.copy()
+            variable = variable.replace("subgrid.", "")
+        else:
+            ds = self.grid.copy()
+        if "msk" not in ds:
+            ds["msk"] = self.mask
 
         fig, ax = plots.plot_basemap(
-            self.staticmaps,
-            staticgeoms=sg,
+            ds,
+            sg,
             variable=variable,
             shaded=shaded,
             plot_bounds=plot_bounds,
             plot_region=plot_region,
             plot_geoms=plot_geoms,
             bmap=bmap,
             zoomlevel=zoomlevel,
             figsize=figsize,
-            geoms=geoms,
+            geom_names=geom_names,
             geom_kwargs=geom_kwargs,
             legend_kwargs=legend_kwargs,
             **kwargs,
         )
 
         if fn_out is not None:
             if not os.path.isabs(fn_out):
@@ -1792,340 +1977,490 @@
             if not os.path.isdir(dirname(fn_out)):
                 os.makedirs(dirname(fn_out))
             plt.savefig(fn_out, dpi=225, bbox_inches="tight")
 
         return fig, ax
 
     # I/O
-    def read(self):
+    def read(self, epsg: int = None):
         """Read the complete model schematization and configuration from file."""
-        self.read_config()
-        self.read_staticmaps()
-        self.read_staticgeoms()
+        self.read_config(epsg=epsg)
+        if epsg is None and "epsg" not in self.config:
+            raise ValueError(f"Please specify epsg to read this model")
+        self.read_grid()
+        self.read_subgrid()
+        self.read_geoms()
         self.read_forcing()
         self.logger.info("Model read")
 
     def write(self):
         """Write the complete model schematization and configuration to file."""
         self.logger.info(f"Writing model data to {self.root}")
-        self.write_staticmaps()
-        self.write_staticgeoms()
+        # TODO - add check for subgrid & quadtree > give flags to self.write_grid() and self.write_config()
+        self.write_grid()
+        self.write_subgrid()
+        self.write_geoms()
         self.write_forcing()
         self.write_states()
         # config last; might be udpated when writing maps, states or forcing
         self.write_config()
         # write data catalog with used data sources
-        self.write_data_catalog()  # new in hydromt v0.4.4
+        # self.write_data_catalog()  # new in hydromt v0.4.4
 
-    def read_staticmaps(self, crs=None):
-        """Read SFINCS binary staticmaps and save to `staticmaps` attribute.
-        Known binary files mentioned in the sfincs.inp configuration file are read,
-        including: msk/dep/scs/manning/qinf.
+    def read_grid(self, data_vars: Union[List, str] = None) -> None:
+        """Read SFINCS binary grid files and save to `grid` attribute.
+        Filenames are taken from the `config` attribute (i.e. input file).
 
         Parameters
         ----------
-        crs: int, CRS
-            Coordinate reference system, if provided use instead of epsg code from sfincs.inp
+        data_vars : Union[List, str], optional
+            List of data variables to read, by default None (all)
         """
-        # read geospatial attributes from sfincs.inp, save with with S->N orientation
-        shape, transform, crs = self.get_spatial_attrs(crs=crs)
 
-        # read raw numbers and reshape to 2D arrays
-        fn_ind = abspath(join(self._root, self.config.get("indexfile")))
-        if not isfile(fn_ind):
-            raise IOError(f".ind path {fn_ind} does not exist")
-        ind = utils.read_binary_map_index(fn_ind)
+        da_lst = []
+        if data_vars is None:
+            data_vars = self._MAPS
+        elif isinstance(data_vars, str):
+            data_vars = list(data_vars)
+
+        # read index file
+        ind_fn = self.get_config("indexfile", fallback="sfincs.ind", abs_path=True)
+        if not isfile(ind_fn):
+            raise IOError(f".ind path {ind_fn} does not exist")
 
         dtypes = {"msk": "u1"}
         mvs = {"msk": 0}
-        data_vars = {}
-        for name, mname in self._MAPS.items():
-            if f"{mname}file" in self.config:
-                fn = self.get_config(f"{mname}file", abs_path=True)
-                if not isfile(fn):
-                    self.logger.warning(f"{mname}file not found at {fn}")
-                    continue
-                dtype = dtypes.get(mname, "f4")
-                mv = mvs.get(mname, -9999.0)
-                data = utils.read_binary_map(fn, ind, shape, mv, dtype)
-                data_vars.update({mname: (data, mv)})
-
-        # create dataset and set as staticmaps
-        ds = RasterDataset.from_numpy(
-            data_vars=data_vars,
-            transform=transform,
-            crs=crs,
-        )
-        for name in ds.data_vars:
-            ds[name].attrs.update(**self._ATTRS.get(name, {}))
-        self.set_staticmaps(ds)
-
-        # keep some metadata maps from gis directory
-        keep_maps = ["flwdir", "uparea", "rivmsk"]
-        fns = glob.glob(join(self.root, "gis", "*.tif"))
-        fns = [fn for fn in fns if basename(fn).split(".")[0] in keep_maps]
-        if fns:
-            ds = hydromt.open_mfraster(fns).load()
-            self.set_staticmaps(ds)
-            ds.close()
-
-    def write_staticmaps(self):
-        """Write SFINCS staticmaps to binary files including map index file.
-        Filenames are taken from the `config` attribute.
+        if self.reggrid is not None:
+            ind = self.reggrid.read_ind(ind_fn=ind_fn)
+
+            for name in data_vars:
+                if f"{name}file" in self.config:
+                    fn = self.get_config(
+                        f"{name}file", fallback=f"sfincs.{name}", abs_path=True
+                    )
+                    if not isfile(fn):
+                        self.logger.warning(f"{name}file not found at {fn}")
+                        continue
+                    dtype = dtypes.get(name, "f4")
+                    mv = mvs.get(name, -9999.0)
+                    da = self.reggrid.read_map(fn, ind, dtype, mv, name=name)
+                    da_lst.append(da)
+            ds = xr.merge(da_lst)
+            epsg = self.config.get("epsg", None)
+            if epsg is not None:
+                ds.raster.set_crs(epsg)
+            self.set_grid(ds)
+
+            # keep some metadata maps from gis directory
+            fns = glob.glob(join(self.root, "gis", "*.tif"))
+            fns = [
+                fn
+                for fn in fns
+                if basename(fn).split(".")[0] not in self.grid.data_vars
+            ]
+            if fns:
+                ds = hydromt.open_mfraster(fns).load()
+                self.set_grid(ds)
+                ds.close()
+
+    def write_grid(self, data_vars: Union[List, str] = None):
+        """Write SFINCS grid to binary files including map index file.
+        Filenames are taken from the `config` attribute (i.e. input file).
 
-        If `write_gis` property is True, all staticmaps are written to geotiff
+        If `write_gis` property is True, all grid variables are written to geotiff
         files in a "gis" subfolder.
-        """
-        if not self._write:
-            raise IOError("Model opened in read-only")
-        elif not self._staticmaps:
-            return
 
-        # make sure a mask is set
-        if self._MAPS["mask"] not in self.staticmaps:
-            self.set_staticmaps(self.mask, self._MAPS["mask"])
-
-        # make sure orientation is S->N
-        ds_out = self.staticmaps
-        if ds_out.raster.res[1] < 0:
-            ds_out = ds_out.raster.flipud()
-
-        self.logger.debug("Write binary map indices based on mask.")
-        msk = ds_out[self._MAPS["mask"]].values
-        fn_ind = self.get_config("indexfile", abs_path=True)
-        utils.write_binary_map_index(fn_ind, msk=msk)
+        Parameters
+        ----------
+        data_vars : Union[List, str], optional
+            List of data variables to write, by default None (all)
+        """
+        self._assert_write_mode
 
-        dvars = [v for v in self._MAPS.values() if v in ds_out]
-        self.logger.debug(f"Write binary map files: {dvars}.")
         dtypes = {"msk": "u1"}  # default to f4
-        for mname in dvars:
-            if f"{mname}file" not in self.config:
-                self.set_config(f"{mname}file", f"sfincs.{mname}")
-            fn_out = self.get_config(f"{mname}file", abs_path=True)
-            utils.write_binary_map(
-                fn_out,
-                ds_out[mname].values,
-                msk=msk,
-                dtype=dtypes.get(mname, "f4"),
-            )
+        if self.reggrid and len(self.grid.data_vars) > 0 and "msk" in self.grid:
+            # make sure orientation is S->N
+            ds_out = self.grid
+            if ds_out.raster.res[1] < 0:
+                ds_out = ds_out.raster.flipud()
+            mask = ds_out["msk"].values
+
+            self.logger.debug("Write binary map indices based on mask.")
+            ind_fn = self.get_config("indexfile", abs_path=True)
+            self.reggrid.write_ind(ind_fn=ind_fn, mask=mask)
+
+            if data_vars is None:  # write all maps
+                data_vars = [v for v in self._MAPS if v in ds_out]
+            elif isinstance(data_vars, str):
+                data_vars = list(data_vars)
+            self.logger.debug(f"Write binary map files: {data_vars}.")
+            for name in data_vars:
+                if f"{name}file" not in self.config:
+                    self.set_config(f"{name}file", f"sfincs.{name}")
+                # do not write depfile if subgrid is used
+                if (name == "dep" or name == "manning") and self.subgrid:
+                    continue
+                self.reggrid.write_map(
+                    map_fn=self.get_config(f"{name}file", abs_path=True),
+                    data=ds_out[name].values,
+                    mask=mask,
+                    dtype=dtypes.get(name, "f4"),
+                )
 
         if self._write_gis:
-            self.write_raster("staticmaps")
+            self.write_raster("grid")
+
+    def read_subgrid(self):
+        """Read SFINCS subgrid file and add to `subgrid` attribute.
+        Filename is taken from the `config` attribute (i.e. input file)."""
+
+        self._assert_read_mode
 
-    def read_staticgeoms(self):
-        """Read geometry files if and save to `staticgeoms` attribute.
+        if "sbgfile" in self.config:
+            fn = self.get_config("sbgfile", abs_path=True)
+            if not isfile(fn):
+                self.logger.warning(f"sbgfile not found at {fn}")
+                return
+
+            self.reggrid.subgrid.load(file_name=fn, mask=self.mask)
+            self.subgrid = self.reggrid.subgrid.to_xarray(
+                dims=self.mask.raster.dims, coords=self.mask.raster.coords
+            )
+
+    def write_subgrid(self):
+        """Write SFINCS subgrid file."""
+        self._assert_write_mode
+
+        if self.subgrid:
+            if f"sbgfile" not in self.config:
+                self.set_config(f"sbgfile", f"sfincs.sbg")
+            fn = self.get_config(f"sbgfile", abs_path=True)
+            self.reggrid.subgrid.save(file_name=fn, mask=self.mask)
+
+    def read_geoms(self):
+        """Read geometry files and save to `geoms` attribute.
         Known geometry files mentioned in the sfincs.inp configuration file are read,
         including: bnd/src/obs xy files and thd/weir structure files.
 
         If other geojson files are present in a "gis" subfolder folder, those are read as well.
         """
-        if not self._write:
-            self._staticgeoms = {}  # fresh start in read-only mode
+        self._assert_read_mode
         # read _GEOMS model files
         for gname in self._GEOMS.values():
             if f"{gname}file" in self.config:
                 fn = self.get_config(f"{gname}file", abs_path=True)
                 if fn is None:
                     continue
                 elif not isfile(fn):
                     self.logger.warning(f"{gname}file not found at {fn}")
                     continue
                 if gname in ["thd", "weir"]:
-                    struct = utils.read_structures(fn)
-                    gdf = utils.structures2gdf(struct, crs=self.crs)
+                    struct = utils.read_geoms(fn)
+                    gdf = utils.linestring2gdf(struct, crs=self.crs)
+                elif gname == "obs":
+                    gdf = utils.read_xyn(fn, crs=self.crs)
                 else:
                     gdf = utils.read_xy(fn, crs=self.crs)
-                self.set_staticgeoms(gdf, name=gname)
+                self.set_geoms(gdf, name=gname)
         # read additional geojson files from gis directory
         for fn in glob.glob(join(self.root, "gis", "*.geojson")):
             name = basename(fn).replace(".geojson", "")
-            gnames = [f[1] for f in self._FORCING.values() if f[1] is not None]
+            gnames = [f[1] for f in self._FORCING_1D.values() if f[1] is not None]
             skip = gnames + list(self._GEOMS.values())
             if name in skip:
                 continue
             gdf = hydromt.open_vector(fn, crs=self.crs)
-            self.set_staticgeoms(gdf, name=name)
+            self.set_geoms(gdf, name=name)
 
-    def write_staticgeoms(self):
-        """Write staticgeoms to bnd/src/obs xy files and thd/weir structure files.
+    def write_geoms(self, data_vars: Union[List, str] = None):
+        """Write geoms to bnd/src/obs xy files and thd/weir structure files.
         Filenames are based on the `config` attribute.
 
-        If `write_gis` property is True, all staticgeoms are written to geojson
+        If `write_gis` property is True, all geoms are written to geojson
         files in a "gis" subfolder.
+
+        Parameters
+        ----------
+        data_vars : list of str, optional
+            List of data variables to write, by default None (all)
+
         """
-        if not self._write:
-            raise IOError("Model opened in read-only mode")
-        if self._staticgeoms:
-            self.logger.info("Write staticgeom files")
-            for gname, gdf in self.staticgeoms.items():
-                if gname in self._GEOMS.values():
+        self._assert_write_mode
+
+        if self.geoms:
+            dvars = self._GEOMS.values()
+            if data_vars is not None:
+                dvars = [name for name in data_vars if name in self._GEOMS.values()]
+            self.logger.info("Write geom files")
+            for gname, gdf in self.geoms.items():
+                if gname in dvars:
                     if f"{gname}file" not in self.config:
                         self.set_config(f"{gname}file", f"sfincs.{gname}")
                     fn = self.get_config(f"{gname}file", abs_path=True)
                     if gname in ["thd", "weir"]:
-                        struct = utils.gdf2structures(gdf)
-                        utils.write_structures(fn, struct, stype=gname)
+                        struct = utils.gdf2linestring(gdf)
+                        utils.write_geoms(fn, struct, stype=gname)
+                    elif gname == "obs":
+                        utils.write_xyn(fn, gdf, crs=self.crs)
                     else:
                         utils.write_xy(fn, gdf, fmt="%8.2f")
+
+            # NOTE: all geoms are written to geojson files in a "gis" subfolder
             if self._write_gis:
-                self.write_vector(variables=["staticgeoms"])
+                self.write_vector(variables=["geoms"])
 
-    def write_config(self, rel_path=""):
-        """Write config to <root/config_fn>
+    def read_forcing(self, data_vars: List = None):
+        """Read forcing files and save to `forcing` attribute.
+        Known forcing files mentioned in the sfincs.inp configuration file are read,
+        including: bzs/dis/precip ascii files and the netampr netcdf file.
 
         Parameters
         ----------
-        rel_path: str, Path, optional
-            Relative path which is prepended to sfincs filenames which are not found in
-            the model root, but are found at this relative path from the root.
+        data_vars : list of str, optional
+            List of data variables to read, by default None (all)
         """
-        if self.staticmaps is None:
-            self.logger.info(
-                f"Empty model. Skip writing model configuration {self._config_fn}."
-            )
-            return
-        for key, value in self.config.items():
-            if key.endswith("file"):
-                if not isfile(join(self.root, value)):
-                    value = basename(value)
-                    if isfile(join(self.root, rel_path, value)):
-                        self.config.update({key: f"{rel_path}/{value}"})
-                    else:
-                        self.logger.error(f"{key} = {value} not found")
-        super().write_config()
+        self._assert_read_mode
+        if isinstance(data_vars, str):
+            data_vars = list(data_vars)
 
-    def read_forcing(self):
-        """Read forcing files and save to `forcing` attribute.
-        Known forcing files mentioned in the sfincs.inp configuration file are read,
-        including: bzd/dis/precip ascii files and the netampr netcdf file.
-        """
-        if not self._write:
-            # start fresh in read-only mode
-            self._forcing = {}
+        # 1D
+        dvars_1d = self._FORCING_1D
+        if data_vars is not None:
+            dvars_1d = [name for name in data_vars if name in dvars_1d]
         tref = utils.parse_datetime(self.config["tref"])
-        for name, (fname, gname) in self._FORCING.items():
-            fn = self.get_config(f"{fname}file", abs_path=True)
-            if fn is None:
-                continue
-            elif not isfile(fn):
-                self.logger.warning(f"{fname}file not found at {fn}")
-                continue
-            # read forcing
-            if "net" in fname:
-                da = xr.open_dataarray(fn, chunks={"time": 24})  # lazy
-                self.set_forcing(da, name=fname)
-
-            else:
-                df = utils.read_timeseries(fn, tref)
-                if gname is not None:  # read bzd/src locations
-                    fn_geom = self.get_config(f"{gname}file", abs_path=True)
-                    if not isfile(fn):
-                        self.logger.warning(f"{gname}file not found at {fn_geom}")
-                        continue
-                    gdf = utils.read_xy(fn_geom, crs=self.crs)
+        for name in dvars_1d:
+            ts_names, xy_name = self._FORCING_1D[name]
+            # read time series
+            da_lst = []
+            for ts_name in ts_names:
+                ts_fn = self.get_config(f"{ts_name}file", abs_path=True)
+                if ts_fn is None or not isfile(ts_fn):
+                    if ts_fn is not None:
+                        self.logger.warning(f"{ts_name}file not found at {ts_fn}")
+                    continue
+                df = utils.read_timeseries(ts_fn, tref)
+                df.index.name = "time"
+                if xy_name is not None:
+                    df.columns.name = "index"
+                    da = xr.DataArray(df, dims=("time", "index"), name=ts_name)
+                else:  # spatially uniform forcing
+                    da = xr.DataArray(df[df.columns[0]], dims=("time"), name=ts_name)
+                da_lst.append(da)
+            ds = xr.merge(da_lst[:])
+            # read xy
+            if xy_name is not None:
+                xy_fn = self.get_config(f"{xy_name}file", abs_path=True)
+                if xy_fn is None or not isfile(xy_fn):
+                    if xy_fn is not None:
+                        self.logger.warning(f"{xy_name}file not found at {xy_fn}")
+                else:
+                    gdf = utils.read_xy(xy_fn, crs=self.crs)
                     # read attribute data from gis files
-                    fn_gis = join(self.root, "gis", f"{gname}.geojson")
-                    if isfile(fn_gis):
-                        gdf1 = gpd.read_file(fn_gis)
+                    gis_fn = join(self.root, "gis", f"{xy_name}.geojson")
+                    if isfile(gis_fn):
+                        gdf1 = gpd.read_file(gis_fn)
+                        if "index" in gdf1.columns:
+                            gdf1 = gdf1.set_index("index")
+                            gdf.index = gdf1.index.values
+                            ds = ds.assign_coords(index=gdf1.index.values)
                         if np.any(gdf1.columns != "geometry"):
                             gdf = gpd.sjoin(gdf, gdf1, how="left")[gdf1.columns]
-                else:
-                    df = df[df.columns[0]]  # to series for spatially uniform forcing
-                    gdf = None
-                self.set_forcing_1d(ts=df, xy=gdf, name=name)
+                    # set locations as coordinates dataset
+                    ds = GeoDataset.from_gdf(gdf, ds, index_dim="index")
+            # save in self.forcing
+            if len(ds) > 1:
+                # keep wave forcing together
+                self.set_forcing(ds, name=name, split_dataset=False)
+            elif len(ds) > 0:
+                self.set_forcing(ds, split_dataset=True)
+
+        # 2D NETCDF format
+        dvars_2d = self._FORCING_NET
+        if data_vars is not None:
+            dvars_2d = [name for name in data_vars if name in dvars_2d]
+        for name in dvars_2d:
+            fname, rename = self._FORCING_NET[name]
+            fn = self.get_config(f"{fname}file", abs_path=True)
+            if fn is None or not isfile(fn):
+                if fn is not None:
+                    self.logger.warning(f"{name}file not found at {fn}")
+                continue
+            elif name in ["netbndbzsbzi", "netsrcdis"]:
+                ds = GeoDataset.from_netcdf(fn, crs=self.crs, chunks="auto")
+            else:
+                ds = xr.open_dataset(fn, chunks="auto")
+            rename = {k: v for k, v in rename.items() if k in ds}
+            if len(rename) > 0:
+                ds = ds.rename(rename).squeeze(drop=True)[list(rename.values())]
+                self.set_forcing(ds, split_dataset=True)
+            else:
+                logger.warning(f"No forcing variables found in {fname}file")
 
-    def write_forcing(self):
-        """Write forcing to ascii (bzd/dis/precip) and netcdf (netampr) files.
+    def write_forcing(self, data_vars: Union[List, str] = None):
+        """Write forcing to ascii or netcdf (netampr) files.
         Filenames are based on the `config` attribute.
+
+        Parameters
+        ----------
+        data_vars : list of str, optional
+            List of data variables to write, by default None (all)
         """
-        if not self._write:
-            raise IOError("Model opened in read-only mode")
-        if self._forcing:
+        self._assert_write_mode
+
+        if self.forcing:
             self.logger.info("Write forcing files")
+
             tref = utils.parse_datetime(self.config["tref"])
             # for nc files -> time in minutes since tref
             tref_str = tref.strftime("%Y-%m-%d %H:%M:%S")
+
+            # 1D timeseries + location text files
+            dvars_1d = self._FORCING_1D
+            if data_vars is not None:
+                dvars_1d = [name for name in data_vars if name in self._FORCING_1D]
+            for name in dvars_1d:
+                ts_names, xy_name = self._FORCING_1D[name]
+                if (
+                    name in self._FORCING_NET
+                    and f"{self._FORCING_NET[name][0]}file" in self.config
+                ):
+                    continue  # write NC file instead of text files
+                # work with wavespectra dataset and bzs/dis dataarray
+                if name in self.forcing and isinstance(self.forcing[name], xr.Dataset):
+                    ds = self.forcing[name]
+                else:
+                    ds = self.forcing  # dict
+                # write timeseries
+                da = None
+                for ts_name in ts_names:
+                    if ts_name not in ds or ds[ts_name].ndim > 2:
+                        continue
+                    # parse data to dataframe
+                    da = ds[ts_name].transpose("time", ...)
+                    df = da.to_pandas()
+                    # get filenames from config
+                    if f"{ts_name}file" not in self.config:
+                        self.set_config(f"{ts_name}file", f"sfincs.{ts_name}")
+                    fn = self.get_config(f"{ts_name}file", abs_path=True)
+                    # write timeseries
+                    utils.write_timeseries(fn, df, tref)
+                # write xy
+                if xy_name and da is not None:
+                    # parse data to geodataframe
+                    try:
+                        gdf = da.vector.to_gdf()
+                    except Exception:
+                        raise ValueError(f"Locations missing for {name} forcing")
+                    # get filenames from config
+                    if f"{xy_name}file" not in self.config:
+                        self.set_config(f"{xy_name}file", f"sfincs.{xy_name}")
+                    fn_xy = self.get_config(f"{xy_name}file", abs_path=True)
+                    # write xy
+                    utils.write_xy(fn_xy, gdf, fmt="%8.2f")
+                    # write geojson file to gis folder
+                    self.write_vector(variables=f"forcing.{ts_names[0]}")
+
+            # netcdf forcing
             encoding = dict(
                 time={"units": f"minutes since {tref_str}", "dtype": "float64"}
             )
-            names = {f[0]: f[1] for f in self._FORCING.values()}
-            gis_names = []
-            for fname in self._forcing:
-                if fname not in names:
-                    logger.warning(f"{fname} forcing unknown and skipped.")
+            dvars_2d = self._FORCING_NET
+            if data_vars is not None:
+                dvars_2d = [name for name in data_vars if name in self._FORCING_NET]
+            for name in dvars_2d:
+                if (
+                    name in self._FORCING_1D
+                    and f"{self._FORCING_1D[name][1]}file" in self.config
+                ):
+                    continue  # timeseries + xy file already written
+                fname, rename = self._FORCING_NET[name]
+                # combine variables and rename to output names
+                rename = {v: k for k, v in rename.items() if v in ds}
+                if len(rename) == 0:
                     continue
+                ds = xr.merge([self.forcing[v] for v in rename.keys()]).rename(rename)
+                # get filename from config
                 if f"{fname}file" not in self.config:
-                    self.set_config(f"{fname}file", f"sfincs.{fname}")
+                    self.set_config(f"{fname}file", f"{name}.nc")
                 fn = self.get_config(f"{fname}file", abs_path=True)
-                da = self._forcing[fname]
-                if "net" in fname:  # spatially distributed forcing
-                    da.to_netcdf(fn, encoding=encoding)
+                # write 1D timeseries
+                if fname in ["netbndbzsbzi", "netsrcdis"]:
+                    ds.vector.to_xy().to_netcdf(fn, encoding=encoding)
+                    # write geojson file to gis folder
+                    self.write_vector(variables=f"forcing.{list(rename.keys())[0]}")
+                # write 2D gridded timeseries
                 else:
-                    if len(da.dims) == 2:  # forcing at point locations
-                        df = da.to_series().unstack(0)
-                        gname = names[fname]
-                        if gname is None:
-                            raise ValueError(f"Locations missing for {fname}")
-                        gdf = self._forcing[fname].vector.to_gdf()
-                        if f"{gname}file" not in self.config:
-                            self.set_config(f"{gname}file", f"sfincs.{gname}")
-                        fn_xy = self.get_config(f"{gname}file", abs_path=True)
-                        utils.write_xy(fn_xy, gdf, fmt="%8.2f")
-                        gis_names.append(fname)
-                    else:  # spatially uniform forcing
-                        df = da.to_series().to_frame()
-                    utils.write_timeseries(fn, df, tref)
-            if self._write_gis and len(gis_names) > 0:
-                self.write_vector(variables=[f"forcing.{name}" for name in gis_names])
+                    ds.to_netcdf(fn, encoding=encoding)
 
-    def read_states(self, crs=None):
-        """Read waterlevel state (zsini) from ascii file and save to `states` attribute.
+    def read_states(self):
+        """Read waterlevel state (zsini) from binary file and save to `states` attribute.
         The inifile if mentioned in the sfincs.inp configuration file is read.
 
-        Parameters
-        ----------
-        crs: int, CRS
-            Coordinate reference system, if provided use instead of epsg code from sfincs.inp
         """
-        if not self._write:
-            # start fresh in read-only mode
-            self._states = {}
-        if "inifile" in self.config:
-            fn = self.get_config("inifile", abs_path=True)
-            if not isfile(fn):
-                self.logger.warning("inifile not found at {fn}")
-                return
-            shape, transform, crs = self.get_spatial_attrs(crs=crs)
-            zsini = RasterDataArray.from_numpy(
-                data=utils.read_ascii_map(fn),  # orientation S-N
-                transform=transform,
-                crs=crs,
-                nodata=-9999,  # TODO: check what a good nodatavalue is
-            )
-            if zsini.shape != shape:
-                raise ValueError('The shape of "inifile" and maps does not match.')
-            if self._MAPS["mask"] in self._staticmaps:
-                zsini = zsini.where(self.mask != 0, -9999)
-            self.set_states(zsini, "zsini")
+        self._assert_read_mode
+
+        # read index file
+        ind_fn = self.get_config("indexfile", fallback="sfincs.ind", abs_path=True)
+        if not isfile(ind_fn):
+            raise IOError(f".ind path {ind_fn} does not exist")
+
+        if self.reggrid is not None:
+            ind = self.reggrid.read_ind(ind_fn=ind_fn)
+            if "inifile" in self.config:
+                fn = self.get_config("inifile", abs_path=True)
+                if not isfile(fn):
+                    self.logger.warning("inifile not found at {fn}")
+                    return
+                zsini = self.reggrid.read_map(
+                    fn, ind, dtype="f4", mv=-9999.0, name="zsini"
+                )
 
-    def write_states(self, fmt="%8.3f"):
-        """Write waterlevel state (zsini)  to ascii map file.
+                if self.crs is not None:
+                    zsini.raster.set_crs(self.crs)
+                self.set_states(zsini, "zsini")
+
+    def write_states(self):
+        """Write waterlevel state (zsini) to binary map file.
         The filenames is based on the `config` attribute.
         """
-        if not self._write:
-            raise IOError("Model opened in read-only mode")
-        assert len(self._states) <= 1
-        for name in self._states:
+        self._assert_write_mode
+
+        name = "zsini"
+
+        if name not in self.states:
+            self.logger.warning(f"{name} not in states, skipping")
+            return
+
+        if self.reggrid and "msk" in self.grid:
+            # make sure orientation is S->N
+            ds_out = self.grid
+            if ds_out.raster.res[1] < 0:
+                ds_out = ds_out.raster.flipud()
+            mask = ds_out["msk"].values
+
+            self.logger.debug("Write binary map indices based on mask.")
+            # write index file
+            ind_fn = self.get_config("indexfile", abs_path=True)
+            self.reggrid.write_ind(ind_fn=ind_fn, mask=mask)
+
             if f"inifile" not in self.config:
                 self.set_config(f"inifile", f"sfincs.{name}")
             fn = self.get_config("inifile", abs_path=True)
-            da = self._states[name].fillna(0)  # TODO check proper nodata value
-            if da.raster.res[1] < 0:  # orientation is S->N
+            da = self.states[name]
+            if da.raster.res[1] < 0:
                 da = da.raster.flipud()
-            utils.write_ascii_map(fn, da.values, fmt=fmt)
+
+            self.logger.debug("Write binary water level state inifile")
+            self.reggrid.write_map(
+                map_fn=fn,
+                data=da.values,
+                mask=mask,
+                dtype="f4",
+            )
+
         if self._write_gis:
             self.write_raster("states")
 
     def read_results(
         self,
         chunksize=100,
         drop=["crs", "sfincsgrid"],
@@ -2137,22 +2472,27 @@
         The staggered nc file format is translated into hydromt.RasterDataArray formats.
         Additionally, hmax is computed from zsmax and zb if present.
 
         Parameters
         ----------
         chunksize: int, optional
             chunk size along time dimension, by default 100
+        drop: list, optional
+            list of variables to drop, by default ["crs", "sfincsgrid"]
+        fn_map: str, optional
+            filename of sfincs_map.nc, by default "sfincs_map.nc"
+        fn_his: str, optional
+            filename of sfincs_his.nc, by default "sfincs_his.nc"
         """
         if not isabs(fn_map):
             fn_map = join(self.root, fn_map)
         if isfile(fn_map):
             ds_face, ds_edge = utils.read_sfincs_map_results(
                 fn_map,
-                crs=self.crs,
-                chunksize=chunksize,
+                ds_like=self.grid,  # TODO: fix for quadtree
                 drop=drop,
                 logger=self.logger,
                 **kwargs,
             )
             # save as dict of DataArray
             self.set_results(ds_face, split_dataset=True)
             self.set_results(ds_edge, split_dataset=True)
@@ -2166,37 +2506,38 @@
             # drop double vars (map files has priority)
             drop_vars = [v for v in ds_his.data_vars if v in self._results or v in drop]
             ds_his = ds_his.drop_vars(drop_vars)
             self.set_results(ds_his, split_dataset=True)
 
     def write_raster(
         self,
-        variables=["staticmaps", "states", "results.hmax"],
+        variables=["grid", "states", "results.hmax"],
         root=None,
         driver="GTiff",
         compress="deflate",
         **kwargs,
     ):
         """Write model 2D raster variables to geotiff files.
 
         NOTE: these files are not used by the model by just saved for visualization/
         analysis purposes.
 
         Parameters
         ----------
         variables: str, list, optional
             Model variables are a combination of attribute and layer (optional) using <attribute>.<layer> syntax.
-            Known ratster attributes are ["staticmaps", "states", "results"].
+            Known ratster attributes are ["grid", "states", "results"].
             Different variables can be combined in a list.
-            By default, variables is ["staticmaps", "states", "results.hmax"]
+            By default, variables is ["grid", "states", "results.hmax"]
         root: Path, str, optional
             The output folder path. If None it defaults to the <model_root>/gis folder (Default)
         kwargs:
             Key-word arguments passed to hydromt.RasterDataset.to_raster(driver='GTiff', compress='lzw').
         """
+
         # check variables
         if isinstance(variables, str):
             variables = [variables]
         if not isinstance(variables, list):
             raise ValueError(f'"variables" should be a list, not {type(list)}.')
         # check root
         if root is None:
@@ -2213,40 +2554,53 @@
             self.logger.info(f"Write raster file(s) for {var} to 'gis' subfolder")
             layers = vsplit[1:] if len(vsplit) >= 2 else list(obj.keys())
             for layer in layers:
                 if layer not in obj:
                     self.logger.warning(f"Variable {attr}.{layer} not found: skipping.")
                     continue
                 da = obj[layer]
-                if len(da.dims) != 2 or "time" in da.dims:
-                    continue
+                if len(da.dims) != 2:
+                    # try to reduce to 2D by taking maximum over time dimension
+                    if "time" in da.dims:
+                        da = da.max("time")
+                    elif "timemax" in da.dims:
+                        da = da.max("timemax")
+                    # if still not 2D, skip
+                    if len(da.dims) != 2:
+                        self.logger.warning(
+                            f"Variable {attr}.{layer} has more than 2 dimensions: skipping."
+                        )
+                        continue
+                # only write active cells to gis files
+                da = da.raster.clip_geom(self.region, mask=True).raster.mask_nodata()
                 if da.raster.res[1] > 0:  # make sure orientation is N->S
                     da = da.raster.flipud()
                 da.raster.to_raster(
                     join(root, f"{layer}.tif"),
                     driver=driver,
                     compress=compress,
                     **kwargs,
                 )
 
     def write_vector(
         self,
-        variables=["staticgeoms", "forcing.bzs", "forcing.dis"],
+        variables=["geoms", "forcing.bzs", "forcing.dis"],
         root=None,
+        gdf=None,
         **kwargs,
     ):
-        """Write model vector (staticgeoms) variables to geojson files.
+        """Write model vector (geoms) variables to geojson files.
 
         NOTE: these files are not used by the model by just saved for visualization/
         analysis purposes.
 
         Parameters
         ----------
         variables: str, list, optional
-            Staticgeoms variables. By default all staticgeoms are saved.
+            geoms variables. By default all geoms are saved.
         root: Path, str, optional
             The output folder path. If None it defaults to the <model_root>/gis folder (Default)
         kwargs:
             Key-word arguments passed to geopandas.GeoDataFrame.to_file(driver='GeoJSON').
         """
         kwargs.update(driver="GeoJSON")  # fixed
         # check variables
@@ -2272,169 +2626,243 @@
                 if name not in obj:
                     self.logger.warning(f"Variable {attr}.{name} not found: skipping.")
                     continue
                 if isinstance(obj[name], gpd.GeoDataFrame):
                     gdf = obj[name]
                 else:
                     try:
-                        da = obj[name]
-                        gdf = da.vector.to_gdf()
-                        name = {f[0]: f[1] for f in self._FORCING.values()}[name]
+                        gdf = obj[name].vector.to_gdf()
+                        # xy name -> difficult!
+                        name = [
+                            v[-1] for v in self._FORCING_1D.values() if name in v[0]
+                        ][0]
                     except:
                         self.logger.debug(
                             f"Variable {attr}.{name} could not be written to vector file."
                         )
                         pass
                 gdf.to_file(join(root, f"{name}.geojson"), **kwargs)
 
-    def set_staticmaps(self, data, name=None):
-        """Add data to staticmaps.
-
-        All layers of staticmaps must have identical spatial coordinates.
+    ## model configuration
 
-        Parameters
-        ----------
-        data: xarray.DataArray or xarray.Dataset
-            new map layer to add to staticmaps
-        name: str, optional
-            Name of new map layer, this is used to overwrite the name of a DataArray
-            or to select a variable from a Dataset.
-        """
-        # make sure data has N->S orientation to easily work with hydrography data
-        if isinstance(data, (xr.Dataset, xr.DataArray)) and data.raster.res[1] > 0:
-            data = data.raster.flipud()
-        super().set_staticmaps(data, name)
-
-    def set_forcing_1d(self, name, ts=None, xy=None):
-        """Set 1D forcing and update staticgoms and config accordingly.
-
-        For waterlevel and discharge forcing point locations are required to set the
-        combined src/dis and bnd/bzs files. If only point locations (and no timeseries)
-        are given a dummy timeseries with zero values is set.
-
-        If ts and xy are both None, the
+    def read_config(self, config_fn: str = "sfincs.inp", epsg: int = None) -> None:
+        """Parse config from SFINCS input file.
+        If in write-only mode the config is initialized with default settings.
 
         Parameters
         ----------
-        name: {'waterlevel', 'discharge', 'precip'}
-            Name of forcing type.
-        ts: pandas.DataFrame, xarray.DataArray
-            Timeseries data. If DataArray it should contain time and index dims; if
-            DataFrame the index should be a datetime index and the columns the location
-            index.
-        xy: geopandas.GeoDataFrame
-            Forcing point locations
-        """
-        fname, gname = self._FORCING.get(name, (None, None))
-        if fname is None:
-            names = [f[0] for f in self._FORCING.values() if "net" not in f[0]]
-            raise ValueError(f'Unknown forcing "{name}", select from {names}')
-        # sort out ts and xy types
-        if isinstance(ts, (pd.DataFrame, pd.Series)):
-            assert np.dtype(ts.index).type == np.datetime64
-            ts.index.name = "time"
-            if isinstance(ts, pd.DataFrame):
-                ts.columns.name = "index"
-                ts = xr.DataArray(ts, dims=("time", "index"), name=fname)
-            else:  # spatially uniform forcing
-                ts = xr.DataArray(ts, dims=("time"), name=fname)
-        if isinstance(xy, gpd.GeoDataFrame):
-            if ts is not None:
-                ts = GeoDataArray.from_gdf(xy, ts, index_dim="index")
-            else:
-                ts = self._dummy_ts(xy, name, fill_value=0)  # dummy timeseries
-            for c in xy.columns:
-                if c in ["geometry", ts.vector.index_dim]:
-                    continue
-                ts[c] = xr.IndexVariable("index", xy[c].values)
-        if not isinstance(ts, xr.DataArray):
-            raise ValueError(
-                f"{name} forcing: Unknown type for ts {type(ts)} should be xarray.DataArray."
-            )
-        # check if locations (bzs / dis)
-        if gname is not None:
-            assert len(ts.dims) == 2
-            # make sure time is on last dim
-            ts = ts.transpose(ts.vector.index_dim, ts.vector.time_dim)
-            # set crs
-            if ts.vector.crs is None:
-                ts.vector.set_crs(self.crs.to_epsg())
-            elif ts.vector.crs != self.crs:
-                ts = ts.vector.to_crs(self.crs.to_epsg())
-            # fix order based on x_dim after setting crs (for comparability between OS)
-            ts = ts.sortby([ts.vector.x_dim, ts.vector.y_dim], ascending=True)
-            # reset index
-            dim = ts.vector.index_dim
-            ts[dim] = xr.IndexVariable(dim, np.arange(1, ts[dim].size + 1, dtype=int))
-            n = ts.vector.index.size
-            self.logger.debug(f"{name} forcing: setting {gname} data for {n} points.")
-        else:
-            if not (len(ts.dims) == 1 and "time" in ts.dims):
-                raise ValueError(
-                    f"{name} forcing: uniform forcing should have single 'time' dimension."
+        config_fn: str
+            Filename of config file, by default "sfincs.inp".
+            If in a different folder than the model root, the root is updated.
+        epsg: int
+            EPSG code of the model CRS. Only used if missing in the SFINCS input file, by default None.
+        """
+        inp = SfincsInput()  # initialize with defaults
+        if self._read:  # in read-only or append mode, try reading config_fn
+            if not isfile(config_fn) and not isabs(config_fn) and self._root:
+                # path relative to self.root
+                config_fn = abspath(join(self.root, config_fn))
+            elif isfile(config_fn) and abspath(dirname(config_fn)) != self._root:
+                # new root
+                mode = (
+                    "r+"
+                    if self._write and self._read
+                    else ("w" if self._write else "r")
                 )
+                root = abspath(dirname(config_fn))
+                self.logger.warning(f"updating the model root to: {root}")
+                self.set_root(root=root, mode=mode)
+            else:
+                raise IOError(f"SFINCS input file not found {config_fn}")
+            # read config_fn
+            inp.read(inp_fn=config_fn)
+        # overwrite / initialize config attribute
+        self._config = inp.to_dict()
+        if epsg is not None and "epsg" not in self.config:
+            self.config.update(epsg=epsg)
+        self.update_grid_from_config()  # update grid properties based on sfincs.inp
+
+    def write_config(self, config_fn: str = "sfincs.inp"):
+        """Write config to <root/config_fn>"""
+        self._assert_write_mode
+        if not isabs(config_fn) and self._root:
+            config_fn = join(self.root, config_fn)
 
-        # set forcing
-        self.logger.debug(f"{name} forcing: setting {fname} data.")
-        ts.attrs.update(**self._ATTRS.get(fname, {}))
-        self.set_forcing(ts, fname)
-
-    ## model configuration
-
-    def set_crs(self, crs):
-        super(SfincsModel, self).set_crs(crs)
-        self.update_spatial_attrs()
-
-    def _configread(self, fn):
-        return utils.read_inp(fn)
-
-    def _configwrite(self, fn):
-        return utils.write_inp(fn, self.config)
+        inp = SfincsInput.from_dict(self.config)
+        inp.write(inp_fn=abspath(config_fn))
 
     def update_spatial_attrs(self):
-        """Update geospatial `config` (sfincs.inp) attributes based on staticmaps"""
+        """Update geospatial `config` (sfincs.inp) attributes based on grid"""
         dx, dy = self.res
+        # TODO check self.bounds with rotation!! origin not necessary equal to total_bounds
         west, south, _, _ = self.bounds
         if self.crs is not None:
             self.set_config("epsg", self.crs.to_epsg())
         self.set_config("mmax", self.width)
         self.set_config("nmax", self.height)
         self.set_config("dx", dx)
         self.set_config("dy", abs(dy))  # dy is always positive (orientation is S -> N)
         self.set_config("x0", west)
         self.set_config("y0", south)
 
-    def get_spatial_attrs(self, crs=None):
-        """Get geospatial `config` (sfincs.inp) attributes.
-
-        Parameters
-        ----------
-        crs: int, CRS
-            Coordinate reference system
-
-        Returns
-        -------
-        shape: tuple of int
-            width, height
-        transform: Affine.transform
-            Geospatial transform
-        crs: pyproj.CRS
-            Coordinate reference system
-        """
-        return utils.get_spatial_attrs(self.config, crs=crs, logger=self.logger)
+    def update_grid_from_config(self):
+        """Update grid properties based on `config` (sfincs.inp) attributes"""
+        self.grid_type = (
+            "quadtree" if self.config.get("qtrfile") is not None else "regular"
+        )
+        if self.grid_type == "regular":
+            self.reggrid = RegularGrid(
+                x0=self.config.get("x0"),
+                y0=self.config.get("y0"),
+                dx=self.config.get("dx"),
+                dy=self.config.get("dy"),
+                nmax=self.config.get("nmax"),
+                mmax=self.config.get("mmax"),
+                rotation=self.config.get("rotation", 0),
+                epsg=self.config.get("epsg"),
+            )
+        else:
+            raise not NotImplementedError("Quadtree grid not implemented yet")
+            # self.quadtree = QuadtreeGrid()
 
     def get_model_time(self):
         """Return (tstart, tstop) tuple with parsed model start and end time"""
         tstart = utils.parse_datetime(self.config["tstart"])
         tstop = utils.parse_datetime(self.config["tstop"])
         return tstart, tstop
 
     ## helper method
 
-    def _dummy_ts(self, gdf, name, fill_value=0):
-        df = pd.DataFrame(
-            index=pd.DatetimeIndex(list(self.get_model_time())),
-            columns=gdf.index.values,
-            data=np.full((2, gdf.index.size), fill_value, dtype=np.float32),
-        )
-        ts = GeoDataArray.from_gdf(gdf, df, dims=("time", "index"), name=name)
-        return ts
+    def _parse_datasets_dep(self, datasets_dep, res):
+        """Parse filenames or paths of Datasets in list of dictionaries datasets_dep into xr.DataArray and gdf.GeoDataFrames:
+        * "elevtn" is parsed into da (xr.DataArray)
+        * "offset" is parsed into da_offset (xr.DataArray)
+        * "mask" is parsed into gdf (gpd.GeoDataFrame)
+
+        Parameters
+        ----------
+        datasets_dep : List[dict]
+            List of dictionaries with topobathy data, each containing a dataset name or Path (dep) and optional merge arguments.
+        res : float
+            Resolution of the model grid in meters. Used to obtain the correct zoom level of the depth datasets.
+        """
+        parse_keys = ["elevtn", "offset", "mask", "da"]
+        copy_keys = ["zmin", "zmax", "reproj_method", "merge_method"]
+
+        datasets_out = []
+        for dataset in datasets_dep:
+            dd = {}
+            # read in depth datasets; replace dep (source name; filename or xr.DataArray)
+            if "elevtn" in dataset or "da" in dataset:
+                try:
+                    da_elv = self.data_catalog.get_rasterdataset(
+                        dataset.get("elevtn", dataset.get("da")),
+                        geom=self.mask.raster.box,
+                        buffer=10,
+                        variables=["elevtn"],
+                        zoom_level=(res, "meter"),
+                    )
+                    dd.update({"da": da_elv})
+                except:
+                    data_name = dataset.get("elevtn")
+                    self.logger.warning(
+                        f"{data_name} not used; probably because all the data is outside of the mask."
+                    )
+                    continue
+            else:
+                raise ValueError(
+                    "No 'elevtn' (topobathy) dataset provided in datasets_dep."
+                )
+
+            # read offset filenames
+            # NOTE offsets can be xr.DataArrays and floats
+            if "offset" in dataset and not isinstance(dataset["offset"], (float, int)):
+                da_offset = self.data_catalog.get_rasterdataset(
+                    dataset.get("offset"),
+                    geom=self.mask.raster.box,
+                    buffer=20,
+                )
+                dd.update({"offset": da_offset})
+
+            # read geodataframes describing valid areas
+            if "mask" in dataset:
+                gdf_valid = self.data_catalog.get_geodataframe(
+                    path_or_key=dataset.get("mask"),
+                    geom=self.mask.raster.box,
+                )
+                dd.update({"gdf_valid": gdf_valid})
+
+            # copy remaining keys
+            for key, value in dataset.items():
+                if key in copy_keys and key not in dd:
+                    dd.update({key: value})
+                elif key not in copy_keys + parse_keys:
+                    self.logger.warning(f"Unknown key {key} in datasets_dep. Ignoring.")
+            datasets_out.append(dd)
+
+        return datasets_out
+
+    def _parse_datasets_rgh(self, datasets_rgh):
+        """Parse filenames or paths of Datasets in list of dictionaries datasets_rgh into xr.DataArrays and gdf.GeoDataFrames:
+        * "manning" is parsed into da (xr.DataArray)
+        * "lulc" is parsed into da (xr.DataArray) using reclassify table in "reclass_table"
+        * "mask" is parsed into gdf_valid (gpd.GeoDataFrame)
+
+        Parameters
+        ----------
+        datasets_rgh : List[dict], optional
+            List of dictionaries with Manning's n datasets. Each dictionary should at least contain one of the following:
+            * (1) manning: filename (or Path) of gridded data with manning values
+            * (2) lulc (and reclass_table) :a combination of a filename of gridded landuse/landcover and a reclassify table.
+            In additon, optional merge arguments can be provided e.g.: merge_method, mask
+        """
+        parse_keys = ["manning", "lulc", "reclass_table", "mask", "da"]
+        copy_keys = ["reproj_method", "merge_method"]
+
+        datasets_out = []
+        for dataset in datasets_rgh:
+            dd = {}
+
+            if "manning" in dataset or "da" in dataset:
+                da_man = self.data_catalog.get_rasterdataset(
+                    dataset.get("manning", dataset.get("da")),
+                    geom=self.mask.raster.box,
+                    buffer=10,
+                )
+                dd.update({"da": da_man})
+            elif "lulc" in dataset:
+                # landuse/landcover should always be combined with mapping
+                lulc = dataset.get("lulc")
+                reclass_table = dataset.get("reclass_table", None)
+                if reclass_table is None and isinstance(lulc, str):
+                    reclass_table = join(DATADIR, "lulc", f"{lulc}_mapping.csv")
+                if not os.path.isfile(reclass_table) and isinstance(lulc, str):
+                    raise IOError(
+                        f"Manning roughness mapping file not found: {reclass_table}"
+                    )
+                da_lulc = self.data_catalog.get_rasterdataset(
+                    lulc, geom=self.mask.raster.box, buffer=10, variables=["lulc"]
+                )
+                df_map = self.data_catalog.get_dataframe(reclass_table, index_col=0)
+                # reclassify
+                da_man = da_lulc.raster.reclassify(df_map[["N"]])["N"]
+                dd.update({"da": da_man})
+            else:
+                raise ValueError("No 'manning' dataset provided in datasets_rgh.")
+
+            # read geodataframes describing valid areas
+            if "mask" in dataset:
+                gdf_valid = self.data_catalog.get_geodataframe(
+                    path_or_key=dataset.get("mask"),
+                    geom=self.mask.raster.box,
+                )
+                dd.update({"gdf_valid": gdf_valid})
+
+            # copy remaining keys
+            for key, value in dataset.items():
+                if key in copy_keys and key not in dd:
+                    dd.update({key: value})
+                elif key not in copy_keys + parse_keys:
+                    self.logger.warning(f"Unknown key {key} in datasets_rgh. Ignoring.")
+            datasets_out.append(dd)
+
+        return datasets_out
```

### Comparing `hydromt_sfincs-0.2.1/hydromt_sfincs/workflows/discharge.py` & `hydromt_sfincs-1.0.0/hydromt_sfincs/workflows/discharge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+"""Workflows for discharge boundary conditions."""
+import logging
+
 import geopandas as gpd
 import numpy as np
 import xarray as xr
-import logging
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "snap_discharge",
 ]
 
@@ -32,44 +34,55 @@
         Dataset with discharge and optional uparea variable.
     gdf: geopandas.GeoDataFrame[Points]
         Dataframe with Point geometries of locations of interest.
     wdw: int, optional
         Window size in number of cells around discharge boundary locations
         to snap to, only used if ``uparea_fn`` is provided. By default 1.
     rel_error, abs_error: float, optional
-        Maximum relative error (defualt 0.05) and absolute error (default 50 km2)
+        Maximum relative error (default 0.05) and absolute error (default 50 km2)
         between the discharge boundary location upstream area and the upstream area of
         the best fit grid cell, only used if "discharge" staticgeoms has a "uparea" column.
 
     Returns
     -------
-    da_q: xarray.DataArray
-        DataArray with snapped discharge values per valid point location.
+    ds: xarray.Dataset
+        snapped dataset
     """
+    ds_wdw = ds.raster.sample(gdf, wdw=wdw)
+    # check if valid discharge
+    valid = ds_wdw[discharge_name].notnull().any("time")
     if uparea_name in ds and uparea_name in gdf.columns:
-        ds_wdw = ds.raster.sample(gdf, wdw=wdw)
         logger.debug(
             f"Snapping {discharge_name} points to best matching uparea cell within wdw (size={wdw})."
         )
         upa0 = xr.DataArray(gdf[uparea_name], dims=("index"))
         upa_dff = np.abs(
             ds_wdw[uparea_name].where(ds_wdw[uparea_name] > 0).load() - upa0
         )
-        valid = np.logical_or((upa_dff / upa0) <= rel_error, upa_dff <= abs_error)
+        upa_check = np.logical_or((upa_dff / upa0) <= rel_error, upa_dff <= abs_error)
+        valid = np.logical_and(valid, upa_check)
         # combine valid local cells with best matching windows cells if local cell invalid
-        i_loc = int((1 + 2 * wdw) ** 2 / 2)
-        i_wdw = upa_dff.argmin("wdw").where(~valid.isel(wdw=i_loc), i_loc)
-        idx_valid = np.where(valid.isel(wdw=i_wdw))[0]
-        if idx_valid.size < gdf.index.size:
-            logger.warning(
-                f"{idx_valid.size}/{gdf.index.size} {discharge_name} points succesfully snapped."
-            )
-        i_wdw = i_wdw.isel(index=idx_valid)
-        ds_out = ds_wdw.isel(wdw=i_wdw.load(), index=idx_valid)
+        # i_loc = int((1 + 2 * wdw) ** 2 / 2)  # center cell
+        # i_wdw = upa_dff.argmin("wdw").where(~valid.isel(wdw=i_loc), i_loc).load()
+        # find best matching uparea cell in window
+        i_wdw = upa_dff.argmin("wdw").load()
     else:
         logger.debug(
             f"No {uparea_name} variable found in ds or gdf; "
             f"sampling {discharge_name} points from nearest grid cell."
         )
-        ds_out = ds.raster.sample(gdf)
+        # add distance (measured in cells)
+        ar_wdw = np.abs(np.arange(-wdw, wdw + 1))
+        dist = np.hypot(**np.meshgrid(ar_wdw, ar_wdw)).ravel()
+        ds_wdw["dist"] = xr.Variable(
+            ("index", "wdw"), np.tile(dist, (ds_wdw["index"].size, 1))
+        )
+        i_wdw = ds_wdw["dist"].where(valid, np.inf).argmin("wdw").load()
+    idx_valid = np.where(valid.isel(wdw=i_wdw).values)[0]
+    if idx_valid.size < gdf.index.size:
+        logger.warning(
+            f"{idx_valid.size}/{gdf.index.size} {discharge_name} points successfully snapped."
+        )
+    i_wdw = i_wdw.isel(index=idx_valid)
+    ds_out = ds_wdw.isel(wdw=i_wdw.load(), index=idx_valid)
 
-    return ds_out.reset_coords()[discharge_name]
+    return ds_out  # .reset_coords()[discharge_name]
```

### Comparing `hydromt_sfincs-0.2.1/pyproject.toml` & `hydromt_sfincs-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [build-system]
-requires = ["flit_core >=3.2.0,<3.3"]
+requires = ["flit_core >=3.4.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "hydromt_sfincs"
 authors = [
+    {name = "Roel de Goede", email = "roel.degoede@deltares.nl"},
+    {name = "Maarten van Ormondt", email = "Maarten.vanOrmondt@deltares-usa.us"},
     {name = "Dirk Eilander", email = "dirk.eilander@deltares.nl"},
     {name = "Tim Leijnse", email = "tim.leijnse@deltares.nl"},
 ]
 dependencies = [
-    "dask",
-    "geopandas >=0.8",
-    "hydromt>=0.4.5",
-    "netcdf4",
+    "affine",
+    "geopandas>=0.8",
+    "hydromt>=0.7.1",
+    "numba",
     "numpy",
     "pandas",
+    "pillow",
     "pyflwdir>=0.5.5",
-    "pygeos",
+    "pyproj",
     "rasterio",
     "scipy",
+    "shapely",
     "xarray",
 ]
 requires-python = ">=3.8" # fix tests to support older versions
 readme = "README.rst"
 classifiers = [
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     "Development Status :: 4 - Beta",
@@ -32,23 +36,30 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ['version', 'description']
 
 [project.optional-dependencies]
 test = [
-	"testpath",
-	"responses",
+	"black",
 	"pytest>=2.7.3",
 	"pytest-cov",
-	"black",
 ]
 doc = [
+    "nbsphinx",
+	"pydata-sphinx-theme",
 	"sphinx",
-	"sphinx_rtd_theme",
+]
+full = [
+    "cartopy",
+    "descartes",
+    "ffmpeg",
+    "jupyterlab",
+    "matplotlib",
+    "pillow",
 ]
 
 [project.urls]
 Documentation = "https://deltares.github.io/hydromt_sfincs/"
 Source = "https://github.com/Deltares/hydromt_sfincs"
 
 [project.entry-points."hydromt.models"]
```

