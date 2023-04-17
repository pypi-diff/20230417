# Comparing `tmp/tabledetect-0.2.7.tar.gz` & `tmp/tabledetect-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabledetect-0.2.7.tar", last modified: Mon Apr 17 12:52:43 2023, max compression
+gzip compressed data, was "tabledetect-0.2.8.tar", last modified: Mon Apr 17 13:08:03 2023, max compression
```

## Comparing `tabledetect-0.2.7.tar` & `tabledetect-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       79 2023-04-17 11:58:32.009004 tabledetect-0.2.7/.gitignore
--rw-r--r--   0        0        0     1101 2023-04-14 14:25:28.181694 tabledetect-0.2.7/LICENSE
--rw-r--r--   0        0        0       34 2023-04-14 15:13:09.654485 tabledetect-0.2.7/MANIFEST.in
--rw-r--r--   0        0        0       79 2023-04-14 08:12:48.122713 tabledetect-0.2.7/README.md
--rw-r--r--   0        0        0      325 2023-04-14 13:59:35.825728 tabledetect-0.2.7/dev_fetchYolo.py
--rw-r--r--   0        0        0      103 2023-04-17 10:01:40.193051 tabledetect-0.2.7/dev_testscript.py
--rw-r--r--   0        0        0     1097 2023-04-17 12:32:01.525185 tabledetect-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      866 2023-04-17 12:39:17.780506 tabledetect-0.2.7/requirements.txt
--rw-r--r--   0        0        0       54 2023-04-14 14:38:40.550190 tabledetect-0.2.7/requirements_build.txt
--rw-r--r--   0        0        0      108 2023-04-14 11:02:28.444381 tabledetect-0.2.7/table-detect-package.code-workspace
--rw-r--r--   0        0        0      110 2023-04-17 12:52:29.299227 tabledetect-0.2.7/tabledetect/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 09:35:31.789513 tabledetect-0.2.7/tabledetect/helpers/__init__.py
--rw-r--r--   0        0        0     2154 2023-04-14 10:59:23.286532 tabledetect-0.2.7/tabledetect/helpers/boundigbox_to_cropped_image.py
--rw-r--r--   0        0        0      730 2023-04-17 11:55:29.344866 tabledetect-0.2.7/tabledetect/helpers/download.py
--rw-r--r--   0        0        0      784 2023-04-14 09:42:29.665778 tabledetect-0.2.7/tabledetect/helpers/yolo_to_boundingbox.py
--rw-r--r--   0        0        0   130362 2023-04-12 07:56:06.151501 tabledetect-0.2.7/tabledetect/resources/examples/2007-01404285-p2.png
--rw-r--r--   0        0        0   145605 2023-04-12 07:55:11.317114 tabledetect-0.2.7/tabledetect/resources/examples/2007-02501625-p3.png
--rw-r--r--   0        0        0   289812 2023-04-12 07:56:06.191500 tabledetect-0.2.7/tabledetect/resources/examples/2008-75500021-p4.png
--rw-r--r--   0        0        0   275074 2023-04-12 07:56:06.196502 tabledetect-0.2.7/tabledetect/resources/examples/2008-75500021-p8.png
--rw-r--r--   0        0        0   196663 2023-04-12 07:56:06.164501 tabledetect-0.2.7/tabledetect/resources/examples/2020-76400425-p1.png
--rw-r--r--   0        0        0     3225 2023-04-17 12:52:24.809497 tabledetect-0.2.7/tabledetect/tabledetect.py
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 tabledetect-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       79 2023-04-17 11:58:32.009004 tabledetect-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1101 2023-04-14 14:25:28.181694 tabledetect-0.2.8/LICENSE
+-rw-r--r--   0        0        0       34 2023-04-14 15:13:09.654485 tabledetect-0.2.8/MANIFEST.in
+-rw-r--r--   0        0        0       79 2023-04-14 08:12:48.122713 tabledetect-0.2.8/README.md
+-rw-r--r--   0        0        0      325 2023-04-14 13:59:35.825728 tabledetect-0.2.8/dev_fetchYolo.py
+-rw-r--r--   0        0        0      103 2023-04-17 10:01:40.193051 tabledetect-0.2.8/dev_testscript.py
+-rw-r--r--   0        0        0     1178 2023-04-17 12:56:55.952433 tabledetect-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      866 2023-04-17 12:39:17.780506 tabledetect-0.2.8/requirements.txt
+-rw-r--r--   0        0        0       54 2023-04-14 14:38:40.550190 tabledetect-0.2.8/requirements_build.txt
+-rw-r--r--   0        0        0      108 2023-04-14 11:02:28.444381 tabledetect-0.2.8/table-detect-package.code-workspace
+-rw-r--r--   0        0        0      110 2023-04-17 12:54:31.586090 tabledetect-0.2.8/tabledetect/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:35:31.789513 tabledetect-0.2.8/tabledetect/helpers/__init__.py
+-rw-r--r--   0        0        0     2154 2023-04-14 10:59:23.286532 tabledetect-0.2.8/tabledetect/helpers/boundigbox_to_cropped_image.py
+-rw-r--r--   0        0        0      730 2023-04-17 11:55:29.344866 tabledetect-0.2.8/tabledetect/helpers/download.py
+-rw-r--r--   0        0        0      784 2023-04-14 09:42:29.665778 tabledetect-0.2.8/tabledetect/helpers/yolo_to_boundingbox.py
+-rw-r--r--   0        0        0   130362 2023-04-12 07:56:06.151501 tabledetect-0.2.8/tabledetect/resources/examples/2007-01404285-p2.png
+-rw-r--r--   0        0        0   145605 2023-04-12 07:55:11.317114 tabledetect-0.2.8/tabledetect/resources/examples/2007-02501625-p3.png
+-rw-r--r--   0        0        0   289812 2023-04-12 07:56:06.191500 tabledetect-0.2.8/tabledetect/resources/examples/2008-75500021-p4.png
+-rw-r--r--   0        0        0   275074 2023-04-12 07:56:06.196502 tabledetect-0.2.8/tabledetect/resources/examples/2008-75500021-p8.png
+-rw-r--r--   0        0        0   196663 2023-04-12 07:56:06.164501 tabledetect-0.2.8/tabledetect/resources/examples/2020-76400425-p1.png
+-rw-r--r--   0        0        0     3351 2023-04-17 13:06:53.864544 tabledetect-0.2.8/tabledetect/tabledetect.py
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 tabledetect-0.2.8/PKG-INFO
```

### Comparing `tabledetect-0.2.7/LICENSE` & `tabledetect-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/pyproject.toml` & `tabledetect-0.2.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# flit build 
+# flit install --python "C:\virtualenvs\testpackages-venv\Scripts\python.exe"
+# flit publish 
 [distutils]
 index-servers = ['pypi', 'testpypi']
 
 [pypi]
 repository = "https://upload.pypi.org/legacy/"
 username = "Danferno"
