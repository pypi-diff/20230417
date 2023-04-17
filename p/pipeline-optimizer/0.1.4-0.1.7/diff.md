# Comparing `tmp/pipeline_optimizer-0.1.4.tar.gz` & `tmp/pipeline_optimizer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_optimizer-0.1.4.tar", max compression
+gzip compressed data, was "pipeline_optimizer-0.1.7.tar", max compression
```

## Comparing `pipeline_optimizer-0.1.4.tar` & `pipeline_optimizer-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.4/LICENSE
--rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.4/pipeline_optimizer/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-17 02:14:54.770549 pipeline_optimizer-0.1.4/pipeline_optimizer/transformers.py
--rw-r--r--   0        0        0      789 2023-04-17 02:14:50.880891 pipeline_optimizer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     7246 2023-04-17 02:01:22.581080 pipeline_optimizer-0.1.4/README.md
--rw-r--r--   0        0        0     8016 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.7/LICENSE
+-rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.7/pipeline_optimizer/__init__.py
+-rw-r--r--   0        0        0     3464 2023-04-17 02:59:58.243039 pipeline_optimizer-0.1.7/pipeline_optimizer/transformers.py
+-rw-r--r--   0        0        0      789 2023-04-17 03:05:34.710261 pipeline_optimizer-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     7192 2023-04-17 02:39:10.108843 pipeline_optimizer-0.1.7/README.md
+-rw-r--r--   0        0        0     7964 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.7/PKG-INFO
```

### Comparing `pipeline_optimizer-0.1.4/LICENSE` & `pipeline_optimizer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.4/pipeline_optimizer/transformers.py` & `pipeline_optimizer-0.1.7/pipeline_optimizer/transformers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,20 @@
     steps: List[Callable] = field(default_factory=list)
     params: Dict[Callable, dict] = field(default_factory=dict)
 
     def fit(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None):
         return self
 
     @staticmethod
-    def _apply_step(step: Callable, params: dict, X: pd.DataFrame, y: Optional[pd.Series] = None) -> Union[pd.DataFrame, pd.Series]:
-        step_signature = inspect.signature(step)
-
-        if 'y' not in step_signature.parameters:
-            return step(X, **params)
+    def _apply_step(step: Callable, params: dict, X: pd.DataFrame) -> Union[pd.DataFrame, pd.Series]:
         
-        if y is None:
-            raise ValueError("The step function expects a 'y' argument, but 'y' is not provided. Please provide a valid 'y' argument or modify the step function to work without it.")
+        if not isinstance(X, pd.DataFrame):
+            raise ValueError("The input 'X' must be a pandas DataFrame.")
         
