# Comparing `tmp/pdstools-3.1.2.tar.gz` & `tmp/pdstools-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdstools-3.1.2.tar", last modified: Thu Apr 13 09:48:24 2023, max compression
+gzip compressed data, was "pdstools-3.1.3.tar", last modified: Mon Apr 17 14:44:19 2023, max compression
```

## Comparing `pdstools-3.1.2.tar` & `pdstools-3.1.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.872912 pdstools-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 09:48:12.000000 pdstools-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-13 09:48:24.872912 pdstools-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-13 09:48:12.000000 pdstools-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.868912 pdstools-3.1.2/pdstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-13 09:48:24.000000 pdstools-3.1.2/pdstools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-13 09:48:24.000000 pdstools-3.1.2/pdstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:48:24.000000 pdstools-3.1.2/pdstools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 09:48:24.000000 pdstools-3.1.2/pdstools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-13 09:48:24.000000 pdstools-3.1.2/pdstools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 09:48:24.000000 pdstools-3.1.2/pdstools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-13 09:48:12.000000 pdstools-3.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.868912 pdstools-3.1.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.868912 pdstools-3.1.2/python/pdstools/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.868912 pdstools-3.1.2/python/pdstools/adm/
--rw-r--r--   0 runner    (1001) docker     (123)    57683 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/adm/ADMDatamart.py
--rw-r--r--   0 runner    (1001) docker     (123)    40057 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/adm/ADMTrees.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/adm/Tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/adm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.868912 pdstools-3.1.2/python/pdstools/app/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/app/Home.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/app/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.868912 pdstools-3.1.2/python/pdstools/app/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/app/pages/Health Check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.872912 pdstools-3.1.2/python/pdstools/ih/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/ih/IHAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/ih/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/ih/legacy_IH.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.872912 pdstools-3.1.2/python/pdstools/pega_io/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/pega_io/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    13543 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/pega_io/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/pega_io/S3.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/pega_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.872912 pdstools-3.1.2/python/pdstools/plots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/plots/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/plots/plots_plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.872912 pdstools-3.1.2/python/pdstools/reports/
--rw-r--r--   0 runner    (1001) docker     (123)    39142 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/reports/HealthCheck.qmd
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/reports/HealthCheckModel.qmd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.872912 pdstools-3.1.2/python/pdstools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/cdh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/hds_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/pega_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/polars_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/streamlit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:24.872912 pdstools-3.1.2/python/pdstools/valuefinder/
--rw-r--r--   0 runner    (1001) docker     (123)    24211 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/valuefinder/ValueFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:48:12.000000 pdstools-3.1.2/python/pdstools/valuefinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 09:48:24.872912 pdstools-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.237483 pdstools-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-17 14:44:07.000000 pdstools-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-17 14:44:19.237483 pdstools-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-17 14:44:07.000000 pdstools-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.233483 pdstools-3.1.3/pdstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-17 14:44:19.000000 pdstools-3.1.3/pdstools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-17 14:44:19.000000 pdstools-3.1.3/pdstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:44:19.000000 pdstools-3.1.3/pdstools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-17 14:44:19.000000 pdstools-3.1.3/pdstools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 14:44:19.000000 pdstools-3.1.3/pdstools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 14:44:19.000000 pdstools-3.1.3/pdstools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-17 14:44:08.000000 pdstools-3.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.233483 pdstools-3.1.3/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.233483 pdstools-3.1.3/python/pdstools/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.233483 pdstools-3.1.3/python/pdstools/adm/
+-rw-r--r--   0 runner    (1001) docker     (123)    56177 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/adm/ADMDatamart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40060 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/adm/ADMTrees.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/adm/Tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/adm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.233483 pdstools-3.1.3/python/pdstools/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/app/Home.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/app/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.233483 pdstools-3.1.3/python/pdstools/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/app/pages/Health Check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.237483 pdstools-3.1.3/python/pdstools/ih/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/ih/IHAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/ih/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/ih/legacy_IH.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.237483 pdstools-3.1.3/python/pdstools/pega_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/pega_io/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14118 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/pega_io/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/pega_io/S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/pega_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.237483 pdstools-3.1.3/python/pdstools/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51016 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/plots/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29608 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/plots/plots_plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.237483 pdstools-3.1.3/python/pdstools/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)    39159 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/reports/HealthCheck.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/reports/HealthCheckModel.qmd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.237483 pdstools-3.1.3/python/pdstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/cdh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/hds_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/pega_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/polars_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/streamlit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/table_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:19.237483 pdstools-3.1.3/python/pdstools/valuefinder/
+-rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/valuefinder/ValueFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:44:08.000000 pdstools-3.1.3/python/pdstools/valuefinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:44:19.237483 pdstools-3.1.3/setup.cfg
```

### Comparing `pdstools-3.1.2/LICENSE` & `pdstools-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/PKG-INFO` & `pdstools-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.2
+Version: 3.1.3
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.2 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.3 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.2/README.md` & `pdstools-3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/pdstools.egg-info/PKG-INFO` & `pdstools-3.1.3/pdstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdstools
-Version: 3.1.2
+Version: 3.1.3
 Summary: Open source tooling that helps Data Scientists to analyze Pega models and conduct impactful analyses.
 Author-email: Stijn Kas <stijn.kas@pega.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pegasystems/pega-datascientist-tools
 Project-URL: Bug Tracker, https://github.com/pegasystems/pega-datascientist-tools/issues
 Project-URL: Wiki, https://github.com/pegasystems/pega-datascientist-tools/wiki
 Project-URL: Docs, https://pegasystems.github.io/pega-datascientist-tools/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdstools Version: 3.1.2 Summary: Open source
