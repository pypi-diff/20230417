# Comparing `tmp/timeframe-0.2.1.tar.gz` & `tmp/timeframe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeframe-0.2.1.tar", last modified: Sat Nov  5 08:16:10 2022, max compression
+gzip compressed data, was "timeframe-1.0.0.tar", last modified: Mon Apr 17 09:13:44 2023, max compression
```

## Comparing `timeframe-0.2.1.tar` & `timeframe-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 08:16:10.980594 timeframe-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-11-05 08:16:02.000000 timeframe-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6117 2022-11-05 08:16:10.980594 timeframe-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5310 2022-11-05 08:16:02.000000 timeframe-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-05 08:16:10.980594 timeframe-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-11-05 08:16:02.000000 timeframe-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 08:16:10.980594 timeframe-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)    20088 2022-11-05 08:16:02.000000 timeframe-0.2.1/test/test_batch_timeframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-11-05 08:16:02.000000 timeframe-0.2.1/test/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (121)    19250 2022-11-05 08:16:02.000000 timeframe-0.2.1/test/test_timeframe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 08:16:10.980594 timeframe-0.2.1/timeframe/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-05 08:16:02.000000 timeframe-0.2.1/timeframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12858 2022-11-05 08:16:02.000000 timeframe-0.2.1/timeframe/timeframe.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-05 08:16:10.980594 timeframe-0.2.1/timeframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6117 2022-11-05 08:16:10.000000 timeframe-0.2.1/timeframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-11-05 08:16:10.000000 timeframe-0.2.1/timeframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-05 08:16:10.000000 timeframe-0.2.1/timeframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-05 08:16:10.000000 timeframe-0.2.1/timeframe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:13:44.743322 timeframe-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-17 09:13:40.000000 timeframe-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-17 09:13:44.743322 timeframe-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-17 09:13:40.000000 timeframe-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 09:13:44.743322 timeframe-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-17 09:13:40.000000 timeframe-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:13:44.739322 timeframe-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-04-17 09:13:40.000000 timeframe-1.0.0/test/test_batch_timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-17 09:13:40.000000 timeframe-1.0.0/test/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19250 2023-04-17 09:13:40.000000 timeframe-1.0.0/test/test_timeframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:13:44.739322 timeframe-1.0.0/timeframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-17 09:13:40.000000 timeframe-1.0.0/timeframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-04-17 09:13:40.000000 timeframe-1.0.0/timeframe/timeframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 09:13:44.743322 timeframe-1.0.0/timeframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-17 09:13:44.000000 timeframe-1.0.0/timeframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-17 09:13:44.000000 timeframe-1.0.0/timeframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 09:13:44.000000 timeframe-1.0.0/timeframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 09:13:44.000000 timeframe-1.0.0/timeframe.egg-info/top_level.txt
```

### Comparing `timeframe-0.2.1/LICENSE` & `timeframe-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeframe-0.2.1/PKG-INFO` & `timeframe-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,68 @@
 Metadata-Version: 2.1
 Name: timeframe
