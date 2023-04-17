# Comparing `tmp/pokemon-go-video-analysis-0.0.0.0.5.2.tar.gz` & `tmp/pokemon-go-video-analysis-0.0.0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokemon-go-video-analysis-0.0.0.0.5.2.tar", last modified: Wed Apr  5 16:50:17 2023, max compression
+gzip compressed data, was "pokemon-go-video-analysis-0.0.0.0.5.3.tar", last modified: Mon Apr 17 06:00:34 2023, max compression
```

## Comparing `pokemon-go-video-analysis-0.0.0.0.5.2.tar` & `pokemon-go-video-analysis-0.0.0.0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-05 16:50:17.245247 pokemon-go-video-analysis-0.0.0.0.5.2/
--rw-r--r--   0 tandonp    (501) staff       (20)    35149 2022-02-28 08:31:59.000000 pokemon-go-video-analysis-0.0.0.0.5.2/LICENSE
--rw-r--r--   0 tandonp    (501) staff       (20)       79 2022-04-03 00:28:35.000000 pokemon-go-video-analysis-0.0.0.0.5.2/MANIFEST.in
--rw-r--r--   0 tandonp    (501) staff       (20)     1357 2023-04-05 16:50:17.245083 pokemon-go-video-analysis-0.0.0.0.5.2/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)      884 2023-04-05 16:38:56.000000 pokemon-go-video-analysis-0.0.0.0.5.2/README.md
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-05 16:50:17.243824 pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/
--rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-02-28 05:34:12.000000 pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/__init__.py
--rw-r--r--   0 tandonp    (501) staff       (20)      739 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/calc.py
--rw-r--r--   0 tandonp    (501) staff       (20)    10102 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/ocr_log_parser.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2507 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/op.py
--rw-r--r--   0 tandonp    (501) staff       (20)     2089 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/pipeline.py
--rw-r--r--   0 tandonp    (501) staff       (20)     7145 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/result.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-05 16:50:17.244580 pokemon-go-video-analysis-0.0.0.0.5.2/pokemon_go_video_analysis.egg-info/
--rw-r--r--   0 tandonp    (501) staff       (20)     1357 2023-04-05 16:50:17.000000 pokemon-go-video-analysis-0.0.0.0.5.2/pokemon_go_video_analysis.egg-info/PKG-INFO
--rw-r--r--   0 tandonp    (501) staff       (20)      504 2023-04-05 16:50:17.000000 pokemon-go-video-analysis-0.0.0.0.5.2/pokemon_go_video_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-05 16:50:17.000000 pokemon-go-video-analysis-0.0.0.0.5.2/pokemon_go_video_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       23 2023-04-05 16:50:17.000000 pokemon-go-video-analysis-0.0.0.0.5.2/pokemon_go_video_analysis.egg-info/requires.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       14 2023-04-05 16:50:17.000000 pokemon-go-video-analysis-0.0.0.0.5.2/pokemon_go_video_analysis.egg-info/top_level.txt
--rw-r--r--   0 tandonp    (501) staff       (20)      135 2023-03-23 06:47:24.000000 pokemon-go-video-analysis-0.0.0.0.5.2/pyproject.toml
--rw-r--r--   0 tandonp    (501) staff       (20)       22 2023-03-23 06:49:46.000000 pokemon-go-video-analysis-0.0.0.0.5.2/requirements.txt
--rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-05 16:50:17.245304 pokemon-go-video-analysis-0.0.0.0.5.2/setup.cfg
--rw-r--r--   0 tandonp    (501) staff       (20)      810 2023-04-05 16:50:11.000000 pokemon-go-video-analysis-0.0.0.0.5.2/setup.py
-drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-05 16:50:17.244879 pokemon-go-video-analysis-0.0.0.0.5.2/test/
--rw-r--r--   0 tandonp    (501) staff       (20)     2527 2023-04-03 05:32:33.000000 pokemon-go-video-analysis-0.0.0.0.5.2/test/test_end_to_end.py
--rw-r--r--   0 tandonp    (501) staff       (20)     1578 2023-04-03 05:32:33.000000 pokemon-go-video-analysis-0.0.0.0.5.2/test/test_op.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 06:00:34.539507 pokemon-go-video-analysis-0.0.0.0.5.3/
+-rw-r--r--   0 tandonp    (501) staff       (20)    35149 2022-02-28 08:31:59.000000 pokemon-go-video-analysis-0.0.0.0.5.3/LICENSE
+-rw-r--r--   0 tandonp    (501) staff       (20)       79 2022-04-03 00:28:35.000000 pokemon-go-video-analysis-0.0.0.0.5.3/MANIFEST.in
+-rw-r--r--   0 tandonp    (501) staff       (20)     1357 2023-04-17 06:00:34.539328 pokemon-go-video-analysis-0.0.0.0.5.3/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)      884 2023-04-05 16:38:56.000000 pokemon-go-video-analysis-0.0.0.0.5.3/README.md
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 06:00:34.537813 pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/
+-rw-r--r--   0 tandonp    (501) staff       (20)        0 2022-02-28 05:34:12.000000 pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/__init__.py
+-rw-r--r--   0 tandonp    (501) staff       (20)      739 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/calc.py
+-rw-r--r--   0 tandonp    (501) staff       (20)    10102 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/ocr_log_parser.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2507 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/op.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     2984 2023-04-17 05:53:35.000000 pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/pipeline.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     7145 2023-04-03 04:46:26.000000 pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/result.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 06:00:34.538569 pokemon-go-video-analysis-0.0.0.0.5.3/pokemon_go_video_analysis.egg-info/
+-rw-r--r--   0 tandonp    (501) staff       (20)     1357 2023-04-17 06:00:34.000000 pokemon-go-video-analysis-0.0.0.0.5.3/pokemon_go_video_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 tandonp    (501) staff       (20)      504 2023-04-17 06:00:34.000000 pokemon-go-video-analysis-0.0.0.0.5.3/pokemon_go_video_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)        1 2023-04-17 06:00:34.000000 pokemon-go-video-analysis-0.0.0.0.5.3/pokemon_go_video_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       23 2023-04-17 06:00:34.000000 pokemon-go-video-analysis-0.0.0.0.5.3/pokemon_go_video_analysis.egg-info/requires.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       14 2023-04-17 06:00:34.000000 pokemon-go-video-analysis-0.0.0.0.5.3/pokemon_go_video_analysis.egg-info/top_level.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)      135 2023-03-23 06:47:24.000000 pokemon-go-video-analysis-0.0.0.0.5.3/pyproject.toml
+-rw-r--r--   0 tandonp    (501) staff       (20)       22 2023-03-23 06:49:46.000000 pokemon-go-video-analysis-0.0.0.0.5.3/requirements.txt
+-rw-r--r--   0 tandonp    (501) staff       (20)       38 2023-04-17 06:00:34.539559 pokemon-go-video-analysis-0.0.0.0.5.3/setup.cfg
+-rw-r--r--   0 tandonp    (501) staff       (20)      810 2023-04-17 06:00:28.000000 pokemon-go-video-analysis-0.0.0.0.5.3/setup.py
+drwxr-xr-x   0 tandonp    (501) staff       (20)        0 2023-04-17 06:00:34.538884 pokemon-go-video-analysis-0.0.0.0.5.3/test/
+-rw-r--r--   0 tandonp    (501) staff       (20)     2527 2023-04-03 05:32:33.000000 pokemon-go-video-analysis-0.0.0.0.5.3/test/test_end_to_end.py
+-rw-r--r--   0 tandonp    (501) staff       (20)     1578 2023-04-03 05:32:33.000000 pokemon-go-video-analysis-0.0.0.0.5.3/test/test_op.py
```

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/LICENSE` & `pokemon-go-video-analysis-0.0.0.0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/PKG-INFO` & `pokemon-go-video-analysis-0.0.0.0.5.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokemon-go-video-analysis
-Version: 0.0.0.0.5.2
+Version: 0.0.0.0.5.3
 Summary: Pokemon Go Video Analysis
 Home-page: https://github.com/prateekt/pokemon-go-video-analysis
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/README.md` & `pokemon-go-video-analysis-0.0.0.0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/calc.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/calc.py`

 * *Files identical despite different names*

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/ocr_log_parser.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/ocr_log_parser.py`

 * *Files identical despite different names*

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/op.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/op.py`

 * *Files identical despite different names*

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/pipeline.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List
+import os
+from typing import List, Optional
 
 from algo_ops.ops.op import Op
 from algo_ops.pipeline.pipeline import Pipeline
 from ocr_ops.framework.op.ffmpeg_op import FFMPEGOp
 from ocr_ops.framework.pipeline.ocr_pipeline import OCRPipeline, OCRMethod, OutputType
 
 from battle_logger.op import BattleLoggerOp
