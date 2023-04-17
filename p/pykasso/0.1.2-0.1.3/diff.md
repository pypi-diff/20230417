# Comparing `tmp/pykasso-0.1.2.tar.gz` & `tmp/pykasso-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykasso-0.1.2.tar", max compression
+gzip compressed data, was "pykasso-0.1.3.tar", max compression
```

## Comparing `pykasso-0.1.2.tar` & `pykasso-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35793 2023-02-20 15:27:40.635814 pykasso-0.1.2/LICENSE
--rw-r--r--   0        0        0     1020 2023-03-24 22:46:57.874808 pykasso-0.1.2/pykasso/__init__.py
--rw-r--r--   0        0        0     2039 2023-02-20 15:27:40.651440 pykasso-0.1.2/pykasso/_misc/SKS_SETTINGS.yaml
--rw-r--r--   0        0        0    15130 2023-02-20 15:27:40.667067 pykasso-0.1.2/pykasso/_misc/statistics.xlsx
--rw-r--r--   0        0        0    10608 2023-02-20 15:27:40.667067 pykasso-0.1.2/pykasso/_misc/statistics_old.xlsx
--rw-r--r--   0        0        0      232 2023-03-25 18:11:31.823406 pykasso-0.1.2/pykasso/_typing/__init__.py
--rw-r--r--   0        0        0     1141 2023-03-24 20:12:28.332365 pykasso-0.1.2/pykasso/_typing/types.py
--rw-r--r--   0        0        0     3656 2023-03-28 16:31:09.797078 pykasso-0.1.2/pykasso/_utils.py
--rw-r--r--   0        0        0      109 2023-03-27 20:49:59.081528 pykasso-0.1.2/pykasso/_version.py
--rw-r--r--   0        0        0      249 2023-03-24 19:52:05.803537 pykasso-0.1.2/pykasso/analysis/__init__.py
--rw-r--r--   0        0        0     6504 2023-03-24 22:56:59.711493 pykasso-0.1.2/pykasso/analysis/analysis.py
--rw-r--r--   0        0        0      246 2023-03-23 17:29:20.117543 pykasso-0.1.2/pykasso/core/__init__.py
--rw-r--r--   0        0        0    23781 2023-03-29 16:37:06.463560 pykasso-0.1.2/pykasso/core/_validations.py
--rw-r--r--   0        0        0     3937 2023-03-25 07:56:09.037750 pykasso-0.1.2/pykasso/core/_wrappers.py
--rw-r--r--   0        0        0    14065 2023-03-27 21:00:45.718253 pykasso-0.1.2/pykasso/core/domain.py
--rw-r--r--   0        0        0    22909 2023-03-28 13:55:58.140035 pykasso-0.1.2/pykasso/core/fracturation.py
--rw-r--r--   0        0        0    10888 2023-03-28 13:54:46.728257 pykasso-0.1.2/pykasso/core/geologic_features.py
--rw-r--r--   0        0        0    15671 2023-03-27 20:59:35.104263 pykasso-0.1.2/pykasso/core/grid.py
--rw-r--r--   0        0        0     6378 2023-03-28 16:30:45.941846 pykasso-0.1.2/pykasso/core/points.py
--rw-r--r--   0        0        0    65081 2023-03-29 20:08:38.390524 pykasso-0.1.2/pykasso/core/sks.py
--rw-r--r--   0        0        0      238 2023-03-28 15:07:32.594123 pykasso-0.1.2/pykasso/visualization/__init__.py
--rw-r--r--   0        0        0    13814 2023-03-28 14:00:54.371156 pykasso-0.1.2/pykasso/visualization/_pyplot.py
--rw-r--r--   0        0        0    17299 2023-03-29 17:47:00.638834 pykasso-0.1.2/pykasso/visualization/_pyvista.py
--rw-r--r--   0        0        0     4790 2023-03-28 18:19:57.066335 pykasso-0.1.2/pykasso/visualization/main.py
--rw-r--r--   0        0        0     1673 2023-03-29 21:19:41.400388 pykasso-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-03-29 20:38:15.607303 pykasso-0.1.2/README.md
--rw-r--r--   0        0        0     4255 1970-01-01 00:00:00.000000 pykasso-0.1.2/setup.py
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 pykasso-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35793 2023-02-20 15:27:40.635814 pykasso-0.1.3/LICENSE
+-rw-r--r--   0        0        0      989 2023-03-31 17:39:08.876694 pykasso-0.1.3/pykasso/__init__.py
+-rw-r--r--   0        0        0     2039 2023-02-20 15:27:40.651440 pykasso-0.1.3/pykasso/_misc/SKS_SETTINGS.yaml
+-rw-r--r--   0        0        0    15130 2023-02-20 15:27:40.667067 pykasso-0.1.3/pykasso/_misc/statistics.xlsx
+-rw-r--r--   0        0        0    10608 2023-02-20 15:27:40.667067 pykasso-0.1.3/pykasso/_misc/statistics_old.xlsx
+-rw-r--r--   0        0        0      214 2023-04-12 17:41:14.221473 pykasso-0.1.3/pykasso/_typing/__init__.py
+-rw-r--r--   0        0        0     1055 2023-04-12 17:41:10.299800 pykasso-0.1.3/pykasso/_typing/types.py
+-rw-r--r--   0        0        0     7996 2023-04-17 14:06:11.209612 pykasso-0.1.3/pykasso/_utils.py
+-rw-r--r--   0        0        0       82 2023-03-31 17:39:32.498170 pykasso-0.1.3/pykasso/_version.py
+-rw-r--r--   0        0        0      249 2023-03-24 19:52:05.803537 pykasso-0.1.3/pykasso/analysis/__init__.py
+-rw-r--r--   0        0        0     6690 2023-04-14 15:05:32.147938 pykasso-0.1.3/pykasso/analysis/analysis.py
+-rw-r--r--   0        0        0      250 2023-04-14 10:04:32.726692 pykasso-0.1.3/pykasso/core/__init__.py
+-rw-r--r--   0        0        0    23433 2023-04-12 18:20:53.220738 pykasso-0.1.3/pykasso/core/_validations.py
+-rw-r--r--   0        0        0     3937 2023-03-25 07:56:09.037750 pykasso-0.1.3/pykasso/core/_wrappers.py
+-rw-r--r--   0        0        0    15427 2023-04-15 15:15:03.846955 pykasso-0.1.3/pykasso/core/domain.py
+-rw-r--r--   0        0        0    25857 2023-04-16 11:33:16.793830 pykasso-0.1.3/pykasso/core/fracturation.py
+-rw-r--r--   0        0        0     4490 2023-04-16 10:21:32.494267 pykasso-0.1.3/pykasso/core/geologic_features.py
+-rw-r--r--   0        0        0    16623 2023-04-14 10:09:50.376344 pykasso-0.1.3/pykasso/core/grid.py
+-rw-r--r--   0        0        0     6437 2023-04-12 16:47:21.503088 pykasso-0.1.3/pykasso/core/points.py
+-rw-r--r--   0        0        0    68283 2023-04-17 16:21:20.258711 pykasso-0.1.3/pykasso/core/sks.py
+-rw-r--r--   0        0        0      238 2023-04-14 13:35:00.683062 pykasso-0.1.3/pykasso/visualization/__init__.py
+-rw-r--r--   0        0        0    20646 2023-04-15 11:24:18.000947 pykasso-0.1.3/pykasso/visualization/_pyplot.py
+-rw-r--r--   0        0        0    17122 2023-04-15 11:25:36.004391 pykasso-0.1.3/pykasso/visualization/_pyvista.py
+-rw-r--r--   0        0        0     4683 2023-04-14 13:36:15.204554 pykasso-0.1.3/pykasso/visualization/main.py
+-rw-r--r--   0        0        0     1693 2023-04-17 21:26:32.610889 pykasso-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3041 2023-04-17 16:58:27.357640 pykasso-0.1.3/README.md
+-rw-r--r--   0        0        0     4311 1970-01-01 00:00:00.000000 pykasso-0.1.3/setup.py
+-rw-r--r--   0        0        0     4715 1970-01-01 00:00:00.000000 pykasso-0.1.3/PKG-INFO
```

### Comparing `pykasso-0.1.2/LICENSE` & `pykasso-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykasso-0.1.2/pykasso/__init__.py` & `pykasso-0.1.3/pykasso/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,23 +24,21 @@
 analysis
    Karst network analysis tool
 visualization
    Karst network visualization tool
    
 Utilities
 ---------
-test
-    Run pyKasso unittests
 __version__
     pyKasso version string
 """
 
 __all__ = []
 
 # Imports pyKasso's core
 from . import core
 from .core import *
 __all__.extend(core.__all__)
 
 # Imports pyKasso version string
 from ._version import __version__
-__all__.extend(['__version__'])
+__all__.extend(['__version__'])
```

### Comparing `pykasso-0.1.2/pykasso/_misc/SKS_SETTINGS.yaml` & `pykasso-0.1.3/pykasso/_misc/SKS_SETTINGS.yaml`

 * *Files identical despite different names*

### Comparing `pykasso-0.1.2/pykasso/_misc/statistics.xlsx` & `pykasso-0.1.3/pykasso/_misc/statistics.xlsx`

 * *Files identical despite different names*

### Comparing `pykasso-0.1.2/pykasso/_misc/statistics_old.xlsx` & `pykasso-0.1.3/pykasso/_misc/statistics_old.xlsx`

 * *Files identical despite different names*

### Comparing `pykasso-0.1.2/pykasso/_typing/types.py` & `pykasso-0.1.3/pykasso/_typing/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Custom pyKasso's typing."""
 
 # Typing
 from typing import TypeVar, TYPE_CHECKING
 
 from numpy import random
 from pandas import core, io
-from matplotlib import path
 
 if TYPE_CHECKING:
     import pykasso.core.grid as pcg
     import pykasso.core.domain as pcd
     import pykasso.core.geologic_features as pcgf
 
 # Custom internal types
@@ -25,9 +24,7 @@
 # Numpy
 RandomNumberGenerator = TypeVar('RandomNumberGenerator',
                                 bound='random._generator.Generator')
 # Pandas
 Series = TypeVar('Series', bound='core.series.Series')
 DataFrame = TypeVar('DataFrame', bound='core.frame.DataFrame')
 Styler = TypeVar('Styler', bound='io.formats.style.Styler')
-# Matplotlib
-Path = TypeVar('Path', bound='path.Path')
```

### Comparing `pykasso-0.1.2/pykasso/analysis/analysis.py` & `pykasso-0.1.3/pykasso/analysis/analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
         Examples
         --------
         >>> import pykasso.analysis as pka
         >>> analysis = pka.Analysis('examples/betteraz/')
         """
         super().__init__(project_directory)
+        self.k = None
         
     def compute_metrics(self) -> DataFrame:
         """
         Computes the statistical metrics for each simulated karst network
         using the karstnet package.
 
         Returns
@@ -98,17 +99,19 @@
             # Drops last item in list (the node type) for each dictionary entry
             for key, value in karstnet_nodes.items():
                 value.pop()
 
             # Computes karstnet metrics
             # Makes graph - edges must be a list, and nodes must be a dic of
             # format {nodeindex: [x,y]}
-            k = kn.KGraph(karstnet_edges, karstnet_nodes)
+            self.edges = karstnet_edges  # TODO - remove self
+            self.nodes = karstnet_nodes  # TODO - remove self
+            self.k = kn.KGraph(karstnet_edges, karstnet_nodes)  # TODO - remove self
             verbosity = 0
-            metrics = k.characterize_graph(verbosity)
+            metrics = self.k.characterize_graph(verbosity)
 
             # Concatenates dataframes
             df_ = pd.DataFrame(metrics, index=[i])
             df_metrics = pd.concat([df_metrics, df_])
 
         return df_metrics
 
@@ -177,15 +180,15 @@
         Examples
         --------
         >>> import pykasso.analysis as pka
         >>> analysis = pka.Analysis('examples/betteraz/')
         >>> karst_mean = analysis.compute_average_karstic_network()
         """
         # Initialization
-        nx, ny, nz = self._get_grid_shape()
+        nx, ny, nz = self._get_grid_dimensions()
         karst_map = np.zeros((nx, ny, nz))
         # For each simulation, retrieves data and sums it
         for path in self.project_state['simulation_locations']:
             results = self._read_pickle(path + 'results.pickle')
             karst_map = np.add(karst_map, results['maps']['karst'][-1]).copy()
         # Calculates the mean
         out = karst_map / self.project_state['n_simulation']
```

### Comparing `pykasso-0.1.2/pykasso/core/_validations.py` & `pykasso-0.1.3/pykasso/core/_validations.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,84 +3,85 @@
 """
 
 import PIL
 import os
 import sys
 import logging
 import numpy as np
+from shapely.geometry import Point
 
 ############
 ### TODO ###
 ############
 # validations verbosity
-# revoir la VERBOSITY des messages 
-# message different quand la feature est vide ?? 
+# revoir la VERBOSITY des messages
+# message different quand la feature est vide ??
 
