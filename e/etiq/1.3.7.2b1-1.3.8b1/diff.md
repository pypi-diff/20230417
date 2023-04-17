# Comparing `tmp/etiq-1.3.7.2b1-cp39-cp39-win_amd64.whl.zip` & `tmp/etiq-1.3.8b1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 4011017 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat  6861312 b- defN 23-Mar-03 11:25 etiq.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3428 b- defN 23-Mar-03 11:25 etiq.pyi
--rw-rw-rw-  2.0 fat     2516 b- defN 23-Mar-03 11:20 etiq/db/migrations/version8.sql
--rw-rw-rw-  2.0 fat     1488 b- defN 23-Mar-03 11:20 etiq/db/migrations/version8.webapi.sql
--rw-rw-rw-  2.0 fat    76123 b- defN 23-Mar-03 11:20 etiq/sample_data/adult_data_sampled.pkl
--rw-rw-rw-  2.0 fat   293857 b- defN 23-Mar-03 11:20 etiq/sample_data/adult_protected_train_resampled.pkl
--rw-rw-rw-  2.0 fat  3812946 b- defN 23-Mar-03 11:20 etiq/sample_data/adult_x_train_resampled.pkl
--rw-rw-rw-  2.0 fat   293857 b- defN 23-Mar-03 11:20 etiq/sample_data/adult_y_train_resampled.pkl
--rw-rw-rw-  2.0 fat  3226815 b- defN 23-Mar-03 11:20 etiq/sample_data/adultdata.pkl
--rw-rw-rw-  2.0 fat  5326370 b- defN 23-Mar-03 11:20 etiq/sample_data/adultdataset.csv
--rw-rw-rw-  2.0 fat  5789538 b- defN 23-Mar-03 11:20 etiq/sample_data/encoded_adult.pkl
--rw-rw-rw-  2.0 fat    44206 b- defN 23-Mar-03 11:25 etiq-1.3.7.2b1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2387 b- defN 23-Mar-03 11:25 etiq-1.3.7.2b1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Mar-03 11:25 etiq-1.3.7.2b1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Mar-03 11:21 etiq-1.3.7.2b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1414 b- defN 23-Mar-03 11:25 etiq-1.3.7.2b1.dist-info/RECORD
-16 files, 25736356 bytes uncompressed, 4008699 bytes compressed:  84.4%
+Zip file size: 4596738 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat  7102464 b- defN 23-Apr-17 12:02 etiq.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3644 b- defN 23-Apr-17 12:02 etiq.pyi
+-rw-rw-rw-  2.0 fat     2516 b- defN 23-Apr-17 11:57 etiq/db/migrations/version8.sql
+-rw-rw-rw-  2.0 fat     1488 b- defN 23-Apr-17 11:57 etiq/db/migrations/version8.webapi.sql
+-rw-rw-rw-  2.0 fat   109275 b- defN 23-Apr-17 11:57 etiq/sample_data/adult_data_sampled.csv
+-rw-rw-rw-  2.0 fat    76123 b- defN 23-Apr-17 11:57 etiq/sample_data/adult_data_sampled.pkl
+-rw-rw-rw-  2.0 fat   293857 b- defN 23-Apr-17 11:57 etiq/sample_data/adult_protected_train_resampled.pkl
+-rw-rw-rw-  2.0 fat  3812946 b- defN 23-Apr-17 11:57 etiq/sample_data/adult_x_train_resampled.pkl
+-rw-rw-rw-  2.0 fat   293857 b- defN 23-Apr-17 11:57 etiq/sample_data/adult_y_train_resampled.pkl
+-rw-rw-rw-  2.0 fat  3226815 b- defN 23-Apr-17 11:57 etiq/sample_data/adultdata.pkl
+-rw-rw-rw-  2.0 fat  5326370 b- defN 23-Apr-17 11:57 etiq/sample_data/adultdataset.csv
+-rw-rw-rw-  2.0 fat  1836780 b- defN 23-Apr-17 11:57 etiq/sample_data/encoded_adult.csv
+-rw-rw-rw-  2.0 fat  5789538 b- defN 23-Apr-17 11:57 etiq/sample_data/encoded_adult.pkl
+-rw-rw-rw-  2.0 fat    44206 b- defN 23-Apr-17 12:03 etiq-1.3.8b1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2363 b- defN 23-Apr-17 12:03 etiq-1.3.8b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-17 12:03 etiq-1.3.8b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-17 11:57 etiq-1.3.8b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1596 b- defN 23-Apr-17 12:03 etiq-1.3.8b1.dist-info/RECORD
+18 files, 27923937 bytes uncompressed, 4594142 bytes compressed:  83.6%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: etiq/db/migrations/version8.sql
 Comment: 
 
 Filename: etiq/db/migrations/version8.webapi.sql
 Comment: 
 
