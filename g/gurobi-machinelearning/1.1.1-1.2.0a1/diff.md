# Comparing `tmp/gurobi-machinelearning-1.1.1.tar.gz` & `tmp/gurobi-machinelearning-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gurobi-machinelearning-1.1.1.tar", last modified: Fri Apr 14 07:36:15 2023, max compression
+gzip compressed data, was "gurobi-machinelearning-1.2.0a1.tar", last modified: Mon Apr 17 13:54:59 2023, max compression
```

## Comparing `gurobi-machinelearning-1.1.1.tar` & `gurobi-machinelearning-1.2.0a1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.753751 gurobi-machinelearning-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.753751 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 07:36:15.000000 gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-14 07:36:07.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/add_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/_var_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/base_predictor_constr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/get_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/neural_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/submodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/register_user_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/registered_predictors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/base_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/mlpregressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/predictors_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/skgetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:36:15.757751 gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-14 07:36:02.000000 gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.031154 gurobi-machinelearning-1.2.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 13:54:59.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 13:54:51.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/add_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/_var_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/base_predictor_constr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/get_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.035154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/neural_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/submodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/register_user_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/registered_predictors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/base_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/mlpregressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/predictors_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/skgetter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:54:59.039154 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-17 13:54:50.000000 gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/sequential.py
```

### Comparing `gurobi-machinelearning-1.1.1/LICENSE` & `gurobi-machinelearning-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/PKG-INFO` & `gurobi-machinelearning-1.2.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
@@ -26,21 +26,21 @@
 [![Gurobi-forum](https://img.shields.io/badge/Help-Gurobi--Forum-red)](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects)
 
 [![Gurobi](https://raw.githubusercontent.com/Gurobi/gurobi-machinelearning/main/docs/source/_static/image8.png)](https://www.gurobi.com)
 
 
 # Gurobi Machine Learning
 
-Gurobi Machine Learning is an [open-source](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com/en/latest/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
+Gurobi Machine Learning is an [open-source](https://gurobi-machinelearning.readthedocs.io/en/stable/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
 
 The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/) and [PyTorch](https://pytorch.org/). Only neural networks with ReLU activation can be used with these two packages.
 
 # Documentation
 
-The latest user manual is available on [readthedocs](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com/).
+The latest user manual is available on [readthedocs](https://gurobi-machinelearning.readthedocs.io/).
 
 # Contact us
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
 For reporting bugs, issues and feature request please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
```

### Comparing `gurobi-machinelearning-1.1.1/README.md` & `gurobi-machinelearning-1.2.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 [![Gurobi-forum](https://img.shields.io/badge/Help-Gurobi--Forum-red)](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects)
 
 [![Gurobi](https://raw.githubusercontent.com/Gurobi/gurobi-machinelearning/main/docs/source/_static/image8.png)](https://www.gurobi.com)
 
 
 # Gurobi Machine Learning
 
-Gurobi Machine Learning is an [open-source](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com/en/latest/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
+Gurobi Machine Learning is an [open-source](https://gurobi-machinelearning.readthedocs.io/en/stable/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
 
 The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/) and [PyTorch](https://pytorch.org/). Only neural networks with ReLU activation can be used with these two packages.
 
 # Documentation
 
-The latest user manual is available on [readthedocs](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com/).
+The latest user manual is available on [readthedocs](https://gurobi-machinelearning.readthedocs.io/).
 
 # Contact us
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
 For reporting bugs, issues and feature request please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
```

### Comparing `gurobi-machinelearning-1.1.1/pyproject.toml` & `gurobi-machinelearning-1.2.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gurobi-machinelearning"
-version = "1.1.1"
+version = "1.2.0a1"
 description = "package to insert ML models in Gurobi"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="Apache-2.0"}
 keywords = ["mathematical optimization", "gurobi", "scikit-learn", "pytorch", "tensorflow", "ml"]
 authors = [
   {name = "Gurobi Optimization LLC"}
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/PKG-INFO` & `gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
@@ -26,21 +26,21 @@
 [![Gurobi-forum](https://img.shields.io/badge/Help-Gurobi--Forum-red)](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects)
 
 [![Gurobi](https://raw.githubusercontent.com/Gurobi/gurobi-machinelearning/main/docs/source/_static/image8.png)](https://www.gurobi.com)
 
 
 # Gurobi Machine Learning
 
-Gurobi Machine Learning is an [open-source](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com/en/latest/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
+Gurobi Machine Learning is an [open-source](https://gurobi-machinelearning.readthedocs.io/en/stable/meta-license.html) python package to embed trained regression models in a [`gurobipy`](https://pypi.org/project/gurobipy/) model to be solved with the Gurobi solver.
 
 The package currently supports various [scikit-learn](https://scikit-learn.org/stable/) objects. It has limited support for the [Keras](https://keras.io/) API of [TensorFlow](https://www.tensorflow.org/) and [PyTorch](https://pytorch.org/). Only neural networks with ReLU activation can be used with these two packages.
 
 # Documentation
 
-The latest user manual is available on [readthedocs](https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com/).
+The latest user manual is available on [readthedocs](https://gurobi-machinelearning.readthedocs.io/).
 
 # Contact us
 
 For questions related to using Gurobi Machine Learning please use [Gurobi's Forum](https://support.gurobi.com/hc/en-us/community/topics/10373864542609-GitHub-Projects).
 
 For reporting bugs, issues and feature request please
 [open an issue](https://github.com/Gurobi/gurobi-machinelearning/issues).
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_machinelearning.egg-info/SOURCES.txt` & `gurobi-machinelearning-1.2.0a1/src/gurobi_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/__init__.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/_version.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/_version.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from importlib import metadata
 
 try:
     __version__ = metadata.version("gurobi_machinelearning")
 except metadata.PackageNotFoundError:
     __version__ = "dev"
 
-GIT_HASH = "c845d69838e1554a657b0653400c0e710ca774ad"
+GIT_HASH = "411376135a2001b5fcd3f57261b51ab673e94761"
 
 
 def get_versions():
     """Get package version."""
     # Downloaded package with inserted git hash.
     if "Format" not in GIT_HASH:
         git_hash = f"-{GIT_HASH}"
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/add_predictor.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/add_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/exceptions.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/__init__.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/keras/keras.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/keras/keras.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/__init__.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/_var_utils.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/_var_utils.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/base_predictor_constr.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/base_predictor_constr.py`

 * *Files 9% similar despite different names*

```diff
@@ -138,15 +138,17 @@
     def _create_output_vars(self, input_vars, name="out"):
         """May be defined in derived class to create the output variables of predictor."""
         try:
             n_outputs = self._output_shape
         except AttributeError:
             return
         output = self._gp_model.addMVar(
-            (input_vars.shape[0], n_outputs), lb=-gp.GRB.INFINITY, name=name
+            (input_vars.shape[0], n_outputs),
+            lb=-gp.GRB.INFINITY,
+            name=self._name_var(name),
         )
         self._gp_model.update()
         return output
 
     @property
     def _has_solution(self):
         """Returns true if we have a solution."""
@@ -176,18 +178,22 @@
         ...
 
     @abstractmethod
     def _mip_model(self, **kwargs):
         """Makes MIP model for the predictor the sub-class implements."""
         ...
 
-    @staticmethod
-    def _indexed_name(index, name):
+    def _indexed_name(self, index, name):
         index = f"{index}".replace(" ", "")
-        return f"{name}[{index}]"
+        return self._name_var(f"{name}[{index}]")
+
+    def _name_var(self, name):
+        if self._name != "" and not self._no_recording:
+            return name
+        return None
 
     @property
     def output(self):
         """Output variables of embedded predictor.
 
         Returns
         -------
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/get_convertor.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/get_convertor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/__init__.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/activations.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/activations.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,15 +77,18 @@
         layer : AbstractNNLayer
             Layer to which activation is applied.
         """
         output = layer.output
         if hasattr(layer, "coefs"):
             if not hasattr(layer, "mixing"):
                 mixing = layer.gp_model.addMVar(
-                    output.shape, lb=-GRB.INFINITY, vtype=GRB.CONTINUOUS, name="_mix"
+                    output.shape,
+                    lb=-GRB.INFINITY,
+                    vtype=GRB.CONTINUOUS,
+                    name=layer._name_var("mix"),
                 )
                 layer.mixing = mixing
             layer.gp_model.update()
 
             layer.gp_model.addConstr(
                 layer.mixing == layer.input @ layer.coefs + layer.intercept
             )
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/layers.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/layers.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/neuralnet/neural_net.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/neuralnet/neural_net.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/modeling/submodel.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/modeling/submodel.py`

 * *Files 7% similar despite different names*

```diff
@@ -114,34 +114,66 @@
         self._last_callback = None
         self._name = None
         self._model_function = model_function
 
         if not hasattr(self, "_default_name"):
             self._default_name = type(self).__name__
 
+        self.verbose = False
         if "verbose" in kwargs:
             self.verbose = kwargs["verbose"]
-            self._start_time = time()
-        else:
-            self.verbose = False
-
+            self._timer = SubModel._ModelingTimer()
+            print()
+            self._timer.timing(f"Start building formulation for {self._default_name}")
+
+        self._no_recording = False
+        if "no_record" in kwargs:
+            self._no_recording = kwargs["no_record"]
+
+        self._no_debug = False
+        if "no_debug" in kwargs:
+            self._no_debug = kwargs["no_debug"]
         before = self._open(gp_model)
+
+        if self.verbose:
+            self._timer.timing("Model statistics")
+
         self._objects = self._build_submodel(gp_model, *args, **kwargs)
+
+        if self.verbose:
+            self._timer.timing("Built model")
+
         if self._objects is None:
             self._objects = {}
+
         self._close(before, name)
 
+        if self.verbose:
+            print()
+
     def _build_submodel(self, gp_model, *args, **kwargs):
         """Method to be overridden for generating the model in a sub-class.
 
         When using SubModel to wrap a modeling function in a SubModel, the default
         implementation of this method simply calls the modeling function.
         """
         return self._model_function(gp_model, *args, **kwargs)
 
+    class _ModelingTimer:
+        def __init__(self):
+            self.start = time()
+            self.last = self.start
+
+        def timing(self, message: str):
+            current = time()
+            print(
+                f"{message} in {current - self.last:.2f} secs (total: {current - self.start:.2f})."
+            )
+            self.last = current
+
     class _ModelingData:
         """Class for recording modeling data in a gurobipy.Model object."""
 
         def __init__(self):
             self.name_handler = None
 
         def pop_name_handler(self):
@@ -259,70 +291,80 @@
         self._gp_model = gp_model
         try:
             modeling_data = gp_model._modeling_data
         except AttributeError:
             modeling_data = SubModel._ModelingData()
         gp_model._modeling_data = modeling_data
 
-        return (self._modelstats(gp_model), gp_model._modeling_data.pop_name_handler())
+        if self._no_recording:
+            modelstats = None
+        else:
+            modelstats = self._modelstats(gp_model)
+        return (modelstats, gp_model._modeling_data.pop_name_handler())
 
     def _close(self, before, name):
         """Finalize addition of modeling objects to the gurobipy.Model object.
 
         Record all added modeling objects in SubModel and prefix their names.
         """
 
         class NameHandler:
             """Handle automatic name generation in gp.Model."""
 
             def __init__(self):
                 self.name = {}
 
-            def get_name(self, sub: SubModel):
+            def get_name(self, sub: SubModel, name: str):
                 """Return a default name for specified submodel sub."""
-                name = sub.default_name
+                if name is None or name == "":
+                    name = sub.default_name
                 try:
                     num = self.name[name]
+                    self.name[name] = num + 1
+                    return f"{name}{num}"
                 except KeyError:
-                    num = 1
-                self.name[name] = num + 1
-                return f"{name}{num}"
+                    self.name[name] = 0
+                    return name
 
         def prefix_names(gp_model, objs, attr, name):
             """Prefix all modeling object names with name."""
             if len(objs) == 0:
                 return
             object_names = gp_model.getAttr(attr, objs)
             new_names = [f"{name}.{obj_name}" for obj_name in object_names]
             gp_model.setAttr(attr, objs, new_names)
 
         # re-install name handler
         self._gp_model._modeling_data.push_name_handler(before[1])
 
+        if self._no_recording:
+            return
+
         # record all newly added modeling objects
         self._record(self._gp_model, before[0])
 
-        # prefix names of newly created modeling objects
+        name_handler = self._gp_model._modeling_data.name_handler
+        if name_handler is None:
+            name_handler = NameHandler()
+            self._gp_model._modeling_data.push_name_handler(name_handler)
+
         if name != "":
-            if name is None:
-                name_handler = self._gp_model._modeling_data.name_handler
-                if name_handler is None:
-                    name_handler = NameHandler()
-                    self._gp_model._modeling_data.push_name_handler(name_handler)
-                name = name_handler.get_name(self)
+            # prefix names of newly created modeling objects
+            name = name_handler.get_name(self, name)
             self._name = name
-            if self.verbose:
-                gen_time = time() - self._start_time
-                print(f"Added {name} took {gen_time:.2f} seconds.")
             prefix_names(self._gp_model, self.vars, "VarName", name)
             prefix_names(self._gp_model, self.constrs, "ConstrName", name)
             prefix_names(self._gp_model, self.qconstrs, "QCName", name)
             prefix_names(self._gp_model, self.genconstrs, "GenConstrName", name)
             # SOS can't have a name! :-O
             # prefix_names(self._gp_model, self.sos, "SOSName", name)
+        else:
+            name = name_handler.get_name(self, name)
+        if self.verbose:
+            self._timer.timing(f"Added {name}")
 
     def print_stats(self, abbrev=False, file=None):
         """Print statistics about submodel.
 
         This functions prints detailed statistics on the variables
         and constraints that where added to the gp_model using this object.
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/register_user_predictor.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/register_user_predictor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/registered_predictors.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/registered_predictors.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/__init__.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/base_regressions.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/base_regressions.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/column_transformer.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/column_transformer.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,31 +95,38 @@
         nex = _input.shape[0]
 
         outdim = output.shape[1]
         assert (
             outdim == 1
         ), "Output dimension of gradient boosting regressor should be 1"
 
-        treevars = model.addMVar(
-            (nex, predictor.n_estimators_, 1), lb=-GRB.INFINITY, name="estimator"
+        estimators = []
+        if self._no_debug:
+            kwargs["no_record"] = True
+
+        tree_vars = model.addMVar(
+            (nex, predictor.n_estimators_, 1),
+            lb=-GRB.INFINITY,
+            name=self._name_var("esimator"),
         )
-        constant = predictor.init_.constant_
 
-        estimators = []
         for i in range(predictor.n_estimators_):
             tree = predictor.estimators_[i]
+            if self.verbose:
+                self._timer.timing(f"Estimator {i}")
             estimators.append(
                 add_decision_tree_regressor_constr(
-                    model, tree[0], _input, treevars[:, i, :], **kwargs
+                    model, tree[0], _input, tree_vars[:, i, :], **kwargs
                 )
             )
         self.estimators_ = estimators
 
+        constant = predictor.init_.constant_
         model.addConstr(
-            output == predictor.learning_rate * treevars.sum(axis=1) + constant[0][0]
+            output == predictor.learning_rate * tree_vars.sum(axis=1) + constant[0][0]
         )
 
     def print_stats(self, abbrev=False, file=None):
         """Print statistics on model additions stored by this class.
 
         This function prints detailed statistics on the variables
         and constraints that where added to the model.
@@ -129,12 +136,12 @@
         Arguments
         ---------
 
         file: None, optional
             Text stream to which output should be redirected. By default sys.stdout.
         """
         super().print_stats(abbrev=abbrev, file=file)
-        if abbrev:
+        if abbrev or self._no_debug:
             return
         print(file=file)
 
         self._print_container_steps("Estimator", self.estimators_, file=file)
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/linear_regression.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/linear_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/logistic_regression.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/mlpregressor.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/mlpregressor.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pipeline.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/pls_regression.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/pls_regression.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/predictors_list.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/predictors_list.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/preprocessing.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,15 +92,17 @@
         """Do the transformation on x."""
         _input = self._input
         output = self._output
 
         scale = self.transformer.scale_
         mean = self.transformer.mean_
 
-        self._gp_model.addConstr(_input - output * scale == mean, name="s")
+        self._gp_model.addConstr(
+            _input - output * scale == mean, name=self._name_var("s")
+        )
         return self
 
 
 class PolynomialFeaturesConstr(SKtransformer):
     """Class to model trained
     :external+sklearn:py:class:`sklearn.preprocessing.PolynomialFeatures` with
     gurobipy.
@@ -131,15 +133,15 @@
                 for j, feat in enumerate(_input[k, :]):
                     if power[j] == 2:
                         q_expr *= feat.item()
                         q_expr *= feat.item()
                     elif power[j] == 1:
                         q_expr *= feat.item()
                 self.gp_model.addConstr(
-                    output[k, i] == q_expr, name=f"polyfeat[{k},{i}]"
+                    output[k, i] == q_expr, name=self._indexed_name((k, i), "polyfeat")
                 )
 
 
 def sklearn_transformers():
     """Return dictionary of Scikit Learn preprocessing objects."""
     return {
         "StandardScaler": add_standard_scaler_constr,
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/random_forest_regressor.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/random_forest_regressor.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,22 +88,32 @@
         model = self._gp_model
         predictor = self.predictor
 
         _input = self._input
         output = self._output
         nex = _input.shape[0]
 
+        if self._no_debug:
+            kwargs["no_record"] = True
+
+        if self._name == "" or self._no_recording:
+            name = ""
+        else:
+            name = "estimator"
+
         tree_vars = model.addMVar(
             (nex, predictor.n_estimators, self._output_shape),
             lb=-GRB.INFINITY,
-            name="estimator",
+            name=name,
         )
 
         estimators = []
         for i in range(predictor.n_estimators):
+            if self.verbose:
+                self._timer.timing(f"Estimator {i}")
             tree = predictor.estimators_[i]
             estimators.append(
                 add_decision_tree_regressor_constr(
                     model, tree, _input, tree_vars[:, i, :], **kwargs
                 )
             )
         self.estimators_ = estimators
@@ -121,12 +131,12 @@
         Arguments
         ---------
 
         file: None, optional
             Text stream to which output should be redirected. By default sys.stdout.
         """
         super().print_stats(abbrev=abbrev, file=file)
-        if abbrev:
+        if abbrev or self._no_debug:
             return
         print(file=file)
 
         self._print_container_steps("Estimator", self.estimators_, file=file)
```

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/sklearn/skgetter.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/sklearn/skgetter.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/__init__.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.1.1/src/gurobi_ml/torch/sequential.py` & `gurobi-machinelearning-1.2.0a1/src/gurobi_ml/torch/sequential.py`

 * *Files identical despite different names*

