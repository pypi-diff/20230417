# Comparing `tmp/cleopatra-0.3.0.tar.gz` & `tmp/cleopatra-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleopatra-0.3.0.tar", last modified: Tue Apr 11 15:48:53 2023, max compression
+gzip compressed data, was "cleopatra-0.3.1.tar", last modified: Mon Apr 17 03:45:09 2023, max compression
```

## Comparing `cleopatra-0.3.0.tar` & `cleopatra-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.285976 cleopatra-0.3.0/
--rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.0/AUTHORS.rst
--rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.0/LICENSE.md
--rw-rw-rw-   0        0        0     6829 2023-04-11 15:48:53.285976 cleopatra-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5081 2023-04-11 15:41:59.000000 cleopatra-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.133428 cleopatra-0.3.0/cleopatra/
--rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/__init__.py
--rw-rw-rw-   0        0        0    34725 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/array.py
--rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/statistics.py
--rw-rw-rw-   0        0        0     6499 2023-04-11 15:41:59.000000 cleopatra-0.3.0/cleopatra/styles.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.175884 cleopatra-0.3.0/cleopatra.egg-info/
--rw-rw-rw-   0        0        0     6829 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-04-11 15:48:53.000000 cleopatra-0.3.0/cleopatra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      107 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 15:48:52.000000 cleopatra-0.3.0/cleopatra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 15:48:53.285976 cleopatra-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1689 2023-04-11 15:41:59.000000 cleopatra-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 15:48:53.251482 cleopatra-0.3.0/tests/
--rw-rw-rw-   0        0        0     7940 2023-04-11 15:41:59.000000 cleopatra-0.3.0/tests/test_plot_array.py
--rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.0/tests/test_statistics.py
--rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.0/tests/test_styles.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.612063 cleopatra-0.3.1/
+-rw-rw-rw-   0        0        0      173 2022-03-20 16:23:15.000000 cleopatra-0.3.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0    35591 2022-03-20 16:22:07.000000 cleopatra-0.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0     6887 2023-04-17 03:45:09.611064 cleopatra-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5081 2023-04-17 03:25:28.000000 cleopatra-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.592188 cleopatra-0.3.1/cleopatra/
+-rw-rw-rw-   0        0        0     1038 2023-04-11 15:41:59.000000 cleopatra-0.3.1/cleopatra/__init__.py
+-rw-rw-rw-   0        0        0    37346 2023-04-17 03:25:28.000000 cleopatra-0.3.1/cleopatra/array.py
+-rw-rw-rw-   0        0        0     2892 2023-04-11 15:41:59.000000 cleopatra-0.3.1/cleopatra/statistics.py
+-rw-rw-rw-   0        0        0     6398 2023-04-17 03:25:28.000000 cleopatra-0.3.1/cleopatra/styles.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.601556 cleopatra-0.3.1/cleopatra.egg-info/
+-rw-rw-rw-   0        0        0     6887 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 15:48:52.000000 cleopatra-0.3.1/cleopatra.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      107 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 03:45:09.000000 cleopatra-0.3.1/cleopatra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 03:45:09.612063 cleopatra-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1689 2023-04-17 03:25:28.000000 cleopatra-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 03:45:09.608555 cleopatra-0.3.1/tests/
+-rw-rw-rw-   0        0        0     8159 2023-04-17 03:25:28.000000 cleopatra-0.3.1/tests/test_plot_array.py
+-rw-rw-rw-   0        0        0      414 2023-04-11 15:41:59.000000 cleopatra-0.3.1/tests/test_statistics.py
+-rw-rw-rw-   0        0        0      218 2023-04-11 15:41:59.000000 cleopatra-0.3.1/tests/test_styles.py
```

### Comparing `cleopatra-0.3.0/LICENSE.md` & `cleopatra-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.0/PKG-INFO` & `cleopatra-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.0
+Version: 0.3.1
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
 Keywords: matplotlib,arrays,visualization
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.0
+pip install cleopatra==0.3.1
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -110,16 +110,19 @@
 * bump up versions
 * add serapeum_utils as a dependency
 
 0.2.7 (2023-01-31)
 ------------------
 * bump up numpy to version 1.24.1
 
