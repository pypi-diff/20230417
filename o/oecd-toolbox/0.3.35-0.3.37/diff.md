# Comparing `tmp/oecd_toolbox-0.3.35.tar.gz` & `tmp/oecd_toolbox-0.3.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oecd_toolbox-0.3.35.tar", last modified: Wed Feb  1 21:40:23 2023, max compression
+gzip compressed data, was "oecd_toolbox-0.3.37.tar", last modified: Mon Apr 17 18:29:11 2023, max compression
```

## Comparing `oecd_toolbox-0.3.35.tar` & `oecd_toolbox-0.3.37.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 21:40:23.338389 oecd_toolbox-0.3.35/
--rw-rw-rw-   0        0        0     1131 2021-12-03 19:53:43.000000 oecd_toolbox-0.3.35/LICENSE
--rw-rw-rw-   0        0        0     4256 2023-02-01 21:40:23.338389 oecd_toolbox-0.3.35/PKG-INFO
--rw-rw-rw-   0        0        0     3652 2021-12-14 19:05:53.000000 oecd_toolbox-0.3.35/README.md
--rw-rw-rw-   0        0        0      108 2021-12-03 19:53:44.000000 oecd_toolbox-0.3.35/pyproject.toml
--rw-rw-rw-   0        0        0      853 2023-02-01 21:40:23.346326 oecd_toolbox-0.3.35/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-01 21:40:23.184855 oecd_toolbox-0.3.35/src/
-drwxrwxrwx   0        0        0        0 2023-02-01 21:40:23.285127 oecd_toolbox-0.3.35/src/oecd_toolbox/
--rw-rw-rw-   0        0        0        0 2021-12-03 19:53:44.000000 oecd_toolbox-0.3.35/src/oecd_toolbox/__init__.py
--rw-rw-rw-   0        0        0     7046 2022-12-01 16:43:33.000000 oecd_toolbox-0.3.35/src/oecd_toolbox/converters.py
--rw-rw-rw-   0        0        0     9058 2023-02-01 21:37:26.000000 oecd_toolbox-0.3.35/src/oecd_toolbox/csv_writers.py
--rw-rw-rw-   0        0        0     5112 2022-02-04 15:48:18.000000 oecd_toolbox-0.3.35/src/oecd_toolbox/downloaders.py
-drwxrwxrwx   0        0        0        0 2023-02-01 21:40:23.330890 oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/
--rw-rw-rw-   0        0        0     4256 2023-02-01 21:40:23.000000 oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-02-01 21:40:23.000000 oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 21:40:23.000000 oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-02-01 21:40:23.000000 oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-01 21:40:23.000000 oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 18:29:11.548172 oecd_toolbox-0.3.37/
+-rw-rw-rw-   0        0        0     1131 2021-12-03 19:53:43.000000 oecd_toolbox-0.3.37/LICENSE
+-rw-rw-rw-   0        0        0     4260 2023-04-17 18:29:11.548172 oecd_toolbox-0.3.37/PKG-INFO
+-rw-rw-rw-   0        0        0     3652 2021-12-14 19:05:53.000000 oecd_toolbox-0.3.37/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-03 19:53:44.000000 oecd_toolbox-0.3.37/pyproject.toml
+-rw-rw-rw-   0        0        0      857 2023-04-17 18:29:11.556378 oecd_toolbox-0.3.37/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 18:29:11.425751 oecd_toolbox-0.3.37/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 18:29:11.494809 oecd_toolbox-0.3.37/src/oecd_toolbox/
+-rw-rw-rw-   0        0        0        0 2021-12-03 19:53:44.000000 oecd_toolbox-0.3.37/src/oecd_toolbox/__init__.py
+-rw-rw-rw-   0        0        0     7046 2022-12-01 16:43:33.000000 oecd_toolbox-0.3.37/src/oecd_toolbox/converters.py
+-rw-rw-rw-   0        0        0    13066 2023-04-17 18:28:06.000000 oecd_toolbox-0.3.37/src/oecd_toolbox/csv_writers.py
+-rw-rw-rw-   0        0        0     5112 2022-02-04 15:48:18.000000 oecd_toolbox-0.3.37/src/oecd_toolbox/downloaders.py
+drwxrwxrwx   0        0        0        0 2023-04-17 18:29:11.541270 oecd_toolbox-0.3.37/src/oecd_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     4260 2023-04-17 18:29:11.000000 oecd_toolbox-0.3.37/src/oecd_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-17 18:29:11.000000 oecd_toolbox-0.3.37/src/oecd_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 18:29:11.000000 oecd_toolbox-0.3.37/src/oecd_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-04-17 18:29:11.000000 oecd_toolbox-0.3.37/src/oecd_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 18:29:11.000000 oecd_toolbox-0.3.37/src/oecd_toolbox.egg-info/top_level.txt
```

### Comparing `oecd_toolbox-0.3.35/LICENSE` & `oecd_toolbox-0.3.37/LICENSE`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.3.35/PKG-INFO` & `oecd_toolbox-0.3.37/src/oecd_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: oecd_toolbox
-Version: 0.3.35
+Name: oecd-toolbox
+Version: 0.3.37
 Summary: OECD fetcher building templates and helpers
-Home-page: https://algobank.oecd.org:4430/oecd-data-fetchers1/OECD-TOOLBOX
+Home-page: https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX
 Author: Gyorgy Gyomai, Isaac Afambo
 Author-email: gyorgy.gyomai@oecd.org
-Project-URL: Bug Tracker, https://algobank.oecd.org:4430/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
+Project-URL: Bug Tracker, https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oecd_toolbox-0.3.35/README.md` & `oecd_toolbox-0.3.37/README.md`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.3.35/setup.cfg` & `oecd_toolbox-0.3.37/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6563 645f 746f 6f6c 626f 780d   = oecd_toolbox.
 00000020: 0a76 6572 7369 6f6e 203d 2030 2e33 2e33  .version = 0.3.3