+Metadata-Version: 2.1 Name: pdstools Version: 3.1.3 Summary: Open source
 tooling that helps Data Scientists to analyze Pega models and conduct impactful
 analyses. Author-email: Stijn Kas
 kas@pega.com> License: Apache-2.0 Project-URL: Homepage, https://github.com/
 pegasystems/pega-datascientist-tools Project-URL: Bug Tracker, https://
 github.com/pegasystems/pega-datascientist-tools/issues Project-URL: Wiki,
 https://github.com/pegasystems/pega-datascientist-tools/wiki Project-URL: Docs,
 https://pegasystems.github.io/pega-datascientist-tools/ Keywords:
```

### Comparing `pdstools-3.1.2/pdstools.egg-info/SOURCES.txt` & `pdstools-3.1.3/pdstools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,10 +34,11 @@
 python/pdstools/utils/datasets.py
 python/pdstools/utils/errors.py
 python/pdstools/utils/hds_utils.py
 python/pdstools/utils/pega_template.py
 python/pdstools/utils/polars_ext.py
 python/pdstools/utils/show_versions.py
 python/pdstools/utils/streamlit_utils.py
+python/pdstools/utils/table_definitions.py
 python/pdstools/utils/types.py
 python/pdstools/valuefinder/ValueFinder.py
 python/pdstools/valuefinder/__init__.py
```

### Comparing `pdstools-3.1.2/pyproject.toml` & `pdstools-3.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "datascientist",
     "tools",
 ]
 dependencies = [
         "plotly>=5.5.0",
         "requests",
         "pydot",
-        "polars>=0.17.0",
+        "polars>=0.17.3",
         "pyarrow",
         "tqdm",
         "pyyaml",
         "aioboto3>=11.0"
     ]
 requires-python = ">=3.8"
