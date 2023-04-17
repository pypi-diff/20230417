# Comparing `tmp/svgelements-1.9.1.tar.gz` & `tmp/svgelements-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgelements-1.9.1.tar", last modified: Sun Mar 12 13:06:06 2023, max compression
+gzip compressed data, was "svgelements-1.9.2.tar", last modified: Mon Apr 17 01:35:32 2023, max compression
```

## Comparing `svgelements-1.9.1.tar` & `svgelements-1.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 13:06:06.184138 svgelements-1.9.1/
--rw-rw-rw-   0        0        0     1086 2021-03-07 12:37:37.000000 svgelements-1.9.1/LICENSE
--rw-rw-rw-   0        0        0       29 2021-03-07 12:37:37.000000 svgelements-1.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0    52532 2023-03-12 13:06:06.184138 svgelements-1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    43759 2022-12-14 13:48:03.000000 svgelements-1.9.1/README.md
--rw-rw-rw-   0        0        0    20174 2021-11-29 01:11:10.000000 svgelements-1.9.1/pyproject.toml
--rw-rw-rw-   0        0        0        2 2021-03-07 12:37:37.000000 svgelements-1.9.1/requirements.txt
--rw-rw-rw-   0        0        0     1293 2023-03-12 13:06:06.186138 svgelements-1.9.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-03-07 12:37:37.000000 svgelements-1.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-12 13:06:06.120135 svgelements-1.9.1/svgelements/
--rw-rw-rw-   0        0        0       50 2021-03-07 12:37:37.000000 svgelements-1.9.1/svgelements/__init__.py
--rw-rw-rw-   0        0        0   338549 2023-03-12 12:52:17.000000 svgelements-1.9.1/svgelements/svgelements.py
-drwxrwxrwx   0        0        0        0 2023-03-12 13:06:06.174138 svgelements-1.9.1/svgelements.egg-info/
--rw-rw-rw-   0        0        0    52532 2023-03-12 13:06:06.000000 svgelements-1.9.1/svgelements.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1792 2023-03-12 13:06:06.000000 svgelements-1.9.1/svgelements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 13:06:06.000000 svgelements-1.9.1/svgelements.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-12 13:06:06.000000 svgelements-1.9.1/svgelements.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2021-03-07 12:40:17.000000 svgelements-1.9.1/svgelements.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-03-12 13:06:06.166137 svgelements-1.9.1/test/
--rw-rw-rw-   0        0        0       16 2021-03-07 12:37:37.000000 svgelements-1.9.1/test/__init__.py
--rw-rw-rw-   0        0        0     2018 2021-11-29 01:11:10.000000 svgelements-1.9.1/test/test_angle.py
--rw-rw-rw-   0        0        0      686 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_approximate.py
--rw-rw-rw-   0        0        0    16931 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_arc_length.py
--rw-rw-rw-   0        0        0    11940 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_bbox.py
--rw-rw-rw-   0        0        0     3920 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_clippath.py
--rw-rw-rw-   0        0        0    11473 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_color.py
--rw-rw-rw-   0        0        0     5587 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_copy.py
--rw-rw-rw-   0        0        0     3002 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_css.py
--rw-rw-rw-   0        0        0     2380 2023-03-12 12:54:16.000000 svgelements-1.9.1/test/test_cubic_bezier.py
--rw-rw-rw-   0        0        0      581 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_descriptive_elements.py
--rw-rw-rw-   0        0        0     3455 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_element.py
--rw-rw-rw-   0        0        0     2722 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_generation.py
--rw-rw-rw-   0        0        0     3558 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_group.py
--rw-rw-rw-   0        0        0     9689 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_image.py
--rw-rw-rw-   0        0        0     2364 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_intersections.py
--rw-rw-rw-   0        0        0     8047 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_length.py
--rw-rw-rw-   0        0        0    14622 2023-03-12 07:17:05.000000 svgelements-1.9.1/test/test_matrix.py
--rw-rw-rw-   0        0        0    43440 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_parsing.py
--rw-rw-rw-   0        0        0    11758 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_path.py
--rw-rw-rw-   0        0        0     3998 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_path_dunder.py
--rw-rw-rw-   0        0        0     1845 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_path_segments.py
--rw-rw-rw-   0        0        0    35183 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_paths.py
--rw-rw-rw-   0        0        0     5696 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_point.py
--rw-rw-rw-   0        0        0     1238 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_quadratic_bezier.py
--rw-rw-rw-   0        0        0     8241 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_repr.py
--rw-rw-rw-   0        0        0    24573 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_shape.py
--rw-rw-rw-   0        0        0     2078 2022-11-22 21:25:13.000000 svgelements-1.9.1/test/test_stroke_width.py
--rw-rw-rw-   0        0        0     7887 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_text.py
--rw-rw-rw-   0        0        0    11074 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_use.py
--rw-rw-rw-   0        0        0    11876 2023-03-12 07:16:49.000000 svgelements-1.9.1/test/test_viewbox.py
--rw-rw-rw-   0        0        0     5279 2023-03-12 07:17:05.000000 svgelements-1.9.1/test/test_write.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:35:32.805911 svgelements-1.9.2/
+-rw-rw-rw-   0        0        0     1086 2021-03-07 12:37:37.000000 svgelements-1.9.2/LICENSE
+-rw-rw-rw-   0        0        0       29 2021-03-07 12:37:37.000000 svgelements-1.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    52412 2023-04-17 01:35:32.805911 svgelements-1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    43759 2022-12-14 13:48:03.000000 svgelements-1.9.2/README.md
+-rw-rw-rw-   0        0        0    20174 2021-11-29 01:11:10.000000 svgelements-1.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0        2 2021-03-07 12:37:37.000000 svgelements-1.9.2/requirements.txt
+-rw-rw-rw-   0        0        0     1195 2023-04-17 01:35:32.807911 svgelements-1.9.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2021-03-07 12:37:37.000000 svgelements-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:35:32.705906 svgelements-1.9.2/svgelements/
+-rw-rw-rw-   0        0        0       50 2021-03-07 12:37:37.000000 svgelements-1.9.2/svgelements/__init__.py
+-rw-rw-rw-   0        0        0   338252 2023-04-17 01:32:51.000000 svgelements-1.9.2/svgelements/svgelements.py
+drwxrwxrwx   0        0        0        0 2023-04-17 01:35:32.793911 svgelements-1.9.2/svgelements.egg-info/
+-rw-rw-rw-   0        0        0    52412 2023-04-17 01:35:32.000000 svgelements-1.9.2/svgelements.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1792 2023-04-17 01:35:32.000000 svgelements-1.9.2/svgelements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 01:35:32.000000 svgelements-1.9.2/svgelements.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-17 01:35:32.000000 svgelements-1.9.2/svgelements.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2021-03-07 12:40:17.000000 svgelements-1.9.2/svgelements.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-17 01:35:32.778910 svgelements-1.9.2/test/
+-rw-rw-rw-   0        0        0       16 2021-03-07 12:37:37.000000 svgelements-1.9.2/test/__init__.py
+-rw-rw-rw-   0        0        0     2018 2021-11-29 01:11:10.000000 svgelements-1.9.2/test/test_angle.py
+-rw-rw-rw-   0        0        0      686 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_approximate.py
+-rw-rw-rw-   0        0        0    16931 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_arc_length.py
+-rw-rw-rw-   0        0        0    11940 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_bbox.py
+-rw-rw-rw-   0        0        0     3920 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_clippath.py
+-rw-rw-rw-   0        0        0    11473 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_color.py
+-rw-rw-rw-   0        0        0     5587 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_copy.py
+-rw-rw-rw-   0        0        0     3002 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_css.py
+-rw-rw-rw-   0        0        0     2869 2023-04-17 01:15:35.000000 svgelements-1.9.2/test/test_cubic_bezier.py
+-rw-rw-rw-   0        0        0      581 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_descriptive_elements.py
+-rw-rw-rw-   0        0        0     3455 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_element.py
+-rw-rw-rw-   0        0        0     2722 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_generation.py
+-rw-rw-rw-   0        0        0     3558 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_group.py
+-rw-rw-rw-   0        0        0     9689 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_image.py
+-rw-rw-rw-   0        0        0     2364 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_intersections.py
+-rw-rw-rw-   0        0        0     8047 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_length.py
+-rw-rw-rw-   0        0        0    14622 2023-03-12 07:17:05.000000 svgelements-1.9.2/test/test_matrix.py
+-rw-rw-rw-   0        0        0    43440 2023-04-16 03:01:52.000000 svgelements-1.9.2/test/test_parsing.py
+-rw-rw-rw-   0        0        0    13239 2023-04-17 01:32:51.000000 svgelements-1.9.2/test/test_path.py
+-rw-rw-rw-   0        0        0     3998 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_path_dunder.py
+-rw-rw-rw-   0        0        0     1845 2023-04-16 03:11:48.000000 svgelements-1.9.2/test/test_path_segments.py
+-rw-rw-rw-   0        0        0    35183 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_paths.py
+-rw-rw-rw-   0        0        0     5696 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_point.py
+-rw-rw-rw-   0        0        0     1238 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_quadratic_bezier.py
+-rw-rw-rw-   0        0        0     8241 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_repr.py
+-rw-rw-rw-   0        0        0    24573 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_shape.py
+-rw-rw-rw-   0        0        0     2078 2022-11-22 21:25:13.000000 svgelements-1.9.2/test/test_stroke_width.py
+-rw-rw-rw-   0        0        0     7887 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_text.py
+-rw-rw-rw-   0        0        0    11074 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_use.py
+-rw-rw-rw-   0        0        0    11876 2023-03-12 07:16:49.000000 svgelements-1.9.2/test/test_viewbox.py
+-rw-rw-rw-   0        0        0     5279 2023-03-12 07:17:05.000000 svgelements-1.9.2/test/test_write.py
```

### Comparing `svgelements-1.9.1/LICENSE` & `svgelements-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/PKG-INFO` & `svgelements-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgelements
-Version: 1.9.1
+Version: 1.9.2
 Summary: Svg Elements Parsing
 Home-page: https://github.com/meerk40t/svgelements
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
 Description: # svgelements
         
