# Comparing `tmp/digital-eval-1.2.1.tar.gz` & `tmp/digital-eval-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital-eval-1.2.1.tar", last modified: Thu Nov 17 06:44:19 2022, max compression
+gzip compressed data, was "digital-eval-1.5.0.tar", last modified: Mon Apr 17 09:23:47 2023, max compression
```

## Comparing `digital-eval-1.2.1.tar` & `digital-eval-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2022-11-17 06:44:19.133403 digital-eval-1.2.1/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1107 2022-07-13 13:34:42.000000 digital-eval-1.2.1/LICENSE
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       11 2022-11-16 10:06:15.000000 digital-eval-1.2.1/MANIFEST.in
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4550 2022-11-17 06:44:19.133403 digital-eval-1.2.1/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     3958 2022-11-15 13:27:11.000000 digital-eval-1.2.1/README.md
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       87 2022-11-15 13:27:11.000000 digital-eval-1.2.1/pyproject.toml
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      909 2022-11-17 06:44:19.133403 digital-eval-1.2.1/setup.cfg
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2022-11-17 06:44:19.133403 digital-eval-1.2.1/src/
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2022-11-17 06:44:19.133403 digital-eval-1.2.1/src/digital_eval/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        5 2022-11-17 06:40:25.000000 digital-eval-1.2.1/src/digital_eval/VERSION
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      556 2022-11-15 13:27:11.000000 digital-eval-1.2.1/src/digital_eval/__init__.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     7484 2022-11-15 13:27:11.000000 digital-eval-1.2.1/src/digital_eval/cli.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    28550 2022-11-15 13:27:11.000000 digital-eval-1.2.1/src/digital_eval/evaluation.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    14661 2022-11-15 13:27:11.000000 digital-eval-1.2.1/src/digital_eval/metrics.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    14348 2022-11-15 13:27:11.000000 digital-eval-1.2.1/src/digital_eval/model.py
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    14939 2022-11-15 13:27:11.000000 digital-eval-1.2.1/src/digital_eval/model_legacy.py
-drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2022-11-17 06:44:19.133403 digital-eval-1.2.1/src/digital_eval.egg-info/
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4550 2022-11-17 06:44:19.000000 digital-eval-1.2.1/src/digital_eval.egg-info/PKG-INFO
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      492 2022-11-17 06:44:19.000000 digital-eval-1.2.1/src/digital_eval.egg-info/SOURCES.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2022-11-17 06:44:19.000000 digital-eval-1.2.1/src/digital_eval.egg-info/dependency_links.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       56 2022-11-17 06:44:19.000000 digital-eval-1.2.1/src/digital_eval.egg-info/entry_points.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       29 2022-11-17 06:44:19.000000 digital-eval-1.2.1/src/digital_eval.egg-info/requires.txt
--rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       13 2022-11-17 06:44:19.000000 digital-eval-1.2.1/src/digital_eval.egg-info/top_level.txt
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:23:47.316821 digital-eval-1.5.0/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     1107 2022-07-13 13:34:42.000000 digital-eval-1.5.0/LICENSE
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       11 2022-11-16 10:06:15.000000 digital-eval-1.5.0/MANIFEST.in
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5495 2023-04-17 09:23:47.316821 digital-eval-1.5.0/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4903 2023-04-17 09:05:33.000000 digital-eval-1.5.0/README.md
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       87 2022-11-15 13:27:11.000000 digital-eval-1.5.0/pyproject.toml
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      940 2023-04-17 09:23:47.316821 digital-eval-1.5.0/setup.cfg
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:23:47.312821 digital-eval-1.5.0/src/
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:23:47.316821 digital-eval-1.5.0/src/digital_eval/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        6 2023-04-17 08:34:47.000000 digital-eval-1.5.0/src/digital_eval/VERSION
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      609 2023-03-28 09:38:32.000000 digital-eval-1.5.0/src/digital_eval/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     7484 2022-11-15 13:27:11.000000 digital-eval-1.5.0/src/digital_eval/cli.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    28362 2023-03-28 09:38:32.000000 digital-eval-1.5.0/src/digital_eval/evaluation.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    16203 2023-04-17 08:22:56.000000 digital-eval-1.5.0/src/digital_eval/metrics.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    26481 2023-03-28 09:38:32.000000 digital-eval-1.5.0/src/digital_eval/model.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)    14939 2022-11-15 13:27:11.000000 digital-eval-1.5.0/src/digital_eval/model_legacy.py
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:23:47.316821 digital-eval-1.5.0/src/digital_eval.egg-info/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     5495 2023-04-17 09:23:47.000000 digital-eval-1.5.0/src/digital_eval.egg-info/PKG-INFO
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)      559 2023-04-17 09:23:47.000000 digital-eval-1.5.0/src/digital_eval.egg-info/SOURCES.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)        1 2023-04-17 09:23:47.000000 digital-eval-1.5.0/src/digital_eval.egg-info/dependency_links.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       86 2023-04-17 09:23:47.000000 digital-eval-1.5.0/src/digital_eval.egg-info/entry_points.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       29 2023-04-17 09:23:47.000000 digital-eval-1.5.0/src/digital_eval.egg-info/requires.txt
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       22 2023-04-17 09:23:47.000000 digital-eval-1.5.0/src/digital_eval.egg-info/top_level.txt
+drwxrwxr-x   0 hartwig   (1000) hartwig   (1000)        0 2023-04-17 09:23:47.316821 digital-eval-1.5.0/src/ocr_util/
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)       21 2023-03-28 09:38:32.000000 digital-eval-1.5.0/src/ocr_util/__init__.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     2690 2023-04-17 08:33:00.000000 digital-eval-1.5.0/src/ocr_util/cli.py
+-rw-rw-r--   0 hartwig   (1000) hartwig   (1000)     4120 2023-04-17 08:29:20.000000 digital-eval-1.5.0/src/ocr_util/frame.py
```

### Comparing `digital-eval-1.2.1/LICENSE` & `digital-eval-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `digital-eval-1.2.1/PKG-INFO` & `digital-eval-1.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,68 @@
-Metadata-Version: 2.1
-Name: digital-eval
-Version: 1.2.1
-Summary: Evaluate Mass Digitalization Data
-Author: Universitäts- und Landesbibliothek Sachsen-Anhalt
-Author-email: development@bibliothek.uni-halle.de
-Maintainer: Uwe Hartwig
-Maintainer-email: uwe.hartwig@bibliothek.uni-halle.de
-Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-eval
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # digital eval
 
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
 * match automatically groundtruth (i.e. reference data) and candidates by filename
-* use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of candidates (requires ALTO or PAGE format)
+* use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
+  candidates (requires ALTO or PAGE format)
 * aggregate evaluation outcome on domain range (with multiple subdomains)
 * choose from textual metrics based on characters or words plus common Information Retrieval
 * choose between accuracy / error rate and different UTF-8 Python norms
 * formats: ALTO, PAGE or plain text for both groundtruth and candidates
 * speedup with parallel execution
+* additional OCR util:
+  * filter custom areas of single OCR files
 
 ## Installation
 
 ```bash
 pip install digital-eval
 ```
 
 ## Usage
 
 ### Metrics
 
-Calculate similarity (`acc`) or difference (`err`) ratios between single reference/groundtruth and test/candidate item.  
+Calculate similarity (`acc`) or difference (`err`) ratios between single reference/groundtruth and test/candidate item.
 
 #### Edit-Distance based
 
-Character-based text string minus whitechars (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whites, punctuation and digits.
+Character-based text string minus whitechars (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whites,
+punctuation and digits.
 Word/Token-based edit-distance of single tokens identified by whitespaces.
 
 #### Set based
 
 Calculate union of sets of tokens/words (`BoW`, `BagOfWords`).
-Operate on sets of tokens/words with respect to language specific stopwords using [nltk](https://www.nltk.org/)-framework for:
+Operate on sets of tokens/words with respect to language specific stopwords using [nltk](https://www.nltk.org/)
+-framework for:
 
 * Precision (`IRPre`, `Pre`, `Precision`): How many tokens from candidate are in groundtruth reference?
 * Recall (`IRRec`, `Rec`, `Recall`): How many tokens from groundtruth reference should candidate include?
 * F-Measure (`IRFMeasure`, `FM`): weighted ratio Precision / Recall
 
 ### UTF-8 Normalisations
 
 Use standard Python Implementation of UTF-8 normalizations; default: `NFKD`.
 
 ### Statistics
 
-Statistics calculated via [numpy](https://numpy.org/) include arithmetic mean, median and outlier detection with interquartile range and are based on the specific groundtruth/reference (ref) for each metric, i.e. char, letters or tokens.
+Statistics calculated via [numpy](https://numpy.org/) include arithmetic mean, median and outlier detection with
+interquartile range and are based on the specific groundtruth/reference (ref) for each metric, i.e. char, letters or
+tokens.
 
 ### Evaluate treelike structures
 
-To evaluate OCR-candidate-data batch-like versus existing Groundtruth, please make sure that your structures fit this way:
+To evaluate OCR-candidate-data batch-like versus existing Groundtruth, please make sure that your structures fit this
+way:
 
 ```bash
 groundtruth root/
 ├── <domain>/ 
 │    └── <subdomain>/
 │         └── <page-01>.gt.xml
 candidate root/
