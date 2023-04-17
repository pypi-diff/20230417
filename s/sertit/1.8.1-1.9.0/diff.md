# Comparing `tmp/sertit-1.8.1.tar.gz` & `tmp/sertit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sertit-1.8.1.tar", last modified: Wed Sep 22 16:21:16 2021, max compression
+gzip compressed data, was "dist/sertit-1.9.0.tar", last modified: Tue Sep 28 12:39:51 2021, max compression
```

## Comparing `sertit-1.8.1.tar` & `sertit-1.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-22 16:21:16.000000 sertit-1.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    10166 2021-09-22 16:20:08.000000 sertit-1.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       84 2021-09-22 16:20:08.000000 sertit-1.8.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1569 2021-09-22 16:20:08.000000 sertit-1.8.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5372 2021-09-22 16:21:16.000000 sertit-1.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4094 2021-09-22 16:20:08.000000 sertit-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-22 16:21:16.000000 sertit-1.8.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      581 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-22 16:21:16.000000 sertit-1.8.1/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)     1559 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     1988 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/_static/favicon.png
--rw-rw-rw-   0 root         (0) root         (0)    46486 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/_static/sertit_utils.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-22 16:21:16.000000 sertit-1.8.1/docs/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      578 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/_templates/custom-class-template.rst
--rw-rw-rw-   0 root         (0) root         (0)     1203 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/_templates/custom-module-template.rst
--rw-rw-rw-   0 root         (0) root         (0)     6849 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-22 16:21:16.000000 sertit-1.8.1/docs/sertit/
--rw-rw-rw-   0 root         (0) root         (0)    19299 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/sertit/index.html
--rw-rw-rw-   0 root         (0) root         (0)   139170 2021-09-22 16:20:08.000000 sertit-1.8.1/docs/sertit/rasters.html
--rw-rw-rw-   0 root         (0) root         (0)      285 2021-09-22 16:20:08.000000 sertit-1.8.1/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-22 16:21:16.000000 sertit-1.8.1/sertit/
--rw-rw-rw-   0 root         (0) root         (0)     1227 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2114 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/arcpy.py
--rw-rw-rw-   0 root         (0) root         (0)    10199 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     2686 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/display.py
--rw-rw-rw-   0 root         (0) root         (0)    34351 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/files.py
--rw-rw-rw-   0 root         (0) root         (0)     9629 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/logs.py
--rw-rw-rw-   0 root         (0) root         (0)    11019 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     6319 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/network.py
--rw-rw-rw-   0 root         (0) root         (0)    44222 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/rasters.py
--rw-rw-rw-   0 root         (0) root         (0)    41753 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/rasters_rio.py
--rw-rw-rw-   0 root         (0) root         (0)     3966 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/snap.py
--rw-rw-rw-   0 root         (0) root         (0)     9967 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/strings.py
--rw-rw-rw-   0 root         (0) root         (0)    17002 2021-09-22 16:20:08.000000 sertit-1.8.1/sertit/vectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-22 16:21:16.000000 sertit-1.8.1/sertit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5372 2021-09-22 16:21:16.000000 sertit-1.8.1/sertit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      695 2021-09-22 16:21:16.000000 sertit-1.8.1/sertit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-22 16:21:16.000000 sertit-1.8.1/sertit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      330 2021-09-22 16:21:16.000000 sertit-1.8.1/sertit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-09-22 16:21:16.000000 sertit-1.8.1/sertit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      290 2021-09-22 16:21:16.000000 sertit-1.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2079 2021-09-22 16:20:08.000000 sertit-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-28 12:39:51.000000 sertit-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    10166 2021-06-28 12:53:17.000000 sertit-1.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       84 2021-06-28 12:53:17.000000 sertit-1.9.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2021-06-28 12:53:17.000000 sertit-1.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5372 2021-09-28 12:39:51.000000 sertit-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2021-09-20 04:14:12.000000 sertit-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-28 12:39:51.000000 sertit-1.9.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      581 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-28 12:39:51.000000 sertit-1.9.0/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/_static/favicon.png
+-rw-rw-rw-   0 root         (0) root         (0)    46486 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/_static/sertit_utils.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-28 12:39:51.000000 sertit-1.9.0/docs/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      578 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/_templates/custom-class-template.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/_templates/custom-module-template.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6849 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-28 12:39:51.000000 sertit-1.9.0/docs/sertit/
+-rw-rw-rw-   0 root         (0) root         (0)    19299 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/sertit/index.html
+-rw-rw-rw-   0 root         (0) root         (0)   139170 2021-09-20 04:14:12.000000 sertit-1.9.0/docs/sertit/rasters.html
+-rw-rw-rw-   0 root         (0) root         (0)      285 2021-08-26 08:24:49.000000 sertit-1.9.0/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-28 12:39:51.000000 sertit-1.9.0/sertit/
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2021-09-28 12:39:16.000000 sertit-1.9.0/sertit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2021-09-06 03:20:38.000000 sertit-1.9.0/sertit/arcpy.py
+-rw-rw-rw-   0 root         (0) root         (0)    10199 2021-09-20 04:14:12.000000 sertit-1.9.0/sertit/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     2686 2021-06-28 12:53:17.000000 sertit-1.9.0/sertit/display.py
+-rw-rw-rw-   0 root         (0) root         (0)    34351 2021-09-22 16:17:08.000000 sertit-1.9.0/sertit/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     9629 2021-09-20 04:14:12.000000 sertit-1.9.0/sertit/logs.py
+-rw-rw-rw-   0 root         (0) root         (0)    11019 2021-09-20 04:14:12.000000 sertit-1.9.0/sertit/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6319 2021-06-28 12:53:17.000000 sertit-1.9.0/sertit/network.py
+-rw-rw-rw-   0 root         (0) root         (0)    45683 2021-09-28 12:39:16.000000 sertit-1.9.0/sertit/rasters.py
+-rw-rw-rw-   0 root         (0) root         (0)    46567 2021-09-28 12:39:16.000000 sertit-1.9.0/sertit/rasters_rio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2021-09-20 04:14:12.000000 sertit-1.9.0/sertit/snap.py
+-rw-rw-rw-   0 root         (0) root         (0)     9967 2021-09-20 04:14:12.000000 sertit-1.9.0/sertit/strings.py
+-rw-rw-rw-   0 root         (0) root         (0)    17002 2021-09-20 04:14:12.000000 sertit-1.9.0/sertit/vectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-28 12:39:51.000000 sertit-1.9.0/sertit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5372 2021-09-28 12:39:51.000000 sertit-1.9.0/sertit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      695 2021-09-28 12:39:51.000000 sertit-1.9.0/sertit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-28 12:39:51.000000 sertit-1.9.0/sertit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      330 2021-09-28 12:39:51.000000 sertit-1.9.0/sertit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-09-28 12:39:51.000000 sertit-1.9.0/sertit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      290 2021-09-28 12:39:51.000000 sertit-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2021-09-20 04:14:12.000000 sertit-1.9.0/setup.py
```

### Comparing `sertit-1.8.1/LICENSE` & `sertit-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/NOTICE` & `sertit-1.9.0/NOTICE`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/PKG-INFO` & `sertit-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sertit
-Version: 1.8.1
+Version: 1.9.0
 Summary: ('SERTIT python library for generic tools',)
 Home-page: UNKNOWN
 Author: ICube-SERTIT
 Author-email: dev-sertit@unistra.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sertit/sertit-utils/issues/
 Project-URL: Documentation, https://sertit-utils.readthedocs.io/en/latest/
```

