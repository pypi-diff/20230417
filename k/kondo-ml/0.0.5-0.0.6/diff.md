# Comparing `tmp/kondo_ml-0.0.5.tar.gz` & `tmp/kondo_ml-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kondo_ml-0.0.5.tar", last modified: Tue Apr 11 13:22:41 2023, max compression
+gzip compressed data, was "kondo_ml-0.0.6.tar", last modified: Mon Apr 17 09:26:12 2023, max compression
```

## Comparing `kondo_ml-0.0.5.tar` & `kondo_ml-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.807948 kondo_ml-0.0.5/
--rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.5/LICENSE
--rw-r--r--   0 rueck      (501) staff       (20)      874 2023-04-11 13:22:41.805916 kondo_ml-0.0.5/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)      203 2023-04-11 10:02:29.000000 kondo_ml-0.0.5/README.md
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.772849 kondo_ml-0.0.5/kondo_ml/
--rw-r--r--   0 rueck      (501) staff       (20)      548 2023-04-11 13:22:25.000000 kondo_ml-0.0.5/kondo_ml/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.790703 kondo_ml-0.0.5/kondo_ml/instance_selection/
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.792705 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)     4284 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/datasets.py
--rw-r--r--   0 rueck      (501) staff       (20)    30404 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/linear.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.798341 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/
--rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
--rw-r--r--   0 rueck      (501) staff       (20)    42909 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/SELCON.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/__init__.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.802602 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/
--rw-r--r--   0 rueck      (501) staff       (20)    13606 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
--rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    14724 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
--rw-r--r--   0 rueck      (501) staff       (20)     4355 2023-01-06 11:10:15.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/time_series.py
--rw-r--r--   0 rueck      (501) staff       (20)      894 2023-03-29 14:07:55.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/__init__.py
--rw-r--r--   0 rueck      (501) staff       (20)    21369 2023-04-11 13:03:10.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_drop.py
--rw-r--r--   0 rueck      (501) staff       (20)     5394 2023-04-11 13:03:10.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_fish.py
--rw-r--r--   0 rueck      (501) staff       (20)     1884 2023-03-21 13:25:30.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_fixed_time_window.py
--rw-r--r--   0 rueck      (501) staff       (20)      747 2023-03-27 12:15:14.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_full_set.py
--rw-r--r--   0 rueck      (501) staff       (20)     3292 2023-02-28 20:37:58.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_gradient_shapley.py
--rw-r--r--   0 rueck      (501) staff       (20)      709 2023-02-07 23:08:48.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_local_outlier_factor.py
--rw-r--r--   0 rueck      (501) staff       (20)     2923 2023-03-28 17:07:35.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_mutual_information.py
--rw-r--r--   0 rueck      (501) staff       (20)      755 2023-02-24 21:17:58.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_random_selection.py
--rw-r--r--   0 rueck      (501) staff       (20)     3277 2023-03-28 17:28:54.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_CNN.py
--rw-r--r--   0 rueck      (501) staff       (20)     8480 2023-04-11 13:03:10.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_ENN.py
--rw-r--r--   0 rueck      (501) staff       (20)     1382 2023-03-29 14:30:04.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/_selcon.py
--rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.5/kondo_ml/instance_selection/base.py
--rw-r--r--   0 rueck      (501) staff       (20)      460 2023-03-29 14:04:12.000000 kondo_ml-0.0.5/kondo_ml/kondo_ml.py
--rw-r--r--   0 rueck      (501) staff       (20)     1713 2023-03-21 13:36:29.000000 kondo_ml-0.0.5/kondo_ml/utils.py
-drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-11 13:22:41.776126 kondo_ml-0.0.5/kondo_ml.egg-info/
--rw-r--r--   0 rueck      (501) staff       (20)      874 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/PKG-INFO
--rw-r--r--   0 rueck      (501) staff       (20)     1352 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/SOURCES.txt
--rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/dependency_links.txt
--rw-r--r--   0 rueck      (501) staff       (20)       32 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/requires.txt
--rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-11 13:22:41.000000 kondo_ml-0.0.5/kondo_ml.egg-info/top_level.txt
--rw-r--r--   0 rueck      (501) staff       (20)      620 2023-04-11 13:22:25.000000 kondo_ml-0.0.5/pyproject.toml
--rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-11 13:22:41.808144 kondo_ml-0.0.5/setup.cfg
--rw-r--r--   0 rueck      (501) staff       (20)     1874 2023-04-11 10:45:56.000000 kondo_ml-0.0.5/setup.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 09:26:12.445496 kondo_ml-0.0.6/
+-rw-r--r--   0 rueck      (501) staff       (20)     1062 2023-03-06 04:08:33.000000 kondo_ml-0.0.6/LICENSE
+-rw-r--r--   0 rueck      (501) staff       (20)      876 2023-04-17 09:26:12.444889 kondo_ml-0.0.6/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)      205 2023-04-17 09:22:08.000000 kondo_ml-0.0.6/README.md
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 09:26:12.425380 kondo_ml-0.0.6/kondo_ml/
+-rw-r--r--   0 rueck      (501) staff       (20)      549 2023-04-17 09:21:38.000000 kondo_ml-0.0.6/kondo_ml/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 09:26:12.436936 kondo_ml-0.0.6/kondo_ml/instance_selection/
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 09:26:12.438562 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4281 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/datasets.py
+-rw-r--r--   0 rueck      (501) staff       (20)    30415 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/linear.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 09:26:12.440237 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/model/
+-rw-r--r--   0 rueck      (501) staff       (20)     1182 2023-01-06 11:10:15.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/model/LinearRegression.py
+-rw-r--r--   0 rueck      (501) staff       (20)    42882 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/model/SELCON.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/model/__init__.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 09:26:12.443733 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/
+-rw-r--r--   0 rueck      (501) staff       (20)    13594 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py
+-rw-r--r--   0 rueck      (501) staff       (20)        0 2023-03-29 14:26:05.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    14712 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py
+-rw-r--r--   0 rueck      (501) staff       (20)     4081 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/time_series.py
+-rw-r--r--   0 rueck      (501) staff       (20)      894 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/__init__.py
+-rw-r--r--   0 rueck      (501) staff       (20)    21413 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_drop.py
+-rw-r--r--   0 rueck      (501) staff       (20)     5428 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_fish.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1911 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_fixed_time_window.py
+-rw-r--r--   0 rueck      (501) staff       (20)      774 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_full_set.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3305 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_gradient_shapley.py
+-rw-r--r--   0 rueck      (501) staff       (20)      705 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_local_outlier_factor.py
+-rw-r--r--   0 rueck      (501) staff       (20)     2916 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_mutual_information.py
+-rw-r--r--   0 rueck      (501) staff       (20)      736 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_random_selection.py
+-rw-r--r--   0 rueck      (501) staff       (20)     3311 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_reg_CNN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     8488 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_reg_ENN.py
+-rw-r--r--   0 rueck      (501) staff       (20)     1381 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/_selcon.py
+-rw-r--r--   0 rueck      (501) staff       (20)      859 2023-02-17 14:38:57.000000 kondo_ml-0.0.6/kondo_ml/instance_selection/base.py
+-rw-r--r--   0 rueck      (501) staff       (20)      462 2023-04-17 09:15:49.000000 kondo_ml-0.0.6/kondo_ml/kondo_ml.py
+-rw-r--r--   0 rueck      (501) staff       (20)     2343 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/kondo_ml/utils.py
+drwxr-xr-x   0 rueck      (501) staff       (20)        0 2023-04-17 09:26:12.429056 kondo_ml-0.0.6/kondo_ml.egg-info/
+-rw-r--r--   0 rueck      (501) staff       (20)      876 2023-04-17 09:26:12.000000 kondo_ml-0.0.6/kondo_ml.egg-info/PKG-INFO
+-rw-r--r--   0 rueck      (501) staff       (20)     1352 2023-04-17 09:26:12.000000 kondo_ml-0.0.6/kondo_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        1 2023-04-17 09:26:12.000000 kondo_ml-0.0.6/kondo_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 rueck      (501) staff       (20)       32 2023-04-17 09:26:12.000000 kondo_ml-0.0.6/kondo_ml.egg-info/requires.txt
+-rw-r--r--   0 rueck      (501) staff       (20)        9 2023-04-17 09:26:12.000000 kondo_ml-0.0.6/kondo_ml.egg-info/top_level.txt
+-rw-r--r--   0 rueck      (501) staff       (20)      620 2023-04-17 09:22:08.000000 kondo_ml-0.0.6/pyproject.toml
+-rw-r--r--   0 rueck      (501) staff       (20)       38 2023-04-17 09:26:12.445681 kondo_ml-0.0.6/setup.cfg
+-rw-r--r--   0 rueck      (501) staff       (20)     1605 2023-04-17 09:18:30.000000 kondo_ml-0.0.6/setup.py
```

### Comparing `kondo_ml-0.0.5/LICENSE` & `kondo_ml-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.5/PKG-INFO` & `kondo_ml-0.0.6/kondo_ml.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: kondo_ml
-Version: 0.0.5
+Name: kondo-ml
+Version: 0.0.6
 Summary: Python package for instance selection algorithms
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.5.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.6.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kondo-ML
 
 kondo-ML is a package containing various instance selection algorithms
