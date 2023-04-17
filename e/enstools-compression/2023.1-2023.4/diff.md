# Comparing `tmp/enstools-compression-2023.1.tar.gz` & `tmp/enstools-compression-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstools-compression-2023.1.tar", last modified: Wed Jan 18 17:53:24 2023, max compression
+gzip compressed data, was "enstools-compression-2023.4.tar", last modified: Mon Apr 17 15:44:23 2023, max compression
```

## Comparing `enstools-compression-2023.1.tar` & `enstools-compression-2023.4.tar`

### file list

```diff
@@ -1,42 +1,15 @@
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    10898 2023-01-18 17:53:22.000000 enstools-compression-2023.1/LICENSE
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       15 2023-01-18 17:53:22.000000 enstools-compression-2023.1/MANIFEST.in
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1660 2023-01-18 17:53:24.000000 enstools-compression-2023.1/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1412 2023-01-18 17:53:22.000000 enstools-compression-2023.1/README.md
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        7 2023-01-18 17:53:22.000000 enstools-compression-2023.1/VERSION
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      444 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/__init__.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/analyzer/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3099 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/AnalysisOptions.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       53 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     6293 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/analyze_data_array.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)    10373 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/analyzer.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     8194 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/analyzer/analyzer_utils.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      344 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/api.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    16861 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/cli.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)    11172 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/compressor.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)     3354 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulation.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/emulators/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1188 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/EmulatorClass.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2353 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/FiltersEmulator.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)     2885 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/LibpressioEmulator.py
--rwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)     2036 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/ZFPEmulator.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      197 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/emulators/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2715 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/evaluator.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    11156 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/metrics.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     4557 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/pruner.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    10801 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/significant_bits.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      910 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/size_metrics.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools/compression/xr_accessor/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       23 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/xr_accessor/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     5314 2023-01-18 17:53:22.000000 enstools-compression-2023.1/enstools/compression/xr_accessor/accessor.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1660 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1208 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/SOURCES.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        1 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/dependency_links.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       71 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/entry_points.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       74 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/requires.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        9 2023-01-18 17:53:24.000000 enstools-compression-2023.1/enstools_compression.egg-info/top_level.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       38 2023-01-18 17:53:24.000000 enstools-compression-2023.1/setup.cfg
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1366 2023-01-18 17:53:22.000000 enstools-compression-2023.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:44:23.756658 enstools-compression-2023.4/
+-rw-rw-rw-   0 root         (0) root         (0)    10898 2023-01-18 16:33:07.000000 enstools-compression-2023.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-18 16:33:07.000000 enstools-compression-2023.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-17 15:44:23.755658 enstools-compression-2023.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-01-18 16:33:07.000000 enstools-compression-2023.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-17 13:09:12.000000 enstools-compression-2023.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:44:23.755658 enstools-compression-2023.4/enstools_compression.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-17 15:44:23.000000 enstools-compression-2023.4/enstools_compression.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-17 15:44:23.000000 enstools-compression-2023.4/enstools_compression.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:44:23.000000 enstools-compression-2023.4/enstools_compression.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-17 15:44:23.000000 enstools-compression-2023.4/enstools_compression.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-04-17 15:44:23.000000 enstools-compression-2023.4/enstools_compression.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:44:23.000000 enstools-compression-2023.4/enstools_compression.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 15:44:23.756658 enstools-compression-2023.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-01-18 16:33:07.000000 enstools-compression-2023.4/setup.py
```

### Comparing `enstools-compression-2023.1/LICENSE` & `enstools-compression-2023.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enstools-compression-2023.1/PKG-INFO` & `enstools-compression-2023.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: enstools-compression
-Version: 2023.1
-Home-page: https://github.com/wavestoweather/enstools-compression
-Author: Oriol Tintó
-Author-email: oriol.tinto@lmu.de
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
 
 
 This package extends [enstools](github.com/wavestoweather/enstools) to enable **lossy** and **lossless** compression 
 by using **HDF5 filters**.
 
 Also, it contains a set of tools to help to find appropriate compression specifications.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `enstools-compression-2023.1/README.md` & `enstools-compression-2023.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: enstools-compression
+Version: 2023.4
+Summary: UNKNOWN
+Home-page: https://github.com/wavestoweather/enstools-compression
+Author: Oriol Tintó
+Author-email: oriol.tinto@lmu.de
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
 
 
 This package extends [enstools](github.com/wavestoweather/enstools) to enable **lossy** and **lossless** compression 
 by using **HDF5 filters**.
 
 Also, it contains a set of tools to help to find appropriate compression specifications.
@@ -32,7 +44,9 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `enstools-compression-2023.1/enstools_compression.egg-info/PKG-INFO` & `enstools-compression-2023.4/enstools_compression.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: enstools-compression
-Version: 2023.1
+Version: 2023.4
+Summary: UNKNOWN
 Home-page: https://github.com/wavestoweather/enstools-compression
 Author: Oriol Tintó
 Author-email: oriol.tinto@lmu.de
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # enstools-compression [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools-compression.readthedocs.io/en/latest/?badge=latest)
 
 
 This package extends [enstools](github.com/wavestoweather/enstools) to enable **lossy** and **lossless** compression 
@@ -41,7 +44,9 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
+
+
```

### Comparing `enstools-compression-2023.1/setup.py` & `enstools-compression-2023.4/setup.py`

 * *Files identical despite different names*