@@ -953,20 +953,18 @@
 Keywords: svg,path,elements,matrix,vector,parser
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `svgelements-1.9.1/README.md` & `svgelements-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/pyproject.toml` & `svgelements-1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/setup.cfg` & `svgelements-1.9.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7667 656c 656d 656e 7473 0d0a   = svgelements..
-00000020: 7665 7273 696f 6e20 3d20 312e 392e 310d  version = 1.9.1.
+00000020: 7665 7273 696f 6e20 3d20 312e 392e 320d  version = 1.9.2.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2053  .description = S
 00000040: 7667 2045 6c65 6d65 6e74 7320 5061 7273  vg Elements Pars
 00000050: 696e 670d 0a6c 6f6e 675f 6465 7363 7269  ing..long_descri
 00000060: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
 00000070: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
 00000080: 776e 0d0a 6c6f 6e67 5f64 6573 6372 6970  wn..long_descrip
 00000090: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
@@ -19,63 +19,57 @@
 00000120: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
 00000130: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
 00000140: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
 00000150: 6465 6e74 0d0a 0950 726f 6772 616d 6d69  dent...Programmi
 00000160: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 00000170: 7974 686f 6e0d 0a09 5072 6f67 7261 6d6d  ython...Programm
 00000180: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000190: 5079 7468 6f6e 203a 3a20 322e 370d 0a09  Python :: 2.7...
+00000190: 5079 7468 6f6e 203a 3a20 332e 360d 0a09  Python :: 3.6...
 000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 000001b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001c0: 3a20 332e 350d 0a09 5072 6f67 7261 6d6d  : 3.5...Programm
+000001c0: 3a20 332e 370d 0a09 5072 6f67 7261 6d6d  : 3.7...Programm
 000001d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001e0: 5079 7468 6f6e 203a 3a20 332e 360d 0a09  Python :: 3.6...
+000001e0: 5079 7468 6f6e 203a 3a20 332e 380d 0a09  Python :: 3.8...
 000001f0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 00000200: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000210: 3a20 332e 370d 0a09 5072 6f67 7261 6d6d  : 3.7...Programm
+00000210: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
 00000220: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000230: 5079 7468 6f6e 203a 3a20 332e 380d 0a09  Python :: 3.8...
-00000240: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000250: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000260: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
-00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000280: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
-00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002b0: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
-000002c0: 6e20 3a3a 2050 7950 790d 0a09 546f 7069  n :: PyPy...Topi
-000002d0: 6320 3a3a 204d 756c 7469 6d65 6469 6120  c :: Multimedia 
-000002e0: 3a3a 2047 7261 7068 6963 730d 0a09 546f  :: Graphics...To
-000002f0: 7069 6320 3a3a 204d 756c 7469 6d65 6469  pic :: Multimedi
-00000300: 6120 3a3a 2047 7261 7068 6963 7320 3a3a  a :: Graphics ::
-00000310: 2045 6469 746f 7273 203a 3a20 5665 6374   Editors :: Vect
-00000320: 6f72 2d42 6173 6564 0d0a 0954 6f70 6963  or-Based...Topic
-00000330: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-00000340: 656c 6f70 6d65 6e74 203a 3a20 4c69 6272  elopment :: Libr
-00000350: 6172 6965 7320 3a3a 2050 7974 686f 6e20  aries :: Python 
-00000360: 4d6f 6475 6c65 730d 0a09 546f 7069 6320  Modules...Topic 
-00000370: 3a3a 2055 7469 6c69 7469 6573 0d0a 6b65  :: Utilities..ke
-00000380: 7977 6f72 6473 203d 2073 7667 2c20 7061  ywords = svg, pa
-00000390: 7468 2c20 656c 656d 656e 7473 2c20 6d61  th, elements, ma
-000003a0: 7472 6978 2c20 7665 6374 6f72 2c20 7061  trix, vector, pa
-000003b0: 7273 6572 0d0a 6175 7468 6f72 203d 2054  rser..author = T
-000003c0: 6174 6172 697a 650d 0a61 7574 686f 725f  atarize..author_
-000003d0: 656d 6169 6c20 3d20 7461 7461 7269 7a65  email = tatarize
-000003e0: 4067 6d61 696c 2e63 6f6d 0d0a 7572 6c20  @gmail.com..url 
-000003f0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000400: 2e63 6f6d 2f6d 6565 726b 3430 742f 7376  .com/meerk40t/sv
-00000410: 6765 6c65 6d65 6e74 730d 0a6c 6963 656e  gelements..licen
-00000420: 7365 203d 204d 4954 0d0a 0d0a 5b6f 7074  se = MIT....[opt
-00000430: 696f 6e73 5d0d 0a7a 6970 5f73 6166 6520  ions]..zip_safe 
-00000440: 3d20 5472 7565 0d0a 696e 636c 7564 655f  = True..include_
-00000450: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000460: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
-00000470: 6669 6e64 3a0d 0a70 6163 6b61 6765 5f64  find:..package_d
-00000480: 6972 203d 200d 0a09 3d20 2e0d 0a74 6573  ir = ...= ...tes
-00000490: 745f 7375 6974 6520 3d20 7465 7374 0d0a  t_suite = test..
-000004a0: 0d0a 5b70 6570 385d 0d0a 6d61 782d 6c69  ..[pep8]..max-li
-000004b0: 6e65 2d6c 656e 6774 6820 3d20 3130 300d  ne-length = 100.
-000004c0: 0a0d 0a5b 6264 6973 745f 7768 6565 6c5d  ...[bdist_wheel]
-000004d0: 0d0a 756e 6976 6572 7361 6c20 3d20 310d  ..universal = 1.
-000004e0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000004f0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000500: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000230: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+00000240: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000250: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000260: 3a3a 2033 2e31 310d 0a09 546f 7069 6320  :: 3.11...Topic 
+00000270: 3a3a 204d 756c 7469 6d65 6469 6120 3a3a  :: Multimedia ::
+00000280: 2047 7261 7068 6963 730d 0a09 546f 7069   Graphics...Topi
+00000290: 6320 3a3a 204d 756c 7469 6d65 6469 6120  c :: Multimedia 
+000002a0: 3a3a 2047 7261 7068 6963 7320 3a3a 2045  :: Graphics :: E
+000002b0: 6469 746f 7273 203a 3a20 5665 6374 6f72  ditors :: Vector
+000002c0: 2d42 6173 6564 0d0a 0954 6f70 6963 203a  -Based...Topic :
+000002d0: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+000002e0: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
+000002f0: 6965 7320 3a3a 2050 7974 686f 6e20 4d6f  ies :: Python Mo
+00000300: 6475 6c65 730d 0a09 546f 7069 6320 3a3a  dules...Topic ::
+00000310: 2055 7469 6c69 7469 6573 0d0a 6b65 7977   Utilities..keyw
+00000320: 6f72 6473 203d 2073 7667 2c20 7061 7468  ords = svg, path
+00000330: 2c20 656c 656d 656e 7473 2c20 6d61 7472  , elements, matr
+00000340: 6978 2c20 7665 6374 6f72 2c20 7061 7273  ix, vector, pars
+00000350: 6572 0d0a 6175 7468 6f72 203d 2054 6174  er..author = Tat
+00000360: 6172 697a 650d 0a61 7574 686f 725f 656d  arize..author_em
+00000370: 6169 6c20 3d20 7461 7461 7269 7a65 4067  ail = tatarize@g
+00000380: 6d61 696c 2e63 6f6d 0d0a 7572 6c20 3d20  mail.com..url = 
+00000390: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000003a0: 6f6d 2f6d 6565 726b 3430 742f 7376 6765  om/meerk40t/svge
+000003b0: 6c65 6d65 6e74 730d 0a6c 6963 656e 7365  lements..license
+000003c0: 203d 204d 4954 0d0a 0d0a 5b6f 7074 696f   = MIT....[optio
+000003d0: 6e73 5d0d 0a7a 6970 5f73 6166 6520 3d20  ns]..zip_safe = 
+000003e0: 5472 7565 0d0a 696e 636c 7564 655f 7061  True..include_pa
+000003f0: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+00000400: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
+00000410: 6e64 3a0d 0a70 6163 6b61 6765 5f64 6972  nd:..package_dir
+00000420: 203d 200d 0a09 3d20 2e0d 0a74 6573 745f   = ...= ...test_
+00000430: 7375 6974 6520 3d20 7465 7374 0d0a 0d0a  suite = test....
+00000440: 5b70 6570 385d 0d0a 6d61 782d 6c69 6e65  [pep8]..max-line
+00000450: 2d6c 656e 6774 6820 3d20 3130 300d 0a0d  -length = 100...
+00000460: 0a5b 6264 6973 745f 7768 6565 6c5d 0d0a  .[bdist_wheel]..
+00000470: 756e 6976 6572 7361 6c20 3d20 310d 0a0d  universal = 1...
+00000480: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+00000490: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000004a0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `svgelements-1.9.1/svgelements/svgelements.py` & `svgelements-1.9.2/svgelements/svgelements.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 be used to provide much of the decisions within path objects. Such that if there is a question on
 implementation if the SVG documentation has a methodology it should be used.
 
 Though not required the Image class acquires new functionality if provided with PIL/Pillow as an import
 and the Arc can do exact arc calculations if scipy is installed.
 """
 
-SVGELEMENTS_VERSION = "1.9.1"
+SVGELEMENTS_VERSION = "1.9.2"
 
 MIN_DEPTH = 5
 ERROR = 1e-12
 
 max_depth = 0
 
 # SVG STATIC VALUES
@@ -4769,15 +4769,15 @@
         """returns the minimum and maximum for a real cubic bezier, with a non-zero denom
         Code by:
         https://github.com/mathandy/svgpathtools
         """
         local_extremizers = [0, 1]
         a = [c[v] for c in self]
         denom = a[0] - 3 * a[1] + 3 * a[2] - a[3]
-        if abs(denom) >= 1e-12:
+        if abs(denom) >= 1e-8:
             delta = (
                 a[1] * a[1] - (a[0] + a[1]) * a[2] + a[2] * a[2] + (a[0] - a[1]) * a[3]
             )
             if delta >= 0:  # otherwise no local extrema
                 sqdelta = sqrt(delta)
                 tau = a[0] - 2 * a[1] + a[2]
                 r1 = (tau + sqdelta) / denom
@@ -6049,162 +6049,130 @@
 
     def start(self):
         pass
 
     def end(self):
         pass
 
-    def move(self, *points, **kwargs):
-        relative = kwargs["relative"] if "relative" in kwargs else False
+    def move(self, *points, relative=False, **kwargs):
         start_pos = self.current_point
         end_pos = points[0]
         if end_pos in ("z", "Z"):
             end_pos = self.z_point
-        segment = Move(start_pos, end_pos)
-        segment.relative = relative
-        self.append(segment)
+        self.append(Move(start_pos, end_pos, relative=relative))
         if len(points) > 1:
             self.line(*points[1:], relative=relative)
         return self
 
-    def line(self, *points, **kwargs):
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        end_pos = points[0]
-        if end_pos in ("z", "Z"):
-            end_pos = self.z_point
-        segment = Line(start_pos, end_pos)
-        segment.relative = relative
-        self.append(segment)
-        if len(points) > 1:
-            self.line(*points[1:])
+    def line(self, *points, relative=False, **kwargs):
+        for index in range(len(points)):
+            start_pos = self.current_point
+            end_pos = points[index]
+            if end_pos in ("z", "Z"):
+                end_pos = self.z_point
+            self.append(Line(start_pos, end_pos, relative=relative))
         return self
 
-    def vertical(self, *y_points, **kwargs):
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        if relative:
-            segment = Line(start_pos, Point(start_pos.x, start_pos.y + y_points[0]))
-        else:
-            segment = Line(start_pos, Point(start_pos.x, y_points[0]))
-        segment.relative = relative
-        self.append(segment)
-        if len(y_points) > 1:
-            self.vertical(*y_points[1:], relative=relative)
+    def vertical(self, *y_points, relative=False, **kwargs):
+        for index in range(len(y_points)):
+            start_pos = self.current_point
+            if relative:
+                self.append(Line(start_pos, Point(start_pos.x, start_pos.y + y_points[index]), relative=relative))
+            else:
+                self.append(Line(start_pos, Point(start_pos.x, y_points[index]), relative=relative))
         return self
 
-    def horizontal(self, *x_points, **kwargs):
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        if relative:
-            segment = Line(start_pos, Point(start_pos.x + x_points[0], start_pos.y))
-            segment.relative = relative
-        else:
-            segment = Line(start_pos, Point(x_points[0], start_pos.y))
-            segment.relative = relative
-        self.append(segment)
-        if len(x_points) > 1:
-            self.horizontal(*x_points[1:], relative=relative)
+    def horizontal(self, *x_points, relative=False, **kwargs):
+        for index in range(len(x_points)):
+            start_pos = self.current_point
+            if relative:
+                self.append(Line(start_pos, Point(start_pos.x + x_points[index], start_pos.y), relative=relative))
+            else:
+                self.append(Line(start_pos, Point(x_points[index], start_pos.y), relative=relative))
         return self
 
-    def smooth_quad(self, *points, **kwargs):
+    def smooth_quad(self, *points, relative=False, **kwargs):
         """Smooth curve. First control point is the "reflection" of
         the second control point in the previous path."""
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        control1 = self.smooth_point
-        end_pos = points[0]
-        if end_pos in ("z", "Z"):
-            end_pos = self.z_point
-        segment = QuadraticBezier(start_pos, control1, end_pos)
-        segment.relative = relative
-        segment.smooth = True
-        self.append(segment)
-        if len(points) > 1:
-            self.smooth_quad(*points[1:])
+        for index in range(len(points)):
+            start_pos = self.current_point
+            control1 = self.smooth_point
+            end_pos = points[index]
+            if end_pos in ("z", "Z"):
+                end_pos = self.z_point
+            self.append(QuadraticBezier(start_pos, control1, end_pos, relative=relative, smooth=True))
         return self
 
-    def quad(self, *points, **kwargs):
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        control = points[0]
-        if control in ("z", "Z"):
-            control = self.z_point
-        end_pos = points[1]
-        if end_pos in ("z", "Z"):
-            end_pos = self.z_point
-        segment = QuadraticBezier(start_pos, control, end_pos)
-        segment.relative = relative
-        segment.smooth = False
-        self.append(segment)
-        if len(points) > 2:
-            self.quad(*points[2:])
+    def quad(self, *points, relative=False, **kwargs):
+        for index in range(0, len(points), 2):
+            start_pos = self.current_point
+            control = points[index]
+            if control in ("z", "Z"):
+                control = self.z_point
+                self.append(QuadraticBezier(start_pos, control, control, relative=relative, smooth=False))
+                return self
+            end_pos = points[index + 1]
+            if end_pos in ("z", "Z"):
+                end_pos = self.z_point
+            self.append(QuadraticBezier(start_pos, control, end_pos, relative=relative, smooth=False))
         return self
 
-    def smooth_cubic(self, *points, **kwargs):
+    def smooth_cubic(self, *points, relative=False, **kwargs):
         """Smooth curve. First control point is the "reflection" of
         the second control point in the previous path."""
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        control1 = self.smooth_point
-        control2 = points[0]
-
-        if control2 in ("z", "Z"):
-            control2 = self.z_point
-        end_pos = points[1]
-        if end_pos in ("z", "Z"):
-            end_pos = self.z_point
-        segment = CubicBezier(start_pos, control1, control2, end_pos)
-        segment.relative = relative
-        segment.smooth = True
-        self.append(segment)
-        if len(points) > 2:
-            self.smooth_cubic(*points[2:])
+        for index in range(0, len(points), 2):
+            start_pos = self.current_point
+            control1 = self.smooth_point
+            control2 = points[index]
+
+            if control2 in ("z", "Z"):
+                control2 = self.z_point
+                self.append(CubicBezier(start_pos, control1, control2, control2, relative=relative, smooth=True))
+                return self
+            end_pos = points[index + 1]
+            if end_pos in ("z", "Z"):
+                end_pos = self.z_point
+            self.append(CubicBezier(start_pos, control1, control2, end_pos, relative=relative, smooth=True))
         return self
 
-    def cubic(self, *points, **kwargs):
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        control1 = points[0]
-        if control1 in ("z", "Z"):
-            control1 = self.z_point
-        control2 = points[1]
-        if control2 in ("z", "Z"):
-            control2 = self.z_point
-        end_pos = points[2]
-        if end_pos in ("z", "Z"):
-            end_pos = self.z_point
-        segment = CubicBezier(start_pos, control1, control2, end_pos)
-        segment.relative = relative
-        segment.smooth = False
-        self.append(segment)
-        if len(points) > 3:
-            self.cubic(*points[3:])
+    def cubic(self, *points, relative=False, **kwargs):
+        for index in range(0, len(points), 3):
+            start_pos = self.current_point
+            control1 = points[index]
+            if control1 in ("z", "Z"):
+                control1 = self.z_point
+                self.append(CubicBezier(start_pos, control1, control1, control1, relative=relative, smooth=True))
+                return self
+            control2 = points[index + 1]
+            if control2 in ("z", "Z"):
+                control2 = self.z_point
+                self.append(CubicBezier(start_pos, control1, control2, control2, relative=relative, smooth=True))
+                return self
+            end_pos = points[index + 2]
+            if end_pos in ("z", "Z"):
+                end_pos = self.z_point
+            self.append(CubicBezier(start_pos, control1, control2, end_pos, relative=relative, smooth=False))
         return self
 
-    def arc(self, *arc_args, **kwargs):
-        relative = kwargs["relative"] if "relative" in kwargs else False
-        start_pos = self.current_point
-        rx = arc_args[0]
-        ry = arc_args[1]
-        if rx < 0:
-            rx = abs(rx)
-        if ry < 0:
-            ry = abs(ry)
-        rotation = arc_args[2]
-        arc = arc_args[3]
-        sweep = arc_args[4]
-        end_pos = arc_args[5]
-        if end_pos in ("z", "Z"):
-            end_pos = self.z_point
-        segment = Arc(start_pos, rx, ry, rotation, arc, sweep, end_pos)
-        segment.relative = relative
-        self.append(segment)
-        if len(arc_args) > 6:
-            self.arc(*arc_args[6:])
+    def arc(self, *arc_args, relative=False, **kwargs):
+        for index in range(0, len(arc_args), 6):
+            start_pos = self.current_point
+            rx = arc_args[index]
+            ry = arc_args[index + 1]
+            if rx < 0:
+                rx = abs(rx)
+            if ry < 0:
+                ry = abs(ry)
+            rotation = arc_args[index + 2]
+            arc = arc_args[index + 3]
+            sweep = arc_args[index + 4]
+            end_pos = arc_args[index + 5]
+            if end_pos in ("z", "Z"):
+                end_pos = self.z_point
+            self.append(Arc(start_pos, rx, ry, rotation, arc, sweep, end_pos, relative=relative))
         return self
 
     def closed(self, relative=False):
         start_pos = self.current_point
         end_pos = self.z_point
         segment = Close(start_pos, end_pos)
         segment.relative = relative
```

### Comparing `svgelements-1.9.1/svgelements.egg-info/PKG-INFO` & `svgelements-1.9.2/svgelements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgelements
-Version: 1.9.1
+Version: 1.9.2
 Summary: Svg Elements Parsing
 Home-page: https://github.com/meerk40t/svgelements
 Author: Tatarize
 Author-email: tatarize@gmail.com
 License: MIT
 Description: # svgelements
         
@@ -953,20 +953,18 @@
 Keywords: svg,path,elements,matrix,vector,parser
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `svgelements-1.9.1/svgelements.egg-info/SOURCES.txt` & `svgelements-1.9.2/svgelements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_angle.py` & `svgelements-1.9.2/test/test_angle.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_approximate.py` & `svgelements-1.9.2/test/test_approximate.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_arc_length.py` & `svgelements-1.9.2/test/test_arc_length.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_bbox.py` & `svgelements-1.9.2/test/test_bbox.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_clippath.py` & `svgelements-1.9.2/test/test_clippath.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_color.py` & `svgelements-1.9.2/test/test_color.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_copy.py` & `svgelements-1.9.2/test/test_copy.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_css.py` & `svgelements-1.9.2/test/test_css.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_cubic_bezier.py` & `svgelements-1.9.2/test/test_quadratic_bezier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,37 @@
-import random
 import unittest
 from random import *
 
 from svgelements import *
 
 
-def get_random_cubic_bezier():
-    return CubicBezier(
-        (random() * 50, random() * 50),
-        (random() * 50, random() * 50),
-        (random() * 50, random() * 50),
-        (random() * 50, random() * 50),
-    )
-
-
-class TestElementCubicBezierLength(unittest.TestCase):
-    def test_cubic_bezier_length(self):
-        n = 100
-        error = 0
-        for _ in range(n):
-            b = get_random_cubic_bezier()
-            l1 = b._length_scipy()
-            l2 = b._length_default(error=1e-6)
-            c = abs(l1 - l2)
-            error += c
-            self.assertAlmostEqual(l1, l2, places=1)
-        print("Average cubic-line error: %g" % (error / n))
+def get_random_quadratic_bezier():
+    return QuadraticBezier((random() * 50, random() * 50), (random() * 50, random() * 50),
+                           (random() * 50, random() * 50))
 
 
-class TestElementCubicBezierPoint(unittest.TestCase):
-    def test_cubic_bezier_point_start_stop(self):
-        import numpy as np
+class TestElementQuadraticBezierPoint(unittest.TestCase):
 
+    def test_quadratic_bezier_point_start_stop(self):
+        import numpy as np
         for _ in range(1000):
-            b = get_random_cubic_bezier()
+            b = get_random_quadratic_bezier()
             self.assertEqual(b.start, b.point(0))
             self.assertEqual(b.end, b.point(1))
-            self.assertTrue(
-                np.all(np.array([list(b.start), list(b.end)]) == b.npoint([0, 1]))
-            )
+            self.assertTrue(np.all(np.array([list(b.start), list(b.end)])
+                                   == b.npoint([0, 1])))
 
-    def test_cubic_bezier_point_implementations_match(self):
+    def test_quadratic_bezier_point_implementations_match(self):
         import numpy as np
-
         for _ in range(1000):
-            b = get_random_cubic_bezier()
+            b = get_random_quadratic_bezier()
 
             pos = np.linspace(0, 1, 100)
 
             v1 = b.npoint(pos)
             v2 = []
             for i in range(len(pos)):
                 v2.append(b.point(pos[i]))
 
             for p, p1, p2 in zip(pos, v1, v2):
                 self.assertEqual(b.point(p), Point(p1))
                 self.assertEqual(Point(p1), Point(p2))
-
-    def test_cubic_bounds_issue_214(self):
-        cubic = CubicBezier(0, -2 - 3j, -1 - 4j, -3j)
-        bbox = cubic.bbox()
-        self.assertLess(bbox[1], -3)
-
-    def test_cubic_bounds_issue_214_random(self):
-        for i in range(100):
-            a = random() * 5
-            b = random() * 5
-            c = random() * 5
-            d = a - 3 * b + 3 * c
-            cubic1 = CubicBezier(a, b, c, d)
-            bbox1 = cubic1.bbox()
-            cubic2 = CubicBezier(a, b, c, d + 1e-11)
-            bbox2 = cubic2.bbox()
-            for a, b in zip(bbox1, bbox2):
-                self.assertAlmostEqual(a, b, delta=1e-5)
```

### Comparing `svgelements-1.9.1/test/test_descriptive_elements.py` & `svgelements-1.9.2/test/test_descriptive_elements.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_element.py` & `svgelements-1.9.2/test/test_element.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_generation.py` & `svgelements-1.9.2/test/test_generation.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_group.py` & `svgelements-1.9.2/test/test_group.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_image.py` & `svgelements-1.9.2/test/test_image.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_intersections.py` & `svgelements-1.9.2/test/test_intersections.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_length.py` & `svgelements-1.9.2/test/test_length.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_matrix.py` & `svgelements-1.9.2/test/test_matrix.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_parsing.py` & `svgelements-1.9.2/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_path.py` & `svgelements-1.9.2/test/test_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -231,23 +231,32 @@
         self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 Q 20,33 100,100 Q 180,167 13,45 T 16,16 T 34,56 T 4,4 z")
 
     def test_path_z_termination(self):
         m = Path("M 4,4 L 20,20 L 25,25 L 6,3 Q 20,33 Z")
         self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 Q 20,33 4,4 Z")
         m = Path("M 4,4 L 20,20 L 25,25 L 6,3 Q 20,33 100,100 T Z")
         self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 Q 20,33 100,100 T 4,4 Z")
+        m = Path("M 4,4 L 20,20 L 25,25 L 6,3 Q Z")
+        self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 Q 4,4 4,4 Z")
+        m = Path("M 4,4 L 20,20 L 25,25 L 6,3 C Z")
+        self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 C 4,4 4,4 4,4 Z")
         m = Path("M 4,4 L 20,20 L 25,25 L 6,3 Q 20,33 100,100 T z")
         self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 Q 20,33 100,100 T 4,4 z")
         m = Path("m 0,0 1,1 A 5.01,5.01 180 0,0 z")
         self.assertEqual(m.d(), "m 0,0 l 1,1 A 5.01,5.01 180 0,0 0,0 z")
         m = Path("m0,0z")
         self.assertEqual(m.d(), "m 0,0 z")
         m = Path("M0,0Lz")
         self.assertEqual(m.d(), "M 0,0 L 0,0 z")
 
+        m = Path("M 4,4 L 20,20 L 25,25 L 6,3").quad("Z").closed()
+        self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 Q 4,4 4,4 Z")
+        m = Path("M 4,4 L 20,20 L 25,25 L 6,3").cubic("Z").closed()
+        self.assertEqual(m.d(), "M 4,4 L 20,20 L 25,25 L 6,3 C 4,4 4,4 4,4 Z")
+
     def test_path_setitem_slice(self):
         m = Path("M0,0 1,1 z")
         m[1:] = 'L2,2z'
         self.assertEqual(m.d(), "M 0,0 L 2,2 z")
         self.assertTrue(m._is_valid())
         del m[1]
         self.assertEqual(m.d(), "M 0,0 z")
@@ -285,7 +294,39 @@
         self.assertEqual(m.d(), "M 0,0 L 1,1 M 5,5 z")
         self.assertTrue(m._is_valid())
 
         m = Path("M0,0 1,1 z")
         def m_assign():
             m[-1] = 'M5,5z'
         self.assertRaises(ValueError, m_assign)
+
+    def test_iterative_loop_building_line(self):
+        path = Path()
+        path.move(0)
+        path.line(*([complex(1, 1)] * 2000))
+
+    def test_iterative_loop_building_vert(self):
+        path = Path()
+        path.move(0)
+        path.vertical(*([5.0] * 2000))
+
+    def test_iterative_loop_building_horiz(self):
+        path = Path()
+        path.move(0)
+        path.horizontal(*([5.0] * 2000))
+
+    def test_iterative_loop_building_quad(self):
+        path = Path()
+        path.move(0)
+        path.quad(*([complex(1, 1), complex(1, 1)] * 1000))
+
+    def test_iterative_loop_building_cubic(self):
+        path = Path()
+        path.move(0)
+        path.cubic(*([complex(1, 1), complex(1, 1), complex(1, 1)] * 1000))
+
+    def test_iterative_loop_building_arc(self):
+        path = Path()
+        path.move(0)
+        q = [0, 0, 0, 0, 0, complex(1, 1)] * 2000
+        path.arc(*q)
+
```

### Comparing `svgelements-1.9.1/test/test_path_dunder.py` & `svgelements-1.9.2/test/test_path_dunder.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_path_segments.py` & `svgelements-1.9.2/test/test_path_segments.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_paths.py` & `svgelements-1.9.2/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_point.py` & `svgelements-1.9.2/test/test_point.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_repr.py` & `svgelements-1.9.2/test/test_repr.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_shape.py` & `svgelements-1.9.2/test/test_shape.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_stroke_width.py` & `svgelements-1.9.2/test/test_stroke_width.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_text.py` & `svgelements-1.9.2/test/test_text.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_use.py` & `svgelements-1.9.2/test/test_use.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_viewbox.py` & `svgelements-1.9.2/test/test_viewbox.py`

 * *Files identical despite different names*

### Comparing `svgelements-1.9.1/test/test_write.py` & `svgelements-1.9.2/test/test_write.py`

 * *Files identical despite different names*