-        return step(X, y.copy(), **params)
+        return step(X, **params)
     
 
     def transform(self, X: pd.DataFrame) -> Union[pd.DataFrame, pd.Series]:
         """Applies a series of preselected transformation steps to the input DataFrame X.
 
         Args:
             X (pd.DataFrame): DataFrame of feature vectors
```

### Comparing `pipeline_optimizer-0.1.4/pyproject.toml` & `pipeline_optimizer-0.1.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-optimizer"
-version = "0.1.4"
+version = "0.1.7"
 description = "Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions."
 authors = ["Stanislav Kharchenko"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pipeline_optimizer"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pipeline_optimizer-0.1.4/README.md` & `pipeline_optimizer-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -56,19 +56,19 @@
 # Step 3: Define preprocessing functions and add them to the pipeline
 
 ```python
 
 pipe = SequentialTransformer()
 
 @add_step(pipe)
-def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame:
+def drop_column(df: pd.DataFrame, col: str = "B") -> pd.DataFrame:
     return df.drop(columns=[col])
 
 @add_step(pipe)
-def multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame:
+def multiply(df: pd.DataFrame, col: str = "A", multiplier: float = 2) -> pd.DataFrame:
     df[col] = df[col] * multiplier
     return df
 
 ```
 
 # Step 4: Transform the input data
 After applying the preprocessing functions, the SequentialTransformer will drop column "B" and multiply column "A" by 2.
@@ -142,33 +142,31 @@
 Here's a quick example of how to integrate initialized `SequentialTransformer` with an sklearn `Pipeline`:
 
 ```python
 
 pipe = SequentialTransformer()
 
 @add_step(pipe)
-def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame:
+def drop_column(df: pd.DataFrame, col: str = "B") -> pd.DataFrame:
     return df.drop(columns=[col])
 
 @add_step(pipe)
-def multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame:
+def multiply(df: pd.DataFrame, col: str = "A", multiplier: float = 2) -> pd.DataFrame:
     df[col] = df[col] * multiplier
     return df
 
-# Create an sklearn pipeline with the custom SequentialTransformer and a LogisticRegression estimator
+# Create an sklearn pipeline with the custom SequentialTransformer and a Linear Discriminant Analysis
 pipeline = Pipeline([
     ("preprocessor", pipe),  # Ensure the SequentialTransformer has been initialized and steps have been added
-    ("classifier", LogisticRegression())
+    ("lda", LinearDiscriminantAnalysis())
 ])
 
-# Fit the pipeline to the training data
-pipeline.fit_transform(X_train, y_train)
+# Fit the pipeline 
+pipeline.fit_transform(X, y)
 
-# Make predictions
-y_pred = pipeline.predict(X_test)
 
 ```
 
 
 # Comparison with scikit-learn
 
 When working with custom preprocessing functions using the scikit-learn library, you would typically define a custom class that inherits from `TransformerMixin` and implement `fit` and `transform` methods for each function. This can be time-consuming and may lead to code duplication.
```

#### html2text {}

```diff
@@ -21,18 +21,18 @@
 a quick demonstration of how to use the `SequentialTransformer` class: # Step
 1: Import necessary libraries ```python import pandas as pd from
 pipeline_optimizer import SequentialTransformer, add_step ``` # Step 2: Load
 your dataset ```python data = pd.DataFrame({ "A": [1, 2, 3, 4, 5], "B": [5, 4,
 3, 2, 1], "C": [10, 20, 30, 40, 50] }) labels = pd.Series([0, 1, 0, 1, 1]) ```
 # Step 3: Define preprocessing functions and add them to the pipeline ```python
 pipe = SequentialTransformer() @add_step(pipe) def drop_column(df:
-pd.DataFrame, col: str) -> pd.DataFrame: return df.drop(columns=[col])
-@add_step(pipe) def multiply(df: pd.DataFrame, col: str, multiplier: float) -
-> pd.DataFrame: df[col] = df[col] * multiplier return df ``` # Step 4:
-Transform the input data After applying the preprocessing functions, the
+pd.DataFrame, col: str = "B") -> pd.DataFrame: return df.drop(columns=[col])
+@add_step(pipe) def multiply(df: pd.DataFrame, col: str = "A", multiplier:
+float = 2) -> pd.DataFrame: df[col] = df[col] * multiplier return df ``` # Step
+4: Transform the input data After applying the preprocessing functions, the
 SequentialTransformer will drop column "B" and multiply column "A" by 2.
 ```python transformed_data = pipe.transform(data) print(transformed_data) ```
 Output: ``` A C 0 2 10 1 4 20 2 6 30 3 8 40 4 10 50 ``` # Step 5: Save the
 transformer object ```python pipe.save("transformer.pkl") ``` # Step 6: Load
 the saved transformer and apply it to deployment data You can load the saved
 transformer using the pickle module and apply it to new deployment data to
 preprocess it. ```python import pickle # Load the saved transformer with open
@@ -46,24 +46,23 @@
 preprocessing and deployment processes, enabling you to create an end-to-end
 machine learning pipeline that combines custom preprocessing steps with scikit-
 learn estimators. By incorporating the `SequentialTransformer` into an sklearn
 `Pipeline`, you can benefit from the full range of features provided by scikit-
 learn, such as cross-validation, grid search, and model evaluation. Here's a
 quick example of how to integrate initialized `SequentialTransformer` with an
 sklearn `Pipeline`: ```python pipe = SequentialTransformer() @add_step(pipe)
-def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame: return df.drop
-(columns=[col]) @add_step(pipe) def multiply(df: pd.DataFrame, col: str,
-multiplier: float) -> pd.DataFrame: df[col] = df[col] * multiplier return df #
-Create an sklearn pipeline with the custom SequentialTransformer and a
-LogisticRegression estimator pipeline = Pipeline([ ("preprocessor", pipe), #
-Ensure the SequentialTransformer has been initialized and steps have been added
-("classifier", LogisticRegression()) ]) # Fit the pipeline to the training data
-pipeline.fit_transform(X_train, y_train) # Make predictions y_pred =
-pipeline.predict(X_test) ``` # Comparison with scikit-learn When working with
-custom preprocessing functions using the scikit-learn library, you would
+def drop_column(df: pd.DataFrame, col: str = "B") -> pd.DataFrame: return
+df.drop(columns=[col]) @add_step(pipe) def multiply(df: pd.DataFrame, col: str
+= "A", multiplier: float = 2) -> pd.DataFrame: df[col] = df[col] * multiplier
+return df # Create an sklearn pipeline with the custom SequentialTransformer
+and a Linear Discriminant Analysis pipeline = Pipeline([ ("preprocessor",
+pipe), # Ensure the SequentialTransformer has been initialized and steps have
+been added ("lda", LinearDiscriminantAnalysis()) ]) # Fit the pipeline
+pipeline.fit_transform(X, y) ``` # Comparison with scikit-learn When working
+with custom preprocessing functions using the scikit-learn library, you would
 typically define a custom class that inherits from `TransformerMixin` and
 implement `fit` and `transform` methods for each function. This can be time-
 consuming and may lead to code duplication. Alternatively, you can use scikit-
 learn's `FunctionTransformer` to create transformers from user-defined
 functions. However, using `FunctionTransformer` can become unwieldy when you
 have many preprocessing functions, as you need to create an instance of
 `FunctionTransformer` for each function and manage them individually. Here's an
```

### Comparing `pipeline_optimizer-0.1.4/PKG-INFO` & `pipeline_optimizer-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-optimizer
-Version: 0.1.4
+Version: 0.1.7
 Summary: Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions.
 License: MIT
 Author: Stanislav Kharchenko
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -73,19 +73,19 @@
 # Step 3: Define preprocessing functions and add them to the pipeline
 
 ```python
 
 pipe = SequentialTransformer()
 
 @add_step(pipe)
-def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame:
+def drop_column(df: pd.DataFrame, col: str = "B") -> pd.DataFrame:
     return df.drop(columns=[col])
 
 @add_step(pipe)
-def multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame:
+def multiply(df: pd.DataFrame, col: str = "A", multiplier: float = 2) -> pd.DataFrame:
     df[col] = df[col] * multiplier
     return df
 
 ```
 
 # Step 4: Transform the input data
 After applying the preprocessing functions, the SequentialTransformer will drop column "B" and multiply column "A" by 2.
@@ -159,33 +159,31 @@
 Here's a quick example of how to integrate initialized `SequentialTransformer` with an sklearn `Pipeline`:
 
 ```python
 
 pipe = SequentialTransformer()
 
 @add_step(pipe)
-def drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame:
+def drop_column(df: pd.DataFrame, col: str = "B") -> pd.DataFrame:
     return df.drop(columns=[col])
 
 @add_step(pipe)
-def multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame:
+def multiply(df: pd.DataFrame, col: str = "A", multiplier: float = 2) -> pd.DataFrame:
     df[col] = df[col] * multiplier
     return df
 
-# Create an sklearn pipeline with the custom SequentialTransformer and a LogisticRegression estimator
+# Create an sklearn pipeline with the custom SequentialTransformer and a Linear Discriminant Analysis
 pipeline = Pipeline([
     ("preprocessor", pipe),  # Ensure the SequentialTransformer has been initialized and steps have been added
-    ("classifier", LogisticRegression())
+    ("lda", LinearDiscriminantAnalysis())
 ])
 
-# Fit the pipeline to the training data
-pipeline.fit_transform(X_train, y_train)
+# Fit the pipeline 
+pipeline.fit_transform(X, y)
 
-# Make predictions
-y_pred = pipeline.predict(X_test)
 
 ```
 
 
 # Comparison with scikit-learn
 
 When working with custom preprocessing functions using the scikit-learn library, you would typically define a custom class that inherits from `TransformerMixin` and implement `fit` and `transform` methods for each function. This can be time-consuming and may lead to code duplication.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.4 Summary: Pipeline
+Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.7 Summary: Pipeline
 Optimizer is a Python library that aims to simplify and automate the machine
 learning pipeline, from preprocessing and testing to deployment. By providing a
 reusable infrastructure, the library allows you to manage custom preprocessing
 functions and reuse them effortlessly during the deployment of your project.
 This is particularly useful when dealing with a large number of custom
 functions. License: MIT Author: Stanislav Kharchenko Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -34,49 +34,48 @@
 demonstration of how to use the `SequentialTransformer` class: # Step 1: Import
 necessary libraries ```python import pandas as pd from pipeline_optimizer
 import SequentialTransformer, add_step ``` # Step 2: Load your dataset
 ```python data = pd.DataFrame({ "A": [1, 2, 3, 4, 5], "B": [5, 4, 3, 2, 1],
 "C": [10, 20, 30, 40, 50] }) labels = pd.Series([0, 1, 0, 1, 1]) ``` # Step 3:
 Define preprocessing functions and add them to the pipeline ```python pipe =
 SequentialTransformer() @add_step(pipe) def drop_column(df: pd.DataFrame, col:
-str) -> pd.DataFrame: return df.drop(columns=[col]) @add_step(pipe) def
-multiply(df: pd.DataFrame, col: str, multiplier: float) -> pd.DataFrame: df
-[col] = df[col] * multiplier return df ``` # Step 4: Transform the input data
-After applying the preprocessing functions, the SequentialTransformer will drop
-column "B" and multiply column "A" by 2. ```python transformed_data =
-pipe.transform(data) print(transformed_data) ``` Output: ``` A C 0 2 10 1 4 20
-2 6 30 3 8 40 4 10 50 ``` # Step 5: Save the transformer object ```python
-pipe.save("transformer.pkl") ``` # Step 6: Load the saved transformer and apply
-it to deployment data You can load the saved transformer using the pickle
-module and apply it to new deployment data to preprocess it. ```python import
-pickle # Load the saved transformer with open("transformer.pkl", "rb") as f:
-loaded_pipe = pickle.load(f) # Deployment data deployment_data = pd.DataFrame(
-{ "A": [6], "B": [3], "C": [60] }) # Transform the deployment data using the
-loaded transformer transformed_deployment_data = loaded_pipe.transform
-(deployment_data) print(transformed_deployment_data) ``` Output: ``` A C 0 12
-60 ``` # Integration with scikit-learn Pipeline A noteworthy feature of the
-`SequentialTransformer` is that it can be seamlessly integrated with scikit-
-learn's `Pipeline` class. This further simplifies the preprocessing and
-deployment processes, enabling you to create an end-to-end machine learning
-pipeline that combines custom preprocessing steps with scikit-learn estimators.
-By incorporating the `SequentialTransformer` into an sklearn `Pipeline`, you
-can benefit from the full range of features provided by scikit-learn, such as
-cross-validation, grid search, and model evaluation. Here's a quick example of
-how to integrate initialized `SequentialTransformer` with an sklearn
-`Pipeline`: ```python pipe = SequentialTransformer() @add_step(pipe) def
-drop_column(df: pd.DataFrame, col: str) -> pd.DataFrame: return df.drop
-(columns=[col]) @add_step(pipe) def multiply(df: pd.DataFrame, col: str,
-multiplier: float) -> pd.DataFrame: df[col] = df[col] * multiplier return df #
-Create an sklearn pipeline with the custom SequentialTransformer and a
-LogisticRegression estimator pipeline = Pipeline([ ("preprocessor", pipe), #
-Ensure the SequentialTransformer has been initialized and steps have been added
-("classifier", LogisticRegression()) ]) # Fit the pipeline to the training data
-pipeline.fit_transform(X_train, y_train) # Make predictions y_pred =
-pipeline.predict(X_test) ``` # Comparison with scikit-learn When working with
-custom preprocessing functions using the scikit-learn library, you would
+str = "B") -> pd.DataFrame: return df.drop(columns=[col]) @add_step(pipe) def
+multiply(df: pd.DataFrame, col: str = "A", multiplier: float = 2) -
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
+def drop_column(df: pd.DataFrame, col: str = "B") -> pd.DataFrame: return
+df.drop(columns=[col]) @add_step(pipe) def multiply(df: pd.DataFrame, col: str
+= "A", multiplier: float = 2) -> pd.DataFrame: df[col] = df[col] * multiplier
+return df # Create an sklearn pipeline with the custom SequentialTransformer
+and a Linear Discriminant Analysis pipeline = Pipeline([ ("preprocessor",
+pipe), # Ensure the SequentialTransformer has been initialized and steps have
+been added ("lda", LinearDiscriminantAnalysis()) ]) # Fit the pipeline
+pipeline.fit_transform(X, y) ``` # Comparison with scikit-learn When working
+with custom preprocessing functions using the scikit-learn library, you would
 typically define a custom class that inherits from `TransformerMixin` and
 implement `fit` and `transform` methods for each function. This can be time-
 consuming and may lead to code duplication. Alternatively, you can use scikit-
 learn's `FunctionTransformer` to create transformers from user-defined
 functions. However, using `FunctionTransformer` can become unwieldy when you
 have many preprocessing functions, as you need to create an instance of
 `FunctionTransformer` for each function and manage them individually. Here's an
```