-sks  = sys.modules['pykasso.core.sks']
+sks = sys.modules['pykasso.core.sks']
 this = sys.modules[__name__]
 
 this.ATTRIBUTES = {
-    'sks' : {
-        'seed'      : ['optional', 0],
-        'algorithm' : ['optional', 'Isotropic3'],
-        'costs'     : ['optional', {}],
-        'modes'     : ['optional', {}],
+    'sks': {
+        'seed': ['optional', 0],
+        'algorithm': ['optional', 'Isotropic3'],
+        'costs': ['optional', {}],
+        'mode': ['optional', 'A'],
     },
-    'grid' : {
-        'x0' : ['required', ''],
-        'y0' : ['required', ''],
-        'z0' : ['required', ''],
-        'nx' : ['required', ''],
-        'ny' : ['required', ''],
-        'nz' : ['required', ''],
-        'dx' : ['required', ''],
-        'dy' : ['required', ''],
-        'dz' : ['required', ''],
+    'grid': {
+        'x0': ['required', ''],
+        'y0': ['required', ''],
+        'z0': ['required', ''],
+        'nx': ['required', ''],
+        'ny': ['required', ''],
+        'nz': ['required', ''],
+        'dx': ['required', ''],
+        'dy': ['required', ''],
+        'dz': ['required', ''],
     },
-    'domain' : {
-        'delimitation' : ['optional', ''],
-        'topography'   : ['optional', ''],
-        'bedrock'      : ['optional', ''],
-        'water_level'  : ['optional', ''],
+    'domain': {
+        'delimitation': ['optional', ''],
+        'topography': ['optional', ''],
+        'bedrock': ['optional', ''],
+        'water_level': ['optional', ''],
     },
-    'geology' : {
-        'data' : ['optional', ''],
-        'axis' : ['optional', 'z'],
+    'geology': {
+        'data': ['optional', ''],
+        'axis': ['optional', 'z'],
     },
-    'beddings' : {
-        'data'  : ['optional', ''],
+    'beddings': {
+        'data': ['optional', ''],
     },
-    'faults' : {
-        'data' : ['optional', ''],
-        'axis' : ['optional', 'z'],
+    'faults': {
+        'data': ['optional', ''],
+        'axis': ['optional', 'z'],
     },
-    'outlets' : {
-        'number'     : ['required', ''],
-        'data'       : ['optional', ''],
-        'shuffle'    : ['optional', False],
-        'importance' : ['required', []],
-        'mode'       : ['optional', 'surface_down'],
-        'geology'    : ['optional', None],
-        'seed'       : ['optional', 0],
+    'outlets': {
+        'number': ['required', ''],
+        'data': ['optional', ''],
+        'shuffle': ['optional', False],
+        'importance': ['required', []],
+        'mode': ['optional', 'surface_down'],
+        'geology': ['optional', None],
+        'seed': ['optional', 0],
     },
-    'inlets'  : {
-        'number'     : ['required', ''],
-        'data'       : ['optional', ''],
-        'shuffle'    : ['optional', False],
-        'importance' : ['required', []],
-        'per_outlet' : ['required', []],
-        'mode'       : ['optional', 'surface_up'],
-        'geology'    : ['optional', None],
-        'seed'       : ['optional', 0],
+    'inlets': {
+        'number': ['required', ''],
+        'data': ['optional', ''],
+        'shuffle': ['optional', False],
+        'importance': ['required', []],
+        'per_outlet': ['required', []],
+        'mode': ['optional', 'surface_up'],
+        'geology': ['optional', None],
+        'seed': ['optional', 0],
     },
-    'tracers'   : {},
-    'fractures' : {
-        'data'     : ['optional', ''],
-        'axis'     : ['optional', 'z'],
-        'seed'     : ['optional', 0],
+    'tracers': {},
+    'fractures': {
+        'data': ['optional', ''],
+        'axis': ['optional', 'z'],
+        'seed': ['optional', 0],
     },
 }
 
 #################
 ### FUNCTIONS ###
 #################
 
@@ -248,15 +249,15 @@
 ############
 
 ####################################################################################
 ####################################################################################
 ####################################################################################
 
 def validate_settings(feature:str, feature_settings:dict, grid=None) -> dict:
-    """ 
+    """
     TODO
     """
     if feature == 'sks': 
         settings = validate_sks_settings(feature_settings)
     elif feature == 'grid':
         settings = validate_grid_settings(feature_settings)
     elif feature == 'domain':
@@ -283,22 +284,14 @@
         
     # Checks the presence of essential fmm costs
     costs = ['ratio', 'conduits', 'out']
     for cost in costs:
         if cost not in settings['costs']:
             settings['costs'][cost] = sks.default_fmm_costs[cost]
             
-    # Checks the presence of modes
-    modes = {
-        'elevation': True,
-        'bedrock': True,
-    }
-    for elem, value in modes.items():
-        if elem not in settings['modes']:
-            settings['modes'][elem] = value
     return settings
 
 ############
 ### GRID ###
 ############
 def validate_grid_settings(settings:dict) -> dict:
     # Checks attributes presence
@@ -379,15 +372,15 @@
     
     # Checks type of coordinates
     for vertex in data:
         for coordinate in vertex:
             is_coordinate_type_valid(coordinate, (int, float), 'delimitation')
             
     # Checks if vertex are well in grid limits
-    validated_vertices = [k for k,(x,y) in enumerate(data) if (grid.path.contains_point((x,y)) == True)]
+    validated_vertices = [k for k,(x,y) in enumerate(data) if (grid.polygon.contains(Point(x,y)) == True)]
 
     if len(validated_vertices) < 3:
         msg = "Not enough vertices inside the grid limits to create a delimitation (3 minimum)."
         this.logger.critical(msg)
         raise ValueError(msg)
 
     if len(validated_vertices) < len(data):
```

### Comparing `pykasso-0.1.2/pykasso/core/_wrappers.py` & `pykasso-0.1.3/pykasso/core/_wrappers.py`

 * *Files identical despite different names*

### Comparing `pykasso-0.1.2/pykasso/core/domain.py` & `pykasso-0.1.3/pykasso/core/domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 """
 
 ### Local dependencies
 from .geologic_features import Surface
 
 ### External dependencies
 import numpy as np
-from matplotlib.path import Path
+from shapely.geometry import Point, Polygon
 from scipy.ndimage import binary_dilation
 
 ### Typing
-from typing import Union
 from pykasso._typing import Grid, Delimitation, Topography, Bedrock, WaterLevel
 
 
 class Domain():
     """
     Class modeling the spatial extension of the domain within the study site
     grid locating where karstic network generation is allowed.
@@ -57,15 +56,15 @@
         # Computes volumetric domain extension
         if delimitation is not None:
             self.data_volume += delimitation.data_volume
         if topography is not None:
             self.data_volume += topography.data_volume
         if bedrock is not None:
             self.data_volume += np.logical_not(bedrock.data_volume).astype(int)
-        # only keeps cells where all the classes joins
+        # only keeps cells where all the classes join
         test = self.data_volume == self.data_volume.max()
         self.data_volume = np.where(test, 1, 0)
             
         # Computes apparent surface from domain according to axis
         self.data_surfaces = {
             'x': self.data_volume.max(axis=0),
             'y': self.data_volume.max(axis=1),
@@ -75,16 +74,18 @@
         ### Computes subdomains from the lower and upper surfaces of the domain
         self._set_faces()
         
         ### Computes subdomains from the borders of the domain
         self._set_border_domains()
         
         ### Computes subdomains from water level elevation model
-        if self.water_level is not None:
-            self._set_phreatic_domains()
+        self._set_phreatic_domains()
+        
+        ### Computes subdomains from bedrock elevation model
+        self._set_bedrock_domains()
             
         ### Names the subdomains
         self.subdomains_names = {
             # domain
             "domain": "self.data_volume",
             "domain_surface": "self.faces['up']",
             "domain_bottom": "self.faces['down']",
@@ -159,40 +160,77 @@
         self.borders['domain_down'] = (
             np.logical_and(self.borders['domain_sides'], self.faces['down'])
         )
         return None
         
     def _set_phreatic_domains(self) -> None:
         """Computes the subdomains derivated from the water level elevation."""
-        water_volume = self.water_level.data_volume
-        water_surface = self.water_level._surface_to_volume('=', self.grid)
+        if self.water_level is None:
+            vadose_zone = self.data_volume.copy()
+            phreatic_zone = np.zeros_like(self.grid.data_volume)
+            water_level_surface = np.zeros_like(self.grid.data_volume)
+            vadose_zone_borders = self.borders['domain_sides']
+            phreatic_zone_borders = np.zeros_like(self.grid.data_volume)
+            wls_borders = np.zeros_like(self.grid.data_volume)
+        else:
+            water_volume = self.water_level.data_volume
+            water_surface = self.water_level._surface_to_volume('=', self.grid)
+            
+            vadose_zone = np.logical_and(self.data_volume,
+                                         np.logical_not(water_volume))
+            phreatic_zone = np.logical_and(self.data_volume, water_volume)
+            water_level_surface = (
+                np.logical_and(self.data_volume, water_surface)
+            )
+            
+            # Water level surface border
+            vadose_zone_borders = np.logical_and(
+                self.borders['domain_sides'], vadose_zone)
+            phreatic_zone_borders = np.logical_and(
+                self.borders['domain_sides'], phreatic_zone)
+            wls_borders = np.logical_and(
+                self.borders['domain_sides'], water_level_surface)
         
-        vadose_zone = np.logical_and(self.data_volume,
-                                     np.logical_not(water_volume))
-        phreatic_zone = np.logical_and(self.data_volume, water_volume)
-        water_level_surface = np.logical_and(self.data_volume, water_surface)
+        # Sets the new domains
         self.phreatic = {
             'vadose_zone': vadose_zone,
             'phreatic_zone': phreatic_zone,
             'water_level_surface': water_level_surface,
+            
         }
-        
-        # Water level surface border
-        vadose_zone_borders = np.logical_and(self.borders['domain_sides'],
-                                             self.phreatic['vadose_zone'])
-        phreatic_zone_borders = np.logical_and(self.borders['domain_sides'],
-                                               self.phreatic['phreatic_zone'])
-        wls_borders = np.logical_and(self.borders['domain_sides'],
-                                     self.phreatic['water_level_surface'])
         self.borders['vadose_zone'] = vadose_zone_borders
         self.borders['phreatic_zone'] = phreatic_zone_borders
         self.borders['water_level_surface'] = wls_borders
         
         return None
     
+    def _set_bedrock_domains(self) -> None:
+        """ """
+        if self.bedrock is None:
+            bedrock = np.zeros_like(self.grid.data_volume)
+            bedrock_vadose = np.zeros_like(self.grid.data_volume)
+            bedrock_phreatic = np.zeros_like(self.grid.data_volume)
+        else:
+            roll_value = 2
+            bedrock = (
+                np.roll(self.bedrock.data_volume, roll_value, axis=2)
+            )
+            bedrock_vadose = np.logical_and(bedrock,
+                                            self.phreatic['vadose_zone'])
+            bedrock_phreatic = np.logical_and(bedrock,
+                                              self.phreatic['phreatic_zone'])
+        
+        # Sets the new domains
+        self.bedrock_domains = {
+            'bedrock': bedrock,
+            'bedrock_vadose': bedrock_vadose,
+            'bedrock_phreatic': bedrock_phreatic,
+        }
+        return None
+    
     ###############
     ### METHODS ###
     ###############
     
     def get_subdomain(self, subdomain_name: str) -> np.ndarray:
         """Returns the numpy.ndarray modeling the requested subdomain.
 
@@ -276,21 +314,29 @@
         y : float
             y-coordinate.
 
         Returns
         -------
         out : bool
         """
-        if self.grid.path.contains_point((x, y)):
+        point = Point(x, y)
+        if self.grid.polygon.contains(point):
             i, j = self.grid.get_indices(x, y)
             out = bool(self.data_surfaces['z'][i, j])
-            return out
+        elif self.grid.polygon.touches(point):
+            i, j = self.grid.get_indices(x, y)
+            test_x = self.grid.is_x_valid(x)
+            test_y = self.grid.is_y_valid(y)
+            if test_x and test_y:
+                out = bool(self.data_surfaces['z'][i, j])
+            else:
+                out = False
         else:
             out = False
-            return out
+        return out
         
     
 #################################
 ### Domain's embedded classes ###
 #################################
     
 class Delimitation():
@@ -308,65 +354,58 @@
             List of vertices.
         grid : Grid
             Grid of the model.
         """
         self.label = 'delimitation'
         self.vertices = vertices
         
-        ### Sets the polygon with a matplotlib Path
+        ### Sets the polygon with shapely
         path_vertices = self.vertices.copy()
-        path_vertices.append(path_vertices[0])
-        self.path = Path(path_vertices)
+        self.polygon = Polygon(path_vertices)
         
         ### Sets the mask array with a numpy-array
         row, col = np.indices((grid.nx, grid.ny))
         pts = np.column_stack((grid.X[row, col, 0].flatten(),
                                grid.Y[row, col, 0].flatten()))
-        msk = self.path.contains_points(pts).reshape((grid.nx, grid.ny)
-                                                     ).astype(int)
+        msk = [self.polygon.contains(Point(x, y)) for (x, y) in pts]
+        msk = np.array(msk).reshape((grid.nx, grid.ny)).astype(int)
         self.data_volume = np.repeat(msk[:, :, np.newaxis], grid.nz, axis=2)
         
 
 class Topography(Surface):
     """
     Class modeling the topography, the horizontal upper limit of the study
     site.
     """
     
-    def __init__(self, data: Union[str, np.ndarray], grid: Grid,
-                 **kwargs) -> None:
+    def __init__(self, *args, **kwargs) -> None:
         label = 'topography'
-        super().__init__(label, data, grid, **kwargs)
-        self.data_volume = self._surface_to_volume('<=', grid)
+        super().__init__(label, *args, **kwargs)
         
         
 class Bedrock(Surface):
     """
     Class modeling the bedrock elevation, the horizontal lower limit of the
     study site.
     """
     
-    def __init__(self, data: Union[str, np.ndarray], grid: Grid,
-                 **kwargs) -> None:
+    def __init__(self, *args, **kwargs) -> None:
         label = 'bedrock_elevation'
-        super().__init__(label, data, grid, **kwargs)
-        self.data_volume = self._surface_to_volume('<=', grid)
+        super().__init__(label, *args, **kwargs)
         
         
 class WaterLevel(Surface):
     """
     Class modeling the water level elevation, the phreatic/vadose limit of the
     study site.
     """
     
-    def __init__(self, data: Union[str, np.ndarray], grid: Grid,
-                 **kwargs) -> None:
+    def __init__(self, *args, **kwargs) -> None:
         label = 'water_level'
-        super().__init__(label, data, grid, **kwargs)
-        self.data_volume = self._surface_to_volume('<=', grid)
+        super().__init__(label, *args, **kwargs)
 
 
 #####################
 ### Documentation ###
 #####################
 
 subdomains_list = """
```

### Comparing `pykasso-0.1.2/pykasso/core/fracturation.py` & `pykasso-0.1.3/pykasso/core/fracturation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,115 @@
 """
 This module contains fonctions designed for fracture generation and
 discretization.
 """
 
-### Internal dependencies
-import math
-
 ### External dependencies
 import mpmath
 import numpy as np
 import pandas as pd
 
+### Local dependencies
+from pykasso.core.geologic_features import Volume
+
 ### Typing
 from pykasso._typing import Grid, RandomNumberGenerator
 
 ## TODO
 # equation _solve_kappa, -1 ???
 # distribution vonmises arguments : mean, std / loc, scale
 # (https://numpy.org/doc/stable/reference/random/generated/numpy.random.normal.html)
 
 
-class FracturesGenerator():
-    """
-    TODO
-    """
+class Fractures(Volume):
+    """Class modeling the fracturation model."""
     
-    def __init__(self, rng: RandomNumberGenerator, grid: Grid):
-        """
-        TODO
-        """
+    def __init__(self, rng: RandomNumberGenerator, *args, **kwargs):
+        label = 'fractures'
+        super().__init__(label, *args, **kwargs)
+        
         self.rng = rng
-        self.grid = grid
+        self.i = 0
+        self.families = pd.DataFrame()
+        self.fractures = pd.DataFrame()
+        self.fractures_voxelized = {}
+        
+    def generate_fracture_family(self, name, grid, **settings):
+        self.i = self.i + 1
+        if 'cost' in settings:
+            cost = settings['cost']
+            del settings['cost']
+        
+        # Creates family
+        frac_family = {
+            'id': [self.i],
+            'name': [name],
+            'cost': [cost],
+            # 'geology': pass # TODO - add geology
+        }
+        frac_family = pd.DataFrame(data=frac_family)
+            
+        # Generates fractures
+        fractures = self.generate_fractures(grid, **settings)
+        fractures.insert(0, 'family_id', self.i)
+        
+        # Updates tables
+        self.fractures = pd.concat([self.fractures, fractures])
+        self.families = pd.concat([self.families, frac_family])
+        
+        # Voxelizes the fractures
+        self.fractures_voxelized[self.i] = voxelize_fractures(grid, fractures)
+        return None
+     
+    def generate_model(self):
+        """Constructs the model for fracturation."""
+
+        frac_model = np.zeros_like(self.fractures_voxelized[self.i])
+        
+        # Sorts fracture families by cost
+        self.families = self.families.sort_values(['cost', 'id'])
+        fractures_family_ids = self.families['id'].values
+        
+        # Updates the final array
+        for family_id in fractures_family_ids:
+            frac_model = np.where(
+                self.fractures_voxelized[family_id] == 1,
+                family_id,
+                frac_model
+            )
+        self.data_volume = frac_model
         
-    def generate_fractures(self, density: float, alpha: float,
+        # Sets the costs
+        costs = pd.Series(self.families['cost'].values,
+                          index=self.families['id']).to_dict()
+        self._set_costs(costs)
+        
+        ######### TODO #########
+        # Sums fractures families
+        # frac_sum = sum([d for d in self.fractures_voxelized.values()])
+        # self.fractures_families['sum'] = frac_sum
+        ###
+        
+        # # Constraints model with geology if provided
+        # if 'geology' in kwargs:
+        #     frac_model_geology = np.zeros_like(frac_model)
+        #     for geologic_id in kwargs['geology']:
+        #         frac_model_geology = np.where(
+        #             Geology.data_volume == geologic_id,
+        #             frac_model,
+        #             frac_model_geology
+        #         )
+        #     self.fractures_families['model'] = frac_model_geology
+                
+        # data = self.fractures_families['model']
+        ######### TODO #########
+        
+        return None
+                
+    def generate_fractures(self, grid, density: float, alpha: float,
                            orientation: float, dip: float,
                            length: float,
                            orientation_distribution: str = 'vonmises',
                            dip_distribution: str = 'vonmises',
                            length_distribution: str = 'power'):
         """
         TODO
@@ -65,30 +138,30 @@
         if isinstance(length, (list)):
             length_min, length_max = min(length), max(length)
         else:
             length_distribution = 'unique'
             length_max = length
 
         ### Redefine fracturation domain
-        Lx = self.grid.xmax - self.grid.xmin
-        Ly = self.grid.ymax - self.grid.ymin
-        Lz = self.grid.zmax - self.grid.zmin
+        Lx = grid.xmax - grid.xmin
+        Ly = grid.ymax - grid.ymin
+        Lz = grid.zmax - grid.zmin
 
         shift_x = min(Lx / 2, length_max / 2)
         shift_y = min(Ly / 2, length_max / 2)
         shift_z = min(Lz / 2, length_max / 2)
 
         Lex = 2 * shift_x + Lx
         Ley = 2 * shift_y + Ly
         Lez = 2 * shift_z + Lz
 
         area = Lex * Ley
-        xmin = self.grid.xmin - shift_x
-        ymin = self.grid.ymin - shift_y
-        zmin = self.grid.zmin - shift_z
+        xmin = grid.xmin - shift_x
+        ymin = grid.ymin - shift_y
+        zmin = grid.zmin - shift_z
 
         ### Total numbers of fractures
         fractures_numbers = np.array(density) * area
 
         ### Generate poisson number for each fracture family
         real_frac_number = self.rng.poisson(fractures_numbers)
         
@@ -119,24 +192,25 @@
                                                          real_frac_number)
         
         # Von Mises distribution case
         elif orientation_distribution == 'vonmises':
             # Computes ...
             orient_mean_angle = (orientation_max + orientation_min) / 2
             orient_std_angle = (orientation_max - orient_mean_angle) / 3
-            orient_mean_angle_rad = math.radians(orient_mean_angle)
-            orient_std_angle_rad = math.radians(orient_std_angle)
+            orient_mean_angle_rad = np.radians(orient_mean_angle)
+            orient_std_angle_rad = np.radians(orient_std_angle)
 
             # Computes the kappa value for the Von Mises orient. distribution
             orient_kappa = self._solve_kappa(orient_std_angle_rad)
             orientation_fractures = (
                 self._random_vonmises(orient_mean_angle_rad,
                                       orient_kappa,
                                       real_frac_number)
             )
+            orientation_fractures = np.degrees(orientation_fractures)
             
         ##### FRACTURE DIP
         
         if dip_min > dip_max:
             dip_min = dip_min - 360
 
         # No distribution case
@@ -149,24 +223,25 @@
                                                  dip_max,
                                                  real_frac_number)
             
         # Von Mises distribution case
         elif dip_distribution == 'vonmises':
             dip_mean_angle = (dip_max + dip_min) / 2
             dip_std_angle = (dip_max - dip_mean_angle) / 3
-            dip_mean_angle_rad = math.radians(dip_mean_angle)
-            dip_std_angle_rad = math.radians(dip_std_angle)
+            dip_mean_angle_rad = np.radians(dip_mean_angle)
+            dip_std_angle_rad = np.radians(dip_std_angle)
             
             # Computes the kappa value for the Von Mises orient. distribution
             dip_kappa = self._solve_kappa(dip_std_angle_rad)
             dip_fractures = (
                 self._random_vonmises(dip_mean_angle_rad,
                                       dip_kappa,
                                       real_frac_number)
             )
+            dip_fractures = np.degrees(dip_fractures)
 
         ##### FRACTURE LENGHT
 
         # No distribution case
         if length_distribution == 'unique':
             radius = [length / 2] * real_frac_number
 
@@ -190,15 +265,15 @@
         #######################
         
         data = {
             'x': xm,
             'y': ym,
             'z': zm,
             'radius': radius,
-            'orientation': np.degrees(orientation_fractures),
+            'orientation': orientation_fractures,
             'dip': dip_fractures,
             'normal': normal
         }
         fractures = pd.DataFrame(data=data)
 
         return fractures
 
@@ -234,17 +309,19 @@
         u = self.rng.random(size=n)
         out = (fmina + u * frangea)**invpalpha
         return out
 
  
 def calculate_normal(dip, orientation):
     """"""
-    x = np.cos(np.radians(dip)) * np.cos(np.radians(90) - orientation)
-    y = np.cos(np.radians(dip)) * np.sin(np.radians(90) - orientation)
-    z = np.sin(np.radians(90) - np.radians(dip))
+    orientation = np.radians(orientation)
+    dip = np.radians(dip)
+    x = np.cos(dip) * np.cos(np.radians(90) - orientation)
+    y = np.cos(dip) * np.sin(np.radians(90) - orientation)
+    z = np.sin(np.radians(90) - dip)
     a = y
     b = -x
     c = -z
     normal = list(zip(a, b, c))
     return normal
```

### Comparing `pykasso-0.1.2/pykasso/core/grid.py` & `pykasso-0.1.3/pykasso/core/grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
 This module contains a class modeling a structured grid.
 """
 
 ### External dependencies
 import numpy as np
-from matplotlib.path import Path
-
-### Typing
-from pykasso._typing import Path as pyplotPath  # TODO
+from shapely.geometry import Polygon
 
 
 class Grid():
     """
     This class models the three dimensional structured grid of the studied
     domain.
     """
@@ -107,16 +104,16 @@
         self.__shape = (nx, ny, nz)  # shape of the modeling array
         
         # Other attributes used in further geometrical operations
         x_path = [self.__xlimits[0], self.__xlimits[0], self.__xlimits[1],
                   self.__xlimits[1], self.__xlimits[0]]
         y_path = [self.__ylimits[0], self.__ylimits[1], self.__ylimits[1],
                   self.__ylimits[0], self.__ylimits[0]]
-        self.__path = Path(list(zip(x_path, y_path)))
         self.__surface_coordinates = list(zip(x_path[:-1], y_path[:-1]))
+        self.__polygon = Polygon(self.__surface_coordinates)
         
     def __str__(self) -> str:
         txt = ("pyKasso's grid"
                "\n[x0, y0, z0] : ({}, {}, {})"
                "\n[nx, ny, nz] : ({}, {}, {})"
                "\n[dx, dy, dz] : ({}, {}, {})"
                .format(self.x0, self.y0, self.z0,
@@ -287,25 +284,25 @@
         """Gets the array modeling the grid."""
         return self.__data_volume
     
     @property
     def shape(self) -> tuple:
         """Gets the dimensions of the grid."""
         return self.__shape
-
-    @property
-    def path(self) -> Path:
-        """Gets the path."""
-        return self.__path
     
     @property
     def surface_coordinates(self) -> list:
         """Gets the surface coordinates."""
         return self.__surface_coordinates
 
+    @property
+    def polygon(self) -> Polygon:
+        """Gets the surface polygon."""
+        return self.__polygon
+    
     ###############
     ### METHODS ###
     ###############
 
     def get_i(self, x: float) -> int:
         """
         Retrieves i-index from x-coordinate.
@@ -313,77 +310,77 @@
         Parameters
         ----------
         x : float
             x-coordinate.
 
         Returns
         -------
-        out : int
+        i : int
             i-index.
 
         Examples
         --------
         >>> grid = pk.Grid(0, 0, 0, 10, 10, 10, 10, 20, 30)
         >>> grid.get_i(70)
         7
         """
         x = np.array(x)
-        out = np.ceil((x - self.x0 - self.dx / 2) / self.dx)
-        out = out.astype('int32')
-        return out
+        i = np.floor((x - (self.x0 - (self.dx / 2))) / self.dx)
+        i = i.astype('int32')
+        return i
 
     def get_j(self, y: float) -> int:
         """
         Retrieves j-index from y-coordinate.
 
         Parameters
         ----------
         y : float
             y-coordinate.
 
         Returns
         -------
-        out : int
+        j : int
             j-index.
 
         Examples
         --------
         >>> grid = pk.Grid(0, 0, 0, 10, 10, 10, 10, 20, 30)
         >>> grid.get_j(70)
         3
         """
         y = np.array(y)
-        out = np.ceil((y - self.y0 - self.dy / 2) / self.dy)
-        out = out.astype('int32')
-        return out
+        j = np.floor((y - (self.y0 - (self.dy / 2))) / self.dy)
+        j = j.astype('int32')
+        return j
 
     def get_k(self, z: float) -> int:
         """
         Retrieves k-index from z-coordinate.
 
         Parameters
         ----------
         z : float
             z-coordinate.
 
         Returns
         -------
-        out : int
+        k : int
             k-index.
 
         Examples
         --------
         >>> grid = pk.Grid(0, 0, 0, 10, 10, 10, 10, 20, 30)
         >>> grid.get_k(70)
         2
         """
         z = np.array(z)
-        out = np.ceil((z - self.z0 - self.dz / 2) / self.dz)
-        out = out.astype('int32')
-        return out
+        k = np.floor((z - (self.z0 - (self.dz / 2))) / self.dz)
+        k = k.astype('int32')
+        return k
     
     def get_indices(self, x: float, y: float, z: float = None) -> tuple:
         """
         Retrieves both i and j-index from x and y-coordinates. Returns also
         k-index when z-coordinate is provided.
 
         Parameters
@@ -522,19 +519,69 @@
         """
         if k is None:
             out = (self.get_x(i), self.get_y(j))
             return out
         else:
             out = (self.get_x(i), self.get_y(j), self.get_z(k))
             return out
+        
+    def is_x_valid(self, x: float) -> bool:
+        """
+        Returns true if the x-coordinate is inside the grid domain.
+
+        Parameters
+        ----------
+        x : float
+            x-coordinate.
+
+        Returns
+        -------
+        out : bool
+        """
+        i = self.get_i(x)
+        out = bool((i - self.nx + 1) * i <= 0)
+        return out
+    
+    def is_y_valid(self, y: float) -> bool:
+        """
+        Returns true if the y-coordinate is inside the grid domain.
+
+        Parameters
+        ----------
+        y : float
+            y-coordinate.
+
+        Returns
+        -------
+        out : bool
+        """
+        j = self.get_j(y)
+        out = bool((j - self.ny + 1) * j <= 0)
+        return out
+    
+    def is_z_valid(self, z: float) -> bool:
+        """
+        Returns true if the z-coordinate is inside the grid domain.
+
+        Parameters
+        ----------
+        z : float
+            z-coordinate.
+
+        Returns
+        -------
+        out : bool
+        """
+        k = self.get_k(z)
+        out = bool((k - self.nz + 1) * k <= 0)
+        return out
 
     def is_inbox(self, x: float, y: float, z: float) -> bool:
         """
-        Returns true if a (x, y, z)-coordinate point is inside the grid,
-        otherwise false.
+        Returns true if a (x, y, z)-coordinate point is inside the grid.
 
         Parameters
         ----------
         x : float
             x-coordinate.
         y : float
             y-coordinate.
@@ -549,12 +596,9 @@
         --------
         >>> grid = pk.Grid(0, 0, 0, 10, 10, 10, 10, 20, 30)
         >>> grid.is_inbox(70, 70, 70)
         True
         >>> grid.is_inbox(70, 70, 1000)
         False
         """
-        i, j, k = self.get_i(x), self.get_j(y), self.get_k(z)
-        out = (bool((k - self.nz + 1) * k <= 0)
-               and ((j - self.ny + 1) * j <= 0)
-               and ((i - self.nx + 1) * i <= 0))
+        out = self.is_x_valid(x) and self.is_y_valid(y) and self.is_z_valid(z)
         return out
```

### Comparing `pykasso-0.1.2/pykasso/core/points.py` & `pykasso-0.1.3/pykasso/core/points.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 ### Internal dependencies
 import logging
 
 ### External dependencies
 import numpy as np
+from shapely.geometry import Point
 
 ### Typing
 from pykasso._typing import Domain, Geology, RandomNumberGenerator
 
 
 class PointGenerator():
     """
@@ -155,15 +156,16 @@
         return (x, y, z)
     
     def _is_coordinate_2D_valid(self, coordinate: tuple) -> bool:
         """Checks if the 2D point is valid."""
         x, y = coordinate
         if self.domain.is_coordinate_2D_valid(x, y):
             i, j = self.domain.grid.get_indices(x, y)
-            return self.valid_domain_surface[i, j]
+            out = self.valid_domain_surface[i, j]
+            return out
         else:
             return False
         
     def _is_coordinate_3D_valid(self, coordinate: tuple) -> bool:
         """Checks if the 3D points is valid."""
         x, y, z = coordinate
```

### Comparing `pykasso-0.1.2/pykasso/core/sks.py` & `pykasso-0.1.3/pykasso/core/sks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 """
-This module contains...
-
-
-Module modeling the karstic network generator tool.
+This module contains a class modeling the karstic network generator tool.
 """
 
-####################
-### Dependencies ###
-####################
-
 ### Internal dependencies
 import os
 import sys
 import copy
 import pickle
 import shutil
 import logging
 import datetime
 
-### Local dependencies
-import pykasso.core._wrappers as wp
-from .grid import Grid
-from .domain import Domain, Delimitation, Topography, Bedrock, WaterLevel
-from .geologic_features import Geology, Faults, Fractures
-from .points import PointGenerator
-
 ### External dependencies
 import yaml
 import numpy as np
 import pandas as pd
 
 ### Fast-Marching package
 import agd
 from agd import Eikonal
 from agd.Metrics import Riemann
 
+### Local dependencies
+import pykasso.core._wrappers as wp
+from .grid import Grid
+from .domain import Domain, Delimitation, Topography, Bedrock, WaterLevel
+from .geologic_features import Geology, Faults
+from .fracturation import Fractures
+from .points import PointGenerator
+
 ### Typing
 from pykasso._typing import DataFrame
 
 ### Module variables
 this = sys.modules[__name__]
 
 # Dictionary used for memory optimization/memoizing operations
 this.ACTIVE_PROJECT = None
 
 # Defines default fast-marching costs
 this.default_fmm_costs = {
-    # 'out'       : 0.999,
+    # 'out': 0.999,
     'out': 10,
     'aquifer': 0.4,
     'aquiclude': 0.8,
     'beddings': 0.35,
     'faults': 0.2,
     'fractures': 0.2,
     'karst': 0.1,
@@ -62,15 +56,15 @@
 this.misc_relative_path = '/../_misc/'
 
 ########################
 ### Module functions ###
 ########################
 
 
-def create_project(project_directory: str) -> None:
+def create_project(project_directory: str, example: str = None) -> None:
     """
     Creates a new pyKasso's project within the provided `project_directory`
     path.
     Three subdirectories will be created :
      - ``inputs/``, for input model data files
      - ``outputs/``, for model results storage
      - ``settings/``, for pyKasso's settings file
@@ -78,53 +72,63 @@
     .. warning:: pyKasso doesn't check if the directory already exists and if
     yes, its actual content.
 
     Parameters
     ----------
     project_directory : str
         Location, path of the new project directory.
+    example : str
+        __doc__ :
+        -"betteraz"
         
     Examples
     --------
     >>> import pykasso as pk
     >>> pk.create_project('examples/betteraz/')
     """
     # Uncomment this to tell apart the development version and the main version
     # print('CAUTION: You are using the development version of this package.')
     
     ### Creates the project subdirectories
-    core_settings = {
+    this.core_settings = {
         'project_directory': project_directory,
         'inputs_directory': project_directory + '/inputs/',
         'outputs_directory': project_directory + '/outputs/',
         'settings_directory': project_directory + '/settings/',
     }
     [os.makedirs(directory, exist_ok=True) for directory in core_settings.values()]
 
     ### Populates the settings directory with initial yaml settings file
     location = os.path.dirname(os.path.abspath(__file__))
     misc_directory = location + this.misc_relative_path
-    core_settings.update({
+    this.core_settings.update({
         'core_settings_filename': 'CORE_SETTINGS.yaml',
         'sks_settings_filename': 'SKS_SETTINGS.yaml',
         'log_filename': 'pyKasso.log',
     })
+    
+    # Copies directly the requested example from the _misc directory
+    if example is not None:
+        example = example.strip('/')
+        # path = 
+        return None
 
     ### Creates the CORE_SETTINGS.yaml file in the project directory
-    core_settings_filename = (core_settings['settings_directory']
-                              + core_settings['core_settings_filename'])
-    with open(core_settings_filename, 'w') as f:
-        text = "# pyKasso CORE SETTINGS \n---\n"
-        yaml_text = yaml.safe_dump(core_settings)
-        text = text + yaml_text + "..."
-        f.write(text)
+    # core_settings_filename = (core_settings['settings_directory']
+    #                           + core_settings['core_settings_filename'])
+    # with open(core_settings_filename, 'w') as f:
+    #     text = "# pyKasso CORE SETTINGS \n---\n"
+    #     yaml_text = yaml.safe_dump(core_settings)
+    #     text = text + yaml_text + "..."
+    #     f.write(text)
 
     ### Copies the default SKS_SETTINGS.yaml file from the misc directory to
     ### the project directory
-    shutil.copy2(misc_directory + core_settings['sks_settings_filename'], project_directory + '/settings/')
+    path = misc_directory + this.core_settings['sks_settings_filename']
+    shutil.copy2(path, project_directory + '/settings/')
 
     ### Constructs the dictionary used for settings comparison between actual
     ### and previous simulation, used for the memoization operation
     this.ACTIVE_PROJECT = this.ACTIVE_PROJECT = {
         'project_directory': project_directory,
         'n_simulation': 0,
         'simulation_locations': [],
@@ -215,16 +219,14 @@
 class SKS():
     """
     Class storing all the parameters, the data and the resulting simulated
     stochastic karst networks.
     
     Attributes
     ----------
-    CORE_SETTINGS : dict
-        ...
     SKS_SETTINGS : dict
         ...
     grid : _type_
         ...
     domain : _type_
         ...
     geology : _type_
@@ -237,24 +239,22 @@
         ...
     outlets : DataFrame
         ...
     
     .. note:: ``faults`` or ``fractures`` will return None when not defined.
     """
 
-    def __init__(self, sks_settings: dict = {}, core_settings: dict = {},
-                 export_settings: dict = {}, debug_level: dict = {}) -> None:
+    def __init__(self, sks_settings: dict = {}, export_settings: dict = {},
+                 debug_level: dict = {}) -> None:
         """Initializes an instance of SKS class.
 
         Parameters
         ----------
         sks_settings : dict, optional
             _description_, by default {}
-        core_settings : dict, optional
-            _description_, by default {}
         export_settings : dict, optional
             _description_, by default {}
         debug_level : dict, optional
             _description_, by default {}
             
         Examples
         --------
@@ -268,18 +268,18 @@
         self.faults = None
         self.fractures = None
         self.inlets = None
         self.outlets = None
         self.conceptual_model = None
         self.conceptual_model_table = None
         self.rng = {}
-        self.orientation = None # TODO
+        self.orientation = None  # TODO
         
         ### Loads core and sks settings
-        settings_list = [copy.deepcopy(core_settings),
+        settings_list = [copy.deepcopy(this.core_settings),
                          copy.deepcopy(sks_settings)]
         settings_names = ['CORE_SETTINGS', 'SKS_SETTINGS']
         for settings, settings_name in zip(settings_list, settings_names):
             if settings == {}:
                 settings = this.ACTIVE_PROJECT['project_directory'] + '/settings/{}.yaml'.format(settings_name)
             if isinstance(settings, str):
                 with open(settings, 'r') as f:
@@ -415,125 +415,149 @@
             this.logger.info('-> max. iteration : {}'.format(self.debug_level['iteration']))
             this.logger.info('---')
         
 ##########################
 ### BUILDING THE MODEL ###
 ##########################
 
-    def build_model(self) -> None:
+    def build(self) -> None:
         """
         Builds the geological model. Should be called right after ``SKS``
         class instantiation.
         
         Model building procedure:
          1. Constructs the grid : ``self.grid`` ;
          2. Defines the model extension : ``self.domain`` ;
          3. Builds the geological features : ``self.geology``, ``self.faults``,
          ``self.inlets``, ``self.outlets``, ``self.fractures``,
          ``self.conceptual_model``, ``self.conceptual_model_table``;
-         4. Prepares the fast-marching method variables : _TODO_ ;
+         4. Prepares the fast-marching method variables.
          
         If a geological feature has not been defined in the settings, calling
         its attribute will returns ``None``.
         
         Examples
         --------
         >>> import pykasso as pk
         >>> simulation = pk.SKS()
-        >>> simulation.build_model()
+        >>> simulation.build()
         """
         self._build_grid()               # 1 - Constructs the grid
         self._build_domain()             # 2 - Constructs the domain
         self._build_model()              # 3 - Constructs the model
         self._construct_fmm_variables()  # 4 - Constructs fmm features
         return None
     
     ##### 1 - GRID #########################
     @wp._debug_level(1)
     @wp._parameters_validation('grid', 'required')
     @wp._memoize('grid')
     @wp._logging()
     def _build_grid(self) -> None:
         """Builds the grid."""
-        self.grid = Grid(**self.SKS_SETTINGS['grid'])
+        if isinstance(self.SKS_SETTINGS['grid'], (str)):
+            # TODO builds the grid according to a .asc or .grd file
+            pass
+        else:
+            self.grid = Grid(**self.SKS_SETTINGS['grid'])
         return None
     
     ##### 2 - DOMAIN #########################
     @wp._debug_level(2)
     @wp._parameters_validation('domain', 'optional')
     @wp._memoize('domain')
     @wp._logging()
     def _build_domain(self) -> None:
         """Builds the domain."""
         delimitation = self._build_domain_delimitation()
         topography = self._build_domain_topography()
         bedrock = self._build_domain_bedrock()
         water_level = self._build_domain_water_level()
-        self.domain = Domain(self.grid, delimitation=delimitation,
+        self.domain = Domain(self.grid,
+                             delimitation=delimitation,
                              topography=topography,
                              bedrock=bedrock,
                              water_level=water_level)
         return None
     
     @wp._debug_level(2.1)
     @wp._logging()
-    def _build_domain_delimitation(self) -> None:
+    def _build_domain_delimitation(self):
         """Builds the delimitation."""
-        if not (isinstance(self.SKS_SETTINGS['domain']['delimitation'], (str))
-                and (self.SKS_SETTINGS['domain']['delimitation'] == '')):
-            if isinstance(self.SKS_SETTINGS['domain']['delimitation'], (str)):
-                self.SKS_SETTINGS['domain']['delimitation'] = (np.genfromtxt(self.SKS_SETTINGS['domain']['delimitation']).tolist())
-            return Delimitation(vertices=self.SKS_SETTINGS['domain']['delimitation'], grid=self.grid)
+        delimitation = self.SKS_SETTINGS['domain']['delimitation']
+        test_a = isinstance(delimitation, (str))
+        test_b = (delimitation == '')
+        if not (test_a and test_b):
+            if isinstance(delimitation, (str)):
+                delimitation = np.genfromtxt(delimitation).tolist()
+                self.SKS_SETTINGS['domain']['delimitation'] = delimitation
+            instance = Delimitation(vertices=delimitation, grid=self.grid)
+            return instance
         else:
             return None
 
     @wp._debug_level(2.2)
     @wp._logging()
-    def _build_domain_topography(self) -> None:
+    def _build_domain_topography(self):
         """Builds the topography."""
-        if not (isinstance(self.SKS_SETTINGS['domain']['topography'], (str)) and (self.SKS_SETTINGS['domain']['topography'] == '')):
-            return Topography(data=self.SKS_SETTINGS['domain']['topography'], grid=self.grid)
+        topography = self.SKS_SETTINGS['domain']['topography']
+        test_a = isinstance(topography, (str))
+        test_b = (topography == '')
+        if not (test_a and test_b):
+            instance = Topography()
+            instance.set_data(data=topography, grid=self.grid)
+            instance._surface_to_volume('<=', self.grid)
+            return instance
         else:
             return None
         
     @wp._debug_level(2.3)
     @wp._logging()
-    def _build_domain_bedrock(self) -> None:
+    def _build_domain_bedrock(self):
         """Builds the bedrock elevation."""
-        if not (isinstance(self.SKS_SETTINGS['domain']['bedrock'], (str)) and (self.SKS_SETTINGS['domain']['bedrock'] == '')):
-            return Bedrock(data=self.SKS_SETTINGS['domain']['bedrock'], grid=self.grid)
+        bedrock = self.SKS_SETTINGS['domain']['bedrock']
+        test_a = isinstance(bedrock, (str))
+        test_b = (bedrock == '')
+        if not (test_a and test_b):
+            instance = Bedrock()
+            instance.set_data(data=bedrock, grid=self.grid)
+            instance._surface_to_volume('<=', self.grid)
+            return instance
         else:
             return None
         
     @wp._debug_level(2.4)
     @wp._logging()
-    def _build_domain_water_level(self) -> None:
+    def _build_domain_water_level(self):
         """Builds the water level elevation."""
-        if not (isinstance(self.SKS_SETTINGS['domain']['water_level'], (str)) and (self.SKS_SETTINGS['domain']['water_level'] == '')):
-            return WaterLevel(data=self.SKS_SETTINGS['domain']['water_level'], grid=self.grid)
+        water_level = self.SKS_SETTINGS['domain']['water_level']
+        test_a = isinstance(water_level, (str))
+        test_b = (water_level == '')
+        if not (test_a and test_b):
+            instance = WaterLevel()
+            instance.set_data(data=water_level, grid=self.grid)
+            instance._surface_to_volume('<=', self.grid)
+            return instance
         else:
             return None
 
-        
     ##### 3 - MODEL #########################
     @wp._debug_level(3)
     @wp._logging()
     def _build_model(self) -> None:
         """Builds the geological features."""
         
         ### Sets the main parameters
         self._build_model_parameters()
         
-        ### Constructs deterministic geological features
-        self._build_model_geology()              
-        # TODO - self._build_model_beddings()
+        ### Constructs the deterministic geological features
+        self._build_model_geology()
         self._build_model_faults()
-        # TODO - self._build_model_karst()
 
-        ### Constructs stochastic geological features
+        ### Constructs the stochastic geological features
         self._build_model_outlets()
         self._build_model_inlets()
         # TODO - self._build_model_tracers()
         self._build_model_fractures()
         
         ### Constructs the conceptual model
         self._build_conceptual_model()
@@ -546,15 +570,16 @@
         
         # Generates a random seed when the seed equals 0 (default setting)
         if self.SKS_SETTINGS[attribute]['seed'] == 0:
             seed = np.random.default_rng().integers(low=0, high=10**6)
             self.SKS_SETTINGS[attribute]['seed'] = seed
             
         # Sets the seed
-        self.rng[attribute] = np.random.default_rng(self.SKS_SETTINGS[attribute]['seed'])
+        seed = self.SKS_SETTINGS[attribute]['seed']
+        self.rng[attribute] = np.random.default_rng(seed)
         return None
     
     @wp._debug_level(3.1)
     @wp._parameters_validation('sks', 'optional')
     def _build_model_parameters(self) -> None:
         """Builds characteristic model parameters."""
         # Defines the main seed
@@ -563,77 +588,72 @@
     
     @wp._debug_level(3.2)
     @wp._parameters_validation('geology', 'optional')
     @wp._memoize('geology')
     @wp._logging()
     def _build_model_geology(self) -> None:
         """Builds the geology."""
-        self.geology = Geology(**self.SKS_SETTINGS['geology'],
-                               grid=self.grid,
-                               domain=self.domain)
-        return None
-    
-    # @wp._debug_level(3.3)
-    # @wp._parameters_validation('beddings', 'optional')
-    # @wp._memoize('beddings')
-    # @wp._logging()
-    # def _build_model_beddings(self):
-    #     """Builds the beddings."""
-    #     if not (isinstance(self.SKS_SETTINGS['beddings']['data'], (str)) and (self.SKS_SETTINGS['beddings']['data'] == '')):
-    #         self.beddings = []
-    #         if isinstance(self.SKS_SETTINGS['beddings']['data'], (list)):
-    #             for data_bedding in self.SKS_SETTINGS['beddings']['data']:
-    #                 self.beddings.append(Bedding(data=data_bedding, grid=self.grid))
-    #             data_volumes = [bedding.data_volume for bedding in self.beddings]
-    #             data_volume  = np.sum(data_volumes)
-    #             beddings = Volume(label='beddings', data=data_volume, grid=self.grid)
-    #             beddings._set_fmm_costs(costs=self.SKS_SETTINGS['beddings']['costs'])
-    #             self.beddings.append(beddings)
-    #         else:
-    #             beddings = Volume(label='beddings', data=self.SKS_SETTINGS['beddings']['data'], grid=self.grid)
-    #             beddings._set_fmm_costs(costs=self.SKS_SETTINGS['beddings']['costs'])
-    #             self.beddings.append(beddings)
-    #     else:
-    #         self.beddings = None
-    #     return None
-
-    @wp._debug_level(3.4)
+        geology = self.SKS_SETTINGS['geology']['data']
+        test_a = isinstance(geology, (str))
+        test_b = (geology == '')
+        self.geology = Geology()
+        if not (test_a and test_b):
+            axis = self.SKS_SETTINGS['geology']['axis']
+            self.geology.set_data(data=geology, grid=self.grid, axis=axis)
+        else:
+            self.geology.data_volume = (
+                self.geology._set_data_full_3D(grid=self.grid, value=1)
+            )
+        costs = self.SKS_SETTINGS['geology']['costs']
+        self.geology._set_costs(costs)
+        self.geology._compute_statistics(self.grid)
+        return None
+    
+    @wp._debug_level(3.3)
     @wp._parameters_validation('faults', 'optional')
     @wp._memoize('faults')
     @wp._logging()
     def _build_model_faults(self) -> None:
         """Builds the faults."""
-        if not (isinstance(self.SKS_SETTINGS['faults']['data'], (str)) and (self.SKS_SETTINGS['faults']['data'] == '')):
-            self.faults = Faults(**self.SKS_SETTINGS['faults'],
-                                 grid=self.grid,
-                                 domain=self.domain)
+        faults = self.SKS_SETTINGS['faults']['data']
+        test_a = isinstance(faults, (str))
+        test_b = (faults == '')
+        if not (test_a and test_b):
+            self.faults = Faults()
+            axis = self.SKS_SETTINGS['faults']['axis']
+            self.faults.set_data(data=faults, grid=self.grid, axis=axis)
+            costs = self.SKS_SETTINGS['faults']['costs']
+            self.faults._set_costs(costs)
+            self.faults._compute_statistics(self.grid)
         return None
 
     @wp._debug_level(3.5)
     @wp._parameters_validation('outlets', 'required')
     @wp._memoize('outlets')
     @wp._logging()
     def _build_model_outlets(self) -> None:
         """Builds the outlets."""
         self._set_rng('outlets')
         self.outlets = self._construct_feature_points('outlets')
         if self.SKS_SETTINGS['outlets']['shuffle']:
-            self.outlets = self.outlets.sample(frac=1, random_state=self.rng['sks']).reset_index(drop=True)
+            pts = self.outlets.sample(frac=1, random_state=self.rng['sks'])
+            self.outlets = pts.reset_index(drop=True)
         return None
 
     @wp._debug_level(3.6)
     @wp._parameters_validation('inlets', 'required')
     @wp._memoize('inlets')
     @wp._logging()
     def _build_model_inlets(self) -> None:
         """Builds the inlets."""
         self._set_rng('inlets')
         self.inlets = self._construct_feature_points('inlets')
         if self.SKS_SETTINGS['inlets']['shuffle']:
-            self.inlets = self.inlets.sample(frac=1, random_state=self.rng['sks']).reset_index(drop=True)
+            pts = self.inlets.sample(frac=1, random_state=self.rng['sks'])
+            self.inlets = pts.reset_index(drop=True)
         return None
     
     def _construct_feature_points(self, kind):
         """Constructs the inlets / outlets.
 
         Four cases possible:
          1. No points declared
@@ -646,29 +666,36 @@
         ### Creates a point generator instance
         point_manager = PointGenerator(
             rng=self.rng[kind],
             mode=self.SKS_SETTINGS[kind]['mode'],
             domain=self.domain,
             geology=self.geology,
             geologic_ids=self.SKS_SETTINGS[kind]['geology']
-        ) 
+        )
 
         ### Gets existing points
 
         # Loads points if needed
-        if isinstance(self.SKS_SETTINGS[kind]['data'], (str)) and not (self.SKS_SETTINGS[kind]['data'] == ''):
-            self.SKS_SETTINGS[kind]['data'] = np.genfromtxt(self.SKS_SETTINGS[kind]['data'])
+        logical_test_01 = isinstance(self.SKS_SETTINGS[kind]['data'], (str))
+        logical_test_02 = not (self.SKS_SETTINGS[kind]['data'] == '')
+        if logical_test_01 and logical_test_02:
+            path = self.SKS_SETTINGS[kind]['data']
+            self.SKS_SETTINGS[kind]['data'] = np.genfromtxt(path)
         
         ### Inspects validity of points
         points = self.SKS_SETTINGS[kind]['data']
         
         # 2D points # TODO - logging ?
         points_2D = [point for point in points if len(point) == 2]
-        validated_points_2D = [point for point in points_2D if point_manager._is_coordinate_2D_valid(point)]
-        validated_points_3D = [point_manager._generate_3D_coord_from_2D_coord(point) for point in validated_points_2D]
+        validated_points_2D = [point for point in points_2D
+                               if point_manager._is_coordinate_2D_valid(point)]
+        validated_points_3D = [
+            point_manager._generate_3D_coord_from_2D_coord(point)
+            for point in validated_points_2D
+        ]
         
         # 3D points # TODO - logging ?
         points_3D = [point for point in points if len(point) == 3]
         validated_points_3D += [point for point in points_3D if point_manager._is_coordinate_3D_valid(point)]
 
         diff = len(points) - len(validated_points_3D)
         if diff > 0:
@@ -709,85 +736,103 @@
     @wp._debug_level(3.8)
     @wp._parameters_validation('fractures', 'optional')
     @wp._memoize('fractures')
     @wp._logging()
     def _build_model_fractures(self) -> None:
         """Builds the fractures."""
         self._set_rng('fractures')
-        if (not (isinstance(self.SKS_SETTINGS['fractures']['data'], (str)) and (self.SKS_SETTINGS['fractures']['data'] == ''))) or ('settings' in self.SKS_SETTINGS['fractures']):
-            self.fractures = Fractures(**self.SKS_SETTINGS['fractures'], grid=self.grid, domain=self.domain, Geology=self.geology, rng=self.rng['fractures'])
-        else:
-            self.fractures = None
+        fractures = self.SKS_SETTINGS['fractures']['data']
+        test_a = isinstance(fractures, (str))
+        test_b = (fractures == '')
+        test_c = ('settings' in self.SKS_SETTINGS['fractures'])
+        if (not (test_a and test_b)) or test_c:
+            self.fractures = Fractures(rng=self.rng['fractures'])
+            axis = self.SKS_SETTINGS['fractures']['axis']
+            
+            # Generates fractures families
+            if 'settings' in self.SKS_SETTINGS['fractures']:
+                frac_settings = self.SKS_SETTINGS['fractures']['settings']
+                for frac_name, frac_settings in frac_settings.items():
+                    self.fractures.generate_fracture_family(frac_name,
+                                                            self.grid,
+                                                            **frac_settings)
+                self.fractures.generate_model()
+            # Loads data
+            else:
+                self.fractures.set_data(fractures, self.grid, axis)
+                costs = self.SKS_SETTINGS['fractures']['costs']
+                self.fractures._set_costs(costs)
+            
+            self.fractures._compute_statistics(self.grid)
         return None
     
     @wp._debug_level(3.9)
     @wp._logging()
     def _build_conceptual_model(self) -> None:
         """Builds the conceptual model.
         
         Data range attributions :
          - 100 - 199 : Geology
-         - 200 - 299 : Bedding
-         - 300 - 399 : Fractures
-         - 400 - 499 : Faults
-         - 500 - 599 : Karsts
+         - 200 - 299 : Fractures
+         - 300 - 399 : Faults
          - 0 - Out
-         - 600 - Bedrock - TODO
         """
         # Initialization
         conceptual_model = np.zeros_like(self.grid.data_volume)
         conceptual_model_table = []
         
         # 100 - Geology
         geology_items = [(100 + i, 'Geology', id, cost) for (i, (id, cost)) in enumerate(self.geology.costs.items())]
         for (id, feature, id_, cost) in geology_items:
-            conceptual_model = np.where(self.geology.data_volume == id_, id, conceptual_model)
+            conceptual_model = np.where(self.geology.data_volume == id_,
+                                        id,
+                                        conceptual_model)
         conceptual_model_table += geology_items
         
-        # 200 - Bedding - TODO
-        # if self.bedding is not None:
-        #     bedding_items += [(200 + i, 'Bedding', id, cost) for (i, (id, cost)) in enumerate(self.bedding.costs.items())]
-        
-        # 300 - Fractures
+        # 200 - Fractures
         if self.fractures is not None:
-            fractures_items = [(300 + i, 'Fractures', id, cost) for (i, (id, cost)) in enumerate(self.fractures.costs.items())]
+            fractures_items = [(200 + i, 'Fractures', id, cost) for (i, (id, cost)) in enumerate(self.fractures.costs.items())]
             for (id, feature, id_, cost) in fractures_items:
-                conceptual_model = np.where(self.fractures.data_volume == id_, id, conceptual_model)
+                conceptual_model = np.where(self.fractures.data_volume == id_,
+                                            id,
+                                            conceptual_model)
             conceptual_model_table += fractures_items
             
-        # 400 - Faults
+        # 300 - Faults
         if self.faults is not None:
-            faults_items = [(400 + i, 'Faults', id, cost) for (i, (id, cost)) in enumerate(self.faults.costs.items())]
+            faults_items = [(300 + i, 'Faults', id, cost) for (i, (id, cost)) in enumerate(self.faults.costs.items())]
             for (id, feature, id_, cost) in faults_items:
-                conceptual_model = np.where(self.faults.data_volume == id_, id, conceptual_model)
+                conceptual_model = np.where(self.faults.data_volume == id_,
+                                            id,
+                                            conceptual_model)
             conceptual_model_table += faults_items
-            
-        # 500 - Karst - TODO
-        # if self.karsts is not None:
-        #     items += [(500 + i, 'Faults', id, cost) for (i, (id, cost)) in enumerate(self.karsts.costs.items())]
         
         # 0 - Out
         out_item = [(0, 'Out', np.nan, self.SKS_SETTINGS['sks']['costs']['out'])]
-        conceptual_model = np.where(self.domain.data_volume == 0, 0, conceptual_model)
+        conceptual_model = np.where(self.domain.data_volume == 0,
+                                    0,
+                                    conceptual_model)
         conceptual_model_table += out_item
         conceptual_model_table = pd.DataFrame(conceptual_model_table, columns=['id', 'feature', 'id-feature', 'cost']).set_index('id').sort_values('id')
 
-        # 
         self.conceptual_model = conceptual_model
         self.conceptual_model_table = conceptual_model_table
         return None
     
     ##### 4 - FMM #########################
     @wp._debug_level(4)
     @wp._logging('fmm', 'construction')
     def _construct_fmm_variables(self) -> None:
         """Constructs the fast-marching method variables."""
-        self._initialize_fmm_iterations()  # Distributes inlets and outlets among karstic generations
-        self._construct_fmm_iterations()   # Distributes inlets and outlets among computing iterations
-        self._initialize_fmm_variables()   # Initializes useful variables for the farst-marching method
+        # Distributes inlets and outlets among karstic generations
+        self._initialize_fmm_iterations()
+        # Distributes inlets and outlets among computing iterations
+        self._construct_fmm_iterations()
+        # Initializes useful variables for the farst-marching method
+        self._initialize_fmm_variables()   
         return None
         
     def _initialize_fmm_iterations(self):
         # Defining some variables
         outlets_nbr = len(self.outlets)
         inlets_nbr = len(self.inlets)
         self.outlets_importance = self.SKS_SETTINGS['outlets']['importance']
@@ -862,16 +907,16 @@
         repartition = [round(proportion[i] * nbr_points) for i in range(len(proportion))]    # number of points to use this iteration (need to round bc percentage will not result in whole number)
         repartition[-1] = nbr_points - sum(repartition[0:-1])                                    # leftover points are assignd to last iteration
         return repartition
 
     def _initialize_fmm_variables(self):
         ### Raster maps
         self.maps = {
-            'outlets': np.full((self.grid.nx, self.grid.ny, self.grid.nz), np.nan),  # map of null values where each cell with an outlet will have the index of that outlet
-            'nodes': np.full((self.grid.nx, self.grid.ny, self.grid.nz), np.nan),  # map of null values where each cell that has a node will be updated with that node index
+            'outlets': np.full(self.grid.shape, np.nan),  # map of null values where each cell with an outlet will have the index of that outlet
+            'nodes': np.full(self.grid.shape, np.nan),  # map of null values where each cell that has a node will be updated with that node index
             'cost': [],   # cost of travel through each cell
             'alpha': [],  # cost of travel along gradient through each cell
             'beta': [],   # cost of travel perpendicular to gradient through each cell
             'time': [],   # travel time to outlet from each cell
             'karst': [],  # presence/absence of karst conduit in each cell
         }
         
@@ -906,36 +951,38 @@
             sides=[[self.grid.xmin, self.grid.xmax],                         # bottom edge,   top edge (NOT centerpoint)
                    [self.grid.ymin, self.grid.ymax],                            # leftmost edge, rightmost edge (NOT centerpoint)
                    [self.grid.zmin, self.grid.zmax]],
             dims=[self.grid.nx, self.grid.ny, self.grid.nz]                  # number of cells, number of cells, number of cells
         )
         return None
 
-
 ###############################################################################
 ### KARST NETWORK SIMULATION ###
 ################################
 
-    def compute_karst_network(self) -> None:
+    def compute(self) -> None:
         """
         Computes the karst network according to the parameters. Must be called
-        after ``build_model()`` method.
+        after ``build()`` method. This method will :
+        1. Computes conduits for each generation and stores nodes & edges for
+        network.
+        2. Stores all the relevant data for this network in specific
+        dictionaries.
+        3. Exports the state of the project, this file could be read by the
+        'analysis' and 'visualization' sub-packages.
 
         Examples
         --------
         >>> import pykasso as pk
         >>> simulation = pk.SKS()
-        >>> simulation.build_model()
-        >>> simulation.compute_karst_network
+        >>> simulation.build()
+        >>> simulation.compute()
         """
-        # Computes conduits for each generation & store nodes&edges for network
         self._compute_karst_network()
-        # Stores all the relevant data for this network in dictionaries
         self._export_results()
-        # Exports the state of the project, useful for the 'analysis' module
         self._export_project_state()
         return None
     
     def _compute_karst_network(self):
         this.logger = logging.getLogger("fmm.modelisation")
         this.logger.info("Computing karst network")
         
@@ -943,237 +990,328 @@
         
         for self.iteration in range(self.nbr_iteration):
         
             # Compute travel time maps and conduit network
             if self.fmm['algorithm'] == 'Isotropic3':
                 self._compute_cost_map()        # 2.1.1
                 self._compute_time_map()        # 2.1.2
-                self._compute_karst_map()       # 2.1.3
 
             elif self.fmm['algorithm'] == 'Riemann3':
-                # TODO - check notebooks mirebeau
-                self._compute_cost_map()        # 2.1.3
+                self._compute_cost_map()        # 2.1.1
                 self._compute_alpha_map()       # 2.1.4
                 self._compute_beta_map()        # 2.1.5
                 self._compute_riemann_metric()  # 2.1.6
                 self._compute_time_map()        # 2.1.7
-                self._compute_karst_map()       # 2.1.3
+            
+            self._compute_karst_map()
+            self._voxelize_karst_network()
 
             msg = "iteration : {}/{}".format(self.iteration + 1,
                                              self.nbr_iteration)
             this.logger.info(msg)
         return None
 
     ### 2.1.1 Iso- and anisotropic case
     @wp._debug_level(1, True)
     @wp._logging()
     def _compute_cost_map(self):
         """
-        Compute the cost map (how difficult it is to traverse each cell).
+        Computes the cost map (how difficult it is to traverse each cell).
 
         TODO
         """
-        # If it's the first iteration:
-        # iniatialize the cost map according to the conceptual model.
+        # During the first iteration, iniatializes the cost map according to
+        # the conceptual model.
         if self.iteration == 0:
             zeros_array = np.zeros((self.grid.nx, self.grid.ny, self.grid.nz))
             self.maps['cost'].append(zeros_array)
             for (i, row) in self.conceptual_model_table.iterrows():
                 logical_test = self.conceptual_model == row.name
                 self.maps['cost'][0] = np.where(logical_test,
                                                 row.cost,
                                                 self.maps['cost'][0])
                 
-        # If it's not the first iteration
+        # During the rest of the iterations
         else:
             self.maps['cost'].append(self.maps['cost'][self.iteration - 1])
             
             self.maps['cost'][self.iteration] = (
                 np.where(self.maps['karst'][self.iteration - 1] > 0,
                          self.SKS_SETTINGS['sks']['costs']['conduits'],
                          self.maps['cost'][self.iteration])
             )
             
         return None
     
     ### 2.1.4 Anisotropic case
     @wp._debug_level(2, True)
     @wp._logging()
-    def _compute_alpha_map(self):
+    def _compute_alpha_map(self) -> None:
         """
         Computes the alpha map: travel cost in the same direction as the
         gradient.
-        
-        Cost map * topography map, so that the cost is higher at higher
-        elevations, encouraging conduits to go downgradient.
-
-        TODO : à terminer
         """
+        alpha_map_0 = self.maps['cost'][self.iteration].copy()
         alpha_map = self.maps['cost'][self.iteration].copy()
         
-        if self.SKS_SETTINGS['sks']['modes']['elevation']:
-            alpha_map = self._set_alpha_from_elevation()
-        else:
-            pass  # TODO
-        
-        if self.domain.water_level is not None:
-            alpha_map = self._set_alpha_in_phreatic_zone(
-                self.maps['cost'][self.iteration],
-                alpha_map
+        ### Option A
+        if self.SKS_SETTINGS['sks']['mode'] == 'A':
+            # Vadose zone = Phreatic zone = Bedrock zone
+            domain = self.grid.data_volume
+            alpha_map = self._set_map_from_elevation(alpha_map, domain)
+            # Bedrock
+            if self.domain.bedrock is not None:
+                alpha_map = self._set_map_from_value(
+                    alpha_map,
+                    alpha_map.max(),
+                    self.domain.bedrock.data_volume)
+        
+        ### Option B
+        if self.SKS_SETTINGS['sks']['mode'] == 'B':
+            # Vadose zone = Bedrock zone
+            domain = self.domain.phreatic['vadose_zone']
+            alpha_map = self._set_map_from_elevation(alpha_map, domain)
+            # Bedrock
+            if self.domain.bedrock is not None:
+                alpha_map = self._set_map_from_value(
+                    alpha_map,
+                    alpha_map.max(),
+                    self.domain.bedrock.data_volume)
+            # Phreatic zone
+            alpha_map = self._set_map_from_value(
+                alpha_map,
+                alpha_map_0,
+                self.domain.phreatic['phreatic_zone'])
+            
+        ### Option C
+        if self.SKS_SETTINGS['sks']['mode'] == 'C':
+            # Vadose zone = Bedrock zone
+            factor = 100
+            alpha_map = self._set_map_from_value(
+                alpha_map,
+                alpha_map * factor,
+                self.domain.phreatic['vadose_zone'])
+            # Bedrock
+            if self.domain.bedrock is not None:
+                alpha_map = self._set_map_from_value(
+                    alpha_map,
+                    alpha_map.max() * 2,
+                    self.domain.bedrock.data_volume)
+            # Phreatic zone
+            if self.domain.water_level is not None:
+                alpha_map = self._set_map_from_value(
+                    alpha_map,
+                    alpha_map_0,
+                    self.domain.phreatic['phreatic_zone'])
+        
+        ### Option D
+        if self.SKS_SETTINGS['sks']['mode'] == 'D':
+            # Vadose zone
+            domain = np.logical_and(
+                np.logical_not(self.domain.bedrock_domains['bedrock_vadose']),
+                self.domain.phreatic['vadose_zone']
             )
+            factor_01 = 100
+            alpha_map = self._set_map_from_value(
+                alpha_map,
+                alpha_map * factor_01,
+                domain)
+            # Bedrock zone
+            factor_02 = 50
+            alpha_map = self._set_map_from_value(
+                alpha_map,
+                alpha_map * factor_02,
+                self.domain.bedrock_domains['bedrock_vadose'])
+            # Bedrock
+            if self.domain.bedrock is not None:
+                alpha_map = self._set_map_from_value(
+                    alpha_map,
+                    alpha_map.max() * 2,
+                    self.domain.bedrock.data_volume)
+            # Phreatic zone
+            alpha_map = self._set_map_from_value(
+                alpha_map,
+                alpha_map_0,
+                self.domain.phreatic['phreatic_zone'])
         
         self.maps['alpha'].append(alpha_map)
         return None
     
-    def _set_alpha_from_elevation(self):
+    def _set_map_from_elevation(self, array_map, domain) -> np.ndarray:
         """"""
         if (self.grid.nz == 1) and (self.domain.bedrock is not None):
-            out = (self.maps['cost'][self.iteration]
-                   * self.domain.bedrock.data_surface.reshape(self.grid.shape))
-            return out
+            bedrock = self.domain.bedrock.data_surface.reshape(self.grid.shape)
+            array_map = array_map * bedrock
+            return array_map
         else:
-            out = self.maps['cost'][self.iteration] * self.grid.Z
-            return out
-            
-    def _set_alpha_in_phreatic_zone(self, alpha, alpha_map):
-        """"""
-        out = np.where(self.domain.phreatic['phreatic_zone'] == 1,
-                       alpha,
-                       alpha_map)
-        return out
+            test = (domain == 1)
+            new_array_map = array_map * self.grid.Z
+            array_map = np.where(test, new_array_map, array_map)
+            return array_map
+    
+    def _set_map_from_value(self, array_map, value, domain) -> np.ndarray:
+        """ """
+        test = (domain == 1)
+        array_map = np.where(test, value, array_map)
+        return array_map
 
     ### 2.1.5 Anisotropic case
     @wp._debug_level(3, True)
     @wp._logging()
-    def _compute_beta_map(self):
+    def _compute_beta_map(self) -> None:
         """
         Computes the beta map: travel cost perpendicular to the gradient. If
         beta is higher than alpha, conduits will follow the steepest gradient.
         If beta is lower than alpha, conduits will follow contours.
         """
-        beta_map = (self.maps['alpha'][self.iteration]
-                    / self.SKS_SETTINGS['sks']['costs']['ratio'])
-        
-        if self.domain.water_level is not None:
-            beta_map = self._set_beta_in_phreatic_zone(
-                self.maps['alpha'][self.iteration],
-                beta_map
-            )
+        ratio = self.SKS_SETTINGS['sks']['costs']['ratio']
+        alpha_map_0 = self.maps['cost'][self.iteration].copy()
+        alpha_map = self.maps['alpha'][self.iteration].copy()
+        
+        ### Option A & default situation
+        # Vadose zone = Phreatic zone = Bedrock zone
+        beta_map = alpha_map / ratio
             
+        ### Options B / C / D
+        if self.SKS_SETTINGS['sks']['mode'] in ['B', 'C', 'D']:
+            # Phreatic zone
+            beta_map = self._set_map_from_value(
+                beta_map,
+                alpha_map_0,
+                self.domain.phreatic['phreatic_zone'])
+        
+        # beta_map[:, :, :] = 1
         self.maps['beta'].append(beta_map)
         return None
-    
-    def _set_beta_in_phreatic_zone(self, beta, beta_map):
-        """"""
-        out = np.where(self.domain.phreatic['phreatic_zone'] == 1,
-                       beta,
-                       beta_map)
-        return out
 
     ### 2.1.6 Anisotropic case
     @wp._debug_level(4, True)
     @wp._logging()
     def _compute_riemann_metric(self) -> None:
         """
         Compute the riemann metric: Define the Riemannian metric needed as
         input for the anisotropic fast marching.
 
         TODO : à terminer
         """
-        orientation_x, orientation_y, orientation_z = (
-            self._set_metrics_from_elevation_gradient()
-        )
+        ### Option A & default situation
+        grad_x = np.zeros_like(self.grid.data_volume)
+        grad_y = np.zeros_like(self.grid.data_volume)
+        grad_z = np.ones_like(self.grid.data_volume)
         
-        if self.domain.water_level is not None:
-            orientation_x, orientation_y, orientation_z = (
-                self._set_metrics_in_phreatic_zone(orientation_x,
-                                                   orientation_y,
-                                                   orientation_z)
-            )
-            
-        if self.SKS_SETTINGS['sks']['modes']['bedrock']:
+        ### Options B / C / D
+        if self.SKS_SETTINGS['sks']['mode'] in ['B', 'C', 'D']:
             if self.domain.bedrock is not None:
-                orientation_x, orientation_y, orientation_z = (
-                    self._set_metrics_on_bedrock_surface(orientation_x,
-                                                         orientation_y,
-                                                         orientation_z)
+                grad_x, grad_y, grad_z = (
+                    self._set_gradient_from_bedrock(grad_x,
+                                                    grad_y,
+                                                    grad_z)
                 )
-    
+        
+        # Sets the needle
         alpha = self.maps['alpha'][self.iteration]
         beta = self.maps['beta'][self.iteration]
-        # TODO
-        self.orientation = (orientation_x, orientation_y, orientation_z)
+        self.orientation = (grad_x, grad_y, grad_z)  # TODO - to remove ??
         self.fmm['riemannMetric'] = agd.Metrics.Riemann.needle(
-            [orientation_x, orientation_y, orientation_z],
+            [grad_x, grad_y, grad_z],
             alpha,
             beta
         )
         return None
     
-    def _set_metrics_from_elevation_gradient(self) -> tuple:
-        """"""
-        orientation_x = np.zeros_like(self.grid.data_volume)
-        orientation_y = np.zeros_like(self.grid.data_volume)
-        orientation_z = (np.ones_like(self.grid.data_volume)
-                         * np.abs(self.grid.dz))
-        out = (orientation_x, orientation_y, orientation_z)
-        return out
-    
-    def _set_metrics_in_phreatic_zone(self, orientation_x, orientation_y,
-                                      orientation_z) -> tuple:
+    def _set_gradient_from_bedrock(self, grad_x, grad_y, grad_z) -> None:
         """"""
-        orientation_x = np.where(self.domain.phreatic['phreatic_zone'] == 1,
-                                 1,
-                                 orientation_x)
-        orientation_y = np.where(self.domain.phreatic['phreatic_zone'] == 1,
-                                 1,
-                                 orientation_y)
-        orientation_z = np.where(self.domain.phreatic['phreatic_zone'] == 1,
-                                 1,
-                                 orientation_z)
-        out = (orientation_x, orientation_y, orientation_z)
-        return out
-    
-    def _set_metrics_on_bedrock_surface(self, orientation_x, orientation_y,
-                                        orientation_z) -> None:
-        """"""
-        if self.grid.nx == 1:
-            bedrock = np.roll(self.domain.bedrock.data_volume, 1, axis=2)
-            bedrock[:, :, 0] = 1
-            gradient_y, gradient_z = np.gradient(bedrock, self.grid.dy,
-                                                 self.grid.dz, axis=(1, 2))
-            gradient_x = np.full_like(gradient_y, 0)
-        elif self.grid.ny == 1:
-            bedrock = np.roll(self.domain.bedrock.data_volume, 1, axis=2)
-            bedrock[:, :, 0] = 1
-            gradient_x, gradient_z = np.gradient(bedrock, self.grid.dx,
-                                                 self.grid.dz, axis=(0, 2))
-            gradient_y = np.full_like(gradient_x, 0)
-        elif self.grid.nz == 1:
-            bedrock = self.domain.bedrock.data_surface
-            gradient_x, gradient_y = np.gradient(bedrock, self.grid.dx,
-                                                 self.grid.dy, axis=(0, 1))
-            gradient_x = gradient_x.reshape(self.grid.shape)
-            gradient_y = gradient_y.reshape(self.grid.shape)
-            gradient_z = np.full_like(gradient_x, 0)
-            bedrock = self.domain.bedrock.data_volume
+        test_grid_nx = (self.grid.nx == 1)
+        test_grid_ny = (self.grid.ny == 1)
+        test_grid_nz = (self.grid.nz == 1)
+        test_domain = (self.domain.bedrock_domains['bedrock_vadose'] == 1)
+        
+        if test_grid_nx or test_grid_ny or test_grid_nz:
+            if test_grid_nx:
+                bedrock = np.roll(self.domain.bedrock.data_volume, 1, axis=2)
+                bedrock[:, :, 0] = 1
+                gradient_y, gradient_z = np.gradient(bedrock, self.grid.dy,
+                                                     self.grid.dz, axis=(1, 2))
+                gradient_x = np.full_like(gradient_y, 0)
+            elif test_grid_ny:
+                bedrock = np.roll(self.domain.bedrock.data_volume, 1, axis=2)
+                bedrock[:, :, 0] = 1
+                gradient_x, gradient_z = np.gradient(bedrock, self.grid.dx,
+                                                     self.grid.dz, axis=(0, 2))
+                gradient_y = np.full_like(gradient_x, 0)
+            elif test_grid_nz:
+                bedrock = self.domain.bedrock.data_surface
+                gradient_x, gradient_y = np.gradient(bedrock, self.grid.dx,
+                                                     self.grid.dy, axis=(0, 1))
+                gradient_x = gradient_x.reshape(self.grid.shape)
+                gradient_y = gradient_y.reshape(self.grid.shape)
+                gradient_z = np.full_like(gradient_x, 0)
+                bedrock = self.domain.bedrock.data_volume
+            
+            grad_x = np.where(test_domain, gradient_x, grad_x)
+            grad_y = np.where(test_domain, gradient_y, grad_y)
+            grad_z = np.where(test_domain, gradient_z, grad_z)
+            
         else:
-            roll = 20
-            bedrock = np.roll(self.domain.bedrock.data_volume, roll, axis=2)
-            bedrock[:, :, :roll] = 1
-            # import pykasso.visualization as pkv
-            # pkv.show_array(bedrock)
-            gradient_x, gradient_y, gradient_z = (
-                np.gradient(bedrock, self.grid.dx, self.grid.dy, self.grid.dz)
-            )
+            # On commence par calculer le gradient en faisant gaffe à l'intervertion x y
+            bedrock = self.domain.bedrock.data_surface
+            gradient_x, gradient_y = np.gradient(bedrock,
+                                                 self.grid.dx,
+                                                 self.grid.dy)
+            
+            # Calcule du vecteur avec ses trois composantes (vx, vy, vz)
+
+            # On créé les matrices de composantes vx, vy, vz vides
+            vx = np.zeros(gradient_x.shape)
+            vy = np.zeros(gradient_x.shape)
+            vz = np.zeros(gradient_x.shape)
+            
+            # positions ou le gradient en x est non nul
+            idx_grad_x_not0 = (gradient_x != 0)
+            
+            # vx = +/- 1 dans la direction oposée au gradient
+            vx[idx_grad_x_not0] = - np.sign(gradient_x[idx_grad_x_not0])
+            
+            # Calcul de vy (pour respecter la direction horizontale)
+            vy[idx_grad_x_not0] = (vx[idx_grad_x_not0]
+                                   * gradient_y[idx_grad_x_not0]
+                                   / gradient_x[idx_grad_x_not0])
+
+            # On traite le cas particulier pour lequel gx = 0 et gy != 0
+            idx_gx_is0 = ((gradient_x == 0) & (gradient_y != 0))
+
+            # Dans ce cas la on normalise vy
+            vy[idx_gx_is0] = - np.sign(gradient_y[idx_gx_is0])
+
+            # Calcul de vz partout
+            vz = gradient_x * vx + gradient_y * vy
+
+            ### Dernier cas particulier problématique: la surface horizontale
+            # Chercher les occurences
+            idx_gxgy_are0 = ((gradient_x == 0) & (gradient_y == 0))
+
+            # Par convention
+            vx[idx_gxgy_are0] = 1
+            vy[idx_gxgy_are0] = 0
+            vz[idx_gxgy_are0] = 0
+
+            ### Finalement on normalise le vecteur
+            norm = np.sqrt(vx**2 + vy**2 + vz**2)
+            vx /= norm
+            vy /= norm
+            vz /= norm
+            
+            args = np.argwhere(test_domain)
+            i, j, k = zip(*args)
+
+            grad_x[i, j, k] = -vx[i, j]
+            grad_y[i, j, k] = -vy[i, j]
+            grad_z[i, j, k] = -vz[i, j]
         
-        orientation_x = np.where(bedrock == 1, gradient_x, orientation_x)
-        orientation_y = np.where(bedrock == 1, gradient_y, orientation_y)
-        orientation_z = np.where(bedrock == 1, gradient_z, orientation_z)
-        out = (orientation_x, orientation_y, orientation_z)
+        out = (grad_x, grad_y, grad_z)
         return out
 
     ### 2.1.2
     @wp._debug_level(5, True)
     @wp._logging()
     def _compute_time_map(self):
         """
@@ -1209,17 +1347,16 @@
             self.fmm['fastMarching']['cost'] = (
                 self.maps['cost'][self.iteration]
             )
         elif self.fmm['algorithm'] == 'Riemann3':
             self.fmm['fastMarching']['metric'] = self.fmm['riemannMetric']
 
         # Set verbosity of hfm run
-        self.fmm['fastMarching']['verbosity'] = (
-            self.SKS_SETTINGS['verbosity']['agd']
-        )
+        verbosity = self.SKS_SETTINGS['verbosity']['agd']
+        self.fmm['fastMarching']['verbosity'] = verbosity
 
         # Run the fast marching algorithm and store the outputs
         self.fmm['fastMarchingOutput'] = self.fmm['fastMarching'].Run()
 
         # Store travel time maps
         self.maps['time'].append(self.fmm['fastMarchingOutput']['values'])
 
@@ -1233,101 +1370,118 @@
     @wp._debug_level(6, True)
     @wp._logging()
     def _compute_karst_map(self):
         """
         Compute the karst map based on the paths from agd-hfm.
         Array of all zeros, with ones in cells containing a karst conduit.
         """
-        # Get karst map from previous iteration (except for the very first iteration)
-        if self.iteration == 0:
-            karst_map_0 = np.zeros((self.grid.nx, self.grid.ny, self.grid.nz))
-            self.maps['karst'].append(karst_map_0)
-        else:
-            self.maps['karst'].append(self.maps['karst'][self.iteration-1].copy())
-
-        # Debugging plot:
-        # Chloe: this should stay in since it is very useful if there are problems
-        # f1, ax1 = plt.subplots(1, 1, figsize=(10, 10))
-
         ### Loop over conduit paths generated by fast marching:
         for path in self.fmm['fastMarchingOutput']['geodesics']: #loop over conduit paths in this iteration (there is one path from each inlet)
             merge = False                                        #reset indicator for whether this conduit has merged with an existing conduit
             for p in range(path.shape[1]):                       #loop over points making up this conduit path
                 point = path[:,p]                                #get coordinates of current point
                 [[ix, iy, iz], error] = self.fmm['fastMarching'].IndexFromPoint(point) #convert to coordinates to indices, /!\ returning iy first then ix TODO ???
-                # ax1.scatter(point[1], point[0], c='g',s=5)  #debugging
                 #Place nodes and links:
                 if np.isnan(self.maps['nodes'][ix, iy, iz]):                                    #if there is no existing conduit node here
                     if ~np.isnan(self.maps['outlets'][ix, iy, iz]):                              #if there is an outlet here (cell value is not nan)
                         outlet = self._outlets.iloc[int(self.maps['outlets'][ix, iy, iz])]         #get the outlet coordinates using the ID in the outlets map
                         self.vectors['nodes'][self.vectors['n']] = [outlet.x, outlet.y, outlet.z, 'outfall']           #add a node at the outlet coordinates (with the node type for SWMM)
                         self.maps['nodes'][ix, iy, iz] = self.vectors['n']                                   #update node map with node index
-                        # ax1.scatter(outlet.x, outlet.y, marker='o', c='b')                   #debugging
                         if p > 0:                                                           #if this is not the first point (i.e. the inlet) in the current path
                             if merge == False:                                               #if this conduit has not merged with an existing conduit
                                 self.vectors['edges'][self.vectors['e']] = [self.vectors['n']-1, self.vectors['n']]                       #add an edge connecting the previous node to the current node
                                 self.vectors['e'] = self.vectors['e'] + 1                                             #increment edge counter up by one
-                                # ax1.plot((self.vectors['nodes'][self.vectors['n']][0], self.vectors['nodes'][self.vectors['n']-1][0]), (self.vectors['nodes'][self.vectors['n']][1], self.vectors['nodes'][self.vectors['n']-1][1]))
                             else:                                                          #if this conduit HAS merged with an existing conduit
                                 [[fromix, fromiy, fromiz], error] = self.fmm['fastMarching'].IndexFromPoint(path[:, p-1]) #get xyz indices of previous point in current conduit path
                                 n_from = self.maps['nodes'][fromix, fromiy, fromiz]           #get node index of the node already in the cell where the previous point was
                                 self.vectors['edges'][self.vectors['e']] = [n_from, self.vectors['n']]                         #add an edge connecting existing conduit node to current node
                                 self.vectors['e'] = self.vectors['e'] + 1                                             #increment edge counter up by one
-                                # ax1.plot((self.vectors['nodes'][self.vectors['n']].x, self.vectors['nodes'][n_from].x), (self.vectors['nodes'][self.vectors['n']].y, self.vectors['nodes'][n_from].y))
                         self.vectors['n'] = self.vectors['n'] + 1                                                   #increment node counter up by one
                     else:                                                                  #if there is NOT an outlet here
                         if p > 0:                                                           #if this is not the first point in the current path
                             #possible improvement: if the next point on the path is on an existing point, skip the current point.
                             self.vectors['nodes'][self.vectors['n']] = [point[0], point[1], point[2], 'junction']            #add a junction node here (with the node type for SWMM)
                             self.maps['nodes'][ix, iy, iz] = self.vectors['n']                               #update node map with node index
-                            #ax1.scatter(point[1],point[0], marker='o', edgecolor='g', facecolor='none')   #debugging
                             if merge == False:                                              #if this conduit has not merged with an existing conduit
                                 self.vectors['edges'][self.vectors['e']] = [self.vectors['n']-1, self.vectors['n']]                      #add and edge connecting the previous node to the current node
                                 self.vectors['e'] = self.vectors['e'] + 1                                            #increment edge counter up by one
-                                #ax1.plot((self.vectors['nodes'][self.vectors['n']][1], self.vectors['nodes'][self.vectors['n']-1][1]),(self.vectors['nodes'][self.vectors['n']][0], self.vectors['nodes'][self.vectors['n']-1][0]), c='gold', marker=None)
                             else:                                                           #if this conduit HAS merged with an existing conduit
                                 [[fromix, fromiy, fromiz], error] = self.fmm['fastMarching'].IndexFromPoint(path[:, p-1]) #get xy indices of previous point in current conduit path
                                 n_from = self.maps['nodes'][fromix, fromiy, fromiz]                   #get node index of the node already in the cell where the previous point was
                                 self.vectors['edges'][self.vectors['e']] = [n_from, self.vectors['n']]                        #add an edge connecting existing conduit node to current node
                                 self.vectors['e'] = self.vectors['e'] + 1                                            #increment edge counter up by one
                                 merge = False                                                #reset merge indicator to show that current conduit has left                                                              #if this is the first point in current path
                         else:                                                                #if this is the first point in the current path (counter <= 0, therefore it is an inlet)
                             self.vectors['nodes'][self.vectors['n']] = [point[0], point[1], point[2], 'inlet']               #add an inlet node here (with the node type for SWMM)
                             self.maps['nodes'][ix, iy, iz] = self.vectors['n']                               #update node map with node index
-                            #ax1.scatter(point[1],point[0], marker='o', edgecolor='sienna', facecolor='none')
                         self.vectors['n'] = self.vectors['n'] + 1                                                   #increment node counter up by one
                 elif ~np.isnan(self.maps['nodes'][ix, iy, iz]):                                 #if there is already a node in this cell (either because there is a conduit here, or because there are two nodes in the same cell)
                     n_existing = self.maps['nodes'][ix, iy, iz]                                  #get index of node already present in current cell
                     if merge == True:                                                       #if this conduit has already merged into an existing conduit
                         pass                                                                 #skip this node (there is already a node here)
                     elif n_existing == self.vectors['n']-1:                                            #if existing index is only one less than next node to be added index, this is a duplicate node and can be skipped
                         pass                                                                 #skip this node (duplicate)
                     else:                                                                   #if existing node index is >1 less than next node to be added index
                         if p > 0:                                                           #if this is not the first point in the current path
                             self.vectors['edges'][self.vectors['e']] = [self.vectors['n']-1, n_existing]                      #add an edge connecting most recently added node and existing node in cell
                             self.vectors['e'] = self.vectors['e'] + 1                                                #increment edge counter up by one
                             merge = True                                                     #add a flag indicating that this conduit has merged into an existing one
-                            #ax1.plot((self.vectors['nodes'][self.vectors['n']-1][1], self.vectors['nodes'][n_existing][1]),(self.vectors['nodes'][self.vectors['n']-1][0], self.vectors['nodes'][n_existing][0]), c='r', marker=None)
                         else:                                                                #if this is the first point in the current path (i.e. the inlet is on an exising conduit)
                             self.vectors['nodes'][self.vectors['n']] = [point[0], point[1], point[2], 'inlet']                #add a node here (with the node type for SWMM)- this will cause there to be two nodes in the same cell
                             self.maps['nodes'][ix, iy, iz] = self.vectors['n']                                #update node map with node index
                             self.vectors['n'] = self.vectors['n'] + 1                                                 #increment node counter by 1
-                            #ax1.scatter(point[1],point[0], marker='o', edgecolor='g', facecolor='none')  #debugging
-                self.maps['karst'][self.iteration][ix, iy, iz] = 1                               #update karst map to put a conduit in current cell
-                
+                # self.maps['karst'][self.iteration][ix, iy, iz] = 1                               #update karst map to put a conduit in current cell
+        return None
+    
+    def _voxelize_karst_network(self) -> None:
+        
+        # Gets karst map from previous iteration
+        # except for the very first iteration
+        if self.iteration == 0:
+            karst_map_0 = np.zeros(self.grid.shape)
+            self.maps['karst'].append(karst_map_0)
+        else:
+            karst_map_copy = self.maps['karst'][self.iteration - 1].copy()
+            self.maps['karst'].append(karst_map_copy)
 
-        ### Debugging plot
-        # # Display inlets and outlets
-        # ax1.scatter(self._outlets.x, self._outlets.y, c='cyan',   s=100)
-        # ax1.scatter(self._inlets.x,  self._inlets.y,  c='orange', s=100)
-        # ax1.scatter(self._outlets[self._outlets.iteration==iteration].x, self._outlets[self._outlets.iteration==iteration].y, c='cyan',   s=100)
-        # ax1.scatter(self._inlets[self._inlets.iteration==iteration].x,   self._inlets[self._inlets.iteration==iteration].y,   c='orange', s=100)
-        # # Display karst network
-        # ax1.imshow(np.transpose(self.maps['karst'][iteration], (1,0,2)), origin='lower', extent=self.grid.extent, cmap='gray_r')
-        # ax1.imshow(np.transpose(self.maps['nodes'], (1,0,2)), origin='lower', extent=self.grid.extent, cmap='gray_r')
+        # Cleans edges and nodes
+        edges = list(self.vectors['edges'].values())
+        nodes = {}
+        for i_node in self.vectors['nodes']:
+            nodes[i_node] = self.vectors['nodes'][i_node][:3]
+
+        # Retrieves the points
+        points = []
+        for (i1, i2) in edges:
+            point1 = nodes[i1]
+            point2 = nodes[i2]
+            x1, y1, z1 = point1
+            x2, y2, z2 = point2
+            x = x2 - x1
+            y = y2 - y1
+            z = z2 - z1
+            x3 = x1 + x / 2
+            y3 = y1 + y / 2
+            z3 = z1 + z / 2
+            points.extend([(x1, y1, z1)])
+            points.extend([(x2, y2, z2)])
+            points.extend([(x3, y3, z3)])
+
+        # Gets the indices
+        try:
+            x, y, z = zip(*points)
+            i, j, k = self.grid.get_indices(x, y, z)
+
+            # Calculates the new karst array
+            new_karst = np.zeros_like(self.grid.data_volume)
+            new_karst[i, j, k] = 1
+            self.maps['karst'][self.iteration] = new_karst
+        except:
+            pass
+        
         return None
     
     def _export_results(self):
         """
         TODO
         """
         path = self.CORE_SETTINGS['simulation_directory'] + 'results'
```

### Comparing `pykasso-0.1.2/pykasso/visualization/_pyvista.py` & `pykasso-0.1.3/pykasso/visualization/_pyvista.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,20 @@
         self._set_pyvista_grid()
 
     def _set_pyvista_grid(self) -> None:
         # Initialization
         x0, y0, z0 = self._get_grid_origin()
         nx, ny, nz = self._get_grid_dimensions()
         dx, dy, dz = self._get_grid_spacing()
-        grid = pv.UniformGrid()
+        pv_grid = pv.UniformGrid()
         # Constructs grid
-        grid.origin = (x0 - dx / 2, y0 - dy / 2, z0 - dz / 2)
-        grid.dimensions = np.array((nx, ny, nz)) + 1
-        grid.spacing = (dx, dy, dz)
-        self.grid = grid.cast_to_unstructured_grid()
+        pv_grid.origin = (x0 - dx / 2, y0 - dy / 2, z0 - dz / 2)
+        pv_grid.dimensions = np.array((nx, ny, nz)) + 1
+        pv_grid.spacing = (dx, dy, dz)
+        self.pv_grid = pv_grid.cast_to_unstructured_grid()
         return None
     
     def show(self, simulations: list, features: list,
              settings: list = [{}]) -> None:
         """
         TODO
         """
@@ -101,16 +101,16 @@
                 rows = 1
                 columns = len(simulations)
             else:
                 side = int(np.ceil(np.sqrt(len(simulations))))
                 rows = side
                 columns = side
         else:
-            rows = len(features)
-            columns = len(simulations)
+            rows = len(simulations)
+            columns = len(features)
         shape = (rows, columns)
         border = True
         plotter = pv.Plotter(shape=shape, border=border)
         
         # For each simulation, prints the required plots
         
         if len(features) == 1:
@@ -120,15 +120,17 @@
                     n_sim = simulations[i]
                     feature = features[0]
                     settings = pyvista_settings[i]
                     plotter.subplot(row, column)
                     plotter = self._fill_plotter(plotter, n_sim,
                                                  feature, settings)
         else:
-            for (row, (n_sim, settings)) in enumerate(zip(simulations, pyvista_settings)):
+            for (row, (n_sim, settings)) in enumerate(zip(simulations,
+                                                          pyvista_settings)
+                                                      ):
                 for (column, feature) in enumerate(features):
                     plotter.subplot(row, column)
                     plotter = self._fill_plotter(plotter, n_sim,
                                                  feature, settings)
                     
         plotter.link_views()
         plotter.show(cpos='xz')
@@ -177,22 +179,15 @@
         
         ### Generates the GIF
         path = plotter.generate_orbital_path(n_points=n_points,
                                              shift=mesh.length)
         plotter.open_gif(location, fps=fps)
         plotter.orbit_on_path(path, write_frames=True)
         plotter.close()
-        
         return None
-    
-    def _get_simulation_data(self, n: int) -> dict:
-        simulation_directory = self.project_state['simulation_locations'][n]
-        simulation_data_path = simulation_directory + 'results.pickle'
-        simulation_data = self._read_pickle(simulation_data_path)
-        return simulation_data
         
     def _show_feature(self, simulation, feature: str, settings: dict = {}):
         
         # Gets the data
         feature_data = self._get_data_from_feature(simulation, feature)
         feature_data_ = feature_data.copy()
         
@@ -209,15 +204,15 @@
         
         ### Creates the plot
         plotter = pv.Plotter()
         actors = []
         
         # Plots the outline of the domain
         if settings['outline']:
-            _ = plotter.add_mesh(self.grid.outline(), color="k")
+            _ = plotter.add_mesh(self.pv_grid.outline(), color="k")
             actors.append(_)
             
         # Plots the grid of the domain
         if settings['grid']:
             _ = plotter.show_grid()
             actors.append(_)
         
@@ -288,15 +283,15 @@
         _ = plotter.add_scalar_bar()
         actors.append(_)
 
         return actors
   
     def _get_data_from_feature(self, simulation, feature: str,
                                iteration: int = -1):
-        mesh = self.grid.copy()
+        mesh = self.pv_grid.copy()
         
         if feature in ANISOTROPIC_FEATURES:
             data = simulation['maps'][feature][iteration]
         elif feature in DOMAIN_FEATURES:
             feature_object = getattr(simulation['domain'], feature)
             data = getattr(feature_object, 'data_volume')
         else:
@@ -308,15 +303,15 @@
     
     def _get_ghosted_data(self, data, ghosts: list):
         ghosted_cells = np.argwhere(np.isin(data["data"], ghosts))
         data = data.remove_cells(ghosted_cells)
         return data
     
     def _get_surface(self, simulation, surface: str):
-        grid = simulation['grid']
+        grid = simulation['grid'] # TODO 
         x = grid.X[:, :, 0]
         y = grid.Y[:, :, 0]
         
         if surface == 'topography':
             z = simulation['domain'].topography.data_surface
         elif surface == 'water_level':
             z = simulation['domain'].water_level.data_surface
@@ -396,18 +391,14 @@
         #         grid = grid.remove_cells(ghosts)
 
         # return None
 
 
 
 
-
-
-
-
 # ##########################################################
 # ### DEBUG ###
 # #############
 
 # def _debug_plot_model(environment, settings):
 #     """
 #     TODO
@@ -520,8 +511,8 @@
 #     ### Plotting
 #     # p.add_title(feature)
 #     p.add_axes()
 #     bounds = p.show_bounds(mesh=vtk)
 #     p.add_actor(bounds)
 #     p.show(cpos='xy')
 
-#     return None
+#     return None
```

### Comparing `pykasso-0.1.2/pykasso/visualization/main.py` & `pykasso-0.1.3/pykasso/visualization/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """
 This module contains ...
 """
 
-# TODO - automatic update when visualization class is already created
-
 ### Internal dependencies
 import sys
 import importlib
 
 ### External dependencies
 import yaml
 import numpy as np
@@ -18,15 +16,14 @@
 ### Module variables
 this = sys.modules[__name__]
 
 GEOLOGICAL_FEATURES = [
     'grid',
     'domain',
     'geology',
-    # 'beddings'
     'faults',
     'fractures',
 ]
 
 SURFACES_FEATURES = [
     'topography',
     'bedrock',
@@ -70,15 +67,14 @@
     TODO
     """
     # ajouter __method__ pour dire qu'elle existe pas
     # si yapa pyvista d'installé
     
     def __init__(self, project_directory: str, notebook: bool = True,
                  *args, **kwargs) -> None:
-        """"""
         super().__init__(project_directory, *args, **kwargs)
         
     def _is_feature_name_valid(self, feature) -> bool:
         """
         TODO
         """
         if feature not in AUTHORIZED_FEATURES:
```

### Comparing `pykasso-0.1.2/pyproject.toml` & `pykasso-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykasso"
-version = "0.1.2"
+version = "0.1.3"
 description = "Python project intended to simulate stochastic karst network"
 license = "GPL-3.0"
 authors = [
     "François Miville <francois@miville.org>",
     "Chloé Fandel",
     "Philippe Renard"
 ]
@@ -26,34 +26,35 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.22.0"
 pandas = "^1.5.2"
 matplotlib = "^3.6.2"
+pyqt5 = "^5.15.9"
 openpyxl = "^3.0.10"
 mpmath = "^1.2.1"
 pyyaml = "^6.0"
 agd = "^0.1.31"
 scipy = "^1.9.3"
 plotly = "^5.13.1"
+shapely = "^2.0.1"
 networkx = {version = "^3.0", optional = true}
 mplstereonet = {version = "^0.6.2", optional = true}
 pyvista = {version = "^0.37.0", optional = true}
 imageio = {version = "^2.26.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.19.4"
 jupyter = "^1.0.0"
 jupyterlab = "^3.5.2"
 ipyvtklink = "^0.2.3"
 snakeviz = "^2.1.1"
 sphinx = "^6.1.3"
 numpydoc = "^1.5.0"
-pytest = "^7.2.2"
 
 [tool.poetry.extras]
 analysis = ["karstnet", "networkx", "mplstereonet"]
 visualization = ["pyvista","imageio"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pykasso-0.1.2/README.md` & `pykasso-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,28 +30,31 @@
 ```
 
 Then:
 ```
 pip install -e pykasso[analysis, visualization]
 ```
 
+<!-- 
 ### Check installation
 
 Work in progress.
 
-<!-- ```
+```
 poetry run pytest tests/
-``` -->
+```
+
 
 ### Dependencies
 
 pyKasso requires the following python packages to function properly:
 - [agd](https://github.com/Mirebeau/AdaptiveGridDiscretizations)
 - [karstnet](https://github.com/UniNE-CHYN/karstnet)
 - [pyvista](https://github.com/pyvista/pyvista)
+-->
 
 ## Documentation
 
 Work in progress.
 
 ## Examples
```

### Comparing `pykasso-0.1.2/setup.py` & `pykasso-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 ['agd>=0.1.31,<0.2.0',
  'matplotlib>=3.6.2,<4.0.0',
  'mpmath>=1.2.1,<2.0.0',
  'numpy>=1.22.0,<2.0.0',
  'openpyxl>=3.0.10,<4.0.0',
  'pandas>=1.5.2,<2.0.0',
  'plotly>=5.13.1,<6.0.0',
+ 'pyqt5>=5.15.9,<6.0.0',
  'pyyaml>=6.0,<7.0',
- 'scipy>=1.9.3,<2.0.0']
+ 'scipy>=1.9.3,<2.0.0',
+ 'shapely>=2.0.1,<3.0.0']
 
 extras_require = \
 {'analysis': ['networkx>=3.0,<4.0', 'mplstereonet>=0.6.2,<0.7.0'],
  'visualization': ['pyvista>=0.37.0,<0.38.0', 'imageio>=2.26.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'pykasso',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Python project intended to simulate stochastic karst network',
-    'long_description': "![pyKasso's banner](/docs/source/_static/pykasso_banner_logo.png)\n\n<!-- ![]() -->\n[![PyPI Version](https://img.shields.io/pypi/v/pykasso.png)](https://pypi.python.org/pypi/pykasso)\n[![PyPI Status](https://img.shields.io/pypi/status/pykasso.png)](https://pypi.python.org/pypi/pykasso)\n[![PyPI Versions](https://img.shields.io/pypi/pyversions/pykasso.png)](https://pypi.python.org/pypi/pykasso)\n\n![license](https://img.shields.io/github/license/randlab/pyKasso)\n![last-commit](https://img.shields.io/github/last-commit/randlab/pyKasso/dev)\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/randlab/pyKasso/dev)\n\n## pyKasso: a stochastic karst network simulation tool\n<!-- ![pyKasso's logo](/docs/source/_static/pykasso_logo.png) -->\n\npyKasso is a python3 open-source package intended to simulate easily and quickly karst networks using a geological model, hydrogeological, and structural data. It relies on a pseudo-genetic methodology where stochastic data and fast-marching methods are combined to perform thousands of simulations rapidly. The method is based on the stochastic karst simulator developed by Borghi et al (2012). It has been extended to account for anisotropy allowing to simplify the algorithm while accounting better for the geological structure following the method presented in Fandel et al. (2022). Statistical geometrical and topological metrics are computed on the simulated networks and compared with the same statistics computed on real karst network to evaluate the plausibility of the simulations.\n\n![gif_01](/docs/source/_static/animation_01.gif)\n![gif_02](/docs/source/_static/animation_02.gif)\n\n## Installation\n\nCurrently, pyKasso is only working with Python 3.9.\n\n### Using conda\n\nDownload *environment.yml*. From source:\n```\nconda env create --name pykasso --file=environment.yml\n```\n\nThen:\n```\npip install -e pykasso[analysis, visualization]\n```\n\n### Check installation\n\nWork in progress.\n\n<!-- ```\npoetry run pytest tests/\n``` -->\n\n### Dependencies\n\npyKasso requires the following python packages to function properly:\n- [agd](https://github.com/Mirebeau/AdaptiveGridDiscretizations)\n- [karstnet](https://github.com/UniNE-CHYN/karstnet)\n- [pyvista](https://github.com/pyvista/pyvista)\n\n## Documentation\n\nWork in progress.\n\n## Examples\n\nSome basic examples are avaible here : [notebooks/geometry/](https://github.com/randlab/pyKasso/tree/dev/notebooks/geometry)\n\n## Contact\n\n- F. Miville\n- Prof. C. Fandel\n- Prof. P. Renard\n\n## Publications\n\n- Fandel, C., Miville, F., Ferré, T. et al. 2022: The stochastic simulation of karst conduit network structure using anisotropic fast marching, and its application to a geologically complex alpine karst system. Hydrogeol J 30, 927–946, https://doi.org/10.1007/s10040-022-02464-x\n- Borghi, A., Renard, P., Jenni, S. 2012: A pseudo-genetic stochastic model to generate karstic networks, Journal of Hydrology, 414–415, https://doi.org/10.1016/j.jhydrol.2011.11.032.",
+    'long_description': "![pyKasso's banner](/docs/source/_static/pykasso_banner_logo.png)\n\n<!-- ![]() -->\n[![PyPI Version](https://img.shields.io/pypi/v/pykasso.png)](https://pypi.python.org/pypi/pykasso)\n[![PyPI Status](https://img.shields.io/pypi/status/pykasso.png)](https://pypi.python.org/pypi/pykasso)\n[![PyPI Versions](https://img.shields.io/pypi/pyversions/pykasso.png)](https://pypi.python.org/pypi/pykasso)\n\n![license](https://img.shields.io/github/license/randlab/pyKasso)\n![last-commit](https://img.shields.io/github/last-commit/randlab/pyKasso/dev)\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/randlab/pyKasso/dev)\n\n## pyKasso: a stochastic karst network simulation tool\n<!-- ![pyKasso's logo](/docs/source/_static/pykasso_logo.png) -->\n\npyKasso is a python3 open-source package intended to simulate easily and quickly karst networks using a geological model, hydrogeological, and structural data. It relies on a pseudo-genetic methodology where stochastic data and fast-marching methods are combined to perform thousands of simulations rapidly. The method is based on the stochastic karst simulator developed by Borghi et al (2012). It has been extended to account for anisotropy allowing to simplify the algorithm while accounting better for the geological structure following the method presented in Fandel et al. (2022). Statistical geometrical and topological metrics are computed on the simulated networks and compared with the same statistics computed on real karst network to evaluate the plausibility of the simulations.\n\n![gif_01](/docs/source/_static/animation_01.gif)\n![gif_02](/docs/source/_static/animation_02.gif)\n\n## Installation\n\nCurrently, pyKasso is only working with Python 3.9.\n\n### Using conda\n\nDownload *environment.yml*. From source:\n```\nconda env create --name pykasso --file=environment.yml\n```\n\nThen:\n```\npip install -e pykasso[analysis, visualization]\n```\n\n<!-- \n### Check installation\n\nWork in progress.\n\n```\npoetry run pytest tests/\n```\n\n\n### Dependencies\n\npyKasso requires the following python packages to function properly:\n- [agd](https://github.com/Mirebeau/AdaptiveGridDiscretizations)\n- [karstnet](https://github.com/UniNE-CHYN/karstnet)\n- [pyvista](https://github.com/pyvista/pyvista)\n-->\n\n## Documentation\n\nWork in progress.\n\n## Examples\n\nSome basic examples are avaible here : [notebooks/geometry/](https://github.com/randlab/pyKasso/tree/dev/notebooks/geometry)\n\n## Contact\n\n- F. Miville\n- Prof. C. Fandel\n- Prof. P. Renard\n\n## Publications\n\n- Fandel, C., Miville, F., Ferré, T. et al. 2022: The stochastic simulation of karst conduit network structure using anisotropic fast marching, and its application to a geologically complex alpine karst system. Hydrogeol J 30, 927–946, https://doi.org/10.1007/s10040-022-02464-x\n- Borghi, A., Renard, P., Jenni, S. 2012: A pseudo-genetic stochastic model to generate karstic networks, Journal of Hydrology, 414–415, https://doi.org/10.1016/j.jhydrol.2011.11.032.",
     'author': 'François Miville',
     'author_email': 'francois@miville.org',
     'maintainer': 'François Miville',
     'maintainer_email': 'francois@miville.org',
     'url': 'https://github.com/randlab/pyKasso',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pykasso-0.1.2/PKG-INFO` & `pykasso-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykasso
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python project intended to simulate stochastic karst network
 Home-page: https://github.com/randlab/pyKasso
 License: GPL-3.0
 Keywords: hydrogeology,3-D modeling,stochasticity
 Author: François Miville
 Author-email: francois@miville.org
 Maintainer: François Miville
@@ -28,17 +28,19 @@
 Requires-Dist: mplstereonet (>=0.6.2,<0.7.0) ; extra == "analysis"
 Requires-Dist: mpmath (>=1.2.1,<2.0.0)
 Requires-Dist: networkx (>=3.0,<4.0) ; extra == "analysis"
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: plotly (>=5.13.1,<6.0.0)
+Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: pyvista (>=0.37.0,<0.38.0) ; extra == "visualization"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/randlab/pyKasso
 Description-Content-Type: text/markdown
 
 ![pyKasso's banner](/docs/source/_static/pykasso_banner_logo.png)
 
 <!-- ![]() -->
 [![PyPI Version](https://img.shields.io/pypi/v/pykasso.png)](https://pypi.python.org/pypi/pykasso)
@@ -70,28 +72,31 @@
 ```
 
 Then:
 ```
 pip install -e pykasso[analysis, visualization]
 ```
 
+<!-- 
 ### Check installation
 
 Work in progress.
 
-<!-- ```
+```
 poetry run pytest tests/
-``` -->
+```
+
 
 ### Dependencies
 
 pyKasso requires the following python packages to function properly:
 - [agd](https://github.com/Mirebeau/AdaptiveGridDiscretizations)
 - [karstnet](https://github.com/UniNE-CHYN/karstnet)
 - [pyvista](https://github.com/pyvista/pyvista)
+-->
 
 ## Documentation
 
 Work in progress.
 
 ## Examples
```

