# Comparing `tmp/pipeline_optimizer-0.1.1.tar.gz` & `tmp/pipeline_optimizer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_optimizer-0.1.1.tar", max compression
+gzip compressed data, was "pipeline_optimizer-0.1.2.tar", max compression
```

## Comparing `pipeline_optimizer-0.1.1.tar` & `pipeline_optimizer-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.1/LICENSE
--rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.1/pipeline_optimizer/__init__.py
--rw-r--r--   0        0        0     3466 2023-04-16 22:20:30.504361 pipeline_optimizer-0.1.1/pipeline_optimizer/transformers.py
--rw-r--r--   0        0        0      789 2023-04-17 00:16:11.427465 pipeline_optimizer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7082 2023-04-16 23:50:07.590243 pipeline_optimizer-0.1.1/README.md
--rw-r--r--   0        0        0     7865 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.2/LICENSE
+-rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.2/pipeline_optimizer/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-17 01:36:06.069315 pipeline_optimizer-0.1.2/pipeline_optimizer/transformers.py
+-rw-r--r--   0        0        0      789 2023-04-17 02:01:34.393052 pipeline_optimizer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7246 2023-04-17 02:01:22.581080 pipeline_optimizer-0.1.2/README.md
+-rw-r--r--   0        0        0     8016 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.2/PKG-INFO
```

### Comparing `pipeline_optimizer-0.1.1/LICENSE` & `pipeline_optimizer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.1/pipeline_optimizer/transformers.py` & `pipeline_optimizer-0.1.2/pipeline_optimizer/transformers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from dataclasses import dataclass, field
 from typing import Callable, Optional, List, Union, Dict
 import pandas as pd
-from sklearn.base import TransformerMixin
+from sklearn.base import TransformerMixin, BaseEstimator
 import inspect
 import pickle
 
 @dataclass
-class SequentialTransformer(TransformerMixin):
+class SequentialTransformer(BaseEstimator, TransformerMixin):
     steps: List[Callable] = field(default_factory=list)
     params: Dict[Callable, dict] = field(default_factory=dict)
 
     @staticmethod
     def _apply_step(step: Callable, params: dict, X: pd.DataFrame, y: Optional[pd.Series] = None) -> Union[pd.DataFrame, pd.Series]:
         step_signature = inspect.signature(step)
 
         if 'y' not in step_signature.parameters:
             return step(X, **params)
         
         if y is None:
             raise ValueError("The step function expects a 'y' argument, but 'y' is not provided. Please provide a valid 'y' argument or modify the step function to work without it.")
         
         return step(X, y.copy(), **params)
