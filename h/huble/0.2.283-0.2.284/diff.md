# Comparing `tmp/huble-0.2.283.tar.gz` & `tmp/huble-0.2.284.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huble-0.2.283.tar", max compression
+gzip compressed data, was "huble-0.2.284.tar", max compression
```

## Comparing `huble-0.2.283.tar` & `huble-0.2.284.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.283/README.md
--rw-r--r--   0        0        0      729 2023-04-17 11:46:22.791020 huble-0.2.283/pyproject.toml
--rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.283/src/huble/__init__.py
--rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.283/src/huble/automl/__init__.py
--rw-r--r--   0        0        0     4953 2023-03-16 13:59:03.136664 huble-0.2.283/src/huble/automl/automl.py
--rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.283/src/huble/connector/__init__.py
--rw-r--r--   0        0        0      675 2023-04-17 11:43:21.388697 huble-0.2.283/src/huble/connector/dataset.py
--rw-r--r--   0        0        0     1564 2023-02-04 14:11:21.308460 huble-0.2.283/src/huble/connector/deployment.py
--rw-r--r--   0        0        0     2499 2023-02-17 05:24:53.511354 huble-0.2.283/src/huble/connector/experiment.py
--rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.283/src/huble/error/__init__.py
--rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.283/src/huble/error/decorators.py
--rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.283/src/huble/error/exceptions.py
--rw-r--r--   0        0        0      421 2023-02-04 12:16:33.294928 huble-0.2.283/src/huble/main.py
--rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.283/src/huble/sklearn/__init__.py
--rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.283/src/huble/sklearn/essentials/__init__.py
--rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.283/src/huble/sklearn/essentials/essentail_params.ts
--rw-r--r--   0        0        0     1184 2023-02-14 03:58:18.837339 huble-0.2.283/src/huble/sklearn/essentials/function.py
--rw-r--r--   0        0        0      965 2023-02-14 06:01:34.257728 huble-0.2.283/src/huble/sklearn/essentials/handler.py
--rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.283/src/huble/sklearn/evaluate.py
--rw-r--r--   0        0        0     3466 2023-02-24 09:49:44.133824 huble-0.2.283/src/huble/sklearn/generate.py
--rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.283/src/huble/sklearn/graph.py
--rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.283/src/huble/sklearn/metrics/__init__.py
--rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.283/src/huble/sklearn/metrics/metrics.py
--rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.283/src/huble/sklearn/process/__init__.py
--rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/sklearn/process/functions.py
--rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/sklearn/process/handler.py
--rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/sklearn/process/preprocess_params.ts
--rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.283/src/huble/sklearn/train/__init__.py
--rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.283/src/huble/sklearn/train/functions.py
--rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.283/src/huble/sklearn/train/handler.py
--rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.283/src/huble/sklearn/train/model_params.ts
--rw-r--r--   0        0        0      255 2023-02-18 07:40:12.798302 huble-0.2.283/src/huble/util/__init__.py
--rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.283/src/huble/util/convert_to_reactflow_graph.py
--rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/util/data_types.py
--rw-r--r--   0        0        0      413 2023-02-01 12:25:17.943452 huble-0.2.283/src/huble/util/feature_selection.py
--rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.283/src/huble/util/inference_pipeline.py
--rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.283/src/huble/util/recommend_model.py
--rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.283/src/huble/util/typed_params.py
--rw-r--r--   0        0        0     2483 2023-03-12 07:57:42.585777 huble-0.2.283/src/huble/util/verify_builder_pipeline.py
--rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.283/src/huble/util/verify_ml.py
--rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 huble-0.2.283/setup.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 huble-0.2.283/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.284/README.md
+-rw-r--r--   0        0        0      729 2023-04-17 12:09:15.891719 huble-0.2.284/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.284/src/huble/__init__.py
+-rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.284/src/huble/automl/__init__.py
+-rw-r--r--   0        0        0     5002 2023-04-17 11:57:46.692196 huble-0.2.284/src/huble/automl/automl.py
+-rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.284/src/huble/connector/__init__.py
+-rw-r--r--   0        0        0      675 2023-04-17 11:43:21.388697 huble-0.2.284/src/huble/connector/dataset.py
+-rw-r--r--   0        0        0     1564 2023-02-04 14:11:21.308460 huble-0.2.284/src/huble/connector/deployment.py
+-rw-r--r--   0        0        0     2499 2023-02-17 05:24:53.511354 huble-0.2.284/src/huble/connector/experiment.py
+-rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.284/src/huble/error/__init__.py
+-rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.284/src/huble/error/decorators.py
+-rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.284/src/huble/error/exceptions.py
+-rw-r--r--   0        0        0      421 2023-02-04 12:16:33.294928 huble-0.2.284/src/huble/main.py
+-rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.284/src/huble/sklearn/__init__.py
+-rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.284/src/huble/sklearn/essentials/__init__.py
+-rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.284/src/huble/sklearn/essentials/essentail_params.ts
+-rw-r--r--   0        0        0     1269 2023-04-17 11:56:37.991446 huble-0.2.284/src/huble/sklearn/essentials/function.py
+-rw-r--r--   0        0        0      983 2023-04-17 12:07:07.254917 huble-0.2.284/src/huble/sklearn/essentials/handler.py
+-rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.284/src/huble/sklearn/evaluate.py
+-rw-r--r--   0        0        0     3466 2023-02-24 09:49:44.133824 huble-0.2.284/src/huble/sklearn/generate.py
+-rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.284/src/huble/sklearn/graph.py
+-rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.284/src/huble/sklearn/metrics/__init__.py
+-rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.284/src/huble/sklearn/metrics/metrics.py
+-rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.284/src/huble/sklearn/process/__init__.py
+-rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.284/src/huble/sklearn/process/functions.py
+-rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.284/src/huble/sklearn/process/handler.py
+-rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.284/src/huble/sklearn/process/preprocess_params.ts
+-rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.284/src/huble/sklearn/train/__init__.py
+-rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.284/src/huble/sklearn/train/functions.py
+-rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.284/src/huble/sklearn/train/handler.py
+-rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.284/src/huble/sklearn/train/model_params.ts
+-rw-r--r--   0        0        0      304 2023-04-17 11:56:37.991446 huble-0.2.284/src/huble/util/__init__.py
+-rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.284/src/huble/util/convert_to_reactflow_graph.py
+-rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.284/src/huble/util/data_types.py
+-rw-r--r--   0        0        0      898 2023-04-17 11:56:37.991446 huble-0.2.284/src/huble/util/feature_selection.py
+-rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.284/src/huble/util/inference_pipeline.py
+-rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.284/src/huble/util/recommend_model.py
+-rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.284/src/huble/util/typed_params.py
+-rw-r--r--   0        0        0     2970 2023-04-17 11:56:37.994780 huble-0.2.284/src/huble/util/verify_builder_pipeline.py
+-rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.284/src/huble/util/verify_ml.py
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 huble-0.2.284/setup.py
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 huble-0.2.284/PKG-INFO
```

### Comparing `huble-0.2.283/pyproject.toml` & `huble-0.2.284/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huble"
-version = "0.2.283"
+version = "0.2.284"
 description = ""
 authors = ["Rugz007 <rugvedsomwanshi007@gmail.com>"]
 maintainers = [
     "Arjit Agarwal <arjitagarwal123@gmail.com>",
     "Ashmika Gupte <ashmikagupte01@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `huble-0.2.283/src/huble/automl/automl.py` & `huble-0.2.284/src/huble/automl/automl.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import evalml
 import json
 import numpy as np
 import pandas as pd
 from evalml.data_checks import DefaultDataChecks
 from evalml.automl import AutoMLSearch
 from evalml.pipelines.utils import generate_pipeline_code
+from ..util.data_types import get_dataframe_types
 
 
 def convert_to_json(my_dict):
     for key, value in my_dict.items():
         if isinstance(value, dict):
             convert_to_json(value)
         elif isinstance(value, list):
@@ -23,24 +24,27 @@
 
 
 def automl(data, target_column, task):
     # split into X and y
     X = data.drop(target_column, axis=1)
     y = data[target_column]
 
-    # Predict task type
-    if task == "classification":
-        n = len(pd.unique(data[target_column]))
-
-        if n == 2:
-            task = "binary"
-        else:
-            task = "multiclass"
+    data_dict = get_dataframe_types(X)
 
-    # train test split
+    #Predict task type
+    if task=="classification":
+      n = len(pd.unique(data[target_column]))
+    
+      if n==2:
+        task="binary"
+      else:
+        task="multiclass"
+     
+
+    #train test split
     X_train, X_test, y_train, y_test = evalml.preprocessing.split_data(X, y, problem_type=task)
 
     # Datachecks
     objective = ""
     if task == "binary":
         objective = objective + "log loss binary"
     elif task == "multiclass":
@@ -55,105 +59,96 @@
     data_issues = []
     for warning in warnings:
         data_issues.append("Warning:" + warning["message"])
 
     for error in errors:
         data_issues.append("Error:" + error["message"])
 
-    # AutoMl Search
+
+
+    #AutoMl Search
     automl = AutoMLSearch(X_train=X_train, y_train=y_train, problem_type=task)
     automl.search()
 
     # Pipeline Rankings
     rankings = automl.rankings
     rankings_json = rankings.to_json(orient="table")
 
     ids = []
     for i in range(6):
         ids.append(rankings["id"].iloc[i])
 
     pipelines = []
 
     for i in ids:
-        pip = {}
-        pipeline = automl.get_pipeline(i)
-        pip["id"] = i
-        pip["name"] = pipeline.name
-        pip["pipeline"] = str(pipeline)
-
-        pipeline.fit(X_train, y_train)
-
-        # metrics
-        objectives = []
-        if task == "binary":
-            objectives.extend(
-                [
-                    "mcc binary",
-                    "log loss binary",
-                    "gini",
-                    "auc",
-                    "recall",
-                    "precision",
-                    "f1",
-                    "balanced accuracy binary",
-                    "accuracy binary",
-                ]
-            )
-        elif task == "multiclass":
-            objectives.extend(
-                [
-                    "mcc multiclass",
-                    "log loss multiclass",
-                    "auc weighted",
-                    "auc macro",
-                    "auc micro",
-                    "recall weighted",
-                    "recall macro",
-                    "recall micro",
-                    "precision weighted",
-                    "precision macro",
-                    "precision micro",
-                    "f1 weighted",
-                    "f1 macro",
-                    "f1 micro",
-                    "balanced accuracy multiclass",
-                    "accuracy multiclass",
-                ]
-            )
-        elif task == "regression":
-            objectives.extend(
-                [
-                    "expvariance",
-                    "maxerror",
-                    "medianae",
-                    "mse",
-                    "mae",
-                    "r2",
-                    "mean squared log error",
-                    "root mean squared log error",
-                    "root mean squared error",
-                ]
-            )
-        pip["metrics"] = dict(pipeline.score(X_test, y_test, objectives))
-
-        # Feature importance for best pipeline
-        feature_imp = pipeline.feature_importance
-        feature_imp_json = feature_imp.to_json(orient="table")
-        pip["feature_importance"] = feature_imp_json
+      pip={}
+      pipeline = automl.get_pipeline(i)
+      pip['id']=i
+      pip['name']=pipeline.name
+      pip['pipeline']=str(pipeline)
+      
+      pipeline.fit(X_train, y_train) 
+      
+      #metrics
+      objectives=[]
+      if task =='binary':
+        objectives.extend(['mcc binary',
+                          'log loss binary',
+                          'gini',
+                          'auc',
+                          'recall',
+                          'precision',
+                          'f1',
+                          'balanced accuracy binary',
+                          'accuracy binary'])
+      elif task == 'multiclass':
+        objectives.extend(['mcc multiclass',
+                          'log loss multiclass',
+                          'auc weighted',
+                          'auc macro',
+                          'auc micro',
+                          'recall weighted',
+                          'recall macro',
+                          'recall micro',
+                          'precision weighted',
+                          'precision macro',
+                          'precision micro',
+                          'f1 weighted',
+                          'f1 macro',
+                          'f1 micro',
+                          'balanced accuracy multiclass',
+                          'accuracy multiclass'])
+      elif task =='regression':
+        objectives.extend(['expvariance',
+                          'maxerror',
+                          'medianae',
+                          'mse',
+                          'mae',
+                          'r2',
+                          'mean squared log error',
+                          'root mean squared log error',
+                          'root mean squared error',])
+      pip['metrics'] = dict(pipeline.score(X_test, y_test, objectives)) 
+      
+      #Feature importance for best pipeline
+      feature_imp = pipeline.feature_importance
+      feature_imp_json = feature_imp.to_json(orient="table")
+      pip['feature_importance']=feature_imp_json
 
         # generating code for best_pipeline
         pip["code"] = generate_pipeline_code(pipeline)
 
         pipelines.append(pip)
 
-    automl_result = {}
-    automl_result["Data Issues"] = data_issues
-    automl_result["Data Issue Messages"] = messages
-    automl_result["Task"] = task
-    automl_result["Pipelines"] = pipelines
-  
+    automl_result={}
+    automl_result['Data Issues']=data_issues
+    automl_result['Data Issue Messages']=messages
+    automl_result['Task']=task
+    automl_result['Pipelines']=pipelines
+    automl_result['input_format']=data_dict
+
     automl_json = convert_to_json(automl_result)
     automl_json = automl_json.replace("\\", "")
     automl_json = automl_json.replace('"{"schema', '{"schema')
     automl_json = automl_json.replace('", "code', ' ,"code')
 
     return automl_json
```

### Comparing `huble-0.2.283/src/huble/connector/dataset.py` & `huble-0.2.284/src/huble/connector/dataset.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/connector/deployment.py` & `huble-0.2.284/src/huble/connector/deployment.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/connector/experiment.py` & `huble-0.2.284/src/huble/connector/experiment.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/error/decorators.py` & `huble-0.2.284/src/huble/error/decorators.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/error/exceptions.py` & `huble-0.2.284/src/huble/error/exceptions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/essentials/essentail_params.ts` & `huble-0.2.284/src/huble/sklearn/essentials/essentail_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/essentials/function.py` & `huble-0.2.284/src/huble/sklearn/essentials/function.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from sklearn.model_selection import train_test_split as sklearn_tts  # type: ignore
 import pandas as pd
 from ...error.decorators import function_error_handling
 from ...connector import Dataset
 import joblib
 from ...util.data_types import get_dataframe_types
+from ...util.feature_selection import select_features
 
 # @function_error_handling("train_test_split")
 def train_test_split(**params):
     data = params["data"]
     target = params["target_column"]
+    model=params['model']
     X = data.drop([target], axis=1)
     data_dict = get_dataframe_types(X)
-    print(params["parameters"]["test_size"])
+    data = select_features(data, target, model)
     train_dataset, test_dataset = sklearn_tts(
         data, test_size=params["parameters"]["test_size"], random_state=42
     )
     return train_dataset, test_dataset, data_dict
 
 
 # @function_error_handling("train_model")
```

### Comparing `huble-0.2.283/src/huble/sklearn/essentials/handler.py` & `huble-0.2.284/src/huble/sklearn/essentials/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,11 +10,11 @@
         }
         return essentials[function_name](params=params, task_type=task_type, target_column=target_column)
 
     def __train_test_split(self, params, target_column, **kwargs):
         parameters = {
             "test_size": params["test_size"],
         }
