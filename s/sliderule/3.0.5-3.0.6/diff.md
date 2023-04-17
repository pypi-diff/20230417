# Comparing `tmp/sliderule-3.0.5.tar.gz` & `tmp/sliderule-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.0.5.tar", last modified: Thu Apr 13 12:49:31 2023, max compression
+gzip compressed data, was "sliderule-3.0.6.tar", last modified: Mon Apr 17 15:44:36 2023, max compression
```

## Comparing `sliderule-3.0.5.tar` & `sliderule-3.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.270126 sliderule-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-13 12:49:11.000000 sliderule-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-13 12:49:11.000000 sliderule-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-13 12:49:31.270126 sliderule-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-13 12:49:11.000000 sliderule-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-13 12:49:11.000000 sliderule-3.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 12:49:31.270126 sliderule-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-13 12:49:11.000000 sliderule-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.262126 sliderule-3.0.5/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/arcticdem.py
--rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    36103 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-13 12:49:11.000000 sliderule-3.0.5/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.262126 sliderule-3.0.5/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-13 12:49:31.000000 sliderule-3.0.5/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-13 12:49:30.000000 sliderule-3.0.5/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 12:49:31.270126 sliderule-3.0.5/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/_landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/hls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/landsat.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-13 12:49:11.000000 sliderule-3.0.5/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-13 12:49:11.000000 sliderule-3.0.5/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.568606 sliderule-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-17 15:44:23.000000 sliderule-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-17 15:44:23.000000 sliderule-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-17 15:44:36.568606 sliderule-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-17 15:44:23.000000 sliderule-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-17 15:44:23.000000 sliderule-3.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 15:44:36.568606 sliderule-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1209 2023-04-17 15:44:23.000000 sliderule-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.564606 sliderule-3.0.6/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/arcticdem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24752 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11492 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9833 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36103 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36286 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85031 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43166 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-04-17 15:44:23.000000 sliderule-3.0.6/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.564606 sliderule-3.0.6/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-17 15:44:36.000000 sliderule-3.0.6/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 15:44:36.568606 sliderule-3.0.6/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4151 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/_landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7509 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/hls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/landsat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6284 2023-04-17 15:44:23.000000 sliderule-3.0.6/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-17 15:44:23.000000 sliderule-3.0.6/version.txt
```

### Comparing `sliderule-3.0.5/LICENSE` & `sliderule-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/PKG-INFO` & `sliderule-3.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.5
+Version: 3.0.6
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.5/README.md` & `sliderule-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/setup.py` & `sliderule-3.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/arcticdem.py` & `sliderule-3.0.6/sliderule/arcticdem.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/earthdata.py` & `sliderule-3.0.6/sliderule/earthdata.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/gedi.py` & `sliderule-3.0.6/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/h5.py` & `sliderule-3.0.6/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/icesat2.py` & `sliderule-3.0.6/sliderule/icesat2.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/io.py` & `sliderule-3.0.6/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/ipxapi.py` & `sliderule-3.0.6/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/ipysliderule.py` & `sliderule-3.0.6/sliderule/ipysliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule/sliderule.py` & `sliderule-3.0.6/sliderule/sliderule.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/sliderule.egg-info/PKG-INFO` & `sliderule-3.0.6/sliderule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.0.5
+Version: 3.0.6
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule-python/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.0.5/sliderule.egg-info/SOURCES.txt` & `sliderule-3.0.6/sliderule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/_landsat.py` & `sliderule-3.0.6/utils/_landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/big_query.py` & `sliderule-3.0.6/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.0.6/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.0.6/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.0.6/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/extract_h5_dataset.py` & `sliderule-3.0.6/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/hls.py` & `sliderule-3.0.6/utils/hls.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/icepyx_region.py` & `sliderule-3.0.6/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/landsat.py` & `sliderule-3.0.6/utils/landsat.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/monitor.py` & `sliderule-3.0.6/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/query_cmr.py` & `sliderule-3.0.6/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/query_elevations.py` & `sliderule-3.0.6/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/query_metrics.py` & `sliderule-3.0.6/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/query_photons.py` & `sliderule-3.0.6/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/query_stac.py` & `sliderule-3.0.6/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/query_version.py` & `sliderule-3.0.6/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/region_of_interest.py` & `sliderule-3.0.6/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/results_to_s3.py` & `sliderule-3.0.6/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/stac.py` & `sliderule-3.0.6/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/stream_events.py` & `sliderule-3.0.6/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/tail_events.py` & `sliderule-3.0.6/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.0.5/utils/utils.py` & `sliderule-3.0.6/utils/utils.py`

 * *Files identical despite different names*

