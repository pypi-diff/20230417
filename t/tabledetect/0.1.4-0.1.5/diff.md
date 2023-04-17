# Comparing `tmp/tabledetect-0.1.4.tar.gz` & `tmp/tabledetect-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabledetect-0.1.4.tar", last modified: Mon Apr 17 12:07:15 2023, max compression
+gzip compressed data, was "tabledetect-0.1.5.tar", last modified: Mon Apr 17 12:17:29 2023, max compression
```

## Comparing `tabledetect-0.1.4.tar` & `tabledetect-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       79 2023-04-17 11:58:32.009004 tabledetect-0.1.4/.gitignore
--rw-r--r--   0        0        0     1101 2023-04-14 14:25:28.181694 tabledetect-0.1.4/LICENSE
--rw-r--r--   0        0        0       34 2023-04-14 15:13:09.654485 tabledetect-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0       79 2023-04-14 08:12:48.122713 tabledetect-0.1.4/README.md
--rw-r--r--   0        0        0      325 2023-04-14 13:59:35.825728 tabledetect-0.1.4/dev_fetchYolo.py
--rw-r--r--   0        0        0      103 2023-04-17 10:01:40.193051 tabledetect-0.1.4/dev_testscript.py
--rw-r--r--   0        0        0     1092 2023-04-17 12:00:35.435881 tabledetect-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      863 2023-04-14 09:00:45.366290 tabledetect-0.1.4/requirements.txt
--rw-r--r--   0        0        0       54 2023-04-14 14:38:40.550190 tabledetect-0.1.4/requirements_build.txt
--rw-r--r--   0        0        0      108 2023-04-14 11:02:28.444381 tabledetect-0.1.4/table-detect-package.code-workspace
--rw-r--r--   0        0        0      110 2023-04-17 12:03:52.923975 tabledetect-0.1.4/tabledetect/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 09:35:31.789513 tabledetect-0.1.4/tabledetect/helpers/__init__.py
--rw-r--r--   0        0        0     2154 2023-04-14 10:59:23.286532 tabledetect-0.1.4/tabledetect/helpers/boundigbox_to_cropped_image.py
--rw-r--r--   0        0        0      730 2023-04-17 11:55:29.344866 tabledetect-0.1.4/tabledetect/helpers/download.py
--rw-r--r--   0        0        0      784 2023-04-14 09:42:29.665778 tabledetect-0.1.4/tabledetect/helpers/yolo_to_boundingbox.py
--rw-r--r--   0        0        0   130362 2023-04-12 07:56:06.151501 tabledetect-0.1.4/tabledetect/resources/examples/2007-01404285-p2.png
--rw-r--r--   0        0        0   145605 2023-04-12 07:55:11.317114 tabledetect-0.1.4/tabledetect/resources/examples/2007-02501625-p3.png
--rw-r--r--   0        0        0   289812 2023-04-12 07:56:06.191500 tabledetect-0.1.4/tabledetect/resources/examples/2008-75500021-p4.png
--rw-r--r--   0        0        0   275074 2023-04-12 07:56:06.196502 tabledetect-0.1.4/tabledetect/resources/examples/2008-75500021-p8.png
--rw-r--r--   0        0        0   196663 2023-04-12 07:56:06.164501 tabledetect-0.1.4/tabledetect/resources/examples/2020-76400425-p1.png
--rw-r--r--   0        0        0     3114 2023-04-17 11:57:24.329984 tabledetect-0.1.4/tabledetect/tabledetect.py
--rw-r--r--   0        0        0     1009 1970-01-01 00:00:00.000000 tabledetect-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       79 2023-04-17 11:58:32.009004 tabledetect-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1101 2023-04-14 14:25:28.181694 tabledetect-0.1.5/LICENSE
+-rw-r--r--   0        0        0       34 2023-04-14 15:13:09.654485 tabledetect-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0       79 2023-04-14 08:12:48.122713 tabledetect-0.1.5/README.md
+-rw-r--r--   0        0        0      325 2023-04-14 13:59:35.825728 tabledetect-0.1.5/dev_fetchYolo.py
+-rw-r--r--   0        0        0      103 2023-04-17 10:01:40.193051 tabledetect-0.1.5/dev_testscript.py
+-rw-r--r--   0        0        0     1092 2023-04-17 12:00:35.435881 tabledetect-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      863 2023-04-14 09:00:45.366290 tabledetect-0.1.5/requirements.txt
+-rw-r--r--   0        0        0       54 2023-04-14 14:38:40.550190 tabledetect-0.1.5/requirements_build.txt
+-rw-r--r--   0        0        0      108 2023-04-14 11:02:28.444381 tabledetect-0.1.5/table-detect-package.code-workspace
+-rw-r--r--   0        0        0      110 2023-04-17 12:17:22.476517 tabledetect-0.1.5/tabledetect/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:35:31.789513 tabledetect-0.1.5/tabledetect/helpers/__init__.py
+-rw-r--r--   0        0        0     2154 2023-04-14 10:59:23.286532 tabledetect-0.1.5/tabledetect/helpers/boundigbox_to_cropped_image.py
+-rw-r--r--   0        0        0      730 2023-04-17 11:55:29.344866 tabledetect-0.1.5/tabledetect/helpers/download.py
+-rw-r--r--   0        0        0      784 2023-04-14 09:42:29.665778 tabledetect-0.1.5/tabledetect/helpers/yolo_to_boundingbox.py
+-rw-r--r--   0        0        0   130362 2023-04-12 07:56:06.151501 tabledetect-0.1.5/tabledetect/resources/examples/2007-01404285-p2.png
+-rw-r--r--   0        0        0   145605 2023-04-12 07:55:11.317114 tabledetect-0.1.5/tabledetect/resources/examples/2007-02501625-p3.png
+-rw-r--r--   0        0        0   289812 2023-04-12 07:56:06.191500 tabledetect-0.1.5/tabledetect/resources/examples/2008-75500021-p4.png
+-rw-r--r--   0        0        0   275074 2023-04-12 07:56:06.196502 tabledetect-0.1.5/tabledetect/resources/examples/2008-75500021-p8.png
+-rw-r--r--   0        0        0   196663 2023-04-12 07:56:06.164501 tabledetect-0.1.5/tabledetect/resources/examples/2020-76400425-p1.png
+-rw-r--r--   0        0        0     3138 2023-04-17 12:16:46.186359 tabledetect-0.1.5/tabledetect/tabledetect.py
+-rw-r--r--   0        0        0     1009 1970-01-01 00:00:00.000000 tabledetect-0.1.5/PKG-INFO
```

### Comparing `tabledetect-0.1.4/LICENSE` & `tabledetect-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/pyproject.toml` & `tabledetect-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/requirements.txt` & `tabledetect-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/helpers/boundigbox_to_cropped_image.py` & `tabledetect-0.1.5/tabledetect/helpers/boundigbox_to_cropped_image.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/helpers/download.py` & `tabledetect-0.1.5/tabledetect/helpers/download.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/helpers/yolo_to_boundingbox.py` & `tabledetect-0.1.5/tabledetect/helpers/yolo_to_boundingbox.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/resources/examples/2007-01404285-p2.png` & `tabledetect-0.1.5/tabledetect/resources/examples/2007-01404285-p2.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/resources/examples/2007-02501625-p3.png` & `tabledetect-0.1.5/tabledetect/resources/examples/2007-02501625-p3.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/resources/examples/2008-75500021-p4.png` & `tabledetect-0.1.5/tabledetect/resources/examples/2008-75500021-p4.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/resources/examples/2008-75500021-p8.png` & `tabledetect-0.1.5/tabledetect/resources/examples/2008-75500021-p8.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/resources/examples/2020-76400425-p1.png` & `tabledetect-0.1.5/tabledetect/resources/examples/2020-76400425-p1.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.1.4/tabledetect/tabledetect.py` & `tabledetect-0.1.5/tabledetect/tabledetect.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tabledetect.helpers.boundigbox_to_cropped_image import extractCroppedImages
 from tabledetect.helpers.download import downloadRepo, downloadWeights
 import logging; logging.basicConfig(level=logging.INFO)
 
 # Check if torch and torchvision installed
 try:
     import torch
+    import torchvision
 except ModuleNotFoundError:
     raise ModuleNotFoundError('pytorch module not found, go to https://pytorch.org/get-started/locally/ to install the correct version')
 
 # Constants
 PATH_PACKAGE = os.path.dirname(os.path.realpath(__file__))
 PATH_WEIGHTS = os.path.join(PATH_PACKAGE, 'resources', 'tabledetect.pt')
 PATH_WEIGHTS_URL = 'https://www.dropbox.com/s/k1iuhwk2k62uifb/tabledetect.pt?dl=1'
```

### Comparing `tabledetect-0.1.4/PKG-INFO` & `tabledetect-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabledetect
-Version: 0.1.4
+Version: 0.1.5
 Summary: Detects tables in images using a custom yolo-v7 model. Very much work in progress
 Author-email: Jesse Wursten <jessaius+tabledetect@hotmail.com>
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: matplotlib>=3.2.2
 Requires-Dist: numpy>=1.18.5,<1.24.0
```