@@ -27,14 +28,15 @@
             ),
             OCRPipeline(
                 img_pipeline=None,
                 ocr_method=OCRMethod.EASYOCR,
                 output_type=OutputType.TEXTBOX,
                 text_pipeline=None,
                 autosave_output_img_path=None,
+                store_intermediate_images=False,
             ),
             BattleLoggerOp(),
         ]
         return ops
 
     def set_output_paths(
         self, image_out_path: str, autosave_output_img_path: str
@@ -49,9 +51,29 @@
         ffmpeg_op = self.ops[op_names[0]]
         assert isinstance(ffmpeg_op, FFMPEGOp)
         ocr_pipeline_op = self.ops[op_names[1]]
         assert isinstance(ocr_pipeline_op, OCRPipeline)
         ffmpeg_op.image_out_path = image_out_path
         ocr_pipeline_op.ocr_op.autosave_output_img_path = autosave_output_img_path
 
+    def save_output(self, out_path: str = ".", basename: Optional[str] = None) -> None:
+        """
+        Saves pipeline Op outputs to file.
+
+        param out_path: Path to where output should go
+        param basename: Basename of output file
+        """
+        os.makedirs(out_path, exist_ok=True)
+        for i, op_name in enumerate(self.ops.keys()):
+            op = self.ops[op_name]
+            assert isinstance(op, Op)
+            op_pipeline_name = self._pipeline_op_name(op=op)
+            if i == 0:
+                op.save_input(out_path=out_path, basename=op_pipeline_name)
+            # This is hack to get around dropping of input/output images in OCRPipeline
+            try:
+                op.save_output(out_path=out_path, basename=op_pipeline_name)
+            except ValueError:
+                pass
+
     def __init__(self):
         super().__init__(ops=self.get_arch())
```

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/battle_logger/result.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/battle_logger/result.py`

 * *Files identical despite different names*

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/pokemon_go_video_analysis.egg-info/PKG-INFO` & `pokemon-go-video-analysis-0.0.0.0.5.3/pokemon_go_video_analysis.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokemon-go-video-analysis
-Version: 0.0.0.0.5.2
+Version: 0.0.0.0.5.3
 Summary: Pokemon Go Video Analysis
 Home-page: https://github.com/prateekt/pokemon-go-video-analysis
 Author: Prateek Tandon
 Author-email: prateek1.tandon@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/setup.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="pokemon-go-video-analysis",
-    version="0.0.0.0.5.2",
+    version="0.0.0.0.5.3",
     author="Prateek Tandon",
     author_email="prateek1.tandon@gmail.com",
     description="Pokemon Go Video Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prateekt/pokemon-go-video-analysis",
     packages=setuptools.find_packages(),
```

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/test/test_end_to_end.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/test/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `pokemon-go-video-analysis-0.0.0.0.5.2/test/test_op.py` & `pokemon-go-video-analysis-0.0.0.0.5.3/test/test_op.py`

 * *Files identical despite different names*

