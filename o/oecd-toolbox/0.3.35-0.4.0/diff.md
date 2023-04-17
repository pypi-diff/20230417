# Comparing `tmp/oecd_toolbox-0.3.35.tar.gz` & `tmp/oecd_toolbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oecd_toolbox-0.3.35.tar", last modified: Wed Feb  1 21:40:23 2023, max compression
+gzip compressed data, was "oecd_toolbox-0.4.0.tar", last modified: Mon Apr 17 20:38:20 2023, max compression
```

## Comparing `oecd_toolbox-0.3.35.tar` & `oecd_toolbox-0.4.0.tar`

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
+drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.148713 oecd_toolbox-0.4.0/
+-rw-rw-rw-   0        0        0     1131 2021-12-03 19:53:43.000000 oecd_toolbox-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5783 2023-04-17 20:38:20.148713 oecd_toolbox-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5176 2023-04-17 20:28:40.000000 oecd_toolbox-0.4.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      856 2023-04-17 20:38:20.158070 oecd_toolbox-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.008434 oecd_toolbox-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.096961 oecd_toolbox-0.4.0/src/oecd_toolbox/
+-rw-rw-rw-   0        0        0        0 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/__init__.py
+-rw-rw-rw-   0        0        0     7046 2022-12-01 16:43:33.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/converters.py
+-rw-rw-rw-   0        0        0    13022 2023-04-17 20:35:35.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/csv_writers.py
+-rw-rw-rw-   0        0        0     5112 2022-02-04 15:48:18.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/downloaders.py
+drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.142523 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     5783 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/top_level.txt
```

### Comparing `oecd_toolbox-0.3.35/LICENSE` & `oecd_toolbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.3.35/PKG-INFO` & `oecd_toolbox-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: oecd_toolbox
-Version: 0.3.35
+Version: 0.4.0
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
 
@@ -73,14 +73,42 @@
 
 ``` powershell
 python datacapture-postprocessor.py <path-to\projectname-json-data> <path-to\projectname-datacapture-data> --force
 ```
 
 A similar command could be added to the postprocessor in the continouous integration pipeline. The usual behaviour modifiers [--only --except --limit] are available.
 
+NEW in version 0.4.0 beyond the basic converter two new converter flavours are available:
+- **DataCaptureConverterWithRegex** can filter series from a resource, so that the conversion is lighter both in used resources and resulting file (filtering is based on an SDMX webservice like syntax - dots for dimension separators, '+' to connect eligible dimension members, empty position allows all members) The above sample code adapted:
+    ```python
+    def main():
+        filterset = [
+            ('sts_trtu_m', '.TOVT+TOVV.G46+G47..I15.'),
+            ('prc_hicp_ctrb', '.I15+INX_A_AVG+RCH_A+RCH_A_AVG+RCH_M..CP00+CP01+CP02+CP03+CP04+CP041+CP043+CP044+CP045')
+        ]
+
+        cnvtr = lbc.DataCaptureConverterWithRegex()
+        cnvtr.init_arguments_and_logging()
+        asyncio.run(cnvtr.convert_resources(cnvtr.prepare_resources(filterset), cnvtr.process_single_resource))
+    ```
+
+- **DataCaptureConverterWithRegexAndAggregator** can handle frequency aggregations, it is sufficient to provide a target frequency from the list ['M','Q','A'] and an aggregator function (pandas-style) 
+
+    ```python
+    def main():
+        filterset = [
+            ("MMSD008A", None, "M", pd.DataFrame.mean),
+            ("MMSD402A", None, "A", pd.DataFrame.median)
+        ]
+
+        cnvtr = lbc.DataCaptureConverterWithRegexAndAggregator()
+        cnvtr.init_arguments_and_logging()
+        asyncio.run(cnvtr.convert_resources(cnvtr.prepare_resources(filterset), cnvtr.process_single_resource))
+    ```
+
 ## Common behaviour modifiers 
 
 All fetcher components that adopt the toolbox inherit some behaviour modifiers from the underlying toolbox. These command line arguments can be used to modify how the programs iterate through `resources`:
 
 - removing the excluded ones if the `--exclude` option is used; provide a space separated list of resource IDs
 - keeping only some of them if the `--only` option is used; provide a space separated list of resource IDs 
 - processing a limited number of resources if the `--limit` option is used; provide an integer after  the argument
