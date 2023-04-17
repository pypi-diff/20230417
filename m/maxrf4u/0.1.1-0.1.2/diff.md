# Comparing `tmp/maxrf4u-0.1.1.tar.gz` & `tmp/maxrf4u-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/maxrf4u-0.1.1.tar", last modified: Wed Mar 22 10:50:16 2023, max compression
+gzip compressed data, was "dist/maxrf4u-0.1.2.tar", last modified: Mon Apr 17 20:07:10 2023, max compression
```

## Comparing `maxrf4u-0.1.1.tar` & `maxrf4u-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/
--rw-rw-r--   0 frank     (1000) frank     (1000)    35149 2022-02-01 10:31:49.000000 maxrf4u-0.1.1/LICENSE
--rw-rw-r--   0 frank     (1000) frank     (1000)      111 2021-02-17 00:39:42.000000 maxrf4u-0.1.1/MANIFEST.in
--rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/PKG-INFO
--rw-rw-r--   0 frank     (1000) frank     (1000)      916 2023-03-22 10:41:52.000000 maxrf4u-0.1.1/README.md
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u/
--rw-rw-r--   0 frank     (1000) frank     (1000)      328 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/__init__.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    11754 2023-03-22 10:49:59.000000 maxrf4u-0.1.1/maxrf4u/_modidx.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     2821 2023-02-08 12:52:01.000000 maxrf4u-0.1.1/maxrf4u/_nbdev.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      171 2022-08-11 10:43:22.000000 maxrf4u-0.1.1/maxrf4u/absorption.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     7929 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/calibration.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      119 2022-09-23 13:00:31.000000 maxrf4u-0.1.1/maxrf4u/fingerprints.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    16777 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/hotmax.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     6169 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/interactive_visualization.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      127 2022-10-07 13:48:18.000000 maxrf4u-0.1.1/maxrf4u/iplotting.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      133 2023-02-08 12:52:01.000000 maxrf4u-0.1.1/maxrf4u/peak_pattern_puzzle_solver.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    13129 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/peakmaps.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    12229 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/peakpuzzle.py
--rw-rw-r--   0 frank     (1000) frank     (1000)      115 2022-09-23 13:00:31.000000 maxrf4u-0.1.1/maxrf4u/speckles.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    11818 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/storage.py
--rw-rw-r--   0 frank     (1000) frank     (1000)    10026 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/warp.py
--rw-rw-r--   0 frank     (1000) frank     (1000)     4131 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/maxrf4u/xphysics.py
-drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u.egg-info/
--rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u.egg-info/PKG-INFO
--rw-rw-r--   0 frank     (1000) frank     (1000)      626 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u.egg-info/SOURCES.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        1 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u.egg-info/dependency_links.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)       57 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u.egg-info/entry_points.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        1 2022-02-01 23:46:37.000000 maxrf4u-0.1.1/maxrf4u.egg-info/not-zip-safe
--rw-rw-r--   0 frank     (1000) frank     (1000)      170 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u.egg-info/requires.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)        8 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/maxrf4u.egg-info/top_level.txt
--rw-rw-r--   0 frank     (1000) frank     (1000)      958 2023-03-22 10:49:58.000000 maxrf4u-0.1.1/settings.ini
--rw-rw-r--   0 frank     (1000) frank     (1000)       38 2023-03-22 10:50:16.000000 maxrf4u-0.1.1/setup.cfg
--rw-rw-r--   0 frank     (1000) frank     (1000)     2560 2023-01-20 02:50:04.000000 maxrf4u-0.1.1/setup.py
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/
+-rw-rw-r--   0 frank     (1000) frank     (1000)    35149 2022-02-01 10:31:49.000000 maxrf4u-0.1.2/LICENSE
+-rw-rw-r--   0 frank     (1000) frank     (1000)      111 2021-02-17 00:39:42.000000 maxrf4u-0.1.2/MANIFEST.in
+-rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/PKG-INFO
+-rw-rw-r--   0 frank     (1000) frank     (1000)      916 2023-03-22 10:41:52.000000 maxrf4u-0.1.2/README.md
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u/
+-rw-rw-r--   0 frank     (1000) frank     (1000)      328 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/__init__.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    11890 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/_modidx.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     2821 2023-02-08 12:52:01.000000 maxrf4u-0.1.2/maxrf4u/_nbdev.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      171 2022-08-11 10:43:22.000000 maxrf4u-0.1.2/maxrf4u/absorption.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     7929 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/calibration.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      119 2022-09-23 13:00:31.000000 maxrf4u-0.1.2/maxrf4u/fingerprints.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    16909 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/hotmax.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     6169 2023-03-22 15:38:39.000000 maxrf4u-0.1.2/maxrf4u/interactive_visualization.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      127 2022-10-07 13:48:18.000000 maxrf4u-0.1.2/maxrf4u/iplotting.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      133 2023-02-08 12:52:01.000000 maxrf4u-0.1.2/maxrf4u/peak_pattern_puzzle_solver.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    13069 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/peakmaps.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    12230 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/peakpuzzle.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)      115 2022-09-23 13:00:31.000000 maxrf4u-0.1.2/maxrf4u/speckles.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    11818 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/storage.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)    10026 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/warp.py
+-rw-rw-r--   0 frank     (1000) frank     (1000)     4131 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/maxrf4u/xphysics.py
+drwxrwxr-x   0 frank     (1000) frank     (1000)        0 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/
+-rw-rw-r--   0 frank     (1000) frank     (1000)     1885 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/PKG-INFO
+-rw-rw-r--   0 frank     (1000) frank     (1000)      626 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/SOURCES.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)        1 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/dependency_links.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)       57 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/entry_points.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)        1 2022-02-01 23:46:37.000000 maxrf4u-0.1.2/maxrf4u.egg-info/not-zip-safe
+-rw-rw-r--   0 frank     (1000) frank     (1000)      170 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/requires.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)        8 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/maxrf4u.egg-info/top_level.txt
+-rw-rw-r--   0 frank     (1000) frank     (1000)      958 2023-04-17 20:06:54.000000 maxrf4u-0.1.2/settings.ini
+-rw-rw-r--   0 frank     (1000) frank     (1000)       38 2023-04-17 20:07:10.000000 maxrf4u-0.1.2/setup.cfg
+-rw-rw-r--   0 frank     (1000) frank     (1000)     2560 2023-01-20 02:50:04.000000 maxrf4u-0.1.2/setup.py
```

### Comparing `maxrf4u-0.1.1/LICENSE` & `maxrf4u-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/PKG-INFO` & `maxrf4u-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxrf4u
-Version: 0.1.1
+Version: 0.1.2
 Summary: Explore your X-Ray Fluorescence spectral images
 Home-page: https://github.com/fligt/maxrf4u
 Author: Frank Ligterink
 Author-email: frank.ligterink@gmail.com
 License: GNU General Public License v3
 Description: # Welcome to maxrf4u
