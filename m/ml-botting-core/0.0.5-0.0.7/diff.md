# Comparing `tmp/ml_botting_core-0.0.5.tar.gz` & `tmp/ml_botting_core-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_botting_core-0.0.5.tar", last modified: Sun Apr 16 22:47:52 2023, max compression
+gzip compressed data, was "ml_botting_core-0.0.7.tar", last modified: Sun Apr 16 22:55:38 2023, max compression
```

## Comparing `ml_botting_core-0.0.5.tar` & `ml_botting_core-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 22:47:52.302261 ml_botting_core-0.0.5/
--rw-rw-rw-   0        0        0     1092 2023-04-16 15:23:47.000000 ml_botting_core-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      945 2023-04-16 22:47:52.302261 ml_botting_core-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-04-16 17:07:24.000000 ml_botting_core-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-04-16 15:28:39.000000 ml_botting_core-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      695 2023-04-16 22:47:52.302261 ml_botting_core-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 22:47:52.279685 ml_botting_core-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 22:47:52.286684 ml_botting_core-0.0.5/src/ml_botting_core/
--rw-rw-rw-   0        0        0        0 2023-04-16 15:26:05.000000 ml_botting_core-0.0.5/src/ml_botting_core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:47:52.290685 ml_botting_core-0.0.5/src/ml_botting_core/classification/
--rw-rw-rw-   0        0        0        0 2023-04-16 16:47:31.000000 ml_botting_core-0.0.5/src/ml_botting_core/classification/__init__.py
--rw-rw-rw-   0        0        0        2 2023-04-16 16:47:04.000000 ml_botting_core-0.0.5/src/ml_botting_core/classification/universal_classifier.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:47:52.292685 ml_botting_core-0.0.5/src/ml_botting_core/regression/
--rw-rw-rw-   0        0        0        0 2023-04-16 16:47:34.000000 ml_botting_core-0.0.5/src/ml_botting_core/regression/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-16 16:44:17.000000 ml_botting_core-0.0.5/src/ml_botting_core/regression/universal_regressor.py
--rw-rw-rw-   0        0        0      724 2023-04-16 17:26:44.000000 ml_botting_core-0.0.5/src/ml_botting_core/universal_predictor.py
-drwxrwxrwx   0        0        0        0 2023-04-16 22:47:52.289685 ml_botting_core-0.0.5/src/ml_botting_core.egg-info/
--rw-rw-rw-   0        0        0      945 2023-04-16 22:47:52.000000 ml_botting_core-0.0.5/src/ml_botting_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2023-04-16 22:47:52.000000 ml_botting_core-0.0.5/src/ml_botting_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 22:47:52.000000 ml_botting_core-0.0.5/src/ml_botting_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-16 22:47:52.000000 ml_botting_core-0.0.5/src/ml_botting_core.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 22:47:52.292685 ml_botting_core-0.0.5/tests/
--rw-rw-rw-   0        0        0       71 2023-04-16 22:34:37.000000 ml_botting_core-0.0.5/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.735451 ml_botting_core-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/classification/universal_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/regression/universal_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/src/ml_botting_core/universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 22:55:38.000000 ml_botting_core-0.0.7/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 22:55:38.739451 ml_botting_core-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-16 22:55:27.000000 ml_botting_core-0.0.7/tests/test_init.py
```

### Comparing `ml_botting_core-0.0.5/LICENSE` & `ml_botting_core-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ryan V. Susman
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Ryan V. Susman
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ml_botting_core-0.0.5/PKG-INFO` & `ml_botting_core-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: ml_botting_core
-Version: 0.0.5
-Summary: Making ML more accessible to botting apps
-Home-page: https://github.com/darkmatter2222/ml_botting_core
-Author: Ryan Susman
-Author-email: ryansusman@gmail.com
-Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ml-botting-core
-![](https://img.shields.io/pypi/v/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/github/actions/workflow/status/darkmatter2222/ml-botting-core/python-publish.yml?style=for-the-badge) ![](https://img.shields.io/pypi/l/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/pypi/pyversions/ml-botting-core?style=for-the-badge) 
-ml-botting-core
+Metadata-Version: 2.1
+Name: ml_botting_core
+Version: 0.0.7
+Summary: Making ML more accessible to botting apps
+Home-page: https://github.com/darkmatter2222/ml_botting_core
+Author: Ryan Susman
+Author-email: ryansusman@gmail.com
+Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ml-botting-core
+![](https://img.shields.io/pypi/v/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/github/actions/workflow/status/darkmatter2222/ml-botting-core/python-publish.yml?style=for-the-badge) ![](https://img.shields.io/pypi/l/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/pypi/pyversions/ml-botting-core?style=for-the-badge) 
+ml-botting-core
```

### Comparing `ml_botting_core-0.0.5/setup.cfg` & `ml_botting_core-0.0.7/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206d 6c5f 626f 7474 696e 675f 636f   = ml_botting_co
-00000020: 7265 0d0a 7665 7273 696f 6e20 3d20 302e  re..version = 0.
-00000030: 302e 350d 0a61 7574 686f 7220 3d20 5279  0.5..author = Ry
-00000040: 616e 2053 7573 6d61 6e0d 0a61 7574 686f  an Susman..autho
-00000050: 725f 656d 6169 6c20 3d20 7279 616e 7375  r_email = ryansu
-00000060: 736d 616e 4067 6d61 696c 2e63 6f6d 0d0a  sman@gmail.com..
-00000070: 6465 7363 7269 7074 696f 6e20 3d20 4d61  description = Ma
-00000080: 6b69 6e67 204d 4c20 6d6f 7265 2061 6363  king ML more acc
-00000090: 6573 7369 626c 6520 746f 2062 6f74 7469  essible to botti
-000000a0: 6e67 2061 7070 730d 0a6c 6f6e 675f 6465  ng apps..long_de
-000000b0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-000000c0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-000000d0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-000000e0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-000000f0: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
-00000100: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000110: 2e63 6f6d 2f64 6172 6b6d 6174 7465 7232  .com/darkmatter2
-00000120: 3232 322f 6d6c 5f62 6f74 7469 6e67 5f63  222/ml_botting_c
-00000130: 6f72 650d 0a70 726f 6a65 6374 5f75 726c  ore..project_url
-00000140: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000150: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-00000160: 6875 622e 636f 6d2f 6461 726b 6d61 7474  hub.com/darkmatt
-00000170: 6572 3232 3232 2f6d 6c5f 626f 7474 696e  er2222/ml_bottin
-00000180: 675f 636f 7265 2f69 7373 7565 730d 0a63  g_core/issues..c
-00000190: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001c0: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
-000001d0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000001e0: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-000001f0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000200: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000210: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000220: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000230: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
-00000240: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-00000250: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000260: 360d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  6....[options.pa
-00000270: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-00000280: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
-00000290: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000002a0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-000002b0: 3d20 300d 0a0d 0a                        = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6d6c 5f62 6f74 7469 6e67 5f63 6f72  = ml_botting_cor
+00000020: 650a 7665 7273 696f 6e20 3d20 302e 302e  e.version = 0.0.
+00000030: 370a 6175 7468 6f72 203d 2052 7961 6e20  7.author = Ryan 
+00000040: 5375 736d 616e 0a61 7574 686f 725f 656d  Susman.author_em
+00000050: 6169 6c20 3d20 7279 616e 7375 736d 616e  ail = ryansusman
+00000060: 4067 6d61 696c 2e63 6f6d 0a64 6573 6372  @gmail.com.descr
+00000070: 6970 7469 6f6e 203d 204d 616b 696e 6720  iption = Making 
+00000080: 4d4c 206d 6f72 6520 6163 6365 7373 6962  ML more accessib
+00000090: 6c65 2074 6f20 626f 7474 696e 6720 6170  le to botting ap
+000000a0: 7073 0a6c 6f6e 675f 6465 7363 7269 7074  ps.long_descript
+000000b0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000c0: 4d45 2e6d 640a 6c6f 6e67 5f64 6573 6372  ME.md.long_descr
+000000d0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+000000e0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+000000f0: 6f77 6e0a 7572 6c20 3d20 6874 7470 733a  own.url = https:
+00000100: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6172  //github.com/dar
+00000110: 6b6d 6174 7465 7232 3232 322f 6d6c 5f62  kmatter2222/ml_b
+00000120: 6f74 7469 6e67 5f63 6f72 650a 7072 6f6a  otting_core.proj
+00000130: 6563 745f 7572 6c73 203d 200a 0942 7567  ect_urls = ..Bug
+00000140: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+00000150: 3a2f 2f67 6974 6875 622e 636f 6d2f 6461  ://github.com/da
+00000160: 726b 6d61 7474 6572 3232 3232 2f6d 6c5f  rkmatter2222/ml_
+00000170: 626f 7474 696e 675f 636f 7265 2f69 7373  botting_core/iss
+00000180: 7565 730a 636c 6173 7369 6669 6572 7320  ues.classifiers 
+00000190: 3d20 0a09 5072 6f67 7261 6d6d 696e 6720  = ..Programming 
+000001a0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001b0: 6f6e 203a 3a20 330a 094c 6963 656e 7365  on :: 3..License
+000001c0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+000001d0: 203a 3a20 4d49 5420 4c69 6365 6e73 650a   :: MIT License.
+000001e0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000001f0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000200: 656e 740a 0a5b 6f70 7469 6f6e 735d 0a70  ent..[options].p
+00000210: 6163 6b61 6765 5f64 6972 203d 200a 093d  ackage_dir = ..=
+00000220: 2073 7263 0a70 6163 6b61 6765 7320 3d20   src.packages = 
+00000230: 6669 6e64 3a0a 7079 7468 6f6e 5f72 6571  find:.python_req
+00000240: 7569 7265 7320 3d20 3e3d 332e 360a 0a5b  uires = >=3.6..[
+00000250: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000260: 2e66 696e 645d 0a77 6865 7265 203d 2073  .find].where = s
+00000270: 7263 0a0a 5b65 6767 5f69 6e66 6f5d 0a74  rc..[egg_info].t
+00000280: 6167 5f62 7569 6c64 203d 200a 7461 675f  ag_build = .tag_
+00000290: 6461 7465 203d 2030 0a0a                 date = 0..
```

### Comparing `ml_botting_core-0.0.5/src/ml_botting_core/universal_predictor.py` & `ml_botting_core-0.0.7/src/ml_botting_core/universal_predictor.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-if 'logger' in locals() or 'logger' in globals():
-    from loguru import logger
-
-class universal_predictor:
-    def __new__(cls):  # make singleton
-        if not hasattr(cls, 'instance'):
-            cls.instance = super(universal_predictor, cls).__new__(cls)
-            cls.instance.__initialized = False
-        else:
-            logger.debug('universal_predictor returning existing')
-        return cls.instance
-
-    def __init__(self, logger):
-        if (self.__initialized): return  # make singleton
-        self.__initialized = True
-        logger.debug('universal_predictor initialized')
-        self.classifiers = {}
-        self.regressors = {}
-
-    def load_models(self):
-        return ''
+if 'logger' in locals() or 'logger' in globals():
+    from loguru import logger
+
+class universal_predictor:
+    def __new__(cls):  # make singleton
+        if not hasattr(cls, 'instance'):
+            cls.instance = super(universal_predictor, cls).__new__(cls)
+            cls.instance.__initialized = False
+        else:
+            logger.debug('universal_predictor returning existing')
+        return cls.instance
+
+    def __init__(self, logger):
+        if (self.__initialized): return  # make singleton
+        self.__initialized = True
+        logger.debug('universal_predictor initialized')
+        self.classifiers = {}
+        self.regressors = {}
+
+    def load_models(self):
+        return ''
```

### Comparing `ml_botting_core-0.0.5/src/ml_botting_core.egg-info/PKG-INFO` & `ml_botting_core-0.0.7/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: ml-botting-core
-Version: 0.0.5
-Summary: Making ML more accessible to botting apps
-Home-page: https://github.com/darkmatter2222/ml_botting_core
-Author: Ryan Susman
-Author-email: ryansusman@gmail.com
-Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ml-botting-core
-![](https://img.shields.io/pypi/v/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/github/actions/workflow/status/darkmatter2222/ml-botting-core/python-publish.yml?style=for-the-badge) ![](https://img.shields.io/pypi/l/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/pypi/pyversions/ml-botting-core?style=for-the-badge) 
-ml-botting-core
+Metadata-Version: 2.1
+Name: ml-botting-core
+Version: 0.0.7
+Summary: Making ML more accessible to botting apps
+Home-page: https://github.com/darkmatter2222/ml_botting_core
+Author: Ryan Susman
+Author-email: ryansusman@gmail.com
+Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml_botting_core/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ml-botting-core
+![](https://img.shields.io/pypi/v/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/github/actions/workflow/status/darkmatter2222/ml-botting-core/python-publish.yml?style=for-the-badge) ![](https://img.shields.io/pypi/l/ml-botting-core?style=for-the-badge) ![](https://img.shields.io/pypi/pyversions/ml-botting-core?style=for-the-badge) 
+ml-botting-core
```

