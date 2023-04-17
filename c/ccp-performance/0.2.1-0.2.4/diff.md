# Comparing `tmp/ccp-performance-0.2.1.tar.gz` & `tmp/ccp-performance-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-jgxa_n5a/ccp-performance-0.2.1.tar", last modified: Wed Mar  1 16:35:15 2023, max compression
+gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-fr8bc0me/ccp-performance-0.2.4.tar", last modified: Mon Apr 17 13:16:56 2023, max compression
```

## Comparing `ccp-performance-0.2.1.tar` & `ccp-performance-0.2.4.tar`

### file list

```diff
@@ -1,56 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1488 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       36 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2330 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1775 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp/
--rw-r--r--   0 runner    (1001) docker     (116)     4094 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp/app/
--rw-r--r--   0 runner    (1001) docker     (116)     7927 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/app/app_engine.py
--rw-r--r--   0 runner    (1001) docker     (116)    55385 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/app/ccp_app_back_to_back.py
--rw-r--r--   0 runner    (1001) docker     (116)    10113 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/app/ccpdash.py
--rw-r--r--   0 runner    (1001) docker     (116)    39668 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/compressor.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp/config/
--rw-r--r--   0 runner    (1001) docker     (116)       46 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4131 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/config/fluids.py
--rw-r--r--   0 runner    (1001) docker     (116)       42 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/config/new_units.txt
--rw-r--r--   0 runner    (1001) docker     (116)     5950 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/config/units.py
--rw-r--r--   0 runner    (1001) docker     (116)      492 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/config/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp/cprofile/
--rw-r--r--   0 runner    (1001) docker     (116)     2825 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/cprofile/cprofile.py
--rw-r--r--   0 runner    (1001) docker     (116)     8923 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/curve.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp/data_io/
--rw-r--r--   0 runner    (1001) docker     (116)      121 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/data_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1226 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/data_io/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (116)       55 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/data_io/read_xl.py
--rw-r--r--   0 runner    (1001) docker     (116)     2943 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/fo.py
--rw-r--r--   0 runner    (1001) docker     (116)    38228 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/impeller.py
--rw-r--r--   0 runner    (1001) docker     (116)    13089 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (116)    57872 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/point.py
--rw-r--r--   0 runner    (1001) docker     (116)     1808 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/similarity.py
--rw-r--r--   0 runner    (1001) docker     (116)    24461 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/state.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)   288892 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/data/UTGCA_1231_A_1s.csv
--rw-r--r--   0 runner    (1001) docker     (116)   502046 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
--rw-r--r--   0 runner    (1001) docker     (116)     2011 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/data/lp-sec1-caso-a-eff.csv
--rw-r--r--   0 runner    (1001) docker     (116)     1960 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/data/lp-sec1-caso-a-head.csv
--rw-r--r--   0 runner    (1001) docker     (116)     1120 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/data/normal-eff.csv
--rw-r--r--   0 runner    (1001) docker     (116)      896 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/data/normal-head.csv
--rw-r--r--   0 runner    (1001) docker     (116)    38383 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_compressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     2946 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (116)      531 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_fo.py
--rw-r--r--   0 runner    (1001) docker     (116)    29427 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_impeller.py
--rw-r--r--   0 runner    (1001) docker     (116)     1366 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (116)    21702 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (116)   277769 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (116)    12743 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (116)     7972 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/ccp/tests/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp_performance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2330 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp_performance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1116 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp_performance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp_performance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      257 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp_performance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/ccp_performance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-01 16:35:15.000000 ccp-performance-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2929 2023-03-01 16:35:06.000000 ccp-performance-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_1s.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-head.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/normal-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/ccp/tests/data/normal-head.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/ccp_performance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:16:56.000000 ccp-performance-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-04-17 13:16:43.000000 ccp-performance-0.2.4/setup.py
```

### Comparing `ccp-performance-0.2.1/PKG-INFO` & `ccp-performance-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.2.1
+Version: 0.2.4
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
-Author-email: raphaelts@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+Author-email: raphaelts@petrobras.com.br
+License: Apache License 2.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ccp-performance-0.2.1/README.md` & `ccp-performance-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.1/ccp/tests/data/UTGCA_1231_A_1s.csv` & `ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_1s.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.1/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h` & `ccp-performance-0.2.4/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.1/ccp/tests/data/lp-sec1-caso-a-eff.csv` & `ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.1/ccp/tests/data/lp-sec1-caso-a-head.csv` & `ccp-performance-0.2.4/ccp/tests/data/lp-sec1-caso-a-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.1/ccp/tests/data/normal-eff.csv` & `ccp-performance-0.2.4/ccp/tests/data/normal-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.1/ccp/tests/data/normal-head.csv` & `ccp-performance-0.2.4/ccp/tests/data/normal-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.2.1/ccp_performance.egg-info/PKG-INFO` & `ccp-performance-0.2.4/ccp_performance.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.2.1
+Version: 0.2.4
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
-Author-email: raphaelts@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
+Author-email: raphaelts@petrobras.com.br
+License: Apache License 2.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `ccp-performance-0.2.1/setup.py` & `ccp-performance-0.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import io
 import os
 import re
 import sys
 
 from setuptools import setup, find_packages
 
 
 def read(path, encoding="utf-8"):
     path = os.path.join(os.path.dirname(__file__), path)
-    with io.open(path, encoding=encoding) as fp:
+    with open(path, encoding=encoding) as fp:
         return fp.read()
 
 
 def version(path):
     """Obtain the package version from a python file e.g. pkg/__init__.py
     See <https://packaging.python.org/en/latest/single_source_version.html>.
     """
@@ -34,41 +33,32 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+    with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
-REQUIRES = [
-        "numpy",
-        "scipy",
-        "CoolProp",
-        "pint>=0.18",
-        "plotly",
-        "toml",
-        "openpyxl",
-        "tqdm",
-        "ctREFPROP",
-    ]
+with open("requirements.txt") as f:
+    REQUIRES = f.read().splitlines()
 if sys.platform in ["win32", "cygwin", "msys"]:
     REQUIRES.append("xlwings")
 
 setup(
     name="ccp-performance",
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Raphael Timbó",
-    author_email="raphaelts@gmail.com",
+    author_email="raphaelts@petrobras.com.br",
     package_data={"ccp.config": ["new_units.txt"], "ccp.tests.data": ["*"]},
     python_requires=">=3.6",
     install_requires=REQUIRES,
     extras_require={
         "dev": [
             "pytest",
             "pytest-cov",
@@ -84,18 +74,19 @@
             "linkify-it-py",
             "sphinx-book-theme",
             "sphinx-panels",
             "sphinx-copybutton",
             "sphinx-rtd-theme",
         ],
     },
-    license="MIT",
+    py_modules=[],
+    license="Apache License 2.0",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: Implementation :: CPython",
         "Operating System :: OS Independent",
     ],
 )
```