+Filename: etiq/sample_data/adult_data_sampled.csv
+Comment: 
+
 Filename: etiq/sample_data/adult_data_sampled.pkl
 Comment: 
 
 Filename: etiq/sample_data/adult_protected_train_resampled.pkl
 Comment: 
 
 Filename: etiq/sample_data/adult_x_train_resampled.pkl
@@ -24,26 +27,29 @@
 
 Filename: etiq/sample_data/adultdata.pkl
 Comment: 
 
 Filename: etiq/sample_data/adultdataset.csv
 Comment: 
 
+Filename: etiq/sample_data/encoded_adult.csv
+Comment: 
+
 Filename: etiq/sample_data/encoded_adult.pkl
 Comment: 
 
-Filename: etiq-1.3.7.2b1.dist-info/LICENSE
+Filename: etiq-1.3.8b1.dist-info/LICENSE
 Comment: 
 
-Filename: etiq-1.3.7.2b1.dist-info/METADATA
+Filename: etiq-1.3.8b1.dist-info/METADATA
 Comment: 
 
-Filename: etiq-1.3.7.2b1.dist-info/WHEEL
+Filename: etiq-1.3.8b1.dist-info/WHEEL
 Comment: 
 
-Filename: etiq-1.3.7.2b1.dist-info/top_level.txt
+Filename: etiq-1.3.8b1.dist-info/top_level.txt
 Comment: 
 
-Filename: etiq-1.3.7.2b1.dist-info/RECORD
+Filename: etiq-1.3.8b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## etiq.pyi

```diff
@@ -6,26 +6,29 @@
 # standalone mode usage of the created library will need it.
 
 # In the future, this will also contain type information for values
 # in the module, so IDEs will use this. Therefore please include it
 # when you make software releases of the extension module that it
 # describes.
 
+import atexit
 import config
 import dataset_loader
 import datasets
 import measures
 import drift_measures
 import db.handlers
 import saas
 import model
 import utils
 import custom_metrics
 import snapshot_stage
 import etiq_dataissues
+import telemetry
+import calculation_handlers
 import drift_decision_tree
 import metric_decision_tree
 import concept_drift_decision_tree
 import collections
 import logging
 import shlex
 import numbers
@@ -43,23 +46,28 @@
 import json
 import pathlib
 import biasparams
 import dataprofile
 import dataclasses
 import enum
 import numpy.random
+import datasets.pandas
 import bias_dataset
 import simple_dataset
 import abstract_dataset
 import builders
-import uuid
-import hashlib
+import backend
 import simple_dataset_builder
 import bias_dataset_builder
 import pandas.api.types
+import simple_pandas_dataset
+import bias_pandas_dataset
+import uuid
+import hashlib
+import base_pandas_dataset
 import datetime
 import etiq
 import etiq.charting
 import etiq.pipeline
 import etiq.pipelines
 import etiq.pipeline_output
 import etiq.db.models.scan
@@ -116,32 +124,33 @@
 import repair_pipeline
 import evaluate_debias_pipeline
 import eda_pipeline
 import infer_protected_pipeline
 import data_issues_pipeline
 import steps
 import pipeline
-import random
 import eda_decisiontree
 import algorithms
 import pipeline_steps
-import db.events
 import leakage_steps
 import sklearn.cluster
 import decisiontree
 import etiq.snapshots
+import db.events
 import db.models
 import urllib.parse
 import requests
 import serialize
 import etiq.biasparams
 import sklearn.inspection
 import etiq.store
 import db.models.session
 import pipelines
+import concurrent.futures
+import etiq.db
 import pickle
 import sklearn.model_selection
 
 # This is not Python source even if it looks so. Make it clear for
 # now. This was decided by PEP 484 designers.
 __name__ = ...
```

## Comparing `etiq-1.3.7.2b1.dist-info/LICENSE` & `etiq-1.3.8b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `etiq-1.3.7.2b1.dist-info/METADATA` & `etiq-1.3.8b1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etiq
-Version: 1.3.7.2b1
+Version: 1.3.8b1
 Summary: ETIQ.ai ML Testing library
 Home-page: https://etiq.ai/
 Author: ETIQ AI
 Author-email: devops@etiq.ai
 License: UNKNOWN
 Keywords: ai,bias,etiq,fairness
 Platform: UNKNOWN