@@ -81,21 +73,44 @@
 
 Now call via:
 
 ```bash
 digital-eval <path-candidate-root>/domain/ -ref <path-groundtruth>/domain/
 ```
 
-for an aggregated overview on stdout. Feel free to increase verbosity via `-v` (or even `-vv`) to get detailed information about each single data set which was evaluated.
+for an aggregated overview on stdout. Feel free to increase verbosity via `-v` (or even `-vv`) to get detailed
+information about each single data set which was evaluated.
+
+Structured OCR is considered to contain valid geometrical and textual data on word level, even though for recent PAGE
+also line level is possible.
+
+### Data problems
+
+Inconsistent OCR Groundtruth with empty texts (ALTO String elements missing CONTENT or PAGE without TextEquiv) or
+invalid geometrical coordinates (less than 3 points or even empty) will lead to evaluation errors if geometry must be
+respected.
+
+## Additional OCR Utils
+
+### Filter Area
 
-Structured OCR is considered to contain valid geometrical and textual data on word level, even though for recent PAGE also line level is possible.
+You can filter a custom area of a page of an OCR file by providing the points of an arbitrary shape.
+The format of the `-p, --points` argument is `<pt_1_x>,<pt_1_y> <pt_2_x>,<pt_2_y> <pt_3_x>,<pt_3_y> ... <pt_n_x>,<pt_n_y>` . For simple rectangular areas this can be expressed also with two points, with first point as top left and second point as bottom right: `<pt_top_left_x>,<pt_top_left_y> <pt_bottom_right_x>,<pt_bottom_right_y>`.
 
-### Data problems  
+The following example filters a rectangular area of 600x400 pixels of a page, which is described by an input ALTO file and saves the result to an output ALTO file
 
-Inconsistent OCR Groundtruth with empty texts (ALTO String elements missing CONTENT or PAGE without TextEquiv) or invalid geometrical coordinates (less than 3 points or even empty) will lead to evaluation errors if geometry must be respected.
+```bash
+ocr-util frame -i page_1.alto.xml -p "0,0 600,0 600,400 0,400" -o page_1_area.alto.xml
+```
+
+Short version with top left and bottom right:
+
+```bash
+ocr-util frame -i page_1.alto.xml -p "0,0 600,400" -o page_1_area.alto.xml
+```
 
 ## Development
 
 Plattform: Intel(R) Core(TM) i5-6500 CPU@3.20GHz, 16GB RAM, Ubuntu 20.04 LTS, Python 3.8.
 
 ```bash
 # clone local
```

### Comparing `digital-eval-1.2.1/setup.cfg` & `digital-eval-1.5.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 project_urls = 
 	Homepage = https://github.com/ulb-sachsen-anhalt/digital-eval
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 install_requires = 
 	rapidfuzz
 	numpy
@@ -29,12 +29,13 @@
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	digital-eval = digital_eval.cli:start
+	ocr-util = ocr_util.cli:start
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `digital-eval-1.2.1/src/digital_eval/__init__.py` & `digital-eval-1.5.0/src/digital_eval/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,18 @@
     MetricIRFM,
 )
 
 from .model import (
     Piece,
     PieceLevel,
     PieceContent,
+    PieceUtil,
+    PieceDimensions,
     to_pieces,
+    from_pieces,
 )
 
 from .model_legacy import (
     OCRToken,
     OCRWord,
     OCRWordLine,
     OCRRegion,
```

