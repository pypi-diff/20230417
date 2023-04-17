# Comparing `tmp/perlib-2.1.4.tar.gz` & `tmp/perlib-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perlib-2.1.4.tar", last modified: Thu Apr 13 12:34:48 2023, max compression
+gzip compressed data, was "perlib-2.1.5.tar", last modified: Mon Apr 17 14:49:02 2023, max compression
```

## Comparing `perlib-2.1.4.tar` & `perlib-2.1.5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.112413 perlib-2.1.4/
--rw-rw-rw-   0        0        0    11558 2023-04-04 21:29:00.000000 perlib-2.1.4/LICENSE.md
--rw-rw-rw-   0        0        0    10622 2023-04-13 12:34:48.112413 perlib-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    10025 2023-04-04 21:32:21.000000 perlib-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.056388 perlib-2.1.4/perlib/
--rw-rw-rw-   0        0        0      922 2023-04-13 12:32:24.000000 perlib-2.1.4/perlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.061529 perlib-2.1.4/perlib/analysis/
--rw-rw-rw-   0        0        0      131 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/analysis/__init__.py
--rw-rw-rw-   0        0        0      863 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/analysis/exceptions.py
--rw-rw-rw-   0        0        0     5664 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/analysis/multivariate.py
--rw-rw-rw-   0        0        0    10432 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/analysis/plotting.py
--rw-rw-rw-   0        0        0     8015 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/analysis/univariate.py
--rw-rw-rw-   0        0        0     3208 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/analysis/validate.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.061529 perlib-2.1.4/perlib/api/
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/api/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/api/api.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.077154 perlib-2.1.4/perlib/core/
--rw-rw-rw-   0        0        0      454 2023-04-04 21:29:00.000000 perlib-2.1.4/perlib/core/__init__.py
--rw-rw-rw-   0        0        0     3740 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/_requests.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.077154 perlib-2.1.4/perlib/core/metrics/
--rw-rw-rw-   0        0        0       56 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/metrics/__init__.py
--rw-rw-rw-   0        0        0    90017 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/metrics/classification.py
--rw-rw-rw-   0        0        0    21214 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/metrics/regression.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.077154 perlib-2.1.4/perlib/core/models/
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/models/__init__.py
--rw-rw-rw-   0        0        0     4843 2023-04-04 22:12:52.000000 perlib-2.1.4/perlib/core/models/dmodels.py
--rw-rw-rw-   0        0        0     7819 2023-04-04 22:13:07.000000 perlib-2.1.4/perlib/core/models/lstnet.py
--rw-rw-rw-   0        0        0     2581 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/models/mmodels.py
--rw-rw-rw-   0        0        0     2302 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/models/smodels.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.077154 perlib-2.1.4/perlib/core/optimizers/
--rw-rw-rw-   0        0        0    32659 2023-04-04 21:52:50.000000 perlib-2.1.4/perlib/core/optimizers/Optimizers.py
--rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/optimizers/__init__.py
--rw-rw-rw-   0        0        0    11942 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/req_utils.py
--rw-rw-rw-   0        0        0    13165 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/core/tester.py
--rw-rw-rw-   0        0        0    19987 2023-04-05 08:15:18.000000 perlib-2.1.4/perlib/core/train.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.092780 perlib-2.1.4/perlib/datasets/
--rw-rw-rw-   0        0        0      273 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/__init__.py
--rw-rw-rw-   0        0        0     3158 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/airpassengers.py
--rw-rw-rw-   0        0        0     5263 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/ausbeer.py
--rw-rw-rw-   0        0        0     3337 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/austres.py
--rw-rw-rw-   0        0        0     4709 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/heartrate.py
--rw-rw-rw-   0        0        0     3515 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/lynx.py
--rw-rw-rw-   0        0        0    36115 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/taylor.py
--rw-rw-rw-   0        0        0     4820 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/wineind.py
--rw-rw-rw-   0        0        0     3645 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/datasets/woolyrnq.py
--rw-rw-rw-   0        0        0    11981 2023-04-05 07:46:38.000000 perlib-2.1.4/perlib/forecaster.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.092780 perlib-2.1.4/perlib/piplines/
--rw-rw-rw-   0        0        0        0 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/piplines/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-04 22:58:03.000000 perlib-2.1.4/perlib/piplines/dpipline.py
--rw-rw-rw-   0        0        0    21347 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/piplines/mpipline.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.112413 perlib-2.1.4/perlib/preprocessing/
--rw-rw-rw-   0        0        0     5447 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/Normalizing.py
--rw-rw-rw-   0        0        0      241 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     9738 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/_split.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.112413 perlib-2.1.4/perlib/preprocessing/_utils/
--rw-rw-rw-   0        0        0      111 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/_utils/__init__.py
--rw-rw-rw-   0        0        0     8551 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/_utils/dataframe.py
--rw-rw-rw-   0        0        0    27299 2023-04-12 17:23:29.000000 perlib-2.1.4/perlib/preprocessing/_utils/dataset_utils.py
--rw-rw-rw-   0        0        0     9766 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/_utils/timeseries_dataset.py
--rw-rw-rw-   0        0        0    12153 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/_utils/tools.py
--rw-rw-rw-   0        0        0    13496 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/autopreprocess.py
--rw-rw-rw-   0        0        0     4491 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/encode.py
--rw-rw-rw-   0        0        0    13956 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/imputer.py
--rw-rw-rw-   0        0        0     3446 2023-04-04 21:29:01.000000 perlib-2.1.4/perlib/preprocessing/outliers.py
--rw-rw-rw-   0        0        0    19319 2023-04-13 12:15:50.000000 perlib-2.1.4/perlib/preprocessing/preparate.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:34:48.061529 perlib-2.1.4/perlib.egg-info/
--rw-rw-rw-   0        0        0    10622 2023-04-13 12:34:48.000000 perlib-2.1.4/perlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1693 2023-04-13 12:34:48.000000 perlib-2.1.4/perlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:34:48.000000 perlib-2.1.4/perlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      143 2023-04-13 12:34:48.000000 perlib-2.1.4/perlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 12:34:48.000000 perlib-2.1.4/perlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 12:34:48.112413 perlib-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-04 21:29:01.000000 perlib-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.987751 perlib-2.1.5/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 21:29:00.000000 perlib-2.1.5/LICENSE.md
+-rw-rw-rw-   0        0        0    10622 2023-04-17 14:49:02.987751 perlib-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10025 2023-04-04 21:32:21.000000 perlib-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.712430 perlib-2.1.5/perlib/
+-rw-rw-rw-   0        0        0      922 2023-04-17 14:48:53.000000 perlib-2.1.5/perlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.750130 perlib-2.1.5/perlib/analysis/
+-rw-rw-rw-   0        0        0      131 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/__init__.py
+-rw-rw-rw-   0        0        0      863 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/exceptions.py
+-rw-rw-rw-   0        0        0     5664 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/multivariate.py
+-rw-rw-rw-   0        0        0    10432 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/plotting.py
+-rw-rw-rw-   0        0        0     8015 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/univariate.py
+-rw-rw-rw-   0        0        0     3208 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/analysis/validate.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.750130 perlib-2.1.5/perlib/api/
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/api/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/api/api.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.765920 perlib-2.1.5/perlib/core/
+-rw-rw-rw-   0        0        0      454 2023-04-04 21:29:00.000000 perlib-2.1.5/perlib/core/__init__.py
+-rw-rw-rw-   0        0        0     3740 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/_requests.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.802855 perlib-2.1.5/perlib/core/metrics/
+-rw-rw-rw-   0        0        0       56 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/metrics/__init__.py
+-rw-rw-rw-   0        0        0    90017 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/metrics/classification.py
+-rw-rw-rw-   0        0        0    21214 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/metrics/regression.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.821182 perlib-2.1.5/perlib/core/models/
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/models/__init__.py
+-rw-rw-rw-   0        0        0     4843 2023-04-04 22:12:52.000000 perlib-2.1.5/perlib/core/models/dmodels.py
+-rw-rw-rw-   0        0        0     7819 2023-04-04 22:13:07.000000 perlib-2.1.5/perlib/core/models/lstnet.py
+-rw-rw-rw-   0        0        0     2581 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/models/mmodels.py
+-rw-rw-rw-   0        0        0     2302 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/models/smodels.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.836801 perlib-2.1.5/perlib/core/optimizers/
+-rw-rw-rw-   0        0        0    32659 2023-04-04 21:52:50.000000 perlib-2.1.5/perlib/core/optimizers/Optimizers.py
+-rw-rw-rw-   0        0        0       25 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/optimizers/__init__.py
+-rw-rw-rw-   0        0        0    11942 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/req_utils.py
+-rw-rw-rw-   0        0        0    13165 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/core/tester.py
+-rw-rw-rw-   0        0        0    20024 2023-04-17 14:45:58.000000 perlib-2.1.5/perlib/core/train.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.887350 perlib-2.1.5/perlib/datasets/
+-rw-rw-rw-   0        0        0      273 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3158 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/airpassengers.py
+-rw-rw-rw-   0        0        0     5263 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/ausbeer.py
+-rw-rw-rw-   0        0        0     3337 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/austres.py
+-rw-rw-rw-   0        0        0     4709 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/heartrate.py
+-rw-rw-rw-   0        0        0     3515 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/lynx.py
+-rw-rw-rw-   0        0        0    36115 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/taylor.py
+-rw-rw-rw-   0        0        0     4820 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/wineind.py
+-rw-rw-rw-   0        0        0     3645 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/datasets/woolyrnq.py
+-rw-rw-rw-   0        0        0    11981 2023-04-05 07:46:38.000000 perlib-2.1.5/perlib/forecaster.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.906883 perlib-2.1.5/perlib/piplines/
+-rw-rw-rw-   0        0        0        0 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/piplines/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-04 22:58:03.000000 perlib-2.1.5/perlib/piplines/dpipline.py
+-rw-rw-rw-   0        0        0    21347 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/piplines/mpipline.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.947866 perlib-2.1.5/perlib/preprocessing/
+-rw-rw-rw-   0        0        0     5447 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/Normalizing.py
+-rw-rw-rw-   0        0        0      241 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     9738 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_split.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.987751 perlib-2.1.5/perlib/preprocessing/_utils/
+-rw-rw-rw-   0        0        0      111 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/__init__.py
+-rw-rw-rw-   0        0        0     8551 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/dataframe.py
+-rw-rw-rw-   0        0        0    27299 2023-04-12 17:23:29.000000 perlib-2.1.5/perlib/preprocessing/_utils/dataset_utils.py
+-rw-rw-rw-   0        0        0     9766 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/timeseries_dataset.py
+-rw-rw-rw-   0        0        0    12153 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/_utils/tools.py
+-rw-rw-rw-   0        0        0    13496 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/autopreprocess.py
+-rw-rw-rw-   0        0        0     4491 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/encode.py
+-rw-rw-rw-   0        0        0    13956 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/imputer.py
+-rw-rw-rw-   0        0        0     3446 2023-04-04 21:29:01.000000 perlib-2.1.5/perlib/preprocessing/outliers.py
+-rw-rw-rw-   0        0        0    19319 2023-04-13 12:15:50.000000 perlib-2.1.5/perlib/preprocessing/preparate.py
+drwxrwxrwx   0        0        0        0 2023-04-17 14:49:02.728283 perlib-2.1.5/perlib.egg-info/
+-rw-rw-rw-   0        0        0    10622 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1693 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 14:49:02.000000 perlib-2.1.5/perlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 14:49:02.987751 perlib-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-04 21:29:01.000000 perlib-2.1.5/setup.py
```

### Comparing `perlib-2.1.4/LICENSE.md` & `perlib-2.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/PKG-INFO` & `perlib-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perlib
-Version: 2.1.4
+Version: 2.1.5
 Summary: Deep learning, Machine learning and Statistical learning for humans.
 Home-page: https://github.com/Ruzzg/perlib
 Author: Rüzgar Ersin Kanar
 Author-email: ruzgarknr@gmail.com
 License: Apache Software License
 Keywords: perlib,tensorflow,machine learning,deep learning
 Platform: UNKNOWN
