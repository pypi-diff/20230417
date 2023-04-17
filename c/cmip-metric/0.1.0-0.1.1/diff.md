# Comparing `tmp/cmip_metric-0.1.0.tar.gz` & `tmp/cmip_metric-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmip_metric-0.1.0.tar", max compression
+gzip compressed data, was "cmip_metric-0.1.1.tar", max compression
```

## Comparing `cmip_metric-0.1.0.tar` & `cmip_metric-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1365 2023-01-29 14:04:35.677059 cmip_metric-0.1.0/README.md
--rw-r--r--   0        0        0       36 2023-04-17 14:01:39.324623 cmip_metric-0.1.0/cmip_metric/__init__.py
--rw-r--r--   0        0        0     2209 2023-04-17 14:01:59.074884 cmip_metric-0.1.0/cmip_metric/divergence.py
--rw-r--r--   0        0        0     1292 2023-01-29 12:43:23.552574 cmip_metric-0.1.0/cmip_metric/knn.py
--rw-r--r--   0        0        0     2064 2023-04-17 14:01:50.236864 cmip_metric-0.1.0/cmip_metric/metric.py
--rw-r--r--   0        0        0      966 2023-01-29 13:10:10.389442 cmip_metric-0.1.0/cmip_metric/util.py
--rw-r--r--   0        0        0      352 2023-04-17 14:00:26.512794 cmip_metric-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 cmip_metric-0.1.0/setup.py
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 cmip_metric-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1372 2023-04-17 14:05:00.034745 cmip_metric-0.1.1/README.md
+-rw-r--r--   0        0        0       36 2023-04-17 14:01:39.324623 cmip_metric-0.1.1/cmip_metric/__init__.py
+-rw-r--r--   0        0        0     2209 2023-04-17 14:01:59.074884 cmip_metric-0.1.1/cmip_metric/divergence.py
+-rw-r--r--   0        0        0     1292 2023-01-29 12:43:23.552574 cmip_metric-0.1.1/cmip_metric/knn.py
+-rw-r--r--   0        0        0     2064 2023-04-17 14:01:50.236864 cmip_metric-0.1.1/cmip_metric/metric.py
+-rw-r--r--   0        0        0      966 2023-01-29 13:10:10.389442 cmip_metric-0.1.1/cmip_metric/util.py
+-rw-r--r--   0        0        0      352 2023-04-17 14:06:40.743716 cmip_metric-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 cmip_metric-0.1.1/setup.py
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 cmip_metric-0.1.1/PKG-INFO
```

### Comparing `cmip_metric-0.1.0/README.md` & `cmip_metric-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Relevance scores of a new policy (in this case, strongly dependent on logging policy) 
 y_predict = y_logging_policy + np.random.randn(n_queries, n_results)
 # Number of documents per query, used for masking
 n = np.full(n_queries, n_results)
 ```
 
 ```Python
-from cmip import CMIP
+from cmip_metric import CMIP
 
 metric = CMIP()
 metric(y_predict, y_logging_policy, y_true, n)
 > 0.2687 # The policy predicting y_predict is not debiased w.r.t. the logging policy.
 ```
 ## Installation
 The package will be made available on [pypi](https://pypi.org/) on acceptance.
```

### Comparing `cmip_metric-0.1.0/cmip_metric/divergence.py` & `cmip_metric-0.1.1/cmip_metric/divergence.py`

 * *Files identical despite different names*

### Comparing `cmip_metric-0.1.0/cmip_metric/knn.py` & `cmip_metric-0.1.1/cmip_metric/knn.py`

 * *Files identical despite different names*

### Comparing `cmip_metric-0.1.0/cmip_metric/metric.py` & `cmip_metric-0.1.1/cmip_metric/metric.py`

 * *Files identical despite different names*

### Comparing `cmip_metric-0.1.0/cmip_metric/util.py` & `cmip_metric-0.1.1/cmip_metric/util.py`

 * *Files identical despite different names*