### Comparing `sertit-1.8.1/README.md` & `sertit-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/Makefile` & `sertit-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/_static/custom.css` & `sertit-1.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/_static/favicon.png` & `sertit-1.9.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/_static/sertit_utils.png` & `sertit-1.9.0/docs/_static/sertit_utils.png`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/_templates/custom-class-template.rst` & `sertit-1.9.0/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/_templates/custom-module-template.rst` & `sertit-1.9.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/conf.py` & `sertit-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/sertit/index.html` & `sertit-1.9.0/docs/sertit/index.html`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/docs/sertit/rasters.html` & `sertit-1.9.0/docs/sertit/rasters.html`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/__init__.py` & `sertit-1.9.0/sertit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # limitations under the License.
 """
 **Source Code**: https://github.com/sertit/sertit-utils
 
 .. include:: ../README.md
 """
 
-__version__ = "1.8.1"
+__version__ = "1.9.0"
 __title__ = "sertit"
 __description__ = ("SERTIT python library for generic tools",)
 __author__ = "ICube-SERTIT"
 __author_email__ = "dev-sertit@unistra.fr"
 __url__ = "https://github.com/sertit/sertit-utils"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2021, SERTIT-ICube - France, https://sertit.unistra.fr/"
```

### Comparing `sertit-1.8.1/sertit/arcpy.py` & `sertit-1.9.0/sertit/arcpy.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/ci.py` & `sertit-1.9.0/sertit/ci.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/display.py` & `sertit-1.9.0/sertit/display.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/files.py` & `sertit-1.9.0/sertit/files.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/logs.py` & `sertit-1.9.0/sertit/logs.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/misc.py` & `sertit-1.9.0/sertit/misc.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/network.py` & `sertit-1.9.0/sertit/network.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/rasters.py` & `sertit-1.9.0/sertit/rasters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1302,7 +1302,55 @@
         # Set nodata to nan
         where_xda = where_xda.where(~np.isnan(master_xda))
 
         # Set mtd
         where_xda = set_metadata(where_xda, master_xda, new_name=new_name)
 
     return where_xda