### Comparing `digital-eval-1.2.1/src/digital_eval/cli.py` & `digital-eval-1.5.0/src/digital_eval/cli.py`

 * *Files identical despite different names*

### Comparing `digital-eval-1.2.1/src/digital_eval/evaluation.py` & `digital-eval-1.5.0/src/digital_eval/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,41 @@
 # -*- coding: utf-8 -*-
 """OCR Evaluation Module"""
 
+import concurrent.futures
 import copy
 import os
 import re
-import sys
-
 import xml.dom.minidom
 import xml.etree.ElementTree as ET
-import concurrent.futures
-
 from datetime import (
     date
 )
 from multiprocessing import (
     cpu_count
 )
-from typing import (
-    List, 
-    Tuple, 
-)
 from pathlib import (
     Path
 )
-
-import numpy as np
-
-from digital_eval.metrics import (
-    MetricChars,
-    MetricLetters,
-    MetricWords,
-    MetricBoW,
-    MetricIRPre,
-    MetricIRRec,
-    MetricIRFM,
+from typing import (
+    List,
+    Tuple,
 )
 
-from digital_eval.model_legacy import (
-    OCRData,
-)
+import numpy as np
+import sys
 
 from digital_eval.model import (
-    to_pieces,
     Piece,
     PieceLevel,
+    to_pieces,
+)
+from digital_eval.model_legacy import (
+    OCRData,
 )
-
 
 PAGE_2013 = 'http://schema.primaresearch.org/PAGE/gts/pagecontent/2013-07-15'
 XML_NS = {'alto': 'http://www.loc.gov/standards/alto/ns-v3#',
           'pg2013': PAGE_2013}
 
 # just use textual information for evaluation
 # do *not* respect any geometrics
@@ -71,16 +57,16 @@
      * above median of quartile 3 (upper fence)
     """
 
     data_points = [e[1] for e in data_tuples]
     median = np.median(data_points)
     Q1 = np.median([v for v in data_points if v < median])
     Q3 = np.median([v for v in data_points if v > median])
-    regulars = [data 
-                for data in data_tuples 
+    regulars = [data
+                for data in data_tuples
                 if data[1] >= (Q1 - fence_ratio * (Q3 - Q1)) and data[1] <= (Q1 + fence_ratio * (Q3 - Q1))]
     return (regulars, Q1, Q3)
 
 
 def get_statistics(data_points):
     """Get common statistics like mean, median and std for data_points"""
 
@@ -168,19 +154,19 @@
             path_candidates) if names_match(cleared_name, f)]
         if matches:
             return [os.path.join(path_candidates, m) for m in matches]
 
     # 3: assume gt is textfile and name is contained in results data
     elif re.match(r'^[\d{5,}].*\.txt$', gt_filename):
         cleared_name = os.path.splitext(gt_filename)[0]
-        matches = [f 
-                   for f in os.listdir(path_candidates) 
+        matches = [f
+                   for f in os.listdir(path_candidates)
                    if names_match(cleared_name, f)]
         if matches:
-            return [os.path.join(path_candidates, m) 
+            return [os.path.join(path_candidates, m)
                     for m in matches]
 
     return []
 
 
 def match_candidate(path_gt_file_pattern):
     '''Find candidates that match groundtruth'''
@@ -191,21 +177,22 @@
     gt_path_xml = path_gt_file_pattern + '.xml'
     if os.path.exists(gt_path_xml):
         return gt_path_xml
 
     # inspect all files in given directory if it fits anyway
     # assume groundtruth starts with same tokens
     gt_dir = os.path.dirname(path_gt_file_pattern)
-    gt_files=[f 
-        for f in os.listdir(gt_dir)
-        if f.endswith(".xml") or f.endswith(".txt")]
+    gt_files = [f
+                for f in os.listdir(gt_dir)
+                if f.endswith(".xml") or f.endswith(".txt")]
     for _file in gt_files:
         if _file.startswith(gt_filename):
             return os.path.join(gt_dir, _file)
 
+
 def names_match(name_groundtruth, name_candidate):
     if '.gt' in name_groundtruth:
         name_groundtruth = name_groundtruth.replace('.gt', '')
     if name_groundtruth in name_candidate:
         candidate_ext = os.path.splitext(name_candidate)[1]
         if candidate_ext == '.txt' or candidate_ext == '.xml':
             return True
@@ -231,15 +218,15 @@
         return ((x0, y0), (x1, y1))
 
     with open(file_path) as _handle:
         # rather brute force approach
         # to recognize OCR formats inside
         start_token = _handle.read(128)
         _frame_points = None
-        
+
         # switch by estimated ocr format
         if 'alto' in start_token:
             # legacy: read from custom ALTO meta data
             root_element = ET.parse(file_path).getroot()
             element = root_element.find(
                 './/alto:Tags/alto:OtherTag[@ID="ulb_groundtruth_points"]', XML_NS)
             if element is not None:
@@ -356,24 +343,24 @@
             _level = top_piece.subject
             if _level:
                 _gt_type = _level
         # explicit filter frame?
         if not frame:
             frame = top_piece.dimensions
         elif len(frame) == 2:
-            frame = [[frame[0][0],frame[0][1]],
-                    [frame[1][0],frame[0][1]],
-                    [frame[1][0],frame[1][1]],
-                    [frame[0][0],frame[1][1]]]
+            frame = [[frame[0][0], frame[0][1]],
+                     [frame[1][0], frame[0][1]],
+                     [frame[1][0], frame[1][1]],
+                     [frame[0][0], frame[1][1]]]
         frame_piece = Piece()
         frame_piece.dimensions = frame
         filter_word_pieces(frame_piece, top_piece)
-        the_lines = [l 
-                     for r in top_piece.pieces 
-                     for l in r.pieces 
+        the_lines = [l
+                     for r in top_piece.pieces
+                     for l in r.pieces
                      if l.transcription and l.level == PieceLevel.LINE]
         if oneliner:
             return (_gt_type, top_piece.transcription, len(the_lines))
         else:
             return (_gt_type, [l.transcription for l in the_lines], len(the_lines))
     except xml.parsers.expat.ExpatError as _:
         with open(file_path, mode='r', encoding='utf-8') as fhandle:
@@ -406,27 +393,27 @@
     while _tmp_stack:
         _current = _tmp_stack.pop()
         if _current.pieces:
             _tmp_stack += _current.pieces
             _total_stack += _current.pieces
     # now pick words
     _words = [_p for _p in _total_stack if _p.level == PieceLevel.WORD]
-        
+
     # check for each word piece
     for _word in _words:
         if _word not in frame:
             _filtered += 1
             _uplete(_word)
     return _filtered
 
 
 def _uplete(curr):
     if len(curr.pieces) == 0:
         _pa = curr.parent
-        _pa.pieces.remove(curr)
+        _pa.remove_pieces(curr)
         _uplete(_pa)
 
 
 def _normalize_gt_type(label) -> str:
     if label.startswith('art'):
         return 'article'
     elif label.startswith('ann'):
@@ -442,15 +429,15 @@
     regarding a specific set
     = a directory, which's name serves as eval_key
 
     optional:
         enclose EvaluationResult with outliers removed
     '''
 
-    def __init__(self, eval_key: str, n_total: int = 1, n_chars = 0, n_lines = 0):
+    def __init__(self, eval_key: str, n_total: int = 1, n_chars=0, n_lines=0):
         self.eval_key = eval_key
         self.total_mean = 0.0
         self.n_total = n_total
         self.n_outlier = 0
         self.n_chars = n_chars
         self.n_lines = n_lines
         self.mean = 0.0
@@ -458,17 +445,17 @@
         self.median = 0.0
         # set special descendant from same type
         # to hold optional metrics regarding
         # removed outliers
         self.cleared_result = None
 
     def get_defaults(self):
-        '''Provide default data (eval_key, number of elements, mean) that must be available'''
+        """Provide default data (eval_key, number of elements, mean) that must be available"""
 
-        return (self.eval_key, self.n_total, self.mean, self.median, self.n_chars)
+        return self.eval_key, self.n_total, self.mean, self.median, self.n_chars
 
 
 class EvalEntry:
     """Container to transform evaluation results into
     string representation"""
 
     def __init__(self, path):
@@ -537,15 +524,15 @@
         if sequential or self.is_sequential:
             _entries = [self._wrap_eval_entry(e) for e in entries]
         else:
             cpus = cpu_count()
             n_executors = cpus - 1 if cpus > 3 else 1
             if self.verbosity == 1:
                 print(f"[DEBUG] use {n_executors} executors ({cpus}) to create evaluation data")
-            
+
             with concurrent.futures.ProcessPoolExecutor(max_workers=n_executors) as executor:
                 try:
                     _entries = list(executor.map(self._wrap_eval_entry, entries, timeout=EVAL_TIMEOUT))
                 except concurrent.futures.TimeoutError:
                     print(f"[ERROR] takes longer than {EVAL_TIMEOUT}s to evaluate {len(entries)} entries!")
                     sys.exit(1)
                 except Exception as err:
@@ -554,24 +541,24 @@
 
         # review evaluation results
         if _entries:
             _not_nones = [e for e in _entries if e is not None]
             if self.verbosity == 1:
                 print(f"[DEBUG] processed {len(_entries)}, omitted {len(_entries) - len(_not_nones)} empty results")
             self.evaluation_entries = _not_nones
-        
+
         self.evaluation_entries = sorted(self.evaluation_entries, key=lambda e: e.path_c)
         # detail report
-        self.evaluation_report['candidates'] = [self._generate_report_candidate(e) 
+        self.evaluation_report['candidates'] = [self._generate_report_candidate(e)
                                                 for e in self.evaluation_entries]
-        
+
     def _wrap_eval_entry(self, entry: EvalEntry):
         """Wrapper for creation of evaluation data
         to be used in common process-pooling"""
-        
+
         if entry.path_g:
             try:
                 return self.eval_entry(entry)
             except Exception as exc:
                 print(f"[WARN ][{entry.path_g}] _wrap {exc}")
 
     def eval_entry(self, entry: EvalEntry) -> EvalEntry:
@@ -587,15 +574,15 @@
         if coords is not None and self.verbosity >= 2:
             print(f"[TRACE] token coordinates {coords[0]}, {coords[1]}")
 
         # load ground-thruth text
         (gt_type, txt_gt, _) = self.to_text_func(path_g, oneliner=True)
         if not txt_gt:
             print(f"[WARN ] {path_g} contains no text")
-        
+
         # if text mode is enforced
         # forget groundtruth coordinates
         coords = None if self.text_mode else coords
 
         # read candidate data as text
         (_, txt_c, _) = self.to_text_func(path_c, coords, oneliner=True)
         if self.verbosity >= 2:
@@ -629,15 +616,15 @@
 
     def _generate_report_candidate(self, the_entry):
         try:
             image_name = os.path.basename(the_entry.path_c)
             _type = the_entry.gt_type
             if '+' in image_name and '_' in image_name:
                 _tkns = image_name.split('_')
-                image_name = _tkns[0].replace('+',':') + '_' + _tkns[1]
+                image_name = _tkns[0].replace('+', ':') + '_' + _tkns[1]
             if '.xml' in image_name:
                 image_name = image_name.replace('.xml', '')
             gt_label = f"({_type[:3]})" if _type and _type != NOT_SET else ''
             return f'[{image_name}]{gt_label} [{the_entry}]'
         except Exception as exc:
             print(f'[WARN ] {exc}')
 
@@ -662,29 +649,29 @@
             # also calculate statistics (mean, std)
             if len(data_points) > 1:
                 (mean, std, median) = get_statistics(data_points)
                 evaluation_result.mean = mean
                 evaluation_result.median = median
                 evaluation_result.std = std
                 if std >= 1.0:
-                    (regulars, _, _ ) = strip_outliers_from(data_tuples)
+                    (regulars, _, _) = strip_outliers_from(data_tuples)
                     regulars_data_points = [e[1] for e in regulars]
                     clear_result = EvaluationResult(k, len(regulars))
                     (mean2, std2, med2) = get_statistics(regulars_data_points)
                     clear_result.mean = mean2
                     clear_result.std = std2
                     clear_result.median = med2
                     clear_result.n_chars = sum([e[2] for e in regulars])
                     # set as child component
                     evaluation_result.cleared_result = clear_result
             self._add(evaluation_result)
             # re-order
             self.evaluation_results = sorted(self.evaluation_results, key=lambda e: e.eval_key)
 
-    def aggregate(self, by_type=False, by_metrics=[0,1,2,3]):
+    def aggregate(self, by_type=False, by_metrics=[0, 1, 2, 3]):
 
         # precheck - having root dir
         self._check_aggregate_preconditions()
 
         root_base = Path(self.domain_reference).parts[-1]
 
         # aggregate on each directory
@@ -753,8 +740,9 @@
         add_stats = f', std: {result.std:.2f}, median: {med:.2f}' if n_total > 1 else ''
         print(f'[INFO ] "{gt_type}"\t∅: {mean_total:.2f}\t{n_total} items, {_n_refs} refs{add_stats}')
         if result.cleared_result:
             (_, n_t2, mean2, med2, n_c2) = result.cleared_result.get_defaults()
             ccr_std = result.cleared_result.std
             drops = n_total - n_t2
             if drops > 0:
-                print(f'[INFO ] "{gt_type}"\t∅: {mean2:.2f}\t{n_t2} items (-{drops}), {n_c2} refs, std: {ccr_std:.2f}, median: {med2:.2f}')
+                print(
+                    f'[INFO ] "{gt_type}"\t∅: {mean2:.2f}\t{n_t2} items (-{drops}), {n_c2} refs, std: {ccr_std:.2f}, median: {med2:.2f}')
```

### Comparing `digital-eval-1.2.1/src/digital_eval/metrics.py` & `digital-eval-1.5.0/src/digital_eval/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,130 +5,148 @@
     Counter
 )
 from functools import partial
 
 import string
 
 from typing import (
-    List, 
+    List,
     Set,
 )
 
 import unicodedata
 
 from nltk import (
     download,
 )
 from nltk.corpus import (
     stopwords
 )
 from nltk.metrics import (
-    precision,
     recall,
     f_measure
 )
+from nltk.metrics import precision as nltk_precision
+
 from rapidfuzz.string_metric import (
     levenshtein
 )
 
 
 # Python3 standard Unicode Normalization
-# 
+#
 UC_NORMALIZATION = 'NFKD'
 
 
 # whitespaces
 #
 # usual spatium and special control sequences
 WHITESPACES = string.whitespace
 
 
 # punctuations
 #
 #   * regular ASCII-punctuations
 #   * Dashes        \u2012-2017
 #   * Quotations    \u2018-201F
-PUNCTUATIONS = string.punctuation + '\u2012' + '\u2013' + '\u2014' + '\u2015' + '\u2016' + '\u2017' + '\u2018' + '\u2019' + '\u201A' + '\u201B' + '\u201C' + '\u201D' + '\u201E' + '\u201F'
+PUNCTUATIONS = string.punctuation + '\u2012' + '\u2013' + '\u2014' + '\u2015' + '\u2016' + \
+    '\u2017' + '\u2018' + '\u2019' + '\u201A' + '\u201B' + \
+    '\u201C' + '\u201D' + '\u201E' + '\u201F'
 # no special line break delimiter
 PUNCTUATIONS = PUNCTUATIONS + '\u2E17'  # DOUBLE OBLIQUE HYPHEN
 # no spaces
-PUNCTUATIONS = PUNCTUATIONS + '\u0020' + '\u00a0' + '\u2000' + '\u2001' + '\u2002' + '\u2003' + '\u2004' + '\u2005' + '\u2006' + '\u2007' + '\u2008' + '\u2009' + '\u200a' + '\u2028' + '\u205f' + '\u3000'
+PUNCTUATIONS = PUNCTUATIONS + '\u0020' + '\u00a0' + '\u2000' + \
+    '\u2001' + '\u2002' + '\u2003' + '\u2004' + '\u2005' + \
+    '\u2006' + '\u2007' + '\u2008' + '\u2009' + \
+    '\u200a' + '\u2028' + '\u205f' + '\u3000'
 
 
 # digits
 #
-#   * ASCII digits 
+#   * ASCII digits
 #   * arabic digits
 #   * persian / indic digits
-DIGITS = string.digits + '\u0660' + '\u0661' + '\u0662' + '\u0663' + '\u0664' + '\u0665' + '\u0666' + '\u0667' + '\u0668' + '\u0669' 
+DIGITS = string.digits + '\u0660' + '\u0661' + '\u0662' + '\u0663' + \
+    '\u0664' + '\u0665' + '\u0666' + '\u0667' + '\u0668' + '\u0669'
 # persian indic digits
-DIGITS = DIGITS + '\u06f0' + '\u06f1' + '\u06f2' + '\u06f3' + '\u06f4' + '\u06f5' + '\u06f6' + '\u06f7' + '\u06f8' + '\u06f9'
+DIGITS = DIGITS + '\u06f0' + '\u06f1' + '\u06f2' + '\u06f3' + \
+    '\u06f4' + '\u06f5' + '\u06f6' + '\u06f7' + '\u06f8' + '\u06f9'
 
 
 # filter mechanics
 #
 # via Python3 string translation maps
-WHITESPACE_TRANSLATOR =str.maketrans('','', WHITESPACES)
+WHITESPACE_TRANSLATOR = str.maketrans('', '', WHITESPACES)
 PUNCT_TRANLATOR = str.maketrans('', '', PUNCTUATIONS)
 DIGIT_TRANSLATOR = str.maketrans('', '', DIGITS)
 
 
-def filter_whitespaces(a_str) -> str:
+def _filter_whitespaces(a_str) -> str:
     return a_str.translate(WHITESPACE_TRANSLATOR)
 
 
-def filter_puncts(a_str) -> str:
+def _filter_puncts(a_str) -> str:
     return a_str.translate(PUNCT_TRANLATOR)
 
 
-def filter_digits(a_str) -> str:
+def _filter_digits(a_str) -> str:
     return a_str.translate(DIGIT_TRANSLATOR)
 
 
-def tokenize(a_str) -> List[str]:
+def _tokenize(a_str) -> List[str]:
     return a_str.split() if isinstance(a_str, str) else a_str
 
 
-def tokenize_to_sorted_set(a_str) -> Set[str]:
-    return set(sorted(tokenize(a_str)))
+def _tokenize_to_sorted_set(a_str) -> Set[str]:
+    return set(sorted(_tokenize(a_str)))
 
 
 #
 # information retrieval (nltk)
 #
-NLTK_STOPWORDS = ['german', 'russian', 'english', 'french', 'greek', 'arabic', 'turkish', 'italian']
-STOPWORDS_DEFAULT = ['german', 'english', 'arabic','russian']
+NLTK_STOPWORDS = [
+    'german',
+    'russian',
+    'english',
+    'french',
+    'greek',
+    'arabic',
+    'turkish',
+    'italian']
+STOPWORDS_DEFAULT = ['german', 'english', 'arabic', 'russian']
+
+
 def get_stopwords(nltk_mappings=NLTK_STOPWORDS, languages=None) -> Set[str]:
     """Helper Function to gather NLTK stopword data
     * ensure stopwords files are locally available
     * extract them as set
     """
     try:
-        for mapping in nltk_mappings: 
+        for mapping in nltk_mappings:
             stopwords.words(mapping)
     except LookupError:
         download('stopwords')
-    if languages == None:
+    if languages is None:
         languages = STOPWORDS_DEFAULT
-    _stopwords = set([_all_words
-                      for _lang in languages
-                      for _all_words in stopwords.words(_lang)]
-                    )  
+    _stopwords = {_all_words
+                  for _lang in languages
+                  for _all_words in stopwords.words(_lang)
+                  }
     return _stopwords
 
 
-def strip_languages_stopwords(tokens, languages):
+def _strip_languages_stopwords(tokens, languages):
     return tokens - get_stopwords(languages=languages)
 
 
-def strip_stopwords_for(languages):
-    return partial(strip_languages_stopwords, languages=languages)
+def _strip_stopwords_for(languages):
+    return partial(_strip_languages_stopwords, languages=languages)
 
 
-def normalize_unicode(input_str: str, uc_norm_by=UC_NORMALIZATION) -> str: 
+def normalize_unicode(input_str: str, uc_norm_by=UC_NORMALIZATION) -> str:
     """Apply basic unicode normalization
     """
 
     if uc_norm_by is not None:
         input_str = unicodedata.normalize(uc_norm_by, input_str)
     return input_str
 
@@ -140,14 +158,15 @@
     digit_translator = str.maketrans('', '', DIGITS)
     the_content = the_content.translate(punct_translator)
     the_content = the_content.translate(digit_translator)
     return the_content
 
 
 class DigitalEvalMetricException(Exception):
+    """Mark Exception during validation/calculating metrics"""
 
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 
 def _inspect_calculation_object(an_object):
     if not isinstance(an_object, OCRDifferenceMetric):
@@ -157,95 +176,97 @@
         _diff = an_object.diff
         _ref = an_object.n_ref
         if _diff is None or _diff < 0:
             raise DigitalEvalMetricException(f"invalid diff: {_diff}!")
         if _ref is None or _ref < 0:
             raise DigitalEvalMetricException(f"invalid ref: {_ref}!")
     except AttributeError as _ae:
-        raise DigitalEvalMetricException(_ae.args[0])
-    
+        raise DigitalEvalMetricException(_ae.args[0]) from _ae
+
 
 def accuracy_for(the_obj) -> float:
     """Calculate accuracy as ratio of
     correct items, with correct items
-    being expected items minus 
+    being expected items minus
     number of differences.
 
     Respect following corner cases:
     * if less correct items than differences => 0
     * if both correct items and differences eq zero => 1
-      means: nothing to find and it did detect nothing 
-      (i.e. no false-positives) 
+      means: nothing to find and it did detect nothing
+      (i.e. no false-positives)
 
     Args:
-        the_obj (object): object containing information 
+        the_obj (object): object containing information
         about reference data and difference
 
     Returns:
         float: accuracy in range 0.0 - 1.0
     """
 
     _inspect_calculation_object(the_obj)
     diffs = the_obj.diff
     n_refs = len(the_obj._data_reference)
     if (n_refs - diffs) < 0:
-        return 0
+        return 0.0
     if n_refs == 0 and diffs == 0:
         return 1.0
     elif n_refs > 0:
         return (n_refs - diffs) / n_refs
+    else:
+        return 0.0
 
 
 def error_for(the_obj) -> float:
     """Calculate error as ratio of
-    difference and number of 
+    difference and number of
     expected items.
 
     Respect following corner cases:
     * if less expected items than differences => 0
     * if both expected items and differences eq zero => 1
-      means: nothing to find and detected nothing 
-      (i.e. no false-positives) 
+      means: nothing to find and detected nothing
+      (i.e. no false-positives)
 
     Args:
-        the_obj (object): object containing information 
+        the_obj (object): object containing information
         about reference data and difference
 
     Returns:
         float: error in range 0.0 - 1.0
     """
 
     _inspect_calculation_object(the_obj)
     diffs = the_obj.diff
     n_refs = len(the_obj._data_reference)
     if (n_refs - diffs) < 0:
-        return 0
+        return 0.0
     if n_refs == 0 and diffs == 0:
         return 1.0
     elif n_refs > 0:
         return diffs / n_refs
+    else:
+        return 0.0
 
 
 def norm_to_scale(value, scale_by) -> float:
-    """
-    Normalize outcome in range 0 - scale_bound
-    """
-
+    """Normalize outcome in range 0 - scale_by"""
     return value * scale_by
 
 
 def norm_percentual(value):
+    """Normalize value in between 0 - 100"""
     return partial(norm_to_scale, scale_by=100)(value)
 
 
 class OCRDifferenceMetric:
     """Basic definition of a OCRDifferenceMetric"""
 
     def __init__(self, precision, normalization, calc_func,
-        preprocessings=None, postprocessings=None) -> None:
+                 preprocessings=None, postprocessings=None) -> None:
         self.precision = precision
         self._value = None
         self.diff = None
         self._label = None
         self.unicode_normalization = normalization
         self.preprocessings = []
         if isinstance(preprocessings, list):
@@ -258,39 +279,45 @@
         self.input_candidate = None
         self._data_reference = None
         self._data_candidate = None
         self.languages = None
 
     @property
     def reference(self):
+        """Reference/Groundtruth data"""
         return self._data_reference
 
     @reference.setter
     def reference(self, value):
         self.input_reference = value
-        self._data_reference = normalize_unicode(value, self.unicode_normalization)
+        self._data_reference = normalize_unicode(
+            value, self.unicode_normalization)
         self._value = None
 
     @property
     def candidate(self):
+        """Candidate data"""
         return self._data_candidate
 
     @candidate.setter
     def candidate(self, value):
         self.input_candidate = value
         self._data_candidate = normalize_unicode(value)
         self._value = None
 
     @property
     def label(self):
+        """Metric's label"""
         return self._label
 
     @property
-    def n_ref(self):
-        if not hasattr(self, '_data_reference') or self._data_reference is None:
+    def n_ref(self) -> int:
+        """Number of current reference data"""
+        if not hasattr(
+                self, '_data_reference') or self._data_reference is None:
             raise DigitalEvalMetricException("invalid reference data!")
         return len(self._data_reference)
 
     @n_ref.setter
     def n_ref(self, value):
         """Exists only for testing purposes"""
 
@@ -319,160 +346,216 @@
     def _forward(self):
         """Calculate metric's value
         remember this needs further refinement"""
         raise NotImplementedError
 
 
 class MetricChars(OCRDifferenceMetric):
+    """Calculate plain sequent character based metric"""
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings)
+                 preprocessings=None, postprocessings=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings)
         self._label = 'Cs'
         self.name = 'Characters'