### Comparing `cmip_metric-0.1.0/setup.py` & `cmip_metric-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['lightgbm>=3.3.5,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'scikit-learn>=1.2.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'cmip-metric',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# CMIP - Conditional Mutual Information with the logging Policy\nCMIP implementation for the paper: `An Offline Metric for the Debiasedness of Click Models`, currently under review at SIGIR 2023.\n\nThe metric quantifies the mutual information between a new click model policy and the production system that collected the train dataset (logging policy), conditional on human relevance judgments. CMIP quantifies the degree of debiasedness (see paper for details). A policy is said to be debiased w.r.t. its logging policy with a `cmip <= 0`.  \n\n## Example\n```Python\nimport numpy as np\n\nn_queries = 1_000\nn_results = 25\n\n# Human relevance annotations per query-document pair\ny_true = np.random.randint(5, size=(n_queries, n_results))\n# Relevance scores of the logging policy\ny_logging_policy = y_true + np.random.randn(n_queries, n_results)\n# Relevance scores of a new policy (in this case, strongly dependent on logging policy) \ny_predict = y_logging_policy + np.random.randn(n_queries, n_results)\n# Number of documents per query, used for masking\nn = np.full(n_queries, n_results)\n```\n\n```Python\nfrom cmip import CMIP\n\nmetric = CMIP()\nmetric(y_predict, y_logging_policy, y_true, n)\n> 0.2687 # The policy predicting y_predict is not debiased w.r.t. the logging policy.\n```\n## Installation\nThe package will be made available on [pypi](https://pypi.org/) on acceptance.\n',
+    'long_description': '# CMIP - Conditional Mutual Information with the logging Policy\nCMIP implementation for the paper: `An Offline Metric for the Debiasedness of Click Models`, currently under review at SIGIR 2023.\n\nThe metric quantifies the mutual information between a new click model policy and the production system that collected the train dataset (logging policy), conditional on human relevance judgments. CMIP quantifies the degree of debiasedness (see paper for details). A policy is said to be debiased w.r.t. its logging policy with a `cmip <= 0`.  \n\n## Example\n```Python\nimport numpy as np\n\nn_queries = 1_000\nn_results = 25\n\n# Human relevance annotations per query-document pair\ny_true = np.random.randint(5, size=(n_queries, n_results))\n# Relevance scores of the logging policy\ny_logging_policy = y_true + np.random.randn(n_queries, n_results)\n# Relevance scores of a new policy (in this case, strongly dependent on logging policy) \ny_predict = y_logging_policy + np.random.randn(n_queries, n_results)\n# Number of documents per query, used for masking\nn = np.full(n_queries, n_results)\n```\n\n```Python\nfrom cmip_metric import CMIP\n\nmetric = CMIP()\nmetric(y_predict, y_logging_policy, y_true, n)\n> 0.2687 # The policy predicting y_predict is not debiased w.r.t. the logging policy.\n```\n## Installation\nThe package will be made available on [pypi](https://pypi.org/) on acceptance.\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cmip_metric-0.1.0/PKG-INFO` & `cmip_metric-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmip-metric
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lightgbm (>=3.3.5,<4.0.0)
@@ -31,15 +31,15 @@
 # Relevance scores of a new policy (in this case, strongly dependent on logging policy) 
 y_predict = y_logging_policy + np.random.randn(n_queries, n_results)
 # Number of documents per query, used for masking
 n = np.full(n_queries, n_results)
 ```
 
 ```Python
-from cmip import CMIP
+from cmip_metric import CMIP
 
 metric = CMIP()
 metric(y_predict, y_logging_policy, y_true, n)
 > 0.2687 # The policy predicting y_predict is not debiased w.r.t. the logging policy.
 ```
 ## Installation
 The package will be made available on [pypi](https://pypi.org/) on acceptance.
```

