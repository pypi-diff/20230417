# Comparing `tmp/PyCytoData-0.1.0.tar.gz` & `tmp/PyCytoData-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCytoData-0.1.0.tar", last modified: Sun Jul 17 19:55:51 2022, max compression
+gzip compressed data, was "PyCytoData-0.1.1.tar", last modified: Sun Apr 16 22:53:45 2023, max compression
```

## Comparing `PyCytoData-0.1.0.tar` & `PyCytoData-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-07-17 19:55:42.101650 PyCytoData-0.1.0/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1080 2022-05-19 02:00:57.000000 PyCytoData-0.1.0/LICENSE.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2669 2022-06-18 21:34:56.000000 PyCytoData-0.1.0/LICENSE_associated.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9500 2022-07-17 19:55:42.099648 PyCytoData-0.1.0/PKG-INFO
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-07-17 19:55:42.030341 PyCytoData-0.1.0/PyCytoData/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      127 2022-07-17 19:48:05.000000 PyCytoData-0.1.0/PyCytoData/__init__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      145 2022-06-18 21:34:56.000000 PyCytoData-0.1.0/PyCytoData/__main__.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    55799 2022-07-17 18:08:06.000000 PyCytoData-0.1.0/PyCytoData/data.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1688 2022-06-04 21:23:36.000000 PyCytoData-0.1.0/PyCytoData/exceptions.py
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)    15944 2022-06-04 21:22:57.000000 PyCytoData-0.1.0/PyCytoData/preprocess.py
-drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2022-07-17 19:55:42.087648 PyCytoData-0.1.0/PyCytoData.egg-info/
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9500 2022-07-17 19:55:41.000000 PyCytoData-0.1.0/PyCytoData.egg-info/PKG-INFO
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)      337 2022-07-17 19:55:41.000000 PyCytoData-0.1.0/PyCytoData.egg-info/SOURCES.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)        1 2022-07-17 19:55:41.000000 PyCytoData-0.1.0/PyCytoData.egg-info/dependency_links.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       29 2022-07-17 19:55:41.000000 PyCytoData-0.1.0/PyCytoData.egg-info/requires.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       11 2022-07-17 19:55:41.000000 PyCytoData-0.1.0/PyCytoData.egg-info/top_level.txt
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9010 2022-07-17 19:52:04.000000 PyCytoData-0.1.0/README.md
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)       38 2022-07-17 19:55:42.101650 PyCytoData-0.1.0/setup.cfg
--rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3217 2022-07-17 19:47:43.000000 PyCytoData-0.1.0/setup.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2023-04-16 22:53:40.860759 PyCytoData-0.1.1/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1080 2022-05-19 02:00:57.000000 PyCytoData-0.1.1/LICENSE.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     2669 2022-06-18 21:34:56.000000 PyCytoData-0.1.1/LICENSE_associated.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9661 2023-04-16 22:53:40.858593 PyCytoData-0.1.1/PKG-INFO
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2023-04-16 22:53:40.799026 PyCytoData-0.1.1/PyCytoData/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      127 2023-04-16 22:39:39.000000 PyCytoData-0.1.1/PyCytoData/__init__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      145 2022-06-18 21:34:56.000000 PyCytoData-0.1.1/PyCytoData/__main__.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    56851 2023-04-16 22:49:34.000000 PyCytoData-0.1.1/PyCytoData/data.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     1688 2022-06-04 21:23:36.000000 PyCytoData-0.1.1/PyCytoData/exceptions.py
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)    16086 2023-04-16 22:39:39.000000 PyCytoData-0.1.1/PyCytoData/preprocess.py
+drwxrwxrwx   0 kevin     (1000) kevin     (1000)        0 2023-04-16 22:53:40.848979 PyCytoData-0.1.1/PyCytoData.egg-info/
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9661 2023-04-16 22:53:40.000000 PyCytoData-0.1.1/PyCytoData.egg-info/PKG-INFO
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)      337 2023-04-16 22:53:40.000000 PyCytoData-0.1.1/PyCytoData.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)        1 2023-04-16 22:53:40.000000 PyCytoData-0.1.1/PyCytoData.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       29 2023-04-16 22:53:40.000000 PyCytoData-0.1.1/PyCytoData.egg-info/requires.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       11 2023-04-16 22:53:40.000000 PyCytoData-0.1.1/PyCytoData.egg-info/top_level.txt
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     9171 2023-04-16 22:39:39.000000 PyCytoData-0.1.1/README.md
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)       38 2023-04-16 22:53:40.860759 PyCytoData-0.1.1/setup.cfg
+-rwxrwxrwx   0 kevin     (1000) kevin     (1000)     3217 2023-04-16 22:39:39.000000 PyCytoData-0.1.1/setup.py
```

### Comparing `PyCytoData-0.1.0/LICENSE.txt` & `PyCytoData-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyCytoData-0.1.0/LICENSE_associated.txt` & `PyCytoData-0.1.1/LICENSE_associated.txt`

 * *Files identical despite different names*

### Comparing `PyCytoData-0.1.0/PKG-INFO` & `PyCytoData-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: PyCytoData
-Version: 0.1.0
+Version: 0.1.1
 Summary: An Elegant Data Analysis Tool for CyTOF
 Home-page: https://github.com/kevin931/PyCytoData
 Author: PyCytoData Developers
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: LICENSE_associated.txt
 