-        self.preprocessings = [filter_whitespaces]
+        self.preprocessings = [_filter_whitespaces]
         self.postprocessings = [norm_percentual]
 
     def _forward(self):
         self.diff = edit_distance(self._data_reference, self._data_candidate)
 
 
 class MetricLetters(OCRDifferenceMetric):
+    """Calculate metric for only a certain sub-set of
+    character sequence"""
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings)
+                 preprocessings=None, postprocessings=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings)
         self._label = 'Ls'
-        self.preprocessings = [filter_whitespaces, filter_puncts, filter_digits]
+        self.preprocessings = [
+            _filter_whitespaces,
+            _filter_puncts,
+            _filter_digits]
 
     def _forward(self):
         self.diff = edit_distance(self._data_reference, self._data_candidate)
 
 
 class MetricWords(OCRDifferenceMetric):
+    """Calculate metric for a sequence of word tokens"""
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings)
+                 preprocessings=None, postprocessings=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings)
         self._label = 'Ws'
-        self.preprocessings = [tokenize]
-    
+        self.preprocessings = [_tokenize]
+
     def _forward(self):
         self.diff = edit_distance(self._data_reference, self._data_candidate)
 
 
 class MetricBoW(OCRDifferenceMetric):
+    """Calculate metric for a multiset of word tokens"""
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings)
+                 preprocessings=None, postprocessings=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings)
         self._label = 'BoWs'
