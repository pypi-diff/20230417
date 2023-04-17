# Comparing `tmp/cbig_network_correspondence-0.0.7.tar.gz` & `tmp/cbig_network_correspondence-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbig_network_correspondence-0.0.7.tar", max compression
+gzip compressed data, was "cbig_network_correspondence-0.0.8.tar", max compression
```

## Comparing `cbig_network_correspondence-0.0.7.tar` & `cbig_network_correspondence-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3180 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/README.md
--rw-r--r--   0        0        0     2376 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      490 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/__init__.py
--rw-r--r--   0        0        0    10455 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/compute_overlap_with_atlases.py
--rw-r--r--   0        0        0     2189 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/grab_data_info.py
--rw-r--r--   0        0        0      429 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/load_example.py
--rw-r--r--   0        0        0        0 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/py.typed
--rw-r--r--   0        0        0     5442 2023-04-14 06:06:59.347488 cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/visualize_overlap_lib.py
--rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     3180 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/README.md
+-rw-r--r--   0        0        0     2376 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/__init__.py
+-rw-r--r--   0        0        0    14137 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/compute_overlap_with_atlases.py
+-rw-r--r--   0        0        0     3143 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/grab_data_info.py
+-rw-r--r--   0        0        0      429 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/load_example.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/py.typed
+-rw-r--r--   0        0        0     5430 2023-04-17 09:14:10.650199 cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/visualize_overlap_lib.py
+-rw-r--r--   0        0        0     4657 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.0.8/PKG-INFO
```

### Comparing `cbig_network_correspondence-0.0.7/README.md` & `cbig_network_correspondence-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.0.7/pyproject.toml` & `cbig_network_correspondence-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbig_network_correspondence"
-version = "0.0.7"
+version = "0.0.8"
 description = "A toolbox for exploring network correspondence across atlases"
 authors = [
     "Ruby Kong <roo.cone@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -30,15 +30,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1, <4.0"
 natsort = "^8.3.1"
 numpy = "^1.20.3"
 nibabel = "^5.0.1"
-scipy = "^1.5.3"
+scipy = "^1.9.0"
 seaborn = "^0.11.2"
 gitpython = "^3.1.27"
 
 [tool.poetry.dev-dependencies]
 autoflake = "*"
 black = "*"
 flake8 = "*"
```

### Comparing `cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/compute_overlap_with_atlases.py` & `cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/compute_overlap_with_atlases.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,92 @@
 """"Modules used for calculating overlap between data and atlases"""
 import copy
 from os import path
 from os import listdir
 from natsort import natsorted
 import numpy as np
 import nibabel as nib
-from . import grab_data_info as grab_info
+import grab_data_info as grab_info
+import visualize_overlap_lib as vis
 from scipy.io import loadmat
-import importlib
-importlib.reload(grab_info)
 
 # define path
 PROJECT_PATH = path.dirname(path.abspath(__file__))
 ATLASES_PATH = path.join(PROJECT_PATH, "data", "atlases")
 NETWORK_ASSIGN_PATH = path.join(PROJECT_PATH, "data", "network_assignment")
 RESULTS_PATH = path.join(PROJECT_PATH, "data", "overlap_results")
+NET_NAME_PATH = path.join(PROJECT_PATH, "data", "network_names")
+
 
 class DataParams:
     """
     This defines the parameter structures for a given data
     """
     def __init__(self, config, data_path):
         self.data_path = data_path
         self.project_path = PROJECT_PATH
         self.atlases_path = ATLASES_PATH
         self.network_assign_path = NETWORK_ASSIGN_PATH
         self.config = grab_info.read_config(config)
 
+
 class RefAtlasParams:
     """
     This defines the parameter structures for an existing atlas.
     This atlas is served as the reference atlas.
     """
     def __init__(self, atlas_name):
-        atlas_config = path.join(PROJECT_PATH, "data", "atlas_config", atlas_name)
+        atlas_config = path.join(PROJECT_PATH,
+                                 "data",
+                                 "atlas_config",
+                                 atlas_name)
         self.config = grab_info.read_config(atlas_config)
-        self.data_path = path.join(ATLASES_PATH, self.config.space, self.config.category)
+        self.data_path = path.join(ATLASES_PATH,
+                                   self.config.space,
+                                   self.config.category)
         self.project_path = PROJECT_PATH
         self.atlases_path = ATLASES_PATH
         self.network_assign_path = NETWORK_ASSIGN_PATH
 
+
 class AtlasParams:
     """
     This defines the parameter structures for an existing atlas.
     This atlas is not served as the reference atlas.
     """
     def __init__(self, atlas_name, atlas_space):
-        atlas_config = path.join(PROJECT_PATH, "data", "atlas_config", atlas_name)
+        atlas_config = path.join(PROJECT_PATH,
+                                 "data",
+                                 "atlas_config",
+                                 atlas_name)
         self.config = grab_info.read_config(atlas_config)
-        self.data_path = path.join(ATLASES_PATH, atlas_space, self.config.category)
+        self.data_path = path.join(ATLASES_PATH,
+                                   atlas_space,
+                                   self.config.category)
         self.project_path = PROJECT_PATH
         self.atlases_path = ATLASES_PATH
         self.network_assign_path = NETWORK_ASSIGN_PATH
 
+
 def sort_files(data_path, filename):
     """
     Reads in files under the path and sort the files based on a natural order.
     """
     if path.isdir(data_path):
         allfiles = listdir(data_path)
         files = []
         for eachfile in allfiles:
             if filename in eachfile:
                 files.append(eachfile)
         files_sorted = natsorted(files)
-        files_sorted_full = [path.join(data_path, str(i)) for i in files_sorted]
-        return files_sorted_full
+        files_sorted_res = [path.join(data_path, str(i)) for i in files_sorted]
+    elif path.isfile(data_path):
+        files_sorted_res = [data_path]
+    return files_sorted_res
 
-    if path.isfile(data_path):
-        return [data_path]
 
 def read_file(data_path):
     """
     Reads in data with given path
 
     data_path:
         the location to the data
@@ -80,31 +94,31 @@
 
     if path.isfile(data_path):
         if ".mat" in data_path:
             mat_data = loadmat(data_path)
             mat_data_lh = mat_data.get('lh_labels')
             mat_data_rh = mat_data.get('rh_labels')
             data = np.concatenate((mat_data_lh, mat_data_rh))
-
+        elif ".npy" in data_path:
+            data = np.load(data_path)
         elif ".nii" in data_path:
             nii_img = nib.load(data_path)
             data = nii_img.get_fdata()
 
     return data
 
 
 def read_atlas(params):
     """
     Reads in atlas based on config information
 
     self.project_path = project_path
     self.atlases_path = atlases_path
     self.network_assign_path = network_assign_path
-    
-    params.config: 
+    params.config:
     - params.config.category:
         the categopry of atlas or data
     - params.config.name:
         the name of atlas or data
     - params.config.space:
         the space of atlas or data
     - params.config.type:
@@ -119,66 +133,70 @@
         print('This is a hard parcellation.')
         params.data_path = sort_files(params.data_path, params.config.name)
         data = read_file(params.data_path[0])
         # The hard parcellation is an areal-level parcellation
         # We need to do network assignment based on the povided mapping
         if params.config.netassign:
             datatmp = copy.deepcopy(data)
-            mapfile = path.join(params.network_assign_path, params.config.name + ".mat")
+            mapfile = path.join(params.network_assign_path, params.config.name
+                                + ".mat")
             mapfile_data = loadmat(mapfile)
-            mapping= mapfile_data.get('mapping')
-            for roi in range(1,mapping.shape[1]+1):
+            mapping = mapfile_data.get('mapping')
+            for roi in range(1, mapping.shape[1]+1):
                 data[datatmp == roi] = mapping[0][roi-1]
             print("Finish network assignmeent!")
 
         # For data in the volumetric space
         # Apply cortical mask
         if "mm" in params.config.space:
             corticalmask = path.join(params.project_path, "data",
-                "cortical_masks",
-                params.config.space + ".nii.gz")
+                                     "cortical_masks",
+                                     params.config.space + ".nii.gz")
             mask = read_file(corticalmask)
             data[mask == 0] = 0
 
     elif params.config.type in ('Soft', 'Metric'):