```

### Comparing `perlib-2.1.4/README.md` & `perlib-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/__init__.py` & `perlib-2.1.5/perlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Bu projenin tüm hakları Rüzgar Ersin Kanar'a aittir. Harici kimse ticari amaçlı kullanamaz.
-__version__ = "2.1.4"
+__version__ = "2.1.5"
 from .forecaster import *
 from .core._requests import req_info,aR_info,m_info
 from .core.models.dmodels import models as dmodels
 from .core.models.mmodels import models as mmodels
 from .core.models.smodels import models as smodels
 from .core.train import dTrain,sTrain,mTrain
 from .core.tester import dTester,sTester
```

### Comparing `perlib-2.1.4/perlib/analysis/exceptions.py` & `perlib-2.1.5/perlib/analysis/exceptions.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/analysis/multivariate.py` & `perlib-2.1.5/perlib/analysis/multivariate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/analysis/plotting.py` & `perlib-2.1.5/perlib/analysis/plotting.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/analysis/univariate.py` & `perlib-2.1.5/perlib/analysis/univariate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/analysis/validate.py` & `perlib-2.1.5/perlib/analysis/validate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/_requests.py` & `perlib-2.1.5/perlib/core/_requests.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/metrics/classification.py` & `perlib-2.1.5/perlib/core/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/metrics/regression.py` & `perlib-2.1.5/perlib/core/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/models/dmodels.py` & `perlib-2.1.5/perlib/core/models/dmodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/models/lstnet.py` & `perlib-2.1.5/perlib/core/models/lstnet.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/models/mmodels.py` & `perlib-2.1.5/perlib/core/models/mmodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/models/smodels.py` & `perlib-2.1.5/perlib/core/models/smodels.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/optimizers/Optimizers.py` & `perlib-2.1.5/perlib/core/optimizers/Optimizers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/req_utils.py` & `perlib-2.1.5/perlib/core/req_utils.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/tester.py` & `perlib-2.1.5/perlib/core/tester.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/core/train.py` & `perlib-2.1.5/perlib/core/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
             X, y = self.pr.unvariate_data_create_dataset(dataset=dataset, window=self.object.req_info.lookback)
             return X, y
         elif self.dataFrame.shape[1] != 1:
             scalerX = self.pr.get_scaler(self.object.req_info.scaler)
             scalerY = self.pr.get_scaler(self.object.req_info.scaler)
             X_data = scalerX.fit_transform(self.dataFrame.values)
             Y_data = scalerY.fit_transform(self.dataFrame[self.object.req_info.targetCol].values.reshape(-1, 1))