-        self.preprocessings = [tokenize]
+        self.preprocessings = [_tokenize]
 
     def _forward(self):
         self.diff = bag_of_tokens(self._data_reference, self._data_candidate)
 
 
 class MetricIR(OCRDifferenceMetric):
+    """Calculate information retrival metrics"""
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None, languages=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings)
+                 preprocessings=None, postprocessings=None, languages=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings)
         self.languages = languages
-        self.preprocessings = [tokenize_to_sorted_set, 
-            strip_stopwords_for(self.languages)
-        ]
+        self.preprocessings = [_tokenize_to_sorted_set,
+                               _strip_stopwords_for(self.languages)
+                               ]
         # no aligning required, we rely on nltk
         self.calc_func = None
         # no percentual value
         self.postprocessings = []
 
     def _forward(self):
         """to remind that this class needs further refinement"""
         raise NotImplementedError
 
 
 class MetricIRPre(MetricIR):
+    """Calculate precision"""
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None, languages=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings, languages)
+                 preprocessings=None, postprocessings=None, languages=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings,
+            languages)
         self._label = 'Pre'
 
     def _forward(self):
         self.diff = ir_precision(self._data_reference, self._data_candidate)
 
 
 class MetricIRRec(MetricIR):
+    "Calculate recall"
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None, languages=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings, languages)
+                 preprocessings=None, postprocessings=None, languages=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings,
+            languages)
         self._label = 'Rec'
 
     def _forward(self):
         self.diff = ir_recall(self._data_reference, self._data_candidate)
 
 
 class MetricIRFM(MetricIR):