+
+
+@path_xarr_dst
+def hillshade(xds: PATH_XARR_DS, azimuth: float = 315, zenith: float = 45) -> XDS_TYPE:
+    """
+    Compute the hillshade of a DEM from an azimuth and elevation angle (in degrees).
+
+    Goal: replace `gdaldem` CLI (https://gdal.org/programs/gdaldem.html)
+
+    NB: altitude = zenith
+
+    Reference:
+    - https://www.neonscience.org/resources/learning-hub/tutorials/create-hillshade-py
+    - http://webhelp.esri.com/arcgisdesktop/9.2/index.cfm?TopicName=How%20Hillshade%20works
+
+    Args:
+        dst (PATH_XARR_DS): Path to the raster, its dataset, its `xarray` or a tuple containing its array and metadata
+        azimuth (float): Azimuth angle in degrees
+        zenith (float): Zenith angle in degrees
+
+    Returns:
+        XDS_TYPE: Hillshade
+    """
+    # Use classic option
+    arr, meta = rasters_rio.hillshade(xds, azimuth=azimuth, zenith=zenith)
+
+    return xds.copy(data=arr)
+
+
+@path_xarr_dst
+def slope(xds: PATH_XARR_DS, in_pct: bool = False, in_rad: bool = False) -> XDS_TYPE:
+    """
+    Compute the slope of a DEM (in degrees).
+
+    Goal: replace `gdaldem` CLI (https://gdal.org/programs/gdaldem.html)
+
+    NB: altitude = zenith
+
+    Args:
+        dst (PATH_XARR_DS): Path to the raster, its dataset, its `xarray` or a tuple containing its array and metadata
+
+    Returns:
+        XDS_TYPE: Slope
+    """
+    # Use classic option
+    arr, meta = rasters_rio.slope(xds, in_pct=in_pct, in_rad=in_rad)
+
+    return xds.copy(data=arr)
```

### Comparing `sertit-1.8.1/sertit/rasters_rio.py` & `sertit-1.9.0/sertit/rasters_rio.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,18 +41,22 @@
 except ModuleNotFoundError as ex:
     raise ModuleNotFoundError(
         "Please install 'rasterio' and 'geopandas' to use the 'rasters_rio' package."
     ) from ex
 
 from sertit import files, misc, strings, vectors
 