+![Logo](./assets/pycytodata.jpg)
+
 # PyCytoData
 > An elegant data analysis tool for CyTOF.
 
 This package is an all-in-one CyTOF data analysis package for your experiments. From loading datasets to DR and evaluation, you have a consistent interface and readable code every step along the way. There is also support for some of ``HDCytoData``'s benchmark datasets as originally implemented in R by Weber & Soneson (2019) in [this repository](https://github.com/lmweber/HDCytoData). Why wait? Start your PyCytoData journal right here, right now! 
 
 ## Installation
 
@@ -124,15 +126,15 @@
 >>> byod.preprocess(arcsinh=True,
 ...                 gate_debris_removal=True,
 ...                 gate_intact_cells=True,
 ...                 gate_live_cells=True,
 ...                 gate_center_offset_residual=True,
 ...                 bead_normalization=True)
 
-byod.expression_matrix # This is preprocessed
+>>> byod.expression_matrix # This is preprocessed
 ```
 As the example shows, we support five unique preprocessing steps! And of course, you can use a subset of these to suit your own needs! By default, we automatically detect the necessary channels, such as "Bead1" or "Center". However, if your dataset is unconventionally named, our auto-detect algorithm may fail. Thus, we can perform a manual override:
 
 ```python
 >>> byod.preprocess(arcsinh=True,
 ...                 gate_debris_removal=True,
 ...                 gate_intact_cells=True,
@@ -171,56 +173,35 @@
 
 ## Documentation
 
 For detailed documentation along with tutorials and API Reference, please visit our [Official Documentation](https://pycytodata.readthedocs.io/en/latest/). This is automatically updated with each update.
 
 If you prefer to build documentation on your own, refer to [this guide](https://pycytodata.readthedocs.io/en/latest/change/build.html) for more details.
 
-## Latest Release: 0.1.0
+## Latest Release: 0.1.1
 
-This is the first official release of ``PyCytoData`` with LTS.
+This is a minor release with various bug fixes and documentation improvents.
 
 ### Bug Fixes
 
-- Fix the default cofactor of ``PyCytoData.preprocess``
-- Fix lineage channels for ``levine32`` and ``samusik``
+- Fixed a potential issue with loading benchmark datasets' samples out of order (This behavior is not guaranteed, but a implementation detail)
+- Fixed an issue with ``DataLoader.load_dataset`` not recognizing downloaded datasets
+- Fixed an issue with ``preprocess.bead_normalization`` having uninitialized array (#9)
 
 ### Changes and New Features
 
-- ``PyCytoData.run_dr_methods`` now runs on lineage channels only
-- Add tutorials and references for documentation
-- Improve docstrings and general documentations
-- Add preprocessing options for loading benchmark datasets
-- Relax ``numpy`` dependency to >=1.20
-- Add descriptors for PyPI releases
-
-### Deprecations
-
-- Permanently remove ``FileIO.make_dir`` function for safety reasons
+- No new feature added
+- Improved documentations with streamlined front page and updated links
+- Added docstrings for `+` and `+=` operators
+- Updated references for CytofDR paper publication in Nature Communications
 
 
 ## References
 
-If you use ``PyCytoData`` to perform DR, citing the [our DR Review paper](https://doi.org/10.1101/2022.04.26.489549) is highly appreciated:
-
-```
-@article {Wang2022.04.26.489549,
-	author = {Wang, Kaiwen and Yang, Yuqiu and Wu, Fangjiang and Song, Bing and Wang, Xinlei and Wang, Tao},
-	title = {Comparative Analysis of Dimension Reduction Methods for Cytometry by Time-of-Flight Data},
-	elocation-id = {2022.04.26.489549},
-	year = {2022},
-	doi = {10.1101/2022.04.26.489549},
-	publisher = {Cold Spring Harbor Laboratory},
-	URL = {https://www.biorxiv.org/content/early/2022/06/02/2022.04.26.489549},
-	eprint = {https://www.biorxiv.org/content/early/2022/06/02/2022.04.26.489549.full.pdf},
-	journal = {bioRxiv}
-}
-```
-
-If you use ``Cytomulate`` with this package, [our paper](https://doi.org/10.1101/2022.06.14.496200) can be cited here:
+If you used ``PyCytoData`` in your research or with ``Cytomulate`` as part of the pipeline, please cite [our paper](https://doi.org/10.1101/2022.06.14.496200) here:
 
 ```
 @article {Yang2022.06.14.496200,
 	author = {Yang, Yuqiu and Wang, Kaiwen and Lu, Zeyu and Wang, Tao and Wang, Xinlei},
 	title = {Cytomulate: Accurate and Efficient Simulation of CyTOF data},
 	elocation-id = {2022.06.14.496200},
 	year = {2022},
@@ -228,10 +209,31 @@
 	publisher = {Cold Spring Harbor Laboratory},
 	URL = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200},
 	eprint = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
+If you use ``PyCytoData`` to perform DR, citing the [our DR Review paper](https://doi.org/10.1038/s41467-023-37478-w) is highly appreciated:
+
+```
+Wang, K., Yang, Y., Wu, F. et al. Comparative analysis of dimension reduction methods for cytometry by time-of-flight data. Nat Commun 14, 1836 (2023). https://doi.org/10.1038/s41467-023-37478-w
+```
+
+or
+
+```
+@article{wang2023comparative,
+  title={Comparative analysis of dimension reduction methods for cytometry by time-of-flight data},
+  author={Wang, Kaiwen and Yang, Yuqiu and Wu, Fangjiang and Song, Bing and Wang, Xinlei and Wang, Tao},
+  journal={Nature communications},
+  volume={14},
+  number={1},
+  pages={1--18},
+  year={2023},
+  publisher={Nature Publishing Group UK London}
+}
+```
+
 If you use the builtin datasets, please visit our [Reference Page](https://pycytodata.readthedocs.io/en/latest/references.html) and cite the papers accordingly.
```

### Comparing `PyCytoData-0.1.0/PyCytoData/data.py` & `PyCytoData-0.1.1/PyCytoData/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         if gate_center_offset_residual:
             _verbose("Runinng gating Center, Offset, and Residual...", verbose=verbose)
             assert cor_channels is not None
             expression_processed, indices_temp = preprocess.gate_center_offset_residual(expression_processed, self.channels, cor_channels, cor_cutoff_quantile)
             indices = indices[indices_temp]
             
         if bead_normalization:
-            _verbose("Runinng bead normalization...", verbose=verbose)
+            _verbose("Running bead normalization...", verbose=verbose)
             assert bead_channels is not None
             assert time_channel is not None
             assert self.lineage_channels is not None
             expression_processed, indices_temp = preprocess.bead_normalization(expression_processed, self.channels, bead_channels, time_channel, self.lineage_channels)
             indices = indices[indices_temp]
         
         self.expression_matrix = expression_processed
@@ -454,21 +454,45 @@
         :return: The length of the object.
         :rtype: int
         """
         return self.n_cells
     
     
     def __iadd__(self, new_object: PyCytoData) -> PyCytoData:
+        """Concatenate a new `PyCytoData` object with the `+=` operator.
+
+        This essentially works the same way the ``add_sample`` method. However,
+        instead of the necessity of providing the expression matrices, sample
+        indices, and the cell types manually, the concatenation is automatically
+        performed from a new `PyCytoData` object.
+
+        :param new_object: The second `PyCytoData` object.
+        :type new_object: PyCytoData
+        :raises TypeError: The provided object is not a `PyCytoData` object.
+        :return: A new `PyCytoData` object after concatenation.
+        :rtype: PyCytoData
+        """
         if not isinstance(new_object, PyCytoData):
             raise TypeError("The right hand side has to be a 'PyCytoData' object.")
         self.add_sample(new_object.expression_matrix, sample_index=new_object.sample_index, cell_types=new_object.cell_types)
         return self
     
     
     def __add__(self, new_object: PyCytoData) -> PyCytoData:
+        """Concatenate two `PyCytoData` objects with the `+` operator.
+
+        This method concatenates two `PyCytOData` objects together by using
+        the `add_sample` method internally. A new `PyCytoData` object is returned.
+
+        :param new_object: The second `PyCytoData` object.
+        :type new_object: PyCytoData
+        :raises TypeError: The provided object is not a `PyCytoData` object.
+        :return: A new `PyCytoData` object after concatenation.
+        :rtype: PyCytoData
+        """
         if not isinstance(new_object, PyCytoData):
             raise TypeError("The right hand side has to be a 'PyCytoData' object.")
         out_object = deepcopy(self)
         out_object.add_sample(new_object.expression_matrix, sample_index=new_object.sample_index, cell_types=new_object.cell_types)
         return out_object
     
     
@@ -794,18 +818,15 @@
     """
 
     # Package data directory and Path
     _data_dir = pkg_resources.resource_filename("PyCytoData", "data/")
     _data_path: Dict[str, str] = {"levine13": _data_dir + "levine13/",
                                   "levine32": _data_dir + "levine32/",
                                   "samusik": _data_dir + "samusik/"}
-    # Check data status
-    _data_status: Dict[str, bool] = {}
-    for d in _data_path.keys():
-        _data_status[d] = os.path.exists(_data_path[d])
+
 
     @classmethod    
     def load_dataset(cls, dataset: str, sample: Optional[ArrayLike]=None, force_download: bool = False, preprocess: bool=False) -> PyCytoData:
         """Load benchmark datasets.
 
         This methods downloads and load benchmark datasets. The dataset is downloaded only once, which is then
         cached for future use. Currently, we support three datasets:
@@ -834,34 +855,35 @@
         :return: The loaded dataset.
         :rtype: PyCytoData
         """
         
         dataset = dataset.lower()
         if dataset not in ["levine13", "levine32", "samusik"]:
             raise ValueError("Unsupported dataset: Have to be 'levine13', 'levine32', or 'samusik'.")
-        
-        if not cls._data_status[dataset]:
+                
+        if not os.path.exists(cls._data_path[dataset]):
             cls._download_data(dataset = dataset, force_download = force_download)
             
         if sample is not None and not isinstance(sample, np.ndarray):
             sample = np.array(sample).flatten()
             
         all_files = glob.glob(cls._data_path[dataset]+dataset+"*.txt")
+        all_files = sorted(all_files)
         files: List[str] = []
         metadata_files: List[str] = []
         for f in all_files:
             if "metadata" in f:
                 metadata_files.append(f)
             else:
                 files.append(f)
 
         if sample is not None:
             r = re.compile("(.*" + ".*)|(.*".join(sample) + ".*)")
             files = list(filter(r.match, files))
-            metadata_files = list(filter(r.match, metadata_files))         
+            metadata_files = list(filter(r.match, metadata_files))   
             
         data: PyCytoData = FileIO.load_expression(files=files, col_names = True)
         metadata: Optional[np.ndarray] = None
         for i, m in enumerate(metadata_files):
             if i == 0:
                 metadata = np.loadtxt(fname=m, dtype ="str", delimiter="\t")
             else:
```

### Comparing `PyCytoData-0.1.0/PyCytoData/exceptions.py` & `PyCytoData-0.1.1/PyCytoData/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyCytoData-0.1.0/PyCytoData/preprocess.py` & `PyCytoData-0.1.1/PyCytoData/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,16 @@
     data = data[np.isin(intervals, unique_intervals),:]
     indices = indices[np.isin(intervals, unique_intervals)]
     
     # Normalization
     intervals: np.ndarray = np.round(data[:,np.isin(channels, time_channel)]/np.max(data[:,np.isin(channels, time_channel)])*200).flatten() # type: ignore
     unique_intervals: np.ndarray = np.unique(intervals)
     interval_mean: np.ndarray = np.empty((unique_intervals.shape[0], data.shape[1]), dtype=float) # type: ignore
+    for i in range(0, unique_intervals.shape[0]):
+        interval_mean[i] = np.mean(data[np.isin(intervals, unique_intervals[i]),:], axis=0)
     
     for c in bead_channels:
         data[:,np.isin(channels, c)] = data[:, np.isin(channels, c)]/np.mean(data[:, np.isin(channels, c)]) #type: ignore
         
     if bead_channels.shape[0] > 1:
         cormat: np.ndarray = np.corrcoef(interval_mean[:, np.isin(channels, bead_channels)], rowvar=False)
         np.fill_diagonal(cormat, -1)
```

### Comparing `PyCytoData-0.1.0/PyCytoData.egg-info/PKG-INFO` & `PyCytoData-0.1.1/PyCytoData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: PyCytoData
-Version: 0.1.0
+Version: 0.1.1
 Summary: An Elegant Data Analysis Tool for CyTOF
 Home-page: https://github.com/kevin931/PyCytoData
 Author: PyCytoData Developers
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: LICENSE_associated.txt
 
+![Logo](./assets/pycytodata.jpg)
+
 # PyCytoData
 > An elegant data analysis tool for CyTOF.
 
 This package is an all-in-one CyTOF data analysis package for your experiments. From loading datasets to DR and evaluation, you have a consistent interface and readable code every step along the way. There is also support for some of ``HDCytoData``'s benchmark datasets as originally implemented in R by Weber & Soneson (2019) in [this repository](https://github.com/lmweber/HDCytoData). Why wait? Start your PyCytoData journal right here, right now! 
 
 ## Installation
 
@@ -124,15 +126,15 @@
 >>> byod.preprocess(arcsinh=True,
 ...                 gate_debris_removal=True,
 ...                 gate_intact_cells=True,
 ...                 gate_live_cells=True,
 ...                 gate_center_offset_residual=True,
 ...                 bead_normalization=True)
 
-byod.expression_matrix # This is preprocessed
+>>> byod.expression_matrix # This is preprocessed
 ```
 As the example shows, we support five unique preprocessing steps! And of course, you can use a subset of these to suit your own needs! By default, we automatically detect the necessary channels, such as "Bead1" or "Center". However, if your dataset is unconventionally named, our auto-detect algorithm may fail. Thus, we can perform a manual override:
 
 ```python
 >>> byod.preprocess(arcsinh=True,
 ...                 gate_debris_removal=True,
 ...                 gate_intact_cells=True,
@@ -171,56 +173,35 @@
 
 ## Documentation
 
 For detailed documentation along with tutorials and API Reference, please visit our [Official Documentation](https://pycytodata.readthedocs.io/en/latest/). This is automatically updated with each update.
 
 If you prefer to build documentation on your own, refer to [this guide](https://pycytodata.readthedocs.io/en/latest/change/build.html) for more details.
 
-## Latest Release: 0.1.0
+## Latest Release: 0.1.1
 
-This is the first official release of ``PyCytoData`` with LTS.
+This is a minor release with various bug fixes and documentation improvents.
 
 ### Bug Fixes
 
-- Fix the default cofactor of ``PyCytoData.preprocess``
-- Fix lineage channels for ``levine32`` and ``samusik``
+- Fixed a potential issue with loading benchmark datasets' samples out of order (This behavior is not guaranteed, but a implementation detail)
+- Fixed an issue with ``DataLoader.load_dataset`` not recognizing downloaded datasets
+- Fixed an issue with ``preprocess.bead_normalization`` having uninitialized array (#9)
 
 ### Changes and New Features
 
-- ``PyCytoData.run_dr_methods`` now runs on lineage channels only
-- Add tutorials and references for documentation
-- Improve docstrings and general documentations
-- Add preprocessing options for loading benchmark datasets
-- Relax ``numpy`` dependency to >=1.20
-- Add descriptors for PyPI releases
-
-### Deprecations
-
-- Permanently remove ``FileIO.make_dir`` function for safety reasons
+- No new feature added
+- Improved documentations with streamlined front page and updated links
+- Added docstrings for `+` and `+=` operators
+- Updated references for CytofDR paper publication in Nature Communications
 
 
 ## References
 
-If you use ``PyCytoData`` to perform DR, citing the [our DR Review paper](https://doi.org/10.1101/2022.04.26.489549) is highly appreciated:
-
-```
-@article {Wang2022.04.26.489549,
-	author = {Wang, Kaiwen and Yang, Yuqiu and Wu, Fangjiang and Song, Bing and Wang, Xinlei and Wang, Tao},
-	title = {Comparative Analysis of Dimension Reduction Methods for Cytometry by Time-of-Flight Data},
-	elocation-id = {2022.04.26.489549},
-	year = {2022},
-	doi = {10.1101/2022.04.26.489549},
-	publisher = {Cold Spring Harbor Laboratory},
-	URL = {https://www.biorxiv.org/content/early/2022/06/02/2022.04.26.489549},
-	eprint = {https://www.biorxiv.org/content/early/2022/06/02/2022.04.26.489549.full.pdf},
-	journal = {bioRxiv}
-}
-```
-
-If you use ``Cytomulate`` with this package, [our paper](https://doi.org/10.1101/2022.06.14.496200) can be cited here:
+If you used ``PyCytoData`` in your research or with ``Cytomulate`` as part of the pipeline, please cite [our paper](https://doi.org/10.1101/2022.06.14.496200) here:
 
 ```
 @article {Yang2022.06.14.496200,
 	author = {Yang, Yuqiu and Wang, Kaiwen and Lu, Zeyu and Wang, Tao and Wang, Xinlei},
 	title = {Cytomulate: Accurate and Efficient Simulation of CyTOF data},
 	elocation-id = {2022.06.14.496200},
 	year = {2022},
@@ -228,10 +209,31 @@
 	publisher = {Cold Spring Harbor Laboratory},
 	URL = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200},
 	eprint = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
+If you use ``PyCytoData`` to perform DR, citing the [our DR Review paper](https://doi.org/10.1038/s41467-023-37478-w) is highly appreciated:
+
+```
+Wang, K., Yang, Y., Wu, F. et al. Comparative analysis of dimension reduction methods for cytometry by time-of-flight data. Nat Commun 14, 1836 (2023). https://doi.org/10.1038/s41467-023-37478-w
+```
+
+or
+
+```
+@article{wang2023comparative,
+  title={Comparative analysis of dimension reduction methods for cytometry by time-of-flight data},
+  author={Wang, Kaiwen and Yang, Yuqiu and Wu, Fangjiang and Song, Bing and Wang, Xinlei and Wang, Tao},
+  journal={Nature communications},
+  volume={14},
+  number={1},
+  pages={1--18},
+  year={2023},
+  publisher={Nature Publishing Group UK London}
+}
+```
+
 If you use the builtin datasets, please visit our [Reference Page](https://pycytodata.readthedocs.io/en/latest/references.html) and cite the papers accordingly.
```

### Comparing `PyCytoData-0.1.0/README.md` & `PyCytoData-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![Logo](./assets/pycytodata.jpg)
+
 # PyCytoData
 > An elegant data analysis tool for CyTOF.
 
 This package is an all-in-one CyTOF data analysis package for your experiments. From loading datasets to DR and evaluation, you have a consistent interface and readable code every step along the way. There is also support for some of ``HDCytoData``'s benchmark datasets as originally implemented in R by Weber & Soneson (2019) in [this repository](https://github.com/lmweber/HDCytoData). Why wait? Start your PyCytoData journal right here, right now! 
 
 ## Installation
 
@@ -108,15 +110,15 @@
 >>> byod.preprocess(arcsinh=True,
 ...                 gate_debris_removal=True,
 ...                 gate_intact_cells=True,
 ...                 gate_live_cells=True,
 ...                 gate_center_offset_residual=True,
 ...                 bead_normalization=True)
 
-byod.expression_matrix # This is preprocessed
+>>> byod.expression_matrix # This is preprocessed
 ```
 As the example shows, we support five unique preprocessing steps! And of course, you can use a subset of these to suit your own needs! By default, we automatically detect the necessary channels, such as "Bead1" or "Center". However, if your dataset is unconventionally named, our auto-detect algorithm may fail. Thus, we can perform a manual override:
 
 ```python
 >>> byod.preprocess(arcsinh=True,
 ...                 gate_debris_removal=True,
 ...                 gate_intact_cells=True,
@@ -155,56 +157,35 @@
 
 ## Documentation
 
 For detailed documentation along with tutorials and API Reference, please visit our [Official Documentation](https://pycytodata.readthedocs.io/en/latest/). This is automatically updated with each update.
 
 If you prefer to build documentation on your own, refer to [this guide](https://pycytodata.readthedocs.io/en/latest/change/build.html) for more details.
 
-## Latest Release: 0.1.0
+## Latest Release: 0.1.1
 
-This is the first official release of ``PyCytoData`` with LTS.
+This is a minor release with various bug fixes and documentation improvents.
 
 ### Bug Fixes
 
-- Fix the default cofactor of ``PyCytoData.preprocess``
-- Fix lineage channels for ``levine32`` and ``samusik``
+- Fixed a potential issue with loading benchmark datasets' samples out of order (This behavior is not guaranteed, but a implementation detail)
+- Fixed an issue with ``DataLoader.load_dataset`` not recognizing downloaded datasets
+- Fixed an issue with ``preprocess.bead_normalization`` having uninitialized array (#9)
 
 ### Changes and New Features
 
-- ``PyCytoData.run_dr_methods`` now runs on lineage channels only
-- Add tutorials and references for documentation
-- Improve docstrings and general documentations
-- Add preprocessing options for loading benchmark datasets
-- Relax ``numpy`` dependency to >=1.20
-- Add descriptors for PyPI releases
-
-### Deprecations
-
-- Permanently remove ``FileIO.make_dir`` function for safety reasons
+- No new feature added
+- Improved documentations with streamlined front page and updated links
+- Added docstrings for `+` and `+=` operators
+- Updated references for CytofDR paper publication in Nature Communications
 
 
 ## References
 
-If you use ``PyCytoData`` to perform DR, citing the [our DR Review paper](https://doi.org/10.1101/2022.04.26.489549) is highly appreciated:
-
-```
-@article {Wang2022.04.26.489549,
-	author = {Wang, Kaiwen and Yang, Yuqiu and Wu, Fangjiang and Song, Bing and Wang, Xinlei and Wang, Tao},
-	title = {Comparative Analysis of Dimension Reduction Methods for Cytometry by Time-of-Flight Data},
-	elocation-id = {2022.04.26.489549},
-	year = {2022},
-	doi = {10.1101/2022.04.26.489549},
-	publisher = {Cold Spring Harbor Laboratory},
-	URL = {https://www.biorxiv.org/content/early/2022/06/02/2022.04.26.489549},
-	eprint = {https://www.biorxiv.org/content/early/2022/06/02/2022.04.26.489549.full.pdf},
-	journal = {bioRxiv}
-}
-```
-
-If you use ``Cytomulate`` with this package, [our paper](https://doi.org/10.1101/2022.06.14.496200) can be cited here:
+If you used ``PyCytoData`` in your research or with ``Cytomulate`` as part of the pipeline, please cite [our paper](https://doi.org/10.1101/2022.06.14.496200) here:
 
 ```
 @article {Yang2022.06.14.496200,
 	author = {Yang, Yuqiu and Wang, Kaiwen and Lu, Zeyu and Wang, Tao and Wang, Xinlei},
 	title = {Cytomulate: Accurate and Efficient Simulation of CyTOF data},
 	elocation-id = {2022.06.14.496200},
 	year = {2022},
@@ -212,8 +193,29 @@
 	publisher = {Cold Spring Harbor Laboratory},
 	URL = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200},
 	eprint = {https://www.biorxiv.org/content/early/2022/06/16/2022.06.14.496200.full.pdf},
 	journal = {bioRxiv}
 }
 ```
 
+If you use ``PyCytoData`` to perform DR, citing the [our DR Review paper](https://doi.org/10.1038/s41467-023-37478-w) is highly appreciated:
+
+```
+Wang, K., Yang, Y., Wu, F. et al. Comparative analysis of dimension reduction methods for cytometry by time-of-flight data. Nat Commun 14, 1836 (2023). https://doi.org/10.1038/s41467-023-37478-w
+```
+
+or
+
+```
+@article{wang2023comparative,
+  title={Comparative analysis of dimension reduction methods for cytometry by time-of-flight data},
+  author={Wang, Kaiwen and Yang, Yuqiu and Wu, Fangjiang and Song, Bing and Wang, Xinlei and Wang, Tao},
+  journal={Nature communications},
+  volume={14},
+  number={1},
+  pages={1--18},
+  year={2023},
+  publisher={Nature Publishing Group UK London}
+}
+```
+
 If you use the builtin datasets, please visit our [Reference Page](https://pycytodata.readthedocs.io/en/latest/references.html) and cite the papers accordingly.
```

### Comparing `PyCytoData-0.1.0/setup.py` & `PyCytoData-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 import shutil
 import distutils.cmd
 
 from typing import List
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 class PypiCommand(distutils.cmd.Command):
     
     description = "Build and upload for PyPi."
     user_options = []
     
     def initialize_options(self):
```