-00000030: 350d 0a61 7574 686f 7220 3d20 4779 6f72  5..author = Gyor
+00000030: 370d 0a61 7574 686f 7220 3d20 4779 6f72  7..author = Gyor
 00000040: 6779 2047 796f 6d61 692c 2049 7361 6163  gy Gyomai, Isaac
 00000050: 2041 6661 6d62 6f0d 0a61 7574 686f 725f   Afambo..author_
 00000060: 656d 6169 6c20 3d20 6779 6f72 6779 2e67  email = gyorgy.g
 00000070: 796f 6d61 6940 6f65 6364 2e6f 7267 0d0a  yomai@oecd.org..
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 4f45  description = OE
 00000090: 4344 2066 6574 6368 6572 2062 7569 6c64  CD fetcher build
 000000a0: 696e 6720 7465 6d70 6c61 7465 7320 616e  ing templates an
 000000b0: 6420 6865 6c70 6572 730d 0a6c 6f6e 675f  d helpers..long_
 000000c0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 000000d0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 000000e0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000f0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 00000100: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
-00000110: 6c20 3d20 6874 7470 733a 2f2f 616c 676f  l = https://algo
-00000120: 6261 6e6b 2e6f 6563 642e 6f72 673a 3434  bank.oecd.org:44
-00000130: 3330 2f6f 6563 642d 6461 7461 2d66 6574  30/oecd-data-fet
-00000140: 6368 6572 7331 2f4f 4543 442d 544f 4f4c  chers1/OECD-TOOL
-00000150: 424f 580d 0a70 726f 6a65 6374 5f75 726c  BOX..project_url
-00000160: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000170: 6572 203d 2068 7474 7073 3a2f 2f61 6c67  er = https://alg
-00000180: 6f62 616e 6b2e 6f65 6364 2e6f 7267 3a34  obank.oecd.org:4
-00000190: 3433 302f 6f65 6364 2d64 6174 612d 6665  430/oecd-data-fe
-000001a0: 7463 6865 7273 312f 4f45 4344 2d54 4f4f  tchers1/OECD-TOO
-000001b0: 4c42 4f58 2f2d 2f69 7373 7565 730d 0a63  LBOX/-/issues..c
-000001c0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-000001d0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001e0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001f0: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
-00000200: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000210: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-00000220: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000230: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000240: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000250: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000260: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
-00000270: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-00000280: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000290: 370d 0a69 6e73 7461 6c6c 5f72 6571 7569  7..install_requi
-000002a0: 7265 7320 3d20 0d0a 0964 626e 6f6d 6963  res = ...dbnomic
-000002b0: 732d 6665 7463 6865 722d 746f 6f6c 626f  s-fetcher-toolbo
-000002c0: 783d 3d30 2e30 2e39 0d0a 0964 626e 6f6d  x==0.0.9...dbnom
-000002d0: 6963 732d 6461 7461 2d6d 6f64 656c 3d3d  ics-data-model==
-000002e0: 302e 3133 2e32 300d 0a09 7079 7468 6f6e  0.13.20...python
-000002f0: 2d73 6c75 6769 6679 3e3d 352e 302e 320d  -slugify>=5.0.2.
-00000300: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-00000310: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-00000320: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
-00000330: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000340: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000350: 300d 0a0d 0a                             0....
+00000110: 6c20 3d20 6874 7470 733a 2f2f 6769 746c  l = https://gitl
+00000120: 6162 2e61 6c67 6f62 616e 6b2e 6f65 6364  ab.algobank.oecd
+00000130: 2e6f 7267 2f6f 6563 642d 6461 7461 2d66  .org/oecd-data-f
+00000140: 6574 6368 6572 7331 2f4f 4543 442d 544f  etchers1/OECD-TO
+00000150: 4f4c 424f 580d 0a70 726f 6a65 6374 5f75  OLBOX..project_u
+00000160: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
+00000170: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+00000180: 6974 6c61 622e 616c 676f 6261 6e6b 2e6f  itlab.algobank.o
+00000190: 6563 642e 6f72 672f 6f65 6364 2d64 6174  ecd.org/oecd-dat
+000001a0: 612d 6665 7463 6865 7273 312f 4f45 4344  a-fetchers1/OECD
+000001b0: 2d54 4f4f 4c42 4f58 2f2d 2f69 7373 7565  -TOOLBOX/-/issue
+000001c0: 730d 0a63 6c61 7373 6966 6965 7273 203d  s..classifiers =
+000001d0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+000001e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001f0: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
+00000200: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000210: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000220: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000230: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000240: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+00000250: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000260: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000270: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000280: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000290: 3e3d 332e 370d 0a69 6e73 7461 6c6c 5f72  >=3.7..install_r
+000002a0: 6571 7569 7265 7320 3d20 0d0a 0964 626e  equires = ...dbn
+000002b0: 6f6d 6963 732d 6665 7463 6865 722d 746f  omics-fetcher-to
+000002c0: 6f6c 626f 783d 3d30 2e30 2e39 0d0a 0964  olbox==0.0.9...d
+000002d0: 626e 6f6d 6963 732d 6461 7461 2d6d 6f64  bnomics-data-mod
+000002e0: 656c 3d3d 302e 3133 2e32 300d 0a09 7079  el==0.13.20...py
+000002f0: 7468 6f6e 2d73 6c75 6769 6679 3e3d 352e  thon-slugify>=5.
+00000300: 302e 320d 0a0d 0a5b 6f70 7469 6f6e 732e  0.2....[options.
+00000310: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000320: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000330: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000340: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000350: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox/converters.py` & `oecd_toolbox-0.3.37/src/oecd_toolbox/converters.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox/csv_writers.py` & `oecd_toolbox-0.3.37/src/oecd_toolbox/csv_writers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 import csv
 import ujson as json
 import warnings
 from pathlib import Path
-from typing import Callable, List, Optional, Tuple, Iterator, Union
+from typing import Any, Callable, Iterable, List, Literal, Optional, Tuple, Iterator, Union
 from dbnomics_data_model.observations import Frequency, detect_period_format_strict, period_format_strict_regex_list
 from oecd_toolbox.converters import SimpleConverter
-from dbnomics_fetcher_toolbox.resources import Resource 
+from dbnomics_fetcher_toolbox.resources import Resource
 from slugify import slugify
 import re
 import daiquiri
+import pandas as pd
 
 logger = daiquiri.getLogger(__name__)
 
 
 class FileResource(Resource):
     """ A resource-type consisting of a single downloadable file, identified by a URL
     and a target path where it should be deposited.
     """
     targetDataset: Path
     sourceFolder: Path
     fileToProcess: str
-    query: Union[str, None] = None # '.TOVT+TOVV.G46+G47..I15.'
-    
-
+    query: Union[str, None] = None  # '.TOVT+TOVV.G46+G47..I15.'
+    targetFreq: Union[Literal["M","Q","A"], None] = None  # (DataCapture target frequencies M|Q|A)
+    fAggregator: Union[Callable[[Iterable], Any], None] = None  # e.g. pd.DataFrame.mean
+  
     def delete(self):
         """ Deletes the local representation of a dataset including its containing folder. """
         for f in self.targetDataset.glob('*.*'):
             f.unlink()
         self.targetDataset.rmdir
     
     def __str__(self) -> str:
         return f'target ds: {self.targetDataset}, source fold: {self.sourceFolder}, file: {self.fileToProcess}, filter: {self.query}'
 
+
 class DataCaptureConverter(SimpleConverter):
     ''' A converter to create DataCapture ready files from DbNomics jsonl files for an entire project.'''
     def prepare_resources(self) -> Iterator[Resource]:
         #print('Create an iterator of resources - can be a similar function outside of a subclass')
         
         for f in self.source_dir.rglob('series.jsonl'):
             dirPath = f.parents[0]
             fileName = f.name
             relDirPath = dirPath.relative_to(self.source_dir)
             did = slugify(str(relDirPath))
-            yield FileResource(id=did, sourceFolder = dirPath, targetDataset = self.target_dir / relDirPath, fileToProcess = fileName)
+            yield FileResource(id=did, sourceFolder= dirPath, targetDataset= self.target_dir / relDirPath, fileToProcess=fileName)
             
 
     def process_single_resource(self, res: Resource):
         if not res.targetDataset.exists():
             res.targetDataset.mkdir(parents=True)
         series_jsonl_to_DataCapturecsv(res.sourceFolder / res.fileToProcess, Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'))
 
@@ -57,20 +60,47 @@
     '''
     
     def prepare_resources(self, params: list) -> Iterator[Resource]:
         #print('Create an iterator of resources - can be a similar function outside of a subclass')
         
         for dirPath, filter in params:
             did = slugify(str(dirPath))
-            yield FileResource(id=did, sourceFolder = self.source_dir / dirPath, targetDataset = self.target_dir / dirPath, fileToProcess = 'series.jsonl', query=filter)
+            yield FileResource(id=did, sourceFolder= self.source_dir / dirPath, targetDataset= self.target_dir / dirPath, fileToProcess='series.jsonl', query=filter)
+
+    def process_single_resource(self, res: Resource):
+        if not res.targetDataset.exists():
+            res.targetDataset.mkdir(parents=True)
+        series_jsonl_to_DataCapturecsv(
+            res.sourceFolder / res.fileToProcess,
+            Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'),
+            get_pattern_from_query(res.query)
+        )
+
+class DataCaptureConverterWithRegexAndAggregator(SimpleConverter):
+    ''' A converter to create DataCapture ready files from DbNomics jsonl files for an entire project.
+        params should be provided as a list of tuples to prepare_resources (datasetID, regexFilter on codes, target frequency, aggregator function)
+    '''
+    
+    def prepare_resources(self, params: list) -> Iterator[Resource]:
+        #print('Create an iterator of resources - can be a similar function outside of a subclass')
+        
+        for dirPath, filter, freq, func in params:
+            did = slugify(str(dirPath))
+            yield FileResource(id=did, sourceFolder= self.source_dir / dirPath, targetDataset= self.target_dir / dirPath, fileToProcess='series.jsonl', query=filter, targetFreq=freq, fAggregator=func)
 
     def process_single_resource(self, res: Resource):
         if not res.targetDataset.exists():
             res.targetDataset.mkdir(parents=True)
-        series_jsonl_to_DataCapturecsv(res.sourceFolder / res.fileToProcess, Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'), get_pattern_from_query(res.query))
+        series_jsonl_to_DataCapturecsv(
+            res.sourceFolder / res.fileToProcess,
+            Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'),
+            get_pattern_from_query(res.query),
+            get_frequency_from_query(res.targetFreq),
+            res.fAggregator
+        )
 
 
 def dataset_json_to_csv(source_dir : Path):
     """Convert dataset.json into a csv file"""
     warnings.warn("Dataset.json to csv conversion is deprecated. Use the json file directly to access structural information.", warnings.DeprecationWarning)    
 
 
@@ -81,17 +111,21 @@
     Needs to be called by a function that provides the fields and methods to convert to.
     """
 
     json_file = []
     for line in open(source_file, 'r', encoding="UTF-8"):
         json_file.append(json.loads(line))
     
+    obslist = obslist_fn(json_file)
+    if not obslist:
+        logger.debug(f'empty observations list, most likely none of the series matched')
+        return None
+    
     def create_csv_file(tf: Path):
-        with open(tf, 'w', encoding="UTF-8", newline='') as csvfile:
-            obslist = obslist_fn(json_file)
+        with open(tf, 'w', encoding="UTF-8", newline='') as csvfile:   
             fieldnames = list(obslist[0].keys())
             writer = csv.DictWriter(f=csvfile, fieldnames=fieldnames, extrasaction='ignore')
             writer.writeheader()
             for data in obslist[1:]:
                 writer.writerow(data)
     
     create_csv_file(target_file)
@@ -125,26 +159,24 @@
     series_jsonl_to_csv_base(source_file=source_file, target_file='series.csv',  obslist_fn=create_observations_list)       
 
 
 DC_eligible_frequencies = [Frequency.ANNUAL, Frequency.QUARTERLY, Frequency.MONTHLY, Frequency.BI_ANNUAL]
 DC_eligible_frequency_codes = [f.to_dimension_code() for f in DC_eligible_frequencies]
 
 
-def series_jsonl_to_DataCapturecsv(source_file: Path, target_file: Path, regex: Union[re.Pattern, None] = None):
+def series_jsonl_to_DataCapturecsv(source_file: Path, target_file: Path, regex: Union[re.Pattern, None] = None, target_freq: Union[Frequency, None] = None, f_aggregation: Union[Callable[[Iterable], Any], None] = None):
     """ DataCapture csv flavour of the convertor. """
     
     def create_DCobservations_list(json_file: List) -> List:
         L=[]
 
         # construct header row
         takefirst = json_file[0]
         fieldnames = ['code', 'year', 'freq', 'period']
-        for v in takefirst['observations'][0][1:]:
-            fieldnames.append(v)
-        L.append({v:v for v in fieldnames})    
+           
 
         # append data rows
         sm = None 
         for series in json_file:
             if regex:
                 sm = regex.match(series['code'])
                 if not sm: 
@@ -153,25 +185,41 @@
             if sm or not regex:        
                 if isinstance(series['dimensions'], list):
                     series_freq = series['dimensions'][0]
                 elif isinstance(series['dimensions'], dict):
                     series_freq = series['dimensions']['FREQ']
 
                 if series_freq in DC_eligible_frequency_codes:
+                    for v in takefirst['observations'][0][1:]:
+                        fieldnames.append(v)
+                    L.append({v:v for v in fieldnames}) 
                     for obs in series['observations'][1:]:
                         dim_dict=dict()
                         dim_dict['code'] = series['code']
                         dim_dict['year'], dim_dict['freq'], dim_dict['period'] = get_DC_compatible_date(obs[0])
                         for c, v in enumerate(series['observations'][0][1:]):
                             dim_dict[v] = obs[c+1]
 
                         L.append(dim_dict)
+                        
+                elif target_freq and f_aggregation and (target_freq in DC_eligible_frequencies):
+                    fieldnames.append('value')
+                    L.append({v:v for v in fieldnames}) 
+                    df = pd.DataFrame(data=series["observations"][1:],columns=series["observations"][0]) 
+                    # this only aggregates values, but omits observation attributes that might be in the original file                   
+                    df_new_freq = df.groupby(pd.PeriodIndex(df['PERIOD'], freq=target_freq.to_dimension_code()))['VALUE'].apply(f_aggregation)
+                    for ind in df_new_freq.index:
+                        dim_dict=dict()
+                        dim_dict['code'] = series['code']
+                        dim_dict['year'], dim_dict['freq'], dim_dict['period'] = get_DC_compatible_date_pandas(ind)
+                        dim_dict['value'] = df_new_freq[ind]
+
+                        L.append(dim_dict)
                     
         return L 
-
     
     series_jsonl_to_csv_base(source_file=source_file, target_file=target_file, obslist_fn=create_DCobservations_list)
 
 
   
 
 def get_DC_compatible_date(period: str) -> Optional[Tuple[int, str, int]]:
@@ -201,24 +249,62 @@
                     return int(m.group(1)), "Y", 1
                 elif freq == Frequency.BI_ANNUAL:
                     return int(m.group(1)), "Q", int(m.group(2)) * 2
                 else:
                     return int(m.group(1)), freq.to_dimension_code(), int(m.group(2))
     return None
 
+def get_DC_compatible_date_pandas(period: pd.Period) -> Optional[Tuple[int, str, int]]:
+    """Return a tuple of (year, frequency_code, period_withinyear) or `None` if unable to detect.
+
+    # Working examples:
+    >>> get_DC_compatible_date("2014")
+    2014, Y, 1 
+    >>> get_DC_compatible_date("2014-Q1")
+    2014, Q, 1 
+    >>> get_DC_compatible_date("2014-01")
+    2014, M, 1
+
+    # Invalid formats:
+    >>> detect_period_format_strict("ABCDE")
+    >>> detect_period_format_strict("2014Z01")
+    """
     
-def get_pattern_from_query(query: str) -> re.Pattern:
+    freq = period.freqstr[0]
+    if freq in DC_eligible_frequency_codes:
+        if freq == 'A':
+            return period.year, 'Y', 1
+        elif freq == 'Q':
+            return period.year, 'Q', period.quarter
+        else:
+            return period.year, 'M', period.month
+    return None
+
+    
+def get_pattern_from_query(query: Union[str, None]) -> re.Pattern:
     """ Working example: 
     >>> get_pattern_from_query('.TOVT+TOVV.G46+G47..I15.')
     ^.+\.(TOVT|TOVV)\.(G46|G47)\..+\.(I15)\..+$
     """ 
+    if not query:
+        return re.compile(r'.*') 
     
     seq = query.split('.')
     reseq = []
     for s in seq:
         if s == '':
             reseq.append(r'.+')
         else:
             plus_to_or = '(' + s.replace('+','|') + ')'
             reseq.append(plus_to_or)
 
-    return re.compile(r'^'+r'\.'.join(reseq)+r'$')            
+    return re.compile(r'^'+r'\.'.join(reseq)+r'$')
+
+def get_frequency_from_query(freq: Union[Literal["M","Q","A"], None]) -> Frequency:
+    if freq == 'M':
+        return Frequency.MONTHLY
+    elif freq == 'Q':
+        return Frequency.QUARTERLY
+    elif freq == 'A':
+        return Frequency.ANNUAL
+    else:
+        return None
```

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox/downloaders.py` & `oecd_toolbox-0.3.37/src/oecd_toolbox/downloaders.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/PKG-INFO` & `oecd_toolbox-0.3.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: oecd-toolbox
-Version: 0.3.35
+Name: oecd_toolbox
+Version: 0.3.37
 Summary: OECD fetcher building templates and helpers
-Home-page: https://algobank.oecd.org:4430/oecd-data-fetchers1/OECD-TOOLBOX
+Home-page: https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX
 Author: Gyorgy Gyomai, Isaac Afambo
 Author-email: gyorgy.gyomai@oecd.org
-Project-URL: Bug Tracker, https://algobank.oecd.org:4430/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
+Project-URL: Bug Tracker, https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