-usable with regression modelsThe implementations are compatible with sklearn and follow
+usable with regression models. The implementations are compatible with sklearn and follow
 its outlier detection interface.
```

### Comparing `kondo_ml-0.0.5/kondo_ml/__init__.py` & `kondo_ml-0.0.6/kondo_ml/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from kondo_ml.kondo_ml import KondoMLPackage
 
-__author__ = 'Lukas Rücker'
-__email__ = 'ruecker.lukas@gmail.com'
-__version__ = '0.0.5'
+__author__ = "Lukas Rücker"
+__email__ = "ruecker.lukas@gmail.com"
+__version__ = "0.0.6"
 
 # module level doc-string
 __doc__ = """
 Kondo-ML
 ================
 
 Description
 -----------
 Kondo-ML is a Python package to gather instance selection algorithms for regression problems.
 The package was created as a byproduct to my master's thesis. The name Kondo is referring to 
 Marie Kondo. The idea is that with the instance selection only those instances are kept
 that spark joy in the model (the user).
 
 
-"""
+"""
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/datasets.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import copy
 import datetime
 import os
 import subprocess
 import sys
 import time
 
-import torch
-
 import numpy as np
+import torch
 
 from kondo_ml.instance_selection.SELCON.utils.Create_Slices import get_slices
 from kondo_ml.instance_selection.SELCON.utils.custom_dataset import (
-    load_dataset_custom,
-    load_std_regress_data,
-)
-from kondo_ml.instance_selection.SELCON.utils.time_series import load_time_series_data
+    load_dataset_custom, load_std_regress_data)
+from kondo_ml.instance_selection.SELCON.utils.time_series import \
+    load_time_series_data
 
 torch.manual_seed(42)
 np.random.seed(42)
 device = "cuda" if torch.cuda.is_available() else "cpu"
 # device = "cpu"
 print("Using Device:", device)
 
@@ -51,15 +49,14 @@
         )
         x_tst, y_tst = (
             torch.from_numpy(testset[0]).float(),
             torch.from_numpy(testset[1]).float(),
         )
 
     elif data_name in ["Community_Crime", "census", "LawSchool"]:
-
         datadir = datadir + "/" + data_name + "/"
 
         fullset, data_dims = load_dataset_custom(datadir, data_name, True)
 
         if data_name == "Community_Crime":
             (
                 x_trn,
@@ -132,12 +129,11 @@
             torch.from_numpy(testset[1]).float(),
         )
 
     return (x_trn, y_trn), (x_val, y_val), (x_tst, y_tst)
 
 
 def get_data(x_train, x_val, y_train, y_val):
-
     x_trn, y_trn = torch.from_numpy(x_train).float(), torch.from_numpy(y_train).float()
     x_val, y_val = torch.from_numpy(x_val).float(), torch.from_numpy(y_val).float()
 
     return x_trn, x_val, y_trn, y_val
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/linear.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import copy
 import time
 
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from torch.utils.data import DataLoader
 
-import numpy as np
-
-from kondo_ml.instance_selection.SELCON.model.LinearRegression import RegressionNet
-from kondo_ml.instance_selection.SELCON.model.SELCON import (
-    FindSubset_Vect_No_ValLoss as FindSubset_Vect,
-)
-from kondo_ml.instance_selection.SELCON.model.SELCON import FindSubset_Vect_TrnLoss
-from kondo_ml.instance_selection.SELCON.utils.custom_dataset import CustomDataset
+from kondo_ml.instance_selection.SELCON.model.LinearRegression import \
+    RegressionNet
+from kondo_ml.instance_selection.SELCON.model.SELCON import \
+    FindSubset_Vect_No_ValLoss as FindSubset_Vect
+from kondo_ml.instance_selection.SELCON.model.SELCON import \
+    FindSubset_Vect_TrnLoss
+from kondo_ml.instance_selection.SELCON.utils.custom_dataset import \
+    CustomDataset
 
 torch.manual_seed(42)
 np.random.seed(42)
 
 
 class Regression:
     def __init__(self):
@@ -52,15 +53,14 @@
         delt=[0.3],
         x_tst=None,
         y_tst=None,
         num_epochs=2000,
         default=False,
         ebud=None,
     ):
-
         sub_epoch = 3
 
         N, M = x_trn.shape
         bud = int(fraction * N)
         print("Budget, fraction and N:", bud, fraction, N)
         train_batch_size = min(bud, 1000)
         print_every = 50
@@ -158,19 +158,17 @@
         prev_loss = 1000
         prev_loss2 = 1000
         i = 0
         mul = 1
         lr_count = 0
 
         for i in range(num_epochs):
-
             temp_loss = 0.0
 
             for batch_idx in list(loader_tr.batch_sampler):
-
                 inputs, targets = loader_tr.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
                 main_optimizer.zero_grad()
 
                 scores = main_model(inputs)
 
                 l2_reg = 0
@@ -204,15 +202,14 @@
                     "\n",
                     "Mul: ",
                     mul,
                 )
                 # print(main_optimizer.param_groups[0]['lr'])
 
             if (i + 1) % self.select_every == 0:
-
                 cached_state_dict = copy.deepcopy(main_model.state_dict())
                 clone_dict = copy.deepcopy(cached_state_dict)
 
                 fsubset_d.lr = main_optimizer.param_groups[0]["lr"] * mul  # ,1e-4)
 
                 state_values = list(main_optimizer.state.values())
                 step = state_values[0]["step"]
@@ -315,18 +312,16 @@
         print("Subset_fair", len(idxs))
         # print(flat)
         self.subset_idx = (
             idxs  # ADDED BY ME, BECAUSE NO self.subset_idx was in this function
         )
 
         with torch.no_grad():
-
             # self.val_loss = 0.
             for batch_idx in list(loader_val.batch_sampler):
-
                 inputs, targets = loader_val.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 val_out = main_model(inputs)
                 """if is_time:
                     val_out = sc_trans.inverse_transform(val_out.cpu().numpy())
                     val_out = torch.from_numpy(val_out).float()"""
@@ -339,23 +334,21 @@
                     e_val_loss = torch.cat((e_val_loss, batch_val_loss), dim=0)
 
             # val_loss /= len(loader_val.batch_sampler)
             self.val_loss = torch.mean(e_val_loss)
             # print(list(e_val_loss.cpu().numpy()))
 
             if default == True:
-
                 loader_tst = DataLoader(
                     CustomDataset(x_tst, y_tst, transform=None),
                     shuffle=False,
                     batch_size=self.batch_size,
                 )
 
                 for batch_idx in list(loader_tst.batch_sampler):
-
                     inputs, targets = loader_tst.dataset[batch_idx]
                     inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                     outputs = main_model(inputs)
                     """if is_time:
                         outputs = sc_trans.inverse_transform(outputs.cpu().numpy())
                         outputs = torch.from_numpy(outputs).float()"""
@@ -384,15 +377,14 @@
         delt=[0.3],
         x_tst=None,
         y_tst=None,
         num_epochs=2000,
         default=False,
         bud=None,
     ):
-
         sub_epoch = 3
 
         N, M = x_trn.shape
         bud = int(fraction * N)
         print("Budget, fraction and N:", bud, fraction, N)
         train_batch_size = min(bud, 1000)
         print_every = 50
@@ -516,24 +508,22 @@
         prev_loss = 1000
         prev_loss2 = 1000
         i = 0
         mul = 1
         lr_count = 0
         # while (True):
         for i in range(num_epochs):
-
             # inputs, targets = x_trn[idxs].to(self.device), y_trn[idxs].to(self.device)
             # inputs, targets = x_trn[sub_idxs], y_trn[sub_idxs]
 
             temp_loss = 0.0
 
             starting = time.process_time()
 
             for batch_idx_t in list(loader_tr.batch_sampler):
-
                 inputs_trn, targets_trn = loader_tr.dataset[batch_idx_t]
                 inputs_trn, targets_trn = inputs_trn.to(self.device), targets_trn.to(
                     self.device
                 )
 
                 main_optimizer.zero_grad()
 
@@ -559,15 +549,14 @@
 
                     inputs_j, targets_j = x_val_list[j], y_val_list[j]
                     scores_j = main_model(inputs_j)
                     constraint[j] = criterion(scores_j, targets_j) - deltas[j]"""
 
                 constraint = 0.0
                 for batch_idx in list(loader_val.batch_sampler):
