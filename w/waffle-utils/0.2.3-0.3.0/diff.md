# Comparing `tmp/waffle_utils-0.2.3.tar.gz` & `tmp/waffle_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_utils-0.2.3.tar", last modified: Mon Apr 10 10:41:33 2023, max compression
+gzip compressed data, was "waffle_utils-0.3.0.tar", last modified: Mon Apr 17 10:32:15 2023, max compression
```

## Comparing `waffle_utils-0.2.3.tar` & `waffle_utils-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,41 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      140 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2619 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1544 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       71 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2667 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3383 2023-04-10 10:41:06.000000 waffle_utils-0.2.3/tests/test_cli.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       22 2023-04-10 10:41:06.000000 waffle_utils-0.2.3/waffle_utils/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       89 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    25766 2023-04-10 10:41:06.000000 waffle_utils-0.2.3/waffle_utils/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/dataset/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      185 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12457 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      550 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5283 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2653 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      188 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/dataset/format.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/file/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4706 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/io.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      475 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/network.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3240 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/file/search.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/image/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      128 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/image/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      332 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/image/io.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/log/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      120 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/log/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1701 2023-03-28 04:12:00.000000 waffle_utils-0.2.3/waffle_utils/log/template.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      238 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/log/time.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4698 2023-03-28 04:12:00.000000 waffle_utils-0.2.3/waffle_utils/run.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       69 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      435 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/utils/validators.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils/video/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1089 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/video/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      693 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/video/io.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4104 2023-03-20 23:39:58.000000 waffle_utils-0.2.3/waffle_utils/video/tools.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-10 10:41:33.833985 waffle_utils-0.2.3/waffle_utils.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2619 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1023 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       78 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       13 2023-04-10 10:41:33.000000 waffle_utils-0.2.3/waffle_utils.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      140 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1398 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      323 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       90 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2667 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2466 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/tests/test_cli.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       22 2023-04-17 10:30:16.000000 waffle_utils-0.3.0/waffle_utils/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/file/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/file/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4706 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/file/io.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      475 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/file/network.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3242 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/file/search.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/image/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      130 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/image/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      332 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/image/io.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/log/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      120 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/log/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1701 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/log/template.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      238 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/log/time.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3295 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/run.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       69 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      435 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/utils/validators.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/video/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1089 2023-04-17 10:27:03.000000 waffle_utils-0.3.0/waffle_utils/video/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1991 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/video/io.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4682 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/video/tools.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils/visualize/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      105 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/visualize/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10198 2023-04-17 10:29:30.000000 waffle_utils-0.3.0/waffle_utils/visualize/plot.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-04-17 10:32:15.284190 waffle_utils-0.3.0/waffle_utils.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1398 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      792 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       44 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       97 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       13 2023-04-17 10:32:15.000000 waffle_utils-0.3.0/waffle_utils.egg-info/top_level.txt
```

### Comparing `waffle_utils-0.2.3/setup.py` & `waffle_utils-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.3/tests/test_cli.py` & `waffle_utils-0.3.0/tests/test_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,24 +33,14 @@
 
 @pytest.fixture(scope="module")
 def extract_dir(tmp_path_module):
     return tmp_path_module / "tmp/extract"
 
 
 @pytest.fixture(scope="module")
-def data_root_dir(tmp_path_module):
-    return tmp_path_module / "tmp/dataset"
-
-
-@pytest.fixture(scope="module")
-def dataset_name():
-    return "mnist"
-
-
-@pytest.fixture(scope="module")
 def coco_root_dir(extract_dir):
     return extract_dir / "images"
 
 
 @pytest.fixture(scope="module")
 def coco_file(extract_dir):
     return extract_dir / "coco.json"
@@ -65,35 +55,14 @@
 
 def test_unzip(zip_file, extract_dir):
     run(
         f"python -m waffle_utils.run unzip --file-path {zip_file} --output-dir {extract_dir}"
     )
 
 
-def test_from_coco(data_root_dir, dataset_name, coco_file, coco_root_dir):
-    run(
-        f"python -m waffle_utils.run from_coco --name {dataset_name} --coco-file {coco_file} --coco-root-dir {coco_root_dir} --root-dir {data_root_dir}"
-    )
-
-
-def test_split(data_root_dir, dataset_name):
-    run(
-        f"python -m waffle_utils.run split --name {dataset_name} --root-dir {data_root_dir} --train-split-ratio 0.8"
-    )
-
-
-def test_export(data_root_dir, dataset_name):
-    run(
-        f"python -m waffle_utils.run export --name {dataset_name} --root-dir {data_root_dir} --export-format yolo_detection"
-    )
-    run(
-        f"python -m waffle_utils.run export --name {dataset_name} --root-dir {data_root_dir} --export-format coco_detection"
-    )
-
-
 # Define fixtures and tests for video-related functions
 @pytest.fixture(scope="module")
 def input_path():
     return Path("tests/video/test.mp4")
 
 
 @pytest.fixture(scope="module")
@@ -110,15 +79,15 @@
 def output_path(tmp_path_module):
     return tmp_path_module / f"test.{DEFAULT_VIDEO_EXTENSION}"
 
 
 # Define tests for video-related functions
 def test_extract_frames(input_path, output_dir):
     run(
-        f"python -m waffle_utils.run extract_frames --input-path {input_path} --output-dir {output_dir} --frame-rate 30  --output-image-extension {DEFAULT_IMAGE_EXTENSION}"
+        f"python -m waffle_utils.run extract_frames --input-path {input_path} --output-dir {output_dir} --num-of-frames 3 --interval-second 3 --output-image-extension {DEFAULT_IMAGE_EXTENSION}"
     )
 
 
 def test_create_video(input_dir, output_path):
     run(
         f"python -m waffle_utils.run create_video --input-dir {input_dir} --output-path {output_path} --frame-rate 30"
     )
```

### Comparing `waffle_utils-0.2.3/waffle_utils/file/io.py` & `waffle_utils-0.3.0/waffle_utils/file/io.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.3/waffle_utils/file/search.py` & `waffle_utils-0.3.0/waffle_utils/file/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import List, Optional, Union
 
 from natsort import natsorted
 
-from waffle_utils.image import SUPPORTED_IMAGE_EXTENSION
+from waffle_utils.image import SUPPORTED_IMAGE_EXTENSIONS
 from waffle_utils.video import SUPPORTED_VIDEO_EXTENSION
 
 
 def get_files(
     directory: Union[str, Path], extension: Union[list[str], str, None] = None
 ) -> list:
     """
@@ -41,15 +41,15 @@
 
     Args:
         directory (Union[str, Path]): Path to the directory.
 
     Returns:
         list: List of image file paths.
     """
-    return get_files(directory, SUPPORTED_IMAGE_EXTENSION)
+    return get_files(directory, SUPPORTED_IMAGE_EXTENSIONS)
 
 
 def get_video_files(directory: Union[str, Path]) -> list:
     """
     Retrieves a list of all video files in a directory.
 
     Args:
```

### Comparing `waffle_utils-0.2.3/waffle_utils/log/template.py` & `waffle_utils-0.3.0/waffle_utils/log/template.py`

 * *Files identical despite different names*

### Comparing `waffle_utils-0.2.3/waffle_utils/video/__init__.py` & `waffle_utils-0.3.0/waffle_utils/video/__init__.py`

 * *Files identical despite different names*

