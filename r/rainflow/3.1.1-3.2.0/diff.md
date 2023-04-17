# Comparing `tmp/rainflow-3.1.1.tar.gz` & `tmp/rainflow-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainflow-3.1.1.tar", max compression
+gzip compressed data, was "rainflow-3.2.0.tar", max compression
```

## Comparing `rainflow-3.1.1.tar` & `rainflow-3.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1074 2021-12-28 13:55:15.696905 rainflow-3.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2351 2021-12-28 13:55:15.696905 rainflow-3.1.1/README.md
--rw-r--r--   0        0        0     1352 2021-12-28 13:55:15.696905 rainflow-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     5436 2021-12-28 13:55:15.696905 rainflow-3.1.1/src/rainflow.py
--rw-r--r--   0        0        0     3189 2021-12-28 13:55:24.202451 rainflow-3.1.1/setup.py
--rw-r--r--   0        0        0     3686 2021-12-28 13:55:24.202817 rainflow-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-17 07:04:59.039532 rainflow-3.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2321 2023-04-17 07:04:59.039532 rainflow-3.2.0/README.md
+-rw-r--r--   0        0        0     1269 2023-04-17 07:04:59.039532 rainflow-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5267 2023-04-17 07:04:59.039532 rainflow-3.2.0/src/rainflow.py
+-rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 rainflow-3.2.0/PKG-INFO
```

### Comparing `rainflow-3.1.1/LICENSE.txt` & `rainflow-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rainflow-3.1.1/README.md` & `rainflow-3.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Rainflow
 ========
 
 [![Test rainflow](https://github.com/iamlikeme/rainflow/actions/workflows/tests.yml/badge.svg)](https://github.com/iamlikeme/rainflow/actions/workflows/tests.yml)
 
 `rainflow` is a Python implementation of the ASTM E1049-85 rainflow cycle counting
-algorythm for fatigue analysis. Supports both Python 2 and 3.
+algorythm for fatigue analysis.
 
 Installation
 ------------
 
 `rainflow` is available [on PyPI](https://pypi.org/project/rainflow/):
 
 ```
```

### Comparing `rainflow-3.1.1/pyproject.toml` & `rainflow-3.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 name = "rainflow"
-version = "3.1.1"
+version = "3.2.0"
 description = "Implementation of ASTM E1049-85 rainflow cycle counting algorithm"
 authors = ["Piotr Janiszewski <i.am.like.me@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/iamlikeme/rainflow"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 2.7",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",    
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = ">2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
-importlib_metadata = { version = "*", python = "<3.8" }
+python = ">=3.7"
 
 [tool.poetry.dev-dependencies]
 pytest = [
     { version = "~4", python = "~2.7" },
     { version = "*", python = "~3" },
     { version = "^6.2.5", python = "~3.10" },
 ]
+importlib_metadata = { version = "*", python = "<3.8" }
 more-itertools = { version = "<6", python = "~2.7" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rainflow-3.1.1/src/rainflow.py` & `rainflow-3.2.0/src/rainflow.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 Implements rainflow cycle counting algorythm for fatigue analysis
 according to section 5.4.4 in ASTM E1049-85 (2011).
 """
 from __future__ import division
 from collections import deque, defaultdict
 import math
 
-try:
-    from importlib import metadata as _importlib_metadata
-except ImportError:
-    import importlib_metadata as _importlib_metadata
-
-__version__ = _importlib_metadata.version("rainflow")
+__version__ = "3.2.0"
 
 
 def _get_round_function(ndigits=None):
     if ndigits is None:
         def func(x):
             return x
     else:
```

### Comparing `rainflow-3.1.1/PKG-INFO` & `rainflow-3.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: rainflow
-Version: 3.1.1
+Version: 3.2.0
 Summary: Implementation of ASTM E1049-85 rainflow cycle counting algorithm
 Home-page: https://github.com/iamlikeme/rainflow
 License: MIT
 Author: Piotr Janiszewski
 Author-email: i.am.like.me@gmail.com
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: importlib_metadata; python_version < "3.8"
 Project-URL: Repository, https://github.com/iamlikeme/rainflow
 Description-Content-Type: text/markdown
 
 Rainflow
 ========
 
 [![Test rainflow](https://github.com/iamlikeme/rainflow/actions/workflows/tests.yml/badge.svg)](https://github.com/iamlikeme/rainflow/actions/workflows/tests.yml)
 
 `rainflow` is a Python implementation of the ASTM E1049-85 rainflow cycle counting
-algorythm for fatigue analysis. Supports both Python 2 and 3.
+algorythm for fatigue analysis.
 
 Installation
 ------------
 
 `rainflow` is available [on PyPI](https://pypi.org/project/rainflow/):
 
 ```
```