```

### Comparing `maxrf4u-0.1.1/README.md` & `maxrf4u-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/maxrf4u/_modidx.py` & `maxrf4u-0.1.2/maxrf4u/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
                                 'maxrf4u.hotmax.HotmaxAtlas.plot_spectra': ('hotmax.html#hotmaxatlas.plot_spectra', 'maxrf4u/hotmax.py'),
                                 'maxrf4u.hotmax.HotmaxAtlas.plot_spectrum': ('hotmax.html#hotmaxatlas.plot_spectrum', 'maxrf4u/hotmax.py'),
                                 'maxrf4u.hotmax._baseline': ('hotmax.html#_baseline', 'maxrf4u/hotmax.py'),
                                 'maxrf4u.hotmax._group_superimposed': ('hotmax.html#_group_superimposed', 'maxrf4u/hotmax.py'),
                                 'maxrf4u.hotmax._noiseline': ('hotmax.html#_noiseline', 'maxrf4u/hotmax.py'),
                                 'maxrf4u.hotmax._untilt': ('hotmax.html#_untilt', 'maxrf4u/hotmax.py'),
                                 'maxrf4u.hotmax.compute_hotmax_noise': ('hotmax.html#compute_hotmax_noise', 'maxrf4u/hotmax.py'),
-                                'maxrf4u.hotmax.compute_hotmax_spectra': ('hotmax.html#compute_hotmax_spectra', 'maxrf4u/hotmax.py')},
+                                'maxrf4u.hotmax.compute_hotmax_spectra': ('hotmax.html#compute_hotmax_spectra', 'maxrf4u/hotmax.py'),
+                                'maxrf4u.hotmax.compute_subpeaks': ('hotmax.html#compute_subpeaks', 'maxrf4u/hotmax.py')},
             'maxrf4u.interactive_visualization': { 'maxrf4u.interactive_visualization.UploadDir': ( 'interactive-plotting.html#uploaddir',
                                                                                                     'maxrf4u/interactive_visualization.py'),
                                                    'maxrf4u.interactive_visualization.UploadDir.__init__': ( 'interactive-plotting.html#uploaddir.__init__',
                                                                                                              'maxrf4u/interactive_visualization.py'),
                                                    'maxrf4u.interactive_visualization.UploadDir.export_interactive_html': ( 'interactive-plotting.html#uploaddir.export_interactive_html',
                                                                                                                             'maxrf4u/interactive_visualization.py'),
                                                    'maxrf4u.interactive_visualization.UploadDir.imsave': ( 'interactive-plotting.html#uploaddir.imsave',
@@ -40,21 +41,21 @@
                                                                                                               'maxrf4u/interactive_visualization.py')},
             'maxrf4u.iplotting': {},
             'maxrf4u.peak_pattern_puzzle_solver': {},
             'maxrf4u.peakmaps': { 'maxrf4u.peakmaps._add_hotlines_ticklabels': ( 'peakmaps.html#_add_hotlines_ticklabels',
                                                                                  'maxrf4u/peakmaps.py'),
                                   'maxrf4u.peakmaps._fit_gaussian': ('peakmaps.html#_fit_gaussian', 'maxrf4u/peakmaps.py'),
                                   'maxrf4u.peakmaps._gaussian': ('peakmaps.html#_gaussian', 'maxrf4u/peakmaps.py'),
+                                  'maxrf4u.peakmaps._get_spectral_slices': ('peakmaps.html#_get_spectral_slices', 'maxrf4u/peakmaps.py'),
                                   'maxrf4u.peakmaps.compute_nmf_element_maps': ( 'peakmaps.html#compute_nmf_element_maps',
                                                                                  'maxrf4u/peakmaps.py'),
                                   'maxrf4u.peakmaps.compute_nmf_peakmaps': ('peakmaps.html#compute_nmf_peakmaps', 'maxrf4u/peakmaps.py'),
-                                  'maxrf4u.peakmaps.fit_spectrum': ('peakmaps.html#fit_spectrum', 'maxrf4u/peakmaps.py'),
+                                  'maxrf4u.peakmaps.fit_spectrum_peaks': ('peakmaps.html#fit_spectrum_peaks', 'maxrf4u/peakmaps.py'),
                                   'maxrf4u.peakmaps.get_continuum': ('peakmaps.html#get_continuum', 'maxrf4u/peakmaps.py'),
                                   'maxrf4u.peakmaps.get_gaussians': ('peakmaps.html#get_gaussians', 'maxrf4u/peakmaps.py'),
-                                  'maxrf4u.peakmaps.get_spectral_slices': ('peakmaps.html#get_spectral_slices', 'maxrf4u/peakmaps.py'),
                                   'maxrf4u.peakmaps.multi_plot': ('peakmaps.html#multi_plot', 'maxrf4u/peakmaps.py')},
             'maxrf4u.peakpuzzle': { 'maxrf4u.peakpuzzle.add_hotlines': ('peak-pattern-puzzle.html#add_hotlines', 'maxrf4u/peakpuzzle.py'),
                                     'maxrf4u.peakpuzzle.colorize': ('peak-pattern-puzzle.html#colorize', 'maxrf4u/peakpuzzle.py'),
                                     'maxrf4u.peakpuzzle.get_instrument_pattern': ( 'peak-pattern-puzzle.html#get_instrument_pattern',
                                                                                    'maxrf4u/peakpuzzle.py'),
                                     'maxrf4u.peakpuzzle.get_patterns': ('peak-pattern-puzzle.html#get_patterns', 'maxrf4u/peakpuzzle.py'),
                                     'maxrf4u.peakpuzzle.plot_patterns': ('peak-pattern-puzzle.html#plot_patterns', 'maxrf4u/peakpuzzle.py'),
```

### Comparing `maxrf4u-0.1.1/maxrf4u/_nbdev.py` & `maxrf4u-0.1.2/maxrf4u/_nbdev.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/maxrf4u/calibration.py` & `maxrf4u-0.1.2/maxrf4u/calibration.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/maxrf4u/hotmax.py` & `maxrf4u-0.1.2/maxrf4u/hotmax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,48 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../notebooks/40_hotmax.ipynb.
 
 # %% auto 0
-__all__ = ['HotmaxAtlas', 'compute_hotmax_spectra', 'compute_hotmax_noise']
+__all__ = ['HotmaxAtlas', 'compute_hotmax_spectra', 'compute_hotmax_noise', 'compute_subpeaks']
 
-# %% ../notebooks/40_hotmax.ipynb 29
+# %% ../notebooks/40_hotmax.ipynb 32
 import maxrf4u 
 import scipy.signal as ssg 
 import numpy as np 
 import time 
 import matplotlib.pyplot as plt 
 from dask.diagnostics import ProgressBar 
 import scipy.ndimage.morphology as morph 
 import scipy.interpolate as sip 
 from IPython.display import SVG 
 
-# %% ../notebooks/40_hotmax.ipynb 30
+# %% ../notebooks/40_hotmax.ipynb 33
 class HotmaxAtlas(): 
     
     def __init__(self, datastack_file, prominence=0.2): 
         
-        # read from datastack file 
+        # read from datastack file (arrays)
         
         ds = maxrf4u.DataStack(datastack_file)
         
         self.x_keVs = ds.read('maxrf_energies') 
         self.y_max = ds.read('maxrf_maxspectrum') 
-        
         self.hotmax_pixels = ds.read('hotmax_pixels')
-        self.hotmax_spectra = ds.read('hotmax_spectra') 
-        self.submax_spectrum = np.max(self.hotmax_spectra, axis=0) # max spectrum skeleton 
+        self.hotmax_spectra = ds.read('hotmax_spectra')
         self.baselines = ds.read('hotmax_baselines')
-        self.noiselines = ds.read('hotmax_noiselines')
-        self.hotmax_mask = ds.read('hotmax_mask')
+        self.noiselines = ds.read('hotmax_noiselines') 
         
         self.n_spectra = len(self.hotmax_spectra) 
+        self.submax_spectrum = np.max(self.hotmax_spectra, axis=0) # core max spectrum
         
-        # find subpeaks and initialize labels 
-        
-        self.peak_idxs_list = []
-        self.peak_labels_list = []
-        
-        for i, y_hot in enumerate(self.hotmax_spectra): 
-            
-            above_noise = y_hot - self.noiselines[i] 
-            above_noise[y_hot < self.noiselines[i]] = 0 
-            peak_idxs, _ = ssg.find_peaks(above_noise, prominence=prominence) 
-        
-            peak_heights = above_noise[peak_idxs]
-            peak_order = np.argsort(peak_heights)[::-1] # sort by peak height
-            peak_idxs = peak_idxs[peak_order] 
-            
-            # hack to correct peak positions due to baseline tilting 
-            peak_idxs = _untilt(peak_idxs, y_hot, delta=5) 
-            
-            # NOT NECESSARY AND POSSIBLE WITH MULTIPLE HOTMAX PEAKS 
-            # INSTEAD USING MASK 
-            # promote hotmax peak to first position in list   
-            #hotmax_i = self.hotmax_pixels[i, 2] # get channel index  
-            #peak_idxs.remove(hotmax_i) # remove from list
-            #peak_idxs.insert(0, hotmax_i) # prepend  
-        
-            self.peak_idxs_list.append(peak_idxs) 
-            
-            peak_labels = [f'[{i}]' for i in range(len(peak_idxs))]
-            self.peak_labels_list.append(peak_labels)
-            
-        
-        # collect all lines in atlas in single list 
-        
-        self.all_peaks = []
-        for peak_idxs in self.peak_idxs_list: 
-            for i in peak_idxs: 
-                self.all_peaks.append(i)
-
-        self.all_peaks_set = np.sort(list(set(self.all_peaks))) 
-        
-        # add a list with hotslice indices 
-        # (hack because we reorder peaks in hotmax spectrum according to height) 
-        
-        # NO LONGER POSSIBLE NOR NEEDED
-        #keV_idxs = self.hotmax_pixels[:,2]  
-    
-        #self.hotslice_idxs = []
-    
-        #for n, peak_idxs in enumerate(self.peak_idxs_list): 
-
-        #     self.hotslice_idxs.append(peak_idxs.index(keV_idxs[n])) 
-    
-        
+        # read from datastack file (ragged lists) 
         
-
+        self.peak_idxs_list = ds.read_list('hotmax_peak_idxs_list')
+        self.subpeak_idxs_list = ds.read_list('hotmax_subpeak_idxs_list')  
         
+         
     def plot_spectrum(self, n, ax=None, legend=False, headspace=1, footspace=0.1, 
                       hotlines_ticklabels=True, tight_layout=False): 
         
         if ax is None: 
 
             fig, ax = plt.subplots(figsize=[9, 3])
             
@@ -120,26 +68,27 @@
    
         # NEED DIFFERENT CODE 
         # the hotmax pixel peak (square marker)
         #hmp_x = self.x_keVs[hmp_i]
         #hmp_y = self.hotmax_spectra[n, hmp_i]
         #ax.scatter(hmp_x, hmp_y, marker='s', zorder=1, edgecolor='r', 
         #           facecolor='w', label=f'hotmax peak #{n}')
-        hmp_x = self.x_keVs[self.hotmax_mask[n]]
-        hmp_y = self.hotmax_spectra[n][self.hotmax_mask[n]]
+        
+        hmp_x = self.x_keVs[self.peak_idxs_list[n]]
+        hmp_y = self.hotmax_spectra[n][self.peak_idxs_list[n]]
         ax.scatter(hmp_x, hmp_y, marker='s', zorder=1, edgecolor='r', 
                    facecolor='w', label=f'hotmax peak #{n}') 
 
         # submax peaks (round markers)
-        peaks_x = self.x_keVs[self.peak_idxs_list[n]]
-        peaks_y = self.hotmax_spectra[n, self.peak_idxs_list[n]]
+        peaks_x = self.x_keVs[self.subpeak_idxs_list[n]]
+        peaks_y = self.hotmax_spectra[n, self.subpeak_idxs_list[n]]
         ax.scatter(peaks_x, peaks_y, edgecolor='b', alpha=1, zorder=0, facecolor='w')
         
         # annotate submax peaks 
-        peak_labels = self.peak_labels_list[n]
+        peak_labels = [f'({i})' for i, _ in enumerate(self.subpeak_idxs_list[n])]
         ann_list = []
         for i, plabel in enumerate(peak_labels):  
             peak_xy = peaks_x[i], peaks_y[i] 
             ann = ax.annotate(plabel, peak_xy, xytext=[0, 10], color='b', 
                               textcoords='offset points', ha='center')
             ann_list.append(ann)
  
@@ -286,62 +235,147 @@
     hot_pixels = []
     for k, c_map in enumerate(channel_maps): 
         hot_i, hot_j = np.argwhere(c_map == peaks_y[k]).flatten()
         hot_pixels.append([hot_i, hot_j, peak_indices[k]]) # xy
 
     hot_pixels = np.array(hot_pixels)  
     
-    # need to deduplicate identical spectra
+    # need to deduplicate identical spectra (i.e. superimposed hotmax pixels)
     
-    n_channels = len(x_keVs)
-    hotmax_spots, hotmax_mask = _group_superimposed(hot_pixels, n_channels)
+    hotmax_spots, hotmax_peak_idxs_list = _group_superimposed(hot_pixels)
     
 
     # read spectrum for each hot max pixel  
     hotmax_spectra = [] 
     for n, [i, j] in enumerate(hotmax_spots):
         print(f'Step 3/3: Reading hot max spectrum {n}/{len(hotmax_spots) - 1}...', end='\r')
         spectrum = ds.maxrf_cube[i,j,:].compute()
         hotmax_spectra.append(spectrum)
         
         ax.plot(x_keVs, spectrum, color='b', linewidth=0.5, alpha=0.5) 
         ax.fill_between(x_keVs, spectrum, color='b', linewidth=0.5, alpha=0.3) 
-        # NOT GOOD need mask now 
         
-        x = x_keVs[hotmax_mask[n]]
-        y = spectrum[hotmax_mask[n]]
+        # DEPRECIATING MASK, INSTEAD USING RAGGED LIST  
+        
+        #x = x_keVs[hotmax_mask[n]]
+        #y = spectrum[hotmax_mask[n]] 
+        
+        x = x_keVs[hotmax_peak_idxs_list[n]]
+        y = spectrum[hotmax_peak_idxs_list[n]]
         ax.scatter(x, y, facecolor='b', edgecolor='r') 
 
         # force updating plot 
         plt.pause(0.2) 
         fig.canvas.draw()
         fig.canvas.flush_events()
         
     print(f'Step 3/3: Ready with reading hot max spectra. ')
 
     hotmax_spectra = np.array(hotmax_spectra)   
     
     # user input           
-    write = input('Write hotmax spectra and pixels to datastack file [y/n]? ')
+    write = input('Write hotmax spectra, spots and peak indices to datastack file [y/n]? ')
          
     if write == 'y': 
         maxrf4u.append(hotmax_spectra, ds.HOTMAX_SPECTRA, ds.datastack_file)
         maxrf4u.append(hotmax_spots, 'hotmax_spots', ds.datastack_file) 
-        maxrf4u.append(hotmax_mask, 'hotmax_mask', ds.datastack_file) 
+        maxrf4u.append_list(hotmax_peak_idxs_list, 'hotmax_peak_idxs_list', ds.datastack_file) 
 
         print(f'\nSaved hotmax data to: {ds.datastack_file}')
         
     # force updating plot 
     plt.pause(0.3) 
     fig.canvas.draw()
     fig.canvas.flush_events()
     
     return  
+
+
+
+def compute_hotmax_noise(datastack_file, radius=200, alpha=0.6, beta=0.1): 
+    '''Utility function to get baselines and noiselines from hotmax spectra in *datastack_file*.  
+    
+    Use once to compute base noise envelopes. Ask user confirmation for saving result to datastack file. '''
+    
+    ds = maxrf4u.DataStack(datastack_file)
+    
+    x_keVs = ds.read(ds.MAXRF_ENERGIES)
+    hotmax_spectra = ds.read(ds.HOTMAX_SPECTRA)
+        
+    baseline_spectra = []  
+    noiseline_spectra = []
+    
+    for i, spectrum in enumerate(hotmax_spectra): 
+        
+        print(f'Computing noise envelope for hotmax spectrum {i+1}/{len(hotmax_spectra)}...', end='\r')
+        
+        baseline, lowest_indices = _baseline(x_keVs, spectrum, radius=radius, return_indices=True)
+        baseline_spectra.append(baseline)
+        
+        noiseline = _noiseline(baseline, alpha=alpha, beta=beta) 
+        noiseline_spectra.append(noiseline) 
+        
+    print(f'Ready computing {len(hotmax_spectra)} noise envelopes.                           \n')
+    
+    # user input           
+    write = input('Write hotmax baselines and noiselines to datastack file [y/n]? ')
+         
+    if write == 'y': 
+        maxrf4u.append(baseline_spectra, ds.HOTMAX_BASELINES, ds.datastack_file)
+        maxrf4u.append(noiseline_spectra, ds.HOTMAX_NOISELINES, ds.datastack_file) 
+
+        print(f'\nSaved hotmax noise data to: {ds.datastack_file}')
     
+    return 
+
+def compute_subpeaks(datastack_file, prominence=0.2): 
+    '''Find subpeaks in hotmax spectrum that exceed the noise envelope.
+    
+    Writes result to datas
+    
+    Returns: list of hotmax sub peak indices'''
+    
+    subpeak_idxs_list = []
+    
+    ds = maxrf4u.DataStack(datastack_file)
+    hotmax_spectra = ds.read('hotmax_spectra')
+    noiselines = ds.read('hotmax_noiselines')
+    
+    for y_hot, noiseline in zip(hotmax_spectra, noiselines): 
+    
+        # clip 
+        above_noise = y_hot - noiseline 
+        above_noise[above_noise < 0] = 0 
+
+        peak_idxs, _ = ssg.find_peaks(above_noise, prominence=prominence) 
+
+        # sort by peak height 
+        peak_heights = above_noise[peak_idxs]
+        peak_order = np.argsort(peak_heights)[::-1] 
+        peak_idxs = peak_idxs[peak_order] 
+
+        # hack to correct peak positions due to baseline tilting 
+        peak_idxs = _untilt(peak_idxs, y_hot, delta=5) 
+        
+        # append 
+        subpeak_idxs_list.append(peak_idxs)
+         
+    # user input           
+    write = input('Write hotmax baselines and noiselines to datastack file [y/n]? ')    
     
+    if write == 'y': 
+         
+        datapath = 'hotmax_subpeak_idxs_list'
+        maxrf4u.append_list(subpeak_idxs_list, datapath, datastack_file)       
+        print(f'\nSaved hotmax subpeak indexes list to: {datastack_file}')
+        
+    
+    return subpeak_idxs_list 
+
+
 
 def _baseline(x_keVs, spectrum, radius=200, return_indices=False): 
     '''Calculate rolling ball baseline for *spectrum*.  
     
     Uses Euclidian distance map to select only the lowest surges that touch the rolling ball.'''
 
     spectrum_norm = spectrum / spectrum.max()
@@ -383,50 +417,14 @@
     '''Estimate Poisson noise line from *baseline*. '''
     
     noiseline = baseline + alpha * np.sqrt(baseline + beta**2)
     
     return noiseline 
 
 
-def compute_hotmax_noise(datastack_file, radius=200, alpha=0.6, beta=0.1): 
-    '''Utility function to get baselines and noiselines from hotmax spectra in *datastack_file*.  
-    
-    Use once to compute base noise envelopes. Ask user confirmation for saving result to datastack file. '''
-    
-    ds = maxrf4u.DataStack(datastack_file)
-    
-    x_keVs = ds.read(ds.MAXRF_ENERGIES)
-    hotmax_spectra = ds.read(ds.HOTMAX_SPECTRA)
-        
-    baseline_spectra = []  
-    noiseline_spectra = []
-    
-    for i, spectrum in enumerate(hotmax_spectra): 
-        
-        print(f'Computing noise envelope for hotmax spectrum {i+1}/{len(hotmax_spectra)}...', end='\r')
-        
-        baseline, lowest_indices = _baseline(x_keVs, spectrum, radius=radius, return_indices=True)
-        baseline_spectra.append(baseline)
-        
-        noiseline = _noiseline(baseline, alpha=alpha, beta=beta) 
-        noiseline_spectra.append(noiseline) 
-        
-    print(f'Ready computing {len(hotmax_spectra)} noise envelopes.                           \n')
-    
-    # user input           
-    write = input('Write hotmax baselines and noiselines to datastack file [y/n]? ')
-         
-    if write == 'y': 
-        maxrf4u.append(baseline_spectra, ds.HOTMAX_BASELINES, ds.datastack_file)
-        maxrf4u.append(noiseline_spectra, ds.HOTMAX_NOISELINES, ds.datastack_file) 
-
-        print(f'\nSaved hotmax noise data to: {ds.datastack_file}')
-    
-    return 
-
 
 def _untilt(peak_idxs, y_hot, delta=5): 
     '''Adjust peak index positions to nearest true maxima.'''
     
     local_maxima = ssg.argrelextrema(y_hot, np.greater)[0] 
     
     new_peak_idxs = []
@@ -444,44 +442,49 @@
     # check  
     for i in new_peak_idxs: 
         assert i in list(local_maxima), 'Peak adjustment error'
             
     return new_peak_idxs 
 
 
-def _group_superimposed(hotmax_pixels, n_channels): 
+def _group_superimposed(hotmax_pixels): 
     '''Group superimposed `hotmax_pixels`. 
     
-    Returns: hotmax_spots, hotmax_mask '''
+    Returns: hotmax_spots, hotmax_peak_idxs_list '''
     
     hotspots = hotmax_pixels[:,:2] 
     unique_hotspots = np.unique(hotspots, axis=0)
     
     # create ragged sorted list of indices 
     indices_list = [] 
 
     for u in unique_hotspots: 
         is_spot = np.all(hotspots == u, axis=1)
         indices = np.arange(len(hotspots))[is_spot].tolist()
         indices_list.append(indices)
         
     first_indices = [idxs[0] for idxs in indices_list]
 
-    # sort 
+    # sort spectrum indices according to lowest energy hotmax peak 
     sorting = np.argsort(first_indices)
-    ragged_indices = [indices_list[s] for s in sorting]  
-    
-    # create corresponding list hotspots 
-    hotmax_spots = np.array([hotmax_pixels[idxs[0]][0:2] for idxs in ragged_indices])
+    ragged_idxs = [indices_list[s] for s in sorting] 
     
+    # create corresponding ragged list of peak channel indices 
+    hotmax_peak_idxs_list = [list(hotmax_pixels[:,2][idxs]) for idxs in ragged_idxs] 
     
-    # creat mask
-    n_hotspots = len(hotmax_spots)
-    shape = [n_hotspots, n_channels]
-    hotmax_mask = np.zeros(shape, dtype=bool)
+    # create corresponding list hotspots 
+    hotmax_spots = np.array([hotmax_pixels[idxs[0]][0:2] for idxs in ragged_idxs])
     
-    for i, idxs in enumerate(ragged_indices): 
-        peak_idxs = hotmax_pixels[idxs][:, 2]
-        hotmax_mask[i][peak_idxs] = True               
+    # DEPRECIATING BOOLEAN MASK: WILL USE append_list() INSTEAD  
+    ## creat mask
+    #n_hotspots = len(hotmax_spots)
+    #shape = [n_hotspots, n_channels]
+    #hotmax_mask = np.zeros(shape, dtype=bool)
+    #
+    #for i, idxs in enumerate(ragged_indices): 
+    #    peak_idxs = hotmax_pixels[idxs][:, 2]
+    #    hotmax_mask[i][peak_idxs] = True               
+    #
+    #return hotmax_spots, hotmax_mask 
     
-    return hotmax_spots, hotmax_mask 
+    return hotmax_spots, hotmax_peak_idxs_list
```

### Comparing `maxrf4u-0.1.1/maxrf4u/interactive_visualization.py` & `maxrf4u-0.1.2/maxrf4u/interactive_visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../notebooks/91_interactive-plotting.ipynb.
 
 # %% auto 0
 __all__ = ['UploadDir', 'make_filenames', 'make_gridbox_widget']
 
-# %% ../notebooks/91_interactive-plotting.ipynb 26
+# %% ../notebooks/91_interactive-plotting.ipynb 25
 import json 
 import os 
 
 import IPython 
 
 from IPython.display import display
 from IPython.display import Image
@@ -23,15 +23,15 @@
 import os 
 
 import PIL
 import urllib 
 import numpy as np 
 import matplotlib.pyplot as plt
 
-# %% ../notebooks/91_interactive-plotting.ipynb 27
+# %% ../notebooks/91_interactive-plotting.ipynb 26
 class UploadDir(): 
     
     def __init__(self, mount_dir, objnr, bucket_url, subdir='images'):
         '''Creates a standard upload (image) directory object. '''
         
         self._mount_dir = mount_dir
         self._objnr = objnr
```

### Comparing `maxrf4u-0.1.1/maxrf4u/peakmaps.py` & `maxrf4u-0.1.2/maxrf4u/peakmaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../notebooks/60_peakmaps.ipynb.
 
 # %% auto 0
-__all__ = ['get_continuum', 'get_gaussians', 'fit_spectrum', 'get_spectral_slices', 'compute_nmf_peakmaps', 'multi_plot',
+__all__ = ['get_continuum', 'get_gaussians', 'fit_spectrum_peaks', 'compute_nmf_peakmaps', 'multi_plot',
            'compute_nmf_element_maps']
 
-# %% ../notebooks/60_peakmaps.ipynb 30
+# %% ../notebooks/60_peakmaps.ipynb 29
 from dask import delayed 
 from dask.diagnostics import ProgressBar 
 import maxrf4u 
 import numpy as np 
 import scipy.interpolate as sip 
 import scipy.signal as ssg 
 import matplotlib.pyplot as plt 
 from IPython.display import SVG 
 
 import sklearn.decomposition as skd 
 
-# %% ../notebooks/60_peakmaps.ipynb 31
+# %% ../notebooks/60_peakmaps.ipynb 30
 def get_continuum(datastack_file): 
     '''Compute continuum baseline from sum spectrum.
     
     Uses rolling ball filter to remove peaks from sum spectrum. 
     
     Returns: y_continuum
     '''
@@ -62,15 +62,15 @@
     
     # pick smallest half width at rel_height 
     dx_left = left_x - x[peak_idx] 
     dx_right = right_x - x[peak_idx] 
     
     dx = sorted([dx_left, dx_right])[0] 
     
-    # create baseline  
+    # create baseline if None   
     if baseline is None:  
         baseline = np.zeros_like(y) 
         
     y_norm = (width_height - baseline[peak_idx]) / (y[peak_idx] - baseline[peak_idx]) 
     
     # assert that y_norm is positive 
     assert y_norm > 0, f"Can't fit Gaussian for peak below baseline for peak index {peak_idx}."   
@@ -81,89 +81,81 @@
     # calculate gaussian with baseline 
     y_gauss = (y[peak_idx] - baseline[peak_idx]) * _gaussian(x, x[peak_idx], sigma) + baseline
     
     return y_gauss, baseline 
 
 
 def get_gaussians(datastack_file, tail_clip=0.05, norm=True): 
-    '''Computes fitted Gaussian peak profiles for all hotmax pixels. 
-    
+    '''Fit Gaussian peak profiles to hotmax peaks in hotmax atlas. 
+
     Returns: y_gauss_list
     '''
-    
+
     # read stuff from datastack 
-    ds = maxrf4u.DataStack(datastack_file) 
+    ds = maxrf4u.DataStack('RP-T-1898-A-3689.datastack') 
 
     x_keVs = ds.read('maxrf_energies') 
-    hotmax_pixels = ds.read('hotmax_pixels')
     hotmax_spectra = ds.read('hotmax_spectra')
     hotmax_baselines = ds.read('hotmax_baselines') 
-
-    peak_idxs = hotmax_pixels[:,2]
+    peak_idxs_list = ds.read_list('hotmax_peak_idxs_list')
 
     # get slices by fitting gaussian to corresponding hotmax spectrum and baseline 
     y_gauss_list = []
 
-    # Create tail clipped gaussians 
-    for i, peak_idx in enumerate(peak_idxs):  
+    # Create tail clipped gaussians for ragged peak indexes list 
+    for n, peak_idxs in enumerate(peak_idxs_list):  
 
-        y_hot = hotmax_spectra[i]
-        baseline = hotmax_baselines[i]
-        y_gauss_fit, baseline = _fit_gaussian(x_keVs, y_hot, peak_idx, baseline=baseline) 
+        y_hot = hotmax_spectra[n]
+        baseline = hotmax_baselines[n] 
 
-        y_gauss_flat =  y_gauss_fit - baseline 
-        
-        if norm is True: 
-            y_gauss_flat = y_gauss_flat / y_gauss_flat.max()
+        # iterate over (possibly multiple) peaks in each hotmax spectrum 
+        for idx in peak_idxs: 
+
+            y_gauss_fit, baseline = _fit_gaussian(x_keVs, y_hot, idx, baseline=baseline) 
+            y_gauss_flat =  y_gauss_fit - baseline 
+
+            if norm is True: 
+                y_gauss_flat = y_gauss_flat / y_gauss_flat.max()
+
+            y_gauss_list.append(y_gauss_flat)
             
-        y_gauss_list.append(y_gauss_flat)
-        
     return y_gauss_list 
 
 
-def fit_spectrum(y, datastack_file): 
+def fit_spectrum_peaks(y, datastack_file): 
     '''Fit Gaussian peak shapes to single spectrum `y`.
     
     Uses NMF with fixed Gaussian component vectors. 
     
     Returns: weighed_components_list 
     '''
 
     X = y.reshape([1, -1]) # make single spectro into two dimenional array 
     
 
     y_continuum = get_continuum('RP-T-1898-A-3689.datastack')
-
     y_gauss_list = get_gaussians('RP-T-1898-A-3689.datastack', norm=False)
 
     # create component vectors 
     H = np.array([y_gauss for y_gauss in y_gauss_list]).astype(np.float32)
     # add continuum as component
     H = np.r_[H, y_continuum[None,:].astype(np.float32)]
     
     n_components, n_channels = H.shape
 
     W, H, n_iter = skd.non_negative_factorization(X, H=H, n_components=n_components, update_H=False)
-
-    X_nmf = W @ H 
-    y_nmf = X_nmf.flatten()
     
-    # now create list of weighed components (peaks) 
-    # for easy plotting fitted peaks with individual colors  
-    
-    W_flat = W.flatten()
-    
-    fitted_list = []
+    # not neede here, but just a reminder  
+    # X_nmf = W @ H 
+    # y_nmf = X_nmf.flatten() 
+
+    # transpose weights for easy multiplication  
+    w =  W.T 
     
-    for i, w in enumerate(W_flat): 
-        
-        fitted = w * H[i]
-        fitted_list.append(fitted) 
-        
-    return fitted_list  
+    return w, H 
         
 
     
 def _add_hotlines_ticklabels(datastack_file, ax, vlines=True, clip_vline=True): 
     '''Utility function. Adds hotlines and tick labels to plot `ax`. 
     
     '''
@@ -193,15 +185,15 @@
     secax.set_xticks(x_keVs[peak_idxs])
     secax.set_xticklabels(range(len(peak_idxs)), fontsize=6, color='r') 
     secax.tick_params(color=[1, 0.5, 0.5], pad=0) 
     
     return ax 
 
 
-def get_spectral_slices(cube): 
+def _get_spectral_slices(cube): 
     '''Low level bookkeeping to compute slice indices for spectral chunks from dask array `cube`. 
        
     Returns: row_slices, column_slices  
     '''
     
     h, w, d = cube.shape 
 
@@ -247,15 +239,15 @@
 
     n_components, n_channels = H.shape
 
     #initialize peak map stack  
     peak_map_stack = np.zeros([h, w, n_components], dtype=np.float32)
 
     # prepare chunk bookkeeping 
-    row_slices, column_slices = get_spectral_slices(cube)
+    row_slices, column_slices = _get_spectral_slices(cube)
 
     n_chunks = len(row_slices) * len(column_slices)
 
     n = 1 
     print('Please wait a few minutes while preparing your peak maps. ')
     for ri, rj in row_slices:
```

### Comparing `maxrf4u-0.1.1/maxrf4u/peakpuzzle.py` & `maxrf4u-0.1.2/maxrf4u/peakpuzzle.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     alpha_keVs = [p['peaks_xy'][0, 0] for p in ptrn_dict_list]        
     indices = np.argsort(alpha_keVs) 
     
     ptrn_list = [ptrn_dict_list[i] for i in indices] 
         
     return ptrn_list  
 
+
 def colorize(elem): 
     '''Pick fixed color from nice color map for elements of interest. '''
     
     # select elements of interest 
     all_elements = ['#H', '#He', '#Li', '#Be', '#B', '#C', 'N', 'O', 'F', 'Ne', 'Na', 'Mg', 'Al', 
                     'Si', 'P', 'S', 'Cl', '#Ar', 'K', 'Ca', '#Sc', 'Ti', 'V', 'Cr', 'Mn', 'Fe', 
                     'Co', 'Ni', 'Cu', 'Zn', '#Ga', '#Ge', 'As', '#Se', 'Br', '#Kr', '#Rb', 'Sr',
```

### Comparing `maxrf4u-0.1.1/maxrf4u/storage.py` & `maxrf4u-0.1.2/maxrf4u/storage.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/maxrf4u/warp.py` & `maxrf4u-0.1.2/maxrf4u/warp.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/maxrf4u/xphysics.py` & `maxrf4u-0.1.2/maxrf4u/xphysics.py`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/maxrf4u.egg-info/PKG-INFO` & `maxrf4u-0.1.2/maxrf4u.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxrf4u
-Version: 0.1.1
+Version: 0.1.2
 Summary: Explore your X-Ray Fluorescence spectral images
 Home-page: https://github.com/fligt/maxrf4u
 Author: Frank Ligterink
 Author-email: frank.ligterink@gmail.com
 License: GNU General Public License v3
 Description: # Welcome to maxrf4u
```

### Comparing `maxrf4u-0.1.1/maxrf4u.egg-info/SOURCES.txt` & `maxrf4u-0.1.2/maxrf4u.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maxrf4u-0.1.1/settings.ini` & `maxrf4u-0.1.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = maxrf4u
 lib_name = maxrf4u
-version = 0.1.1
+version = 0.1.2
 min_python = 3.7
 license = gpl3
 black_formatting = False
 doc_path = _docs
 lib_path = maxrf4u
 nbs_path = notebooks
 recursive = True
```

### Comparing `maxrf4u-0.1.1/setup.py` & `maxrf4u-0.1.2/setup.py`

 * *Files identical despite different names*

