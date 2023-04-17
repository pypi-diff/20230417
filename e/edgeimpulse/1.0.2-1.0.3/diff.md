# Comparing `tmp/edgeimpulse-1.0.2.tar.gz` & `tmp/edgeimpulse-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse-1.0.2.tar", max compression
+gzip compressed data, was "edgeimpulse-1.0.3.tar", max compression
```

## Comparing `edgeimpulse-1.0.2.tar` & `edgeimpulse-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1531 2023-04-11 14:48:06.888998 edgeimpulse-1.0.2/README.md
--rw-r--r--   0        0        0      297 2023-04-11 14:48:06.889249 edgeimpulse-1.0.2/edgeimpulse/__init__.py
--rw-r--r--   0        0        0     3017 2023-04-11 14:48:06.889354 edgeimpulse-1.0.2/edgeimpulse/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-17 15:56:20.819238 edgeimpulse-1.0.2/edgeimpulse/methods/__init__.py
--rw-r--r--   0        0        0      179 2023-04-13 14:10:19.981597 edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      124 2023-04-13 20:28:50.677287 edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    13356 2023-04-13 14:10:19.986029 edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/deploy.cpython-310.pyc
--rw-r--r--   0        0        0    13241 2023-04-13 20:28:50.158896 edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/deploy.cpython-38.pyc
--rw-r--r--   0        0        0     6401 2023-04-13 14:21:36.704259 edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/profile.cpython-310.pyc
--rw-r--r--   0        0        0     6187 2023-04-13 20:28:50.429340 edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/profile.cpython-38.pyc
--rw-r--r--   0        0        0    16925 2023-04-13 14:43:29.187839 edgeimpulse-1.0.2/edgeimpulse/methods/deploy.py
--rw-r--r--   0        0        0     7079 2023-04-13 14:24:20.503484 edgeimpulse-1.0.2/edgeimpulse/methods/profile.py
--rw-r--r--   0        0        0      313 2023-04-13 14:43:29.187994 edgeimpulse-1.0.2/edgeimpulse/model/__init__.py
--rw-r--r--   0        0        0      459 2023-04-13 14:16:13.974578 edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      410 2023-04-13 20:28:51.718454 edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1199 2023-04-13 14:10:19.986757 edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/input_type.cpython-310.pyc
--rw-r--r--   0        0        0     1140 2023-04-13 20:28:51.468709 edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/input_type.cpython-38.pyc
--rw-r--r--   0        0        0      919 2023-04-13 20:28:51.969256 edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/model_info.cpython-38.pyc
--rw-r--r--   0        0        0     1372 2023-04-13 14:10:19.986426 edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/output_type.cpython-310.pyc
--rw-r--r--   0        0        0     1305 2023-04-13 20:28:52.222246 edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/output_type.cpython-38.pyc
--rw-r--r--   0        0        0      466 2023-04-03 13:45:58.875930 edgeimpulse-1.0.2/edgeimpulse/model/input_type.py
--rw-r--r--   0        0        0      673 2023-04-03 13:45:58.876012 edgeimpulse-1.0.2/edgeimpulse/model/model_info.py
--rw-r--r--   0        0        0      607 2023-04-03 13:45:58.876076 edgeimpulse-1.0.2/edgeimpulse/model/output_type.py
--rw-r--r--   0        0        0    15524 2023-04-13 19:51:28.026063 edgeimpulse-1.0.2/edgeimpulse/util.py
--rw-r--r--   0        0        0      802 2023-04-13 20:14:38.968427 edgeimpulse-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 edgeimpulse-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-11 14:48:06.888998 edgeimpulse-1.0.3/README.md
+-rw-r--r--   0        0        0      297 2023-04-11 14:48:06.889249 edgeimpulse-1.0.3/edgeimpulse/__init__.py
+-rw-r--r--   0        0        0     3017 2023-04-11 14:48:06.889354 edgeimpulse-1.0.3/edgeimpulse/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-17 15:56:20.819238 edgeimpulse-1.0.3/edgeimpulse/methods/__init__.py
+-rw-r--r--   0        0        0      179 2023-04-13 14:10:19.981597 edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      124 2023-04-13 20:28:50.677287 edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    13356 2023-04-13 14:10:19.986029 edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/deploy.cpython-310.pyc
+-rw-r--r--   0        0        0    13241 2023-04-13 20:28:50.158896 edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/deploy.cpython-38.pyc
+-rw-r--r--   0        0        0     6401 2023-04-13 14:21:36.704259 edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/profile.cpython-310.pyc
+-rw-r--r--   0        0        0     6187 2023-04-13 20:28:50.429340 edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/profile.cpython-38.pyc
+-rw-r--r--   0        0        0    16925 2023-04-13 14:43:29.187839 edgeimpulse-1.0.3/edgeimpulse/methods/deploy.py
+-rw-r--r--   0        0        0     7079 2023-04-17 10:42:04.811317 edgeimpulse-1.0.3/edgeimpulse/methods/profile.py
+-rw-r--r--   0        0        0      313 2023-04-13 14:43:29.187994 edgeimpulse-1.0.3/edgeimpulse/model/__init__.py
+-rw-r--r--   0        0        0      459 2023-04-13 14:16:13.974578 edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      410 2023-04-13 20:28:51.718454 edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1199 2023-04-13 14:10:19.986757 edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/input_type.cpython-310.pyc
+-rw-r--r--   0        0        0     1140 2023-04-13 20:28:51.468709 edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/input_type.cpython-38.pyc
+-rw-r--r--   0        0        0      919 2023-04-13 20:28:51.969256 edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/model_info.cpython-38.pyc
+-rw-r--r--   0        0        0     1372 2023-04-13 14:10:19.986426 edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/output_type.cpython-310.pyc
+-rw-r--r--   0        0        0     1305 2023-04-13 20:28:52.222246 edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/output_type.cpython-38.pyc
+-rw-r--r--   0        0        0      466 2023-04-03 13:45:58.875930 edgeimpulse-1.0.3/edgeimpulse/model/input_type.py
+-rw-r--r--   0        0        0      673 2023-04-03 13:45:58.876012 edgeimpulse-1.0.3/edgeimpulse/model/model_info.py
+-rw-r--r--   0        0        0      607 2023-04-03 13:45:58.876076 edgeimpulse-1.0.3/edgeimpulse/model/output_type.py
+-rw-r--r--   0        0        0    15524 2023-04-17 10:42:04.811798 edgeimpulse-1.0.3/edgeimpulse/util.py
+-rw-r--r--   0        0        0      802 2023-04-17 13:34:59.147011 edgeimpulse-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 edgeimpulse-1.0.3/PKG-INFO
```

### Comparing `edgeimpulse-1.0.2/README.md` & `edgeimpulse-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/exceptions.py` & `edgeimpulse-1.0.3/edgeimpulse/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/deploy.cpython-310.pyc` & `edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/deploy.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/deploy.cpython-38.pyc` & `edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/deploy.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/profile.cpython-310.pyc` & `edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/profile.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/methods/__pycache__/profile.cpython-38.pyc` & `edgeimpulse-1.0.3/edgeimpulse/methods/__pycache__/profile.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/methods/deploy.py` & `edgeimpulse-1.0.3/edgeimpulse/methods/deploy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/methods/profile.py` & `edgeimpulse-1.0.3/edgeimpulse/methods/profile.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/input_type.cpython-310.pyc` & `edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/input_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/input_type.cpython-38.pyc` & `edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/input_type.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/model_info.cpython-38.pyc` & `edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/model_info.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/output_type.cpython-310.pyc` & `edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/output_type.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/model/__pycache__/output_type.cpython-38.pyc` & `edgeimpulse-1.0.3/edgeimpulse/model/__pycache__/output_type.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/model/model_info.py` & `edgeimpulse-1.0.3/edgeimpulse/model/model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/model/output_type.py` & `edgeimpulse-1.0.3/edgeimpulse/model/output_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/edgeimpulse/util.py` & `edgeimpulse-1.0.3/edgeimpulse/util.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse-1.0.2/pyproject.toml` & `edgeimpulse-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "edgeimpulse"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python SDK for Edge Impulse."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Embedded Systems"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-edgeimpulse-api = "1.22.1"
+edgeimpulse-api = "1.22.2"
 
 [tool.poetry.dev-dependencies]
 sphinx = "5.3.0"
 sphinx-markdown-builder = "0.5.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `edgeimpulse-1.0.2/PKG-INFO` & `edgeimpulse-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for Edge Impulse.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Embedded Systems