-        return f"training_dataset, test_dataset, input_format = huble.sklearn.train_test_split(data=data,parameters={parameters}, target_column='{target_column}')"
+        return f"training_dataset, test_dataset, input_format = huble.sklearn.train_test_split(data=data,parameters={parameters}, target_column='{target_column}, model=model')"
 
-    def __train_model(self, params, task_type, **kwargs):
-        return f"Model, filename = huble.sklearn.train_model(data=training_dataset, model=model, column='{params['target_column']}', task_type='{task_type}')"
+    def __train_model(self, params, task_type, target_column, **kwargs):
+        return f"Model, filename = huble.sklearn.train_model(data=training_dataset, model=model, column='{target_column}', task_type='{task_type}')"
```

### Comparing `huble-0.2.283/src/huble/sklearn/evaluate.py` & `huble-0.2.284/src/huble/sklearn/evaluate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/generate.py` & `huble-0.2.284/src/huble/sklearn/generate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/graph.py` & `huble-0.2.284/src/huble/sklearn/graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/metrics/metrics.py` & `huble-0.2.284/src/huble/sklearn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/process/__init__.py` & `huble-0.2.284/src/huble/sklearn/process/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/process/functions.py` & `huble-0.2.284/src/huble/sklearn/process/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/process/handler.py` & `huble-0.2.284/src/huble/sklearn/process/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/process/preprocess_params.ts` & `huble-0.2.284/src/huble/sklearn/process/preprocess_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/train/__init__.py` & `huble-0.2.284/src/huble/sklearn/train/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/train/functions.py` & `huble-0.2.284/src/huble/sklearn/train/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/train/handler.py` & `huble-0.2.284/src/huble/sklearn/train/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/sklearn/train/model_params.ts` & `huble-0.2.284/src/huble/sklearn/train/model_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/util/convert_to_reactflow_graph.py` & `huble-0.2.284/src/huble/util/convert_to_reactflow_graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/util/data_types.py` & `huble-0.2.284/src/huble/util/data_types.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/util/inference_pipeline.py` & `huble-0.2.284/src/huble/util/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/util/typed_params.py` & `huble-0.2.284/src/huble/util/typed_params.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/src/huble/util/verify_builder_pipeline.py` & `huble-0.2.284/src/huble/util/verify_builder_pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,64 +4,75 @@
 
 
 def verify_pipeline(graph):
     issues = []
     steps = {}
     for node in graph["nodes"]:
         steps[node["data"]["name"]] = node["data"]["node_type"]