-
                     inputs, targets = loader_val.dataset[batch_idx]
                     inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                     val_out = main_model(inputs)
                     """if is_time:
                         val_out = sc_trans.inverse_transform(val_out.cpu().numpy())
                         val_out = torch.from_numpy(val_out).float()"""
@@ -603,15 +592,14 @@
                 alphas.requires_grad = True"""
 
                 dual_optimizer.zero_grad()
 
                 # if constraint > 0:
                 constraint = 0.0
                 for batch_idx in list(loader_val.batch_sampler):
-
                     inputs, targets = loader_val.dataset[batch_idx]
                     inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                     val_out = main_model(inputs)
                     """if is_time:
                         val_out = sc_trans.inverse_transform(val_out.cpu().numpy())
                         val_out = torch.from_numpy(val_out).float()"""
@@ -658,15 +646,14 @@
                 )
                 # print(main_optimizer.state)#.keys())
                 # print(alphas,constraint)
                 # print(criterion(scores, targets) , reg_lambda*l2_reg*len(idxs) ,multiplier)
                 # print(main_optimizer.param_groups)#[0]['lr'])
 
             if (i + 1) % self.select_every == 0:
-
                 cached_state_dict = copy.deepcopy(main_model.state_dict())
                 clone_dict = copy.deepcopy(cached_state_dict)
 
                 alpha_orig = alphas.detach().clone()  # copy.deepcopy(alphas)
 
                 """alpha_orig.requires_grad = False
                 alpha_orig = alpha_orig*((constraint >0).float())
@@ -812,19 +799,19 @@
         # print(flat,file=modelfile)
 
         with torch.no_grad():
             """full_trn_out = main_model(x_trn)
             full_trn_loss = criterion(full_trn_out, y_trn)
             sub_trn_out = main_model(x_trn[idxs])
             sub_trn_loss = criterion(sub_trn_out, y_trn[idxs])
-            print("\nFinal SubsetTrn and FullTrn Loss:", sub_trn_loss.item(),full_trn_loss.item(),file=logfile)"""
+            print("\nFinal SubsetTrn and FullTrn Loss:", sub_trn_loss.item(),full_trn_loss.item(),file=logfile)
+            """
 
             # val_loss = 0.
             for batch_idx in list(loader_val.batch_sampler):
-
                 inputs, targets = loader_val.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 val_out = main_model(inputs)
                 """if is_time:
                     val_out = sc_trans.inverse_transform(val_out.cpu().numpy())
                     val_out = torch.from_numpy(val_out).float()"""
@@ -838,15 +825,14 @@
 
             # val_loss /= len(loader_val.batch_sampler)
             self.val_loss = torch.mean(e_val_loss)
             # print(list(e_val_loss.cpu().numpy()),file=modelfile)
 
             if default == True:
                 for batch_idx in list(loader_tst.batch_sampler):
-
                     inputs, targets = loader_tst.dataset[batch_idx]
                     inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                     outputs = main_model(inputs)
                     """if is_time:
                         outputs = sc_trans.inverse_transform(outputs.cpu().numpy())
                         outputs = torch.from_numpy(outputs).float()"""
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/LinearRegression.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/model/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/model/SELCON.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/model/SELCON.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import math
 
+import numpy as np
 import torch
 from torch.utils.data import DataLoader
 
-import numpy as np
-
-from kondo_ml.instance_selection.SELCON.utils.custom_dataset import CustomDataset, CustomDataset_WithId
+from kondo_ml.instance_selection.SELCON.utils.custom_dataset import (
+    CustomDataset, CustomDataset_WithId)
 
 
 class FindSubset_Vect_No_ValLoss(object):
     def __init__(
         self, x_trn, y_trn, x_val, y_val, model, loss, device, delta, lr, lam, batch
     ):
-
         self.x_trn = x_trn
         self.y_trn = y_trn
         # self.trn_batch = trn_batch
 
         self.x_val = x_val
         self.y_val = y_val
 
@@ -62,28 +61,26 @@
         # for i in range(f_pi_epoch):
 
         prev_loss = 1000
         stop_count = 0
         i = 0
 
         while True:
-
             main_optimizer.zero_grad()
 
             """l2_reg = 0
             for param in self.model.parameters():
                 l2_reg += torch.norm(param)"""
 
             # l = [torch.flatten(p) for p in main_model.parameters()]
             # flat = torch.cat(l)
             # l2_reg = torch.sum(flat*flat)
 
             constraint = 0.0
             for batch_idx in list(loader_val.batch_sampler):
-
                 inputs, targets = loader_val.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 val_out = self.model(inputs)
                 constraint += self.criterion(val_out, targets)
 
             constraint /= len(loader_val.batch_sampler)
@@ -101,15 +98,14 @@
                 param.requires_grad = False
             alphas.requires_grad = True"""
 
             dual_optimizer.zero_grad()
 
             constraint = 0.0
             for batch_idx in list(loader_val.batch_sampler):
-
                 inputs, targets = loader_val.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 val_out = self.model(inputs)
                 constraint += self.criterion(val_out, targets)
 
             constraint /= len(loader_val.batch_sampler)
@@ -190,15 +186,14 @@
         loader_val = DataLoader(
             CustomDataset(self.x_val, self.y_val, device=self.device, transform=None),
             shuffle=False,
             batch_size=self.batch_size * 20,
         )
 
         for batch_idx in list(loader_tr.batch_sampler):
-
             inputs, targets, idxs = loader_tr.dataset[batch_idx]
             inputs, targets = inputs.to(self.device), targets.to(self.device)
 
             ele_delta = self.delta.repeat(targets.shape[0]).to(self.device)
 
             weights = flat.view(1, -1).repeat(targets.shape[0], 1)
             ele_alphas = alphas.detach().repeat(targets.shape[0]).to(self.device)
@@ -215,15 +210,14 @@
                 dim=1,
             )
 
             bias_correction1 = 1.0
             bias_correction2 = 1.0
 
             for i in range(p_epoch):
-
                 trn_loss_g = torch.sum(exten_inp * weights, dim=1) - targets
                 fin_trn_loss_g = exten_inp * 2 * trn_loss_g[:, None]
 
                 # no_bias = weights.clone()
                 # no_bias[-1,:] = torch.zeros(weights.shape[0])
 
                 weight_grad = fin_trn_loss_g + 2 * self.lam * torch.cat(
@@ -246,15 +240,14 @@
                     * math.sqrt(1.0 - bias_correction2)
                     / (1.0 - bias_correction1)
                 )
                 weights.addcdiv_(-step_size, exp_avg_w, denom)
 
             val_losses = 0.0
             for batch_idx_val in list(loader_val.batch_sampler):