+np.seterr(divide="ignore", invalid="ignore")
+
 MAX_CORES = os.cpu_count() - 2
 PATH_ARR_DS = Union[str, tuple, rasterio.DatasetReader]
 LOGGER = logging.getLogger(SU_NAME)
 
+DEG_2_RAD = np.pi / 180
+
 """
 Types:
 
 - Path
 - Rasterio open data: (array, meta)
 - rasterio Dataset
 - `xarray`
@@ -1259,7 +1263,160 @@
     # Only keep the bit number bit_id and reshape the vector
     if isinstance(bit_id, list):
         bit_arr = [msk[..., bid] for bid in bit_id]
     else:
         bit_arr = msk[..., bit_id]
 
     return bit_arr
+
+
+@path_arr_dst
+def hillshade(
+    dst: PATH_ARR_DS, azimuth: float = 315, zenith: float = 45
+) -> (np.ma.masked_array, dict):
+    """
+    Compute the hillshade of a DEM from an azimuth and elevation angle (in degrees).
+
+    Goal: replace `gdaldem` CLI (https://gdal.org/programs/gdaldem.html)
+
+    NB: altitude = 90 - zenith
+
+    .. WARNING::
+
+        - It uses a 2nd order gradient instead of Horn's or Zevenbergen & Thorne's formula
+        - z_factor is fixed to 1.0
+        - scale managed by dst resolution
+
+    Reference:
+    - https://git.earthdata.nasa.gov/projects/GEE/repos/gdal-enhancements-for-esdis/browse/gdal-1.10.0/apps/gdaldem.cpp
+
+    Args:
+        dst (PATH_ARR_DS): Path to the raster, its dataset, its `xarray` or a tuple containing its array and metadata
+        azimuth (float): Azimuth angle in degrees
+        zenith (float): Zenith angle in degrees
+
+    Returns:
+        (np.ma.masked_array, dict): Hillshade and its metadata
+    """
+    array = dst.read(masked=True)
+
+    # Squeeze if needed
+    expand = False
+    if len(array.shape) == 3 and array.shape[0] == 1:
+        array = np.squeeze(array)  # Use this trick to make the sieve work
+        expand = True
+
+    # Compute angles
+    az_rad = azimuth * DEG_2_RAD
+    alt_rad = (90 - zenith) * DEG_2_RAD
+
+    # Compute slope and aspect
+    dx, dy = np.gradient(np.where(array.mask, 0.0, array.data), *dst.res)
+    x2_y2 = dx ** 2 + dy ** 2
+    aspect = np.arctan2(dx, dy)
+
+    # Compute hillshade (GDAL algo)
+    hillshade = (
+        np.sin(alt_rad) + np.cos(alt_rad) * np.sqrt(x2_y2) * np.sin(aspect - az_rad)
+    ) / np.sqrt(1 + x2_y2)
+    hillshade = np.where(hillshade <= 0, 1.0, 254.0 * hillshade + 1)
+
+    # Use this trick to get the array back to 'normal'
+    if expand:
+        hillshade = np.expand_dims(hillshade, axis=0)
+
+    # Convert to masked array
+    hillshade_msk = np.ma.masked_array(hillshade, array.mask, fill_value=dst.nodata)
+
+    # Meta
+    meta = update_meta(hillshade_msk, dst.meta)
+
+    return hillshade_msk, meta
+
+
+@path_arr_dst
+def slope(
+    dst: PATH_ARR_DS,
+    in_pct: bool = False,
+    in_rad: bool = False,
+) -> (np.ma.masked_array, dict):
+    """
+    Compute the slope of a DEM (in degrees).
+
+    Goal: replace `gdaldem` CLI (https://gdal.org/programs/gdaldem.html)
+
+    .. WARNING::
+
+        - It uses a 2nd order gradient instead of Horn's or Zevenbergen & Thorne's formula
+        - z_factor is fixed to 1.0
+        - scale managed by dst resolution
+
+    Reference:
+    - https://git.earthdata.nasa.gov/projects/GEE/repos/gdal-enhancements-for-esdis/browse/gdal-1.10.0/apps/gdaldem.cpp
+
+    Args:
+        dst (PATH_ARR_DS): Path to the raster, its dataset, its `xarray` or a tuple containing its array and metadata
+        in_pct (bool): Outputs slope in percents
+        in_rad (bool): Outputs slope in radians. Not taken into account if `in_pct == True`
+
+    Returns:
+        (np.ma.masked_array, dict): Slope and its metadata
+    """
+    array = dst.read(masked=True)
+
+    # Squeeze if needed
+    expand = False
+    if len(array.shape) == 3 and array.shape[0] == 1:
+        array = np.squeeze(array)  # Use this trick to make the sieve work
+        expand = True
+
+    # Compute slope (on unmasked data)
+    dx, dy = np.gradient(np.where(array.mask, 0.0, array.data), *dst.res)
+    x2_y2 = dx ** 2 + dy ** 2
+
+    if in_pct:
+        slope = 100 * (np.sqrt(x2_y2))
+    else:
+        slope = np.arctan(np.sqrt(x2_y2))
+
+        # Convert into degrees
+        if not in_rad:
+            slope = slope / DEG_2_RAD
+
+    # Use this trick to get the array back to 'normal'
+    if expand:
+        slope = np.expand_dims(slope, axis=0)
+
+    # Convert to masked array
+    slope_msk = np.ma.masked_array(slope, array.mask, fill_value=dst.nodata)
+
+    # Meta
+    meta = update_meta(slope_msk, dst.meta)
+
+    return slope_msk, meta
+
+
+# def _horn(arr, res_x, res_y):
+#     """
+#           0 1 2
+#           3 4 5
+#           6 7 8
+#
+#     Args:
+#         arr:
+#
+#     Returns:
+#
+#     """
+#     arr_0 = np.pad(arr, ((0, 1), (0, 1)), mode='constant')[1:, 1:]
+#     arr_1 = np.pad(arr, ((0, 1), (0, 0)), mode='constant')[1:, :]
+#     arr_2 = np.pad(arr, ((0, 1), (1, 0)), mode='constant')[1:, :-1]
+#     arr_3 = np.pad(arr, ((0, 0), (0, 1)), mode='constant')[:, 1:]
+#     arr_5 = np.pad(arr, ((0, 0), (1, 0)), mode='constant')[:, :-1]
+#     arr_6 = np.pad(arr, ((1, 0), (0, 1)), mode='constant')[:-1, 1:]
+#     arr_7 = np.pad(arr, ((1, 0), (0, 0)), mode='constant')[:-1, :]
+#     arr_8 = np.pad(arr, ((1, 0), (1, 0)), mode='constant')[:-1, :-1]
+#
+#     dy = ((arr_0 + 2 * arr_3 + arr_6) - (arr_2 + 2 * arr_5 + arr_8)) / res_y / 8.0
+#     dx = ((arr_6 + 2 * arr_7 + arr_8) - (arr_0 + 2 * arr_1 + arr_2)) / res_x / 8.0
+#
+#     return dx, dy
```

### Comparing `sertit-1.8.1/sertit/snap.py` & `sertit-1.9.0/sertit/snap.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/strings.py` & `sertit-1.9.0/sertit/strings.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit/vectors.py` & `sertit-1.9.0/sertit/vectors.py`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/sertit.egg-info/PKG-INFO` & `sertit-1.9.0/sertit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sertit
-Version: 1.8.1
+Version: 1.9.0
 Summary: ('SERTIT python library for generic tools',)
 Home-page: UNKNOWN
 Author: ICube-SERTIT
 Author-email: dev-sertit@unistra.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sertit/sertit-utils/issues/
 Project-URL: Documentation, https://sertit-utils.readthedocs.io/en/latest/
```

### Comparing `sertit-1.8.1/sertit.egg-info/SOURCES.txt` & `sertit-1.9.0/sertit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sertit-1.8.1/setup.py` & `sertit-1.9.0/setup.py`

 * *Files identical despite different names*