+    
+    def fit(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None):
+        return self
 
     def transform(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None) -> Union[pd.DataFrame, pd.Series]:
         """Applies a series of preselected transformation steps to the input DataFrame X.
 
         Args:
             X (pd.DataFrame): DataFrame of feature vectors
             y (Optional[Union[pd.DataFrame, pd.Series]], optional): Outcome vectors. Defaults to None.
@@ -44,14 +47,17 @@
             if not callable(step):
                 raise ValueError("Expected a callable object (function/method) in 'steps' list, but encountered a non-callable object.")
             
             step_params = self.params.get(step, {})
             X_copy = self._apply_step(step, step_params, X_copy, y)
 
         return X_copy
+    
+    def fit_transform(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None) -> Union[pd.DataFrame, pd.Series]:
+        return self.transform(X, y)
 
     def _add(self, step: Callable, params: Optional[dict] = None) -> None:
         self.steps.append(step)
 
         if params:
             self.params[step] = params
```

### Comparing `pipeline_optimizer-0.1.1/pyproject.toml` & `pipeline_optimizer-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-optimizer"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions."
 authors = ["Stanislav Kharchenko"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pipeline_optimizer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pipeline_optimizer-0.1.1/README.md` & `pipeline_optimizer-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 
-![pipe-logo](https://user-images.githubusercontent.com/84877088/232350231-c115e4bf-700a-4b54-82bb-682dcd85e202.png)
+
+
+![pipe-logo](https://user-images.githubusercontent.com/84877088/232358047-f8545063-5053-4a9e-a24e-e9c266283f5d.png)
 
 
 
-# Pipeline Optimizer
 
 [![Tests and Coverage](https://github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml/badge.svg)](https://github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml)
 <a href="https://codecov.io/gh/sk8997/pipeline-optimizer" > 
  <img src="https://codecov.io/gh/sk8997/pipeline-optimizer/branch/main/graph/badge.svg?token=BCWYCTXZPA"/> 
  </a>
 
 
 Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions.
 
 The library currently features a single class called `SequentialTransformer` which allows you to add custom preprocessing functions using a simple decorator. This class also integrates with scikit-learn's `TransformerMixin`, making it compatible with the widely-used scikit-learn library.
 
+# Installation
+
+```bash
+pip install pipeline_optimizer
+```
+
 # SequentialTransformer
 
 `SequentialTransformer` is a class that stores a list of preprocessing steps and applies them sequentially to input data. You can easily add a custom preprocessing function to its memory using the `@add_step` decorator. The class also provides methods to transform the input data, save the transformer to disk, and load it for later use.
 
 
 Here's a quick demonstration of how to use the `SequentialTransformer` class:
 
@@ -132,27 +139,33 @@
 
 By incorporating the `SequentialTransformer` into an sklearn `Pipeline`, you can benefit from the full range of features provided by scikit-learn, such as cross-validation, grid search, and model evaluation.
 
 Here's a quick example of how to integrate initialized `SequentialTransformer` with an sklearn `Pipeline`:
 
 ```python
 
-from sklearn.pipeline import Pipeline
-from sklearn.linear_model import LogisticRegression
-from sklearn.model_selection import train_test_split
-from sklearn.metrics import accuracy_score
+pipe = SequentialTransformer()
+
+@add_step(pipe)
+def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame:
+    return df.drop(columns=[col])
+
+@add_step(pipe)
+def multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame:
+    df[col] = df[col] * multiplier
+    return df
 
 # Create an sklearn pipeline with the custom SequentialTransformer and a LogisticRegression estimator
 pipeline = Pipeline([
     ("preprocessor", pipe),  # Ensure the SequentialTransformer has been initialized and steps have been added
     ("classifier", LogisticRegression())
 ])
 
 # Fit the pipeline to the training data
-pipeline.fit(X_train, y_train)
+pipeline.fit_transform(X_train, y_train)
 
 # Make predictions
 y_pred = pipeline.predict(X_test)
 
 ```
```

#### html2text {}

```diff
@@ -1,85 +1,87 @@
- ![pipe-logo](https://user-images.githubusercontent.com/84877088/232350231-
-c115e4bf-700a-4b54-82bb-682dcd85e202.png) # Pipeline Optimizer [![Tests and
-Coverage](https://github.com/sk8997/pipeline-optimizer/actions/workflows/
-tests.yml/badge.svg)](https://github.com/sk8997/pipeline-optimizer/actions/
-workflows/tests.yml) [https://codecov.io/gh/sk8997/pipeline-optimizer/branch/
-main/graph/badge.svg?token=BCWYCTXZPA] Pipeline Optimizer is a Python library
-that aims to simplify and automate the machine learning pipeline, from
-preprocessing and testing to deployment. By providing a reusable
-infrastructure, the library allows you to manage custom preprocessing functions
-and reuse them effortlessly during the deployment of your project. This is
-particularly useful when dealing with a large number of custom functions. The
-library currently features a single class called `SequentialTransformer` which
-allows you to add custom preprocessing functions using a simple decorator. This
-class also integrates with scikit-learn's `TransformerMixin`, making it
-compatible with the widely-used scikit-learn library. # SequentialTransformer
-`SequentialTransformer` is a class that stores a list of preprocessing steps
-and applies them sequentially to input data. You can easily add a custom
-preprocessing function to its memory using the `@add_step` decorator. The class
-also provides methods to transform the input data, save the transformer to
-disk, and load it for later use. Here's a quick demonstration of how to use the
-`SequentialTransformer` class: # Step 1: Import necessary libraries ```python
-import pandas as pd from pipeline_optimizer import SequentialTransformer,
-add_step ``` # Step 2: Load your dataset ```python data = pd.DataFrame({ "A":
-[1, 2, 3, 4, 5], "B": [5, 4, 3, 2, 1], "C": [10, 20, 30, 40, 50] }) labels =
-pd.Series([0, 1, 0, 1, 1]) ``` # Step 3: Define preprocessing functions and add
-them to the pipeline ```python pipe = SequentialTransformer() @add_step(pipe)
+ ![pipe-logo](https://user-images.githubusercontent.com/84877088/232358047-
+f8545063-5053-4a9e-a24e-e9c266283f5d.png) [![Tests and Coverage](https://
+github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml/badge.svg)]
+(https://github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml)
+[https://codecov.io/gh/sk8997/pipeline-optimizer/branch/main/graph/
+badge.svg?token=BCWYCTXZPA] Pipeline Optimizer is a Python library that aims to
+simplify and automate the machine learning pipeline, from preprocessing and
+testing to deployment. By providing a reusable infrastructure, the library
+allows you to manage custom preprocessing functions and reuse them effortlessly
+during the deployment of your project. This is particularly useful when dealing
+with a large number of custom functions. The library currently features a
+single class called `SequentialTransformer` which allows you to add custom
+preprocessing functions using a simple decorator. This class also integrates
+with scikit-learn's `TransformerMixin`, making it compatible with the widely-
+used scikit-learn library. # Installation ```bash pip install
+pipeline_optimizer ``` # SequentialTransformer `SequentialTransformer` is a
+class that stores a list of preprocessing steps and applies them sequentially
+to input data. You can easily add a custom preprocessing function to its memory
+using the `@add_step` decorator. The class also provides methods to transform
+the input data, save the transformer to disk, and load it for later use. Here's
+a quick demonstration of how to use the `SequentialTransformer` class: # Step
+1: Import necessary libraries ```python import pandas as pd from
+pipeline_optimizer import SequentialTransformer, add_step ``` # Step 2: Load
+your dataset ```python data = pd.DataFrame({ "A": [1, 2, 3, 4, 5], "B": [5, 4,
+3, 2, 1], "C": [10, 20, 30, 40, 50] }) labels = pd.Series([0, 1, 0, 1, 1]) ```
+# Step 3: Define preprocessing functions and add them to the pipeline ```python
+pipe = SequentialTransformer() @add_step(pipe) def drop_column(df:
+pd.DataFrame, col: str) -> pd.DataFrame: return df.drop(columns=[col])
+@add_step(pipe) def multiply(df: pd.DataFrame, col: str, multiplier: float) -
+> pd.DataFrame: df[col] = df[col] * multiplier return df ``` # Step 4:
+Transform the input data After applying the preprocessing functions, the
+SequentialTransformer will drop column "B" and multiply column "A" by 2.
+```python transformed_data = pipe.transform(data) print(transformed_data) ```
+Output: ``` A C 0 2 10 1 4 20 2 6 30 3 8 40 4 10 50 ``` # Step 5: Save the
+transformer object ```python pipe.save("transformer.pkl") ``` # Step 6: Load
+the saved transformer and apply it to deployment data You can load the saved
+transformer using the pickle module and apply it to new deployment data to
+preprocess it. ```python import pickle # Load the saved transformer with open
+("transformer.pkl", "rb") as f: loaded_pipe = pickle.load(f) # Deployment data
+deployment_data = pd.DataFrame({ "A": [6], "B": [3], "C": [60] }) # Transform
+the deployment data using the loaded transformer transformed_deployment_data =
+loaded_pipe.transform(deployment_data) print(transformed_deployment_data) ```
+Output: ``` A C 0 12 60 ``` # Integration with scikit-learn Pipeline A
+noteworthy feature of the `SequentialTransformer` is that it can be seamlessly
+integrated with scikit-learn's `Pipeline` class. This further simplifies the
+preprocessing and deployment processes, enabling you to create an end-to-end
+machine learning pipeline that combines custom preprocessing steps with scikit-
+learn estimators. By incorporating the `SequentialTransformer` into an sklearn
+`Pipeline`, you can benefit from the full range of features provided by scikit-
+learn, such as cross-validation, grid search, and model evaluation. Here's a
+quick example of how to integrate initialized `SequentialTransformer` with an
+sklearn `Pipeline`: ```python pipe = SequentialTransformer() @add_step(pipe)
 def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame: return df.drop
 (columns=[col]) @add_step(pipe) def multiply(df: pd.DataFrame, col: str,
-multiplier: float) -> pd.DataFrame: df[col] = df[col] * multiplier return df
-``` # Step 4: Transform the input data After applying the preprocessing
-functions, the SequentialTransformer will drop column "B" and multiply column
-"A" by 2. ```python transformed_data = pipe.transform(data) print
-(transformed_data) ``` Output: ``` A C 0 2 10 1 4 20 2 6 30 3 8 40 4 10 50 ```
-# Step 5: Save the transformer object ```python pipe.save("transformer.pkl")
-``` # Step 6: Load the saved transformer and apply it to deployment data You
-can load the saved transformer using the pickle module and apply it to new
-deployment data to preprocess it. ```python import pickle # Load the saved
-transformer with open("transformer.pkl", "rb") as f: loaded_pipe = pickle.load
-(f) # Deployment data deployment_data = pd.DataFrame({ "A": [6], "B": [3], "C":
-[60] }) # Transform the deployment data using the loaded transformer
-transformed_deployment_data = loaded_pipe.transform(deployment_data) print
-(transformed_deployment_data) ``` Output: ``` A C 0 12 60 ``` # Integration
-with scikit-learn Pipeline A noteworthy feature of the `SequentialTransformer`
-is that it can be seamlessly integrated with scikit-learn's `Pipeline` class.
-This further simplifies the preprocessing and deployment processes, enabling
-you to create an end-to-end machine learning pipeline that combines custom
-preprocessing steps with scikit-learn estimators. By incorporating the
-`SequentialTransformer` into an sklearn `Pipeline`, you can benefit from the
-full range of features provided by scikit-learn, such as cross-validation, grid
-search, and model evaluation. Here's a quick example of how to integrate
-initialized `SequentialTransformer` with an sklearn `Pipeline`: ```python from
-sklearn.pipeline import Pipeline from sklearn.linear_model import
-LogisticRegression from sklearn.model_selection import train_test_split from
-sklearn.metrics import accuracy_score # Create an sklearn pipeline with the
-custom SequentialTransformer and a LogisticRegression estimator pipeline =
-Pipeline([ ("preprocessor", pipe), # Ensure the SequentialTransformer has been
-initialized and steps have been added ("classifier", LogisticRegression()) ]) #
-Fit the pipeline to the training data pipeline.fit(X_train, y_train) # Make
-predictions y_pred = pipeline.predict(X_test) ``` # Comparison with scikit-
-learn When working with custom preprocessing functions using the scikit-learn
-library, you would typically define a custom class that inherits from
-`TransformerMixin` and implement `fit` and `transform` methods for each
-function. This can be time-consuming and may lead to code duplication.
-Alternatively, you can use scikit-learn's `FunctionTransformer` to create
-transformers from user-defined functions. However, using `FunctionTransformer`
-can become unwieldy when you have many preprocessing functions, as you need to
-create an instance of `FunctionTransformer` for each function and manage them
-individually. Here's an example of how you would use `FunctionTransformer` to
-accomplish the same preprocessing steps as in the previous example: ```python
-from sklearn.preprocessing import FunctionTransformer # Define the
-preprocessing functions def drop_column(df: pd.DataFrame, col: str) -
-> pd.DataFrame: return df.drop(columns=[col]) def multiply(df: pd.DataFrame,
-col: str, multiplier: float) -> pd.DataFrame: df[col] = df[col] * multiplier
-return df # Create FunctionTransformer instances for each function
-drop_column_transformer = FunctionTransformer(drop_column, kw_args={"col":
-"B"}) multiply_transformer = FunctionTransformer(multiply, kw_args={"col": "A",
-"multiplier": 2}) # Apply the preprocessing functions to the toy dataset
-data_dropped = drop_column_transformer.transform(data) data_transformed =
+multiplier: float) -> pd.DataFrame: df[col] = df[col] * multiplier return df #
+Create an sklearn pipeline with the custom SequentialTransformer and a
+LogisticRegression estimator pipeline = Pipeline([ ("preprocessor", pipe), #
+Ensure the SequentialTransformer has been initialized and steps have been added
+("classifier", LogisticRegression()) ]) # Fit the pipeline to the training data
+pipeline.fit_transform(X_train, y_train) # Make predictions y_pred =
+pipeline.predict(X_test) ``` # Comparison with scikit-learn When working with
+custom preprocessing functions using the scikit-learn library, you would
+typically define a custom class that inherits from `TransformerMixin` and
+implement `fit` and `transform` methods for each function. This can be time-
+consuming and may lead to code duplication. Alternatively, you can use scikit-
+learn's `FunctionTransformer` to create transformers from user-defined
+functions. However, using `FunctionTransformer` can become unwieldy when you
+have many preprocessing functions, as you need to create an instance of
+`FunctionTransformer` for each function and manage them individually. Here's an
+example of how you would use `FunctionTransformer` to accomplish the same
+preprocessing steps as in the previous example: ```python from
+sklearn.preprocessing import FunctionTransformer # Define the preprocessing
+functions def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame: return
+df.drop(columns=[col]) def multiply(df: pd.DataFrame, col: str, multiplier:
+float) -> pd.DataFrame: df[col] = df[col] * multiplier return df # Create
+FunctionTransformer instances for each function drop_column_transformer =
+FunctionTransformer(drop_column, kw_args={"col": "B"}) multiply_transformer =
+FunctionTransformer(multiply, kw_args={"col": "A", "multiplier": 2}) # Apply
+the preprocessing functions to the toy dataset data_dropped =
+drop_column_transformer.transform(data) data_transformed =
 multiply_transformer.transform(data_dropped) ``` As you can see, using
 `FunctionTransformer` requires creating separate instances for each
 preprocessing function and managing them individually. This approach can become
 cumbersome when dealing with a large number of custom functions. In contrast,
 the `SequentialTransformer` class in the Pipeline Optimizer library provides a
 more streamlined and efficient way to manage and apply multiple preprocessing
 functions. With the Pipeline Optimizer library, you can easily define
```

### Comparing `pipeline_optimizer-0.1.1/PKG-INFO` & `pipeline_optimizer-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-optimizer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions.
 License: MIT
 Author: Stanislav Kharchenko
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,30 +12,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: scikit-learn (>=0.24.0,<0.25.0)
 Description-Content-Type: text/markdown
 
 
-![pipe-logo](https://user-images.githubusercontent.com/84877088/232350231-c115e4bf-700a-4b54-82bb-682dcd85e202.png)
+
+
+![pipe-logo](https://user-images.githubusercontent.com/84877088/232358047-f8545063-5053-4a9e-a24e-e9c266283f5d.png)
 
 
 
-# Pipeline Optimizer
 
 [![Tests and Coverage](https://github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml/badge.svg)](https://github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml)
 <a href="https://codecov.io/gh/sk8997/pipeline-optimizer" > 
  <img src="https://codecov.io/gh/sk8997/pipeline-optimizer/branch/main/graph/badge.svg?token=BCWYCTXZPA"/> 
  </a>
 
 
 Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions.
 
 The library currently features a single class called `SequentialTransformer` which allows you to add custom preprocessing functions using a simple decorator. This class also integrates with scikit-learn's `TransformerMixin`, making it compatible with the widely-used scikit-learn library.
 
+# Installation
+
+```bash
+pip install pipeline_optimizer
+```
+
 # SequentialTransformer
 
 `SequentialTransformer` is a class that stores a list of preprocessing steps and applies them sequentially to input data. You can easily add a custom preprocessing function to its memory using the `@add_step` decorator. The class also provides methods to transform the input data, save the transformer to disk, and load it for later use.
 
 
 Here's a quick demonstration of how to use the `SequentialTransformer` class:
 
@@ -149,27 +156,33 @@
 
 By incorporating the `SequentialTransformer` into an sklearn `Pipeline`, you can benefit from the full range of features provided by scikit-learn, such as cross-validation, grid search, and model evaluation.
 
 Here's a quick example of how to integrate initialized `SequentialTransformer` with an sklearn `Pipeline`:
 
 ```python
 
-from sklearn.pipeline import Pipeline
-from sklearn.linear_model import LogisticRegression
-from sklearn.model_selection import train_test_split
-from sklearn.metrics import accuracy_score
+pipe = SequentialTransformer()
+
+@add_step(pipe)
+def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame:
+    return df.drop(columns=[col])
+
+@add_step(pipe)
+def multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame:
+    df[col] = df[col] * multiplier
+    return df
 
 # Create an sklearn pipeline with the custom SequentialTransformer and a LogisticRegression estimator
 pipeline = Pipeline([
     ("preprocessor", pipe),  # Ensure the SequentialTransformer has been initialized and steps have been added
     ("classifier", LogisticRegression())
 ])
 
 # Fit the pipeline to the training data
-pipeline.fit(X_train, y_train)
+pipeline.fit_transform(X_train, y_train)
 
 # Make predictions
 y_pred = pipeline.predict(X_test)
 
 ```
```

#### html2text {}

```diff
@@ -1,86 +1,88 @@
-Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.1 Summary: Pipeline
+Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.2 Summary: Pipeline
 Optimizer is a Python library that aims to simplify and automate the machine
 learning pipeline, from preprocessing and testing to deployment. By providing a
 reusable infrastructure, the library allows you to manage custom preprocessing
 functions and reuse them effortlessly during the deployment of your project.
 This is particularly useful when dealing with a large number of custom
 functions. License: MIT Author: Stanislav Kharchenko Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: pandas (>=2.0.0,<3.0.0) Requires-Dist: scikit-
 learn (>=0.24.0,<0.25.0) Description-Content-Type: text/markdown ![pipe-logo]
-(https://user-images.githubusercontent.com/84877088/232350231-c115e4bf-700a-
-4b54-82bb-682dcd85e202.png) # Pipeline Optimizer [![Tests and Coverage](https:/
-/github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml/badge.svg)]
-(https://github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml)
-[https://codecov.io/gh/sk8997/pipeline-optimizer/branch/main/graph/
-badge.svg?token=BCWYCTXZPA] Pipeline Optimizer is a Python library that aims to
-simplify and automate the machine learning pipeline, from preprocessing and
-testing to deployment. By providing a reusable infrastructure, the library
-allows you to manage custom preprocessing functions and reuse them effortlessly
-during the deployment of your project. This is particularly useful when dealing
-with a large number of custom functions. The library currently features a
-single class called `SequentialTransformer` which allows you to add custom
-preprocessing functions using a simple decorator. This class also integrates
-with scikit-learn's `TransformerMixin`, making it compatible with the widely-
-used scikit-learn library. # SequentialTransformer `SequentialTransformer` is a
-class that stores a list of preprocessing steps and applies them sequentially
-to input data. You can easily add a custom preprocessing function to its memory
-using the `@add_step` decorator. The class also provides methods to transform
-the input data, save the transformer to disk, and load it for later use. Here's
-a quick demonstration of how to use the `SequentialTransformer` class: # Step
-1: Import necessary libraries ```python import pandas as pd from
-pipeline_optimizer import SequentialTransformer, add_step ``` # Step 2: Load
-your dataset ```python data = pd.DataFrame({ "A": [1, 2, 3, 4, 5], "B": [5, 4,
-3, 2, 1], "C": [10, 20, 30, 40, 50] }) labels = pd.Series([0, 1, 0, 1, 1]) ```
-# Step 3: Define preprocessing functions and add them to the pipeline ```python
-pipe = SequentialTransformer() @add_step(pipe) def drop_column(df:
-pd.DataFrame, col: str) -> pd.DataFrame: return df.drop(columns=[col])
-@add_step(pipe) def multiply(df: pd.DataFrame, col: str, multiplier: float) -
-> pd.DataFrame: df[col] = df[col] * multiplier return df ``` # Step 4:
-Transform the input data After applying the preprocessing functions, the
-SequentialTransformer will drop column "B" and multiply column "A" by 2.
-```python transformed_data = pipe.transform(data) print(transformed_data) ```
-Output: ``` A C 0 2 10 1 4 20 2 6 30 3 8 40 4 10 50 ``` # Step 5: Save the
-transformer object ```python pipe.save("transformer.pkl") ``` # Step 6: Load
-the saved transformer and apply it to deployment data You can load the saved
-transformer using the pickle module and apply it to new deployment data to
-preprocess it. ```python import pickle # Load the saved transformer with open
-("transformer.pkl", "rb") as f: loaded_pipe = pickle.load(f) # Deployment data
-deployment_data = pd.DataFrame({ "A": [6], "B": [3], "C": [60] }) # Transform
-the deployment data using the loaded transformer transformed_deployment_data =
-loaded_pipe.transform(deployment_data) print(transformed_deployment_data) ```
-Output: ``` A C 0 12 60 ``` # Integration with scikit-learn Pipeline A
-noteworthy feature of the `SequentialTransformer` is that it can be seamlessly
-integrated with scikit-learn's `Pipeline` class. This further simplifies the
-preprocessing and deployment processes, enabling you to create an end-to-end
-machine learning pipeline that combines custom preprocessing steps with scikit-
-learn estimators. By incorporating the `SequentialTransformer` into an sklearn
-`Pipeline`, you can benefit from the full range of features provided by scikit-
-learn, such as cross-validation, grid search, and model evaluation. Here's a
-quick example of how to integrate initialized `SequentialTransformer` with an
-sklearn `Pipeline`: ```python from sklearn.pipeline import Pipeline from
-sklearn.linear_model import LogisticRegression from sklearn.model_selection
-import train_test_split from sklearn.metrics import accuracy_score # Create an
-sklearn pipeline with the custom SequentialTransformer and a LogisticRegression
-estimator pipeline = Pipeline([ ("preprocessor", pipe), # Ensure the
-SequentialTransformer has been initialized and steps have been added
+(https://user-images.githubusercontent.com/84877088/232358047-f8545063-5053-
+4a9e-a24e-e9c266283f5d.png) [![Tests and Coverage](https://github.com/sk8997/
+pipeline-optimizer/actions/workflows/tests.yml/badge.svg)](https://github.com/
+sk8997/pipeline-optimizer/actions/workflows/tests.yml) [https://codecov.io/gh/
+sk8997/pipeline-optimizer/branch/main/graph/badge.svg?token=BCWYCTXZPA]
+Pipeline Optimizer is a Python library that aims to simplify and automate the
+machine learning pipeline, from preprocessing and testing to deployment. By
+providing a reusable infrastructure, the library allows you to manage custom
+preprocessing functions and reuse them effortlessly during the deployment of
+your project. This is particularly useful when dealing with a large number of
+custom functions. The library currently features a single class called
+`SequentialTransformer` which allows you to add custom preprocessing functions
+using a simple decorator. This class also integrates with scikit-learn's
+`TransformerMixin`, making it compatible with the widely-used scikit-learn
+library. # Installation ```bash pip install pipeline_optimizer ``` #
+SequentialTransformer `SequentialTransformer` is a class that stores a list of
+preprocessing steps and applies them sequentially to input data. You can easily
+add a custom preprocessing function to its memory using the `@add_step`
+decorator. The class also provides methods to transform the input data, save
+the transformer to disk, and load it for later use. Here's a quick
+demonstration of how to use the `SequentialTransformer` class: # Step 1: Import
+necessary libraries ```python import pandas as pd from pipeline_optimizer
+import SequentialTransformer, add_step ``` # Step 2: Load your dataset
+```python data = pd.DataFrame({ "A": [1, 2, 3, 4, 5], "B": [5, 4, 3, 2, 1],
+"C": [10, 20, 30, 40, 50] }) labels = pd.Series([0, 1, 0, 1, 1]) ``` # Step 3:
+Define preprocessing functions and add them to the pipeline ```python pipe =
+SequentialTransformer() @add_step(pipe) def drop_column(df: pd.DataFrame, col:
+str) -> pd.DataFrame: return df.drop(columns=[col]) @add_step(pipe) def
+multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame: df
+[col] = df[col] * multiplier return df ``` # Step 4: Transform the input data
+After applying the preprocessing functions, the SequentialTransformer will drop
+column "B" and multiply column "A" by 2. ```python transformed_data =
+pipe.transform(data) print(transformed_data) ``` Output: ``` A C 0 2 10 1 4 20
+2 6 30 3 8 40 4 10 50 ``` # Step 5: Save the transformer object ```python
+pipe.save("transformer.pkl") ``` # Step 6: Load the saved transformer and apply
+it to deployment data You can load the saved transformer using the pickle
+module and apply it to new deployment data to preprocess it. ```python import
+pickle # Load the saved transformer with open("transformer.pkl", "rb") as f:
+loaded_pipe = pickle.load(f) # Deployment data deployment_data = pd.DataFrame(
+{ "A": [6], "B": [3], "C": [60] }) # Transform the deployment data using the
+loaded transformer transformed_deployment_data = loaded_pipe.transform
+(deployment_data) print(transformed_deployment_data) ``` Output: ``` A C 0 12
+60 ``` # Integration with scikit-learn Pipeline A noteworthy feature of the
+`SequentialTransformer` is that it can be seamlessly integrated with scikit-
+learn's `Pipeline` class. This further simplifies the preprocessing and
+deployment processes, enabling you to create an end-to-end machine learning
+pipeline that combines custom preprocessing steps with scikit-learn estimators.
+By incorporating the `SequentialTransformer` into an sklearn `Pipeline`, you
+can benefit from the full range of features provided by scikit-learn, such as
+cross-validation, grid search, and model evaluation. Here's a quick example of
+how to integrate initialized `SequentialTransformer` with an sklearn
+`Pipeline`: ```python pipe = SequentialTransformer() @add_step(pipe) def
+drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame: return df.drop
+(columns=[col]) @add_step(pipe) def multiply(df: pd.DataFrame, col: str,
+multiplier: float) -> pd.DataFrame: df[col] = df[col] * multiplier return df #
+Create an sklearn pipeline with the custom SequentialTransformer and a
+LogisticRegression estimator pipeline = Pipeline([ ("preprocessor", pipe), #
+Ensure the SequentialTransformer has been initialized and steps have been added
 ("classifier", LogisticRegression()) ]) # Fit the pipeline to the training data
-pipeline.fit(X_train, y_train) # Make predictions y_pred = pipeline.predict
-(X_test) ``` # Comparison with scikit-learn When working with custom
-preprocessing functions using the scikit-learn library, you would typically
-define a custom class that inherits from `TransformerMixin` and implement `fit`
-and `transform` methods for each function. This can be time-consuming and may
-lead to code duplication. Alternatively, you can use scikit-learn's
-`FunctionTransformer` to create transformers from user-defined functions.
-However, using `FunctionTransformer` can become unwieldy when you have many
-preprocessing functions, as you need to create an instance of
+pipeline.fit_transform(X_train, y_train) # Make predictions y_pred =
+pipeline.predict(X_test) ``` # Comparison with scikit-learn When working with
+custom preprocessing functions using the scikit-learn library, you would
+typically define a custom class that inherits from `TransformerMixin` and
+implement `fit` and `transform` methods for each function. This can be time-
+consuming and may lead to code duplication. Alternatively, you can use scikit-
+learn's `FunctionTransformer` to create transformers from user-defined
+functions. However, using `FunctionTransformer` can become unwieldy when you
+have many preprocessing functions, as you need to create an instance of
 `FunctionTransformer` for each function and manage them individually. Here's an
 example of how you would use `FunctionTransformer` to accomplish the same
 preprocessing steps as in the previous example: ```python from
 sklearn.preprocessing import FunctionTransformer # Define the preprocessing
 functions def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame: return
 df.drop(columns=[col]) def multiply(df: pd.DataFrame, col: str, multiplier:
 float) -> pd.DataFrame: df[col] = df[col] * multiplier return df # Create
```