```

### Comparing `oecd_toolbox-0.3.35/setup.cfg` & `oecd_toolbox-0.4.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6563 645f 746f 6f6c 626f 780d   = oecd_toolbox.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e33 2e33  .version = 0.3.3
-00000030: 350d 0a61 7574 686f 7220 3d20 4779 6f72  5..author = Gyor
-00000040: 6779 2047 796f 6d61 692c 2049 7361 6163  gy Gyomai, Isaac
-00000050: 2041 6661 6d62 6f0d 0a61 7574 686f 725f   Afambo..author_
-00000060: 656d 6169 6c20 3d20 6779 6f72 6779 2e67  email = gyorgy.g
-00000070: 796f 6d61 6940 6f65 6364 2e6f 7267 0d0a  yomai@oecd.org..
-00000080: 6465 7363 7269 7074 696f 6e20 3d20 4f45  description = OE
-00000090: 4344 2066 6574 6368 6572 2062 7569 6c64  CD fetcher build
-000000a0: 696e 6720 7465 6d70 6c61 7465 7320 616e  ing templates an
-000000b0: 6420 6865 6c70 6572 730d 0a6c 6f6e 675f  d helpers..long_
-000000c0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000d0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-000000e0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-000000f0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000100: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
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
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e30  .version = 0.4.0
+00000030: 0d0a 6175 7468 6f72 203d 2047 796f 7267  ..author = Gyorg
+00000040: 7920 4779 6f6d 6169 2c20 4973 6161 6320  y Gyomai, Isaac 
+00000050: 4166 616d 626f 0d0a 6175 7468 6f72 5f65  Afambo..author_e
+00000060: 6d61 696c 203d 2067 796f 7267 792e 6779  mail = gyorgy.gy
+00000070: 6f6d 6169 406f 6563 642e 6f72 670d 0a64  omai@oecd.org..d
+00000080: 6573 6372 6970 7469 6f6e 203d 204f 4543  escription = OEC
+00000090: 4420 6665 7463 6865 7220 6275 696c 6469  D fetcher buildi
+000000a0: 6e67 2074 656d 706c 6174 6573 2061 6e64  ng templates and
+000000b0: 2068 656c 7065 7273 0d0a 6c6f 6e67 5f64   helpers..long_d
+000000c0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+000000d0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
+000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000000f0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000100: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
+00000110: 203d 2068 7474 7073 3a2f 2f67 6974 6c61   = https://gitla
+00000120: 622e 616c 676f 6261 6e6b 2e6f 6563 642e  b.algobank.oecd.
+00000130: 6f72 672f 6f65 6364 2d64 6174 612d 6665  org/oecd-data-fe
+00000140: 7463 6865 7273 312f 4f45 4344 2d54 4f4f  tchers1/OECD-TOO
+00000150: 4c42 4f58 0d0a 7072 6f6a 6563 745f 7572  LBOX..project_ur
+00000160: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
+00000170: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000180: 746c 6162 2e61 6c67 6f62 616e 6b2e 6f65  tlab.algobank.oe
+00000190: 6364 2e6f 7267 2f6f 6563 642d 6461 7461  cd.org/oecd-data
+000001a0: 2d66 6574 6368 6572 7331 2f4f 4543 442d  -fetchers1/OECD-
+000001b0: 544f 4f4c 424f 582f 2d2f 6973 7375 6573  TOOLBOX/-/issues
+000001c0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
+000001d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000001f0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
+00000200: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000210: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
+00000220: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+00000230: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000240: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
+00000250: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
+00000260: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
+00000270: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+00000280: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000290: 3d33 2e37 0d0a 696e 7374 616c 6c5f 7265  =3.7..install_re
+000002a0: 7175 6972 6573 203d 200d 0a09 6462 6e6f  quires = ...dbno
+000002b0: 6d69 6373 2d66 6574 6368 6572 2d74 6f6f  mics-fetcher-too
+000002c0: 6c62 6f78 3d3d 302e 302e 390d 0a09 6462  lbox==0.0.9...db
+000002d0: 6e6f 6d69 6373 2d64 6174 612d 6d6f 6465  nomics-data-mode
+000002e0: 6c3d 3d30 2e31 332e 3230 0d0a 0970 7974  l==0.13.20...pyt
+000002f0: 686f 6e2d 736c 7567 6966 793e 3d35 2e30  hon-slugify>=5.0
+00000300: 2e32 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .2....[options.p
+00000310: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000320: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+00000330: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000340: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000350: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox/converters.py` & `oecd_toolbox-0.4.0/src/oecd_toolbox/converters.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox/csv_writers.py` & `oecd_toolbox-0.4.0/src/oecd_toolbox/csv_writers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,138 @@
 import csv
 import ujson as json
-import warnings
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
+    targetFreq: Union[Literal["M", "Q", "A"], None] = None  # (DataCapture target frequencies M|Q|A)
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
-        #print('Create an iterator of resources - can be a similar function outside of a subclass')
+        # print('Create an iterator of resources - can be a similar function outside of a subclass')
         
         for f in self.source_dir.rglob('series.jsonl'):
             dirPath = f.parents[0]
             fileName = f.name
             relDirPath = dirPath.relative_to(self.source_dir)
             did = slugify(str(relDirPath))
-            yield FileResource(id=did, sourceFolder = dirPath, targetDataset = self.target_dir / relDirPath, fileToProcess = fileName)
+            yield FileResource(id=did, sourceFolder=dirPath, targetDataset=self.target_dir / relDirPath, fileToProcess=fileName)
             
-
     def process_single_resource(self, res: Resource):
         if not res.targetDataset.exists():
             res.targetDataset.mkdir(parents=True)
         series_jsonl_to_DataCapturecsv(res.sourceFolder / res.fileToProcess, Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'))
 
 
 class DataCaptureConverterWithRegex(SimpleConverter):
     ''' A converter to create DataCapture ready files from DbNomics jsonl files for an entire project.
         params should be provided as a list of tuples to prepare_resources (datasetID, regexFilter on codes)
     '''
     
     def prepare_resources(self, params: list) -> Iterator[Resource]:
-        #print('Create an iterator of resources - can be a similar function outside of a subclass')
+        # print('Create an iterator of resources - can be a similar function outside of a subclass')
         
         for dirPath, filter in params:
             did = slugify(str(dirPath))
-            yield FileResource(id=did, sourceFolder = self.source_dir / dirPath, targetDataset = self.target_dir / dirPath, fileToProcess = 'series.jsonl', query=filter)
+            yield FileResource(
+                id=did,
+                sourceFolder=self.source_dir / dirPath,
+                targetDataset=self.target_dir / dirPath,
+                fileToProcess='series.jsonl',
+                query=filter
+            )
 
     def process_single_resource(self, res: Resource):
         if not res.targetDataset.exists():
             res.targetDataset.mkdir(parents=True)
-        series_jsonl_to_DataCapturecsv(res.sourceFolder / res.fileToProcess, Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'), get_pattern_from_query(res.query))
+        series_jsonl_to_DataCapturecsv(
+            res.sourceFolder / res.fileToProcess,
+            Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'),
+            get_pattern_from_query(res.query)
+        )
 
 
-def dataset_json_to_csv(source_dir : Path):
-    """Convert dataset.json into a csv file"""
-    warnings.warn("Dataset.json to csv conversion is deprecated. Use the json file directly to access structural information.", warnings.DeprecationWarning)    
+class DataCaptureConverterWithRegexAndAggregator(SimpleConverter):
+    ''' A converter to create DataCapture ready files from DbNomics jsonl files for an entire project.
+        params should be provided as a list of tuples to prepare_resources (datasetID, regexFilter on codes, target frequency, aggregator function)
+    '''
+    
+    def prepare_resources(self, params: list) -> Iterator[Resource]:
+        # print('Create an iterator of resources - can be a similar function outside of a subclass')
+        
+        for dirPath, filter, freq, func in params:
+            did = slugify(str(dirPath))
+            yield FileResource(
+                id=did,
+                sourceFolder=self.source_dir / dirPath,
+                targetDataset=self.target_dir / dirPath,
+                fileToProcess='series.jsonl',
+                query=filter,
+                targetFreq=freq,
+                fAggregator=func
+            )
 
+    def process_single_resource(self, res: Resource):
+        if not res.targetDataset.exists():
+            res.targetDataset.mkdir(parents=True)
+        series_jsonl_to_DataCapturecsv(
+            res.sourceFolder / res.fileToProcess,
+            Path(res.targetDataset / res.fileToProcess).with_suffix('.csv'),
+            get_pattern_from_query(res.query),
+            get_frequency_from_query(res.targetFreq),
+            res.fAggregator
+        )
 
 #----------------------series_jsonl conversions----------------------
 def series_jsonl_to_csv_base(source_file: Path, target_file: Path, obslist_fn: Callable[[List], None]):
     """ Convert series.jsonl into a csv file. 
     Base function.
     Needs to be called by a function that provides the fields and methods to convert to.
     """
 
     json_file = []
     for line in open(source_file, 'r', encoding="UTF-8"):
         json_file.append(json.loads(line))
     
+    obslist = obslist_fn(json_file)
+    if not obslist:
+        logger.debug('empty observations list, most likely none of the series matched')
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
@@ -109,15 +150,15 @@
         for v in takefirst['observations'][0][1:]:
             fieldnames.append(v)
         L.append({v:v for v in fieldnames}) 
 
         # append data rows
         for series in json_file:
             for obs in series['observations'][1:]:
-                dim_dict=dict()
+                dim_dict = dict()
                 dim_dict['code'] = series['code']
                 dim_dict['PERIOD'] =  obs[0]
                 for c, v in enumerate(series['observations'][0][1:]):
                         dim_dict[v] = obs[c+1]
 
                 L.append(dim_dict)
         return L 
@@ -125,26 +166,24 @@
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
@@ -153,25 +192,41 @@
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
@@ -201,24 +256,62 @@
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
+    
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
     
-def get_pattern_from_query(query: str) -> re.Pattern:
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

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox/downloaders.py` & `oecd_toolbox-0.4.0/src/oecd_toolbox/downloaders.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.3.35/src/oecd_toolbox.egg-info/PKG-INFO` & `oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: oecd-toolbox
-Version: 0.3.35
+Version: 0.4.0
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
 
@@ -73,14 +73,42 @@
 
 ``` powershell
 python datacapture-postprocessor.py <path-to\projectname-json-data> <path-to\projectname-datacapture-data> --force
 ```
 
 A similar command could be added to the postprocessor in the continouous integration pipeline. The usual behaviour modifiers [--only --except --limit] are available.
 
+NEW in version 0.4.0 beyond the basic converter two new converter flavours are available:
+- **DataCaptureConverterWithRegex** can filter series from a resource, so that the conversion is lighter both in used resources and resulting file (filtering is based on an SDMX webservice like syntax - dots for dimension separators, '+' to connect eligible dimension members, empty position allows all members) The above sample code adapted:
+    ```python
+    def main():
+        filterset = [
+            ('sts_trtu_m', '.TOVT+TOVV.G46+G47..I15.'),
+            ('prc_hicp_ctrb', '.I15+INX_A_AVG+RCH_A+RCH_A_AVG+RCH_M..CP00+CP01+CP02+CP03+CP04+CP041+CP043+CP044+CP045')
+        ]
+
+        cnvtr = lbc.DataCaptureConverterWithRegex()
+        cnvtr.init_arguments_and_logging()
+        asyncio.run(cnvtr.convert_resources(cnvtr.prepare_resources(filterset), cnvtr.process_single_resource))
+    ```
+
+- **DataCaptureConverterWithRegexAndAggregator** can handle frequency aggregations, it is sufficient to provide a target frequency from the list ['M','Q','A'] and an aggregator function (pandas-style) 
+
+    ```python
+    def main():
+        filterset = [
+            ("MMSD008A", None, "M", pd.DataFrame.mean),
+            ("MMSD402A", None, "A", pd.DataFrame.median)
+        ]
+
+        cnvtr = lbc.DataCaptureConverterWithRegexAndAggregator()
+        cnvtr.init_arguments_and_logging()
+        asyncio.run(cnvtr.convert_resources(cnvtr.prepare_resources(filterset), cnvtr.process_single_resource))
+    ```
+
 ## Common behaviour modifiers 
 
 All fetcher components that adopt the toolbox inherit some behaviour modifiers from the underlying toolbox. These command line arguments can be used to modify how the programs iterate through `resources`:
 
 - removing the excluded ones if the `--exclude` option is used; provide a space separated list of resource IDs
 - keeping only some of them if the `--only` option is used; provide a space separated list of resource IDs 
 - processing a limited number of resources if the `--limit` option is used; provide an integer after  the argument
```