-
 0.3.0 (2023-04-11)
 ------------------
 * change API to work completly with numpy array inputs
 * chenge to conda config
 * add hpc-utils to filter and access arrays
 * restructure the whole modules to array, statistics, and styles modules.
 * all modules has classes.
 * save animation function using ffmpeg.
+
+0.3.1 (2023-04-17)
+------------------
+* plot RGB plots
```

### Comparing `cleopatra-0.3.0/README.md` & `cleopatra-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.0
+pip install cleopatra==0.3.1
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
```

### Comparing `cleopatra-0.3.0/cleopatra/__init__.py` & `cleopatra-0.3.1/cleopatra/__init__.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.0/cleopatra/array.py` & `cleopatra-0.3.1/cleopatra/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,42 +26,74 @@
 DEFAULT_OPTIONS = style_defaults | DEFAULT_OPTIONS
 SUPPORTED_VIDEO_FORMAT = ["gif", "mov", "avi", "mp4"]
 
 
 class Array:
     """Map."""
 
-    def __init__(self, array: np.ndarray, exclude_value: List = np.nan):
+    def __init__(
+        self,
+        array: np.ndarray,
+        exclude_value: List = np.nan,
+        rgb: List[int] = None,
+        surface_reflectance: int = 10000,
+        cutoff: List = None,
+    ):
         """Plot array.
 
         Parameters
         ----------
         array: [numpy array]
             array.
         exclude_value : [numeric]
             value used to fill cells out of the domain. Optional, Default is np.nan
             needed only in case of plotting array
+        rgb: [List]
+            Default is [3,2,1]
+        surface_reflectance: [int]
+            Default is  10000
+        cutoff: [List]
+            clip the range of pixel values for each band. (take only the pixel values from 0 to value of the cutoff and
+            scale them back to between 0 and 1. Default is None.
 
         the object does not need any parameters to be initialized.
         """
         # first replace the no_data_value by nan
         # convert the array to float32 to be able to replace the no data value with nan
-        array = array.astype(np.float32)
-
-        if exclude_value is not None:
+        print(f"display_cell_value: {DEFAULT_OPTIONS['display_cell_value']}")
+        if exclude_value is not np.nan:
+            array = array.astype(np.float32)
             if len(exclude_value) > 1:
                 mask = np.logical_or(
                     np.isclose(array, exclude_value[0], rtol=0.001),
                     np.isclose(array, exclude_value[1], rtol=0.001),
                 )
             else:
                 mask = np.isclose(array, exclude_value[0], rtol=0.0000001)
 
             array[mask] = np.nan
 
+        if rgb is not None:
+            self.rgb = True
+            # prepare to plot rgb plot only if there are three arrays
+            if array.shape[0] < 3:
+                raise ValueError(
+                    f"To plot RGB plot the given array should have only 3 arrays, given array have "
+                    f"{len(array.shape[0])}"
+                )
+            else:
+                array = self._prepare_rgb(
+                    array,
+                    rgb=rgb,
+                    surface_reflectance=surface_reflectance,
+                    cutoff=cutoff,
+                )
+        else:
+            self.rgb = False
+
         self._exclude_value = exclude_value
         self._vmin = np.nanmin(array)
         self._vmax = np.nanmax(array)
         self.arr = array
         # get the tick spacing that have 10 ticks only
         self.ticks_spacing = (self._vmax - self._vmin) / 10
         shape = array.shape
@@ -71,14 +103,50 @@
             )
         else:
             no_elem = np.size(array[:, :]) - np.count_nonzero((array[np.isnan(array)]))
 
         self.no_elem = no_elem
         self._default_options = DEFAULT_OPTIONS
 
