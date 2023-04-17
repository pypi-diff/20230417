# Comparing `tmp/tract-0.19.7.tar.gz` & `tmp/tract-0.19.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tract-0.19.7.tar", last modified: Fri Feb 24 15:04:53 2023, max compression
+gzip compressed data, was "tract-0.19.8.tar", last modified: Mon Mar 27 13:41:16 2023, max compression
```

## Comparing `tract-0.19.7.tar` & `tract-0.19.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:04:53.837229 tract-0.19.7/
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-02-24 15:04:53.837229 tract-0.19.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-24 15:04:44.000000 tract-0.19.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 15:04:53.837229 tract-0.19.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-24 15:04:44.000000 tract-0.19.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:04:53.833229 tract-0.19.7/tract/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-02-24 15:04:44.000000 tract-0.19.7/tract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-24 15:04:44.000000 tract-0.19.7/tract/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-02-24 15:04:44.000000 tract-0.19.7/tract/fact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-02-24 15:04:44.000000 tract-0.19.7/tract/inference_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-02-24 15:04:44.000000 tract-0.19.7/tract/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-02-24 15:04:44.000000 tract-0.19.7/tract/nnef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-02-24 15:04:44.000000 tract-0.19.7/tract/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-02-24 15:04:44.000000 tract-0.19.7/tract/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-02-24 15:04:44.000000 tract-0.19.7/tract/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:04:53.833229 tract-0.19.7/tract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-02-24 15:04:53.000000 tract-0.19.7/tract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-24 15:04:53.000000 tract-0.19.7/tract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 15:04:53.000000 tract-0.19.7/tract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 15:04:53.000000 tract-0.19.7/tract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-24 15:04:53.000000 tract-0.19.7/tract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-24 15:04:53.000000 tract-0.19.7/tract.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:41:16.459127 tract-0.19.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-03-27 13:41:16.459127 tract-0.19.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-27 13:41:03.000000 tract-0.19.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 13:41:16.459127 tract-0.19.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-27 13:41:03.000000 tract-0.19.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:41:16.459127 tract-0.19.8/tract/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-27 13:41:03.000000 tract-0.19.8/tract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-27 13:41:03.000000 tract-0.19.8/tract/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-27 13:41:03.000000 tract-0.19.8/tract/fact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-03-27 13:41:03.000000 tract-0.19.8/tract/inference_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-03-27 13:41:03.000000 tract-0.19.8/tract/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-27 13:41:03.000000 tract-0.19.8/tract/nnef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-03-27 13:41:03.000000 tract-0.19.8/tract/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-27 13:41:03.000000 tract-0.19.8/tract/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-03-27 13:41:03.000000 tract-0.19.8/tract/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:41:16.459127 tract-0.19.8/tract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-27 13:41:16.000000 tract-0.19.8/tract.egg-info/top_level.txt
```

### Comparing `tract-0.19.7/PKG-INFO` & `tract-0.19.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tract
-Version: 0.19.7
+Version: 0.19.8
 Summary: Python bindings for tract, a neural network inference engine
 Author: Mathieu Poumeyrol, Sonos, and tract contributors
 Author-email: mathieu@poumeyrol.fr
 License: Apache License, Version 2.0 OR MIT
 Project-URL: Documentation, https://github.com/sonos/tract
 Project-URL: Source, https://github.com/sonos/tract
 Keywords: onnx tensorflow nnef runtime neural network
```

### Comparing `tract-0.19.7/pyproject.toml` & `tract-0.19.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/setup.py` & `tract-0.19.8/setup.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/__init__.py` & `tract-0.19.8/tract/__init__.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/bindings.py` & `tract-0.19.8/tract/bindings.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/fact.py` & `tract-0.19.8/tract/fact.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/inference_model.py` & `tract-0.19.8/tract/inference_model.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/model.py` & `tract-0.19.8/tract/model.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/nnef.py` & `tract-0.19.8/tract/nnef.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,22 @@
         """
         Enable tract-opl extensions to NNEF for tract pulse operators (for audio streaming)
         """
         self._valid()
         check(lib.tract_nnef_enable_pulse(self.ptr))
         return self
 
+    def with_extended_identifier_syntax(self) -> "Nnef":
+        """
+        Enable tract-opl extensions to NNEF for extended identifiers (will support PyTorch 2 path-like ids)
+        """
+        self._valid()
+        check(lib.tract_nnef_allow_extended_identifier_syntax(self.ptr, True))
+        return self
+
     def write_model_to_dir(self, model: Model, path: Union[str, Path]) -> None:
         """
         Save `model` as a NNEF directory model in `path`.
 
         tract tries to stick to strict NNEF even if extensions has been enabled.
         """
         self._valid()
```

### Comparing `tract-0.19.7/tract/onnx.py` & `tract-0.19.8/tract/onnx.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/runnable.py` & `tract-0.19.8/tract/runnable.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract/value.py` & `tract-0.19.8/tract/value.py`

 * *Files identical despite different names*

### Comparing `tract-0.19.7/tract.egg-info/PKG-INFO` & `tract-0.19.8/tract.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tract
-Version: 0.19.7
+Version: 0.19.8
 Summary: Python bindings for tract, a neural network inference engine
 Author: Mathieu Poumeyrol, Sonos, and tract contributors
 Author-email: mathieu@poumeyrol.fr
 License: Apache License, Version 2.0 OR MIT
 Project-URL: Documentation, https://github.com/sonos/tract
 Project-URL: Source, https://github.com/sonos/tract
 Keywords: onnx tensorflow nnef runtime neural network
```

