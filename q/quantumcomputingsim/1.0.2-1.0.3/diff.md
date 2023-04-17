# Comparing `tmp/quantumcomputingsim-1.0.2.tar.gz` & `tmp/quantumcomputingsim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumcomputingsim-1.0.2.tar", last modified: Mon Apr 17 20:49:19 2023, max compression
+gzip compressed data, was "quantumcomputingsim-1.0.3.tar", last modified: Mon Apr 17 21:03:34 2023, max compression
```

## Comparing `quantumcomputingsim-1.0.2.tar` & `quantumcomputingsim-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:49:19.533093 quantumcomputingsim-1.0.2/
--rw-rw-rw-   0        0        0     4320 2023-04-17 20:49:19.534148 quantumcomputingsim-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-04-17 20:39:03.000000 quantumcomputingsim-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-17 20:49:19.529415 quantumcomputingsim-1.0.2/quantumcomputingsim.egg-info/
--rw-rw-rw-   0        0        0     4320 2023-04-17 20:49:19.000000 quantumcomputingsim-1.0.2/quantumcomputingsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-17 20:49:19.000000 quantumcomputingsim-1.0.2/quantumcomputingsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:49:19.000000 quantumcomputingsim-1.0.2/quantumcomputingsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:49:19.000000 quantumcomputingsim-1.0.2/quantumcomputingsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      704 2023-04-17 20:49:19.540052 quantumcomputingsim-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.841882 quantumcomputingsim-1.0.3/
+-rw-rw-rw-   0        0        0     4320 2023-04-17 21:03:34.842887 quantumcomputingsim-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-17 20:39:03.000000 quantumcomputingsim-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      708 2023-04-17 21:03:34.846413 quantumcomputingsim-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.769178 quantumcomputingsim-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.791263 quantumcomputingsim-1.0.3/src/quantum/
+-rw-rw-rw-   0        0        0        0 2023-04-17 21:01:23.000000 quantumcomputingsim-1.0.3/src/quantum/__init__.py
+-rw-rw-rw-   0        0        0    35759 2023-04-17 19:59:55.000000 quantumcomputingsim-1.0.3/src/quantum/quantum.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.840901 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/
+-rw-rw-rw-   0        0        0     4320 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/top_level.txt
```

### Comparing `quantumcomputingsim-1.0.2/PKG-INFO` & `quantumcomputingsim-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumcomputingsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library to simulate quantum computations
 Home-page: https://github.com/StealthyPanda/quantumcomputingsim
 Author: Shaik Mohammed Touseef
 Author-email: shaikm259@gmail.com
 Project-URL: repository, https://github.com/StealthyPanda/quantumcomputingsim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.2 Summary: A
+Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.3 Summary: A
 library to simulate quantum computations Home-page: https://github.com/
 StealthyPanda/quantumcomputingsim Author: Shaik Mohammed Touseef Author-email:
 shaikm259@gmail.com Project-URL: repository, https://github.com/StealthyPanda/
 quantumcomputingsim Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
                      **** Quantum Computing Simulator ****
```

### Comparing `quantumcomputingsim-1.0.2/README.md` & `quantumcomputingsim-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.2/quantumcomputingsim.egg-info/PKG-INFO` & `quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumcomputingsim
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library to simulate quantum computations
 Home-page: https://github.com/StealthyPanda/quantumcomputingsim
 Author: Shaik Mohammed Touseef
 Author-email: shaikm259@gmail.com
 Project-URL: repository, https://github.com/StealthyPanda/quantumcomputingsim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.2 Summary: A
+Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.3 Summary: A
 library to simulate quantum computations Home-page: https://github.com/
 StealthyPanda/quantumcomputingsim Author: Shaik Mohammed Touseef Author-email:
 shaikm259@gmail.com Project-URL: repository, https://github.com/StealthyPanda/
 quantumcomputingsim Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
                      **** Quantum Computing Simulator ****
```

### Comparing `quantumcomputingsim-1.0.2/setup.cfg` & `quantumcomputingsim-1.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7561 6e74 756d 636f 6d70 7574   = quantumcomput
 00000020: 696e 6773 696d 0d0a 7665 7273 696f 6e20  ingsim..version 
-00000030: 3d20 312e 302e 320d 0a61 7574 686f 7220  = 1.0.2..author 
+00000030: 3d20 312e 302e 330d 0a61 7574 686f 7220  = 1.0.3..author 
 00000040: 3d20 5368 6169 6b20 4d6f 6861 6d6d 6564  = Shaik Mohammed
 00000050: 2054 6f75 7365 6566 0d0a 6175 7468 6f72   Touseef..author
 00000060: 5f65 6d61 696c 203d 2073 6861 696b 6d32  _email = shaikm2
 00000070: 3539 4067 6d61 696c 2e63 6f6d 0d0a 6465  59@gmail.com..de
 00000080: 7363 7269 7074 696f 6e20 3d20 4120 6c69  scription = A li
 00000090: 6272 6172 7920 746f 2073 696d 756c 6174  brary to simulat
 000000a0: 6520 7175 616e 7475 6d20 636f 6d70 7574  e quantum comput
@@ -30,15 +30,16 @@
 000001d0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
 000001e0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
 000001f0: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
 00000200: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
 00000210: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
 00000220: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
 00000230: 6b61 6765 5f64 6972 203d 200d 0a09 3d20  kage_dir = ...= 
-00000240: 2e0d 0a70 6163 6b61 6765 7320 3d20 6669  ...packages = fi
-00000250: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
-00000260: 6972 6573 203d 203e 3d33 2e36 0d0a 0d0a  ires = >=3.6....
-00000270: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000280: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000290: 202e 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d   .....[egg_info]
-000002a0: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000002b0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000240: 7372 630d 0a70 6163 6b61 6765 7320 3d20  src..packages = 
+00000250: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000260: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
+00000270: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000280: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+00000290: 203d 2073 7263 0d0a 0d0a 5b65 6767 5f69   = src....[egg_i
+000002a0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000002b0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000002c0: 0d0a 0d0a                                ....
```