-            X, y = self.pr.multivariate_data_create_dataset(dataset=X_data, target=Y_data)
+            X, y = self.pr.multivariate_data_create_dataset(dataset=X_data, target=Y_data,window=self.object.req_info.lookback)
             return X, y
 
     def __check_folder(self):
         if os.path.exists("models") is False:
             os.mkdir("models")
 
     def fit(self):
```

### Comparing `perlib-2.1.4/perlib/datasets/airpassengers.py` & `perlib-2.1.5/perlib/datasets/airpassengers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/datasets/ausbeer.py` & `perlib-2.1.5/perlib/datasets/ausbeer.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/datasets/austres.py` & `perlib-2.1.5/perlib/datasets/austres.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/datasets/heartrate.py` & `perlib-2.1.5/perlib/datasets/heartrate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/datasets/lynx.py` & `perlib-2.1.5/perlib/datasets/lynx.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/datasets/taylor.py` & `perlib-2.1.5/perlib/datasets/taylor.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/datasets/wineind.py` & `perlib-2.1.5/perlib/datasets/wineind.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/datasets/woolyrnq.py` & `perlib-2.1.5/perlib/datasets/woolyrnq.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/forecaster.py` & `perlib-2.1.5/perlib/forecaster.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/piplines/dpipline.py` & `perlib-2.1.5/perlib/piplines/dpipline.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/piplines/mpipline.py` & `perlib-2.1.5/perlib/piplines/mpipline.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/Normalizing.py` & `perlib-2.1.5/perlib/preprocessing/Normalizing.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/_split.py` & `perlib-2.1.5/perlib/preprocessing/_split.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/_utils/dataframe.py` & `perlib-2.1.5/perlib/preprocessing/_utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/_utils/dataset_utils.py` & `perlib-2.1.5/perlib/preprocessing/_utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/_utils/timeseries_dataset.py` & `perlib-2.1.5/perlib/preprocessing/_utils/timeseries_dataset.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/_utils/tools.py` & `perlib-2.1.5/perlib/preprocessing/_utils/tools.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/autopreprocess.py` & `perlib-2.1.5/perlib/preprocessing/autopreprocess.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/encode.py` & `perlib-2.1.5/perlib/preprocessing/encode.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/imputer.py` & `perlib-2.1.5/perlib/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/outliers.py` & `perlib-2.1.5/perlib/preprocessing/outliers.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib/preprocessing/preparate.py` & `perlib-2.1.5/perlib/preprocessing/preparate.py`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/perlib.egg-info/PKG-INFO` & `perlib-2.1.5/perlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perlib
-Version: 2.1.4
+Version: 2.1.5
 Summary: Deep learning, Machine learning and Statistical learning for humans.
 Home-page: https://github.com/Ruzzg/perlib
 Author: Rüzgar Ersin Kanar
 Author-email: ruzgarknr@gmail.com
 License: Apache Software License
 Keywords: perlib,tensorflow,machine learning,deep learning
 Platform: UNKNOWN
```

### Comparing `perlib-2.1.4/perlib.egg-info/SOURCES.txt` & `perlib-2.1.5/perlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perlib-2.1.4/setup.py` & `perlib-2.1.5/setup.py`

 * *Files identical despite different names*