-
                 inputs_val, targets_val = loader_val.dataset[batch_idx_val]
                 inputs_val, targets_val = inputs_val.to(self.device), targets_val.to(
                     self.device
                 )
 
                 exten_val = torch.cat(
                     (
@@ -304,15 +297,14 @@
         batch,
         step,
         w_exp_avg,
         w_exp_avg_sq,
         a_exp_avg,
         a_exp_avg_sq,
     ):
-
         m_values = self.F_values.detach().clone()  # torch.zeros(len(self.x_trn))
 
         self.model.load_state_dict(theta_init)
 
         loader_tr = DataLoader(
             CustomDataset_WithId(
                 self.x_trn[curr_subset], self.y_trn[curr_subset], transform=None
@@ -326,19 +318,17 @@
             shuffle=False,
             batch_size=batch,
         )
 
         sum_error = torch.nn.MSELoss(reduction="sum")
 
         with torch.no_grad():
-
             F_curr = 0.0
 
             for batch_idx in list(loader_tr.batch_sampler):
-
                 inputs, targets, _ = loader_tr.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 scores = self.model(inputs)
                 # print(self.criterion(scores, targets).item())
 
                 F_curr += sum_error(scores, targets).item()
@@ -348,15 +338,14 @@
 
             l = [torch.flatten(p) for p in self.model.parameters()]
             flatt = torch.cat(l)
             l2_reg = torch.sum(flatt[:-1] * flatt[:-1])
 
             valloss = 0.0
             for batch_idx in list(loader_val.batch_sampler):
-
                 inputs, targets = loader_val.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 scores = self.model(inputs)
                 valloss += self.criterion(scores, targets).item()
 
             constraint = valloss / len(loader_val.batch_sampler) - self.delta
@@ -393,15 +382,14 @@
         rem_len = len(curr_subset) - 1
 
         b_idxs = 0
 
         device_new = self.device  # "cuda:2" #self.device #
 
         for batch_idx in list(loader_tr.batch_sampler):
-
             inputs, targets, _ = loader_tr.dataset[batch_idx]
             inputs, targets = inputs.to(self.device), targets.to(self.device)
 
             ele_delta = self.delta.repeat(targets.shape[0]).to(self.device)
 
             weights = flat.repeat(targets.shape[0], 1)
             ele_alphas = alphas.detach().repeat(targets.shape[0]).to(self.device)
@@ -425,19 +413,17 @@
                 dim=1,
             )
 
             bias_correction1 = beta1**step  # 1.0
             bias_correction2 = beta2**step  # 1.0
 
             for i in range(p_epoch):
-
                 fin_val_loss_g = torch.zeros_like(weights).to(device_new)
                 # val_losses = torch.zeros_like(ele_delta).to(device_new)
                 for batch_idx_val in list(loader_val.batch_sampler):
-
                     inputs_val, targets_val = loader_val.dataset[batch_idx_val]
                     inputs_val, targets_val = inputs_val.to(
                         self.device
                     ), targets_val.to(self.device)
 
                     exten_val = torch.cat(
                         (
@@ -483,15 +469,14 @@
                     torch.cuda.empty_cache()
 
                 fin_val_loss_g /= len(loader_val.batch_sampler)
                 fin_val_loss_g = fin_val_loss_g.to(self.device)
 
                 sum_fin_trn_loss_g = torch.zeros_like(weights).to(device_new)
                 for batch_idx_trn in list(loader_tr.batch_sampler):
-
                     inputs_trn, targets_trn, _ = loader_tr.dataset[batch_idx_trn]
                     inputs_trn, targets_trn = inputs_trn.to(
                         self.device
                     ), targets_trn.to(self.device)
 
                     exten_trn = torch.cat(
                         (
@@ -575,15 +560,14 @@
                 """print(self.lr)
                 print((fin_trn_loss_g+ 2*self.lam*weights +fin_val_loss_g*ele_alphas[:,None])[0])"""
 
                 # print(weights[0])
 
                 val_losses = torch.zeros_like(ele_delta).to(device_new)
                 for batch_idx_val in list(loader_val.batch_sampler):
-
                     inputs_val, targets_val = loader_val.dataset[batch_idx_val]
                     inputs_val, targets_val = inputs_val.to(
                         self.device
                     ), targets_val.to(self.device)
 
                     exten_val = torch.cat(
                         (
@@ -625,15 +609,14 @@
                 ele_alphas[ele_alphas < 0] = 0
                 # print(ele_alphas[0])
 
                 # ele_alphas = ele_alphas + self.lr*(torch.mean(val_loss_p*val_loss_p,dim=0)-ele_delta)
 
             val_losses = 0.0
             for batch_idx_val in list(loader_val.batch_sampler):
-
                 inputs_val, targets_val = loader_val.dataset[batch_idx_val]
                 inputs_val, targets_val = inputs_val.to(self.device), targets_val.to(
                     self.device
                 )
 
                 exten_val = torch.cat(
                     (
@@ -651,15 +634,14 @@
 
                 val_losses += torch.mean(val_loss * val_loss, dim=0)
 
             reg = torch.sum(weights[:, :-1] * weights[:, :-1], dim=1)
 
             trn_losses = 0.0
             for batch_idx_trn in list(loader_tr.batch_sampler):
-
                 inputs_trn, targets_trn, _ = loader_tr.dataset[batch_idx_trn]
                 inputs_trn, targets_trn = inputs_trn.to(self.device), targets_trn.to(
                     self.device
                 )
 
                 exten_trn = torch.cat(
                     (
@@ -707,15 +689,14 @@
         return list(indices.cpu().numpy())
 
 
 class FindSubset_Vect_TrnLoss(object):
     def __init__(
         self, x_trn, y_trn, x_val, y_val, model, loss, device, delta, lr, lam, batch
     ):
-
         self.x_trn = x_trn
         self.y_trn = y_trn
         # self.trn_batch = trn_batch
 
         self.x_val = x_val
         self.y_val = y_val
 
@@ -730,15 +711,14 @@
         self.batch_size = batch
 
         torch.manual_seed(42)
         torch.cuda.manual_seed(42)
         np.random.seed(42)
 
     def precompute(self, f_pi_epoch, p_epoch, alphas):
-
         main_optimizer = torch.optim.Adam(
             [{"params": self.model.parameters()}], lr=self.lr
         )
 
         dual_optimizer = torch.optim.Adam([{"params": alphas}], lr=self.lr)
 
         print("starting Pre compute")
@@ -760,28 +740,26 @@
         # for i in range(f_pi_epoch):
 
         prev_loss = 1000
         stop_count = 0
         i = 0
 
         while True:
-
             main_optimizer.zero_grad()
 
             """l2_reg = 0
             for param in self.model.parameters():
                 l2_reg += torch.norm(param)"""
 
             # l = [torch.flatten(p) for p in main_model.parameters()]
             # flat = torch.cat(l)
             # l2_reg = torch.sum(flat*flat)
 
             constraint = 0.0
             for batch_idx in list(loader_val.batch_sampler):
-
                 inputs, targets = loader_val.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 val_out = self.model(inputs)
                 constraint += self.criterion(val_out, targets)
 
             constraint /= len(loader_val.batch_sampler)
@@ -799,15 +777,14 @@
                 param.requires_grad = False
             alphas.requires_grad = True"""
 
             dual_optimizer.zero_grad()
 
             constraint = 0.0
             for batch_idx in list(loader_val.batch_sampler):
-
                 inputs, targets = loader_val.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 val_out = self.model(inputs)
                 constraint += self.criterion(val_out, targets)
 
             constraint /= len(loader_val.batch_sampler)
@@ -871,15 +848,14 @@
         loader_val = DataLoader(
             CustomDataset(self.x_val, self.y_val, device=self.device, transform=None),
             shuffle=False,
             batch_size=self.batch_size * 20,
         )
 
         for batch_idx in list(loader_tr.batch_sampler):
-
             inputs, targets, idxs = loader_tr.dataset[batch_idx]
             inputs, targets = inputs.to(self.device), targets.to(self.device)
 
             ele_delta = self.delta.repeat(targets.shape[0]).to(self.device)
 
             weights = flat.view(1, -1).repeat(targets.shape[0], 1)
             ele_alphas = alphas.detach().repeat(targets.shape[0]).to(self.device)
@@ -896,15 +872,14 @@
                 dim=1,
             )
 
             bias_correction1 = 1.0
             bias_correction2 = 1.0
 
             for i in range(p_epoch):
-
                 trn_loss_g = torch.sum(exten_inp * weights, dim=1) - targets
                 fin_trn_loss_g = exten_inp * 2 * trn_loss_g[:, None]
 
                 # no_bias = weights.clone()
                 # no_bias[-1,:] = torch.zeros(weights.shape[0])
 
                 weight_grad = fin_trn_loss_g + 2 * self.lam * torch.cat(
@@ -927,15 +902,14 @@
                     * math.sqrt(1.0 - bias_correction2)
                     / (1.0 - bias_correction1)
                 )
                 weights.addcdiv_(-step_size, exp_avg_w, denom)
 
             val_losses = 0.0
             for batch_idx_val in list(loader_val.batch_sampler):
-
                 inputs_val, targets_val = loader_val.dataset[batch_idx_val]
                 inputs_val, targets_val = inputs_val.to(self.device), targets_val.to(
                     self.device
                 )
 
                 exten_val = torch.cat(
                     (
@@ -990,15 +964,14 @@
         curr_subset,
         budget,
         batch,
         step,
         w_exp_avg,
         w_exp_avg_sq,
     ):  # ,alphas,a_exp_avg,a_exp_avg_sq):
-
         m_values = self.F_values.detach().clone()  # torch.zeros(len(self.x_trn))
 
         self.model.load_state_dict(theta_init)
 
         # print(theta_init)
         # print(curr_subset)
 
@@ -1017,19 +990,17 @@
 
         # loader_val = DataLoader(CustomDataset(self.x_val, self.y_val,transform=None),\
         #    shuffle=False,batch_size=batch)
 
         sum_error = torch.nn.MSELoss(reduction="sum")
 
         with torch.no_grad():
-
             F_curr = 0.0
 
             for batch_idx in list(loader_tr.batch_sampler):
-
                 inputs, targets, _ = loader_tr.dataset[batch_idx]
                 inputs, targets = inputs.to(self.device), targets.to(self.device)
 
                 scores = self.model(inputs)
                 # print(self.criterion(scores, targets).item())
 
                 F_curr += sum_error(scores, targets).item()
@@ -1074,15 +1045,14 @@
         rem_len = len(curr_subset) - 1
 
         b_idxs = 0
 
         device_new = self.device  # "cuda:2" #self.device #
 
         for batch_idx in list(loader_tr.batch_sampler):
-
             inputs, targets, _ = loader_tr.dataset[batch_idx]
             inputs, targets = inputs.to(self.device), targets.to(self.device)
 
             # ele_delta = self.delta.repeat(targets.shape[0]).to(self.device)
 
             weights = flat.repeat(targets.shape[0], 1)
             # ele_alphas = alphas.detach().repeat(targets.shape[0]).to(self.device)
@@ -1102,18 +1072,16 @@
                 dim=1,
             )
 
             bias_correction1 = beta1**step  # 1.0
             bias_correction2 = beta2**step  # 1.0
 
             for i in range(p_epoch):
-
                 sum_fin_trn_loss_g = torch.zeros_like(weights).to(device_new)
                 for batch_idx_trn in list(loader_tr.batch_sampler):
-
                     inputs_trn, targets_trn, _ = loader_tr.dataset[batch_idx_trn]
                     inputs_trn, targets_trn = inputs_trn.to(
                         self.device
                     ), targets_trn.to(self.device)
 
                     exten_trn = torch.cat(
                         (
@@ -1187,15 +1155,14 @@
                 )
                 weights.addcdiv_(-step_size, exp_avg_w, denom)
 
             reg = torch.sum(weights[:, :-1] * weights[:, :-1], dim=1)
 
             trn_losses = 0.0
             for batch_idx_trn in list(loader_tr.batch_sampler):
-
                 inputs_trn, targets_trn, _ = loader_tr.dataset[batch_idx_trn]
                 inputs_trn, targets_trn = inputs_trn.to(self.device), targets_trn.to(
                     self.device
                 )
 
                 exten_trn = torch.cat(
                     (
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/Create_Slices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import torch
-
 import numpy as np
-
+import torch
 from sklearn import preprocessing
 from sklearn.preprocessing import MinMaxScaler, StandardScaler
 
 """def gen_rand_prior_indices(curr_size,num_cls,x_trn,y_trn,remainList=None):
 
     per_sample_budget = int(curr_size/num_cls)
     if remainList is None:
@@ -31,15 +29,14 @@
     for i in indices:
         total_set.remove(i)
     indices.extend(list(np.random.choice(total_set, size= count, replace=False)))
     return indices"""
 
 
 def get_slices(data_name, data, labels, device, buckets=None, clean=True):
-
     # data_slices = []
     # abel_slices =[]
 
     val_data_slices = []
     val_label_slices = []
 
     tst_data_slices = []
@@ -56,29 +53,27 @@
         data_class = []
 
         N = int(0.1 * len(data) / (buckets * len(protect_feature)))
 
         total_set = set(list(np.arange(len(data))))
 
         for i in protect_feature:
-
             digit = np.ones(data.shape[0], dtype=np.int8) * (i - 1)
             low = np.min(data[:, i])
             high = np.max(data[:, i])
             bins = np.linspace(low, high, buckets)
             digitized = np.digitize(data[:, i], bins)
             digit = digit * 10 + digitized
 
             classes, times = np.unique(digit, return_counts=True)
             times, classes = zip(*sorted(zip(times, classes)))
             data_class.append(classes)
 
             count = 0
             for cl in classes[:-1]:
-
                 indices = []
                 indices_tst = []
 
                 idx = (digit == cl).nonzero()[0].flatten()
                 idx.tolist()
                 idxs = set(idx)
                 idxs.intersection_update(total_set)
@@ -149,15 +144,14 @@
 
         final_lables = [j for sub in data_class for j in sub]
         left = list(total_set)
         data_left = data[left]
         label_left = labels[left]
 
     elif data_name == "OnlineNewsPopularity":
-
         protect_feature = [11, 12, 13, 14, 15, 16]
 
         final_lables = [
             "Lifestyle",
             "Entertainment",
             "Business",
             "Social Media",
@@ -168,15 +162,14 @@
         total_set = set(list(np.arange(len(data))))
 
         N = int(0.1 * len(data) / len(protect_feature))
 
         max_times = 0
 
         for pf in protect_feature:
-
             classes, times = np.unique(data[:, pf], return_counts=True)
 
             one_id = (classes == 1.0).nonzero()[0].flatten()[0]
 
             if max_times < times[one_id]:
                 max_times = times[one_id]
                 max_id = pf
@@ -184,15 +177,14 @@
         most = final_lables[max_id - protect_feature[0]]
         final_lables.remove(most)
         final_lables.append(most)
 
         count = 0
 
         for pf in protect_feature:
-
             if pf == max_id:
                 continue
 
             idx = (data[:, pf] == 1.0).nonzero()[0].flatten()
             idx.tolist()
             idxs = set(idx)
             idxs.intersection_update(total_set)
@@ -261,15 +253,14 @@
         label_left = np.reshape(
             sc_l.fit_transform(np.reshape(labels[left], (-1, 1))), (-1)
         )
         # print(data_left[0])
         # preprocessing.normalize(data[left])
 
         for j in range(len(val_data_slices)):
-
             val_data_slices[j] = (
                 torch.from_numpy(sc.transform(val_data_slices[j])).float().to(device)
             )
             tst_data_slices[j] = (
                 torch.from_numpy(sc.transform(tst_data_slices[j])).float().to(device)
             )
 
@@ -289,15 +280,14 @@
                     )
                 )
                 .float()
                 .to(device)
             )
 
     elif data_name in ["census", "LawSchool", "German_credit", "Community_Crime"]:
-
         if data_name == "census":
             protect_feature = 8  # 9
         elif data_name == "LawSchool":
             protect_feature = 0
         elif data_name == "German_credit":
             protect_feature = 8
         elif data_name == "Community_Crime":
@@ -311,15 +301,14 @@
         # print(times)
         # print(classes)
 
         N = int(0.1 * len(data) / len(classes))
 
         count = 0
         for cl in classes[:-1]:
-
             indices = []
             indices_tst = []
 
             idx = (data[:, protect_feature] == cl).nonzero()[0].flatten()
             idx.tolist()
 
             curr_N = int(len(idx) / 3)
@@ -381,15 +370,14 @@
 
         final_lables = classes
         left = list(total_set)
         data_left = data[left]  # preprocessing.normalize(data[left])
         label_left = labels[left]
 
         if not clean:
-
             noise_size = int(len(label_left) * 0.5)
             noise_indices = np.random.choice(
                 np.arange(len(label_left)), size=noise_size, replace=False
             )
 
             sigma = 40
             label_left[noise_indices] = label_left[noise_indices] + np.random.normal(
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/custom_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import os
 
-import torch
-from torch.utils.data import Dataset
-
 import numpy as np
 import pandas as pd
-
+import torch
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder, StandardScaler
+from torch.utils.data import Dataset
 
 
 ## Custom PyTorch Dataset Class wrapper
 class CustomDataset(Dataset):
     def __init__(self, data, target, device=None, transform=None):
         self.transform = transform
         if device is not None:
@@ -145,15 +143,14 @@
         target_np_path = path + ".label.npy"
         np.save(data_np_path, X_data)
         np.save(target_np_path, Y_label)
     return (X_data, Y_label)
 
 
 def clean_lawschool_full(path):
-
     df = pd.read_csv(path)
     df = df.dropna()
     # remove y from df
     y = df["ugpa"]
     y = y / 4
     df = df.drop("ugpa", 1)
     # convert gender variables to 0,1
@@ -211,15 +208,14 @@
 
     # print(df.head())
 
     return df.to_numpy(), Y.to_numpy()
 
 
 def house_price_load(trn_path, tst_path, save_data=False):
-
     train_csv = pd.read_csv(trn_path)
     test_csv = pd.read_csv(tst_path)
 
     drop_columns = (
         train_csv.isnull()
         .sum()
         .sort_values(ascending=False)
@@ -312,30 +308,28 @@
     return (
         X_train_clean_encoded.to_numpy(),
         trn_y.to_numpy(),
     )  # ,X_test_clean_encoded,tst_y
 
 
 def community_crime_load(path, dim, save_data=False):
-
     data = []
     target = []
     with open(path) as fp:
         line = fp.readline()
         while line:
             temp = [i.strip() for i in line.strip().split(",")][5:]
 
             target.append(float(temp[-1]))
 
             temp_data = [0.0] * dim
 
             # print(temp)
 
             for i in range(len(temp[:-1])):
-
                 if temp[i] != "?":
                     temp_data[i] = float(temp[i])
 
             data.append(temp_data)
             line = fp.readline()
 
     X_data = np.array(data, dtype=np.float32)
@@ -347,42 +341,38 @@
         target_np_path = path + ".label.npy"
         np.save(data_np_path, X_data)
         np.save(target_np_path, Y_label)
     return (X_data, Y_label)
 
 
 def load_dataset_custom(datadir, dset_name, isnumpy=True):
-
     if dset_name == "Community_Crime":
-
         x_trn, y_trn = clean_communities_full(os.path.join(datadir, "communities.csv"))
 
         if isnumpy:
             fullset = (x_trn, y_trn)
 
         else:
             fullset = CustomDataset(x_trn, y_trn)
 
         return fullset, x_trn.shape[1]
 
     elif dset_name == "LawSchool":
-
         x_trn, y_trn = clean_lawschool_full(os.path.join(datadir, "lawschool.csv"))
 
         if isnumpy:
             fullset = (x_trn, y_trn)
 
         else:
             fullset = CustomDataset(x_trn, y_trn)
 
         return fullset, x_trn.shape[1]
 
 
 def load_std_regress_data(datadir, dset_name, isnumpy=True, clean=True):
-
     if dset_name == "cadata":
         trn_file = os.path.join(datadir, "cadata.txt")
         x_trn, y_trn = libsvm_file_load(trn_file, 8)
 
     elif dset_name == "abalone":
         trn_file = os.path.join(datadir, "abalone_scale.txt")
         x_trn, y_trn = libsvm_file_load(trn_file, 8)
@@ -405,15 +395,14 @@
 
     elif dset_name == "house_pricing":
         trn_file = os.path.join(datadir, "train.csv")
         test_file = os.path.join(datadir, "test.csv")
         x_trn, y_trn = house_price_load(trn_file, test_file)  # ,x_tst,y_tst
 
     elif dset_name == "synthetic":
-
         data_dims = 30  # 100
         samples = 5000  # 1000000
 
         np.random.seed(42)
 
         avg = np.zeros(data_dims)
         cov = np.identity(data_dims)
@@ -440,15 +429,14 @@
             x_trn, y_trn, test_size=0.1, random_state=42
         )
         x_trn, x_val, y_trn, y_val = train_test_split(
             x_trn, y_trn, test_size=0.1, random_state=42
         )
 
     if not clean:
-
         noise_size = int(len(y_trn) * 0.5)
         noise_indices = np.random.choice(
             np.arange(len(y_trn)), size=noise_size, replace=False
         )
 
         sigma = 40
         y_trn[noise_indices] = y_trn[noise_indices] + np.random.normal(
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/SELCON/utils/time_series.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/SELCON/utils/time_series.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 import os
 
-import torch
-import torchvision
-from matplotlib import pyplot as plt
-from torch.utils.data import Dataset
-from torchvision import transforms
-
 import numpy as np
 import pandas as pd
-
-from sklearn import datasets, preprocessing
-from sklearn.datasets import make_classification
 from sklearn.model_selection import train_test_split
-from sklearn.preprocessing import MinMaxScaler, OrdinalEncoder, StandardScaler
+from sklearn.preprocessing import MinMaxScaler
 
 
 def process_time_series(datadir, past_length, col_name, name, save_data=True):
-
     x_trn = []
     y_trn = []
 
     path = os.path.join(datadir, "prices-split-adjusted.csv")
 
     prices_split_adjusted = pd.read_csv(path, index_col="date", parse_dates=["date"])
 
@@ -30,15 +20,14 @@
     prices_split_adjusted = prices_split_adjusted[
         ~prices_split_adjusted["symbol"].isin(omit)
     ]
 
     symbol = pd.DataFrame(prices_split_adjusted["symbol"].value_counts())
 
     for sym in symbol.index:
-
         stock = prices_split_adjusted[prices_split_adjusted["symbol"] == sym]
 
         data_len = len(stock.index)
 
         x_trn_slice = np.zeros((data_len - past_length, past_length))
         y_trn_slice = np.zeros(data_len - past_length)
 
@@ -63,30 +52,27 @@
         np.save(data_np_path, finaL_x_trn)
         np.save(target_np_path, finaL_y_trn)
 
     return finaL_x_trn, finaL_y_trn
 
 
 def load_time_series_data(datadir, dset_name, past_length, clean=True):
-
     if os.path.isfile(
         os.path.join(datadir, dset_name + "_" + str(past_length) + ".data.npy")
     ) and os.path.isfile(
         os.path.join(datadir, dset_name + "_" + str(past_length) + ".label.npy")
     ):
-
         x_trn = np.load(
             os.path.join(datadir, dset_name + "_" + str(past_length) + ".data.npy")
         )
         y_trn = np.load(
             os.path.join(datadir, dset_name + "_" + str(past_length) + ".label.npy")
         )
 
     else:
-
         if dset_name == "NY_Stock_exchange_close":
             x_trn, y_trn = process_time_series(datadir, past_length, "close", dset_name)
 
         elif dset_name == "NY_Stock_exchange_open":
             x_trn, y_trn = process_time_series(datadir, past_length, "open", dset_name)
 
         elif dset_name == "NY_Stock_exchange_high":
@@ -101,15 +87,14 @@
         x_trn, y_trn, test_size=0.1, random_state=42
     )
     x_trn, x_val, y_trn, y_val = train_test_split(
         x_trn, y_trn, test_size=0.005, random_state=42
     )
 
     if not clean:
-
         noise_size = int(len(y_trn) * 0.5)
         noise_indices = np.random.choice(
             np.arange(len(y_trn)), size=noise_size, replace=False
         )
 
         sigma = 40
         y_trn[noise_indices] = y_trn[noise_indices] + np.random.normal(
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/__init__.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._drop import DROPRE2RE, DROP2RT, DROP3RE, DROP3RT
+from ._drop import DROP2RT, DROP3RE, DROP3RT, DROPRE2RE
 from ._fish import Fish1Selector, Fish2Selector
 from ._fixed_time_window import FixedTimeSelector
 from ._full_set import FullSetSelector
 from ._gradient_shapley import GradientShapleySelector
 from ._local_outlier_factor import LOFSelector
 from ._mutual_information import MutualInformationSelector
 from ._random_selection import RandomSelector
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_drop.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_drop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
-
 from sklearn.base import BaseEstimator
 from sklearn.metrics import pairwise_distances
 from sklearn.neighbors import NearestNeighbors
 
-from kondo_ml.utils import transform_selector_output_into_mask, train_lr_model
-from ._reg_ENN import RegEnnSelector
-from .base import SelectorMixin
+from kondo_ml.instance_selection import RegEnnSelector
+from kondo_ml.instance_selection.base import SelectorMixin
+from kondo_ml.utils import train_lr_model, transform_selector_output_into_mask
 
 
 class DROPRESuperClass(BaseEstimator, SelectorMixin):
     """
     Class that contain the basic function that DROP variants 2/3 - RE/RT share.
     The algorithm can be found in the paper by Arnaiz-Gonzalez et al.
     https://www.sciencedirect.com/science/article/abs/pii/S0925231216301953
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_fish.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_fish.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 import pandas as pd
-
 from sklearn.base import BaseEstimator
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import euclidean_distances, mean_squared_error
 from sklearn.model_selection import cross_validate
 
+from kondo_ml.instance_selection.base import SelectorMixin
 from kondo_ml.utils import normalize_array, train_lr_model
-from .base import SelectorMixin
 
 
 class Fish1Selector(SelectorMixin, BaseEstimator):
-    """ FISH1 instance selection algorithm from the paper Combining Similarity in Time and Space for
+    """FISH1 instance selection algorithm from the paper Combining Similarity in Time and Space for
     Training Set Formation under Concept Drift by Zliobaite
     https://eprints.bournemouth.ac.uk/18567/1/FISH_journal_preprint.pdf
     """
+
     def __init__(
         self,
         temporal_weight=0.5,
         subsize_frac=1,
     ):
         super().__init__(subsize_frac)
         self.temporal_weight = temporal_weight
@@ -80,23 +80,23 @@
         self.scores = -1 * self.distance_vector
         self.labels = np.ones(self.nr_samples, dtype="int8") * -1
         return self
 
     def predict(self, X, y=None):
         """Predict the labels (1 use for training, -1 rejected) of X that was passed to the fit function
 
-        Parameters
-        ----------
-       X: Ignored
-            Not used, present for API consistency by convention.
-        y: Ignored
-            Not used, present for API consistency by convention.
+         Parameters
+         ----------
+        X: Ignored
+             Not used, present for API consistency by convention.
+         y: Ignored
+             Not used, present for API consistency by convention.
 
-        Returns
-        -------
+         Returns
+         -------
 
         """
         idx_to_pick = np.argsort(self.distance_vector, axis=0).flatten()[
             : self.samples_to_pick
         ]  # pick smallest dist
         self.labels[idx_to_pick] = 1
         return self.labels
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_fixed_time_window.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_fixed_time_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pandas as pd
-
 from sklearn.base import BaseEstimator
 
-from .base import SelectorMixin
+from kondo_ml.instance_selection.base import SelectorMixin
 
 
 class FixedTimeSelector(BaseEstimator, SelectorMixin):
     """Selects samples based on the recency of the sample"""
+
     def __init__(self, subsize_frac=0.5):
         super().__init__(subsize_frac)
 
     def fit(self, X, y=None):
         """
         The time vector needs to be that last column in the X array
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_gradient_shapley.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_gradient_shapley.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
-
 from sklearn.base import BaseEstimator
-from sklearn.metrics import mean_squared_error, r2_score
+from sklearn.metrics import r2_score
 
-from ..model import get_lr_model_random_params
-from .base import SelectorMixin
+from kondo_ml.instance_selection.base import SelectorMixin
+from kondo_ml.utils import get_lr_model_random_params
 
 
 class GradientShapleySelector(SelectorMixin, BaseEstimator):
     def __init__(
         self,
         convergence_error=0.05,
         learning_rate=0.001,
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_local_outlier_factor.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_local_outlier_factor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
-
 from sklearn.base import BaseEstimator
 from sklearn.neighbors import LocalOutlierFactor
 
-from prism_kondo.instance_selection.base import SelectorMixin
+from kondo_ml.instance_selection.base import SelectorMixin
 
 
 class LOFSelector(SelectorMixin, BaseEstimator):
     def __init__(self, nr_of_neighbors=2):
         self.k = nr_of_neighbors
 
     def fit(self, X, y):
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_mutual_information.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_mutual_information.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-from mutual_info.mutual_info import mutual_information
-
 # from sklearn.feature_selection import mutual_info_regression
 import numpy as np
-
+from mutual_info.mutual_info import mutual_information
 from sklearn.base import BaseEstimator
 from sklearn.neighbors import NearestNeighbors
 
-from prism_kondo.instance_selection.base import SelectorMixin
-from prism_kondo.utils import normalize_array
+from kondo_ml.instance_selection.base import SelectorMixin
+from kondo_ml.utils import normalize_array
 
 
 class MutualInformationSelector(SelectorMixin, BaseEstimator):
     """
     Instance Selection bas on the concept of Mutual Information from Information Theory.
     The algorithm is presented in the paper #TODO
     """
+
     def __init__(self, alpha=0.05, nr_of_neighbors=6, subsize_frac=1):
         super().__init__(subsize_frac)
         self.k = nr_of_neighbors
         self.alpha = alpha
 
     def fit(self, X, y):
         """
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_random_selection.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_random_selection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import numpy as np
-
 from sklearn.base import BaseEstimator
-from sklearn.utils import check_random_state
 
-from .base import SelectorMixin
+from kondo_ml.instance_selection.base import SelectorMixin
 
 
 class RandomSelector(SelectorMixin, BaseEstimator):
     def __init__(self, subsize_frac):
         super().__init__(subsize_frac)
 
     def fit(self, X, y=None):
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_CNN.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_reg_CNN.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
-
 from sklearn.base import BaseEstimator
 from sklearn.neighbors import NearestNeighbors
 
-from ..model import train_lr_model
-from .base import SelectorMixin
+from kondo_ml.instance_selection.base import SelectorMixin
+from kondo_ml.utils import train_lr_model
 
 
 class RegCnnSelector(SelectorMixin, BaseEstimator):
     """Adaption of the Condensed Nearest Neighbor Algorithm by (Hart 1968) for Regression. The adaptation
     was presented in the following paper: #TODO . The RegCNN algorithm removes instances that are redundant/very
     similar to instances already added to the subset.
     """
+
     def __init__(self, alpha=0.25, nr_of_neighbors=7, subsize_frac=1):
         super().__init__(subsize_frac=subsize_frac)
         self.k = nr_of_neighbors
         self.alpha = alpha
 
     def fit(self, X, y):
         """
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_reg_ENN.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_reg_ENN.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import numpy as np
 import pandas as pd
 from scipy.special import softmax
-
 from sklearn.base import BaseEstimator
 from sklearn.neighbors import NearestNeighbors
 
-from ..model import train_lr_model
-from kondo_ml.utils import weighted_avg_and_std
-from .base import SelectorMixin
+from kondo_ml.instance_selection.base import SelectorMixin
+from kondo_ml.utils import train_lr_model, weighted_avg_and_std
 
 
 class RegEnnSelector(SelectorMixin, BaseEstimator):
     def __init__(self, alpha: float = 5, nr_of_neighbors: int = 9, subsize_frac=1):
         super().__init__(subsize_frac=subsize_frac)
         self.nr_of_neighbors = nr_of_neighbors
         self.alpha = alpha
@@ -121,14 +119,15 @@
 class RegENNSelectorTime(RegEnnSelector):
     """RegENNTime is an adaption of RegENN, presented by the author of this package.
 
     RegENNTime makes use of a time vector by calculating weights according to the distance of each instance
     to the last (newest) instance in the set. These weights are used to calculate a weighted
     standard deviation which is the basis for the threshold theta and the selection criterion.
     """
+
     def __init__(
         self,
         alpha=5,
         nr_of_neighbors=9,
         subsize_frac=1,
         time_scaling_factor=300,
         distance_measure: str = "linear",
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/_selcon.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/_selcon.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 from sklearn.base import BaseEstimator
 from sklearn.model_selection import train_test_split
 
 from kondo_ml.instance_selection.base import SelectorMixin
 from kondo_ml.instance_selection.SELCON.datasets import get_data
 from kondo_ml.instance_selection.SELCON.linear import Regression
```

### Comparing `kondo_ml-0.0.5/kondo_ml/instance_selection/base.py` & `kondo_ml-0.0.6/kondo_ml/instance_selection/base.py`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.5/kondo_ml/utils.py` & `kondo_ml-0.0.6/kondo_ml/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from sklearn.linear_model import LinearRegression, LassoLarsCV
+from sklearn.linear_model import LassoLarsCV, LinearRegression
 
 
 def convert_recorded_at_to_seconds(datetime_values):
     unix_epoch = np.datetime64(0, "s")
     one_second = np.timedelta64(1, "s")
     return (datetime_values - unix_epoch) / one_second
 
@@ -49,16 +49,36 @@
 
     values, weights -- Numpy ndarrays with the same shape.
     """
     average = np.average(values, weights=weights)
     variance = np.average((values - average) ** 2, weights=weights)
     return (average, np.sqrt(variance))
 
+
 def train_lr_model(X, y, model_type: str = "linear"):
     if model_type == "linear":
         reg = LinearRegression()
     elif model_type == "lasso_lars_cv":
         reg = LassoLarsCV(normalize=False, max_iter=500)
     else:
         raise ValueError(f"{model_type} is not implemented")
     reg.fit(X, y)
-    return reg
+    return reg
+
+
+def get_random_intercept_coef(nr_of_features):
+    rnd_intercept = np.random.normal(0, 2)
+    rnd_coefs = np.random.normal(0, 2, nr_of_features)
+    return (rnd_intercept, rnd_coefs)
+
+
+def get_lr_model_random_params(nr_of_features, model_type="linear"):
+    if model_type == "linear":
+        reg = LinearRegression()
+    elif model_type == "lasso_lars_cv":
+        reg = LassoLarsCV(normalize=False, max_iter=50)
+    else:
+        raise ValueError("we don't have this model")
+    rnd_intercept, rnd_coefs = get_random_intercept_coef(nr_of_features)
+    reg.intercept_ = rnd_intercept
+    reg.coef_ = rnd_coefs
+    return reg
```

### Comparing `kondo_ml-0.0.5/kondo_ml.egg-info/PKG-INFO` & `kondo_ml-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: kondo-ml
-Version: 0.0.5
+Name: kondo_ml
+Version: 0.0.6
 Summary: Python package for instance selection algorithms
 Home-page: https://github.com/lurue101/instance-selection-for-regression
-Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.5.tar.gz
+Download-URL: https://github.com/lurue101/instance-selection-for-regression/archive/0.0.6.tar.gz
 Author: L.Rücker
 Author-email: Lukas Rücker <ruecker.lukas@gmail.com>
 Project-URL: Homepage, https://github.com/lurue101/instance-selection-for-regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # kondo-ML
 
 kondo-ML is a package containing various instance selection algorithms
-usable with regression modelsThe implementations are compatible with sklearn and follow
+usable with regression models. The implementations are compatible with sklearn and follow
 its outlier detection interface.
```

### Comparing `kondo_ml-0.0.5/kondo_ml.egg-info/SOURCES.txt` & `kondo_ml-0.0.6/kondo_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kondo_ml-0.0.5/pyproject.toml` & `kondo_ml-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kondo_ml"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Lukas Rücker", email="ruecker.lukas@gmail.com" },
 ]
 description = "Python package for instance selection algorithms"
 readme = "README.md"
 dependencies = ['numpy','pandas','scikit-learn','torch']
 requires-python = ">=3.7"
```

### Comparing `kondo_ml-0.0.5/setup.py` & `kondo_ml-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,41 @@
-import setuptools
 import re
 
+import setuptools
+
 # Extract the version from the init file.
-VERSIONFILE="kondo_ml/__init__.py"
-getversion = re.search( r"^__version__ = ['\"]([^'\"]*)['\"]", open(VERSIONFILE, "rt").read(), re.M)
+VERSIONFILE = "kondo_ml/__init__.py"
+getversion = re.search(
+    r"^__version__ = ['\"]([^'\"]*)['\"]", open(VERSIONFILE, "rt").read(), re.M
+)
 if getversion:
     new_version = getversion.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['numpy','pandas','scikit-learn','torch'],        # Dependencies
-     python_requires='>=3.10',                                   # Minimum Python version
-     name='kondo_ml',                                  # Package name
-     version=new_version,                                     # Version
-     author="L.Rücker",                                     # Author name
-     author_email="ruecker.lukas@gmail.com",                           # Author mail
-     description="Python package for instance selection algorithms",    # Short package description
-     long_description=long_description,                       # Long package description
-     long_description_content_type="text/markdown",
-     url="https://github.com/lurue101/instance-selection-for-regression",       # Url to your Git Repo
-     download_url = 'https://github.com/lurue101/instance-selection-for-regression/archive/'+new_version+'.tar.gz',
-     packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
-     include_package_data=True,                               # Must be true to include files depicted in MANIFEST.in
-     license_files=["LICENSE"],                               # License file
-     classifiers=[
-         "Programming Language :: Python :: 3",
-         "License :: OSI Approved :: MIT License",
-         "Operating System :: OS Independent",
-     ],
- )
+    install_requires=["numpy", "pandas", "scikit-learn", "torch"],  # Dependencies
+    python_requires=">=3.10",  # Minimum Python version
+    name="kondo_ml",  # Package name
+    version=new_version,  # Version
+    author="L.Rücker",  # Author name
+    author_email="ruecker.lukas@gmail.com",  # Author mail
+    description="Python package for instance selection algorithms",  # Short package description
+    long_description=long_description,  # Long package description
+    long_description_content_type="text/markdown",
+    url="https://github.com/lurue101/instance-selection-for-regression",  # Url to your Git Repo
+    download_url="https://github.com/lurue101/instance-selection-for-regression/archive/"
+    + new_version
+    + ".tar.gz",
+    packages=setuptools.find_packages(),  # Searches throughout all dirs for files to include
+    include_package_data=True,  # Must be true to include files depicted in MANIFEST.in
+    license_files=["LICENSE"],  # License file
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+)
```

