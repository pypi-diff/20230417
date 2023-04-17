# Comparing `tmp/numerblox-0.5.6.tar.gz` & `tmp/numerblox-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerblox-0.5.6.tar", last modified: Wed Apr  5 12:35:59 2023, max compression
+gzip compressed data, was "numerblox-0.5.7.tar", last modified: Mon Apr 17 15:41:31 2023, max compression
```

## Comparing `numerblox-0.5.6.tar` & `numerblox-0.5.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-05 12:35:59.443124 numerblox-0.5.6/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4767 2023-04-05 12:06:33.000000 numerblox-0.5.6/CONTRIBUTING.md
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11357 2023-04-05 12:06:33.000000 numerblox-0.5.6/LICENSE
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      111 2023-04-05 12:06:33.000000 numerblox-0.5.6/MANIFEST.in
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-05 12:35:59.443124 numerblox-0.5.6/PKG-INFO
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11651 2023-04-05 12:35:32.000000 numerblox-0.5.6/README.md
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-05 12:35:59.443124 numerblox-0.5.6/numerblox/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       22 2023-04-05 12:35:32.000000 numerblox-0.5.6/numerblox/__init__.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    67966 2023-04-05 12:35:32.000000 numerblox-0.5.6/numerblox/_modidx.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4073 2023-04-05 12:06:33.000000 numerblox-0.5.6/numerblox/_nbdev.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    22382 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/download.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    69836 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/evaluation.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      103 2023-04-05 12:06:33.000000 numerblox-0.5.6/numerblox/index.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      947 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/key.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      333 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/misc.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    26837 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/model.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     5985 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/model_pipeline.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     6929 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/numerframe.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15357 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/postprocessing.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    30218 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/preprocessing.py
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15925 2023-04-05 12:12:10.000000 numerblox-0.5.6/numerblox/submission.py
-drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-05 12:35:59.443124 numerblox-0.5.6/numerblox.egg-info/
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-05 12:35:59.000000 numerblox-0.5.6/numerblox.egg-info/PKG-INFO
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      612 2023-04-05 12:35:59.000000 numerblox-0.5.6/numerblox.egg-info/SOURCES.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-05 12:35:59.000000 numerblox-0.5.6/numerblox.egg-info/dependency_links.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       40 2023-04-05 12:35:59.000000 numerblox-0.5.6/numerblox.egg-info/entry_points.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-05 12:35:40.000000 numerblox-0.5.6/numerblox.egg-info/not-zip-safe
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      194 2023-04-05 12:35:59.000000 numerblox-0.5.6/numerblox.egg-info/requires.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       10 2023-04-05 12:35:59.000000 numerblox-0.5.6/numerblox.egg-info/top_level.txt
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     1071 2023-04-05 12:35:32.000000 numerblox-0.5.6/settings.ini
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       38 2023-04-05 12:35:59.443124 numerblox-0.5.6/setup.cfg
--rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     2537 2023-04-05 12:06:33.000000 numerblox-0.5.6/setup.py
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-17 15:41:31.393349 numerblox-0.5.7/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4767 2023-04-05 12:06:33.000000 numerblox-0.5.7/CONTRIBUTING.md
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11357 2023-04-05 12:06:33.000000 numerblox-0.5.7/LICENSE
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      111 2023-04-05 12:06:33.000000 numerblox-0.5.7/MANIFEST.in
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-17 15:41:31.393349 numerblox-0.5.7/PKG-INFO
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    11651 2023-04-05 12:35:32.000000 numerblox-0.5.7/README.md
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-17 15:41:31.389349 numerblox-0.5.7/numerblox/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       22 2023-04-17 15:39:55.000000 numerblox-0.5.7/numerblox/__init__.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    67939 2023-04-17 15:39:55.000000 numerblox-0.5.7/numerblox/_modidx.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     4073 2023-04-05 12:06:33.000000 numerblox-0.5.7/numerblox/_nbdev.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    22382 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/download.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    70911 2023-04-17 15:39:55.000000 numerblox-0.5.7/numerblox/evaluation.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      103 2023-04-05 12:06:33.000000 numerblox-0.5.7/numerblox/index.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      947 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/key.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      333 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/misc.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    26837 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/model.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     5985 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/model_pipeline.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     6929 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/numerframe.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15357 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/postprocessing.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    30218 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/preprocessing.py
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    15925 2023-04-17 15:28:39.000000 numerblox-0.5.7/numerblox/submission.py
+drwxr-xr-x   0 clepelaars  (1003) clepelaars  (1004)        0 2023-04-17 15:41:31.393349 numerblox-0.5.7/numerblox.egg-info/
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)    12474 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/PKG-INFO
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      612 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/SOURCES.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/dependency_links.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       40 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/entry_points.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)        1 2023-04-05 12:35:40.000000 numerblox-0.5.7/numerblox.egg-info/not-zip-safe
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)      194 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/requires.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       10 2023-04-17 15:41:31.000000 numerblox-0.5.7/numerblox.egg-info/top_level.txt
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     1071 2023-04-17 15:39:55.000000 numerblox-0.5.7/settings.ini
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)       38 2023-04-17 15:41:31.393349 numerblox-0.5.7/setup.cfg
+-rw-r--r--   0 clepelaars  (1003) clepelaars  (1004)     2537 2023-04-05 12:06:33.000000 numerblox-0.5.7/setup.py
```

### Comparing `numerblox-0.5.6/CONTRIBUTING.md` & `numerblox-0.5.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/LICENSE` & `numerblox-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/PKG-INFO` & `numerblox-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerblox
-Version: 0.5.6
+Version: 0.5.7
 Summary: Tools for solid Numerai pipelines
 Home-page: https://github.com/crowdcent/numerblox/
 Author: Jason Rosenfeld, Carlo Lepelaars and contributors
 Author-email: support@crowdcent.com
 License: Apache Software License 2.0
 Keywords: Numerai,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `numerblox-0.5.6/README.md` & `numerblox-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/_modidx.py` & `numerblox-0.5.7/numerblox/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,26 +114,26 @@
                                                                                               'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.max_drawdown': ( 'evaluation.html#baseevaluator.max_drawdown',
                                                                                            'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.max_feature_exposure': ( 'evaluation.html#baseevaluator.max_feature_exposure',
                                                                                                    'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.mean_std_sharpe': ( 'evaluation.html#baseevaluator.mean_std_sharpe',
                                                                                               'numerblox/evaluation.py'),
+                                      'numerblox.evaluation.BaseEvaluator.numerai_corr': ( 'evaluation.html#baseevaluator.numerai_corr',
+                                                                                           'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.per_era_corrs': ( 'evaluation.html#baseevaluator.per_era_corrs',
                                                                                             'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.plot_correlations': ( 'evaluation.html#baseevaluator.plot_correlations',
                                                                                                 'numerblox/evaluation.py'),
                                       'numerblox.evaluation.BaseEvaluator.tbx_mean_std_sharpe': ( 'evaluation.html#baseevaluator.tbx_mean_std_sharpe',
                                                                                                   'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiClassicEvaluator': ( 'evaluation.html#numeraiclassicevaluator',
                                                                                         'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiClassicEvaluator.__init__': ( 'evaluation.html#numeraiclassicevaluator.__init__',
                                                                                                  'numerblox/evaluation.py'),
-                                      'numerblox.evaluation.NumeraiClassicEvaluator.__load_json': ( 'evaluation.html#numeraiclassicevaluator.__load_json',
-                                                                                                    'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiClassicEvaluator.full_evaluation': ( 'evaluation.html#numeraiclassicevaluator.full_evaluation',
                                                                                                         'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiSignalsEvaluator': ( 'evaluation.html#numeraisignalsevaluator',
                                                                                         'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiSignalsEvaluator.__await_diagnostics': ( 'evaluation.html#numeraisignalsevaluator.__await_diagnostics',
                                                                                                             'numerblox/evaluation.py'),
                                       'numerblox.evaluation.NumeraiSignalsEvaluator.__init__': ( 'evaluation.html#numeraisignalsevaluator.__init__',
```