-Version: 0.2.1
+Version: 1.0.0
 Summary: Calculation of time frames using the built-in datetime module
 Home-page: https://github.com/meysam81/timeframe
 Author: Meysam Azad
 Author-email: MeysamAzad81@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TimeFrame
 
 [![linter](https://github.com/meysam81/timeframe/actions/workflows/linter.yml/badge.svg?branch=main&event=push)](./.pre-commit-config.yaml)
 [![tests](https://github.com/meysam81/timeframe/actions/workflows/tests.yml/badge.svg?branch=main)](./tox.ini)
 [![codecov](https://codecov.io/gh/meysam81/timeframe/branch/main/graph/badge.svg?token=NM0LMWP0X2)](https://codecov.io/gh/meysam81/timeframe)
 [![License](https://img.shields.io/github/license/meysam81/timeframe)](./LICENSE)
+[![Stars](https://img.shields.io/github/stars/meysam81/timeframe?label=GitHub%20stars&style=flat)](https://github.com/meysam81/timeframe/stargazers)
+[![Downloads](https://img.shields.io/pypi/dm/timeframe)](https://pypi.org/project/timeframe/)
 [![Open Issues](https://img.shields.io/github/issues-raw/meysam81/timeframe)](https://github.com/meysam81/timeframe/issues)
 [![Open PRs](https://img.shields.io/github/issues-pr-raw/meysam81/timeframe)](https://github.com/meysam81/timeframe/pulls)
+[![CodeClimate Maintainability](https://img.shields.io/codeclimate/maintainability/meysam81/timeframe)](https://codeclimate.com/github/meysam81/timeframe)
+[![CodeClimate Issues](https://img.shields.io/codeclimate/issues/meysam81/timeframe?label=codeclimate%20issues)](https://codeclimate.com/github/meysam81/timeframe/issues)
+[![CodeClimate Tech Debt](https://img.shields.io/codeclimate/tech-debt/meysam81/timeframe)](https://codeclimate.com/github/meysam81/timeframe/trends/technical_debt)
 [![Contributors](https://img.shields.io/github/contributors/meysam81/timeframe)](https://github.com/meysam81/timeframe/graphs/contributors)
 [![Version](https://img.shields.io/pypi/v/timeframe)](https://pypi.org/project/timeframe/)
-[![Downloads](https://img.shields.io/pypi/dm/timeframe)](https://pypi.org/project/timeframe/)
 [![Python](https://img.shields.io/pypi/pyversions/timeframe)](https://pypi.org/project/timeframe/)
 [![Wheel](https://img.shields.io/pypi/wheel/timeframe)](https://pypi.org/project/timeframe/)
+[![Repo Size](https://img.shields.io/github/repo-size/meysam81/timeframe)](https://github.com/meysam81/timeframe/)
+[![Code Size](https://img.shields.io/github/languages/code-size/meysam81/timeframe)](https://github.com/meysam81/timeframe/)
+
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+
+- [TimeFrame](#timeframe)
+  - [Introduction](#introduction)
+  - [Install](#install)
+  - [Examples](#examples)
+    - [Inclusion](#inclusion)
+      - [New API](#new-api)
+      - [Deprecated](#deprecated)
+    - [Duration](#duration)
+    - [Comparison](#comparison)
+    - [Overlap](#overlap)
+    - [Summation (union)](#summation-union)
+    - [Minus](#minus)
+  - [Acknowledgment](#acknowledgment)
+  - [Contribution](#contribution)
+  - [Stargazers over time](#stargazers-over-time)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
 
 ## Introduction
 
 This package makes the following calculations on `datetime`:
 
 * Adding two time frames, resulting in one bigger time frame or two disjoint one.
 * Multiplying two time frames, resuling in either an overlapped time frame or
@@ -239,7 +266,11 @@
 Thank you for showing interest in this package. Feel free to contact me if you
 feel like it. 🥂
 
 ## Contribution
 
 Any contribution of any size is greatly appreciated. Feel free to open a PR or
 issue in the github page at any time. 🤗
+
+## Stargazers over time
+
+[![Star History Chart](https://api.star-history.com/svg?repos=meysam81/timeframe&type=Date)](https://star-history.com/#meysam81/timeframe&Date)
```

### Comparing `timeframe-0.2.1/README.md` & `timeframe-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,48 @@
 # TimeFrame
 
 [![linter](https://github.com/meysam81/timeframe/actions/workflows/linter.yml/badge.svg?branch=main&event=push)](./.pre-commit-config.yaml)
 [![tests](https://github.com/meysam81/timeframe/actions/workflows/tests.yml/badge.svg?branch=main)](./tox.ini)
 [![codecov](https://codecov.io/gh/meysam81/timeframe/branch/main/graph/badge.svg?token=NM0LMWP0X2)](https://codecov.io/gh/meysam81/timeframe)
 [![License](https://img.shields.io/github/license/meysam81/timeframe)](./LICENSE)
+[![Stars](https://img.shields.io/github/stars/meysam81/timeframe?label=GitHub%20stars&style=flat)](https://github.com/meysam81/timeframe/stargazers)
+[![Downloads](https://img.shields.io/pypi/dm/timeframe)](https://pypi.org/project/timeframe/)
 [![Open Issues](https://img.shields.io/github/issues-raw/meysam81/timeframe)](https://github.com/meysam81/timeframe/issues)
 [![Open PRs](https://img.shields.io/github/issues-pr-raw/meysam81/timeframe)](https://github.com/meysam81/timeframe/pulls)
+[![CodeClimate Maintainability](https://img.shields.io/codeclimate/maintainability/meysam81/timeframe)](https://codeclimate.com/github/meysam81/timeframe)
+[![CodeClimate Issues](https://img.shields.io/codeclimate/issues/meysam81/timeframe?label=codeclimate%20issues)](https://codeclimate.com/github/meysam81/timeframe/issues)
+[![CodeClimate Tech Debt](https://img.shields.io/codeclimate/tech-debt/meysam81/timeframe)](https://codeclimate.com/github/meysam81/timeframe/trends/technical_debt)
 [![Contributors](https://img.shields.io/github/contributors/meysam81/timeframe)](https://github.com/meysam81/timeframe/graphs/contributors)
 [![Version](https://img.shields.io/pypi/v/timeframe)](https://pypi.org/project/timeframe/)
-[![Downloads](https://img.shields.io/pypi/dm/timeframe)](https://pypi.org/project/timeframe/)
 [![Python](https://img.shields.io/pypi/pyversions/timeframe)](https://pypi.org/project/timeframe/)
 [![Wheel](https://img.shields.io/pypi/wheel/timeframe)](https://pypi.org/project/timeframe/)
+[![Repo Size](https://img.shields.io/github/repo-size/meysam81/timeframe)](https://github.com/meysam81/timeframe/)
+[![Code Size](https://img.shields.io/github/languages/code-size/meysam81/timeframe)](https://github.com/meysam81/timeframe/)
+
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+
+- [TimeFrame](#timeframe)
+  - [Introduction](#introduction)
+  - [Install](#install)
+  - [Examples](#examples)
+    - [Inclusion](#inclusion)
+      - [New API](#new-api)
+      - [Deprecated](#deprecated)
+    - [Duration](#duration)
+    - [Comparison](#comparison)
+    - [Overlap](#overlap)
+    - [Summation (union)](#summation-union)
+    - [Minus](#minus)
+  - [Acknowledgment](#acknowledgment)
+  - [Contribution](#contribution)
+  - [Stargazers over time](#stargazers-over-time)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
 
 ## Introduction
 
 This package makes the following calculations on `datetime`:
 
 * Adding two time frames, resulting in one bigger time frame or two disjoint one.
 * Multiplying two time frames, resuling in either an overlapped time frame or
@@ -218,7 +246,11 @@
 Thank you for showing interest in this package. Feel free to contact me if you
 feel like it. 🥂
 
 ## Contribution
 
 Any contribution of any size is greatly appreciated. Feel free to open a PR or
 issue in the github page at any time. 🤗
+
+## Stargazers over time
+
+[![Star History Chart](https://api.star-history.com/svg?repos=meysam81/timeframe&type=Date)](https://star-history.com/#meysam81/timeframe&Date)
```

### Comparing `timeframe-0.2.1/setup.py` & `timeframe-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,15 @@
     url="https://github.com/meysam81/timeframe",
     packages=PACKAGES,
     classifiers=[
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

### Comparing `timeframe-0.2.1/test/test_batch_timeframe.py` & `timeframe-1.0.0/test/test_batch_timeframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,14 @@
     with pytest.raises(TypeError):
         faker.pybool() in BatchTimeFrame([TimeFrame(dt1, dt2)])
 
 
 def test_batch_timeframe_inclusion_check_with_include_warns_deprecation(
     random_timeframe, random_batch_timeframes
 ):
-
     with pytest.warns(DeprecationWarning):
         random_batch_timeframes.includes(random_timeframe)
 
 
 # ======================= Summation ============================
 def test_batch_timeframe_add_two_instances_successfully():
     tf1 = TimeFrame(datetime(2021, 1, 18, 10), datetime(2021, 1, 18, 11))
```

### Comparing `timeframe-0.2.1/test/test_empty.py` & `timeframe-1.0.0/test/test_empty.py`

 * *Files identical despite different names*

### Comparing `timeframe-0.2.1/test/test_timeframe.py` & `timeframe-1.0.0/test/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `timeframe-0.2.1/timeframe/timeframe.py` & `timeframe-1.0.0/timeframe/timeframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,14 @@
 
         if isinstance(tf, BatchTimeFrame):
             return all(map(self.__eq__, tf))
 
         return self.start == tf.start and self.end == tf.end
 
     def _has_common_ground(self, tf: BaseTimeFrame) -> bool:
-
         if isinstance(tf, _Empty):
             return False
 
         return (
             self.start < tf.start < self.end
             or self.start < tf.end < self.end
             or tf.start < self.start < tf.end
```

### Comparing `timeframe-0.2.1/timeframe.egg-info/PKG-INFO` & `timeframe-1.0.0/timeframe.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,68 @@
 Metadata-Version: 2.1
 Name: timeframe
-Version: 0.2.1
+Version: 1.0.0
 Summary: Calculation of time frames using the built-in datetime module
 Home-page: https://github.com/meysam81/timeframe
 Author: Meysam Azad
 Author-email: MeysamAzad81@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TimeFrame
 
 [![linter](https://github.com/meysam81/timeframe/actions/workflows/linter.yml/badge.svg?branch=main&event=push)](./.pre-commit-config.yaml)
 [![tests](https://github.com/meysam81/timeframe/actions/workflows/tests.yml/badge.svg?branch=main)](./tox.ini)
 [![codecov](https://codecov.io/gh/meysam81/timeframe/branch/main/graph/badge.svg?token=NM0LMWP0X2)](https://codecov.io/gh/meysam81/timeframe)
 [![License](https://img.shields.io/github/license/meysam81/timeframe)](./LICENSE)
+[![Stars](https://img.shields.io/github/stars/meysam81/timeframe?label=GitHub%20stars&style=flat)](https://github.com/meysam81/timeframe/stargazers)
+[![Downloads](https://img.shields.io/pypi/dm/timeframe)](https://pypi.org/project/timeframe/)
 [![Open Issues](https://img.shields.io/github/issues-raw/meysam81/timeframe)](https://github.com/meysam81/timeframe/issues)
 [![Open PRs](https://img.shields.io/github/issues-pr-raw/meysam81/timeframe)](https://github.com/meysam81/timeframe/pulls)
+[![CodeClimate Maintainability](https://img.shields.io/codeclimate/maintainability/meysam81/timeframe)](https://codeclimate.com/github/meysam81/timeframe)
+[![CodeClimate Issues](https://img.shields.io/codeclimate/issues/meysam81/timeframe?label=codeclimate%20issues)](https://codeclimate.com/github/meysam81/timeframe/issues)
+[![CodeClimate Tech Debt](https://img.shields.io/codeclimate/tech-debt/meysam81/timeframe)](https://codeclimate.com/github/meysam81/timeframe/trends/technical_debt)
 [![Contributors](https://img.shields.io/github/contributors/meysam81/timeframe)](https://github.com/meysam81/timeframe/graphs/contributors)
 [![Version](https://img.shields.io/pypi/v/timeframe)](https://pypi.org/project/timeframe/)
-[![Downloads](https://img.shields.io/pypi/dm/timeframe)](https://pypi.org/project/timeframe/)
 [![Python](https://img.shields.io/pypi/pyversions/timeframe)](https://pypi.org/project/timeframe/)
 [![Wheel](https://img.shields.io/pypi/wheel/timeframe)](https://pypi.org/project/timeframe/)
+[![Repo Size](https://img.shields.io/github/repo-size/meysam81/timeframe)](https://github.com/meysam81/timeframe/)
+[![Code Size](https://img.shields.io/github/languages/code-size/meysam81/timeframe)](https://github.com/meysam81/timeframe/)
+
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+
+- [TimeFrame](#timeframe)
+  - [Introduction](#introduction)
+  - [Install](#install)
+  - [Examples](#examples)
+    - [Inclusion](#inclusion)
+      - [New API](#new-api)
+      - [Deprecated](#deprecated)
+    - [Duration](#duration)
+    - [Comparison](#comparison)
+    - [Overlap](#overlap)
+    - [Summation (union)](#summation-union)
+    - [Minus](#minus)
+  - [Acknowledgment](#acknowledgment)
+  - [Contribution](#contribution)
+  - [Stargazers over time](#stargazers-over-time)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
 
 ## Introduction
 
 This package makes the following calculations on `datetime`:
 
 * Adding two time frames, resulting in one bigger time frame or two disjoint one.
 * Multiplying two time frames, resuling in either an overlapped time frame or
@@ -239,7 +266,11 @@
 Thank you for showing interest in this package. Feel free to contact me if you
 feel like it. 🥂
 
 ## Contribution
 
 Any contribution of any size is greatly appreciated. Feel free to open a PR or
 issue in the github page at any time. 🤗
+
+## Stargazers over time
+
+[![Star History Chart](https://api.star-history.com/svg?repos=meysam81/timeframe&type=Date)](https://star-history.com/#meysam81/timeframe&Date)
```