-        print('This is a soft parcellation.')
+        print('This is a soft parcellation or metric data.')
         data = []
         # Read in cortical mask for data in volumetric space
         if "mm" in params.config.space:
             corticalmask = path.join(params.project_path, "data",
-                "cortical_masks",
-                params.config.space + ".nii.gz")
+                                     "cortical_masks",
+                                     params.config.space + ".nii.gz")
             mask = read_file(corticalmask)
         params.data_path = sort_files(params.data_path, params.config.name)
         for curr_data_file in params.data_path:
             curr_data = read_file(curr_data_file)
             # Apply cortical mask
             if "mm" in params.config.space:
                 curr_data[mask == 0] = 0
             # Apply threshold
             if params.config.threshold is not None:
                 th_l = params.config.threshold[0]
-                th_h = params.config.threshold[1]            
-                curr_data = np.where(np.logical_and(curr_data > th_l, curr_data < th_h), 1, 0)
+                th_h = params.config.threshold[1]
+                curr_data = np.where(
+                    np.logical_and(curr_data > th_l, curr_data < th_h), 1, 0)
             data.append(curr_data)
 
     return data
 
+
 def dice_coeff(net1, net2):
     """
     Computes Dice coefficient between two arrays
     """
     intersection = np.sum(net1[net2 == 1])
     coefficient = (2.0 * intersection) / (np.sum(net1) + np.sum(net2))
     return coefficient
 
 
