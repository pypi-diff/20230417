# Comparing `tmp/huble-0.2.282.tar.gz` & `tmp/huble-0.2.283.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huble-0.2.282.tar", max compression
+gzip compressed data, was "huble-0.2.283.tar", max compression
```

## Comparing `huble-0.2.282.tar` & `huble-0.2.283.tar`

### file list

```diff
@@ -1,50 +1,42 @@
--rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.282/README.md
--rw-r--r--   0        0        0      729 2023-04-15 08:29:10.250370 huble-0.2.282/pyproject.toml
--rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.282/src/huble/__init__.py
--rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.282/src/huble/automl/__init__.py
--rw-r--r--   0        0        0     4953 2023-03-16 13:59:03.136664 huble-0.2.282/src/huble/automl/automl.py
--rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.282/src/huble/connector/__init__.py
--rw-r--r--   0        0        0      538 2023-04-15 08:28:57.376925 huble-0.2.282/src/huble/connector/dataset.py
--rw-r--r--   0        0        0     1564 2023-02-04 14:11:21.308460 huble-0.2.282/src/huble/connector/deployment.py
--rw-r--r--   0        0        0     2499 2023-02-17 05:24:53.511354 huble-0.2.282/src/huble/connector/experiment.py
--rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.282/src/huble/error/__init__.py
--rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.282/src/huble/error/decorators.py
--rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.282/src/huble/error/exceptions.py
--rw-r--r--   0        0        0      421 2023-02-04 12:16:33.294928 huble-0.2.282/src/huble/main.py
--rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.282/src/huble/sklearn/__init__.py
--rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.282/src/huble/sklearn/essentials/__init__.py
--rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.282/src/huble/sklearn/essentials/essentail_params.ts
--rw-r--r--   0        0        0     1184 2023-02-14 03:58:18.837339 huble-0.2.282/src/huble/sklearn/essentials/function.py
--rw-r--r--   0        0        0      965 2023-02-14 06:01:34.257728 huble-0.2.282/src/huble/sklearn/essentials/handler.py
--rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.282/src/huble/sklearn/evaluate.py
--rw-r--r--   0        0        0     3466 2023-02-24 09:49:44.133824 huble-0.2.282/src/huble/sklearn/generate.py
--rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.282/src/huble/sklearn/graph.py
--rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.282/src/huble/sklearn/metrics/__init__.py
--rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.282/src/huble/sklearn/metrics/metrics.py
--rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.282/src/huble/sklearn/process/__init__.py
--rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.282/src/huble/sklearn/process/functions.py
--rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.282/src/huble/sklearn/process/handler.py
--rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.282/src/huble/sklearn/process/preprocess_params.ts
--rw-r--r--   0        0        0    29474 2023-03-18 13:13:37.398836 huble-0.2.282/src/huble/sklearn/temp/QmRspeqXi9J2PVTmXYwMaBif9dYWVkNhM8EFomUAfajnT1
--rw-r--r--   0        0        0        0 2023-01-29 12:30:52.174946 huble-0.2.282/src/huble/sklearn/temp/content/output.py
--rw-r--r--   0        0        0   268473 2023-03-18 13:13:37.498838 huble-0.2.282/src/huble/sklearn/temp/model.joblib
--rw-r--r--   0        0        0      960 2023-03-18 13:13:37.328835 huble-0.2.282/src/huble/sklearn/temp/output.py
--rw-r--r--   0        0        0    29474 2022-11-27 08:35:27.624396 huble-0.2.282/src/huble/sklearn/temp/test.csv
--rw-r--r--   0        0        0     1485 2023-03-18 13:45:46.190804 huble-0.2.282/src/huble/sklearn/temp/test.ipynb
--rw-r--r--   0        0        0      571 2023-02-04 10:24:04.374326 huble-0.2.282/src/huble/sklearn/temp/test.py
--rw-r--r--   0        0        0    29474 2022-11-27 08:35:27.624396 huble-0.2.282/src/huble/sklearn/temp/tested.csv
--rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.282/src/huble/sklearn/train/__init__.py
--rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.282/src/huble/sklearn/train/functions.py
--rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.282/src/huble/sklearn/train/handler.py
--rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.282/src/huble/sklearn/train/model_params.ts
--rw-r--r--   0        0        0      255 2023-02-18 07:40:12.798302 huble-0.2.282/src/huble/util/__init__.py
--rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.282/src/huble/util/convert_to_reactflow_graph.py
--rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.282/src/huble/util/data_types.py
--rw-r--r--   0        0        0      413 2023-02-01 12:25:17.943452 huble-0.2.282/src/huble/util/feature_selection.py
--rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.282/src/huble/util/inference_pipeline.py
--rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.282/src/huble/util/recommend_model.py
--rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.282/src/huble/util/typed_params.py
--rw-r--r--   0        0        0     2483 2023-03-12 07:57:42.585777 huble-0.2.282/src/huble/util/verify_builder_pipeline.py
--rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.282/src/huble/util/verify_ml.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 huble-0.2.282/setup.py
--rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 huble-0.2.282/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-01 20:06:17.369927 huble-0.2.283/README.md
+-rw-r--r--   0        0        0      729 2023-04-17 11:46:22.791020 huble-0.2.283/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-02-04 11:17:14.977888 huble-0.2.283/src/huble/__init__.py
+-rw-r--r--   0        0        0       26 2023-03-13 11:26:31.526581 huble-0.2.283/src/huble/automl/__init__.py
+-rw-r--r--   0        0        0     4953 2023-03-16 13:59:03.136664 huble-0.2.283/src/huble/automl/automl.py
+-rw-r--r--   0        0        0       98 2023-02-04 11:17:06.597876 huble-0.2.283/src/huble/connector/__init__.py
+-rw-r--r--   0        0        0      675 2023-04-17 11:43:21.388697 huble-0.2.283/src/huble/connector/dataset.py
+-rw-r--r--   0        0        0     1564 2023-02-04 14:11:21.308460 huble-0.2.283/src/huble/connector/deployment.py
+-rw-r--r--   0        0        0     2499 2023-02-17 05:24:53.511354 huble-0.2.283/src/huble/connector/experiment.py
+-rw-r--r--   0        0        0      156 2023-02-01 12:25:17.923451 huble-0.2.283/src/huble/error/__init__.py
+-rw-r--r--   0        0        0      524 2023-02-01 07:34:10.430416 huble-0.2.283/src/huble/error/decorators.py
+-rw-r--r--   0        0        0      608 2023-02-01 12:25:17.930118 huble-0.2.283/src/huble/error/exceptions.py
+-rw-r--r--   0        0        0      421 2023-02-04 12:16:33.294928 huble-0.2.283/src/huble/main.py
+-rw-r--r--   0        0        0      118 2023-02-01 12:25:17.910118 huble-0.2.283/src/huble/sklearn/__init__.py
+-rw-r--r--   0        0        0       75 2023-01-30 06:53:33.773046 huble-0.2.283/src/huble/sklearn/essentials/__init__.py
+-rw-r--r--   0        0        0      933 2023-01-29 09:39:15.224016 huble-0.2.283/src/huble/sklearn/essentials/essentail_params.ts
+-rw-r--r--   0        0        0     1184 2023-02-14 03:58:18.837339 huble-0.2.283/src/huble/sklearn/essentials/function.py
+-rw-r--r--   0        0        0      965 2023-02-14 06:01:34.257728 huble-0.2.283/src/huble/sklearn/essentials/handler.py
+-rw-r--r--   0        0        0     1388 2023-02-24 09:49:44.133824 huble-0.2.283/src/huble/sklearn/evaluate.py
+-rw-r--r--   0        0        0     3466 2023-02-24 09:49:44.133824 huble-0.2.283/src/huble/sklearn/generate.py
+-rw-r--r--   0        0        0     1410 2023-02-14 03:58:18.837339 huble-0.2.283/src/huble/sklearn/graph.py
+-rw-r--r--   0        0        0       33 2023-02-01 12:25:17.910118 huble-0.2.283/src/huble/sklearn/metrics/__init__.py
+-rw-r--r--   0        0        0     4860 2023-02-24 09:49:44.133824 huble-0.2.283/src/huble/sklearn/metrics/metrics.py
+-rw-r--r--   0        0        0      570 2023-02-01 12:25:17.916785 huble-0.2.283/src/huble/sklearn/process/__init__.py
+-rw-r--r--   0        0        0     6548 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/sklearn/process/functions.py
+-rw-r--r--   0        0        0    11268 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/sklearn/process/handler.py
+-rw-r--r--   0        0        0    21731 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/sklearn/process/preprocess_params.ts
+-rw-r--r--   0        0        0      602 2023-02-01 12:25:17.926785 huble-0.2.283/src/huble/sklearn/train/__init__.py
+-rw-r--r--   0        0        0     4944 2023-02-15 04:48:23.675688 huble-0.2.283/src/huble/sklearn/train/functions.py
+-rw-r--r--   0        0        0    13409 2023-02-04 12:30:51.391609 huble-0.2.283/src/huble/sklearn/train/handler.py
+-rw-r--r--   0        0        0    35186 2023-01-12 16:42:04.986469 huble-0.2.283/src/huble/sklearn/train/model_params.ts
+-rw-r--r--   0        0        0      255 2023-02-18 07:40:12.798302 huble-0.2.283/src/huble/util/__init__.py
+-rw-r--r--   0        0        0     3792 2023-02-01 12:25:17.993452 huble-0.2.283/src/huble/util/convert_to_reactflow_graph.py
+-rw-r--r--   0        0        0      564 2023-02-18 12:25:51.014331 huble-0.2.283/src/huble/util/data_types.py
+-rw-r--r--   0        0        0      413 2023-02-01 12:25:17.943452 huble-0.2.283/src/huble/util/feature_selection.py
+-rw-r--r--   0        0        0     2528 2023-02-14 06:45:35.870429 huble-0.2.283/src/huble/util/inference_pipeline.py
+-rw-r--r--   0        0        0      502 2023-02-01 12:25:17.946785 huble-0.2.283/src/huble/util/recommend_model.py
+-rw-r--r--   0        0        0     1259 2023-02-01 12:03:16.155209 huble-0.2.283/src/huble/util/typed_params.py
+-rw-r--r--   0        0        0     2483 2023-03-12 07:57:42.585777 huble-0.2.283/src/huble/util/verify_builder_pipeline.py
+-rw-r--r--   0        0        0     4888 2023-02-14 03:58:18.837339 huble-0.2.283/src/huble/util/verify_ml.py
+-rw-r--r--   0        0        0     1138 1970-01-01 00:00:00.000000 huble-0.2.283/setup.py
+-rw-r--r--   0        0        0      804 1970-01-01 00:00:00.000000 huble-0.2.283/PKG-INFO
```

### Comparing `huble-0.2.282/pyproject.toml` & `huble-0.2.283/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huble"
-version = "0.2.282"
+version = "0.2.283"
 description = ""
 authors = ["Rugz007 <rugvedsomwanshi007@gmail.com>"]
 maintainers = [
     "Arjit Agarwal <arjitagarwal123@gmail.com>",
     "Ashmika Gupte <ashmikagupte01@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `huble-0.2.282/src/huble/automl/automl.py` & `huble-0.2.283/src/huble/automl/automl.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/connector/dataset.py` & `huble-0.2.283/src/huble/connector/dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import pandas as pd
-import requests
-from pydantic import BaseModel
-
+import boto3
 # import woodwork as ww
 from ..util.data_types import get_dataframe_types
 import boto3
 
 
 class Dataset:
     def __init__(self, url) -> None:
         self.url = url
         self.dataframe = self.__load_dataset(url)
 
     def __load_dataset(self, url: str) -> pd.DataFrame:
-        return pd.read_csv(url)
+        bucket = "const-bucket"
+        file_name = url.split("/")[-1]
+        s3 = boto3.client('s3') 
+        obj = s3.get_object(Bucket= bucket, Key= file_name)
+        return pd.read_csv(obj['Body'])
 
     def parse_dataset(self):
         data_dict = get_dataframe_types(self.dataframe)
         data_dict["rows"] = len(self.dataframe.axes[0])
         return data_dict
```

### Comparing `huble-0.2.282/src/huble/connector/deployment.py` & `huble-0.2.283/src/huble/connector/deployment.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/connector/experiment.py` & `huble-0.2.283/src/huble/connector/experiment.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/error/decorators.py` & `huble-0.2.283/src/huble/error/decorators.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/error/exceptions.py` & `huble-0.2.283/src/huble/error/exceptions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/essentials/essentail_params.ts` & `huble-0.2.283/src/huble/sklearn/essentials/essentail_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/essentials/function.py` & `huble-0.2.283/src/huble/sklearn/essentials/function.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/essentials/handler.py` & `huble-0.2.283/src/huble/sklearn/essentials/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/evaluate.py` & `huble-0.2.283/src/huble/sklearn/evaluate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/generate.py` & `huble-0.2.283/src/huble/sklearn/generate.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/graph.py` & `huble-0.2.283/src/huble/sklearn/graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/metrics/metrics.py` & `huble-0.2.283/src/huble/sklearn/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/process/__init__.py` & `huble-0.2.283/src/huble/sklearn/process/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/process/functions.py` & `huble-0.2.283/src/huble/sklearn/process/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/process/handler.py` & `huble-0.2.283/src/huble/sklearn/process/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/process/preprocess_params.ts` & `huble-0.2.283/src/huble/sklearn/process/preprocess_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/train/__init__.py` & `huble-0.2.283/src/huble/sklearn/train/__init__.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/train/functions.py` & `huble-0.2.283/src/huble/sklearn/train/functions.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/train/handler.py` & `huble-0.2.283/src/huble/sklearn/train/handler.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/sklearn/train/model_params.ts` & `huble-0.2.283/src/huble/sklearn/train/model_params.ts`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/util/convert_to_reactflow_graph.py` & `huble-0.2.283/src/huble/util/convert_to_reactflow_graph.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/util/data_types.py` & `huble-0.2.283/src/huble/util/data_types.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/util/inference_pipeline.py` & `huble-0.2.283/src/huble/util/inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/util/typed_params.py` & `huble-0.2.283/src/huble/util/typed_params.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/util/verify_builder_pipeline.py` & `huble-0.2.283/src/huble/util/verify_builder_pipeline.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/src/huble/util/verify_ml.py` & `huble-0.2.283/src/huble/util/verify_ml.py`

 * *Files identical despite different names*

### Comparing `huble-0.2.282/setup.py` & `huble-0.2.283/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,14 @@
  'huble.automl',
  'huble.connector',
  'huble.error',
  'huble.sklearn',
  'huble.sklearn.essentials',
  'huble.sklearn.metrics',
  'huble.sklearn.process',
- 'huble.sklearn.temp',
- 'huble.sklearn.temp.content',
  'huble.sklearn.train',
  'huble.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -32,15 +30,15 @@
  'pydantic>=1.10.4,<2.0.0',
  'scikit-learn==1.1.2',
  'scipy>=1.7.0,<1.8.0',
  'woodwork>=0.21.1,<0.22.0']
 
 setup_kwargs = {
     'name': 'huble',
-    'version': '0.2.282',
+    'version': '0.2.283',
     'description': '',
     'long_description': '',
     'author': 'Rugz007',
     'author_email': 'rugvedsomwanshi007@gmail.com',
     'maintainer': 'Arjit Agarwal',
     'maintainer_email': 'arjitagarwal123@gmail.com',
     'url': 'None',
```

### Comparing `huble-0.2.282/PKG-INFO` & `huble-0.2.283/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huble
-Version: 0.2.282
+Version: 0.2.283
 Summary: 
 Author: Rugz007
 Author-email: rugvedsomwanshi007@gmail.com
 Maintainer: Arjit Agarwal
 Maintainer-email: arjitagarwal123@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: Programming Language :: Python :: 3
```