-        if node["data"]["node_type"] == "primary_dataset" or node["data"]["node_type"] == "model":
+        if node["data"]["node_type"] == "primary_dataset" or node["data"]["node_type"] == "model" or node["data"]["node_type"] == "classification_model" or node["data"]["node_type"] == "regression_model":
             if "target" not in node:
                 issues.append(node["data"]["name"] + " Node not connected")
         elif node["data"]["node_type"] == "evaluate_model":
-            if "source" not in node:
+            counter =0
+            for i in graph['edges']:
+              if i["target"]=="998":
+                  counter+=1
+            if counter<2:
                 issues.append(node["data"]["name"] + " Node not connected")
         else:
-            if "source" not in node or "target" not in node:
+            id = node['id']
+            
+            inputs = len(node['data']['inputParameters']['types'])
+            outputs = len(node['data']['outputParameters']['types'])
+            input=0
+            output=0
+            for i in graph['edges']:
+              if i['target']==id:
+                input+=1
+              elif i['source']==id:
+                output+=1
+            
+            if input!=inputs or output!=outputs:
                 issues.append(node["data"]["name"] + " Node not connected")
 
     value_counter = Counter(steps.values())
     key_counter = Counter(steps.keys())
-
-    if "Train Model" not in steps:
-        issues.append("Train Model Node Missing")
-    elif key_counter["Train Model"] > 1:
-        issues.append("More than one Train Model Node found")
-    if "Train-Test Split" not in steps:
-        issues.append("Train-Test Split Node Missing")
-    elif key_counter["Train-Test Split"] > 1:
-        issues.append("More than one Train-Test Split Node found")
-    if "Evaluate Model" not in steps:
-        issues.append("Evaluate Model Node Missing")
-    elif key_counter["Evaluate Model"] > 1:
-        issues.append("More than one Evaluate Model Node found")
-    if (
-        "model" not in steps.values()
-        and "classification_model" not in steps.values()
-        and "regression_model" not in steps.values()
-        and "clustering_model" not in steps.values()
-    ):
-        issues.append("Model Node Missing")
-    elif value_counter["model"] > 1:
-        issues.append("More than one Model Node found")
-    if "primary_dataset" not in steps.values():
-        issues.append("Dataset Node Missing")
-    elif value_counter["primary_dataset"] > 1:
-        issues.append("More than one Dataset Node found")
+  
+    if 'Train Model' not in steps:
+      issues.append('Train Model Node Missing')
+    elif key_counter['Train Model']>1:
+      issues.append('More than one Train Model Node found')
+    if 'Train-Test Split' not in steps:
+      issues.append('Train-Test Split Node Missing')
+    elif key_counter['Train-Test Split']>1:
+      issues.append('More than one Train-Test Split Node found')
+    if 'Evaluate Model' not in steps:
+      issues.append('Evaluate Model Node Missing')
+    elif key_counter['Evaluate Model']>1:
+      issues.append('More than one Evaluate Model Node found')
+    if 'model' not in steps.values() and 'classification_model' not in steps.values() and 'regression_model' not in steps.values():
+      issues.append('Model Node Missing')
+    elif value_counter['model']>1:
+      issues.append('More than one Model Node found')
+    if 'primary_dataset' not in steps.values():
+      issues.append('Dataset Node Missing')
+    elif value_counter['primary_dataset']>1:
+      issues.append('More than one Dataset Node found')
 
     g = Graph(len(graph["nodes"]))
     graph_dict = {}
     for i in graph["nodes"]:
         graph_dict[(i["data"]["name"])] = i
     map = {}
     j = 0
     while j < (len(graph["nodes"])):
         for i in graph["nodes"]:
             map[(i["id"])] = j
             j += 1