```

### Comparing `tabledetect-0.2.7/requirements.txt` & `tabledetect-0.2.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/helpers/boundigbox_to_cropped_image.py` & `tabledetect-0.2.8/tabledetect/helpers/boundigbox_to_cropped_image.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/helpers/download.py` & `tabledetect-0.2.8/tabledetect/helpers/download.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/helpers/yolo_to_boundingbox.py` & `tabledetect-0.2.8/tabledetect/helpers/yolo_to_boundingbox.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/resources/examples/2007-01404285-p2.png` & `tabledetect-0.2.8/tabledetect/resources/examples/2007-01404285-p2.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/resources/examples/2007-02501625-p3.png` & `tabledetect-0.2.8/tabledetect/resources/examples/2007-02501625-p3.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/resources/examples/2008-75500021-p4.png` & `tabledetect-0.2.8/tabledetect/resources/examples/2008-75500021-p4.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/resources/examples/2008-75500021-p8.png` & `tabledetect-0.2.8/tabledetect/resources/examples/2008-75500021-p8.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/resources/examples/2020-76400425-p1.png` & `tabledetect-0.2.8/tabledetect/resources/examples/2020-76400425-p1.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.7/tabledetect/tabledetect.py` & `tabledetect-0.2.8/tabledetect/tabledetect.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,42 +27,44 @@
     downloadRepo(url='https://github.com/Danferno/yolov7/archive/master.zip', destination=PATH_PACKAGE)
 
 if not os.path.exists(PATH_WEIGHTS):
     downloadWeights(url=PATH_WEIGHTS_URL, destination=PATH_WEIGHTS)
 
 
 # Detect tables
