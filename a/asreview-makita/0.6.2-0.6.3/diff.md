# Comparing `tmp/asreview-makita-0.6.2.tar.gz` & `tmp/asreview-makita-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asreview-makita-0.6.2.tar", last modified: Thu Jan 19 11:18:32 2023, max compression
+gzip compressed data, was "asreview-makita-0.6.3.tar", last modified: Mon Apr 17 20:08:05 2023, max compression
```

## Comparing `asreview-makita-0.6.2.tar` & `asreview-makita-0.6.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:18:32.878081 asreview-makita-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-01-19 11:18:32.878081 asreview-makita-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:18:32.878081 asreview-makita-0.6.2/asreview_makita.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-01-19 11:18:32.000000 asreview-makita-0.6.2/asreview_makita.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-19 11:18:32.000000 asreview-makita-0.6.2/asreview_makita.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 11:18:32.000000 asreview-makita-0.6.2/asreview_makita.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-19 11:18:32.000000 asreview-makita-0.6.2/asreview_makita.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-19 11:18:32.000000 asreview-makita-0.6.2/asreview_makita.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-19 11:18:32.000000 asreview-makita-0.6.2/asreview_makita.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:18:32.878081 asreview-makita-0.6.2/asreviewcontrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:18:32.882081 asreview-makita-0.6.2/asreviewcontrib/makita/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-19 11:18:32.882081 asreview-makita-0.6.2/asreviewcontrib/makita/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/template_arfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/template_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/template_multiple_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 11:18:32.878081 asreview-makita-0.6.2/asreviewcontrib/makita/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/doc_README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_get_plot.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_merge_descriptives.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_merge_metrics.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_merge_tds.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/template_arfi.txt.template
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/template_basic.txt.template
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/templates/template_multiple_models.txt.template
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-01-19 11:18:26.000000 asreview-makita-0.6.2/asreviewcontrib/makita/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-19 11:18:32.882081 asreview-makita-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-01-19 11:18:27.000000 asreview-makita-0.6.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-01-19 11:18:27.000000 asreview-makita-0.6.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:08:05.180390 asreview-makita-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-17 20:08:05.184390 asreview-makita-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:08:05.180390 asreview-makita-0.6.3/asreview_makita.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-17 20:08:05.000000 asreview-makita-0.6.3/asreview_makita.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-17 20:08:05.000000 asreview-makita-0.6.3/asreview_makita.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:08:05.000000 asreview-makita-0.6.3/asreview_makita.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 20:08:05.000000 asreview-makita-0.6.3/asreview_makita.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-17 20:08:05.000000 asreview-makita-0.6.3/asreview_makita.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-17 20:08:05.000000 asreview-makita-0.6.3/asreview_makita.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:08:05.176390 asreview-makita-0.6.3/asreviewcontrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:08:05.184390 asreview-makita-0.6.3/asreviewcontrib/makita/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-17 20:08:05.184390 asreview-makita-0.6.3/asreviewcontrib/makita/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/template_arfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/template_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/template_multiple_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:08:05.180390 asreview-makita-0.6.3/asreviewcontrib/makita/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/doc_README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_get_plot.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_merge_descriptives.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_merge_metrics.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_merge_tds.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/template_arfi.txt.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/template_basic.txt.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/templates/template_multiple_models.txt.template
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-17 20:07:58.000000 asreview-makita-0.6.3/asreviewcontrib/makita/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-17 20:08:05.184390 asreview-makita-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-17 20:07:59.000000 asreview-makita-0.6.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-17 20:07:59.000000 asreview-makita-0.6.3/versioneer.py
```

### Comparing `asreview-makita-0.6.2/LICENSE` & `asreview-makita-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/PKG-INFO` & `asreview-makita-0.6.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,11 @@
-Metadata-Version: 2.1
-Name: asreview-makita
-Version: 0.6.2
-Summary: Makita workflow tool for the ASReview project
-Home-page: https://github.com/asreview/asreview-makita
-Author: ASReview LAB developers
-Author-email: asreview@uu.nl
-Project-URL: Bug Reports, https://github.com/asreview/asreview-makita/issues
-Project-URL: Source, https://github.com/asreview/asreview-makita
-Keywords: asreview makita
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ASReview Makita
 
