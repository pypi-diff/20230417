# Comparing `tmp/pipeline_optimizer-0.1.0.tar.gz` & `tmp/pipeline_optimizer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_optimizer-0.1.0.tar", max compression
+gzip compressed data, was "pipeline_optimizer-0.1.1.tar", max compression
```

## Comparing `pipeline_optimizer-0.1.0.tar` & `pipeline_optimizer-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.0/LICENSE
--rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.0/pipeline_optimizer/__init__.py
--rw-r--r--   0        0        0     3466 2023-04-16 22:20:30.504361 pipeline_optimizer-0.1.0/pipeline_optimizer/transformers.py
--rw-r--r--   0        0        0      787 2023-04-16 23:59:38.306468 pipeline_optimizer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7082 2023-04-16 23:50:07.590243 pipeline_optimizer-0.1.0/README.md
--rw-r--r--   0        0        0     7860 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-13 05:13:58.333629 pipeline_optimizer-0.1.1/LICENSE
+-rw-r--r--   0        0        0       57 2023-04-15 02:02:16.182399 pipeline_optimizer-0.1.1/pipeline_optimizer/__init__.py
+-rw-r--r--   0        0        0     3466 2023-04-16 22:20:30.504361 pipeline_optimizer-0.1.1/pipeline_optimizer/transformers.py
+-rw-r--r--   0        0        0      789 2023-04-17 00:16:11.427465 pipeline_optimizer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7082 2023-04-16 23:50:07.590243 pipeline_optimizer-0.1.1/README.md
+-rw-r--r--   0        0        0     7865 1970-01-01 00:00:00.000000 pipeline_optimizer-0.1.1/PKG-INFO
```

### Comparing `pipeline_optimizer-0.1.0/LICENSE` & `pipeline_optimizer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.0/pipeline_optimizer/transformers.py` & `pipeline_optimizer-0.1.1/pipeline_optimizer/transformers.py`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.0/pyproject.toml` & `pipeline_optimizer-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pipeline-optimizer"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions."
 authors = ["Stanislav Kharchenko"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pipeline_optimizer"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-sklearn = "^0.0.post4"
+scikit-learn = "^0.24.0"
 pandas = "^2.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pipeline_optimizer-0.1.0/README.md` & `pipeline_optimizer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_optimizer-0.1.0/PKG-INFO` & `pipeline_optimizer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pipeline-optimizer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pipeline Optimizer is a Python library that aims to simplify and automate the machine learning pipeline, from preprocessing and testing to deployment. By providing a reusable infrastructure, the library allows you to manage custom preprocessing functions and reuse them effortlessly during the deployment of your project. This is particularly useful when dealing with a large number of custom functions.
 License: MIT
 Author: Stanislav Kharchenko
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: sklearn (>=0.0.post4,<0.1)
+Requires-Dist: scikit-learn (>=0.24.0,<0.25.0)
 Description-Content-Type: text/markdown
 
 
 ![pipe-logo](https://user-images.githubusercontent.com/84877088/232350231-c115e4bf-700a-4b54-82bb-682dcd85e202.png)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.0 Summary: Pipeline
+Metadata-Version: 2.1 Name: pipeline-optimizer Version: 0.1.1 Summary: Pipeline
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
-Python :: 3.11 Requires-Dist: pandas (>=2.0.0,<3.0.0) Requires-Dist: sklearn
-(>=0.0.post4,<0.1) Description-Content-Type: text/markdown ![pipe-logo](https:/
-/user-images.githubusercontent.com/84877088/232350231-c115e4bf-700a-4b54-82bb-
-682dcd85e202.png) # Pipeline Optimizer [![Tests and Coverage](https://
-github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml/badge.svg)]
+Python :: 3.11 Requires-Dist: pandas (>=2.0.0,<3.0.0) Requires-Dist: scikit-
+learn (>=0.24.0,<0.25.0) Description-Content-Type: text/markdown ![pipe-logo]
+(https://user-images.githubusercontent.com/84877088/232350231-c115e4bf-700a-
+4b54-82bb-682dcd85e202.png) # Pipeline Optimizer [![Tests and Coverage](https:/
+/github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml/badge.svg)]
 (https://github.com/sk8997/pipeline-optimizer/actions/workflows/tests.yml)
 [https://codecov.io/gh/sk8997/pipeline-optimizer/branch/main/graph/
 badge.svg?token=BCWYCTXZPA] Pipeline Optimizer is a Python library that aims to
 simplify and automate the machine learning pipeline, from preprocessing and
 testing to deployment. By providing a reusable infrastructure, the library
 allows you to manage custom preprocessing functions and reuse them effortlessly
 during the deployment of your project. This is particularly useful when dealing
```