-def detect_table(path_input=PATH_EXAMPLES, path_cropped_output=os.path.join(PATH_OUT, 'cropped'), device=None, threshold_confidence=0.5, model_image_size=992, trace='--no-trace', image_format='.png', save_bounding_box_file=True, verbosity=logging.INFO):
+def detect_table(path_input=PATH_EXAMPLES, path_output=os.path.join(PATH_OUT, 'examples_out'), device=None, threshold_confidence=0.5, model_image_size=992, trace='--no-trace', image_format='.png', save_bounding_box_file=True, verbosity=logging.INFO):
     # Parse options
     logging.basicConfig(level=verbosity)
     logging.debug('Checking if torch is properly installed')
     if not device:
         device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
     if not image_format.startswith('.'):
         image_format = f'.{image_format}'
 
     # Detect
     logging.info('Detecting objects in your source files')
-    if os.path.exists(PATH_OUT):
-        shutil.rmtree(PATH_OUT)
-    #os.makedirs(os.path.join(PATH_OUT, 'out', 'table-detect'))
+    pathMlOutput = os.path.join(path_output, 'out')
+    if os.path.exists(pathMlOutput):
+        shutil.rmtree(pathMlOutput)
+    os.makedirs(path_output, exist_ok=True)
     command = f'{PATH_PYTHON} "{PATH_SCRIPT_DETECT}"' \
                 f' --weights {PATH_WEIGHTS}' \
                 f' --conf {threshold_confidence}' \
                 f' --img-size {model_image_size}' \
                 f' --source {path_input}' \
                 f' --save-txt --save-conf' \
                 f' --project out --name table-detect' \
                 f' {trace}'
-    subprocess.run(command, check=True)
+    subprocess.run(command, check=True, cwd=path_output)
 
     # Extract bounding boxes
     logging.info('Extracting bounding box information from the YOLO files')
-    bbox_lists_per_file = [getBoundingBoxesPerFile(annotationfile.path) for annotationfile in os.scandir(os.path.join(PATH_OUT, 'table-detect', 'labels'))]
+    bbox_lists_per_file = [getBoundingBoxesPerFile(annotationfile.path) for annotationfile in os.scandir(os.path.join(PATH_OUT, 'out', 'table-detect', 'labels'))]
 
     # Crop images
     logging.info('Extracting cropped images and saving single bounding box json file')
+    path_cropped_output = os.path.join(path_output, 'cropped')
     extractCroppedImages(bbox_lists_per_file_list=bbox_lists_per_file, outDir=path_cropped_output, imageFormat=image_format, imageDir=path_input, saveBoundingBoxFile=save_bounding_box_file)
```

### Comparing `tabledetect-0.2.7/PKG-INFO` & `tabledetect-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabledetect
-Version: 0.2.7
+Version: 0.2.8
 Summary: Detects tables in images using a custom yolo-v7 model. Very much work in progress
 Author-email: Jesse Wursten <jessaius+tabledetect@hotmail.com>
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: matplotlib>=3.2.2
 Requires-Dist: numpy>=1.18.5,<1.24.0
```

