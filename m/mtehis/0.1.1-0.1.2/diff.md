# Comparing `tmp/mtehis-0.1.1.tar.gz` & `tmp/mtehis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtehis-0.1.1.tar", last modified: Wed Apr 12 16:17:36 2023, max compression
+gzip compressed data, was "mtehis-0.1.2.tar", last modified: Mon Apr 17 13:45:38 2023, max compression
```

## Comparing `mtehis-0.1.1.tar` & `mtehis-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:36.743040 mtehis-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 16:17:22.000000 mtehis-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-12 16:17:36.743040 mtehis-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:17:22.000000 mtehis-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:36.739040 mtehis-0.1.1/mtehis/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:36.739040 mtehis-0.1.1/mtehis/base/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/base/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:36.743040 mtehis-0.1.1/mtehis/data/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/data/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:36.743040 mtehis-0.1.1/mtehis/model/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/model/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/model/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:36.743040 mtehis-0.1.1/mtehis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/util/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 16:17:22.000000 mtehis-0.1.1/mtehis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:17:36.739040 mtehis-0.1.1/mtehis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-12 16:17:36.000000 mtehis-0.1.1/mtehis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-12 16:17:36.000000 mtehis-0.1.1/mtehis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:17:36.000000 mtehis-0.1.1/mtehis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 16:17:36.000000 mtehis-0.1.1/mtehis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 16:17:36.000000 mtehis-0.1.1/mtehis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:17:36.743040 mtehis-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-12 16:17:22.000000 mtehis-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 13:45:24.000000 mtehis-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 13:45:38.221960 mtehis-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 13:45:24.000000 mtehis-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/base/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/data/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/model/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/model/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/util/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 13:45:24.000000 mtehis-0.1.2/mtehis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 13:45:38.221960 mtehis-0.1.2/mtehis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 13:45:38.000000 mtehis-0.1.2/mtehis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 13:45:38.221960 mtehis-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 13:45:24.000000 mtehis-0.1.2/setup.py
```

### Comparing `mtehis-0.1.1/LICENSE` & `mtehis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.1/PKG-INFO` & `mtehis-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtehis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Maintenance Tool for Evolving Hybrid Intelligent Systems: Core Package.
 Home-page: https://github.com/MT-EHIS/core
 Author: Oleksandr Pokhylenko
 Author-email: pokhilenko.alex@gmail.com
 License: UNKNOWN
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `mtehis-0.1.1/mtehis/base/detector.py` & `mtehis-0.1.2/mtehis/base/detector.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.1/mtehis/data/detector.py` & `mtehis-0.1.2/mtehis/data/detector.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.1/mtehis/model/classifier.py` & `mtehis-0.1.2/mtehis/model/classifier.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.1/mtehis/model/detector.py` & `mtehis-0.1.2/mtehis/model/detector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import inspect
 import numpy as np
 import streamad.model as streamad_models
 from streamad.process import ZScoreCalibrator
 from ..data import LearningDetectorData
 from ..base import ConfiguredDetector
 from .classifier import CustomMLPClassifier
+from typing import Callable
 
 
 class LearningDetector:
-    def __init__(self, features_count):
+    def __init__(self, features_count: int, logging_func: Callable[[int], None] = None):
         self.features_count = features_count
         self.detectors = []
+        self.logging_func = logging_func
 
         for name, detector in inspect.getmembers(streamad_models, inspect.isclass):
             if name == 'RandomDetector':
                 continue
             current_detector = detector()
             if current_detector.data_type == 'multivariate':
                 self.detectors.append(ConfiguredDetector(current_detector, ZScoreCalibrator(sigma=3)))
@@ -36,17 +38,27 @@
         learning_detector = cls(data.features_count)
         for i in range(len(learning_detector.detectors)):
             detector_str = str(learning_detector.detectors[i])
             learning_detector.classifier.coefs_[0][i][0] = data.coefs.get(detector_str, 0.0)
         learning_detector.classifier.intercepts_[0][0] = data.bias
         return learning_detector
 
+    def _get_scores(self, xs):
+        if self.logging_func is None:
+            return np.array([[detector.fit_score(x) for detector in self.detectors] for x in xs], np.float32)
+        else:
+            scores = []
+            for i in range(len(xs)):
+                scores.append([detector.fit_score(xs[i]) for detector in self.detectors])
+                self.logging_func(i)
+            return np.array(scores, np.float32)
+
     def fit(self, xs, ys):
-        scores = np.array([[detector.fit_score(x) for detector in self.detectors] for x in xs], np.float32)
+        scores = self._get_scores(xs)
         ys = ys[~np.isnan(scores).any(axis=1)]
         scores = scores[~np.isnan(scores).any(axis=1)]
         self.classifier.fit(scores, ys)
 
     def predict(self, xs):
-        scores = np.array([[detector.fit_score(x) for detector in self.detectors] for x in xs], np.float32)
+        scores = self._get_scores(xs)
         scores[np.isnan(scores)] = 0
         return self.classifier.predict(scores)
```

### Comparing `mtehis-0.1.1/mtehis/util/evaluate.py` & `mtehis-0.1.2/mtehis/util/evaluate.py`

 * *Files identical despite different names*

### Comparing `mtehis-0.1.1/mtehis.egg-info/PKG-INFO` & `mtehis-0.1.2/mtehis.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtehis
-Version: 0.1.1
+Version: 0.1.2
 Summary: Maintenance Tool for Evolving Hybrid Intelligent Systems: Core Package.
 Home-page: https://github.com/MT-EHIS/core
 Author: Oleksandr Pokhylenko
 Author-email: pokhilenko.alex@gmail.com
 License: UNKNOWN
 Platform: all
 Classifier: Intended Audience :: Developers
```

### Comparing `mtehis-0.1.1/setup.py` & `mtehis-0.1.2/setup.py`

 * *Files identical despite different names*

