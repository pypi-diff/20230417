# Comparing `tmp/seg2map-0.0.6.tar.gz` & `tmp/seg2map-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seg2map-0.0.6.tar", last modified: Tue Mar  7 22:52:12 2023, max compression
+gzip compressed data, was "seg2map-0.0.7.tar", last modified: Mon Apr 17 16:16:42 2023, max compression
```

## Comparing `seg2map-0.0.6.tar` & `seg2map-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:52:12.155803 seg2map-0.0.6/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-03-07 22:52:00.000000 seg2map-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-07 22:52:00.000000 seg2map-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-03-07 22:52:12.155803 seg2map-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-03-07 22:52:00.000000 seg2map-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-07 22:52:00.000000 seg2map-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 22:52:12.155803 seg2map-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-07 22:52:00.000000 seg2map-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:52:12.147803 seg2map-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:52:12.151803 seg2map-0.0.6/src/seg2map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52142 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30222 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/exception_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/log_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)    24067 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/map_UI.py
--rw-r--r--   0 runner    (1001) docker     (123)    45856 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/map_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/models_UI.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)    41301 2023-03-07 22:52:00.000000 seg2map-0.0.6/src/seg2map/zoo_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:52:12.151803 seg2map-0.0.6/src/seg2map.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-03-07 22:52:12.000000 seg2map-0.0.6/src/seg2map.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-07 22:52:12.000000 seg2map-0.0.6/src/seg2map.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 22:52:12.000000 seg2map-0.0.6/src/seg2map.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-07 22:52:12.000000 seg2map-0.0.6/src/seg2map.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-07 22:52:12.000000 seg2map-0.0.6/src/seg2map.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.857835 seg2map-0.0.7/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-17 16:16:33.000000 seg2map-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-17 16:16:33.000000 seg2map-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-17 16:16:42.857835 seg2map-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-04-17 16:16:33.000000 seg2map-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 16:16:33.000000 seg2map-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 16:16:42.857835 seg2map-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-17 16:16:33.000000 seg2map-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.853835 seg2map-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.853835 seg2map-0.0.7/src/seg2map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55318 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32288 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/exception_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/log_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/map_UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/map_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24669 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/model_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/models_UI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35003 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/new_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40888 2023-04-17 16:16:33.000000 seg2map-0.0.7/src/seg2map/zoo_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 16:16:42.857835 seg2map-0.0.7/src/seg2map.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19521 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 16:16:42.000000 seg2map-0.0.7/src/seg2map.egg-info/top_level.txt
```

### Comparing `seg2map-0.0.6/LICENSE` & `seg2map-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.6/PKG-INFO` & `seg2map-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg2map
-Version: 0.0.6
+Version: 0.0.7
 Summary: An interactive jupyter notebook for downloading satellite imagery
 Author-email:  Sharon Fitzpatrick <sharon.fitzpatrick23@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Doodleverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `seg2map-0.0.6/README.md` & `seg2map-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.6/pyproject.toml` & `seg2map-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seg2map"
 dynamic = ["readme"]
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name=" Sharon Fitzpatrick", email="sharon.fitzpatrick23@gmail.com" },
 ]
 # find` directive with `include` or `exclude`
 description = "An interactive jupyter notebook for downloading satellite imagery"
 dependencies = [
   "scikit-image",
```

### Comparing `seg2map-0.0.6/src/seg2map/common.py` & `seg2map-0.0.7/src/seg2map/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,81 +1,194 @@
 import os
 import re
 import random
 import string
+from pathlib import Path
 import glob
 import shutil
 import json
 import math
 from datetime import datetime
 import logging
 from typing import Set, Union, List
 import json
 import math
 import logging
 import os, json, shutil
 from glob import glob
 import concurrent.futures
 from datetime import datetime
+from time import perf_counter
 
 # Internal dependencies imports
-from seg2map import exception_handler
+from seg2map import map_functions
 
 from tqdm.auto import tqdm
-import imageio
 import requests
 import zipfile
 from area import area
 import geopandas as gpd
 import numpy as np
 import geojson
 import matplotlib
 from leafmap import check_file_path
-import pandas as pd
 from osgeo import gdal
-
-
+from skimage.io import imsave
+import time
+from PIL import Image
+import rasterio
 from ipywidgets import ToggleButton
 from ipywidgets import HBox
 from ipywidgets import VBox
 from ipywidgets import Layout
 from ipywidgets import HTML
 from ipyfilechooser import FileChooser
 
 
 logger = logging.getLogger(__name__)
 
 
-import time
-from base64 import b64encode
-from PIL import Image, ImageSequence
-from io import BytesIO
-import rasterio
-from ipyleaflet import ImageOverlay
+def time_func(func):
+    def wrapper(*args, **kwargs):
+        start = perf_counter()
+        result = func(*args, **kwargs)
+        end = perf_counter()
+        print(f"{func.__name__} took {end - start:.6f} seconds to run.")
+        return result
+
+    return wrapper
+
+
+def find_file(path: str, filename: str = "session.json"):
+    # if session.json is found in main directory then session path was identified
+    filepath = os.path.join(path, filename)
+    if os.path.isfile(filepath):
+        return filepath
+    else:
+        parent_directory = os.path.dirname(path)
+        filepath = os.path.join(parent_directory, filename)
+        if os.path.isfile(filepath):
+            return filepath
+        else:
+            raise ValueError(
+                f"File '{filename}' not found in the parent directory: {parent_directory} or path"
+            )
 
 
-def get_rgb_img(img_path: str) -> str:
+def write_greylabel_to_png(npz_location: str) -> str:
+    """
+    Given the path of an .npz file containing a 'grey_label' key with an array of uint8 values,
+    writes the array to a PNG file with the same name and location as the .npz file, with the extension
+    changed to .png. Returns the path of the PNG file.
+
+    Parameters:
+    npz_location (str): The path of the .npz file to read from.
+
+    Returns:
+    str: The path of the written PNG file.
+    """
+    png_path = npz_location.replace(".npz", ".png")
+    with np.load(npz_location) as data:
+        dat = 1 + np.round(data["grey_label"].astype("uint8"))
+    imsave(png_path, dat, check_contrast=False, compression=0)
+    return png_path
+
+
+def create_greylabel_pngs(full_path: str) -> List[str]:
+    """
+    Given a directory path, finds all .npz files in the directory, writes the 'grey_label' array of each .npz
+    file to a corresponding PNG file, and returns a list of the paths of the written PNG files.
+
+    Parameters:
+    full_path (str): The path of the directory to search for .npz files.
+
+    Returns:
+    List[str]: A list of the paths of the written PNG files.
+    """
+    png_files = []
+    npzs = sorted(glob(os.path.join(full_path, "*.npz")))
+    for npz in npzs:
+        png_files.append(write_greylabel_to_png(npz))
+    return png_files
+
+
+def get_subdirectories_with_ids(base_path: str) -> dict:
+    all_items = os.listdir(base_path)
+    subdirs_with_ids = {}
+
+    for item in all_items:
+        item_path = os.path.join(base_path, item)
+        if os.path.isdir(item_path) and item.startswith("ID_"):
+            id = item.split("_")[1]
+            subdirs_with_ids[id] = item_path
+
+    return subdirs_with_ids
+
+
+def extract_roi_id_from_path(path):
+    """
+    Extracts roi_id from a directory name in a given path.
+
+    The function assumes that the directory name is in the format "ID_{roiid}_dates_*".
+
+    Args:
+        path (str): A string representing the path to the directory containing the roi id.
+
+    Returns:
+        A string representing the extracted roi id, or None if the roi id is not found.
+    """
+    start_index = path.find("ID_") + len("ID_")
+    end_index = path.find("_dates_")
+    if start_index != -1 and end_index != -1:
+        return path[start_index:end_index]
+    else:
+        return None
+
+
+def read_text_file(file_path: str) -> List[str]:
+    """
+    Read the contents of a text file and return them as a list of strings.
+
+    Args:
+        file_path: The path to the text file to read.
+
+    Returns:
+        A list of strings representing the lines of text in the file. The list will not include any line ending characters
+        ('\n', '\r', or '\r\n').
+
+    Raises:
+        ValueError: If the file does not exist at the specified file path.
+    """
+    if not os.path.isfile(file_path):
+        raise ValueError(f"{os.path.basename(file_path)} did not exist at {file_path}")
+    with open(file_path) as f:
+        data = f.read().split("\n")
+    return data
+
+
+def convert_to_rgb(img_path: str) -> str:
     """
     Converts an image to RGB format and saves it to a new file.
     Compatable image types: '.jpg' and '.png'
 
     Parameters:
     img_path (str): The file path of the image to be converted.
 
     Returns:
     str: The file path of the converted image.
     """
+    logger.info(f"img_path: {img_path}")
     if img_path.endswith(".jpg"):
         im = Image.open(img_path, formats=("JPEG",)).convert("RGB")
         out_path = img_path.replace(".jpg", "_RGB.jpg")
     elif img_path.endswith(".png"):
         im = Image.open(img_path, formats=("PNG",)).convert("RGB")
         out_path = img_path.replace(".png", "_RGB.png")
     im.save(out_path)
-
+    logger.info(f"out_path: {out_path}")
     return out_path
 
 
 def get_bounds(tif_path):
     """
     Gets the bounds of a GeoTIFF file.
 
@@ -89,50 +202,108 @@
     """
     dataset = rasterio.open(tif_path)
     b = dataset.bounds
     bounds = [(b.bottom, b.left), (b.top, b.right)]
     return bounds
 
 
-def get_image_overlay(tif_path, jpg_path, layer_name: str):
+def get_years_in_path(full_path: Path) -> List[str]:
+    """
+    Return a list of directory names within the given directory that match the pattern of a four-digit year (e.g. '2022').
+
+    Args:
+        directory: The directory to search for year folders. This can be a string or a Path object.
+
+    Returns:
+        A list of directory names within the given directory that match the pattern of a four-digit year.
+    """
+    full_path = Path(full_path)
+    years = []
+    with os.scandir(full_path) as entries:
+        for entry in entries:
+            if entry.is_dir() and re.match(r"^\d{4}$", entry.name):
+                years.append(entry.name)
+    return years
+
+
+def find_file(dir_path, filename, case_insensitive=True):
+    if case_insensitive:
+        filename = filename.lower()
+    for file in os.listdir(dir_path):
+        if file.lower() == filename:
+            return os.path.join(dir_path, file)
+    return None
+
+
+# @time_func
+def get_image_overlay(
+    tif_path,
+    image_path,
+    layer_name: str,
+    convert_RGB: bool = True,
+    file_format: str = "png",
+):
     """
     Creates an image overlay for a GeoTIFF file using a JPG image.
 
     Parameters:
     tif_path (str): The file path of the GeoTIFF file.
     jpg_path (str): The file path of the JPG image.
     layer_name (str): The name of the layer.
 
     Returns:
     ImageOverlay: An image overlay for the GeoTIFF file.
     """
+    logger.info(f"tif_path: {tif_path}")
+    logger.info(f"image_path: {image_path}")
+    logger.info(f"convert_RGB: {convert_RGB}")
+    logger.info(f"file_format: {file_format}")
     bounds = get_bounds(tif_path)
-    RGB_path = get_rgb_img(jpg_path)
-    image = Image.open(RGB_path)
-    f = BytesIO()
-    image.save(f, "JPEG")
-
-    data = b64encode(f.getvalue())
-    data = data.decode("ascii")
-    url = "data:image/JPEG;base64," + data
-    image_overlay = ImageOverlay(url=url, bounds=bounds, name=layer_name)
+    # convert image to RGB
+    if convert_RGB:
+        image_path = convert_to_rgb(image_path)
+
+    image_overlay = map_functions.get_overlay_for_image(
+        image_path, bounds, layer_name, file_format=file_format
+    )
     return image_overlay
 
 
 class Timer:
     def __enter__(self):
         self.start = time.perf_counter()
         return self
 
     def __exit__(self, *args):
         self.end = time.perf_counter()
         self.interval = self.end - self.start
         print(f"Elapsed time: {self.interval:.6f} seconds")
 
 
+def build_tiff(tif_path, vrt_path):
+    # then build tiff
+    ds = gdal.Translate(
+        destName=tif_path,
+        creationOptions=["NUM_THREADS=ALL_CPUS", "COMPRESS=LZW", "TILED=YES"],
+        srcDS=vrt_path,
+    )
+    ds.FlushCache()
+    ds = None
+
+
+def build_vrt(vrt_path: str, imgsToMosaic: List[str], resampleAlg: str = "mode"):
+    vrt_options = gdal.BuildVRTOptions(resampleAlg=resampleAlg)
+    try:
+        ds = gdal.BuildVRT(vrt_path, imgsToMosaic, options=vrt_options)
+        ds.FlushCache()
+        ds = None
+    except Exception as e:
+        print(f"Error building VRT file: {e}")
+
+
 def create_dir_chooser(callback, title: str = None, starting_directory: str = "data"):
     """
     Creates a file chooser widget for selecting directories and a button to close the file chooser.
 
     Parameters:
     callback (function): A function to be called when the user selects a directory.
     title (str): The title of the file chooser (optional).
@@ -208,55 +379,14 @@
 
         if not found_group:
             tif_groups[(x_min, x_size, y_max, y_size)] = [tif_file]
 
     return list(tif_groups.values())
 
 
-def delete_tifs_at_same_location(path):
-    multiple_tifs_same_location = [
-        tifs for tifs in group_tif_locations(path) if len(tifs) > 1
-    ]
-    delete_tifs_with_black_pixels(multiple_tifs_same_location)
-
-
-def delete_tifs_except(tif_paths, keep_tif_path):
-    for tif_path in tif_paths:
-        if tif_path != keep_tif_path:
-            os.remove(tif_path)
-
-
-def delete_tifs_with_black_pixels(tif_groups):
-    # only keep tifs where ratio of non-black pixels to total pixels is the highest
-    for tif_paths in tif_groups:
-        max_tif_path = max(tif_paths, key=get_pixel_ratio)
-        delete_tifs_except(tif_paths, max_tif_path)
-
-
-def get_pixel_ratio(tif_path):
-    """
-    Calculates the ratio of non-black pixels to total pixels in a GeoTIFF file.
-
-    Args:
-        tif_path: str - The file path to the GeoTIFF file.
-
-    Returns:
-        float - The ratio of non-black pixels to total pixels in the GeoTIFF file.
-
-    Example:
-        ratio = get_pixel_ratio("path/to/tif_file.tif")
-        # Returns a float representing the ratio of non-black pixels to total pixels in the GeoTIFF file.
-    """
-    img = imageio.imread(tif_path)
-    total_pixels = (img >= 0).sum()
-    non_black_pixels = (img > 0).sum()
-    pixel_ratio = non_black_pixels / total_pixels
-    return pixel_ratio
-
-
 def group_files(files: List[str], size: int = 2) -> List[List[str]]:
     """
     Groups a list of file paths into sublists of a specified size.
 
     This function takes a list of file paths and groups them into sublists of a specified size. The default size is 2. The function returns a list of sublists, where each sublist contains up to `size` file paths.
 
     Parameters:
@@ -280,19 +410,24 @@
     Returns:
     None: This function does not return anything.
     """
     for roi_path in roi_paths:
         year_dirs = get_matching_dirs(roi_path, pattern=r"^\d{4}$")
         for year_path in year_dirs:
             glob_str = os.path.join(year_path, "*merged_multispectral.jpg")
+            # A merged jpg has already been createed
             if len(glob(glob_str)) >= 1:
+                logger.warning(f"*merged_multispectral.jpg already exists {year_path}")
                 continue
+            # no tifs exist to merge
             if len(os.listdir(year_path)) == 0:
+                logger.warning(f"*{year_path} contains no tifs")
                 continue
             try:
+                # create merged_multispectral.jpg
                 get_merged_multispectural(year_path)
             except Exception as merge_error:
                 logger.error(f"Year: {year_path}\nmerge_error: {merge_error}")
                 print(f"Year: {year_path}\nmerge_error: {merge_error}")
                 continue
 
 
@@ -304,84 +439,72 @@
 
     Parameters:
     - src_path (str): The path of the directory containing the GeoTIFF files.
 
     Returns:
     - The path of the merged VRT file.
     """
+    # get all the unmerged tif files
     tif_files = glob(os.path.join(src_path, "*.tif"))
     tif_files = [file for file in tif_files if "merged_multispectral" not in file]
 
     logger.info(f"Found {len(tif_files)} GeoTIFF files in {src_path}")
     logger.info(f"tif_files: {tif_files}")
-    merged_files = []
-    for idx, files in enumerate(group_files(tif_files, 4)):
-        filename = f"merged_multispectral_{idx}.vrt"
-        dst_path = os.path.join(src_path, filename)
-        merged_tif = merge_files(files, dst_path, create_jpg=False)
-        merged_files.append(merged_tif)
-
-    logger.info(f"merged_files {merged_files}")
-    dst_path = os.path.join(src_path, "merged_multispectral.vrt")
-    merged_file = merge_files(merged_files, dst_path)
-    # delete intermediate merged tifs and vrts
-    pattern = ".*merged_multispectral_\d+.*"
-    deleted_files = delete_files(pattern, src_path)
-    logger.info(f"deleted_files {deleted_files}")
+
+    vrt_path = os.path.join(src_path, "merged_multispectral.vrt")
+    merged_file = merge_files(tif_files, vrt_path, create_jpg=True)
     return merged_file
 
 
-def merge_files(src_files: str, dest_path: str, create_jpg: bool = True) -> str:
+def merge_files(src_files: str, vrt_path: str, create_jpg: bool = True) -> str:
     """Merge a list of GeoTIFF files into a single JPEG file.
 
     Args:
     src_files (List[str]): A list of file paths to be merged.
     dest_path (str): The path to the output JPEG file.
 
     Returns:
     str: The path to the output JPEG file.
     """
     # Check if path to source exists
     for file in src_files:
         if not os.path.exists(file):
             raise FileNotFoundError(f"{file} not found.")
     try:
-        ## create vrt(virtual world format) file
-        # Create VRT file
-        vrt_options = gdal.BuildVRTOptions(
-            resampleAlg="average", srcNodata=0, VRTNodata=0
-        )
+        # create vrt(virtual world format) file
+        vrt_options = gdal.BuildVRTOptions(resampleAlg="mode", srcNodata=0, VRTNodata=0)
+        logger.info(f"dest_path: {vrt_path}")
         # creates a virtual world file using all the tifs and overwrites any pre-existing .vrt
-        virtual_dataset = gdal.BuildVRT(dest_path, src_files, options=vrt_options)
+        virtual_dataset = gdal.BuildVRT(vrt_path, src_files, options=vrt_options)
         # flushing the cache causes the vrt file to be created
         virtual_dataset.FlushCache()
         # reset the dataset object
         virtual_dataset = None
 
         # create geotiff (.tiff) from merged vrt file
-        tif_path = dest_path.replace(".vrt", ".tif")
+        tif_path = vrt_path.replace(".vrt", ".tif")
         virtual_dataset = gdal.Translate(
             tif_path,
             creationOptions=["COMPRESS=LZW", "TILED=YES"],
-            srcDS=dest_path,
+            srcDS=vrt_path,
         )
         virtual_dataset.FlushCache()
         virtual_dataset = None
 
         if create_jpg:
             # convert .vrt to .jpg file
             virtual_dataset = gdal.Translate(
-                dest_path.replace(".vrt", ".jpg"),
+                vrt_path.replace(".vrt", ".jpg"),
                 creationOptions=["WORLDFILE=YES", "QUALITY=100"],
-                srcDS=dest_path.replace(".vrt", ".tif"),
+                srcDS=tif_path,
             )
             virtual_dataset.FlushCache()
             virtual_dataset = None
 
-        return dest_path
+        return vrt_path
     except Exception as e:
         print(e)
         logger.error(e)
         raise e
 
 
 def delete_files(pattern, path):
@@ -412,66 +535,14 @@
                 full_path = os.path.join(dirpath, filename)
                 os.remove(full_path)
                 deleted_files.append(full_path)
 
     return deleted_files
 
 
-# def merge_tifs(src_dir: str, dest_dir: str) -> str:
-#     # Check if path to destination directory exists
-#     if not os.path.exists(dest_dir):
-#         raise FileNotFoundError(f"{dest_dir} not found.")
-#     # Check if path to source exists
-#     if not os.path.exists(src_dir):
-#         raise FileNotFoundError(f"{src_dir} not found.")
-#     try:
-
-#         # Create a list of tif files in source directory
-#         tif_files = glob(os.path.join(src_dir, "*.tif"))
-#         if not tif_files:
-#             raise FileNotFoundError(f"No tif files found in {src_dir}.")
-
-#         vrt_path = os.path.join(dest_dir, "merged_multispectral.vrt")
-#         logger.info(f"vrt_path: {vrt_path}")
-
-#         ## create vrt(virtual world format) file
-#         vrtoptions = gdal.BuildVRTOptions(
-#             resampleAlg="average", srcNodata=0, VRTNodata=0
-#         )
-#         # creates a virtual world file using all the tifs and overwrites any pre-existing .vrt
-#         virtual_dataset = gdal.BuildVRT(vrt_path, tif_files, options=vrtoptions)
-#         # flushing the cache causes the vrt file to be created
-#         virtual_dataset.FlushCache()
-#         # reset the dataset object
-#         virtual_dataset = None
-
-#         # create geotiff (.tiff) from merged vrt file
-#         virtual_dataset = gdal.Translate(
-#             vrt_path.replace(".vrt", ".tif"),
-#             creationOptions=["COMPRESS=LZW", "TILED=YES"],
-#             srcDS=vrt_path,
-#         )
-#         virtual_dataset.FlushCache()
-#         virtual_dataset = None
-
-#         # convert .vrt to .jpg file
-#         virtual_dataset = gdal.Translate(
-#             vrt_path.replace(".vrt", ".jpg"),
-#             creationOptions=["WORLDFILE=YES", "QUALITY=100"],
-#             srcDS=vrt_path.replace(".vrt", ".tif"),
-#         )
-#         virtual_dataset.FlushCache()
-#         virtual_dataset = None
-#         return vrt_path
-#     except Exception as e:
-#         print(e)
-#         logger.error(e)
-#         raise e
-
-
 def gdal_translate_png_to_tiff(
     files: List[str],
     translateoptions: str = "-of JPEG -co COMPRESS=JPEG -co TFW=YES -co QUALITY=100",
 ):
     """Convert TIFF files to JPEG files using GDAL.
 
     Args:
@@ -490,35 +561,63 @@
         else:
             dst = gdal.Translate(new_file, file, options=translateoptions)
             new_files.append(new_file)
             dst = None  # close and save ds
     return new_files
 
 
-def gdal_translate_jpeg(
+def move_files_resurcively(src, dest):
+    """Move all files and subdirectories from the source directory to the destination directory recursively.
+
+    Args:
+        source_dir (str): The path to the source directory.
+        destination_dir (str): The path to the destination directory.
+
+    Returns:
+        None
+    """
+    if not os.path.isdir(src):
+        os.makedirs(src)
+    if not os.path.isdir(dest):
+        os.makedirs(dest)
+    # Move all files and subdirectories from the source directory to the destination directory
+    for entry in os.scandir(src):
+        # Move the entry to the destination directory
+        shutil.move(entry.path, os.path.join(dest, entry.name))
+
+
+def gdal_translate_jpegs(
     files: List[str],
-    translateoptions: str = "-of JPEG -co COMPRESS=JPEG -co TFW=YES -co QUALITY=100",
+    translateoptions: str = None,
+    kwargs=None,
 ):
     """Convert TIFF files to JPEG files using GDAL.
 
     Args:
         files (List[str]): List of file paths to TIFF files to be converted.
-        translateoptions (str, optional): GDAL options for converting TIFF files to JPEG files. Defaults to "-of JPEG -co COMPRESS=JPEG -co TFW=YES -co QUALITY=100".
-
+        translateoptions (str, optional): GDAL options for converting TIFF files to JPEG files.
+        kwargs(dict, optional): dictionary of GDAL options for converting TIFF files to JPEG files. Options located at:
+            https://gdal.org/api/python/osgeo.gdal.html#osgeo.gdal.TranslateOptions
     Returns:
         List[str]: List of file paths to the newly created JPEG files.
     """
     new_files = []
-    for f in files:
-        jpg_file = f.replace(".tif", ".jpg")
+    for file in files:
+        jpg_file = file.replace(".tif", ".jpg")
         if os.path.exists(jpg_file):
-            print(f"File: {jpg_file} already exists")
+            logger.info(f"File: {jpg_file} already exists")
         else:
-            dst = gdal.Translate(f.replace(".tif", ".jpg"), f, options=translateoptions)
-            new_files.append(f.replace(".tif", ".jpg"))
+            if kwargs:
+                dst = gdal.Translate(jpg_file, file, **kwargs)
+                new_files.append(jpg_file)
+            elif translateoptions:
+                dst = gdal.Translate(jpg_file, file, options=translateoptions)
+                new_files.append(jpg_file)
+            else:
+                raise ValueError("Must provide value for kwargs or translateoptions.")
             dst = None  # close and save ds
     return new_files
 
 
 def rename_files(directory: str, pattern: str, new_name: str, replace_name: str):
     """Rename all files in a directory that match a glob pattern
 
@@ -780,18 +879,20 @@
             raise FileExistsError(dir_path)
     else:
         os.makedirs(dir_path)
     return dir_path
 
 
 def create_directory(file_path: str, name: str) -> str:
+    """
+    Creates a new directory with the given name in the specified file path, if it does not already exist.
+    Returns the full path to the new directory.
+    """
     new_directory = os.path.join(file_path, name)
-    # If the directory named 'name' does not exist, create it
-    if not os.path.exists(new_directory):
-        os.makedirs(new_directory)
+    os.makedirs(new_directory, exist_ok=True)
     return new_directory
 
 
 def generate_random_string(avoid_list=[]):
     alphanumeric = string.ascii_letters + string.digits
     random_string = "".join(random.choice(alphanumeric) for i in range(6))
     if random_string in avoid_list:
```

### Comparing `seg2map-0.0.6/src/seg2map/downloads.py` & `seg2map-0.0.7/src/seg2map/downloads.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,152 @@
 import os
-import time
 import json
 import math
-from typing import List
+from typing import List, Tuple
 import platform
 import logging
 import os, json, shutil
 from glob import glob
 import concurrent.futures
-from datetime import datetime
 
 from seg2map import exceptions
 from seg2map import common
 
 import asyncio
 import nest_asyncio
 import aiohttp
 import tqdm
 import tqdm.auto
 import tqdm.asyncio
 import ee
+import zipfile
+from area import area
+import geopandas as gpd
+from shapely.geometry import LineString, MultiPolygon, Polygon
+from shapely.ops import split
+from osgeo import gdal
 
 
 logger = logging.getLogger(__name__)
 
+import asyncio
+import aiohttp
+import logging
+from aiohttp import ClientResponseError, ClientConnectionError
+
+
+async def async_download_url_dict(url_dict: dict = {}):
+    async with aiohttp.ClientSession() as session:
+        tasks = []
+        for save_path, url in url_dict.items():
+            task = asyncio.create_task(
+                download_data_with_retries(session, url, save_path, total_attempts=2)
+            )
+            tasks.append(task)
+        results = await tqdm.asyncio.tqdm.gather(*tasks)
+
+
+async def download_data_with_retries(
+    session,
+    url,
+    save_location,
+    retries=3,
+    initial_delay=1,
+    max_delay=32,
+    total_attempts=2,
+):
+    attempts = 0
+    while attempts < total_attempts:
+        success = await download_with_retries(
+            session, url, save_location, retries, initial_delay, max_delay
+        )
+        if success:
+            return True  # Download successful
+        attempts += 1
+
+    logger.error(f"Download failed after {total_attempts} attempts: {url}")
+    print(f"Download failed after {total_attempts} attempts: {url}")
+    return False
+
+
+async def async_download_url(session, url: str, save_path: str):
+    model_name = url.split("/")[-1]
+    chunk_size: int = 2048
+    async with session.get(url, raise_for_status=True) as r:
+        content_length = r.headers.get("Content-Length")
+        if content_length is not None:
+            content_length = int(content_length)
+            with open(save_path, "wb") as fd:
+                with tqdm.auto.tqdm(
+                    total=content_length,
+                    unit="B",
+                    unit_scale=True,
+                    unit_divisor=1024,
+                    desc=f"Downloading {model_name}",
+                    initial=0,
+                    ascii=False,
+                    position=0,
+                ) as pbar:
+                    async for chunk in r.content.iter_chunked(chunk_size):
+                        fd.write(chunk)
+                        pbar.update(len(chunk))
+        else:
+            with open(save_path, "wb") as fd:
+                async for chunk in r.content.iter_chunked(chunk_size):
+                    fd.write(chunk)
+
+
+async def download_with_retries(
+    session, url, save_location, retries, initial_delay, max_delay
+):
+    delay = initial_delay
+    for i in range(retries):
+        try:
+            async with session.get(url) as response:
+                response.raise_for_status()
+                content_length = response.headers.get("Content-Length")
+                if content_length is not None:
+                    content_length = int(content_length)
+                    with open(save_location, "wb") as fd:
+                        with tqdm.auto.tqdm(
+                            total=content_length,
+                            unit="B",
+                            unit_scale=True,
+                            unit_divisor=1024,
+                            desc=f"Downloading {os.path.dirname(save_location)}",
+                            initial=0,
+                            ascii=False,
+                            position=0,
+                        ) as pbar:
+                            async for chunk in response.content.iter_chunked(1024):
+                                if not chunk:
+                                    break
+                                fd.write(chunk)
+                                pbar.update(len(chunk))
+                else:
+                    with open(save_location, "wb") as fd:
+                        async for chunk in response.content.iter_chunked(1024):
+                            fd.write(chunk)
+                return True  # Download successful
+        except (ClientResponseError, ClientConnectionError) as e:
+            logger.error(f"Error downloading {url}: {e}")
+        except asyncio.exceptions.TimeoutError as e:
+            logger.error(f"Timeout error for {url}: {e}")
+        except Exception as e:
+            logger.error(f"Unexpected error downloading {url}: {e}")
+        if i < retries - 1:
+            logger.warning(
+                f"Retrying download in {delay} seconds... ({i + 1}/{retries})"
+            )
+            await asyncio.sleep(delay)
+            # Update delay for the next iteration, doubling it while ensuring it doesn't exceed max_delay
+            delay = min(delay * 2, max_delay)
+        else:
+            return False
+
 
 async def download_file(session, url, save_location):
     retries = 3  # number of times to retry download
     for i in range(retries):
         try:
             async with session.get(url) as response:
                 if response.status != 200:
@@ -43,22 +162,28 @@
                 break  # break out of retry loop if download is successful
         except asyncio.exceptions.TimeoutError as e:
             logger.error(e)
             logger.error(f"An error occurred while downloading {save_location}.{e}")
             print(
                 f"Timeout error occurred for {url}. Retrying with new session in 1 second... ({i + 1}/{retries})"
             )
+            logger.warning(
+                f"Timeout error occurred for {url}. Retrying with new session in 1 second... ({i + 1}/{retries})"
+            )
             await asyncio.sleep(1)
             async with aiohttp.ClientSession() as new_session:
                 return await download_file(new_session, url, save_location)
         except Exception as e:
             logger.error(e)
             logger.error(
                 f"Download failed for {save_location} {url}. Retrying in 1 second... ({i + 1}/{retries})"
             )
+            logger.warning(
+                f"Timeout error occurred for {url}. Retrying with new session in 1 second... ({i + 1}/{retries})"
+            )
             print(
                 f"Download failed for {url}. Retrying in 1 second... ({i + 1}/{retries})"
             )
             await asyncio.sleep(1)
     else:
         logger.error(f"Download failed for {save_location} {url}.")
         print(f"Download failed for {url}.")
@@ -69,15 +194,14 @@
     coroutines = []
     logger.info(f"group: {group}")
     for tile_number, tile in enumerate(group):
         polygon = tile["polygon"]
         filepath = os.path.abspath(tile["filepath"])
         filenames = {
             "multiband": "multiband" + str(tile_number),
-            "singleband": os.path.basename(filepath),
         }
         for tile_id in tile["ids"]:
             logger.info(f"tile_id: {tile_id}")
             file_id = tile_id.replace("/", "_")
             filename = filenames["multiband"] + "_" + file_id
             save_location = os.path.join(filepath, filename.replace("/", "_") + ".zip")
             logger.info(f"save_location: {save_location}")
@@ -99,15 +223,15 @@
     )
     # await asyncio.gather(*coroutines)
 
     logger.info(f"Files downloaded to {group[0]['filepath']}")
     common.unzip_dir(group[0]["filepath"])
     common.delete_empty_dirs(group[0]["filepath"])
     # delete duplicate tifs. keep tif with most non-black pixels