+    def _prepare_rgb(
+        self,
+        array: np.ndarray,
+        rgb: List[int] = None,
+        surface_reflectance: int = 10000,
+        cutoff: List = None,
+    ) -> np.ndarray:
+        """Prepare for RGB plot.
+
+        Parameters
+        ----------
+        array: [numpy array]
+            array.
+        rgb: [List]
+            Default is [3,2,1]
+        surface_reflectance: [int]
+            Default is  10000
+        cutoff: [List]
+            clip the range of pixel values for each band. (take only the pixel values from 0 to value of the cutoff and
+            scale them back to between 0 and 1. Default is None.
+
+        Returns
+        -------
+
+        """
+        # take the rgb arrays and reorder them to have the red-green-blue, if the order is not given assume the
+        # order as sentinel data. [3, 2, 1]
+        array = array[rgb].transpose(1, 2, 0)
+        array = np.clip(array / surface_reflectance, 0, 1)
+        if cutoff is not None:
+            array[0] = np.clip(rgb[0], 0, cutoff[0]) / cutoff[0]
+            array[1] = np.clip(rgb[1], 0, cutoff[1]) / cutoff[1]
+            array[2] = np.clip(rgb[2], 0, cutoff[2]) / cutoff[2]
+
+        return array
+
     @property
     def vmin(self):
         """min value in the array"""
         return self._vmin
 
     @property
     def vmax(self):
@@ -331,53 +399,58 @@
             if key not in self.default_options.keys():
                 raise ValueError(
                     f"The given keyword argument:{key} is not correct, possible parameters are,"
                     f" {DEFAULT_OPTIONS}"
                 )
             else:
                 self.default_options[key] = val
-        # if user did not input ticks spacing use the calculated one.
-        if "ticks_spacing" in kwargs.keys():
-            self.default_options["ticks_spacing"] = kwargs["ticks_spacing"]
-        else:
-            self.default_options["ticks_spacing"] = self.ticks_spacing
-
-        if "vmin" in kwargs.keys():
-            self.default_options["vmin"] = kwargs["vmin"]
-        else:
-            self.default_options["vmin"] = self.vmin
-
-        if "vmax" in kwargs.keys():
-            self.default_options["vmax"] = kwargs["vmax"]
-        else:
-            self.default_options["vmax"] = self.vmax
 
         arr = self.arr
         fig = plt.figure(figsize=self.default_options["figsize"])
         # gs = gridspec.GridSpec(nrows=2, ncols=2, figure=fig)
         ax = fig.add_subplot()  # gs[:,:]
-        # creating the ticks/bounds
-        ticks = self.get_ticks()
-        im, cbar_kw = self.get_im_cbar(ax, arr, ticks)
-
-        # Create colorbar
-        cbar = ax.figure.colorbar(
-            im,
-            ax=ax,
-            shrink=self.default_options["cbar_length"],
-            orientation=self.default_options["orientation"],
-            **cbar_kw,
-        )
-        cbar.ax.set_ylabel(
-            self.default_options["cbar_label"],
-            rotation=self.default_options["rotation"],
-            va="bottom",
-            fontsize=self.default_options["cbar_label_size"],
-        )
-        cbar.ax.tick_params(labelsize=10)
+
+        if self.rgb:
+            ax.imshow(arr)
+        else:
+            # if user did not input ticks spacing use the calculated one.
+            if "ticks_spacing" in kwargs.keys():
+                self.default_options["ticks_spacing"] = kwargs["ticks_spacing"]
+            else:
+                self.default_options["ticks_spacing"] = self.ticks_spacing
+
+            if "vmin" in kwargs.keys():
+                self.default_options["vmin"] = kwargs["vmin"]
+            else:
+                self.default_options["vmin"] = self.vmin
+
+            if "vmax" in kwargs.keys():
+                self.default_options["vmax"] = kwargs["vmax"]
+            else:
+                self.default_options["vmax"] = self.vmax
+
+            # creating the ticks/bounds
+            ticks = self.get_ticks()
+            im, cbar_kw = self.get_im_cbar(ax, arr, ticks)
+
+            # Create colorbar
+            cbar = ax.figure.colorbar(
+                im,
+                ax=ax,
+                shrink=self.default_options["cbar_length"],
+                orientation=self.default_options["orientation"],
+                **cbar_kw,
+            )
+            cbar.ax.set_ylabel(
+                self.default_options["cbar_label"],
+                rotation=self.default_options["rotation"],
+                va="bottom",
+                fontsize=self.default_options["cbar_label_size"],
+            )
+            cbar.ax.tick_params(labelsize=10)
 
         ax.set_title(
             self.default_options["title"], fontsize=self.default_options["title_size"]
         )
         ax.set_xticklabels([])
         ax.set_yticklabels([])