```

### Comparing `pdstools-3.1.2/python/pdstools/__init__.py` & `pdstools-3.1.3/python/pdstools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python pdstools"""
 
-__version__ = "3.1.2"
+__version__ = "3.1.3"
 
 from polars import enable_string_cache
 
 enable_string_cache(True)
 
 import sys
 from pathlib import Path
@@ -14,14 +14,15 @@
 from .pega_io import getToken, readClientCredentialFile, readDSExport
 from .pega_io import File, API, S3
 from .utils import cdh_utils, datasets, errors, hds_utils
 from .utils.cdh_utils import defaultPredictorCategorization
 from .utils.show_versions import show_versions
 from .utils.datasets import CDHSample, SampleTrees, SampleValueFinder
 from .utils.hds_utils import Config, DataAnonymization
+from .utils.table_definitions import PegaDefaultTables
 from .valuefinder.ValueFinder import ValueFinder
 from .utils.polars_ext import *
 
 if "streamlit" in sys.modules:
     from .utils import streamlit_utils
 
 __reports__ = Path(__file__).parents[0] / "reports"
```

### Comparing `pdstools-3.1.2/python/pdstools/adm/ADMDatamart.py` & `pdstools-3.1.3/python/pdstools/adm/ADMDatamart.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,15 +286,17 @@
                 BinPropensity=pl.col("BinPositives") / pl.col("BinResponseCount"),
                 BinAdjustedPropensity=(
                     (pl.col("BinPositives") + pl.lit(0.5))
                     / (pl.col("BinResponseCount") + pl.lit(1))
                 ),
             )
             if self.predictorCategorization is not None:
-                df2 = df2.with_columns(PredictorCategory=self.predictorCategorization())
+                if not isinstance(self.predictorCategorization, pl.Expr):
+                    self.predictorCategorization = self.predictorCategorization()
+                df2 = df2.with_columns(PredictorCategory=self.predictorCategorization)
 
         if df1 is not None and df2 is not None:
             total_missing = (
                 set(self.missing_model)
                 & set(self.missing_preds) - set(df1.columns) - set(df2.columns)
             ) - {"Treatment"}
             if len(total_missing) > 0 and verbose:  # pragma: no cover
@@ -376,21 +378,22 @@
         df = cdh_utils._polarsCapitalize(df)
         cols, missing = self._available_columns(
             df, include_cols=include_cols, drop_cols=drop_cols
         )
         if subset:
             df = df.select(cols)
         if extract_keys:
-            df = self._extract_keys(df)
+            df = cdh_utils._extract_keys(df, import_strategy=self.import_strategy)
             df = cdh_utils._polarsCapitalize(df)
 
         df = self._set_types(
             df,
             timestamp_fmt=reading_opts.get("timestamp_fmt", None),
             strict_conversion=reading_opts.get("strict_conversion", True),
+            table=reading_opts.get("typesetting_table", "infer"),
         )
 
         if self.query is not None:
             try:
                 df = self._apply_query(df, self.query)
                 if self.verbose:
                     print(f"Query succesful for {name}.")
@@ -467,64 +470,54 @@
 
         include_cols = default_names.union(include_cols).difference(drop_cols)
         missing = {col for col in include_cols if col not in df.columns}
         to_import = include_cols.intersection(set(df.columns))
 
         return to_import, missing
 
-    @staticmethod
     def _set_types(
+        self,
         df: any_frame,
+        table: str = "infer",
         *,
         timestamp_fmt: str = None,
         strict_conversion: bool = True,
     ) -> any_frame:
         """A method to change columns to their proper type
 
         Parameters
         ----------
         df : Union[pl.DataFrame, pl.LazyFrame]
             The input dataframe
+        table: str
+            The table to set types for. Default is infer, in which case
+            it infers the table type from the columns in it.
 
         Keyword arguments
         -----------------
         timestamp_fmt: str
             The format of Date type columns
         strict_conversion: bool
             Raises an error if timestamp conversion to given/default date format(timestamp_fmt) fails
             See 'https://strftime.org/' for timestamp formats
         Returns
         -------
         Union[pl.DataFrame, pl.LazyFrame]
             The input dataframe, but the proper typing applied
         """
-        from polars.datatypes import Datetime, Date
 
-        retype = {
-            pl.Categorical: ["Issue", "Group", "Channel", "Direction", "Configuration"],
-            # pl.Int64: ["Positives", "Negatives", "ResponseCount"],
-            pl.Float64: ["Performance"],
-        }
-        to_retype = []
-        for type, cols in retype.items():
-            for col in cols:
-                if col in set(df.columns):
-                    to_retype.append(pl.col(col).cast(type))
-        df = df.with_columns(to_retype)
-
-        timestampCol = "SnapshotTime"
-        if timestampCol not in df.columns:
+        df = cdh_utils.set_types(
+            df,
+            table,
+            verbose=self.verbose,
+            timestamp_fmt=timestamp_fmt,
+            strict_conversion=strict_conversion,
+        )
+        if "SnapshotTime" not in df.columns:
             df = df.with_columns(SnapshotTime=None)
-        elif df.schema[timestampCol].base_type() not in {Datetime, Date}:
-            df = df.with_columns(
-                cdh_utils.parsePegaDateTimeFormats(
-                    timestampCol, timestamp_fmt, strict_conversion
-                )
-            )
-
         return df
 
     def last(
         self, table="modelData", strategy: Literal["eager", "lazy"] = "eager"
     ) -> any_frame:
         """Convenience function to get the last values for a table
 