@@ -18,18 +18,18 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: platformdirs
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: sqlalchemy (<2,>=1.4)
 Requires-Dist: scikit-learn
```

## Comparing `etiq-1.3.7.2b1.dist-info/RECORD` & `etiq-1.3.8b1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-etiq.cp39-win_amd64.pyd,sha256=od2SPuSabDXtcCD13aFdMT4aJUt77Xh1HSM2Fybe_KQ,6861312
-etiq.pyi,sha256=FWl5jWJa0NNGu2VTwZgNU3cFXwaG9d2u5TxD3VXN77s,3428
+etiq.cp39-win_amd64.pyd,sha256=y-v802PU2Gj1bqQWRpzVHbeHTqudJmIptgNxJj7eWus,7102464
+etiq.pyi,sha256=rxvOtw08M-irzwf_Q1bU8SW_VZB6XsfNhLEXC-inH-g,3644
 etiq/db/migrations/version8.sql,sha256=oFtWtyC508rXaMPF1FKO4QPOcQlu0-d36yJe5HFmxk8,2516
 etiq/db/migrations/version8.webapi.sql,sha256=pwfC3hus1tNgh-HpLwIpQSlF2q7EuI6siVgJCRD4AFk,1488
+etiq/sample_data/adult_data_sampled.csv,sha256=xY7td4iCl8-o3t8P1emV5ISUZoEnbpsEQJalg-Kijxg,109275
 etiq/sample_data/adult_data_sampled.pkl,sha256=k5Z1s0L25NDcr3IDAcMED1iZqq80vGwlgkmEvNpHPsU,76123
 etiq/sample_data/adult_protected_train_resampled.pkl,sha256=oBcVQjfcJ38D2D2zMNa9ofNNIETU6Hlzmf_CzBj0uS0,293857
 etiq/sample_data/adult_x_train_resampled.pkl,sha256=VMJPcID9oBwnp8wqiPFfbMpLB6r5FQ28QmxRWo7vAHs,3812946
 etiq/sample_data/adult_y_train_resampled.pkl,sha256=MH7631Z9p2_YTg9X8GPyowRWm_TSdumNt_-6fP58fHI,293857
 etiq/sample_data/adultdata.pkl,sha256=dVgz4YEzZYQYjZmuqOP2OcsE-L_BUpwGUkPZ5fPzoAY,3226815
 etiq/sample_data/adultdataset.csv,sha256=tUOyd-nSnrr8ul7iwnkcTzQdhQJVp1HLvV-GMXCd234,5326370
+etiq/sample_data/encoded_adult.csv,sha256=_VhBzOj2MBIysxOFuG10G-1CuGmbiwD5k8MgxsMjIpo,1836780
 etiq/sample_data/encoded_adult.pkl,sha256=uYVVi70zhCmPopn7EydRJQELhkH0PgcgiAk2y0tmypQ,5789538
-etiq-1.3.7.2b1.dist-info/LICENSE,sha256=4YUnT8m5mSe2Dl6tK6RkjgGbgHiIaNTPtkumHS3ifX4,44206
-etiq-1.3.7.2b1.dist-info/METADATA,sha256=o0kQdeUNcEnzsmjNGlyOFTprQ5dKiYcrKMSP8UGZVZQ,2387
-etiq-1.3.7.2b1.dist-info/WHEEL,sha256=METhDxvF3AeSZA3kue2-ln1bIdNR4WvCRt56wSAGLbc,94
-etiq-1.3.7.2b1.dist-info/top_level.txt,sha256=qdr7hqmhoEm6vftJCKRQZkVYQ0cN3rklxzEqdyOkrus,5
-etiq-1.3.7.2b1.dist-info/RECORD,,
+etiq-1.3.8b1.dist-info/LICENSE,sha256=4YUnT8m5mSe2Dl6tK6RkjgGbgHiIaNTPtkumHS3ifX4,44206
+etiq-1.3.8b1.dist-info/METADATA,sha256=bSS0wsEQmGHv2KVfq08slj-hPKn0R78FejeN_YJSLT8,2363
+etiq-1.3.8b1.dist-info/WHEEL,sha256=4Js21CeqxstYuRusMkuxpu1_Dz5nsZfYBExpe3gMC24,94
+etiq-1.3.8b1.dist-info/top_level.txt,sha256=qdr7hqmhoEm6vftJCKRQZkVYQ0cN3rklxzEqdyOkrus,5
+etiq-1.3.8b1.dist-info/RECORD,,
```