-def compute_overlap(ref_params,other_params):
+def compute_overlap(ref_params, other_params):
     """
-    Computes network overlap between reference data or atlas with another atlas.
+    Computes network overlap between reference data or atlas with
+    another atlas.
     """
     other_params.config.space = copy.deepcopy(ref_params.config.space)
     ref_data = read_atlas(ref_params)
     other_data = read_atlas(other_params)
     if ref_params.config.type == 'Hard':
         # Reference atlas/data is a hard parcellation
         ref_net_uni = np.unique(ref_data.flatten())
@@ -193,76 +211,155 @@
             idx_i = 0
             overlap_val = np.zeros((len(ref_net_uni), len(other_net_uni)))
             for each_ref_net in ref_net_uni:
                 curr_ref_net = ref_data == each_ref_net
                 idx_j = 0
                 for each_other_net in other_net_uni:
                     curr_other_net = other_data == each_other_net
-                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net, curr_other_net)
+                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net,
+                                                           curr_other_net)
                     idx_j = idx_j + 1
                 idx_i = idx_i + 1
         elif other_params.config.type in ('Soft', 'Metric'):
-            other_net_uni = range(0,len(other_data))
+            other_net_uni = range(0, len(other_data))
             idx_i = 0
             overlap_val = np.zeros((len(ref_net_uni), len(other_net_uni)))
             for each_ref_net in ref_net_uni:
                 curr_ref_net = ref_data == each_ref_net
                 idx_j = 0
                 for each_other_net in other_net_uni:
                     curr_other_net = other_data[each_other_net]
-                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net, curr_other_net)
+                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net,
+                                                           curr_other_net)
                     idx_j = idx_j + 1
                 idx_i = idx_i + 1
     elif ref_params.config.type in ('Soft', 'Metric'):
         # Reference atlas/data is a soft parcellation or any metric data
-        ref_net_uni = range(0,len(ref_data))
+        ref_net_uni = range(0, len(ref_data))
         if other_params.config.type == 'Hard':
             # Other atlas is also a hard parcellation
             other_net_uni = np.unique(other_data.flatten())
             # Exclude regions labeled as 0
             other_net_uni = np.setdiff1d(other_net_uni, np.array([0]))
             idx_i = 0
             overlap_val = np.zeros((len(ref_net_uni), len(other_net_uni)))
             for each_ref_net in ref_net_uni:
                 curr_ref_net = ref_data[each_ref_net]
                 idx_j = 0
                 for each_other_net in other_net_uni:
                     curr_other_net = other_data == each_other_net
-                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net, curr_other_net)
+                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net,
+                                                           curr_other_net)
                     idx_j = idx_j + 1
                 idx_i = idx_i + 1
         elif other_params.config.type in ('Soft', 'Metric'):
-            other_net_uni = range(0,len(other_data))
+            other_net_uni = range(0, len(other_data))
             idx_i = 0
             overlap_val = np.zeros((len(ref_net_uni), len(other_net_uni)))
             for each_ref_net in ref_net_uni:
                 curr_ref_net = ref_data[each_ref_net]
                 idx_j = 0
                 for each_other_net in other_net_uni:
                     curr_other_net = other_data[each_other_net]
-                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net, curr_other_net)
+                    overlap_val[idx_i][idx_j] = dice_coeff(curr_ref_net,
+                                                           curr_other_net)
                     idx_j = idx_j + 1
                 idx_i = idx_i + 1
 
     return overlap_val
 
+
 def compute_overlap_data(data_params, atlas_name):
     """
     Computes overlap matrix for a given data and an existing atlas
     """
-    ## Reads in the atlas in the same space as the data
-    atlas_params = AtlasParams(atlas_name,data_params.config.space)
+    # Reads in the atlas in the same space as the data
+    atlas_params = AtlasParams(atlas_name, data_params.config.space)
 
-    ## Compute the overlap matrix between data and the atlas
-    overlap_val = compute_overlap(data_params,atlas_params)
+    # Compute the overlap matrix between data and the atlas
+    overlap_val = compute_overlap(data_params, atlas_params)
 
     return overlap_val
 
+
 def load_overlap_atlases(ref_atlas_name, other_atlas_name):
     """
     Load overlap matrix for any pair of existing atlases
     """