+    """Calculate harmonic mean for precision/recall"""
 
     def __init__(self, precision=2, normalization=UC_NORMALIZATION, calc_func=accuracy_for,
-        preprocessings=None, postprocessings=None, languages=None):
-        super().__init__(precision, normalization, calc_func, preprocessings, postprocessings, languages)
+                 preprocessings=None, postprocessings=None, languages=None):
+        super().__init__(
+            precision,
+            normalization,
+            calc_func,
+            preprocessings,
+            postprocessings,
+            languages)
         self._label = 'FM'
 
     def _forward(self):
         self.diff = ir_fmeasure(self._data_reference, self._data_candidate)
 
 
 def edit_distance(reference_data, candidate_data) -> int:
     """Calculate edit distance with levenshtein-distance.
     as sum of edit operations required to get from
     candidate to reference string / token_list
-    
+
     Works with characters and word-like tokens, where
     tokens correspond also to:
     * abbreviations  (like "Nr." or "Etg.")
     * numbers/years  (like "1899")
     * split-up words (line endings/beginnings)
     """
 
     return levenshtein(reference_data, candidate_data)
 
 
-def bag_of_tokens(reference_tokens: List[str], candidate_tokens: List[str]) -> int:
+def bag_of_tokens(reference_tokens: List[str],
+                  candidate_tokens: List[str]) -> int:
     """Calculate intersection/difference
     between reference and candidate token list
     """
 
     return len(_diff(reference_tokens, candidate_tokens))
 
 
 def _diff(gt_tokens, cd_tokens) -> List[str]:
     return list((Counter(gt_tokens) - Counter(cd_tokens)).elements())
 
 
 def ir_precision(reference_data, candidate_data) -> float:
     """Calculate Precision for given languages"""