```

### Comparing `cleopatra-0.3.0/cleopatra/statistics.py` & `cleopatra-0.3.1/cleopatra/statistics.py`

 * *Files identical despite different names*

### Comparing `cleopatra-0.3.0/cleopatra/styles.py` & `cleopatra-0.3.1/cleopatra/styles.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,14 @@
     line_scale=0.001,
     line_threshold=0.0001,
     bounds=None,
     midpoint=0,
     grid_alpha=0.75,
 )
 
-# figure_default_options = dict(
-#         name="hist.tif",
-#         Axisfontsize=15,
-#     )
-
 
 class Styles:
     """Styles"""
 
     line_styles = OrderedDict(
         [
             ("solid", (0, ())),  # 0
```

### Comparing `cleopatra-0.3.0/cleopatra.egg-info/PKG-INFO` & `cleopatra-0.3.1/cleopatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleopatra
-Version: 0.3.0
+Version: 0.3.1
 Summary: visualization package
 Home-page: https://github.com/MAfarrag/cleopatra
 Author: Mostafa Farrag
 Author-email: moah.farag@gmail.come
 License: GNU General Public License v3
 Keywords: matplotlib,arrays,visualization
 Classifier: Development Status :: 5 - Production/Stable
@@ -68,15 +68,15 @@
 ```
 pip install git+https://github.com/MAfarrag/cleopatra
 ```
 
 ## pip
 to install the last release you can easly use pip
 ```
-pip install cleopatra==0.3.0
+pip install cleopatra==0.3.1
 ```
 
 Quick start
 ===========
 
 ```
   >>> import cleopatra
@@ -110,16 +110,19 @@
 * bump up versions
 * add serapeum_utils as a dependency
 
 0.2.7 (2023-01-31)
 ------------------
 * bump up numpy to version 1.24.1
 
-
 0.3.0 (2023-04-11)
 ------------------
 * change API to work completly with numpy array inputs
 * chenge to conda config
 * add hpc-utils to filter and access arrays
 * restructure the whole modules to array, statistics, and styles modules.
 * all modules has classes.
 * save animation function using ffmpeg.
+
+0.3.1 (2023-04-17)
+------------------
+* plot RGB plots
```

### Comparing `cleopatra-0.3.0/setup.py` & `cleopatra-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     history = history_file.read()
 
 requirements = [line.strip() for line in open("requirements.txt").readlines()]
 requirements_dev = [line.strip() for line in open("requirements-dev.txt").readlines()]
 
 setup(
     name="cleopatra",
-    version="0.3.0",
+    version="0.3.1",
     description="visualization package",
     author="Mostafa Farrag",
     author_email="moah.farag@gmail.come",
     url="https://github.com/MAfarrag/cleopatra",
     keywords=["matplotlib", "arrays", "visualization"],
     long_description=readme + "\n\n" + history,
     repository="https://github.com/MAfarrag/celopatra",
```

### Comparing `cleopatra-0.3.0/tests/test_plot_array.py` & `cleopatra-0.3.1/tests/test_plot_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 from typing import List
-from pathlib import Path
 import numpy as np
 
 from matplotlib.figure import Figure
 from matplotlib.animation import FuncAnimation
 from cleopatra.array import Array
 
 
@@ -14,14 +13,21 @@
         assert isinstance(array.arr, np.ndarray)
         assert np.isnan(array.arr[0, 0])
         assert array.no_elem == 89
         assert array.vmin == 0
         assert array.vmax == 88
 
 
+class TestRGB:
+    def test_plot_rgb(self, sentinel_2: np.ndarray):
+        array = Array(sentinel_2, rgb=[3, 2, 1], cutoff=[0.3, 0.3, 0.3])
+        fig, ax = array.plot(title="Flow Accumulation")
+        assert isinstance(fig, Figure)
+
+
 class TestPlotArray:
     def test_plot_numpy_array(
         self,
         arr: np.ndarray,
         no_data_value: float,
     ):
         array = Array(arr, exclude_value=[no_data_value])
```