-    overlap_file = path.join(RESULTS_PATH, ref_atlas_name, other_atlas_name + '.mat')
+    overlap_file = path.join(RESULTS_PATH,
+                             ref_atlas_name,
+                             other_atlas_name + '.mat')
     data = loadmat(overlap_file)
     overlap_val = np.array(data.get('overlap'))
 
-    return overlap_val
+    return overlap_val
+
+
+def locate_label_name(params, specify_net_name):
+    """
+    Returns the binarized data for a specific network of an atlas
+    """
+    data = read_atlas(params)
+    network_names = vis.construct_network_name(params.config.name)
+    if specify_net_name in network_names:
+        index = network_names.index(specify_net_name)
+        if params.config.type == 'Hard':
+            net_uni = np.unique(data.flatten())
+            # Exclude regions labeled as 0
+            net_uni = np.setdiff1d(net_uni, np.array([0]))
+            return (data == net_uni[index]).astype(int)
+        else:
+            return np.squeeze(data[index])
+    elif specify_net_name is None and len(data) == 1:
+        return np.squeeze(data)
+    else:
+        print('Please specify a valid network name.')
+        return None
+
+
+def obtain_overlap(ref_params, other_params, ref_net_name, other_net_name):
+    """
+    Computes network overlap between reference network or reference data
+    and a network from another atlas. Reference network will be labeled as 1,
+    other network will be labeled as 2, the overlap area will be labeled as 3.
+    """
+    other_params.config.space = copy.deepcopy(ref_params.config.space)
+    net_data = locate_label_name(ref_params, ref_net_name)
+    other_data = locate_label_name(other_params, other_net_name)
+    other_data[other_data != 0] = 2
+    overlap_data = net_data + other_data
+    return overlap_data
+
+
+def obtain_overlap_data(data_params, atlas_name, atlas_net_name):
+    """
+    Computes network overlap between binarized data and a network from another
+    atlas. The binarized data will be labeled as 1, other network will be
+    labeled as 2, the overlap area will be labeled as 3.
+    """
+    # Reads in the atlas in the same space as the data
+    atlas_params = AtlasParams(atlas_name, data_params.config.space)
+    overlap_data = obtain_overlap(data_params,
+                                  atlas_params,
+                                  data_params.config.name,
+                                  atlas_net_name)
+    return overlap_data
+
+
+def obtain_overlap_atlases(ref_atlas_name, other_atlas_name,
+                           ref_net_name, other_net_name):
+    """
+    Computes network overlap between a network from reference atlas and
+    a network from another atlas. Reference network will be labeled as 1,
+    other network will be labeled as 2, the overlap area will be labeled as 3.
+    """
+    ref_params = RefAtlasParams(ref_atlas_name)
+    other_params = AtlasParams(other_atlas_name, ref_params.config.space)
+    overlap_data = obtain_overlap(ref_params,
+                                  other_params,
+                                  ref_net_name,
+                                  other_net_name)
+    return overlap_data
+
+
+
+
```

### Comparing `cbig_network_correspondence-0.0.7/src/cbig_network_correspondence/visualize_overlap_lib.py` & `cbig_network_correspondence-0.0.8/src/cbig_network_correspondence/visualize_overlap_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,8 @@
     Draw overlap matrix for any pair of existing atlases
     """
     overlap_file = path.join(RESULTS_PATH, ref_atlas_name, other_atlas_name + '.mat')
     data = scipy.io.loadmat(overlap_file)
     overlap_data = np.array(data.get('overlap'))
     draw_overlap_mat(overlap_data, ref_atlas_name, other_atlas_name, minv, maxv, figfile)
         
-            
+
```

### Comparing `cbig_network_correspondence-0.0.7/PKG-INFO` & `cbig_network_correspondence-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbig-network-correspondence
-Version: 0.0.7
+Version: 0.0.8
 Summary: A toolbox for exploring network correspondence across atlases
 Home-page: https://rubykong.github.io/cbig_network_correspondence
 License: MIT
 Author: Ruby Kong
 Author-email: roo.cone@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: gitpython (>=3.1.27,<4.0.0)
 Requires-Dist: natsort (>=8.3.1,<9.0.0)
 Requires-Dist: nibabel (>=5.0.1,<6.0.0)
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
-Requires-Dist: scipy (>=1.5.3,<2.0.0)
+Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: seaborn (>=0.11.2,<0.12.0)
 Project-URL: Documentation, https://rubykong.github.io/cbig_network_correspondence
 Project-URL: Repository, https://github.com/rubykong/cbig_network_correspondence
 Description-Content-Type: text/markdown
 
 # cbig_network_correspondence
```