-    
-    _prec = precision(reference_data, candidate_data) 
+
+    _prec = nltk_precision(reference_data, candidate_data)
     # nltk actually handles this inconsistently ...
-    if _prec == None:
+    if _prec is None:
         _prec = 0.0
     return _prec
 
 
 def ir_recall(reference_data, candidate_data) -> float:
     """Calculate Recall for given languages"""
-    
+
     # here nltk reports 0.0 if nothing recalled
     return recall(reference_data, candidate_data)
 
 
 def ir_fmeasure(reference_data, candidate_data) -> float:
     """Calculate F-Measure for given languages"""
-    
+
     _fm = f_measure(reference_data, candidate_data)
     # required since nltk actually handles this inconsistently ...
-    if _fm == None:
+    if _fm is None:
         _fm = 0.0
     return _fm
```

### Comparing `digital-eval-1.2.1/src/digital_eval/model_legacy.py` & `digital-eval-1.5.0/src/digital_eval/model_legacy.py`

 * *Files identical despite different names*

### Comparing `digital-eval-1.2.1/src/digital_eval.egg-info/PKG-INFO` & `digital-eval-1.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,76 +1,84 @@
 Metadata-Version: 2.1
 Name: digital-eval
-Version: 1.2.1
+Version: 1.5.0
 Summary: Evaluate Mass Digitalization Data
 Author: Universitäts- und Landesbibliothek Sachsen-Anhalt
 Author-email: development@bibliothek.uni-halle.de
 Maintainer: Uwe Hartwig
 Maintainer-email: uwe.hartwig@bibliothek.uni-halle.de
 Project-URL: Homepage, https://github.com/ulb-sachsen-anhalt/digital-eval
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # digital eval
 
 ![example workflow](https://github.com/ulb-sachsen-anhalt/digital-eval/actions/workflows/python-app.yml/badge.svg)
 
 Python3 Tool to report evaluation outcomes from mass digitalization workflows.
 
 ## Features
 
 * match automatically groundtruth (i.e. reference data) and candidates by filename
-* use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of candidates (requires ALTO or PAGE format)
+* use geometric information to evaluate only specific frame (i.e. specific column or region from large page) of
+  candidates (requires ALTO or PAGE format)
 * aggregate evaluation outcome on domain range (with multiple subdomains)
 * choose from textual metrics based on characters or words plus common Information Retrieval
 * choose between accuracy / error rate and different UTF-8 Python norms
 * formats: ALTO, PAGE or plain text for both groundtruth and candidates
 * speedup with parallel execution
+* additional OCR util:
+  * filter custom areas of single OCR files
 
 ## Installation
 
 ```bash
 pip install digital-eval
 ```
 
 ## Usage
 
 ### Metrics
 
-Calculate similarity (`acc`) or difference (`err`) ratios between single reference/groundtruth and test/candidate item.  
+Calculate similarity (`acc`) or difference (`err`) ratios between single reference/groundtruth and test/candidate item.
 
 #### Edit-Distance based
 
-Character-based text string minus whitechars (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whites, punctuation and digits.
+Character-based text string minus whitechars (`Cs`, `Characters`) or Letter-based (`Ls`, `Letters`) minus whites,
+punctuation and digits.
 Word/Token-based edit-distance of single tokens identified by whitespaces.
 
 #### Set based
 
 Calculate union of sets of tokens/words (`BoW`, `BagOfWords`).
-Operate on sets of tokens/words with respect to language specific stopwords using [nltk](https://www.nltk.org/)-framework for:
+Operate on sets of tokens/words with respect to language specific stopwords using [nltk](https://www.nltk.org/)
+-framework for:
 
 * Precision (`IRPre`, `Pre`, `Precision`): How many tokens from candidate are in groundtruth reference?
 * Recall (`IRRec`, `Rec`, `Recall`): How many tokens from groundtruth reference should candidate include?
 * F-Measure (`IRFMeasure`, `FM`): weighted ratio Precision / Recall
 
 ### UTF-8 Normalisations
 
 Use standard Python Implementation of UTF-8 normalizations; default: `NFKD`.
 
 ### Statistics
 
-Statistics calculated via [numpy](https://numpy.org/) include arithmetic mean, median and outlier detection with interquartile range and are based on the specific groundtruth/reference (ref) for each metric, i.e. char, letters or tokens.
+Statistics calculated via [numpy](https://numpy.org/) include arithmetic mean, median and outlier detection with
+interquartile range and are based on the specific groundtruth/reference (ref) for each metric, i.e. char, letters or
+tokens.
 
 ### Evaluate treelike structures
 
-To evaluate OCR-candidate-data batch-like versus existing Groundtruth, please make sure that your structures fit this way:
+To evaluate OCR-candidate-data batch-like versus existing Groundtruth, please make sure that your structures fit this
+way:
 
 ```bash
 groundtruth root/
 ├── <domain>/ 
 │    └── <subdomain>/
 │         └── <page-01>.gt.xml
 candidate root/
@@ -81,21 +89,44 @@
 
 Now call via:
 
 ```bash
 digital-eval <path-candidate-root>/domain/ -ref <path-groundtruth>/domain/
 ```
 
-for an aggregated overview on stdout. Feel free to increase verbosity via `-v` (or even `-vv`) to get detailed information about each single data set which was evaluated.
+for an aggregated overview on stdout. Feel free to increase verbosity via `-v` (or even `-vv`) to get detailed
+information about each single data set which was evaluated.
 
-Structured OCR is considered to contain valid geometrical and textual data on word level, even though for recent PAGE also line level is possible.
+Structured OCR is considered to contain valid geometrical and textual data on word level, even though for recent PAGE
+also line level is possible.
 
-### Data problems  
+### Data problems
 
-Inconsistent OCR Groundtruth with empty texts (ALTO String elements missing CONTENT or PAGE without TextEquiv) or invalid geometrical coordinates (less than 3 points or even empty) will lead to evaluation errors if geometry must be respected.
+Inconsistent OCR Groundtruth with empty texts (ALTO String elements missing CONTENT or PAGE without TextEquiv) or
+invalid geometrical coordinates (less than 3 points or even empty) will lead to evaluation errors if geometry must be
+respected.
+
+## Additional OCR Utils
+
+### Filter Area
+
+You can filter a custom area of a page of an OCR file by providing the points of an arbitrary shape.
+The format of the `-p, --points` argument is `<pt_1_x>,<pt_1_y> <pt_2_x>,<pt_2_y> <pt_3_x>,<pt_3_y> ... <pt_n_x>,<pt_n_y>` . For simple rectangular areas this can be expressed also with two points, with first point as top left and second point as bottom right: `<pt_top_left_x>,<pt_top_left_y> <pt_bottom_right_x>,<pt_bottom_right_y>`.
+
+The following example filters a rectangular area of 600x400 pixels of a page, which is described by an input ALTO file and saves the result to an output ALTO file
+
+```bash
+ocr-util frame -i page_1.alto.xml -p "0,0 600,0 600,400 0,400" -o page_1_area.alto.xml
+```
+
+Short version with top left and bottom right:
+
+```bash
+ocr-util frame -i page_1.alto.xml -p "0,0 600,400" -o page_1_area.alto.xml
+```
 
 ## Development
 
 Plattform: Intel(R) Core(TM) i5-6500 CPU@3.20GHz, 16GB RAM, Ubuntu 20.04 LTS, Python 3.8.
 
 ```bash
 # clone local
```