@@ -749,60 +742,14 @@
                 if not type(val) == list:
                     raise ValueError("query values must be list")
 
             for col, val in query.items():
                 df = df.filter(pl.col(col).is_in(val))
         return df
 
-    def _extract_keys(
-        self,
-        df: any_frame,
-    ) -> any_frame:
-        """Extracts keys out of the pyName column
-
-        This is not a lazy operation as we don't know the possible keys
-        in advance. For that reason, we select only the pyName column,
-        extract the keys from that, and then collect the resulting dataframe.
-        This dataframe is then joined back to the original dataframe.
-
-        This is relatively efficient, but we still do need the whole
-        pyName column in memory to do this, so it won't work completely
-        lazily from e.g. s3. That's why it only works with eager mode.
-
-        Parameters
-        ----------
-        df: Union[pl.DataFrame, pl.LazyFrame]
-            The dataframe to extract the keys from
-        """
-        if self.import_strategy != "eager":
-            raise NotEagerError("Extracting keys")
-        if self.verbose:
-            print("Extracting keys...")
-
-        def safeName():
-            return (
-                pl.when(~pl.col("Name").cast(pl.Utf8).str.starts_with("{"))
-                .then(
-                    pl.concat_str([pl.lit('{"pyName":"'), pl.col("Name"), pl.lit('"}')])
-                )
-                .otherwise(pl.col("Name"))
-                .alias("tempName")
-            )
-
-        return df.with_columns(
-            cdh_utils._polarsCapitalize(
-                df.select(
-                    safeName().str.json_extract(),
-                )
-                .unnest("tempName")
-                .lazy()
-                .collect()
-            )
-        )
-
     def discover_modelTypes(
         self, df: pl.LazyFrame, by: str = "Configuration"
     ) -> Dict:  # pragma: no cover
         """Discovers the type of model embedded in the pyModelData column.
 
         By default, we do a groupby Configuration, because a model rule can only
         contain one type of model. Then, for each configuration, we look into the
@@ -958,15 +905,20 @@
             )
             .groupby_dynamic("SnapshotTime", every=every, by=by)
             .agg(pl.sum("Daily_increase").alias("Increase"))
         )
         if pivot:
             df = (
                 df.collect()
-                .pivot(index="SnapshotTime", columns=by, values="Increase")
+                .pivot(
+                    index="SnapshotTime",
+                    columns=by,
+                    values="Increase",
+                    aggregate_function="first",
+                )
                 .lazy()
             )
         if mask:
             df = df.with_columns((pl.all().exclude([by, "SnapshotTime"]).sign()))
         return df
 
     def model_summary(
@@ -1078,15 +1030,20 @@
             df = (
                 df.with_columns(pl.col("PerformanceBin").fill_nan(0.5))
                 .sort("PerformanceBin", descending=True)
                 .head(top_n)
             )
         df = (
             df.collect()
-            .pivot(index=by, columns="PredictorName", values="PerformanceBin")
+            .pivot(
+                index=by,
+                columns="PredictorName",
+                values="PerformanceBin",
+                aggregate_function="first",
+            )
             .fill_null(0.5)
             .fill_nan(0.5)
         )
         mod_order = (
             df.select(
                 pl.concat_list(pl.col(pl.Float64))
                 .arr.eval(pl.element().mean())
```

### Comparing `pdstools-3.1.2/python/pdstools/adm/ADMTrees.py` & `pdstools-3.1.3/python/pdstools/adm/ADMTrees.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,15 +484,15 @@
         the mean gains, and the number of times the split is performed.
         """
         return (
             self.gainsPerSplit.groupby("split", maintain_order=True)
             .agg(
                 [
                     pl.first("predictor"),
-                    pl.col("gains").list(),
+                    pl.col("gains").implode(),
                     pl.col("gains").mean().alias("mean"),
                     pl.first("split")
                     .apply(lambda x: self.parseSplitValues(x)[1])
                     .alias("sign"),
                     pl.first("split")
                     .apply(lambda x: self.parseSplitValues(x)[2])
                     .alias("values"),
```

### Comparing `pdstools-3.1.2/python/pdstools/adm/Tables.py` & `pdstools-3.1.3/python/pdstools/adm/Tables.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/app/cli.py` & `pdstools-3.1.3/python/pdstools/app/cli.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/app/pages/Health Check.py` & `pdstools-3.1.3/python/pdstools/app/pages/Health Check.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/ih/IHAnalysis.py` & `pdstools-3.1.3/python/pdstools/ih/IHAnalysis.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/ih/legacy_IH.py` & `pdstools-3.1.3/python/pdstools/ih/legacy_IH.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/pega_io/API.py` & `pdstools-3.1.3/python/pdstools/pega_io/API.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/pega_io/File.py` & `pdstools-3.1.3/python/pdstools/pega_io/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,27 +146,36 @@
     -------
     pl.LazyFrame
         The (imported) lazy dataframe
     """
     if extension == ".zip":
         logging.debug("Zip file found, extracting data.json to BytesIO.")
         file, extension = readZippedFile(file)
+    elif extension == ".gz":
+        import gzip
+
+        extension = os.path.splitext(os.path.splitext(file)[0])[1]
+        file = BytesIO(gzip.GzipFile(file).read())
 
     if extension == ".csv":
+        csv_opts = dict(
+            separator=reading_opts.get("sep", ","),
+            infer_schema_length=reading_opts.pop("infer_schema_length", 10000),
+            null_values=["", "NA", "N/A", "NULL"],
+            dtypes={"PYMODELID": pl.Utf8},
+            try_parse_dates=True,
+            ignore_errors=reading_opts.get("ignore_errors", False),
+        )
         if isinstance(file, BytesIO):
             file = pl.read_csv(
                 file,
-                infer_schema_length=reading_opts.pop("infer_schema_length", 10000),
-                try_parse_dates=True,
+                **csv_opts,
             ).lazy()
         else:
-            file = pl.scan_csv(
-                file,
-                separator=reading_opts.get("sep", ","),
-            )
+            file = pl.scan_csv(file, **csv_opts)
 
     elif extension == ".json":
         try:
             if isinstance(file, BytesIO):
                 from pyarrow import json
 
                 file = pl.LazyFrame(
@@ -176,15 +185,21 @@
                 )
             else:
                 file = pl.scan_ndjson(
                     file,
                     infer_schema_length=reading_opts.pop("infer_schema_length", 10000),
                 )
         except:  # pragma: no cover
-            file = pl.read_json(file).lazy()
+            try:
+                file = pl.read_json(file).lazy()
+            except:
+                import json
+
+                with open(file) as f:
+                    file = pl.from_dicts(json.loads(f.read())["pxResults"]).lazy()
 
     elif extension == ".parquet":
         file = pl.scan_parquet(file)
 
     elif extension.casefold() in {".feather", ".ipc", ".arrow"}:
         if isinstance(file, BytesIO):
             file = pl.read_ipc(file).lazy()
@@ -243,15 +258,14 @@
                 )
             with z.open(file) as zippedfile:
                 return (BytesIO(zippedfile.read()), ".json")
         else:  # pragma: no cover
             raise FileNotFoundError("Cannot find a 'data.json' file in the zip folder.")
 
 
-
 def readMultiZip(files: list, zip_type: Literal["gzip"] = "gzip", verbose: bool = True):
     """Reads multiple zipped ndjson files, and concats them to one Polars dataframe.
 
     Parameters
     ----------
     files : list
         The list of files to concat
@@ -269,15 +283,14 @@
         table.append(pl.read_ndjson(gzip.open(file).read()))
     df = pl.concat(table, how="diagonal")
     if verbose:
         print("Combining completed")
     return df
 
 
-
 def get_latest_file(path: str, target: str, verbose: bool = False) -> str:
     """Convenience method to find the latest model snapshot.
     It has a set of default names to search for and finds all files who match it.
     Once it finds all matching files in the directory, it chooses the most recent one.
     Supports [".json", ".csv", ".zip", ".parquet", ".feather", ".ipc"].
     Needs a path to the directory and a target of either 'modelData' or 'predictorData'.
 
@@ -333,14 +346,15 @@
     default_model_names = [
         "Data-Decision-ADM-ModelSnapshot",
         "PR_DATA_DM_ADMMART_MDL_FACT",
         "model_snapshots",
         "MD_FACT",
         "ADMMART_MDL_FACT_Data",
         "cached_modelData",
+        "Models_data",
     ]
     default_predictor_names = [
         "Data-Decision-ADM-PredictorBinningSnapshot",
         "PR_DATA_DM_ADMMART_PRED",
         "predictor_binning_snapshots",
         "PRED_FACT",
         "cached_predictorData",
@@ -398,8 +412,8 @@
         df = df.collect()
     if cache_type == "ipc":
         outpath = f"{outpath}.arrow"
         df.write_ipc(outpath, compression=compression)
     if cache_type == "parquet":
         outpath = f"{outpath}.parquet"
         df.write_parquet(outpath, compression=compression)
-    return outpath
+    return outpath
```

### Comparing `pdstools-3.1.2/python/pdstools/pega_io/S3.py` & `pdstools-3.1.3/python/pdstools/pega_io/S3.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/plots/plot_base.py` & `pdstools-3.1.3/python/pdstools/plots/plot_base.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/plots/plots_plotly.py` & `pdstools-3.1.3/python/pdstools/plots/plots_plotly.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/reports/HealthCheck.qmd` & `pdstools-3.1.3/python/pdstools/reports/HealthCheck.qmd`

 * *Files 1% similar despite different names*

```diff
@@ -854,15 +854,15 @@
 
 So when one of the graphs shows more volume on the left, that is to be interpreted as relative to the other graphs.
 
 ```{python}
 to_plot = "Propensity"
 if to_plot == "Propensity" and to_plot not in datamart.predictorData.columns:
     to_plot = "BinPropensity"
-df = datamart.combinedData.filter(pl.col("PredictorName")!="Classifier").groupby([to_plot, "Channel", "Direction"]).agg(pl.sum("BinResponseCount")).with_columns(pl.col(to_plot).round(4)).collect()
+df = datamart.combinedData.filter(pl.col("PredictorName")!="Classifier").groupby([to_plot, "Channel", "Direction"]).agg(pl.sum("BinResponseCount")).with_columns(pl.col(to_plot).round(4).cast(pl.Float64)).collect()
 color_col = "Channel"
 smallest_bin = 0
 
 for color in df.get_column(color_col).unique().to_list():
     color_df = df.filter(pl.col(color_col) == color)
     propensity_list = list(set(color_df.select(to_plot).fill_null(0).fill_nan(0).filter(pl.col(to_plot)>0).get_column(to_plot).to_list()))
     if len(propensity_list) > 0:
```

### Comparing `pdstools-3.1.2/python/pdstools/reports/HealthCheckModel.qmd` & `pdstools-3.1.3/python/pdstools/reports/HealthCheckModel.qmd`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/utils/cdh_utils.py` & `pdstools-3.1.3/python/pdstools/utils/cdh_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 """
 
 from typing import List, Union
 import polars as pl
 import re
 import numpy as np
 import datetime
+from .types import any_frame
+from .errors import NotEagerError
+from .table_definitions import PegaDefaultTables
 
 import pytz
 
 
 def defaultPredictorCategorization(
     x: Union[str, pl.Expr] = pl.col("PredictorName")
 ) -> pl.Expr:
@@ -42,14 +45,59 @@
     return (
         pl.when(x.str.split(".").arr.lengths() > 1)
         .then(x.str.split(".").arr.get(0))
         .otherwise(pl.lit("Primary"))
     ).alias("PredictorCategory")
 
 
+def _extract_keys(
+    df: any_frame,
+    col="Name",
+    capitalize=True,
+    import_strategy="eager",
+) -> any_frame:
+    """Extracts keys out of the pyName column
+
+    This is not a lazy operation as we don't know the possible keys
+    in advance. For that reason, we select only the pyName column,
+    extract the keys from that, and then collect the resulting dataframe.
+    This dataframe is then joined back to the original dataframe.
+
+    This is relatively efficient, but we still do need the whole
+    pyName column in memory to do this, so it won't work completely
+    lazily from e.g. s3. That's why it only works with eager mode.
+
+    Parameters
+    ----------
+    df: Union[pl.DataFrame, pl.LazyFrame]
+        The dataframe to extract the keys from
+    """
+    if import_strategy != "eager":
+        raise NotEagerError("Extracting keys")
+
+    def safeName():
+        return (
+            pl.when(~pl.col(col).cast(pl.Utf8).str.starts_with("{"))
+            .then(pl.concat_str([pl.lit('{"pyName":"'), pl.col(col), pl.lit('"}')]))
+            .otherwise(pl.col(col))
+        ).alias("tempName")
+
+    series = (
+        df.select(
+            safeName().str.json_extract(),
+        )
+        .unnest("tempName")
+        .lazy()
+        .collect()
+    )
+    if not capitalize:
+        return df.with_columns(series)
+    return df.with_columns(_polarsCapitalize(series))
+
+
 def parsePegaDateTimeFormats(
     timestampCol="SnapshotTime",
     timestamp_fmt: str = None,
     strict_conversion: bool = True,
 ):
     """Parses Pega DateTime formats.
 
@@ -83,21 +131,85 @@
             .then(
                 pl.col(timestampCol)
                 .str.strptime(pl.Datetime, "%Y-%m-%d %H:%M:%S", strict=False)
                 .dt.cast_time_unit("ns")
             )
             .otherwise(
                 pl.col(timestampCol)
-                .str.strptime(pl.Datetime, "%Y%m%dT%H%M%S.%f %Z", strict=False)
+                .str.strptime(pl.Datetime, "%Y%m%dT%H%M%S.%3f %Z", strict=False)
                 .dt.replace_time_zone(None)
                 .dt.cast_time_unit("ns")
             )
         ).alias(timestampCol)
 
 
+def getTypeMapping(df, definition, verbose=False, **timestamp_opts):
+    def getMapping(columns, reverse=False):
+        if not reverse:
+            return dict(zip(columns, _capitalize(columns)))
+        else:
+            return dict(zip(_capitalize(columns), columns))
+
+    named = getMapping(df.columns)
+    typed = getMapping(
+        [col for col in dir(definition) if not col.startswith("__")], reverse=True
+    )
+    types = []
+    for col, renamedCol in named.items():
+        try:
+            new_type = getattr(definition, typed[renamedCol])
+            if df.schema[col].base_type() != new_type:
+                if new_type == pl.Datetime and df.schema[col] != pl.Date:
+                    types.append(parsePegaDateTimeFormats(col, **timestamp_opts))
+                else:
+                    types.append(pl.col(col).cast(new_type))
+        except:
+            if verbose:
+                print(f"Column {col} not in default table schema, can't set type.")
+    return types
+
+
+def set_types(df, table="infer", verbose=False, **timestamp_opts):
+    if table == "infer":
+        table = inferTableDefinition(df)
+
+    if table == "pyValueFinder":
+        definition = PegaDefaultTables.pyValueFinder()
+    elif table == "ADMModelSnapshot":
+        definition = PegaDefaultTables.ADMModelSnapshot()
+    elif table == "ADMPredictorBinningSnapshot":
+        definition = PegaDefaultTables.ADMPredictorBinningSnapshot()
+
+    else:
+        raise ValueError(table)
+
+    mapping = getTypeMapping(df, definition, verbose=verbose, **timestamp_opts)
+
+    if len(mapping) > 0:
+        return df.with_columns(mapping)
+    else:
+        return df
+
+
+def inferTableDefinition(df):
+    cols = _capitalize(df.columns)
+    vf = ["Propensity", "Stage"]
+    predictors = ["PredictorName", "ModelID", "BinSymbol"]
+    models = ["ModelID", "Performance"]
+    if all(value in cols for value in vf):
+        return "pyValueFinder"
+    elif all(value in cols for value in predictors):
+        return "ADMPredictorBinningSnapshot"
+    elif all(value in cols for value in models):
+        return "ADMModelSnapshot"
+    else:
+        print("Could not find table definition.")
+        return cols
+
+
 def safe_range_auc(auc: float) -> float:
     """Internal helper to keep auc a safe number between 0.5 and 1.0 always.
 
     Parameters
     ----------
     auc : float
         The AUC (Area Under the Curve) score
```

### Comparing `pdstools-3.1.2/python/pdstools/utils/datasets.py` & `pdstools-3.1.3/python/pdstools/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/utils/hds_utils.py` & `pdstools-3.1.3/python/pdstools/utils/hds_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/utils/pega_template.py` & `pdstools-3.1.3/python/pdstools/utils/pega_template.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/utils/polars_ext.py` & `pdstools-3.1.3/python/pdstools/utils/polars_ext.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/utils/show_versions.py` & `pdstools-3.1.3/python/pdstools/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/utils/streamlit_utils.py` & `pdstools-3.1.3/python/pdstools/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `pdstools-3.1.2/python/pdstools/valuefinder/ValueFinder.py` & `pdstools-3.1.3/python/pdstools/valuefinder/ValueFinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,27 @@
             "pyStage",
             "pyIssue",
             "pyGroup",
             "pyChannel",
             "pyDirection",
             "CustomerID",
             "pyName",
-            "pyWorkID",
             "pyModelPropensity",
             "pyPropensity",
             "FinalPropensity",
         ]
 
         if df is not None:
             self.df = pega_io.readDSExport(df, verbose=verbose)
         else:
             filename = kwargs.pop("filename", "ValueFinder")
             self.df = pega_io.readDSExport(filename, path, verbose=verbose)
-
         if kwargs.get("subset", True):
             self.df = self.df.select(keep_cols)
+        self.df = cdh_utils.set_types(self.df, "pyValueFinder")
 
         if "th" not in kwargs:
             self.th = self.df.filter(pl.col("pyStage") == "Eligibility").select(
                 pl.quantile("pyModelPropensity", 0.05).alias("th")
             )
         else:
             self.th = pl.LazyFrame({"th": kwargs.pop("th")})
@@ -659,30 +658,32 @@
         elif level.casefold() in {"issue", "pyissue"}:
             level, cat = "pyIssue", "Issues"
         elif level.casefold() in {"group", "pygroup"}:
             level, cat = "pyGroup", "Groups"
 
         df = self.df if query is None else self.df.filter(query)
         df = (
-            pl.LazyFrame({"pyStage": self.NBADStages})
+            pl.LazyFrame(
+                {"pyStage": self.NBADStages}, schema={"pyStage": pl.Categorical}
+            )
             .join(
                 df.groupby("pyStage")
                 .agg(pl.col(level).value_counts().sort())
                 .explode(level)
                 .unnest(level),
                 on="pyStage",
             )
             .rename({level: "Name", "counts": "Count", "pyStage": "Stage"})
             .collect()
         )
         if return_df:
             return df
 
         fig = px.funnel(
-            df.to_pandas(),
+            df.with_columns(pl.col(pl.Categorical).cast(pl.Utf8)).to_pandas(),
             y="Count",
             x="Stage",
             color="Name",
             text="Name",
             title=f"Distribution of {cat.casefold()} over the stages",
             template="none",
         )
```