-    common.delete_tifs_at_same_location(group[0]["filepath"])
+    # common.delete_tifs_at_same_location(group[0]["filepath"])
 
 
 # Download the information for each year
 async def download_groups(
     groups,
     semaphore: asyncio.Semaphore,
     group_id: str = "",
@@ -209,46 +333,14 @@
     # get nested running loop and wait for async downloads to complete
     loop = asyncio.get_running_loop()
     result = loop.run_until_complete(async_callback(**kwargs))
     logger.info(f"result: {result}")
     return result
 
 
-import json
-import math
-import logging
-import os, json, shutil
-from glob import glob
-import concurrent.futures
-from datetime import datetime
-import platform
-
-from seg2map import exceptions
-from seg2map import common
-
-from typing import List, Tuple
-
-import tqdm
-import tqdm.auto
-import zipfile
-from area import area
-import numpy as np
-import geopandas as gpd
-import asyncio
-import aiohttp
-import tqdm.asyncio
-import nest_asyncio
-from shapely.geometry import LineString, MultiPolygon, Polygon
-from shapely.ops import split
-import ee
-from osgeo import gdal
-
-logger = logging.getLogger(__name__)
-
-
 # GEE allows for 20 concurrent requests at once
 limit = asyncio.Semaphore(20)
 
 
 def get_num_splitters(gdf: gpd.GeoDataFrame) -> int:
     """
     Calculates the minimum number of splitters required to divide a geographic region represented by a GeoDataFrame into smaller, equal-sized tiles whose
@@ -409,18 +501,15 @@
 
 
 def create_tasks(
     session: aiohttp.ClientSession,
     polygon: List[tuple],
     tile_id: str,
     filepath: str,
-    multiband_filepath: str,
-    filenames: dict,
-    file_id: str,
-    download_bands: str,
+    filename: str,
 ) -> list:
     """
 
     creates a list of tasks that are used to download the data.
 
     Parameters
     ----------
@@ -430,96 +519,70 @@
     polygon : List[tuple] coordinates of the polygon in lat/lon
     ex: [(1,2),(3,4)(4,3),(3,3),(1,2)]
     tile_id : str
         GEE id of the tile
         ex: 'USDA/NAIP/DOQQ/m_4012407_se_10_1_20100612'
     filepath : str
         full path to tile directory that data will be saved to
-    multiband_filepath : str
-        The path to a directory will save multiband files
-    filenames : dict
-        A dictionary of filenames:
-        'singleband': name of singleband files
-        'multiband': name of multiband files
+    filename : str
+       name of file that data will be downloaded to
     file_id : str
         name that file will be saved as based on tile_id
-    download_bands : str
-        type of imagery to download
-        must be one of the following strings "multiband","singleband", or "both"
 
     Returns
     -------
     tasks : list
         A list of tasks that are used to download the data.
 
     """
     tasks = []
-    if download_bands == "multiband" or download_bands == "both":
-
-        task = asyncio.create_task(
-            async_download_tile(
-                session,
-                polygon,
-                tile_id,
-                multiband_filepath,
-                filename=filenames["multiband"] + "_" + file_id,
-                filePerBand=False,
-            )
-        )
-        tasks.append(task)
-    if download_bands == "singleband" or download_bands == "both":
-        task = asyncio.create_task(
-            async_download_tile(
-                session,
-                polygon,
-                tile_id,
-                filepath,
-                filename=filenames["singleband"] + "_" + file_id,
-                filePerBand=False,
-            )
+    task = asyncio.create_task(
+        async_download_tile(
+            session,
+            polygon,
+            tile_id,
+            filepath,
+            filename,
+            filePerBand=False,
         )
-        tasks.append(task)
+    )
+    tasks.append(task)
     return tasks
 
 
-async def async_download_all_tiles(tiles_info: List[dict], download_bands: str) -> None:
+async def async_download_all_tiles(tiles_info: List[dict]) -> None:
     # creates task for each tile to be downloaded and waits for tasks to complete
     tasks = []
     for counter, tile_dict in enumerate(tiles_info):
         polygon = tile_dict["polygon"]
         filepath = os.path.abspath(tile_dict["filepath"])
         parent_dir = os.path.dirname(filepath)
         multiband_filepath = os.path.join(parent_dir, "multiband")
-        filenames = {
-            "multiband": "multiband" + str(counter),
-            "singleband": os.path.basename(filepath),
-        }
-
-        timeout = aiohttp.ClientTimeout(total=3000)
-        async with aiohttp.ClientSession(timeout=timeout) as session:
+        async with aiohttp.ClientSession(timeout=3000) as session:
             for tile_id in tile_dict["ids"]:
                 logger.info(f"tile_id: {tile_id}")
                 file_id = tile_id.replace("/", "_")
                 # handles edge case where tile has 2 years in the tile ID by extracting the ealier year
                 year_str = file_id.split("_")[-1][:4]
                 if len(file_id.split("_")[-2]) == 8:
                     year_str = file_id.split("_")[-2][:4]
+
+                filename = "multiband" + str(counter) + "_" + file_id
                 # full path to year directory within multiband dir eg. ./multiband/2012
                 year_filepath = os.path.join(multiband_filepath, year_str)
                 logger.info(f"year_filepath: {year_filepath}")
                 tasks.extend(
                     create_tasks(
                         session,
                         polygon,
                         tile_id,
                         filepath,
                         year_filepath,
-                        filenames,
+                        filename,
                         file_id,
-                        download_bands,
                     )
                 )
     # show a progress bar of all the requests in progress
     await tqdm.asyncio.tqdm.gather(*tasks, position=0, desc=f"All Downloads")
 
 
 async def get_ids_for_tile(
@@ -721,16 +784,14 @@
 ) -> None:
     """creates a nested loop that's used to asynchronously download imagery and waits for all the imagery to download
     Args:
         download_path (str): full path to directory to download imagery to
         roi_gdf (gpd.GeoDataFrame): geodataframe of ROIs on the map
         ids (List[str]): ids of ROIs to download imagery for
         dates (Tuple[str]): start and end dates
-        download_bands (str): type of imagery to download
-            must be one of the following strings "multiband","singleband", or "both"
     """
     ROI_tiles = {}
     tasks = []
     semaphore = asyncio.Semaphore(50)
 
     for roi_path, roi_id in zip(roi_paths, selected_ids):
         tasks.append(
@@ -749,88 +810,68 @@
     for roi_id in ROI_tiles.keys():
         for year in ROI_tiles[roi_id].keys():
             mk_filepaths(ROI_tiles[roi_id][year])
 
     return ROI_tiles
 
 
-async def async_download_ROIs(ROI_tiles: List[dict], download_bands: str) -> None:
+async def async_download_ROIs(ROI_tiles: List[dict]) -> None:
     """
     Downloads the specified bands for each ROI tile asynchronously using aiohttp and asyncio.
 
     Parameters:
     ROI_tiles (List[dict]): A list of dictionaries representing the ROI tiles to download.
-    download_bands (str): A comma-separated string of band numbers to download.
-
     Returns:
     None: This function does not return anything.
     """
     async with aiohttp.ClientSession() as session:
         # creates task for each tile to be downloaded and waits for tasks to complete
         tasks = []
         for ROI_tile in ROI_tiles:
             for year in ROI_tile.keys():
                 print(f"YEAR for ROI tile: {year}")
-                task = asyncio.create_task(
-                    async_download_year(ROI_tile[year], download_bands, session)
-                )
+                task = asyncio.create_task(async_download_year(ROI_tile[year], session))
                 tasks.append(task)
         # show a progress bar of all the requests in progress
         await tqdm.asyncio.tqdm.gather(*tasks, position=0, desc=f"All Downloads")
 
 
-async def async_download_year(
-    tiles_info: List[dict], download_bands: str, session
-) -> None:
+async def async_download_year(tiles_info: List[dict], session) -> None:
     """
     Downloads the specified bands for each tile in the specified year asynchronously using aiohttp and asyncio.
 
     Parameters:
     tiles_info (List[dict]): A list of dictionaries representing the tiles to download.
-    download_bands (str): A comma-separated string of band numbers to download.
     session: The aiohttp session to use for downloading.
 
     Returns:
     None: This function does not return anything.
     """
     # creates task for each tile to be downloaded and waits for tasks to complete
     tasks = []
     for counter, tile_dict in enumerate(tiles_info):
 
         polygon = tile_dict["polygon"]
         filepath = os.path.abspath(tile_dict["filepath"])
         filenames = {
             "multiband": "multiband" + str(counter),
-            "singleband": os.path.basename(filepath),
         }
         for tile_id in tile_dict["ids"]:
             logger.info(f"tile_id: {tile_id}")
             file_id = tile_id.replace("/", "_")
             logger.info(f"year_filepath: {filepath}")
             tasks.extend(
                 create_tasks(
                     session,
                     polygon,
                     tile_id,
                     filepath,
                     filepath,
                     filenames,
                     file_id,
-                    download_bands,
                 )
             )
     # show a progress bar of all the requests in progress
     await tqdm.asyncio.tqdm.gather(*tasks, position=0, desc=f"All Downloads")
     common.unzip_data(os.path.dirname(filepath))
     # delete any directories that were empty
     common.delete_empty_dirs(os.path.dirname(filepath))
-
-
-# call asyncio to run download_ROIs
-def run_magic_function_to_download(ROI_tiles: List[dict], download_bands: str) -> None:
-    if platform.system() == "Windows":
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-    # apply a nested loop to jupyter's event loop for async downloading
-    nest_asyncio.apply()
-    # get nested running loop and wait for async downloads to complete
-    loop = asyncio.get_running_loop()
-    loop.run_until_complete(async_download_ROIs(ROI_tiles, download_bands))
```

### Comparing `seg2map-0.0.6/src/seg2map/exception_handler.py` & `seg2map-0.0.7/src/seg2map/exception_handler.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.6/src/seg2map/exceptions.py` & `seg2map-0.0.7/src/seg2map/exceptions.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.6/src/seg2map/log_maker.py` & `seg2map-0.0.7/src/seg2map/log_maker.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.6/src/seg2map/map_UI.py` & `seg2map-0.0.7/src/seg2map/map_UI.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from ipywidgets import DatePicker
 from ipywidgets import HTML
 from ipywidgets import RadioButtons
 from ipywidgets import Text
 from ipywidgets import Output
 from ipywidgets import FloatSlider
 from ipywidgets import SelectionSlider
+from ipywidgets import Dropdown
 
 
 logger = logging.getLogger(__name__)
 
 
 def create_file_chooser(callback, title: str = None):
     padding = "0px 0px 0px 5px"  # upper, right, bottom, left
@@ -130,26 +131,22 @@
         dates_vbox = self.get_dates_picker()
         self.sitename_field = Text(
             value="sitename",
             placeholder="Type sitename",
             description="Sitename:",
             disabled=False,
         )
-
-        img_type_picker = self.get_image_types_picker()
-
         settings_button = Button(description="Save Settings", style=self.action_style)
         settings_button.on_click(self.save_settings_clicked)
 
         # create settings vbox
         settings_vbox = VBox(
             [
                 dates_vbox,
                 self.sitename_field,
-                img_type_picker,
                 settings_button,
                 UI.settings_messages,
             ]
         )
 
         return settings_vbox
 
@@ -166,28 +163,14 @@
             disabled=False,
         )
         date_instr = HTML(value="<b>Pick a date:</b>", layout=Layout(padding="10px"))
         dates_box = HBox([self.start_date, self.end_date])
         dates_vbox = VBox([date_instr, dates_box])
         return dates_vbox
 
-    def get_image_types_picker(self) -> VBox:
-        image_types = ["multiband", "singleband", "both"]
-        self.img_type_radio = RadioButtons(
-            options=image_types,
-            value=image_types[0],
-            description="",
-            disabled=False,
-        )
-        instr = HTML(
-            value="<b>Pick type of imagery:</b>", layout=Layout(padding="10px")
-        )
-        img_type_vbox = HBox([instr, self.img_type_radio])
-        return img_type_vbox
-
     def remove_buttons(self):
         # define remove feature radio box button
         remove_instr = HTML(
             value="<h2>Remove Feature from Map</h2>",
             layout=Layout(padding="0px"),
         )
         self.remove_button = Button(description=f"Remove ROIs", style=self.remove_style)
@@ -214,14 +197,26 @@
 
     def segmentation_controls(self):
         # define remove feature radio box button
         instr = HTML(
             value="<h2>Load Segmentations on the Map</h2>",
             layout=Layout(padding="0px"),
         )
+        inital_options = ["all"]
+        classes = list(self.seg2map.get_classes())
+        classes = ["all"] + classes
+        if len(self.seg2map.get_classes()) == 0:
+            classes = inital_options
+        self.class_dropdown = Dropdown(
+            options=classes,
+            description="Select Class:",
+            value=classes[0],
+            style={"description_width": "initial"},
+        )
+
         self.load_segmentations_button = Button(
             description="Load Segmentations", style=self.load_style
         )
         self.load_segmentations_button.on_click(self.on_load_session_clicked)
 
         self.opacity_slider = FloatSlider(
             value=1.0,
@@ -232,84 +227,111 @@
             disabled=False,
             continuous_update=False,
             orientation="horizontal",
             readout=True,
             readout_format=".2f",
         )
 
-        years = ["2010", "2012", "2013", "2015"]
+        default_years = ["2021"]
+        years = self.seg2map.get_years()
+        if len(years) == 0:
+            years = default_years
         self.year_slider = SelectionSlider(
             options=years,
             value=years[0],
             description="Select a year:",
             disabled=False,
             continuous_update=False,
             orientation="horizontal",
             readout=True,
         )
 
         def year_slider_changed(change):
             year = self.year_slider.value
-            for layer in self.seg2map.original_layers + self.seg2map.seg_layers:
-                # if year in layer name and layer not on map
-                if (
-                    year in layer.name
-                    and self.seg2map.map.find_layer(layer.name) is None
-                ):
-                    self.seg2map.map.add_layer(layer)
-                if year not in layer.name and layer.name != "ROI":
-                    if layer in self.seg2map.map.layers:
-                        self.seg2map.map.remove_layer(layer)
+            seg_layers = self.seg2map.get_seg_layers()
+            original_layers = self.seg2map.get_original_layers()
+            # order matters: original layers must be before seg layer otherwise so segmentations will appear on to of image
+            layers = original_layers + seg_layers
+            self.seg2map.load_layers_by_year(layers, year)
 
         self.year_slider.observe(year_slider_changed, "value")
 
         def opacity_slider_changed(change):
+            # apply opacity to all layers
             year = self.year_slider.value
-            layer_name = ""
-            for layer in self.seg2map.seg_layers:
-                if year in layer.name:
-                    layer_name = layer.name
-
-            value = self.opacity_slider.value
-            if layer_name != "":
-                self.seg2map.map.layer_opacity(layer_name, value)
+            opacity = self.opacity_slider.value
+            logger.info(f"self.class_dropdown.value: {self.class_dropdown.value}")
+            print(f"self.class_dropdown.value: {self.class_dropdown.value}")
+            logger.info(f"year: {year}")
+            print(f"year: {year}")
+            if self.class_dropdown.value == "all":
+                seg_layers = self.seg2map.get_seg_layers()
+            if self.class_dropdown.value != "all":
+                # apply opacity to selected layer name
+                seg_layers = self.seg2map.get_seg_layers(self.class_dropdown.value)
+
+            if seg_layers == []:
+                return
+            self.seg2map.modify_layers_opacity_by_year(seg_layers, year, opacity)
 
         self.opacity_slider.observe(opacity_slider_changed, "value")
 
+        def handle_class_dropdown(change):
+            # apply opacity to all layers
+            logger.info(f"handle_class_dropdown: {change['new']}")
+            print(f"handle_class_dropdown: {change['new']}")
+            if change["new"] == "all":
+                year = self.year_slider.value
+                seg_layers = self.seg2map.get_seg_layers()
+                logger.info(f"seg_layers: {seg_layers}")
+                if seg_layers == []:
+                    return
+                opacity = self.opacity_slider.value
+                self.seg2map.modify_layers_opacity_by_year(seg_layers, year, opacity)
+            if change["new"] != "all":
+                # apply opacity to selected layer name
+                year = self.year_slider.value
+                seg_layers = self.seg2map.get_seg_layers(change["new"])
+                logger.info(f"seg_layers: {seg_layers}")
+                if seg_layers == []:
+                    return
+                opacity = self.opacity_slider.value
+                self.seg2map.modify_layers_opacity_by_year(seg_layers, year, opacity)
+
+        self.class_dropdown.observe(handle_class_dropdown, "value")
+
+        opacity_controls = HBox([self.opacity_slider, self.class_dropdown])
         segmentation_box = VBox(
             [
                 instr,
                 self.load_segmentations_button,
                 self.year_slider,
-                self.opacity_slider,
+                opacity_controls,
             ]
         )
         return segmentation_box
 
     def get_settings_html(
         self,
         settings: dict,
     ):
         # Modifies setttings html
         default = "unknown"
         keys = [
             "dates",
             "sitename",
-            "download_bands",
         ]
         values = defaultdict(lambda: "unknown", settings)
         return """ 
         <h2>Settings</h2>
         <p>dates: {}</p>
         <p>sitename: {}</p>
-        <p>download_bands: {}</p>
         """.format(
             values["dates"],
             values["sitename"],
-            values["download_bands"],
         )
 
     def _create_HTML_widgets(self):
         """create HTML widgets that display the instructions.
         widgets created: instr_create_ro, instr_save_roi, instr_load_btns
          instr_download_roi
         """
@@ -411,18 +433,17 @@
             self.settings_html.value = self.get_settings_html(self.seg2map.settings)
         except Exception as error:
             exception_handler.handle_exception(error, self.seg2map.warning_box)
 
     @settings_messages.capture(clear_output=True)
     def save_settings_clicked(self, btn):
         # Save dates selected by user
-        image_type = str(self.img_type_radio.value)
         dates = [str(self.start_date.value), str(self.end_date.value)]
         sitename = self.sitename_field.value.replace(" ", "")
-        settings = {"dates": dates, "sitename": sitename, "download_bands": image_type}
+        settings = {"dates": dates, "sitename": sitename}
         dates = [datetime.datetime.strptime(_, "%Y-%m-%d") for _ in dates]
         if dates[1] <= dates[0]:
             print("Dates are not correct chronological order")
             print("Settings not saved")
             return
         # check if sitename path exists and if it does tell user they need a new name
         parent_path = os.path.join(os.getcwd(), "data")
@@ -478,22 +499,23 @@
     @debug_view.capture(clear_output=True)
     def on_load_session_clicked(self, button):
         # Prompt user to select a config geojson file
         def load_callback(filechooser: FileChooser) -> None:
             try:
                 if filechooser.selected:
                     self.seg2map.load_session(filechooser.selected)
-                    if self.seg2map.years == []:
-                        self.year_slider.disabled = True
-                        self.opacity_slider.disabled = True
-                    elif self.seg2map.years != []:
-                        self.year_slider.disabled = False
-                        self.opacity_slider.disabled = False
-                        self.year_slider.options = self.seg2map.years
-                        self.year_slider.value = self.seg2map.years[0]
+                    years = self.seg2map.years
+                    classes = self.seg2map.get_classes()
+                    classes = list(classes)
+                    if classes:
+                        self.class_dropdown.options = ["all"] + classes
+                        self.class_dropdown.value = classes[0]
+                    if years:
+                        self.year_slider.options = years
+                        self.year_slider.value = years[0]
 
             except Exception as error:
                 # renders error message as a box on map
                 exception_handler.handle_exception(error, self.seg2map.warning_box)
 
         # create instance of chooser that calls load_callback
         dir_chooser = common.create_dir_chooser(
@@ -547,17 +569,15 @@
         self.clear_row(self.file_chooser_row)
         # add instance of file_chooser to file_chooser_row
         self.file_chooser_row.children = [file_chooser]
 
     @debug_view.capture(clear_output=True)
     def on_save_config_clicked(self, button):
         try:
-            print("Save config clicked")
             self.seg2map.save_config()
-            print("Done!")
         except Exception as error:
             # renders error message as a box on map
             exception_handler.handle_exception(error, self.seg2map.warning_box)
 
     @debug_view.capture(clear_output=True)
     def remove_feature_from_map(self, btn):
         UI.debug_view.clear_output(wait=True)
```

### Comparing `seg2map-0.0.6/src/seg2map/map_interface.py` & `seg2map-0.0.7/src/seg2map/map_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 import os
 import pathlib
 from glob import glob
 import json
 import logging
-from typing import List
+from typing import List, Optional
 from collections import defaultdict
 from datetime import datetime
 from typing import Union
 
 from seg2map import common
 from seg2map.roi import ROI
 from seg2map import exceptions
 from seg2map import exception_handler
 from seg2map import downloads
+from seg2map import map_functions
+from seg2map import sessions
 
 import geopandas as gpd
 import tqdm
 import tqdm.auto
 from ipyleaflet import DrawControl, LayersControl, WidgetControl, GeoJSON
 from leafmap import Map
 from ipywidgets import Layout, HTML, Accordion
 from ipywidgets import ToggleButton
 from ipywidgets import HBox
 from ipywidgets import VBox
 from ipywidgets import HTML
+import ipyleaflet
 
 
 logger = logging.getLogger(__name__)
 
 
 class Seg2Map:
     def __init__(self):
         # settings:  used to select data to download and preprocess settings
         self.settings = {
             "dates": "",
             "sitename": "",
         }
         # segmentation layers for each year
         self.seg_layers = []
+        # years: available years to show for segmentations
+        self.years = []
+        # segmentation data associated with each ROI
+        self.roi_segmentations = {}
+        # classes : all classes available for segmentations
+        self.classes = set()
         # original imagery layers for each year
         self.original_layers = []
         # year that have imagery downloaded
         self.years = []
         # selected_set set(str): ids of the selected rois
         self.selected_set = set()
         # selected_set set(str): ids of rois selected for deletion
@@ -66,14 +75,97 @@
         self.remove_box = HBox([])
         self.action_widget = WidgetControl(widget=self.remove_box, position="topleft")
         self.map.add(self.action_widget)
         self.warning_box = HBox([])
         self.warning_widget = WidgetControl(widget=self.warning_box, position="topleft")
         self.map.add(self.warning_widget)
 
+    def get_original_layers(
+        self, layer_name: Optional[str] = None
+    ) -> Union[ipyleaflet.Layer, list[ipyleaflet.Layer], None]:
+        """
+        Returns the first matching original layer with the specified name, or all original layers if no name is given.
+
+        Args:
+            layer_name (str, optional): The name of the layer to look for. If not specified, returns all original layers.
+
+        Returns:
+            ipyleaflet.Layer or list[ipyleaflet.Layer] or None: The first matching layer, or all layers if no name is given.
+            Returns None if no layer is found.
+
+        Examples:
+            # Get the original layer with name "My Layer"
+            my_layer = get_original_layers("My Layer")
+
+            # Get all original layers
+            all_layers = get_original_layers()
+        """
+        matching_layers = []
+        if layer_name is not None:
+            for layer in self.seg_layers:
+                if layer_name in layer.name:
+                    matching_layers.append(layer)
+            return matching_layers
+        else:
+            return self.original_layers
+
+    def get_seg_layers(self, layer_name: Optional[str] = None) -> List:
+        """
+        Returns the first matching segmentation layer with the specified name, or all segmentation layers if no name is given.
+
+        Args:
+            layer_name (str, optional): The name of the layer to look for. If not specified, returns all segmentation layers.
+
+        Returns:
+            ipyleaflet.Layer or list[ipyleaflet.Layer]: The first matching layer, or all layers if no name is given. Returns None if no layer is found.
+
+        Examples:
+            # Get the segmentation layer with name "My Layer"
+            my_layer = get_seg_layer("My Layer")
+
+            # Get all segmentation layers
+            all_layers = get_seg_layer()
+        """
+        matching_layers = []
+        if layer_name is not None:
+            for layer in self.seg_layers:
+                if layer_name in layer.name:
+                    matching_layers.append(layer)
+            return matching_layers
+        else:
+            return self.seg_layers
+
+    def get_roi_segmentations(self):
+        return self.roi_segmentations.copy()
+
+    def set_roi_segmentations(
+        self, roi_id: str, years: List[str], classes: List[str]
+    ) -> None:
+        """Sets the segmentation information for a given ROI.
+
+        Args:
+            roi_id (str): The ID of the ROI.
+            years (List[str]): The years for which segmentation data is available.
+            classes (List[str]): The classes for which segmentation data is available.
+        """
+        classes = list(classes)
+        self.roi_segmentations[roi_id] = {"years": years, "classes": classes}
+
+    def get_classes(self, roi_id=None):
+        if roi_id:
+            classes = self.get_roi_segmentations()[roi_id]["classes"]
+            classes = set(classes)
+            return classes
+        return self.classes
+
+    def get_years(self, roi_id=None):
+        if roi_id:
+            return self.get_roi_segmentations()[roi_id]["years"]
+        return self.years
+
     def get_setttings(self) -> dict:
         logger.info(f"settings: {self.settings}")
 
         if self.settings["sitename"] == "":
             raise Exception("No sitename given")
 
         dates = self.settings["dates"]
@@ -82,97 +174,199 @@
         elif dates != "":
             dates = [datetime.strptime(_, "%Y-%m-%d") for _ in dates]
             if dates[1] <= dates[0]:
                 raise Exception("Dates are not correct chronological order")
 
         return self.settings
 
+    def load_session_layers(self, session_path: str, classes: List[str], roi_id: str):
+        # load model_settings and read roi directory from it
+        model_settings_path = os.path.join(session_path, "model_settings.json")
+        model_settings = common.read_json_file(model_settings_path)
+        roi_path = model_settings.get("sample_direc", "")
+        if not roi_path:
+            raise ValueError(
+                f"model_settings.json is missing sample_direc. {model_settings_path}"
+            )
+
+        roi_directory = pathlib.Path(model_settings["sample_direc"])
+        # if the directory name is 'tiles' chdir to the parent directory
+        if "tile" in os.path.basename(roi_directory):
+            roi_directory = os.path.dirname(roi_directory)
+        # Load original imagery on map
+        original_jpg_path = os.path.join(roi_directory, "merged_multispectral.jpg")
+        original_tif_path = os.path.join(roi_directory, "merged_multispectral.tif")
+        if not os.path.isfile(original_jpg_path):
+            logger.warning(f"Does not exist {original_jpg_path}")
+            return
+        if not os.path.isfile(original_tif_path):
+            logger.warning(f"Does not exist {original_tif_path}")
+            return
+        logger.info(f"original_jpg_path: {original_jpg_path}")
+        logger.info(f"original_tif_path: {original_tif_path}")
+        # create layer name in the form of {image_name}{year}
+        year_name = os.path.basename(session_path)
+        layer_name = f"{roi_id}_{year_name}"
+        new_layer = common.get_image_overlay(
+            str(original_tif_path),
+            str(original_jpg_path),
+            layer_name,
+            convert_RGB=True,
+            file_format="jpeg",
+        )
+        if new_layer:
+            self.original_layers.append(new_layer)
+        # create layers for each class present in greyscale tiff
+        class_layers = map_functions.get_class_layers(
+            session_path, classes, year_name, roi_id
+        )
+        if class_layers:
+            self.seg_layers.extend(class_layers)
+
     def load_session(self, session_path: str) -> None:
         """
         Loads a session onto the map, containing the segmented imagery and a model settings.json file that contains a reference to the original imagery.
+        """
+        self.map.default_style = {"cursor": "wait"}
+        session_path = os.path.abspath(session_path)
+
+        session = sessions.Session()
+        session.load(session_path)
+        classes = list(session.classes)
+        years = list(session.years)
+        roi_ids = list(session.roi_ids)
+        if not years:
+            raise Exception(f"No year directories found in session {session_path}")
+        if not classes:
+            raise ValueError(f"Session is missing classes {session_path}")
+        if not roi_ids:
+            raise ValueError(f"No ROI directories found in session. {session_path}")
+
+        self.classes = sorted(classes)
+        self.years = sorted(years)
+
+        # if selected path is not the session name then an ROI directory was selected
+        logger.info(f"session_path: {session_path}")
+        logger.info(f"os.path.basename(session_path): {os.path.basename(session_path)}")
+        logger.info(f"session.name: {session.name}")
+
+        if session.name != os.path.basename(session_path):
+            roi_id = os.path.basename(session_path)
+            self.set_roi_segmentations(roi_id, years, classes)
+            top_level_directories = [
+                os.path.join(session_path, d)
+                for d in os.listdir(session_path)
+                if os.path.isdir(os.path.join(session_path, d))
+            ]
+            logger.info(f"top_level_directories: {top_level_directories}")
+            for session_year_path in top_level_directories:
+                self.load_session_layers(session_year_path, classes, roi_id)
+
+        else:
+            for roi_id in roi_ids:
+                self.set_roi_segmentations(roi_id, years, classes)
+                session_roi_directory = os.path.join(session_path, roi_id)
+                top_level_directories = [
+                    os.path.join(session_roi_directory, d)
+                    for d in os.listdir(session_roi_directory)
+                    if os.path.isdir(os.path.join(session_roi_directory, d))
+                ]
+                logger.info(f"top_level_directories: {top_level_directories}")
+                for session_year_path in top_level_directories:
+                    self.load_session_layers(session_year_path, classes, roi_id)
+
+        # get lists of original and segmentation layers for imagery
+        original_layers = self.get_original_layers()
+        seg_layers = self.get_seg_layers()
+
+        # By default load first available year of segmentations on the map
+        if len(original_layers) == 0:
+            logger.error(f"No imagery to load on map")
+            raise Exception(f"No imagery to load on map")
+        if len(seg_layers) == 0:
+            logger.warning(f"No segmentations to load on map")
+        # Display first available year by default
+        year = original_layers[0].name.split("_")[-1]
+        layers = original_layers + seg_layers
+        self.load_layers_by_year(layers, year)
+        self.map.default_style = {"cursor": "default"}
+
+    def load_layers_by_year(self, layers: List[ipyleaflet.Layer], year: str) -> None:
+        # load layers on map if year is in layer name
+        # remove layers where year is not in layer name
+        # make sure layer name does not contain 'ROI'
+        year = str(year)
+        if len(layers) == 0:
+            logger.warning(f"No imagery to load on map for year {year}:{layers}")
+        # load layers on map by year
+        for layer in layers:
+            # load the layer on the map if layer name contains year and layer not on map
+            if year in layer.name and self.map.find_layer(layer.name) is None:
+                self.map.add_layer(layer)
+            if year not in layer.name and layer.name != "ROI":
+                if layer in self.map.layers:
+                    self.map.remove_layer(layer)
+
+    def modify_layers_opacity_by_year(
+        self, layers: list, year: str = "", opacity: float = 1.0
+    ) -> None:
+        """
+        Modifies the opacity of all layers in the given list whose name contains the specified year.
 
         Args:
-            session_path: str - The path to the session directory containing the segmented imagery and model settings file.
+            layers (list): A list of layers to modify.
+            year (str, optional): The year to match against layer names. Default is an empty string, which matches all layers.
+            opacity (float, optional): The opacity value to set for the matching layers. Default is 1.0 (fully opaque).
 
         Returns:
-            None.
+            None: This function doesn't return anything.
+
+        Examples:
+            # Set opacity to 0.5 for all layers with "2020" in their name
+            modify_layers_opacity_by_year(layers, "2020", 0.5)
         """
-        self.map.default_style = {"cursor": "wait"}
+        year = str(year)
+        # for each layer with year in its name modify the opacity
+        for layer in layers:
+            # load the layer on the map if layer name contains year and layer not on map
+            if year in layer.name:
+                self.modify_layer_opacity(layer, opacity)
 
-        session_path = pathlib.Path(session_path)
-        for year_path in session_path.glob("*"):
-            if not year_path.is_dir():
-                continue
-
-            logger.info(f"year_path: {year_path}")
-            merged_tif_path = year_path.glob("*merged_multispectral.tif*")
-            merged_tif_path = next(merged_tif_path, None)
-            if merged_tif_path is None:
-                logger.warning(
-                    f"Does not exist {os.path.join(year_path, '*merged_multispectral.tif*')}"
-                )
-                continue
-            logger.info(f"merged_tif_path: {merged_tif_path}")
+    def modify_layer_opacity(
+        self, layer: ipyleaflet.Layer, opacity: float = 1.0
+    ) -> None:
+        """
+        Modifies the opacity of the specified layer on a map.
 
-            # Load original imagery on map
-            model_settings_path = year_path / "model_settings.json"
-            model_settings = common.read_json_file(model_settings_path)
-
-            roi_directory = pathlib.Path(model_settings["sample_direc"])
-            original_jpg_path = roi_directory / "merged_multispectral.jpg"
-            original_tif_path = roi_directory / "merged_multispectral.tif"
-            if not original_jpg_path.is_file():
-                logger.warning(f"Does not exist {original_jpg_path}")
-                continue
-            if not original_tif_path.is_file():
-                logger.warning(f"Does not exist {original_tif_path}")
-                continue
-            logger.info(f"original_jpg_path: {original_jpg_path}")
-            logger.info(f"original_tif_path: {original_tif_path}")
-            layer_name = f"{merged_tif_path.stem}_{year_path.name}"
-            logger.info(f"layer_name: {layer_name}")
-            new_layer = common.get_image_overlay(
-                str(original_tif_path), str(original_jpg_path), layer_name
-            )
-            self.original_layers.append(new_layer)
+        Args:
+            layer (ipyleaflet.Layer): The layer to modify.
+            opacity (float, optional): The opacity value to set for the layer, between 0.0 (fully transparent) and 1.0 (fully opaque).
+                Default is 1.0.
 
-            # Load segmentation on map
-            jpg_path = year_path.glob("*merged_multispectral.jp*g*")
-            jpg_path = next(jpg_path, None)
-            if jpg_path is None:
-                logger.warning(
-                    f"Does not exist {os.path.join(year_path, '*merged_multispectral.jp*g*')}"
-                )
-                continue
-            logger.info(f"jpg_path: {jpg_path}")
-            layer_name = f"{merged_tif_path.stem}_segmentation_{year_path.name}"
-            logger.info(f"layer_name: {layer_name}")
-            new_layer = common.get_image_overlay(
-                str(merged_tif_path), str(jpg_path), layer_name
-            )
-            self.seg_layers.append(new_layer)
-            self.years.append(year_path.name)
+        Returns:
+            None: This function doesn't return anything.
 
-        # Display first year by default
-        if self.original_layers != []:
-            print(self.map.find_layer(self.original_layers[0].name))
-            self.map.add_layer(self.original_layers[0])
-        if self.seg_layers != []:
-            self.map.add_layer(self.seg_layers[0])
-        self.map.default_style = {"cursor": "default"}
+        Raises:
+            TypeError: If the `layer` argument is not an instance of `ipyleaflet.Layer`.
+            ValueError: If the layer is not found on the map.
+
+        Examples:
+            # Set opacity to 0.5 for the layer with name "My Layer"
+            my_layer = ipyleaflet.TileLayer(name="My Layer")
+            modify_layer_opacity(my_layer, 0.5)
+        """
+        if isinstance(layer, ipyleaflet.Layer):
+            if self.map.find_layer(layer.name):
+                self.map.layer_opacity(layer.name, opacity)
 
     def download_imagery(
         self,
     ) -> None:
         """Download imagery for the selected ROIs on the map.
 
-        Args:
-            download_bands (str): The type of imagery to download. Defaults to "multiband".
-            Possible options: "multiband", "singleband" or "both"
-
         Raises:
             exceptions.Object_Not_Found: If no ROIs exist.
             Exception: If the sitename in settings already exists.
 
         This function checks for the existence of ROIs and selected sets, gets the settings used to download the ROIs,
         creates a directory to store the downloads, downloads the selected ROIs to the directory, and deletes any empty
         directories. Finally, it saves the configuration.
@@ -187,20 +381,17 @@
         # get settings used to download ROIs
         settings = self.get_setttings()
         # create directory named sitename within data directory in current working directory to hold all downloads
         site_path = common.get_site_path(settings)
         logger.info(
             f"Download in process.\nsitepath: {site_path}\nselected ids:{selected_ids}"
         )
-        # select number of bands to download
-        download_bands = settings["download_bands"]
         # download all selected ROIs on map to sitename directory
         print("Download in process")
 
-        # refactor_downloads.prepare_ROI_for_download()
         roi_paths = []
         with common.Timer():
             for roi_id in selected_ids:
                 roi_path = downloads.create_ROI_directories(
                     site_path, roi_id, settings["dates"]
                 )
                 roi_paths.append(roi_path)
@@ -219,34 +410,14 @@
             downloads.run_async_function(downloads.download_ROIs, ROI_tiles=ROI_tiles)
 
         self.save_config()
 
         # create merged multispectural for each year in each ROI
         common.create_merged_multispectural_for_ROIs(roi_paths)
 
-        # # create multispectral tif for each year only if multiband imagery was downloaded
-
-        # if download_bands != "singleband":
-        #     for dir_name in tqdm.auto.tqdm(
-        #         os.listdir(site_path),
-        #         desc="Merging tifs for all ROI",
-        #         leave=False,
-        #         unit_scale=True,
-        #     ):
-        #         roi_path = os.path.join(site_path, dir_name)
-        #         multiband_path = os.path.join(roi_path, "multiband")
-        #         for dir_name in tqdm.auto.tqdm(
-        #             os.listdir(multiband_path),
-        #             desc="Merging tifs per year",
-        #             leave=False,
-        #             unit_scale=True,
-        #         ):
-        #             dir_path = os.path.join(multiband_path, dir_name)
-        #             common.merge_tifs(multiband_path=dir_path, roi_path=dir_path)
-
     def create_delete_box(self, title: str = None, msg: str = None):
         padding = "0px 5px 0px 5px"  # upper, right, bottom, left
         # create title
         if title is None:
             title = "Delete Selected ROIs?"
         warning_title = HTML(f"<b>⚠️<u>{title}</u></b>")
         # create msg
```

### Comparing `seg2map-0.0.6/src/seg2map/models_UI.py` & `seg2map-0.0.7/src/seg2map/models_UI.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # standard python imports
 import os
-import glob
 import logging
 
 # internal python imports
 from seg2map import common
 from seg2map import zoo_model
 
 # external python imports
@@ -59,30 +58,14 @@
     return chooser
 
 
 class UI_Models:
     # all instances of UI will share the same debug_view
     model_view = Output()
     run_model_view = Output()
-    # uav_RGB_10class_7566797: https://zenodo.org/record/7566797
-    # uav_RGB_10class_7566810: https://zenodo.org/record/7566810
-    # CoastTrain
-    # ortho_RGB_8class_7574784: https://zenodo.org/record/7574784
-    # naip_RGB_5class_7566992: https://zenodo.org/record/7566992
-    # naip_RGB_8class_7570583: https://zenodo.org/record/7570583
-    # CHESAPEAKE
-    # ortho_RGB_7class_7576904:  https://zenodo.org/record/7576904
-    # OPEN EARTH NET
-    # ortho_RGB_9class_7576894: https://zenodo.org/record/7576894
-    # DeepGlobe
-    # ortho_RGB_7clas_7576898 https://zenodo.org/record/7576898
-    # EnviroAtlas
-    # ortho_RGB_6class_7576909 https://zenodo.org/record/7576909
-    # AAAI-Buildings
-    # ortho_RGB_7class_7607895 https://zenodo.org/record/7607895
 
     def __init__(self):
         # Controls size of ROIs generated on map
         self.model_dict = {
             "sample_direc": None,
             "use_GPU": "0",
             "implementation": "BEST",
@@ -162,15 +145,15 @@
         session_name_controls = HBox([self.session_name_text, enter_button])
         return VBox([session_name_controls, output])
 
     def create_dashboard(self):
         model_choices_box = HBox(
             [self.model_type_dropdown, self.model_dropdown, self.model_implementation]
         )
-        checkboxes = HBox([self.GPU_checkbox, self.otsu_radio, self.tta_radio])
+        checkboxes = HBox([self.otsu_radio, self.tta_radio])
         instr_vbox = VBox(
             [
                 self.instr_select_images,
                 self.instr_run_model,
             ]
         )
         self.file_row = HBox([])
@@ -345,26 +328,25 @@
         # Disable run and open results buttons while the model is running
         # self.open_results_button.disabled = True
         # self.run_model_button.disabled = True
 
         # gets GPU or CPU depending on whether use_GPU is True
         use_GPU = self.model_dict["use_GPU"]
         model_implementation = self.model_dict["implementation"]
-        model_name = self.model_dict["model_type"]
+        model_id = self.model_dict["model_type"]
         use_otsu = self.model_dict["otsu"]
         use_tta = self.model_dict["tta"]
 
-        zoo_model.get_GPU(use_GPU)
-        zoo_model_instance = zoo_model.Zoo_Model()
+        zoo_model_instance = zoo_model.ZooModel()
 
         zoo_model_instance.run_model(
             model_implementation,
             session_name=session_name,
             src_directory=inputs_directory,
-            model_name=model_name,
+            model_id=model_id,
             use_GPU=use_GPU,
             use_otsu=use_otsu,
             use_tta=use_tta,
         )
         # # Enable run and open results buttons when model has executed
         # self.run_model_button.disabled = False
         # self.open_results_button.disabled = False
```

### Comparing `seg2map-0.0.6/src/seg2map/roi.py` & `seg2map-0.0.7/src/seg2map/roi.py`

 * *Files identical despite different names*

### Comparing `seg2map-0.0.6/src/seg2map/zoo_model.py` & `seg2map-0.0.7/src/seg2map/zoo_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
+from typing import List, Set
+import requests
+import logging
 import os
-import re
-import glob
 import shutil
-import asyncio
-import platform
 import json
-import logging
-from typing import List, Set
+from glob import glob
+
 from seg2map import common
-import requests
-import skimage
-import aiohttp
+from seg2map import downloads
+from seg2map import sessions
+from seg2map import map_functions
+
+from skimage.io import imsave
 import tqdm
 import numpy as np
-from glob import glob
+from osgeo import gdal
 import tqdm.asyncio
-import nest_asyncio
-from skimage.io import imread
-from tensorflow.keras import mixed_precision
 from doodleverse_utils.prediction_imports import do_seg
 from doodleverse_utils.model_imports import (
     simple_resunet,
     custom_resunet,
     custom_unet,
     simple_unet,
     simple_resunet,
@@ -29,16 +27,14 @@
     segformer,
 )
 from doodleverse_utils.model_imports import dice_coef_loss, iou_multi, dice_multi
 import tensorflow as tf
 
 logger = logging.getLogger(__name__)
 
-from time import perf_counter
-
 
 def get_sorted_files_with_extension(
     sample_direc: str, file_extensions: List[str]
 ) -> List[str]:
     """
     Get a sorted list of paths to files that have one of the file_extensions.
     It will return the first set of files that matches the first file_extension, so put the
@@ -57,368 +53,155 @@
         filenames = sorted(tf.io.gfile.glob(os.path.join(sample_direc, f"*{ext}")))
         sample_filenames.extend(filenames)
         if sample_filenames:
             break
     return sample_filenames
 
 
-def get_merged_multispectural(src_path: str) -> str:
+def write_greylabel_to_png(npz_location: str) -> str:
     """
-    Merges multiple GeoTIFF files into a single VRT file and returns the path of the merged file.
-
-    This function looks for all GeoTIFF files in the specified directory, except for any files that contain the string "merged_multispectral" in their name. It groups the remaining files into batches of 4, and merges each batch into a separate VRT file. Finally, it merges all the VRT files into a single VRT file and returns the path of the merged file.
+    Given the path of an .npz file containing a 'grey_label' key with an array of uint8 values,
+    writes the array to a PNG file with the same name and location as the .npz file, with the extension
+    changed to .png. Returns the path of the PNG file.
 
     Parameters:
-    - src_path (str): The path of the directory containing the GeoTIFF files.
+    npz_location (str): The path of the .npz file to read from.
 
     Returns:
-    - The path of the merged VRT file.
+    str: The path of the written PNG file.
     """
-    year_name = os.path.basename(src_path)
-    tif_files = glob(os.path.join(src_path, "*.tif"))
-    tif_files = common.filter_files(tif_files, [r".*merged_multispectral.*"])
-    logger.info(
-        f"Found {len(tif_files)} GeoTIFF files in {src_path}.\n tif_files: {tif_files}"
-    )
-    merged_files = []
-    # old grouping strategy... doesn't really do anything
-    for idx, files in enumerate(common.group_files(tif_files, 6)):
-        filename = f"merged_multispectral_{idx}.vrt"
-        dst_path = os.path.join(src_path, filename)
-        merged_tif = common.merge_files(files, dst_path, create_jpg=False)
-        merged_files.append(merged_tif)
-
-    logger.info(f"merged_files {merged_files}")
-    dst_path = os.path.join(src_path, "merged_multispectral.vrt")
-    merged_file = common.merge_files(merged_files, dst_path)
-    # delete intermediate merged tifs and vrts
-    deleted_files = common.delete_files(
-        pattern=".*merged_multispectral_\d+.*", path=src_path
-    )
-    logger.info(f"deleted_files {deleted_files}")
-    return merged_file
-
-
-def time_func(func):
-    def wrapper(*args, **kwargs):
-        start = perf_counter()
-        result = func(*args, **kwargs)
-        end = perf_counter()
-        print(f"{func.__name__} took {end - start:.6f} seconds to run.")
-        return result
-
-    return wrapper
-
-
-def get_seg_files_by_year(dir_path: str) -> dict:
-    """
-    Returns a dictionary of segmentation files organized by year.
-
-    The function searches the specified directory and its subdirectories for
-    directories that are named as 4-digit years. For each year directory, it
-    finds all `.jpg` files that do not contain the string "merged_multispectral".
-
-    The returned dictionary has the year as the key and a dictionary as the value.
-    The value dictionary has two keys: "file_path" and "jpgs". "file_path" is the
-    full path of the year directory, and "jpgs" is a list of the full paths of
-    the `.jpg` files that meet the criteria.
+    png_path = npz_location.replace(".npz", ".png")
+    with np.load(npz_location) as data:
+        dat = 1 + np.round(data["grey_label"].astype("uint8"))
+    imsave(png_path, dat, check_contrast=False, compression=0)
+    return png_path
 
-    Args:
-    - dir_path (str): The directory to search for segmentation files.
 
-    Returns:
-    - dict: A dictionary of segmentation files organized by year.
+def create_greylabel_pngs(full_path: str) -> List[str]:
     """
-    files_per_year = {}
-    for root, dirs, files in os.walk(dir_path):
-        if root == dir_path:
-            continue
-        folder_name = os.path.basename(root)
-        if not re.match(r"^\d{4}$", folder_name):
-            continue
-        jpg_paths = sorted(tf.io.gfile.glob(os.path.join(root, "*.jpg")))
-        jpg_paths = [file for file in jpg_paths if "merged_multispectral" not in file]
-        files_per_year[folder_name] = {"file_path": root, "jpgs": jpg_paths}
-    return files_per_year
-
+    Given a directory path, finds all .npz files in the directory, writes the 'grey_label' array of each .npz
+    file to a corresponding PNG file, and returns a list of the paths of the written PNG files.
 
-def get_five_band_imagery(
-    RGB_path: str, MNDWI_path: str, NDWI_path: str, output_path: str
-):
-    paths = [RGB_path, MNDWI_path, NDWI_path]
-    files = []
-    for data_path in paths:
-        f = sorted(glob(data_path + os.sep + "*.jpg"))
-        if len(f) < 1:
-            f = sorted(glob(data_path + os.sep + "images" + os.sep + "*.jpg"))
-        files.append(f)
-
-    # number of bands x number of samples
-    files = np.vstack(files).T
-    # returns path to five band imagery
-    for counter, file in enumerate(files):
-        im = []  # read all images into a list
-        for k in file:
-            im.append(imread(k))
-        datadict = {}
-        # create stack which takes care of different sized inputs
-        im = np.dstack(im)
-        datadict["arr_0"] = im.astype(np.uint8)
-        datadict["num_bands"] = im.shape[-1]
-        datadict["files"] = [file_name.split(os.sep)[-1] for file_name in file]
-        ROOT_STRING = file[0].split(os.sep)[-1].split(".")[0]
-        segfile = (
-            output_path
-            + os.sep
-            + ROOT_STRING
-            + "_noaug_nd_data_000000"
-            + str(counter)
-            + ".npz"
-        )
-        np.savez_compressed(segfile, **datadict)
-        del datadict, im
-        logger.info(f"segfile: {segfile}")
-    return output_path
-
-
-def get_files(RGB_dir_path: str, img_dir_path: str):
-    """returns matrix of files in RGB_dir_path and img_dir_path
-    creates matrix: RGB x number of samples in img_dir_path
-    Example:
-    [['full_RGB_path.jpg','full_NIR_path.jpg'],
-    ['full_jpg_path.jpg','full_NIR_path.jpg']....]
-    Args:
-        RGB_dir_path (str): full path to directory of RGB images
-        img_dir_path (str): full path to directory of non-RGB images
-        usually NIR and SWIR
+    Parameters:
+    full_path (str): The path of the directory to search for .npz files.
 
-    Raises:
-        FileNotFoundError: raised if directory is not found
+    Returns:
+    List[str]: A list of the paths of the written PNG files.
     """
-    paths = [RGB_dir_path, img_dir_path]
-    files = []
-    for data_path in paths:
-        if not os.path.exists(data_path):
-            raise FileNotFoundError(f"{data_path} not found")
-        f = sorted(glob(data_path + os.sep + "*.jpg"))
-        if len(f) < 1:
-            f = sorted(glob(data_path + os.sep + "images" + os.sep + "*.jpg"))
-        files.append(f)
-    # creates matrix:  bands(RGB) x number of samples
-    files = np.vstack(files).T
-    return files
-
-
-def RGB_to_infrared(
-    RGB_path: str, infrared_path: str, output_path: str, output_type: str
-) -> None:
-    """Converts two directories of RGB and NIR imagery to NDWI imagery in a directory named
-     'NDWI' created at output_path.
-     imagery saved as jpg
-
-     to generate NDWI imagery set infrared_path to full path of NIR images
-     to generate MNDWI imagery set infrared_path to full path of SWIR images
-
-    Args:
-        RGB_path (str): full path to directory containing RGB images
-        infrared_path (str): full path to directory containing NIR or SWIR images
-        output_path (str): full path to directory to create NDWI/MNDWI directory in
-        output_type (str): 'MNDWI' or 'NDWI'
-    Based on code from doodleverse_utils by Daniel Buscombe
-    source: https://github.com/Doodleverse/doodleverse_utils
-    """
-    if output_type.upper() not in ["MNDWI", "NDWI"]:
-        logger.error(
-            f"Invalid output_type given must be MNDWI or NDWI. Cannot be {output_type}"
-        )
-        raise Exception(
-            f"Invalid output_type given must be MNDWI or NDWI. Cannot be {output_type}"
-        )
-    # matrix:bands(RGB) x number of samples(NIR)
-    files = get_files(RGB_path, infrared_path)
-    # output_path: directory to store MNDWI or NDWI outputs
-    output_path += os.sep + output_type.upper()
-    logger.info(f"output_path {output_path}")
-    if not os.path.exists(output_path):
-        os.mkdir(output_path)
-
-    for file in files:
-        # Read green band from RGB image and cast to float
-        green_band = skimage.io.imread(file[0])[:, :, 1].astype("float")
-        # Read infrared(SWIR or NIR) and cast to float
-        infrared = skimage.io.imread(file[1]).astype("float")
-        # Transform 0 to np.NAN
-        green_band[green_band == 0] = np.nan
-        infrared[infrared == 0] = np.nan
-        # Mask out NaNs
-        green_band = np.ma.filled(green_band)
-        infrared = np.ma.filled(infrared)
-
-        # ensure both matrices have equivalent size
-        if not np.shape(green_band) == np.shape(infrared):
-            gx, gy = np.shape(green_band)
-            nx, ny = np.shape(infrared)
-            # resize both matrices to have equivalent size
-            green_band = common.scale(
-                green_band, np.maximum(gx, nx), np.maximum(gy, ny)
-            )
-            infrared = common.scale(infrared, np.maximum(gx, nx), np.maximum(gy, ny))
-
-        # output_img(MNDWI/NDWI) imagery formula (Green - SWIR) / (Green + SWIR)
-        output_img = np.divide(infrared - green_band, infrared + green_band)
-        # Convert the NaNs to -1
-        output_img[np.isnan(output_img)] = -1
-        # Rescale to be between 0 - 255
-        output_img = common.rescale_array(output_img, 0, 255)
-        # create new filenames by replacing image type(SWIR/NIR) with output_type
-        if output_type.upper() == "MNDWI":
-            new_filename = file[1].split(os.sep)[-1].replace("SWIR", output_type)
-        if output_type.upper() == "NDWI":
-            new_filename = file[1].split(os.sep)[-1].replace("NIR", output_type)
-
-        # save output_img(MNDWI/NDWI) as .jpg in output directory
-        skimage.io.imsave(
-            output_path + os.sep + new_filename,
-            output_img.astype("uint8"),
-            check_contrast=False,
-            quality=100,
-        )
-
-    return output_path
-
-
-async def fetch(session, url: str, save_path: str):
-    model_name = url.split("/")[-1]
-    # chunk_size: int = 128
-    chunk_size: int = 2048
-    async with session.get(url, raise_for_status=True) as r:
-        content_length = r.headers.get("Content-Length")
-        if content_length is not None:
-            content_length = int(content_length)
-            with open(save_path, "wb") as fd:
-                with tqdm.auto.tqdm(
-                    total=content_length,
-                    unit="B",
-                    unit_scale=True,
-                    unit_divisor=1024,
-                    desc=f"Downloading {model_name}",
-                    initial=0,
-                    ascii=False,
-                    position=0,
-                ) as pbar:
-                    async for chunk in r.content.iter_chunked(chunk_size):
-                        fd.write(chunk)
-                        pbar.update(len(chunk))
-        else:
-            with open(save_path, "wb") as fd:
-                async for chunk in r.content.iter_chunked(chunk_size):
-                    fd.write(chunk)
-
+    png_files = []
+    logger.info(f"full_path: {full_path}")
+    npzs = sorted(glob(os.path.join(full_path, "*.npz")))
+    logger.info(f"npzs: {npzs}")
+    for npz in npzs:
+        png_files.append(write_greylabel_to_png(npz))
+    return png_files
+
+
+def rename_xmls(src, old_name, new_name):
+    xml_files = sorted(glob(os.path.join(src, "*.xml")))
+    ## rename xmls
+    for xml_file in xml_files:
+        new_filename = xml_file.replace(old_name, new_name)
+        if not os.path.isfile(new_filename):
+            os.rename(xml_file, new_filename)
+
+
+def copy_xmls(src, dst):
+    ## copy the xml files into the 'out' folder
+    xml_files = sorted(glob(os.path.join(src, "*.xml")))
+    for xml_file in xml_files:
+        new_filename = xml_file.replace(src, dst)
+        if not os.path.isfile(new_filename):
+            shutil.copyfile(xml_file, new_filename)
+
+
+def remove_unused_files(outputs_path):
+    # Remove "prob.png" files
+    _ = [os.remove(k) for k in glob(os.path.join(outputs_path, "*prob.png"))]
+    # Remove "overlay.png" files ...
+    _ = [os.remove(k) for k in glob(os.path.join(outputs_path, "*overlay.png"))]
+
+
+def rename_predictions(predictions_location):
+    # find predictions and rename
+    # Get imgs list
+    predicition_pngs = sorted(glob(os.path.join(predictions_location, "*.png")))
+    # rename pngs
+    for prediction in predicition_pngs:
+        new_filename = prediction.replace("_predseg", "")
+        if not os.path.isfile(new_filename):
+            os.rename(prediction, new_filename)
 
-async def fetch_all(session, url_dict):
-    tasks = []
-    for save_path, url in url_dict.items():
-        task = asyncio.create_task(fetch(session, url, save_path))
-        tasks.append(task)
-    await tqdm.asyncio.tqdm.gather(*tasks)
-
-
-async def async_download_urls(url_dict: dict) -> None:
-    async with aiohttp.ClientSession() as session:
-        await fetch_all(session, url_dict)
-
-
-def run_async_download(url_dict: dict):
-    logger.info("run_async_download")
-    if platform.system() == "Windows":
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-    logger.info("Scheduling task")
-    # apply a nested loop to jupyter's event loop for async downloading
-    nest_asyncio.apply()
-    # get nested running loop and wait for async downloads to complete
-    loop = asyncio.get_running_loop()
-    result = loop.run_until_complete(async_download_urls(url_dict))
-    logger.info("Scheduled task")
-    logger.info(f"result: {result}")
-
-
-def get_GPU(num_GPU: str) -> None:
-    num_GPU = str(num_GPU)
-    if num_GPU == "0":
-        logger.info("Not using GPU")
-        print("Not using GPU")
-        # use CPU (not recommended):
-        os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
-    elif num_GPU == "1":
-        print("Using single GPU")
-        logger.info(f"Using 1 GPU")
-        # use first available GPU
-        os.environ["CUDA_VISIBLE_DEVICES"] = "1"
-    if int(num_GPU) == 1:
-        # read physical GPUs from machine
-        physical_devices = tf.config.experimental.list_physical_devices("GPU")
-        print(f"physical_devices (GPUs):{physical_devices}")
-        logger.info(f"physical_devices (GPUs):{physical_devices}")
-        if physical_devices:
-            # Restrict TensorFlow to only use the first GPU
-            try:
-                tf.config.experimental.set_visible_devices(physical_devices, "GPU")
-            except RuntimeError as e:
-                # Visible devices must be set at program startup
-                logger.error(e)
-                print(e)
-        # disable memory growth on all GPUs
-        for i in physical_devices:
-            tf.config.experimental.set_memory_growth(i, True)
-            print(f"visible_devices: {tf.config.get_visible_devices()}")
-            logger.info(f"visible_devices: {tf.config.get_visible_devices()}")
-        # if multiple GPUs are used use mirror strategy
-        if int(num_GPU) > 1:
-            # Create a MirroredStrategy.
-            strategy = tf.distribute.MirroredStrategy(
-                [p.name.split("/physical_device:")[-1] for p in physical_devices],
-                cross_device_ops=tf.distribute.HierarchicalCopyAllReduce(),
-            )
-            print(f"Number of distributed devices: {strategy.num_replicas_in_sync}")
-            logger.info(
-                f"Number of distributed devices: {strategy.num_replicas_in_sync}"
-            )
-
-
-def get_url_dict_to_download(models_json_dict: dict) -> dict:
-    """Returns dictionary of paths to save files to download
-    and urls to download file
 
-    ex.
-    {'C:\Home\Project\file.json':"https://website/file.json"}
+def make_greyscale_tif(tiles_location: str, tif_location: str) -> str:
+    """
+    Converts a set of tiled images into a greyscale mosaic TIFF file.
 
     Args:
-        models_json_dict (dict): full path to files and links
+    tiles_location (str): Path to the directory containing the input tiled images.
+    tif_location (str): Path to the directory where the output TIFF file will be saved.
 
     Returns:
-        dict: full path to files and links
+    str: The path to the generated greyscale mosaic TIFF file.
+
+    Raises:
+    None.
     """
-    url_dict = {}
-    for save_path, link in models_json_dict.items():
-        if not os.path.isfile(save_path):
-            url_dict[save_path] = link
-        json_filepath = save_path.replace("_fullmodel.h5", ".json")
-        if not os.path.isfile(json_filepath):
-            json_link = link.replace("_fullmodel.h5", ".json")
-            url_dict[json_filepath] = json_link
+    logger.info(f"tiles_location: {tiles_location}")
+    logger.info(f"tif_location: {tif_location}")
+    outputs_path = os.path.join(tiles_location, "out")
+    logger.info(f"outputs_path: {outputs_path}")
+    # copy xmls to the out folder
+    copy_xmls(tiles_location, outputs_path)
+    rename_xmls(outputs_path, ".jpg.aux.xml", ".png.aux.xml")
+    rename_predictions(outputs_path)
+    # create pngs from the npz files (segmentations)
+    imgsToMosaic = create_greylabel_pngs(outputs_path)
+    if len(imgsToMosaic) == 0:
+        logger.warning("No segmented images were found")
+        return ""
+    # rename the segmented images
+    rename_xmls(outputs_path, ".png", "_res.png")
+    outVRT = os.path.join(tif_location, "Mosaic_greyscale.vrt")
+    outTIF = os.path.join(tif_location, "Mosaic_greyscale.tif")
+    common.build_vrt(outVRT, imgsToMosaic, resampleAlg="mode")
+    # create greyscale tiff
+    common.build_tiff(outTIF, outVRT)
+    return outTIF
 
-    return url_dict
 
+def create_overlapping_tiles(
+    tif_path: str, tiles_path: str, OVERLAP_PX: int = None, TARGET_SIZE: int = 768
+):
+    # retile merged tif and create jpgs ready for model
+    if not OVERLAP_PX:
+        OVERLAP_PX = TARGET_SIZE // 2
+    # run retile script with system command. retiles merged_multispectral.tif to have overlap
+    cmd = f"python gdal_retile.py -r near -ot Byte -ps {TARGET_SIZE} {TARGET_SIZE} -overlap {OVERLAP_PX} -co 'tiled=YES' -targetDir {tiles_path} {tif_path}"
+    os.system(cmd)
+    tif_files = glob(os.path.join(tiles_path, "*.tif"))
+    kwargs = {"format": "JPEG", "outputType": gdal.GDT_Byte}
+    # create jpgs for new tifs
+    common.gdal_translate_jpegs(tif_files, kwargs=kwargs)
+    # delete tif files
+    for file in tif_files:
+        os.remove(file)
+    if len(os.listdir(tiles_path)) == 0:
+        return None
+    return tiles_path
 
-def download_url(url: str, save_path: str, chunk_size: int = 128):
+
+def download_url(
+    url: str, save_path: str, progress_bar_name: str = "", chunk_size: int = 1024
+):
     """Downloads the model from the given url to the save_path location.
     Args:
         url (str): url to model to download
         save_path (str): directory to save model
-        chunk_size (int, optional):  Defaults to 128.
+        chunk_size (int, optional):  Defaults to 1024.
     """
     logger.info(f"url: {url}")
     logger.info(f"save_path: {save_path}")
     # make an HTTP request within a context manager
     with requests.get(url, stream=True) as r:
         # check header to get content length, in bytes
         content_length = r.headers.get("Content-Length")
@@ -432,273 +215,243 @@
             content_length = int(content_length)
             with open(save_path, "wb") as fd:
                 with tqdm.auto.tqdm(
                     total=content_length,
                     unit="B",
                     unit_scale=True,
                     unit_divisor=1024,
-                    desc="Downloading Model",
+                    desc=progress_bar_name,
                     initial=0,
                     ascii=True,
                 ) as pbar:
                     for chunk in r.iter_content(chunk_size=chunk_size):
                         fd.write(chunk)
                         pbar.update(len(chunk))
 
 
-class Zoo_Model:
+def get_zenodo_release(zenodo_id: str) -> dict:
+    """
+    Retrieves the JSON data for the Zenodo release with the given ID.
+    """
+    root_url = f"https://zenodo.org/api/records/{zenodo_id}"
+    response = requests.get(root_url)
+    response.raise_for_status()
+    return response.json()
+
+
+def get_files_to_download(
+    available_files: List[dict], filenames: List[str], model_id: str, model_path: str
+) -> dict:
+    """Constructs a dictionary of file paths and their corresponding download links, based on the available files and a list of desired filenames.
+
+    Args:
+    - available_files: A list of dictionaries representing the metadata of available files, including the file key and download links.
+    - filenames: A list of strings representing the desired filenames.
+    - model_id: A string representing the ID of the model being downloaded.
+    - model_path: A string representing the path to the directory where the files will be downloaded.
+
+    Returns:
+    A dictionary with file paths as keys and their corresponding download links as values.
+    Raises a ValueError if any of the desired filenames are not available in the available_files list.
+    """
+    # make sure classes.txt file is downloaded
+    if isinstance(filenames, str):
+        filenames = [filenames]
+    url_dict = {}
+    for filename in filenames:
+        response = next((f for f in available_files if f["key"] == filename), None)
+        if response is None:
+            raise ValueError(f"Cannot find {filename} at {model_id}")
+        link = response["links"]["self"]
+        file_path = os.path.join(model_path, filename)
+        url_dict[file_path] = link
+    return url_dict
+
+
+def check_if_files_exist(files_dict: dict) -> dict:
+    """Checks if each file in a given dictionary of file paths and download links already exists in the local filesystem.
+
+    Args:
+    - files_dict: A dictionary with file paths as keys and their corresponding download links as values.
+
+    Returns:
+    A dictionary with file paths as keys and their corresponding download links as values, for any files that do not exist in the local filesystem.
+    """
+    url_dict = {}
+    for save_path, link in files_dict.items():
+        if not os.path.isfile(save_path):
+            url_dict[save_path] = link
+    return url_dict
+
+
+class ZooModel:
     def __init__(self):
-        self.weights_direc = None
+        self.model = None
+        self.weights_directory = ""
+        self.model_dict = {}
 
-    def get_files_for_seg(
-        self, sample_direc: str, avoid_patterns: List[str] = []
-    ) -> list:
-        """
-        Returns a list of files to be segmented.
+    def get_model_directory(self, model_id: str):
+        # Create a directory to hold the downloaded models
+        downloaded_models_path = self.get_downloaded_models_dir()
+        model_directory = common.create_directory(downloaded_models_path, model_id)
+        return model_directory
 
-        The function reads in the image filenames as either (`.npz`) OR (`.jpg`, or `.png`)
-        and returns a sorted list of the file paths.
+    def download_model(
+        self, model_choice: str, model_id: str, model_path: str = None
+    ) -> None:
+        """downloads model specified by zenodo id in model_id.
 
-        Args:
-        - sample_direc (str): The directory containing files to be segmented.
-        - avoid_patterns (List[str], optional): A list of file names to be avoided.Don't include any file extensions. Default is [].
+        Downloads best model is model_choice = 'BEST' or all models in
+        zenodo release if model_choice = 'ENSEMBLE'
 
-        Returns:
-        - list: A list of files to be segmented.
+        Args:
+            model_choice (str): 'BEST' or 'ENSEMBLE'
+            model_id (str): name of model followed by underscore zenodo_id ex.'orthoCT_RGB_2class_7574784'
+            model_path (str): path to directory to save the downloaded files to
         """
-        file_extensions = [".npz", ".jpg", ".png"]
-        sample_filenames = get_sorted_files_with_extension(
-            sample_direc, file_extensions
-        )
-        # filter out files whose filenames match any of the avoid_patterns
-        sample_filenames = common.filter_files(sample_filenames, avoid_patterns)
-        logger.info(f"files to seg: {sample_filenames}")
-        return sample_filenames
+        # Extract the Zenodo ID from the dataset ID
+        zenodo_id = model_id.split("_")[-1]
+        # get list of files available in zenodo release
+        json_content = get_zenodo_release(zenodo_id)
+        available_files = json_content["files"]
 
-    def create_model_data(self, directories: List[str], avoid_patterns: List[str] = []):
-        translateoptions = "-of JPEG -co COMPRESS=JPEG -co TFW=YES -co QUALITY=100"
-        for dir in directories:
-            files = glob(os.path.join(dir, ".tif"))
-            files = common.filter_files(files, avoid_patterns)
-            logger.info(f"Translating tifs to jpgs {files}")
-            common.gdal_translate_jpeg(files, translateoptions)
+        # Download the best model if best or all models if ensemble
+        if model_choice.upper() == "BEST":
+            self.download_best(available_files, model_path, model_id)
+        elif model_choice.upper() == "ENSEMBLE":
+            self.download_ensemble(available_files, model_path, model_id)
 
-    def create_jpgs_for_tifs(
-        self, directories: List[str], avoid_patterns: List["str"] = []
+    def download_best(
+        self, available_files: List[dict], model_path: str, model_id: str
     ):
         """
-        Creates JPEG files for TIF files in specified directories.
+        Downloads the best model file and its corresponding JSON and classes.txt files from the given list of available files.
 
         Args:
-            directories (List[str]): List of directory paths where TIF files are located.
-            avoid_patterns (List[str], optional): List of file names to exclude. Defaults to [].
+            available_files (list): A list of files available to download.
+            model_path (str): The local directory where the downloaded files will be stored.
+            model_id (str): The ID of the model being downloaded.
+
+        Raises:
+            ValueError: If BEST_MODEL.txt file is not found in the given model_id.
 
         Returns:
             None
         """
+        download_dict = {}
+        # download best_model.txt and read the name of the best model
+        best_model_json = next(
+            (f for f in available_files if f["key"] == "BEST_MODEL.txt"), None
+        )
+        if best_model_json is None:
+            raise ValueError(f"Cannot find BEST_MODEL.txt in {model_id}")
+        # download best model file to check if it exists
+        BEST_MODEL_txt_path = os.path.join(model_path, "BEST_MODEL.txt")
+        logger.info(f"model_path for BEST_MODEL.txt: {BEST_MODEL_txt_path}")
+        # if best BEST_MODEL.txt file not exist then download it
+        if not os.path.isfile(BEST_MODEL_txt_path):
+            download_url(
+                best_model_json["links"]["self"],
+                BEST_MODEL_txt_path,
+                progress_bar_name="Downloading best_model.txt",
+            )
 
-        translateoptions = "-of JPEG -co COMPRESS=JPEG -co TFW=YES -co QUALITY=100"
-        for directory in tqdm.auto.tqdm(
-            directories, desc="Convert .tif to .jpg", leave=False, unit_scale=True
-        ):
-            tif_files = self.get_tifs_missing_jpgs(directory, avoid_patterns)
-            if len(tif_files) == 0:
-                logger.info(
-                    f"All tifs in directory '{directory}' have corresponding jpgs."
-                )
-                continue
-            print(f"Converting tif files to jpgs in {directory}")
-            logger.info(f"Translating tifs to jpgs {tif_files}")
-            common.gdal_translate_jpeg(tif_files, translateoptions)
+        with open(BEST_MODEL_txt_path, "r") as f:
+            best_model_filename = f.read().strip()
+        # get the json data of the best model _fullmodel.h5 file
+        best_json_filename = best_model_filename.replace("_fullmodel.h5", ".json")
+        best_modelcard_filename = best_model_filename.replace(
+            "_fullmodel.h5", "_modelcard.json"
+        )
+
+        # download best model files(.h5, .json) file and classes.txt
+        download_filenames = [
+            "classes.txt",
+            best_json_filename,
+            best_model_filename,
+            best_modelcard_filename,
+        ]
+        download_dict.update(
+            get_files_to_download(
+                available_files, download_filenames, model_id, model_path
+            )
+        )
+
+        download_dict = check_if_files_exist(download_dict)
+        # download the files that don't exist
+        logger.info(f"URLs to download: {download_dict}")
+        # if any files are not found locally download them asynchronous
+        if download_dict != {}:
+            downloads.run_async_function(
+                downloads.async_download_url_dict, url_dict=download_dict
+            )
 
-    def get_tifs_missing_jpgs(
-        self, full_path: str, avoid_patterns: List[str] = []
-    ) -> List[str]:
+    def download_ensemble(
+        self, available_files: List[dict], model_path: str, model_id: str
+    ):
         """
-        Returns a list of TIF files in `full_path` that are missing corresponding JPG files.
+        Downloads all the model files and their corresponding JSON and classes.txt files from the given list of available files, for an ensemble model.
 
         Args:
-            full_path (str): The path to the directory containing the TIF files.
-            avoid_patterns (List[str]): A list of TIF file names to ignore.
+            available_files (list): A list of files available to download.
+            model_path (str): The local directory where the downloaded files will be stored.
+            model_id (str): The ID of the model being downloaded.
+
+        Raises:
+            Exception: If no .h5 files or corresponding .json files are found in the given model_id.
 
         Returns:
-            List[str]: A list of TIF file names that are missing corresponding JPG files.
+            None
         """
-        tif_files = glob(os.path.join(full_path, "*.tif"))
-        logger.info(f"all tif_files {tif_files}")
-        tif_files = common.filter_files(tif_files, avoid_patterns)
-        missing_jpgs = [
-            file
-            for file in tif_files
-            if not os.path.exists(file.replace(".tif", ".jpg"))
+        download_dict = {}
+        # get json and models
+        all_models_reponses = [f for f in available_files if f["key"].endswith(".h5")]
+        all_model_names = [f["key"] for f in all_models_reponses]
+        json_file_names = [
+            model_name.replace("_fullmodel.h5", ".json")
+            for model_name in all_model_names
         ]
-        logger.info(f"Tiffs missing_jpgs {missing_jpgs}")
-        return missing_jpgs
-
-    def run_model(
-        self,
-        model_implementation: str,
-        session_name: str,
-        src_directory: str,
-        model_name: str,
-        use_GPU: str,
-        use_otsu: bool,
-        use_tta: bool,
-    ):
-        logger.info(f"ROI directory: {src_directory}")
-        logger.info(f"session name: {session_name}")
-        logger.info(f"model_name: {model_name}")
-        logger.info(f"model_implementation: {model_implementation}")
-        logger.info(f"use_GPU: {use_GPU}")
-        logger.info(f"use_otsu: {use_otsu}")
-        logger.info(f"use_tta: {use_tta}")
-
-        self.download_model(model_implementation, model_name)
-        print("")
-        weights_list = self.get_weights_list(model_implementation)
-
-        # Load the model from the config files
-        model, model_list, config_files, model_types = self.get_model(weights_list)
-        metadatadict = self.get_metadatadict(weights_list, config_files, model_types)
-        logger.info(f"metadatadict: {metadatadict}")
-        model_dict = {
-            "sample_direc": None,
-            "use_GPU": use_GPU,
-            "implementation": model_implementation,
-            "model_type": model_name,
-            "otsu": False,
-            "tta": False,
-        }
-
-        session_path = common.create_directory(os.getcwd(), "sessions")
-        session_dir = common.create_directory(session_path, session_name)
-
-        search_pattern = r"config_gdf.*\.geojson"
-        parent_directory = os.path.dirname(src_directory)
-        print(f"parent_directory : {parent_directory }")
-        config_gdf_path = common.find_config_json(parent_directory, search_pattern)
-        config_json_path = common.find_config_json(parent_directory, r"^config\.json$")
-
-        year_dirs = common.get_matching_dirs(src_directory, pattern=r"^\d{4}$")
-
-        # create jpgs for all tifs that don't have one
-        self.create_jpgs_for_tifs(
-            year_dirs, avoid_patterns=[".*merged_multispectral.*"]
-        )
-        # @todo get jpgs in each directory and add to a total to use for the progress bar
-
-        logger.info(f"session directory: {session_dir}")
-
-        for year_dir in tqdm.auto.tqdm(
-            year_dirs, desc="Running models on each year", leave=False, unit_scale=True
-        ):
-            # make a model_settings{year}.json
-            model_year_dict = model_dict.copy()
-            model_year_dict["sample_direc"] = year_dir
-            logger.info(f"model_year_dict: {model_year_dict}")
-            year_name = os.path.basename(year_dir)
-            logger.info(f"year_name: {year_name}")
-            session_year_path = common.create_directory(session_dir, year_name)
-            logger.info(f"session_year_path: {session_year_path}")
-
-            model_settings_path = os.path.join(session_year_path, "model_settings.json")
-            common.write_to_json(model_settings_path, model_year_dict)
-            # Compute the segmentation
-            self.compute_segmentation(
-                model_year_dict["sample_direc"],
-                model_list,
-                metadatadict,
-                model_types,
-                use_tta,
-                use_otsu,
+        modelcard_file_names = [
+            model_name.replace("_fullmodel.h5", "_modelcard.json")
+            for model_name in all_model_names
+        ]
+        all_json_reponses = []
+        for available_file in available_files:
+            if available_file["key"] in json_file_names + modelcard_file_names:
+                all_json_reponses.append(available_file)
+        if len(all_models_reponses) == 0:
+            raise Exception(f"Cannot find any .h5 files at {model_id}")
+        if len(all_json_reponses) == 0:
+            raise Exception(
+                f"Cannot find corresponding .json files for .h5 files at {model_id}"
             )
 
-        for year_dir in tqdm.auto.tqdm(
-            year_dirs, desc="Creating tifs", leave=False, unit_scale=True
-        ):
-            # move files from out dir to session directory under folder with year name
-            year_name = os.path.basename(year_dir)
-            outputs_path = os.path.join(src_directory, year_name, "out")
-            session_year_path = common.create_directory(session_dir, year_name)
-            logger.info(f"Moving from {outputs_path} files to {session_year_path}")
-            if not os.path.exists(outputs_path):
-                logger.info(f"No model outputs were generated for year {year_name}")
-                print(f"No model outputs were generated for year {year_name}")
-                continue
-
-            common.move_files(outputs_path, session_year_path, delete_src=True)
-            common.rename_files(
-                session_year_path, "*.png", new_name="", replace_name="_predseg"
-            )
-            # copy the xml files associated with each model output
-            xml_files = glob(os.path.join(year_dir, "*aux.xml"))
-            common.copy_files(
-                xml_files, session_year_path, avoid_patterns=[".*merged.*"]
+        logger.info(f"all_models_reponses : {all_models_reponses }")
+        logger.info(f"all_json_reponses : {all_json_reponses }")
+        for response in all_models_reponses + all_json_reponses:
+            # get the link of the best model
+            link = response["links"]["self"]
+            filename = response["key"]
+            filepath = os.path.join(model_path, filename)
+            download_dict[filepath] = link
+        # download classes.txt file
+        download_dict.update(
+            get_files_to_download(
+                available_files, ["classes.txt"], model_id, model_path
             )
-            # rename all the xml files
-            common.rename_files(
-                session_year_path, "*aux.xml", new_name=".png", replace_name=".jpg"
-            )
-            png_files = glob(os.path.join(session_year_path, "*png"))
-            png_files = common.filter_files(png_files, [".*overlay.*"])
-            common.gdal_translate_png_to_tiff(png_files, translateoptions="-of GTiff")
-            logger.info(f"Done moving files for year : {session_year_path}")
-            # create orthomoasic
-            merged_multispectural = get_merged_multispectural(session_year_path)
-            logger.info(f"merged_multispectural: {merged_multispectural}")
-
-            # copy config files to session directory
-            dst_file = os.path.join(session_year_path, "config_gdf.geojson")
-            logger.info(f"dst_config_gdf: {dst_file}")
-            shutil.copy(config_gdf_path, dst_file)
-            dst_file = os.path.join(session_year_path, "config.json")
-            logger.info(f"dst_config.json: {dst_file}")
-            shutil.copy(config_json_path, dst_file)
-
-    def compute_segmentation(
-        self,
-        sample_direc: str,
-        model_list: list,
-        metadatadict: dict,
-        model_types,
-        use_tta: bool,
-        use_otsu: bool,
-    ):
-
-        logger.info(f"Test Time Augmentation: {use_tta}")
-        logger.info(f"Otsu Threshold: {use_otsu}")
-        # Read in the image filenames as either .npz,.jpg, or .png
-        files_to_segment = self.get_files_for_seg(
-            sample_direc, avoid_patterns=[r".*merged_multispectral.*"]
         )
-        logger.info(f"files_to_segment: {files_to_segment}")
-        if model_types[0] != "segformer":
-            ### mixed precision
-            from tensorflow.keras import mixed_precision
-
-            mixed_precision.set_global_policy("mixed_float16")
-        # Compute the segmentation for each of the files
-        for file_to_seg in tqdm.auto.tqdm(files_to_segment):
-            do_seg(
-                file_to_seg,
-                model_list,
-                metadatadict,
-                model_types[0],
-                sample_direc=sample_direc,
-                NCLASSES=self.NCLASSES,
-                N_DATA_BANDS=self.N_DATA_BANDS,
-                TARGET_SIZE=self.TARGET_SIZE,
-                TESTTIMEAUG=use_tta,
-                WRITE_MODELMETADATA=False,
-                OTSU_THRESHOLD=use_otsu,
-                out_dir_name="out",
-                profile="meta",
+        download_dict = check_if_files_exist(download_dict)
+        # download the files that don't exist
+        logger.info(f"URLs to download: {download_dict}")
+        # if any files are not found locally download them asynchronous
+        if download_dict != {}:
+            downloads.run_async_function(
+                downloads.async_download_url_dict, url_dict=download_dict
             )
 
-    @time_func
     def get_model(self, weights_list: list):
         model_list = []
         config_files = []
         model_types = []
         if weights_list == []:
             raise Exception("No Model Info Passed")
         for weights in weights_list:
@@ -851,134 +604,375 @@
 
             model_types.append(MODEL)
             model_list.append(model)
             config_files.append(configfile)
 
         return model, model_list, config_files, model_types
 
-    @time_func
-    def get_metadatadict(
-        self, weights_list: list, config_files: list, model_types: list
+    def get_files_for_seg(
+        self, sample_direc: str, avoid_patterns: List[str] = []
+    ) -> list:
+        """
+        Returns a list of files to be segmented.
+
+        The function reads in the image filenames as either (`.npz`) OR (`.jpg`, or `.png`)
+        and returns a sorted list of the file paths.
+
+        Args:
+        - sample_direc (str): The directory containing files to be segmented.
+        - avoid_patterns (List[str], optional): A list of file names to be avoided.Don't include any file extensions. Default is [].
+
+        Returns:
+        - list: A list of files to be segmented.
+        """
+        file_extensions = [".npz", ".jpg", ".png"]
+        sample_filenames = get_sorted_files_with_extension(
+            sample_direc, file_extensions
+        )
+        # filter out files whose filenames match any of the avoid_patterns
+        sample_filenames = common.filter_files(sample_filenames, avoid_patterns)
+        logger.info(f"files to seg: {sample_filenames}")
+        return sample_filenames
+
+    def preprocess_data(
+        self, src_directory: str, model_dict: dict, session: sessions.Session
     ):
-        metadatadict = {}
-        metadatadict["model_weights"] = weights_list
-        metadatadict["config_files"] = config_files
-        metadatadict["model_types"] = model_types
-        return metadatadict
+        # load year directories for each ROI
+        roi_dict = common.get_subdirectories_with_ids(src_directory)
+        session.roi_ids = list(roi_dict.keys())
+
+        # create dictionary to run on model on for each year in each ROI
+        preprocessed_data = {}
+        for roi_id, roi_path in roi_dict.items():
+            # for each year create overlapping tiles and save location of tiles
+            model_data_per_year = {}
+            multiband_path = os.path.join(roi_path, "multiband")
+            year_dirs = common.get_matching_dirs(multiband_path, pattern=r"^\d{4}$")
+            for year_dir in tqdm.auto.tqdm(
+                year_dirs, desc="Preparing data", leave=False, unit_scale=True
+            ):
+                if len(os.listdir(year_dir)) == 0:
+                    continue
+                original_merged_tif = os.path.join(year_dir, "merged_multispectral.tif")
+                tiles_path = common.create_directory(year_dir, "tiles")
+                tiles_path = create_overlapping_tiles(original_merged_tif, tiles_path)
+                if tiles_path == "":
+                    continue
+                model_year_dict = model_dict.copy()
+                model_year_dict["sample_direc"] = tiles_path
+                # use year name as the key ex.{ roi_id: '2010':{},'2011':{}}
+                model_data_per_year[os.path.basename(year_dir)] = model_year_dict
+                model_data_per_year["roi_path"] = roi_path
+            # if ROI directory had no years then skip it
+            if len(year_dirs) == 0:
+                continue
+            preprocessed_data[roi_id] = model_data_per_year
 
-    @time_func
-    def get_weights_list(self, model_choice: str = "ENSEMBLE"):
-        """Returns of the weights files(.h5) within weights_direc"""
-        if model_choice == "ENSEMBLE":
-            weights_list = glob(self.weights_direc + os.sep + "*.h5")
-            logger.info(f"ENSEMBLE: weights_list: {weights_list}")
-            logger.info(
-                f"ENSEMBLE: {len(weights_list)} sets of model weights were found "
-            )
-            return weights_list
-        elif model_choice == "BEST":
-            # read model name (fullmodel.h5) from BEST_MODEL.txt
-            with open(self.weights_direc + os.sep + "BEST_MODEL.txt") as f:
-                model_name = f.readlines()
-            weights_list = [self.weights_direc + os.sep + model_name[0]]
-            logger.info(f"BEST: weights_list: {weights_list}")
-            logger.info(f"BEST: {len(weights_list)} sets of model weights were found ")
-            return weights_list
+        logger.info(f"preprocessed_data: {preprocessed_data}")
+        return preprocessed_data
+
+    def compute_segmentation(
+        self,
+        preprocessed_data: dict,
+    ):
+        """
+        Computes the segmentation of the input multispectral images using the preprocessed data.
+
+        Args:
+            preprocessed_data (dict): A dictionary containing the preprocessed data that's in a format that's
+            ready for segmentation.
+
+        Returns:
+            None.
+
+        Raises:
+            None.
+        """
+        # perform segmentations for each year in each ROI
+        for roi_data in preprocessed_data.values():
+            for key in roi_data.keys():
+                if key == "roi_path":
+                    continue
+                logger.info(f"key: {key}")
+                logger.info(f"roi_data[key]: {roi_data[key]}")
+                sample_direc = roi_data[key]["sample_direc"]
+                use_tta = roi_data[key]["tta"]
+                use_otsu = roi_data[key]["otsu"]
+                files_to_segment = self.get_files_for_seg(sample_direc)
+                logger.info(f"files_to_segment: {files_to_segment}")
+                if self.model_types[0] != "segformer":
+                    ### mixed precision
+                    from tensorflow.keras import mixed_precision
+
+                    mixed_precision.set_global_policy("mixed_float16")
+                # run model for each file
+                for file_to_seg in tqdm.auto.tqdm(files_to_segment):
+                    do_seg(
+                        file_to_seg,
+                        self.model_list,
+                        self.metadata_dict,
+                        self.model_types[0],
+                        sample_direc=sample_direc,
+                        NCLASSES=self.NCLASSES,
+                        N_DATA_BANDS=self.N_DATA_BANDS,
+                        TARGET_SIZE=self.TARGET_SIZE,
+                        TESTTIMEAUG=use_tta,
+                        WRITE_MODELMETADATA=False,
+                        OTSU_THRESHOLD=use_otsu,
+                        out_dir_name="out",
+                        profile="meta",
+                    )
+
+    def postprocess_data(self, preprocessed_data: dict, session: sessions.Session):
+        """
+        Preprocesses the outputs of the model by preparing moving the outputs to the session directory and creating a mask for each
+        class in the output. For example if the model outputs 3 classes then this will create 3 masks for each year in each ROI.
+
+        Args:
+            src_directory (str): The path to the directory containing the multispectral images to be segmented.
+            model_dict (dict): A dictionary containing the model configuration.
+            session (sessions.Session): A session object to keep track of segmentation parameters and results.
+
+        Returns:
+            dict: A dictionary containing the preprocessed the outputs of the model.
+
+        Raises:
+            None.
+        """
+        # get roi_ids
+        for roi_id in preprocessed_data.keys():
+            # create session roi directories
+            roi_session_directory = common.create_directory(session.path, roi_id)
+            # copy config files to session directory
+            roi_directory = preprocessed_data[roi_id]["roi_path"]
+            self.copy_configs(roi_directory, roi_session_directory)
+
+            for key in preprocessed_data[roi_id].keys():
+                if key == "roi_path":
+                    continue
+                year = key
+                session.add_years(year)
+                # create session year sub directories
+                year_session_directory = common.create_directory(
+                    roi_session_directory, year
+                )
+                tiles_path = preprocessed_data[roi_id][year]["sample_direc"]
+                # move 'tiles' to session directories
+                session_tiles_path = common.create_directory(
+                    year_session_directory, "tiles"
+                )
+                common.move_files_resurcively(src=tiles_path, dest=session_tiles_path)
+                # remove empty tiles directory
+                if os.path.basename(tiles_path).lower() == "tiles":
+                    os.rmdir(tiles_path)
+                # save model settings
+                model_settings_path = os.path.join(
+                    year_session_directory, "model_settings.json"
+                )
+                common.write_to_json(
+                    model_settings_path, preprocessed_data[roi_id][year]
+                )
+                # merge tiles to create greyscale tif
+                # outputs of model are in session_name/ROI_ID/year/tiles/out
+                greyscale_tif = make_greyscale_tif(
+                    session_tiles_path, year_session_directory
+                )
+                if not greyscale_tif:
+                    logger.info(f"Year {year} could not generate a  greyscale tif")
+                    continue
+                # create class mask pngs for each merged tif
+                # get class names to create class mapping
+                class_mapping = map_functions.get_class_mapping(session.classes)
+                # see if any class masks already exist in directory and if they don't exist then create them
+                class_masks_filenames = map_functions.get_existing_class_files(
+                    year_session_directory, session.classes
+                )
+
+                # in year_session_directory make a separate png containing all the pixels in each class within the tif
+                if not class_masks_filenames:
+                    class_masks_filenames = map_functions.generate_class_masks(
+                        greyscale_tif, class_mapping, year_session_directory
+                    )
+
+        # save session copy_configssettings
+        preprocessed_data_path = os.path.join(session.path, "preprocessed_data.json")
+        common.write_to_json(preprocessed_data_path, preprocessed_data)
+        session.save(session.path)
+
+    def copy_configs(self, src: str, dst: str) -> None:
+        """
+        Copies 'config.geojson' and 'config.json' files from the source to the destination directories.
+
+        Args:
+            src (str): The path to the directory containing the source files.
+            dst (str): The path to the directory where the files will be copied.
+
+        Returns:
+            None.
+
+        Raises:
+            None.
+        """
+        # copy config.geojson and config.json files from souce to destination directories
+        config_gdf_path = common.find_config_json(src, r"config_gdf.*\.geojson")
+        config_json_path = common.find_config_json(src, r"^config\.json$")
+        dst_file = os.path.join(dst, "config_gdf.geojson")
+        logger.info(f"dst_config_gdf: {dst_file}")
+        shutil.copy(config_gdf_path, dst_file)
+        dst_file = os.path.join(dst, "config.json")
+        logger.info(f"dst_config.json: {dst_file}")
+        shutil.copy(config_json_path, dst_file)
+
+    def get_classes(self, model_directory_path: str) -> list:
+        """
+        Reads the 'classes.txt' file from the given model directory path and returns a list of classes.
+
+        Args:
+            model_directory_path (str): The path to the directory containing the model files.
+
+        Returns:
+            list: A list of classes.
+
+        Raises:
+            None.
+        """
+        class_path = os.path.join(model_directory_path, "classes.txt")
+        classes = common.read_text_file(class_path)
+        return classes
 
     def get_downloaded_models_dir(self) -> str:
-        """returns full path to downloaded_models directory and
-        if downloaded_models directory does not exist then it is created
+        """
+        Returns the full path to the downloaded models directory, creating it if necessary.
 
         Returns:
             str: full path to downloaded_models directory
         """
+
         # directory to hold downloaded models from Zenodo
         script_dir = os.path.dirname(os.path.abspath(__file__))
-        downloaded_models_path = os.path.abspath(
-            os.path.join(script_dir, "downloaded_models")
-        )
-        if not os.path.exists(downloaded_models_path):
-            os.mkdir(downloaded_models_path)
-        logger.info(f"downloaded_models_path: {downloaded_models_path}")
+        downloaded_models_path = os.path.join(script_dir, "downloaded_models")
+        os.makedirs(downloaded_models_path, exist_ok=True)
         return downloaded_models_path
 
-    def download_model(self, model_choice: str, dataset_id: str) -> None:
-        """downloads model specified by zenodo id in dataset_id.
+    def get_weights_list(self, model_path: str, model_choice: str = "BEST"):
+        """
+        Returns a list of the weights files (.h5) within the weights directory, based on the model choice specified.
 
-        Downloads best model is model_choice = 'BEST' or all models in
-        zenodo release if model_choice = 'ENSEMBLE'
+        Args:
+            model_path (str): The path to the directory containing the model
+            model_choice (str): The type of model weights to return. Possible choices are "BEST" (default) or "ENSEMBLE".
+
+        Returns:
+            A list of weights files (.h5) within the weights directory, based on the model choice specified.
+        """
+        if model_choice == "ENSEMBLE":
+            weights_list = glob(model_path + os.sep + "*.h5")
+        elif model_choice == "BEST":
+            # read model name (fullmodel.h5) from BEST_MODEL.txt
+            with open(model_path + os.sep + "BEST_MODEL.txt") as f:
+                model_name = f.readlines()
+            weights_list = [model_path + os.sep + model_name[0]]
+        logger.info(f"{model_choice}: {len(weights_list)} weights_list: {weights_list}")
+        return weights_list
+
+    def prepare_model(self, model_implementation: str, model_id: str):
+        """
+        Prepares the model for use by downloading the required files and loading the model.
 
         Args:
-            model_choice (str): 'BEST' or 'ENSEMBLE'
-            dataset_id (str): name of model followed by underscore zenodo_id'name_of_model_zenodoid'
+            model_implementation (str): The model implementation name.
+            model_id (str): The ID of the model.
         """
-        zenodo_id = dataset_id.split("_")[-1]
-        root_url = "https://zenodo.org/api/records/" + zenodo_id
-        # read raw json and get list of available files in zenodo release
-        response = requests.get(root_url)
-        json_content = json.loads(response.text)
-        # logger.info(f"json_content {json_content}")
-        files = json_content["files"]
+        # create the model directory
+        self.weights_directory = self.get_model_directory(model_id)
+        logger.info(f"self.weights_directory:{self.weights_directory}")
+
+        self.download_model(model_implementation, model_id, self.weights_directory)
+        weights_list = self.get_weights_list(
+            self.weights_directory, model_implementation
+        )
 
-        downloaded_models_path = self.get_downloaded_models_dir()
-        # directory to hold specific model referenced by dataset_id
-        self.weights_direc = os.path.abspath(
-            os.path.join(downloaded_models_path, dataset_id)
+        # Load the model from the config files
+        model, model_list, config_files, model_types = self.get_model(weights_list)
+
+        self.model_types = model_types
+        self.model_list = model_list
+        self.metadata_dict = self.get_metadatadict(
+            weights_list, config_files, model_types
         )
-        if not os.path.exists(self.weights_direc):
-            os.mkdir(self.weights_direc)
+        logger.info(f"self.metadatadict: {self.metadata_dict}")
 
-        logger.info(f"self.weights_direc:{self.weights_direc}")
-        print(f"\n Model located at: {self.weights_direc}")
-        models_json_dict = {}
-        if model_choice.upper() == "BEST":
-            # retrieve best model text file
-            best_model_json = [f for f in files if f["key"] == "BEST_MODEL.txt"][0]
-            if len(best_model_json) == 0:
-                raise Exception(f"Cannot find BEST_MODEL.txt at {root_url}")
-            logger.info(f"list of best_model_txt: {best_model_json}")
-            best_model_txt_path = self.weights_direc + os.sep + "BEST_MODEL.txt"
-            logger.info(f"BEST: best_model_txt_path : {best_model_txt_path }")
-
-            # if best BEST_MODEL.txt file not exist then download it
-            if not os.path.isfile(best_model_txt_path):
-                download_url(
-                    best_model_json["links"]["self"],
-                    best_model_txt_path,
-                )
-            # read contents of BEST_MODEL.txt
-            with open(best_model_txt_path) as f:
-                filename = f.read()
-
-            # check if json and h5 file in BEST_MODEL.txt exist
-            model_json = [f for f in files if f["key"] == filename][0]
-            # path to save model
-            outfile = self.weights_direc + os.sep + filename
-            logger.info(f"BEST: outfile: {outfile}")
-            # path to save file and json data associated with file saved to dict
-            models_json_dict[outfile] = model_json["links"]["self"]
-            url_dict = get_url_dict_to_download(models_json_dict)
-            # if any files are not found locally download them asynchronous
-            if url_dict != {}:
-                run_async_download(url_dict)
-        elif model_choice.upper() == "ENSEMBLE":
-            # get list of all models
-            all_models = [f for f in files if f["key"].endswith(".h5")]
-            if len(all_models) == 0:
-                raise Exception(f"Cannot find any .h5 files at {root_url}")
-            logger.info(f"all_models : {all_models }")
-            # check if all h5 files in files are in self.weights_direc
-            for model_json in all_models:
-                outfile = (
-                    self.weights_direc
-                    + os.sep
-                    + model_json["links"]["self"].split("/")[-1]
-                )
-                logger.info(f"ENSEMBLE: outfile: {outfile}")
-                # path to save file and json data associated with file saved to dict
-                models_json_dict[outfile] = model_json["links"]["self"]
-            logger.info(f"models_json_dict: {models_json_dict}")
-            url_dict = get_url_dict_to_download(models_json_dict)
-            logger.info(f"URLs to download: {url_dict}")
-            # if any files are not found locally download them asynchronous
-            if url_dict != {}:
-                run_async_download(url_dict)
+    def get_metadatadict(
+        self, weights_list: list, config_files: list, model_types: list
+    ) -> dict:
+        """Returns a dictionary containing metadata about the models.
+
+        Args:
+            weights_list (list): A list of model weights.
+            config_files (list): A list of model configuration files.
+            model_types (list): A list of model types.
+
+        Returns:
+            dict: A dictionary containing metadata about the models. The keys
+            are 'model_weights', 'config_files', and 'model_types', and the
+            values are the corresponding input lists.
+
+        Example:
+            weights = ['weights1.h5', 'weights2.h5']
+            configs = ['config1.json', 'config2.json']
+            types = ['unet', 'resunet']
+            metadata = get_metadatadict(weights, configs, types)
+            print(metadata)
+            # Output: {'model_weights': ['weights1.h5', 'weights2.h5'],
+            #          'config_files': ['config1.json', 'config2.json'],
+            #          'model_types': ['unet', 'resunet']}
+        """
+        metadatadict = {}
+        metadatadict["model_weights"] = weights_list
+        metadatadict["config_files"] = config_files
+        metadatadict["model_types"] = model_types
+        return metadatadict
+
+    def get_model_dict(self):
+        return self.model_dict
+
+    def run_model(
+        self,
+        model_implementation: str,
+        session_name: str,
+        src_directory: str,
+        model_id: str,
+        use_GPU: str,
+        use_otsu: bool,
+        use_tta: bool,
+    ):
+
+        logger.info(f"ROI directory: {src_directory}")
+        logger.info(f"session name: {session_name}")
+
+        self.prepare_model(model_implementation, model_id)
+        classes = self.get_classes(self.weights_directory)
+        model_dict = {
+            "sample_direc": None,
+            "use_GPU": use_GPU,
+            "implementation": model_implementation,
+            "model_type": model_id,
+            "otsu": use_otsu,
+            "tta": use_tta,
+            "classes": classes,
+        }
+        logger.info(f"model_dict: {model_dict}")
+        # create a session
+        session = sessions.Session()
+        sessions_path = common.create_directory(os.getcwd(), "sessions")
+        session_path = common.create_directory(sessions_path, session_name)
+
+        session.classes = classes
+        session.path = session_path
+        session.name = session_name
+
+        preprocessed_data = self.preprocess_data(src_directory, model_dict, session)
+
+        self.compute_segmentation(preprocessed_data)
+        self.postprocess_data(preprocessed_data, session)
+        # save session data after postprocessing data
+        session.save(session_path)
```

### Comparing `seg2map-0.0.6/src/seg2map.egg-info/PKG-INFO` & `seg2map-0.0.7/src/seg2map.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg2map
-Version: 0.0.6
+Version: 0.0.7
 Summary: An interactive jupyter notebook for downloading satellite imagery
 Author-email:  Sharon Fitzpatrick <sharon.fitzpatrick23@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Doodleverse
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