-
+  
     for i in graph["edges"]:
         g.addEdge(map[i["source"]], map[i["target"]])
 
     if g.isCyclic() == 1:
         issues.append("Graph contains cycle")
     else:
         pass
```

### Comparing `huble-0.2.283/src/huble/util/verify_ml.py` & `huble-0.2.284/src/huble/util/verify_ml.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.283/setup.py` & `huble-0.2.284/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'pydantic>=1.10.4,<2.0.0',
  'scikit-learn==1.1.2',
  'scipy>=1.7.0,<1.8.0',
  'woodwork>=0.21.1,<0.22.0']
 
 setup_kwargs = {
     'name': 'huble',
-    'version': '0.2.283',
+    'version': '0.2.284',
     'description': '',
     'long_description': '',
     'author': 'Rugz007',
     'author_email': 'rugvedsomwanshi007@gmail.com',
     'maintainer': 'Arjit Agarwal',
     'maintainer_email': 'arjitagarwal123@gmail.com',
     'url': 'None',
```

### Comparing `huble-0.2.283/PKG-INFO` & `huble-0.2.284/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huble
-Version: 0.2.283
+Version: 0.2.284
 Summary: 
 Author: Rugz007
 Author-email: rugvedsomwanshi007@gmail.com
 Maintainer: Arjit Agarwal
 Maintainer-email: arjitagarwal123@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: Programming Language :: Python :: 3
```

