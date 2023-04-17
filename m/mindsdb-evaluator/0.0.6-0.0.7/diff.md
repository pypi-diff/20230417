# Comparing `tmp/mindsdb_evaluator-0.0.6.tar.gz` & `tmp/mindsdb_evaluator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindsdb_evaluator-0.0.6.tar", max compression
+gzip compressed data, was "mindsdb_evaluator-0.0.7.tar", max compression
```

## Comparing `mindsdb_evaluator-0.0.6.tar` & `mindsdb_evaluator-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    35103 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/LICENSE
--rw-r--r--   0        0        0       69 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/README.md
--rw-r--r--   0        0        0      186 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/__init__.py
--rw-r--r--   0        0        0      717 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/__init__.py
--rw-r--r--   0        0        0      330 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/classification.py
--rw-r--r--   0        0        0     3512 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/forecasting.py
--rw-r--r--   0        0        0     3711 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/general.py
--rw-r--r--   0        0        0      763 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/regression.py
--rw-r--r--   0        0        0       69 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/calibration/__init__.py
--rw-r--r--   0        0        0      126 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/mindsdb_evaluator/calibration/ece.py
--rw-r--r--   0        0        0      500 2023-01-19 22:25:38.533561 mindsdb_evaluator-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 mindsdb_evaluator-0.0.6/setup.py
--rw-r--r--   0        0        0      799 1970-01-01 00:00:00.000000 mindsdb_evaluator-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35103 2023-04-17 03:01:27.093942 mindsdb_evaluator-0.0.7/LICENSE
+-rw-r--r--   0        0        0       69 2023-04-17 03:01:27.093942 mindsdb_evaluator-0.0.7/README.md
+-rw-r--r--   0        0        0      186 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/__init__.py
+-rw-r--r--   0        0        0      714 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/classification.py
+-rw-r--r--   0        0        0     3512 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/forecasting.py
+-rw-r--r--   0        0        0     3928 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/general.py
+-rw-r--r--   0        0        0      763 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/regression.py
+-rw-r--r--   0        0        0       69 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/calibration/__init__.py
+-rw-r--r--   0        0        0      126 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/mindsdb_evaluator/calibration/ece.py
+-rw-r--r--   0        0        0      492 2023-04-17 03:01:27.097942 mindsdb_evaluator-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 mindsdb_evaluator-0.0.7/PKG-INFO
```

### Comparing `mindsdb_evaluator-0.0.6/LICENSE` & `mindsdb_evaluator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/__init__.py` & `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mindsdb_evaluator.accuracy.general import evaluate_accuracy, evaluate_accuracies
 from mindsdb_evaluator.accuracy.regression import evaluate_regression_accuracy
-from mindsdb_evaluator.accuracy.classification import evaluate_multilabel_accuracy
+from mindsdb_evaluator.accuracy.classification import evaluate_multilabel_accuracy, evaluate_top_k_accuracy
 from mindsdb_evaluator.accuracy.forecasting import \
     evaluate_array_accuracy, \
     evaluate_num_array_accuracy, \
     evaluate_cat_array_accuracy, \
     complementary_smape_array_accuracy
 
 __all__ = ['evaluate_accuracy', 'evaluate_accuracies', 'evaluate_regression_accuracy', 'evaluate_multilabel_accuracy',
-           'evaluate_array_accuracy', 'evaluate_num_array_accuracy', 'evaluate_cat_array_accuracy',
-           'complementary_smape_array_accuracy']  # noqa
+           'evaluate_top_k_accuracy', 'evaluate_array_accuracy', 'evaluate_num_array_accuracy',
+           'evaluate_cat_array_accuracy', 'complementary_smape_array_accuracy']  # noqa
```

### Comparing `mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/forecasting.py` & `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/forecasting.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/general.py` & `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
     evaluate_num_array_accuracy, \
     evaluate_cat_array_accuracy, \
     complementary_smape_array_accuracy
 
 
 def evaluate_accuracy(data: pd.DataFrame,
                       predictions: pd.Series,
-                      target: str,
                       accuracy_function: str,
+                      target: Optional[str] = None,
                       ts_analysis: Optional[dict] = {},
                       n_decimals: Optional[int] = 3) -> float:
     """
     Dispatcher for accuracy evaluation.
 
     :param data: original dataframe.
     :param predictions: output of a machine learning model for the input `data`.
@@ -72,11 +72,16 @@
                         predictions: pd.Series,
                         target: str,
                         accuracy_functions: List[str],
                         ts_analysis: Optional[dict] = {},
                         n_decimals: Optional[int] = 3) -> Dict[str, float]:
     score_dict = {}
     for accuracy_function in accuracy_functions:
-        score = evaluate_accuracy(data, predictions, target, accuracy_function, ts_analysis, n_decimals)
+        score = evaluate_accuracy(data,
+                                  predictions,
+                                  accuracy_function,
+                                  target=target,
+                                  ts_analysis=ts_analysis,
+                                  n_decimals=n_decimals)
         score_dict[accuracy_function] = score
 
     return score_dict
```

### Comparing `mindsdb_evaluator-0.0.6/mindsdb_evaluator/accuracy/regression.py` & `mindsdb_evaluator-0.0.7/mindsdb_evaluator/accuracy/regression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_evaluator-0.0.6/PKG-INFO` & `mindsdb_evaluator-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mindsdb-evaluator
-Version: 0.0.6
+Version: 0.0.7
 Summary: Model evaluation for Machine Learning pipelines.
 License: GPL-3.0
 Author: MindsDB Inc.
 Author-email: hello@mindsdb.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: dataprep-ml (>=0.0.8,<0.0.9)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pandas (>=1,<2)
-Requires-Dist: scikit-learn (>=1.0.0,<=1.0.2)
+Requires-Dist: scikit-learn (>=0.24.2)
 Requires-Dist: type-infer (>=0.0.9,<0.0.10)
 Description-Content-Type: text/markdown
 
 # mindsdb_evaluator
 
 Model evaluation for Machine Learning pipelines.
```

