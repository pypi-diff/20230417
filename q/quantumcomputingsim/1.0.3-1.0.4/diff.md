# Comparing `tmp/quantumcomputingsim-1.0.3.tar.gz` & `tmp/quantumcomputingsim-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantumcomputingsim-1.0.3.tar", last modified: Mon Apr 17 21:03:34 2023, max compression
+gzip compressed data, was "quantumcomputingsim-1.0.4.tar", last modified: Mon Apr 17 21:11:12 2023, max compression
```

## Comparing `quantumcomputingsim-1.0.3.tar` & `quantumcomputingsim-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.841882 quantumcomputingsim-1.0.3/
--rw-rw-rw-   0        0        0     4320 2023-04-17 21:03:34.842887 quantumcomputingsim-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-04-17 20:39:03.000000 quantumcomputingsim-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      708 2023-04-17 21:03:34.846413 quantumcomputingsim-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.769178 quantumcomputingsim-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.791263 quantumcomputingsim-1.0.3/src/quantum/
--rw-rw-rw-   0        0        0        0 2023-04-17 21:01:23.000000 quantumcomputingsim-1.0.3/src/quantum/__init__.py
--rw-rw-rw-   0        0        0    35759 2023-04-17 19:59:55.000000 quantumcomputingsim-1.0.3/src/quantum/quantum.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:03:34.840901 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/
--rw-rw-rw-   0        0        0     4320 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 21:03:34.000000 quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 21:11:12.283948 quantumcomputingsim-1.0.4/
+-rw-rw-rw-   0        0        0     4320 2023-04-17 21:11:12.283948 quantumcomputingsim-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3772 2023-04-17 20:47:22.000000 quantumcomputingsim-1.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-17 20:39:03.000000 quantumcomputingsim-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      708 2023-04-17 21:11:12.286929 quantumcomputingsim-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-17 21:11:12.248565 quantumcomputingsim-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 21:11:12.258487 quantumcomputingsim-1.0.4/src/quantum/
+-rw-rw-rw-   0        0        0       21 2023-04-17 21:10:27.000000 quantumcomputingsim-1.0.4/src/quantum/__init__.py
+-rw-rw-rw-   0        0        0    35759 2023-04-17 19:59:55.000000 quantumcomputingsim-1.0.4/src/quantum/quantum.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:11:12.283027 quantumcomputingsim-1.0.4/src/quantumcomputingsim.egg-info/
+-rw-rw-rw-   0        0        0     4320 2023-04-17 21:11:12.000000 quantumcomputingsim-1.0.4/src/quantumcomputingsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-17 21:11:12.000000 quantumcomputingsim-1.0.4/src/quantumcomputingsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:11:12.000000 quantumcomputingsim-1.0.4/src/quantumcomputingsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-17 21:11:12.000000 quantumcomputingsim-1.0.4/src/quantumcomputingsim.egg-info/top_level.txt
```

### Comparing `quantumcomputingsim-1.0.3/PKG-INFO` & `quantumcomputingsim-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumcomputingsim
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.3 Summary: A
+Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.4 Summary: A
 library to simulate quantum computations Home-page: https://github.com/
 StealthyPanda/quantumcomputingsim Author: Shaik Mohammed Touseef Author-email:
 shaikm259@gmail.com Project-URL: repository, https://github.com/StealthyPanda/
 quantumcomputingsim Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
                      **** Quantum Computing Simulator ****
```

### Comparing `quantumcomputingsim-1.0.3/README.md` & `quantumcomputingsim-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.3/setup.cfg` & `quantumcomputingsim-1.0.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7561 6e74 756d 636f 6d70 7574   = quantumcomput
 00000020: 696e 6773 696d 0d0a 7665 7273 696f 6e20  ingsim..version 
-00000030: 3d20 312e 302e 330d 0a61 7574 686f 7220  = 1.0.3..author 
+00000030: 3d20 312e 302e 340d 0a61 7574 686f 7220  = 1.0.4..author 
 00000040: 3d20 5368 6169 6b20 4d6f 6861 6d6d 6564  = Shaik Mohammed
 00000050: 2054 6f75 7365 6566 0d0a 6175 7468 6f72   Touseef..author
 00000060: 5f65 6d61 696c 203d 2073 6861 696b 6d32  _email = shaikm2
 00000070: 3539 4067 6d61 696c 2e63 6f6d 0d0a 6465  59@gmail.com..de
 00000080: 7363 7269 7074 696f 6e20 3d20 4120 6c69  scription = A li
 00000090: 6272 6172 7920 746f 2073 696d 756c 6174  brary to simulat
 000000a0: 6520 7175 616e 7475 6d20 636f 6d70 7574  e quantum comput
```

### Comparing `quantumcomputingsim-1.0.3/src/quantum/quantum.py` & `quantumcomputingsim-1.0.4/src/quantum/quantum.py`

 * *Files identical despite different names*

### Comparing `quantumcomputingsim-1.0.3/src/quantumcomputingsim.egg-info/PKG-INFO` & `quantumcomputingsim-1.0.4/src/quantumcomputingsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantumcomputingsim
-Version: 1.0.3
+Version: 1.0.4
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
-Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.3 Summary: A
+Metadata-Version: 2.1 Name: quantumcomputingsim Version: 1.0.4 Summary: A
 library to simulate quantum computations Home-page: https://github.com/
 StealthyPanda/quantumcomputingsim Author: Shaik Mohammed Touseef Author-email:
 shaikm259@gmail.com Project-URL: repository, https://github.com/StealthyPanda/
 quantumcomputingsim Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
                      **** Quantum Computing Simulator ****
```

