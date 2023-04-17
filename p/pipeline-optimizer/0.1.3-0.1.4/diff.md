# Comparing `tmp/pipeline_optimizer-0.1.3.tar.gz` & `tmp/pipeline_optimizer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_optimizer-0.1.3.tar", max compression
+gzip compressed data, was "pipeline_optimizer-0.1.4.tar", max compression
```

## Comparing `pipeline_optimizer-0.1.3.tar` & `pipeline_optimizer-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.3/LICENSE
--rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.3/pipeline_optimizer/__init__.py
--rw-r--r--   0        0        0     3819 2023-04-17 02:07:26.821014 pipeline_optimizer-0.1.3/pipeline_optimizer/transformers.py
--rw-r--r--   0        0        0      789 2023-04-17 02:07:44.909642 pipeline_optimizer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7246 2023-04-17 02:01:22.581080 pipeline_optimizer-0.1.3/README.md
--rw-r--r--   0        0        0     8016 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.4/LICENSE
+-rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.4/pipeline_optimizer/__init__.py
+-rw-r--r--   0        0        0     3732 2023-04-17 02:14:54.770549 pipeline_optimizer-0.1.4/pipeline_optimizer/transformers.py
+-rw-r--r--   0        0        0      789 2023-04-17 02:14:50.880891 pipeline_optimizer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7246 2023-04-17 02:01:22.581080 pipeline_optimizer-0.1.4/README.md
+-rw-r--r--   0        0        0     8016 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.4/PKG-INFO
```

### Comparing `pipeline_optimizer-0.1.3/LICENSE` & `pipeline_optimizer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.3/pipeline_optimizer/transformers.py` & `pipeline_optimizer-0.1.4/pipeline_optimizer/transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 import pickle
 
 @dataclass
 class SequentialTransformer(BaseEstimator, TransformerMixin):
     steps: List[Callable] = field(default_factory=list)
     params: Dict[Callable, dict] = field(default_factory=dict)
 
+    def fit(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None):
+        return self
+
     @staticmethod
     def _apply_step(step: Callable, params: dict, X: pd.DataFrame, y: Optional[pd.Series] = None) -> Union[pd.DataFrame, pd.Series]:
         step_signature = inspect.signature(step)
 
         if 'y' not in step_signature.parameters:
             return step(X, **params)
         
         if y is None:
             raise ValueError("The step function expects a 'y' argument, but 'y' is not provided. Please provide a valid 'y' argument or modify the step function to work without it.")
         
         return step(X, y.copy(), **params)
     
-    def fit(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None) -> Union[pd.DataFrame, pd.Series]:
-        return X
 
-    def transform(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None) -> Union[pd.DataFrame, pd.Series]:
+    def transform(self, X: pd.DataFrame) -> Union[pd.DataFrame, pd.Series]:
         """Applies a series of preselected transformation steps to the input DataFrame X.
 
         Args:
             X (pd.DataFrame): DataFrame of feature vectors
             y (Optional[Union[pd.DataFrame, pd.Series]], optional): Outcome vectors. Defaults to None.
 
         Raises:
@@ -44,20 +45,20 @@
 
         X_copy = X.copy()
         for step in self.steps:
             if not callable(step):
                 raise ValueError("Expected a callable object (function/method) in 'steps' list, but encountered a non-callable object.")
             
             step_params = self.params.get(step, {})
-            X_copy = self._apply_step(step, step_params, X_copy, y)
+            X_copy = self._apply_step(step, step_params, X_copy)
 
         return X_copy
     
     def fit_transform(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None) -> Union[pd.DataFrame, pd.Series]:
-        return self.transform(X, y)
+        return self.transform(X)
 
     def _add(self, step: Callable, params: Optional[dict] = None) -> None:
         self.steps.append(step)
 
         if params:
             self.params[step] = params
```

### Comparing `pipeline_optimizer-0.1.3/pyproject.toml` & `pipeline_optimizer-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-optimizer"
-version = "0.1.3"
+version = "0.1.4"
 description = "Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions."
 authors = ["Stanislav Kharchenko"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pipeline_optimizer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pipeline_optimizer-0.1.3/README.md` & `pipeline_optimizer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.3/PKG-INFO` & `pipeline_optimizer-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-optimizer
-Version: 0.1.3
+Version: 0.1.4
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
-Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.3 Summary: Pipeline
+Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.4 Summary: Pipeline
 Optimizer is a Python library that aims to simplify and automate the machine
 learning pipeline, from preprocessing and testing to deployment. By providing a
 reusable infrastructure, the library allows you to manage custom preprocessing
 functions and reuse them effortlessly during the deployment of your project.
 This is particularly useful when dealing with a large number of custom
 functions. License: MIT Author: Stanislav Kharchenko Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
```

