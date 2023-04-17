# Comparing `tmp/enstools-2023.1.tar.gz` & `tmp/enstools-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enstools-2023.1.tar", last modified: Wed Jan 18 17:18:57 2023, max compression
+gzip compressed data, was "enstools-2023.4.tar", last modified: Mon Apr 17 13:19:59 2023, max compression
```

## Comparing `enstools-2023.1.tar` & `enstools-2023.4.tar`

### file list

```diff
@@ -1,87 +1,17 @@
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    10898 2023-01-18 17:18:55.000000 enstools-2023.1/LICENSE
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       15 2023-01-18 17:18:55.000000 enstools-2023.1/MANIFEST.in
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1486 2023-01-18 17:18:57.000000 enstools-2023.1/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1256 2023-01-18 17:18:55.000000 enstools-2023.1/README.md
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        7 2023-01-18 17:18:55.000000 enstools-2023.1/VERSION
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      232 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/api.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/clustering/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      122 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/clustering/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3337 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/clustering/preparation.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     4641 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/clustering/wrapper.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/core/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    28494 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/core/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    13652 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/core/batchjob.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     6383 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/core/cluster.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      324 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/core/errors.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     8307 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/core/os_support.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     5956 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/core/parallelisation.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1970 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/core/tempdir.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/filters/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     4076 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/filters/DCT2D.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       34 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/filters/__init__.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/interpolation/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      150 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/interpolation/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      757 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/interpolation/coarse_graining.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    11307 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/interpolation/nearest_neighbour_interpolator.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     9515 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/interpolation/vertical_interpolation.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/io/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      949 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2623 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/dataset.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/io/eccodes/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    21996 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/eccodes/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    25816 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/eccodes/eccodes_cffi.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1604 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/file_type.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1180 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/paths.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    22789 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/reader.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     6962 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/io/writer.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/misc/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    14839 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/misc/__init__.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/opendata/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    35717 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/opendata/DWDContent.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    19964 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/opendata/DWDRadar.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      154 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/opendata/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     9419 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/opendata/cli.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1825 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/opendata/retrieve_nwp.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1132 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/opendata/retrieve_radar.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/plot/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      141 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    19189 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/core.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3809 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/ensemble.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/plot/interactive/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    35423 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/interactive/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    16919 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/interactive/backend.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)    15765 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/interactive/backend3D.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     6881 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/interactive/backend_bokeh.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     5204 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/plot/interactive/backend_plotly.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/post/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     4069 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/post/ConvectiveAdjustmentTimescale.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1839 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/post/EnsembleStat.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     5117 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/post/Vorticity.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      184 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/post/__init__.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/scores/
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools/scores/DisplacementAmplitudeScore/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3764 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/DisplacementAmplitudeScore/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3742 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/DisplacementAmplitudeScore/calc_das.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     6744 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/DisplacementAmplitudeScore/match_pyramid_ic.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2235 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/__init__.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3145 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/continuous_ranked_probability_score.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      762 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/fix_attributes.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3060 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/kolmogorov_smirnov.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2998 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/kolmogorov_smirnov_multicell.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     3526 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/normalized_root_mean_square_error.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1144 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/peak_signal_to_noise_ratio.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2087 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/pearson_correlation.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      615 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/positivity.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2657 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/structural_similarity_index.py
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      545 2023-01-18 17:18:55.000000 enstools-2023.1/enstools/scores/template.py
-drwxr-xr-x   0 oriol.tinto (24207) ls-craig (11075)        0 2023-01-18 17:18:57.000000 enstools-2023.1/enstools.egg-info/
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1486 2023-01-18 17:18:56.000000 enstools-2023.1/enstools.egg-info/PKG-INFO
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     2221 2023-01-18 17:18:56.000000 enstools-2023.1/enstools.egg-info/SOURCES.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        1 2023-01-18 17:18:56.000000 enstools-2023.1/enstools.egg-info/dependency_links.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       65 2023-01-18 17:18:56.000000 enstools-2023.1/enstools.egg-info/entry_points.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)      251 2023-01-18 17:18:56.000000 enstools-2023.1/enstools.egg-info/requires.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)        9 2023-01-18 17:18:56.000000 enstools-2023.1/enstools.egg-info/top_level.txt
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)       38 2023-01-18 17:18:57.000000 enstools-2023.1/setup.cfg
--rw-r--r--   0 oriol.tinto (24207) ls-craig (11075)     1981 2023-01-18 17:18:55.000000 enstools-2023.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:19:59.416557 enstools-2023.4/
+-rw-rw-rw-   0 root         (0) root         (0)    10898 2022-12-23 06:03:14.000000 enstools-2023.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       15 2022-12-23 06:03:14.000000 enstools-2023.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-04-17 13:19:59.416557 enstools-2023.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2022-12-23 06:03:14.000000 enstools-2023.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-17 12:40:25.000000 enstools-2023.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:19:59.415557 enstools-2023.4/enstools/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2022-12-23 06:03:14.000000 enstools-2023.4/enstools/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 13:19:59.415557 enstools-2023.4/enstools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-04-17 13:19:59.000000 enstools-2023.4/enstools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-17 13:19:59.000000 enstools-2023.4/enstools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 13:19:59.000000 enstools-2023.4/enstools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-17 13:19:59.000000 enstools-2023.4/enstools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-04-17 13:19:59.000000 enstools-2023.4/enstools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 13:19:59.000000 enstools-2023.4/enstools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 13:19:59.416557 enstools-2023.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2022-12-23 06:03:14.000000 enstools-2023.4/setup.py
```

### Comparing `enstools-2023.1/LICENSE` & `enstools-2023.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enstools-2023.1/PKG-INFO` & `enstools-2023.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: enstools
-Version: 2023.1
-Home-page: https://github.com/wavestoweather/enstools
-Author: Robert Redl et al.
-Author-email: robert.redl@lmu.de
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ensemble Tools [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools.readthedocs.io/en/latest/?badge=latest)
 
 This package provides core functionality to Python-based tools developed within
 the framework of [Waves to Weather - Transregional Collaborative Research 
 Project (SFB/TRR165)](https://wavestoweather.de). 
 
 Shared functionality includes:
```

### Comparing `enstools-2023.1/README.md` & `enstools-2023.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: enstools
+Version: 2023.4
+Summary: UNKNOWN
+Home-page: https://github.com/wavestoweather/enstools
+Author: Robert Redl et al.
+Author-email: robert.redl@lmu.de
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Ensemble Tools [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools.readthedocs.io/en/latest/?badge=latest)
 
 This package provides core functionality to Python-based tools developed within
 the framework of [Waves to Weather - Transregional Collaborative Research 
 Project (SFB/TRR165)](https://wavestoweather.de). 
 
 Shared functionality includes:
@@ -30,7 +42,9 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
+
+
```

### Comparing `enstools-2023.1/enstools.egg-info/PKG-INFO` & `enstools-2023.4/enstools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: enstools
-Version: 2023.1
+Version: 2023.4
+Summary: UNKNOWN
 Home-page: https://github.com/wavestoweather/enstools
 Author: Robert Redl et al.
 Author-email: robert.redl@lmu.de
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ensemble Tools [![Documentation Status](https://readthedocs.org/projects/enstools/badge/?version=latest)](https://enstools.readthedocs.io/en/latest/?badge=latest)
 
 This package provides core functionality to Python-based tools developed within
 the framework of [Waves to Weather - Transregional Collaborative Research 
@@ -39,7 +42,9 @@
 Waves to Weather (SFB/TRR165) coordinated by the subproject 
 [Z2](https://www.wavestoweather.de/research_areas/phase2/z2) and funded by the
 German Research Foundation (DFG).
 
 A full list of code contributors can [CONTRIBUTORS.md](./CONTRIBUTORS.md).
 
 The code is released under an [Apache-2.0 licence](./LICENSE).
+
+
```

### Comparing `enstools-2023.1/setup.py` & `enstools-2023.4/setup.py`

 * *Files identical despite different names*