+[![PyPI version](https://badge.fury.io/py/asreview-makita.svg)](https://badge.fury.io/py/asreview-makita) [![Downloads](https://pepy.tech/badge/asreview-makita)](https://pepy.tech/project/asreview-makita) ![PyPI - License](https://img.shields.io/pypi/l/asreview-makita) ![Deploy and release](https://github.com/asreview/asreview-makita/workflows/Deploy%20and%20release/badge.svg) ![Build status](https://github.com/asreview/asreview-makita/workflows/test-suite/badge.svg) [![DOI](https://zenodo.org/badge/530642619.svg)](https://zenodo.org/badge/latestdoi/530642619)
+
 [ASReviews](https://github.com/asreview/asreview)' Makita (**MAK**e **IT** **A**utomatic) is a workflow generator for simulation studies using the command line interface of [ASReview
 LAB](https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita can be used to effortlessly generate the framework and code for your simulation study.
 
 A simulation involves mimicking the screening process for a systematic review of a human in interaction with an Active learning model (i.e., a combination of a feature extractor, classifier,
 balancing method, and a query strategy). The simulation reenacts the screening process as if a researcher were using active learning. The performance of one or multiple model(s) can then be
 measured by performance metrics, such as the Work Saved over Sampling, recall at a given point in the screening process, or the average time to discover a relevant record.
```

### Comparing `asreview-makita-0.6.2/README.md` & `asreview-makita-0.6.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,30 @@
+Metadata-Version: 2.1
+Name: asreview-makita
+Version: 0.6.3
+Summary: Makita workflow tool for the ASReview project
+Home-page: https://github.com/asreview/asreview-makita
+Author: ASReview LAB developers
+Author-email: asreview@uu.nl
+Project-URL: Bug Reports, https://github.com/asreview/asreview-makita/issues
+Project-URL: Source, https://github.com/asreview/asreview-makita
+Keywords: asreview makita
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ASReview Makita
 
+[![PyPI version](https://badge.fury.io/py/asreview-makita.svg)](https://badge.fury.io/py/asreview-makita) [![Downloads](https://pepy.tech/badge/asreview-makita)](https://pepy.tech/project/asreview-makita) ![PyPI - License](https://img.shields.io/pypi/l/asreview-makita) ![Deploy and release](https://github.com/asreview/asreview-makita/workflows/Deploy%20and%20release/badge.svg) ![Build status](https://github.com/asreview/asreview-makita/workflows/test-suite/badge.svg) [![DOI](https://zenodo.org/badge/530642619.svg)](https://zenodo.org/badge/latestdoi/530642619)
+
 [ASReviews](https://github.com/asreview/asreview)' Makita (**MAK**e **IT** **A**utomatic) is a workflow generator for simulation studies using the command line interface of [ASReview
 LAB](https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita can be used to effortlessly generate the framework and code for your simulation study.
 
 A simulation involves mimicking the screening process for a systematic review of a human in interaction with an Active learning model (i.e., a combination of a feature extractor, classifier,
 balancing method, and a query strategy). The simulation reenacts the screening process as if a researcher were using active learning. The performance of one or multiple model(s) can then be
 measured by performance metrics, such as the Work Saved over Sampling, recall at a given point in the screening process, or the average time to discover a relevant record.
```

### Comparing `asreview-makita-0.6.2/asreview_makita.egg-info/PKG-INFO` & `asreview-makita-0.6.3/asreview_makita.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asreview-makita
-Version: 0.6.2
+Version: 0.6.3
 Summary: Makita workflow tool for the ASReview project
 Home-page: https://github.com/asreview/asreview-makita
 Author: ASReview LAB developers
 Author-email: asreview@uu.nl
 Project-URL: Bug Reports, https://github.com/asreview/asreview-makita/issues
 Project-URL: Source, https://github.com/asreview/asreview-makita
 Keywords: asreview makita
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ASReview Makita
 
+[![PyPI version](https://badge.fury.io/py/asreview-makita.svg)](https://badge.fury.io/py/asreview-makita) [![Downloads](https://pepy.tech/badge/asreview-makita)](https://pepy.tech/project/asreview-makita) ![PyPI - License](https://img.shields.io/pypi/l/asreview-makita) ![Deploy and release](https://github.com/asreview/asreview-makita/workflows/Deploy%20and%20release/badge.svg) ![Build status](https://github.com/asreview/asreview-makita/workflows/test-suite/badge.svg) [![DOI](https://zenodo.org/badge/530642619.svg)](https://zenodo.org/badge/latestdoi/530642619)
+
 [ASReviews](https://github.com/asreview/asreview)' Makita (**MAK**e **IT** **A**utomatic) is a workflow generator for simulation studies using the command line interface of [ASReview
 LAB](https://asreview.readthedocs.io/en/latest/simulation_cli.html). Makita can be used to effortlessly generate the framework and code for your simulation study.
 
 A simulation involves mimicking the screening process for a systematic review of a human in interaction with an Active learning model (i.e., a combination of a feature extractor, classifier,
 balancing method, and a query strategy). The simulation reenacts the screening process as if a researcher were using active learning. The performance of one or multiple model(s) can then be
 measured by performance metrics, such as the Work Saved over Sampling, recall at a given point in the screening process, or the average time to discover a relevant record.
```

### Comparing `asreview-makita-0.6.2/asreview_makita.egg-info/SOURCES.txt` & `asreview-makita-0.6.3/asreview_makita.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/entrypoint.py` & `asreview-makita-0.6.3/asreviewcontrib/makita/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         return True
     else:
         raise ValueError(f"Template {fp} not found")
 
 
 def _valid_job_file(param):
     ext = Path(param).suffix
-    if ext.lower() not in ('.sh', '.bat'):
-        raise argparse.ArgumentTypeError('File must have a .sh or .bat extension')
+    if ext.lower() not in ('.sh', '.bat', '.yaml'):
+        raise argparse.ArgumentTypeError('File must have a .sh, .bat, .yaml extension')
     return param
 
 
 def _shell_to_batch(job):
     job = f'@ echo off\nCOLOR E0{job}'
     job = job.replace('#', '::')
     job = job.replace('/', '\\')
```

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/template_arfi.py` & `asreview-makita-0.6.3/asreviewcontrib/makita/template_arfi.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,45 +51,51 @@
     params = []
 
     for i, fp_dataset in enumerate(sorted(datasets)):
 
         check_filename_dataset(fp_dataset)
 
         # render priors
-        priors = get_priors(fp_dataset, init_seed=init_seed + i, n_priors=n_priors)
+        priors = get_priors(fp_dataset,
+                            init_seed=init_seed + i,
+                            n_priors=n_priors
+                            )
 
         # params for single dataset
         params.append(
             {
                 "input_file": fp_dataset.as_posix(),
                 "input_file_stem": fp_dataset.stem,
                 "priors": priors,
                 "model_seed": model_seed + i,
             }
         )
 
     # open template TODO@{Replace by more sustainable module}
     template = ConfigTemplate(fp_template)
 
-    for s in template.scripts:
-        t_script = get_file(s, "script")
-        export_fp = Path(scripts_folder, s)
-        add_file(t_script, export_fp)
-
-    for s in template.docs:
-        t_docs = get_file(s,
-                          "doc",
-                          datasets=datasets,
-                          template_name=template.name if template.name == "ARFI" else "custom", # NOQA
-                          template_name_long=template.name_long,
-                          template_scripts=template.scripts,
-                          output_folder=output_folder,
-                          job_file=job_file,
-                          )
-        add_file(t_docs, s)
+    # check if template.script is not NoneType
+    if template.scripts is not None:
+        for s in template.scripts:
+            t_script = get_file(s, "script")
+            export_fp = Path(scripts_folder, s)
+            add_file(t_script, export_fp)
+
+    if template.docs is not None:
+        for s in template.docs:
+            t_docs = get_file(s,
+                              "doc",
+                              datasets=datasets,
+                              template_name=template.name if template.name == "ARFI" else "custom",  # NOQA
+                              template_name_long=template.name_long,
+                              template_scripts=template.scripts,
+                              output_folder=output_folder,
+                              job_file=job_file,
+                              )
+            add_file(t_docs, s)
 
     return template.render(
         {
             "datasets": params,
             "init_seed": init_seed,
             "output_folder": output_folder,
             "scripts_folder": scripts_folder,
```

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/template_basic.py` & `asreview-makita-0.6.3/asreviewcontrib/makita/template_basic.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/template_multiple_models.py` & `asreview-makita-0.6.3/asreviewcontrib/makita/template_multiple_models.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/doc_README.md.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/doc_README.md.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_get_plot.py.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_get_plot.py.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_get_settings_from_state.py.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_merge_descriptives.py.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_merge_descriptives.py.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_merge_metrics.py.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_merge_metrics.py.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_merge_tds.py.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_merge_tds.py.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/script_split_data_with_multiple_labels.py.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/template_arfi.txt.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/template_arfi.txt.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/template_basic.txt.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/template_basic.txt.template`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives/wordcloud_{{ dataset.input_file_stem }}.png --width 800 --height 500
 asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives/wordcloud_relevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --relevant
 asreview wordcloud {{ dataset.input_file }} -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/descriptives/wordcloud_irrelevant_{{ dataset.input_file_stem }}.png --width 800 --height 500 --irrelevant
 
 # Simulate runs
 mkdir {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files
 {% for run in range(dataset.n_runs) %}
-asreview simulate {{ dataset.input_file }} -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ run }}.asreview --init_seed {{ dataset.init_seed }} --seed {{ dataset.model_seed }}
+asreview simulate {{ dataset.input_file }} -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ run }}.asreview --init_seed {{ dataset.init_seed + run}} --seed {{ dataset.model_seed + run}}
 asreview metrics {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/sim_{{ dataset.input_file_stem }}_{{ run }}.asreview -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/metrics/metrics_sim_{{ dataset.input_file_stem }}_{{ run }}.json
 {% endfor %}
 
 # Generate plot for dataset
 python {{ scripts_folder }}/get_plot.py -s {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/state_files/ -o {{ output_folder }}/simulation/{{ dataset.input_file_stem }}/plot_recall_sim_{{ dataset.input_file_stem }}.png
 {% endfor %}
```

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/templates/template_multiple_models.txt.template` & `asreview-makita-0.6.3/asreviewcontrib/makita/templates/template_multiple_models.txt.template`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/asreviewcontrib/makita/utils.py` & `asreview-makita-0.6.3/asreviewcontrib/makita/utils.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/setup.py` & `asreview-makita-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `asreview-makita-0.6.2/versioneer.py` & `asreview-makita-0.6.3/versioneer.py`

 * *Files identical despite different names*

