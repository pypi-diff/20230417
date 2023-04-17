# Comparing `tmp/pipeline_optimizer-0.1.2.tar.gz` & `tmp/pipeline_optimizer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_optimizer-0.1.2.tar", max compression
+gzip compressed data, was "pipeline_optimizer-0.1.3.tar", max compression
```

## Comparing `pipeline_optimizer-0.1.2.tar` & `pipeline_optimizer-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.2/LICENSE
--rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.2/pipeline_optimizer/__init__.py
--rw-r--r--   0        0        0     3788 2023-04-17 01:36:06.069315 pipeline_optimizer-0.1.2/pipeline_optimizer/transformers.py
--rw-r--r--   0        0        0      789 2023-04-17 02:01:34.393052 pipeline_optimizer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7246 2023-04-17 02:01:22.581080 pipeline_optimizer-0.1.2/README.md
--rw-r--r--   0        0        0     8016 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.3/LICENSE
+-rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.3/pipeline_optimizer/__init__.py
+-rw-r--r--   0        0        0     3819 2023-04-17 02:07:26.821014 pipeline_optimizer-0.1.3/pipeline_optimizer/transformers.py
+-rw-r--r--   0        0        0      789 2023-04-17 02:07:44.909642 pipeline_optimizer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7246 2023-04-17 02:01:22.581080 pipeline_optimizer-0.1.3/README.md
+-rw-r--r--   0        0        0     8016 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.3/PKG-INFO
```

### Comparing `pipeline_optimizer-0.1.2/LICENSE` & `pipeline_optimizer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.2/pipeline_optimizer/transformers.py` & `pipeline_optimizer-0.1.3/pipeline_optimizer/transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
             return step(X, **params)
         
         if y is None:
             raise ValueError("The step function expects a 'y' argument, but 'y' is not provided. Please provide a valid 'y' argument or modify the step function to work without it.")
         
         return step(X, y.copy(), **params)
     
-    def fit(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None):
-        return self
+    def fit(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None) -> Union[pd.DataFrame, pd.Series]:
+        return X
 
     def transform(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None) -> Union[pd.DataFrame, pd.Series]:
         """Applies a series of preselected transformation steps to the input DataFrame X.
 
         Args:
             X (pd.DataFrame): DataFrame of feature vectors
             y (Optional[Union[pd.DataFrame, pd.Series]], optional): Outcome vectors. Defaults to None.
```

### Comparing `pipeline_optimizer-0.1.2/pyproject.toml` & `pipeline_optimizer-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-optimizer"
-version = "0.1.2"
+version = "0.1.3"
 description = "Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions."
 authors = ["Stanislav Kharchenko"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pipeline_optimizer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pipeline_optimizer-0.1.2/README.md` & `pipeline_optimizer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.2/PKG-INFO` & `pipeline_optimizer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-optimizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions.
 License: MIT
 Author: Stanislav Kharchenko
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.2 Summary: Pipeline
+Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.3 Summary: Pipeline
 Optimizer is a Python library that aims to simplify and automate the machine
 learning pipeline, from preprocessing and testing to deployment. By providing a
 reusable infrastructure, the library allows you to manage custom preprocessing
 functions and reuse them effortlessly during the deployment of your project.
 This is particularly useful when dealing with a large number of custom
 functions. License: MIT Author: Stanislav Kharchenko Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
```