-Requires-Dist: edgeimpulse-api (==1.22.1)
+Requires-Dist: edgeimpulse-api (==1.22.2)
 Project-URL: Documentation, https://docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://www.edgeimpulse.com/"><img src="https://events.edgeimpulse.com/hs-fs/hubfs/Edge%20Impulse%20Full%20Logo_RGB.png?width=1817&name=Edge%20Impulse%20Full%20Logo_RGB.png?raw=true" alt="Edge Impulse logo"/></a>
 </p>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: edgeimpulse Version: 1.0.2 Summary: Python SDK for
+Metadata-Version: 2.1 Name: edgeimpulse Version: 1.0.3 Summary: Python SDK for
 Edge Impulse. Home-page: https://edgeimpulse.com License: Apache-2.0 Author:
 EdgeImpulse Inc. Author-email: hello@edgeimpulse.com Requires-Python:
 >=3.7,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Embedded Systems Requires-Dist:
-edgeimpulse-api (==1.22.1) Project-URL: Documentation, https://
+edgeimpulse-api (==1.22.2) Project-URL: Documentation, https://
 docs.edgeimpulse.com/docs/edge-impulse-python-sdk/overview Description-Content-
 Type: text/markdown
                               [Edge_Impulse_logo]
 # Edge Impulse SDK The official Python SDK for Edge Impulse is designed to help
 machine learning practitioners build and deploy models for embedded hardware
 and edge AI applications. * Profile your model to estimate RAM, ROM, and
 inference speed * Convert your model to C++ to deploy on edge hardware *
```