### Comparing `numerblox-0.5.6/numerblox/_nbdev.py` & `numerblox-0.5.7/numerblox/_nbdev.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/download.py` & `numerblox-0.5.7/numerblox/download.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/evaluation.py` & `numerblox-0.5.7/numerblox/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
            'NumeraiSignalsEvaluator']
 
 # %% ../nbs/07_evaluation.ipynb 4
 import time
 import json
 import numpy as np
 import pandas as pd
+from scipy import stats
 from tqdm.auto import tqdm
 import matplotlib.pyplot as plt
 from typing import Tuple, Union
 from numerapi import SignalsAPI
 from rich import print as rich_print
 
 from .numerframe import NumerFrame, create_numerframe
@@ -97,21 +98,25 @@
         )
         mean, std, sharpe = self.mean_std_sharpe(era_corrs=val_corrs)
         max_drawdown = self.max_drawdown(era_corrs=val_corrs)
         apy = self.apy(era_corrs=val_corrs)
         example_corr = self.example_correlation(
             dataf=dataf, pred_col=pred_col, example_col=example_col
         )
+        numerai_corr = self.numerai_corr(
+            dataf=dataf, pred_col=pred_col, target_col=target_col
+        )
 
         col_stats.loc[pred_col, "target"] = target_col
         col_stats.loc[pred_col, "mean"] = mean
         col_stats.loc[pred_col, "std"] = std
         col_stats.loc[pred_col, "sharpe"] = sharpe
         col_stats.loc[pred_col, "max_drawdown"] = max_drawdown
         col_stats.loc[pred_col, "apy"] = apy
