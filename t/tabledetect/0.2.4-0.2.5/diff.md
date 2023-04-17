# Comparing `tmp/tabledetect-0.2.4.tar.gz` & `tmp/tabledetect-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabledetect-0.2.4.tar", last modified: Mon Apr 17 12:45:36 2023, max compression
+gzip compressed data, was "tabledetect-0.2.5.tar", last modified: Mon Apr 17 12:47:15 2023, max compression
```

## Comparing `tabledetect-0.2.4.tar` & `tabledetect-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       79 2023-04-17 11:58:32.009004 tabledetect-0.2.4/.gitignore
--rw-r--r--   0        0        0     1101 2023-04-14 14:25:28.181694 tabledetect-0.2.4/LICENSE
--rw-r--r--   0        0        0       34 2023-04-14 15:13:09.654485 tabledetect-0.2.4/MANIFEST.in
--rw-r--r--   0        0        0       79 2023-04-14 08:12:48.122713 tabledetect-0.2.4/README.md
--rw-r--r--   0        0        0      325 2023-04-14 13:59:35.825728 tabledetect-0.2.4/dev_fetchYolo.py
--rw-r--r--   0        0        0      103 2023-04-17 10:01:40.193051 tabledetect-0.2.4/dev_testscript.py
--rw-r--r--   0        0        0     1097 2023-04-17 12:32:01.525185 tabledetect-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      866 2023-04-17 12:39:17.780506 tabledetect-0.2.4/requirements.txt
--rw-r--r--   0        0        0       54 2023-04-14 14:38:40.550190 tabledetect-0.2.4/requirements_build.txt
--rw-r--r--   0        0        0      108 2023-04-14 11:02:28.444381 tabledetect-0.2.4/table-detect-package.code-workspace
--rw-r--r--   0        0        0      110 2023-04-17 12:45:34.581852 tabledetect-0.2.4/tabledetect/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 09:35:31.789513 tabledetect-0.2.4/tabledetect/helpers/__init__.py
--rw-r--r--   0        0        0     2154 2023-04-14 10:59:23.286532 tabledetect-0.2.4/tabledetect/helpers/boundigbox_to_cropped_image.py
--rw-r--r--   0        0        0      730 2023-04-17 11:55:29.344866 tabledetect-0.2.4/tabledetect/helpers/download.py
--rw-r--r--   0        0        0      784 2023-04-14 09:42:29.665778 tabledetect-0.2.4/tabledetect/helpers/yolo_to_boundingbox.py
--rw-r--r--   0        0        0   130362 2023-04-12 07:56:06.151501 tabledetect-0.2.4/tabledetect/resources/examples/2007-01404285-p2.png
--rw-r--r--   0        0        0   145605 2023-04-12 07:55:11.317114 tabledetect-0.2.4/tabledetect/resources/examples/2007-02501625-p3.png
--rw-r--r--   0        0        0   289812 2023-04-12 07:56:06.191500 tabledetect-0.2.4/tabledetect/resources/examples/2008-75500021-p4.png
--rw-r--r--   0        0        0   275074 2023-04-12 07:56:06.196502 tabledetect-0.2.4/tabledetect/resources/examples/2008-75500021-p8.png
--rw-r--r--   0        0        0   196663 2023-04-12 07:56:06.164501 tabledetect-0.2.4/tabledetect/resources/examples/2020-76400425-p1.png
--rw-r--r--   0        0        0     3191 2023-04-17 12:45:27.880480 tabledetect-0.2.4/tabledetect/tabledetect.py
--rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 tabledetect-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       79 2023-04-17 11:58:32.009004 tabledetect-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1101 2023-04-14 14:25:28.181694 tabledetect-0.2.5/LICENSE
+-rw-r--r--   0        0        0       34 2023-04-14 15:13:09.654485 tabledetect-0.2.5/MANIFEST.in
+-rw-r--r--   0        0        0       79 2023-04-14 08:12:48.122713 tabledetect-0.2.5/README.md
+-rw-r--r--   0        0        0      325 2023-04-14 13:59:35.825728 tabledetect-0.2.5/dev_fetchYolo.py
+-rw-r--r--   0        0        0      103 2023-04-17 10:01:40.193051 tabledetect-0.2.5/dev_testscript.py
+-rw-r--r--   0        0        0     1097 2023-04-17 12:32:01.525185 tabledetect-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      866 2023-04-17 12:39:17.780506 tabledetect-0.2.5/requirements.txt
+-rw-r--r--   0        0        0       54 2023-04-14 14:38:40.550190 tabledetect-0.2.5/requirements_build.txt
+-rw-r--r--   0        0        0      108 2023-04-14 11:02:28.444381 tabledetect-0.2.5/table-detect-package.code-workspace
+-rw-r--r--   0        0        0      110 2023-04-17 12:47:08.820554 tabledetect-0.2.5/tabledetect/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 09:35:31.789513 tabledetect-0.2.5/tabledetect/helpers/__init__.py
+-rw-r--r--   0        0        0     2154 2023-04-14 10:59:23.286532 tabledetect-0.2.5/tabledetect/helpers/boundigbox_to_cropped_image.py
+-rw-r--r--   0        0        0      730 2023-04-17 11:55:29.344866 tabledetect-0.2.5/tabledetect/helpers/download.py
+-rw-r--r--   0        0        0      784 2023-04-14 09:42:29.665778 tabledetect-0.2.5/tabledetect/helpers/yolo_to_boundingbox.py
+-rw-r--r--   0        0        0   130362 2023-04-12 07:56:06.151501 tabledetect-0.2.5/tabledetect/resources/examples/2007-01404285-p2.png
+-rw-r--r--   0        0        0   145605 2023-04-12 07:55:11.317114 tabledetect-0.2.5/tabledetect/resources/examples/2007-02501625-p3.png
+-rw-r--r--   0        0        0   289812 2023-04-12 07:56:06.191500 tabledetect-0.2.5/tabledetect/resources/examples/2008-75500021-p4.png
+-rw-r--r--   0        0        0   275074 2023-04-12 07:56:06.196502 tabledetect-0.2.5/tabledetect/resources/examples/2008-75500021-p8.png
+-rw-r--r--   0        0        0   196663 2023-04-12 07:56:06.164501 tabledetect-0.2.5/tabledetect/resources/examples/2020-76400425-p1.png
+-rw-r--r--   0        0        0     3187 2023-04-17 12:47:04.755949 tabledetect-0.2.5/tabledetect/tabledetect.py
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 tabledetect-0.2.5/PKG-INFO
```

### Comparing `tabledetect-0.2.4/LICENSE` & `tabledetect-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/pyproject.toml` & `tabledetect-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/requirements.txt` & `tabledetect-0.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/helpers/boundigbox_to_cropped_image.py` & `tabledetect-0.2.5/tabledetect/helpers/boundigbox_to_cropped_image.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/helpers/download.py` & `tabledetect-0.2.5/tabledetect/helpers/download.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/helpers/yolo_to_boundingbox.py` & `tabledetect-0.2.5/tabledetect/helpers/yolo_to_boundingbox.py`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/resources/examples/2007-01404285-p2.png` & `tabledetect-0.2.5/tabledetect/resources/examples/2007-01404285-p2.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/resources/examples/2007-02501625-p3.png` & `tabledetect-0.2.5/tabledetect/resources/examples/2007-02501625-p3.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/resources/examples/2008-75500021-p4.png` & `tabledetect-0.2.5/tabledetect/resources/examples/2008-75500021-p4.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/resources/examples/2008-75500021-p8.png` & `tabledetect-0.2.5/tabledetect/resources/examples/2008-75500021-p8.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/resources/examples/2020-76400425-p1.png` & `tabledetect-0.2.5/tabledetect/resources/examples/2020-76400425-p1.png`

 * *Files identical despite different names*

### Comparing `tabledetect-0.2.4/tabledetect/tabledetect.py` & `tabledetect-0.2.5/tabledetect/tabledetect.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     if not image_format.startswith('.'):
         image_format = f'.{image_format}'
 
     # Detect
     logging.info('Detecting objects in your source files')
     if os.path.exists(PATH_OUT):
         shutil.rmtree(PATH_OUT)
-        os.makedirs(PATH_OUT)
+    os.makedirs(PATH_OUT)
     command = f'{PATH_PYTHON} "{PATH_SCRIPT_DETECT}"' \
                 f' --weights {PATH_WEIGHTS}' \
                 f' --conf {threshold_confidence}' \
                 f' --img-size {model_image_size}' \
                 f' --source {path_input}' \
                 f' --save-txt --save-conf' \
                 f' --project out --name table-detect' \
```

### Comparing `tabledetect-0.2.4/PKG-INFO` & `tabledetect-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabledetect
-Version: 0.2.4
+Version: 0.2.5
 Summary: Detects tables in images using a custom yolo-v7 model. Very much work in progress
 Author-email: Jesse Wursten <jessaius+tabledetect@hotmail.com>
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: matplotlib>=3.2.2
 Requires-Dist: numpy>=1.18.5,<1.24.0
```