+        col_stats.loc[pred_col, "numerai_corr"] = numerai_corr
         col_stats.loc[pred_col, "corr_with_example_preds"] = example_corr
 
         # Compute intensive stats
         if not self.fast_mode:
             max_feature_exposure = self.max_feature_exposure(
                 dataf=dataf, pred_col=pred_col
             )
@@ -159,14 +164,36 @@
         correlations per era.
         """
         mean = pd.Series(era_corrs.mean()).item()
         std = pd.Series(era_corrs.std(ddof=0)).item()
         sharpe = mean / std
         return mean, std, sharpe
 
+    def numerai_corr(
+        self, dataf: pd.DataFrame, pred_col: str, target_col: str
+    ) -> np.float64:
+        """
+        Computes 'Numerai Corr'.
+        More info: https://forum.numer.ai/t/target-cyrus-new-primary-target/6303
+
+        Assumes original target col as input (i.e. in [0, 1] range).
+        """
+        # Rank and gaussianize predictions
+        ranked_preds = self._normalize_uniform(dataf[pred_col].fillna(0.5), 
+                                               method="average")
+        gauss_ranked_preds = stats.norm.ppf(ranked_preds)
+        # Transform target from [0...1] to [-2...2] range
+        centered_target = dataf[target_col]*4 - 2
+        # Accentuate tails of predictions and targets
+        preds_p15 = np.sign(gauss_ranked_preds) * np.abs(gauss_ranked_preds) ** 1.5
+        target_p15 = np.sign(centered_target) * np.abs(centered_target) ** 1.5
+        # Pearson correlation
+        corr, _ = stats.pearsonr(preds_p15, target_p15)
+        return corr
+
     @staticmethod
     def max_drawdown(era_corrs: pd.Series) -> np.float64:
         """Maximum drawdown per era."""
         # Arbitrarily large window
         rolling_max = (
             (era_corrs + 1).cumprod().rolling(window=9000, min_periods=1).max()
         )
@@ -298,17 +325,17 @@
                 ccs = np.array(ccs)
             computed.append(ccs)
         return pd.DataFrame(
             np.array(computed), columns=columns, index=dataf[self.era_col].unique()
         )
 
     @staticmethod
-    def _normalize_uniform(df: pd.DataFrame) -> pd.Series:
+    def _normalize_uniform(df: pd.DataFrame, method: str = "first") -> pd.Series:
         """Normalize predictions uniformly using ranks."""
-        x = (df.rank(method="first") - 0.5) / len(df)
+        x = (df.rank(method=method) - 0.5) / len(df)
         return pd.Series(x, index=df.index)
 
     def plot_correlations(
         self,
         dataf: NumerFrame,
         pred_cols: list = None,
         corr_cols: list = None,
@@ -420,19 +447,14 @@
                 )
                 col_stats.loc[col, "feature_neutral_mean_v3"] = fnc_v3
                 col_stats.loc[col, "feature_neutral_std_v3"] = fn_std_v3
                 col_stats.loc[col, "feature_neutral_sharpe_v3"] = fn_sharpe_v3
             val_stats = pd.concat([val_stats, col_stats], axis=0)
         return val_stats
 
-    def __load_json(self, json_path: str) -> dict:
-        with open(json_path, 'r') as f:
-            data = json.load(f)
-        return data
-
 # %% ../nbs/07_evaluation.ipynb 15
 class NumeraiSignalsEvaluator(BaseEvaluator):
     """Evaluator for all metrics that are relevant in Numerai Signals."""
     def __init__(self, era_col: str = "friday_date", fast_mode=False):
         super().__init__(era_col=era_col, fast_mode=fast_mode)
 
     def get_neutralized_corr(self, val_dataf: pd.DataFrame, model_name: str, key: Key, timeout_min: int = 2) -> pd.Series:
```

### Comparing `numerblox-0.5.6/numerblox/key.py` & `numerblox-0.5.7/numerblox/key.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/model.py` & `numerblox-0.5.7/numerblox/model.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/model_pipeline.py` & `numerblox-0.5.7/numerblox/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/numerframe.py` & `numerblox-0.5.7/numerblox/numerframe.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/postprocessing.py` & `numerblox-0.5.7/numerblox/postprocessing.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/preprocessing.py` & `numerblox-0.5.7/numerblox/preprocessing.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox/submission.py` & `numerblox-0.5.7/numerblox/submission.py`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/numerblox.egg-info/PKG-INFO` & `numerblox-0.5.7/numerblox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerblox
-Version: 0.5.6
+Version: 0.5.7
 Summary: Tools for solid Numerai pipelines
 Home-page: https://github.com/crowdcent/numerblox/
 Author: Jason Rosenfeld, Carlo Lepelaars and contributors
 Author-email: support@crowdcent.com
 License: Apache Software License 2.0
 Keywords: Numerai,Machine Learning
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `numerblox-0.5.6/numerblox.egg-info/SOURCES.txt` & `numerblox-0.5.7/numerblox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numerblox-0.5.6/settings.ini` & `numerblox-0.5.7/settings.ini`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 user = crowdcent
 description = Tools for solid Numerai pipelines
 keywords = Numerai, Machine Learning
 author = Jason Rosenfeld, Carlo Lepelaars and contributors
 author_email = support@crowdcent.com
 copyright = CrowdCent 2023
 branch = master
-version = 0.5.6
+version = 0.5.7
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 4
 requirements = jupyter eod wandb numpy scipy umap-learn pandas tqdm rich kaggle joblib pyarrow numerapi numerbay lightgbm catboost scikit-learn python-dateutil google-cloud-storage tensorflow pandas_ta
```

### Comparing `numerblox-0.5.6/setup.py` & `numerblox-0.5.7/setup.py`

 * *Files identical despite different names*

