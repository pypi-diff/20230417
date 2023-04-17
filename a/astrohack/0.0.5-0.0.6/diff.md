# Comparing `tmp/astrohack-0.0.5.tar.gz` & `tmp/astrohack-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.0.5.tar", last modified: Wed Apr 12 18:56:15 2023, max compression
+gzip compressed data, was "astrohack-0.0.6.tar", last modified: Mon Apr 17 17:07:41 2023, max compression
```

## Comparing `astrohack-0.0.5.tar` & `astrohack-0.0.6.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 18:56:15.661412 astrohack-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-12 18:55:57.000000 astrohack-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:55:57.000000 astrohack-0.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 18:55:58.000000 astrohack-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 18:56:15.661412 astrohack-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.653411 astrohack-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.657411 astrohack-0.0.5/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.657411 astrohack-0.0.5/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    25210 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20228 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_dio_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    33979 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/astrohack_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-12 18:55:58.000000 astrohack-0.0.5/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.657411 astrohack-0.0.5/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 18:56:15.000000 astrohack-0.0.5/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:56:15.661412 astrohack-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19951 2023-04-12 18:55:58.000000 astrohack-0.0.5/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-12 18:55:58.000000 astrohack-0.0.5/tests/test_class_ring_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 17:07:41.110303 astrohack-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 17:07:23.000000 astrohack-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:23.000000 astrohack-0.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 17:07:24.000000 astrohack-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:07:41.110303 astrohack-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.102303 astrohack-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.106303 astrohack-0.0.6/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.106303 astrohack-0.0.6/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    27476 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dio_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33916 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/astrohack_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.102303 astrohack-0.0.6/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/data/telescopes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.106303 astrohack-0.0.6/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-17 17:07:24.000000 astrohack-0.0.6/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-17 17:07:24.000000 astrohack-0.0.6/tests/test_class_ring_panel.py
```

### Comparing `astrohack-0.0.5/PKG-INFO` & `astrohack-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 # astroHACK
```

### Comparing `astrohack-0.0.5/README.md` & `astrohack-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/pyproject.toml` & `astrohack-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.0.5"
+version = "0.0.6"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.0.5/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.0.6/src/astrohack/_classes/antenna_surface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,106 +1,141 @@
 import xarray as xr
 from matplotlib import pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
-from astrohack._classes.base_panel import panelkinds, irigid
+from astrohack._classes.base_panel import panel_models, irigid
 from astrohack._classes.ring_panel import RingPanel
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_to_db
 from astrohack._utils._conversion import _convert_unit
+from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 lnbr = "\n"
 
 
 class AntennaSurface:
-    def __init__(self, inputxds, telescope, cutoff=None, pkind=None, crop=False, panel_margins=None):
+    def __init__(self, inputxds, telescope, cutoff=None, pmodel=None, crop=False, panel_margins=None, reread=False):
         """
         Antenna Surface description capable of computing RMS, Gains, and fitting the surface to obtain screw adjustments
         Args:
             inputxds: Input xarray dataset
             telescope: Telescope object
             cutoff: fractional cutoff on the amplitude image to exclude regions with weak amplitude from the panel,
                     defaults to 20% if None
-            pkind: Kind of panel surface fitting, if is None defaults to telescope default
+            pmodel: model of panel surface fitting, if is None defaults to telescope default
             crop: Crop apertures to slightly larger frames than the antenna diameter
             panel_margins: Margin to be ignored at edges of panels when fitting, defaults to 20% if None
+            reread: Read a previously processed holography
         """
+        self.reread = reread
         self._nullify()
+        self._read_xds(inputxds)
         self.telescope = telescope
-        computephase = self._read_xds(inputxds)
 
-        if cutoff is None:
-            self.cut = 0.2 * np.nanmax(self.amplitude)
-        else:
-            self.cut = cutoff * np.nanmax(self.amplitude)
-        if pkind is None:
-            self.panelkind = panelkinds[irigid]
-        else:
-            self.panelkind = pkind
-        if panel_margins is None:
-            self.panel_margins = 0.2
-        else:
-            self.panel_margins = panel_margins
-        self.reso = self.telescope.diam / self.npoint
-
-        if crop:
-            self._crop_maps()
+        if not self.reread:
+            if cutoff is None:
+                self.cut = 0.2 * np.nanmax(self.amplitude)
+            else:
+                self.cut = cutoff * np.nanmax(self.amplitude)
+            if pmodel is None:
+                self.panelmodel = panel_models[irigid]
+            else:
+                self.panelmodel = pmodel
+            if panel_margins is None:
+                self.panel_margins = 0.2
+            else:
+                self.panel_margins = panel_margins
+            self.reso = self.telescope.diam / self.npoint
 
+            if crop:
+                self._crop_maps()
         if self.telescope.ringed:
             self._init_ringed()
+        if not self.reread:
+            if self.computephase:
+                self.phase = self._deviation_to_phase(self.deviation)
+            else:
+                self.deviation = self._phase_to_deviation(self.phase)
 
-        if computephase:
-            self.phase = self._deviation_to_phase(self.deviation)
+            self.phase = self._nan_out_of_bounds(self.phase)
+            self.amplitude = self._nan_out_of_bounds(self.amplitude)
+            self.deviation = self._nan_out_of_bounds(self.deviation)
+
+    def _read_aips_xds(self, inputxds):
+        self.amplitude = np.flipud(inputxds["AMPLITUDE"].values)
+        self.deviation = np.flipud(inputxds["DEVIATION"].values)
+        self.npoint = inputxds.attrs['npoint']
+        self.wavelength = inputxds.attrs['wavelength']
+        self.amp_unit = inputxds.attrs['amp_unit']
+        self.u_axis = inputxds.u.values
+        self.v_axis = inputxds.v.values
+        self.computephase = True
+        self.processed = False
+
+    def _read_holog_xds(self, inputxds):
+        if 'chan' in inputxds.dims:
+            if inputxds.dims['chan'] != 1:
+                raise Exception("Only single channel holographies supported")
+            self.wavelength = clight / inputxds.chan.values[0]
         else:
-            self.deviation = self._phase_to_deviation(self.phase)
+            self.wavelength = inputxds.attrs['wavelength']
+
+        self.amplitude = inputxds["AMPLITUDE"].values[0, 0, 0, :, :]
+        self.phase = inputxds["ANGLE"].values[0, 0, 0, :, :]
 
-        self.phase = self._nan_out_of_bounds(self.phase)
-        self.amplitude = self._nan_out_of_bounds(self.amplitude)
-        self.deviation = self._nan_out_of_bounds(self.deviation)
+        self.npoint = np.sqrt(inputxds.dims['l'] ** 2 + inputxds.dims['m'] ** 2)
+        self.amp_unit = 'V'
+        self.u_axis = inputxds.u_prime.values * self.wavelength
+        self.v_axis = inputxds.v_prime.values * self.wavelength
+        self.computephase = False
+
+    def _read_panel_xds(self, inputxds):
+        self.wavelength = inputxds.attrs['wavelength']
+        self.amp_unit = inputxds.attrs['amp_unit']
+        self.panelmodel = inputxds.attrs['panel_model']
+        self.panel_margins = inputxds.attrs['panel_margin']
+        self.cut = inputxds.attrs['cutoff']
+        self.solved = inputxds.attrs['solved']
+        self.fitted = inputxds.attrs['fitted']
+        # Arrays
+        self.amplitude = inputxds['AMPLITUDE'].values
+        self.phase = inputxds['PHASE'].values
+        self.deviation = inputxds['DEVIATION'].values
+        self.mask = inputxds['MASK']
+        self.u_axis = inputxds.u.values
+        self.v_axis = inputxds.u.values
+
+        if self.solved:
+            self.phase_residuals = inputxds['PHASE_RESIDUALS'].values
+            self.residuals = inputxds['RESIDUALS'].values
+            self.phase_corrections = inputxds['PHASE_CORRECTIONS'].values
+            self.corrections = inputxds['CORRECTIONS'].values
+            self.panel_pars = inputxds['PANEL_PARAMETERS'].values
+            self.screw_adjustments = inputxds['PANEL_SCREWS'].values
+            self.panel_labels = inputxds.labels.values
 
     def _read_xds(self, inputxds):
         """
         Read input XDS, distinguishing what is derived from AIPS data and what was created by astrohack.holog
         Args:
             inputxds: X array dataset
         """
-        # Origin dependant Reading
-        if inputxds.attrs['AIPS']:
-            self.amplitude = np.flipud(inputxds["AMPLITUDE"].values)
-            self.deviation = np.flipud(inputxds["DEVIATION"].values)
-            self.npoint = inputxds.attrs['npoint']
-            self.wavelength = inputxds.attrs['wavelength']
-            self.amp_unit = inputxds.attrs['amp_unit']
-            self.u_axis = inputxds.u.values
-            self.v_axis = inputxds.v.values
-            computephase = True
+        # Origin dependant reading
+        if self.reread:
+            self._read_panel_xds(inputxds)
         else:
-            if 'chan' in inputxds.dims:
-                if inputxds.dims['chan'] != 1:
-                    raise Exception("Only single channel holographies supported")
-                self.wavelength = clight / inputxds.chan.values[0]
+            if inputxds.attrs['AIPS']:
+                self._read_aips_xds(inputxds)
             else:
-                self.wavelength = inputxds.attrs['wavelength']
-
-            self.amplitude = inputxds["AMPLITUDE"].values[0, 0, 0, :, :]
-            self.phase = inputxds["ANGLE"].values[0, 0, 0, :, :]
-
-            self.npoint = np.sqrt(inputxds.dims['l']**2 + inputxds.dims['m']**2)
-            self.amp_unit = 'V'
-            self.u_axis = inputxds.u_prime.values * self.wavelength
-            self.v_axis = inputxds.v_prime.values * self.wavelength
-            computephase = False
+                self._read_holog_xds(inputxds)
 
         # Common elements
         self.unpix = self.u_axis.shape[0]
         self.vnpix = self.v_axis.shape[0]
         self.antenna_name = inputxds.attrs['ant_name']
-        
-        self.panel_meta = [inputxds.attrs['ant_name'],inputxds.attrs['ddi']]
-
-        return computephase
+        self.ddi = inputxds.attrs['ddi']
 
     def _nullify(self):
         """
         Part of the initialization process, nullify the data objects to be used later
         """
         self.phase = None
         self.deviation = None
@@ -109,14 +144,15 @@
         self.phase_corrections = None
         self.phase_residuals = None
         self.solved = False
         self.ingains = np.nan
         self.ougains = np.nan
         self.in_rms = np.nan
         self.out_rms = np.nan
+        self.fitted = False
 
     def _init_ringed(self):
         """
         Do the proper method association for the case of a ringed antenna
         """
         if self.telescope.panel_numbering == 'ring, clockwise, top':
             self._panel_label = self._vla_panel_labeling
@@ -250,21 +286,20 @@
         Build list of panels, specific for circular antennas with panels arranged in rings
         """
         self.panels = []
         for iring in range(self.telescope.nrings):
             angle = 2.0 * np.pi / self.telescope.npanel[iring]
             for ipanel in range(self.telescope.npanel[iring]):
                 panel = RingPanel(
-                    self.panelkind,
+                    self.panelmodel,
                     angle,
                     ipanel,
                     self._panel_label(iring, ipanel),
                     self.telescope.inrad[iring],
                     self.telescope.ourad[iring],
-                    panel_meta=self.panel_meta,
                     margin=self.panel_margins,
                     screw_scheme=self.telescope.screw_description,
                     screw_offset=self.telescope.screw_offset
                 )
                 self.panels.append(panel)
         return
 
@@ -360,34 +395,45 @@
         """
         return np.sqrt(np.mean(array[self.mask] ** 2))
 
     def fit_surface(self):
         """
         Loops over the panels to fit the panel surfaces
         """
+        panels = []
         for panel in self.panels:
-            panel.solve()
-        self.solved = True
+            if not panel.solve():
+                panels.append(panel.label)
+        self.fitted = True
+        if len(panels) > 0:
+            msg = f'Fit failed with the {self.panelmodel} model and a simple mean has been used instead for the ' \
+                  f'following panels: ' + str([self.antenna_name, self.ddi])
+            logger = _get_astrohack_logger()
+            logger.warning(msg)
+            msg = str(panels)
+            logger.warning(msg)
 
     def correct_surface(self):
         """
         Apply corrections determined by the panel surface fitting methods to the antenna surface
         """
-        if not self.solved:
+        if not self.fitted:
             raise Exception("Panels must be fitted before atempting a correction")
         self.corrections = np.where(self.mask, 0, np.nan)
         self.residuals = np.copy(self.deviation)
         for panel in self.panels:
             corrections = panel.get_corrections()
             for corr in corrections:
                 ix, iy = int(corr[0]), int(corr[1])
                 self.residuals[ix, iy] -= corr[-1]
                 self.corrections[ix, iy] = -corr[-1]
         self.phase_corrections = self._deviation_to_phase(self.corrections)
         self.phase_residuals = self._deviation_to_phase(self.residuals)
+        self._build_panel_data_arrays()
+        self.solved = True
 
     def print_misc(self):
         """
         Print miscelaneous information on the panels in the antenna surface
         """
         for panel in self.panels:
             panel.print_misc()
@@ -511,86 +557,87 @@
         Build arrays with data from the panels so that they can be stored on the XDS
         Returns:
             List with panel labels, panel fitting parameters, screw_adjustments
         """
         npanels = len(self.panels)
         NPAR = self.panels[0].NPAR
         nscrews = self.panels[0].screws.shape[0]
-        panel_labels = np.ndarray([npanels], dtype=object)
-        panel_pars = np.ndarray((npanels, NPAR), dtype=float)
-        screw_adjustments = np.ndarray((npanels, nscrews), dtype=float)
+        self.panel_labels = np.ndarray([npanels], dtype=object)
+        self.panel_pars = np.ndarray((npanels, NPAR), dtype=float)
+        self.screw_adjustments = np.ndarray((npanels, nscrews), dtype=float)
         for ipanel in range(npanels):
-            panel_labels[ipanel] = self.panels[ipanel].label
-            panel_pars[ipanel, :] = self.panels[ipanel].par
-            screw_adjustments[ipanel, :] = self.panels[ipanel].export_screws_float(unit='m')
-        return panel_labels, panel_pars, screw_adjustments
+            self.panel_labels[ipanel] = self.panels[ipanel].label
+            self.panel_pars[ipanel, :] = self.panels[ipanel].par
+            self.screw_adjustments[ipanel, :] = self.panels[ipanel].export_screws(unit='m')
 
-    def export_screw_adjustments(self, filename, unit="mm"):
+    def export_screws(self, filename, unit="mm"):
         """
         Export screw adjustments for all panels onto an ASCII file
         Args:
             filename: ASCII file name/path
             unit: unit for panel screw adjustments ['mm','miliinches']
         """
-        spc = " "
-        outfile = "Screw adjustments for {0:s} {1:s} antenna\n".format(
-            self.telescope.name, self.antenna_name
-        )
+        outfile = "Screw adjustments for {0:s} {1:s} antenna\n".format(self.telescope.name, self.antenna_name)
         outfile += "Adjustments are in " + unit + lnbr
         outfile += 2 * lnbr
-        outfile += 25 * spc + "{0:22s}{1:22s}".format("Inner Edge", "Outer Edge") + lnbr
-        outfile += 5 * spc + "{0:8s}{1:8s}".format("Ring", "panel")
-        outfile += 2 * spc + 2 * "{0:11s}{1:11s}".format("left", "right") + lnbr
-        for panel in self.panels:
-            outfile += panel.export_adjustments(unit=unit) + lnbr
+        outfile += "{0:8s}".format('Panel')
+        nscrews = len(self.telescope.screw_description)
+        for screw in self.telescope.screw_description:
+            outfile += "{0:11s}".format(screw)
+        outfile += lnbr
+        fac = _convert_unit('m', unit, 'length')
+        for ipanel in range(len(self.panel_labels)):
+            outfile += "{0:8s}".format(self.panel_labels[ipanel])
+            for iscrew in range(nscrews):
+                outfile += " {0:10.2f}".format(fac*self.screw_adjustments[ipanel, iscrew])
+            outfile += lnbr
+
         lefile = open(filename, "w")
         lefile.write(outfile)
         lefile.close()
 
     def export_xds(self):
         """
         Export all the data to Xarray dataset
         Returns:
             XarrayDataSet contaning all the relevant information
         """
         xds = xr.Dataset()
         gains = self.gains()
         rms = self.get_rms(unit='m')
         xds.attrs['telescope_name'] = self.telescope.name
-        xds.attrs['antenna_name'] = self.antenna_name
+        xds.attrs['ant_name'] = self.antenna_name
+        xds.attrs['ddi'] = self.ddi
         xds.attrs['wavelength'] = self.wavelength
-        xds.attrs['AIPS'] = False
         xds.attrs['amp_unit'] = self.amp_unit
-        xds.attrs['panel_kind'] = self.panelkind
+        xds.attrs['panel_model'] = self.panelmodel
         xds.attrs['panel_margin'] = self.panel_margins
         xds.attrs['cutoff'] = self.cut
+        xds.attrs['solved'] = self.solved
+        xds.attrs['fitted'] = self.fitted
         xds['AMPLITUDE'] = xr.DataArray(self.amplitude, dims=["u", "v"])
         xds['PHASE'] = xr.DataArray(self.phase, dims=["u", "v"])
         xds['DEVIATION'] = xr.DataArray(self.deviation, dims=["u", "v"])
         xds['MASK'] = xr.DataArray(self.mask, dims=["u", "v"])
         xds['PANEL_DISTRIBUTION'] = xr.DataArray(self.panel_distribution, dims=["u", "v"])
-        if self.residuals is not None:
+        if self.solved:
             xds['PHASE_RESIDUALS'] = xr.DataArray(self.phase_residuals, dims=["u", "v"])
             xds['RESIDUALS'] = xr.DataArray(self.residuals, dims=["u", "v"])
             xds['PHASE_CORRECTIONS'] = xr.DataArray(self.phase_corrections, dims=["u", "v"])
             xds['CORRECTIONS'] = xr.DataArray(self.corrections, dims=["u", "v"])
             xds.attrs['input_rms'] = rms[0]
             xds.attrs['output_rms'] = rms[1]
             xds.attrs['input_gain'] = gains[0][0]
             xds.attrs['output_gain'] = gains[1][0]
             xds.attrs['theoretical_gain'] = gains[0][1]
+            xds['PANEL_PARAMETERS'] = xr.DataArray(self.panel_pars, dims=['labels', 'pars'])
+            xds['PANEL_SCREWS'] = xr.DataArray(self.screw_adjustments, dims=['labels', 'screws'])
+            coords = {"u": self.u_axis, "v": self.v_axis, 'labels': self.panel_labels,
+                      'screws': self.telescope.screw_description, 'pars': np.arange(self.panel_pars.shape[1])}
         else:
             xds.attrs['input_rms'] = rms
             xds.attrs['input_gain'] = gains[0]
             xds.attrs['theoretical_gain'] = gains[1]
-
-        if self.solved:
-            labels, pars, screws = self._build_panel_data_arrays()
-            xds['PANEL_PARAMETERS'] = xr.DataArray(pars, dims=['labels', 'pars'])
-            xds['PANEL_SCREWS'] = xr.DataArray(screws, dims=['labels', 'screws'])
-            coords = {"u": self.u_axis, "v": self.v_axis, 'labels': labels, 'screws': self.telescope.screw_description,
-                      'pars': np.arange(pars.shape[1])}
-        else:
             coords = {"u": self.u_axis, "v": self.v_axis}
 
         xds = xds.assign_coords(coords)
         return xds
```

### Comparing `astrohack-0.0.5/src/astrohack/_classes/base_panel.py` & `astrohack-0.0.6/src/astrohack/_classes/base_panel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from scipy import optimize as opt
 
 from astrohack._utils._algorithms import _gauss_elimination_numpy, _least_squares_fit
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
-panelkinds = ["mean", "rigid", "corotated_scipy", "corotated_lst_sq", "corotated_robust", "xy_paraboloid",
-              "rotated_paraboloid", "full_paraboloid_lst_sq"]
+panel_models = ["mean", "rigid", "corotated_scipy", "corotated_lst_sq", "corotated_robust", "xy_paraboloid",
+                "rotated_paraboloid", "full_paraboloid_lst_sq"]
 imean = 0
 irigid = 1
 icorscp = 2
 icorlst = 3
 icorrob = 4
 ixypara = 5
 irotpara = 6
@@ -34,94 +34,93 @@
     markers = ['X', 'o', '*', 'P', 'D']
     colors = ['g', 'g', 'r', 'r', 'b']
     fontsize = 4
     linewidth = 0.5
     markersize = 2
     linecolor = 'black'
 
-    def __init__(self, kind, screws, label, panel_meta, center=None, zeta=None):
+    def __init__(self, model, screws, label, center=None, zeta=None):
         """
         Initializes the base panel with the appropriated fitting methods and providing basic functionality
-        Fitting method kinds are:
-        AIPS fitting kinds:
+        Fitting method models are:
+        AIPS fitting models:
             mean: The panel is corrected by the mean of its samples
             rigid: The panel samples are fitted to a rigid surface
         Corotated Paraboloids (the two bending axes are parallel and perpendicular to the radius of the antenna crossing
         the middle of the panel):
             corotated_scipy: Paraboloid is fitted using scipy.optimize, robust but slow
             corotated_lst_sq: Paraboloid is fitted using the linear algebra least squares method, fast but unreliable
             corotated_robust: Tries corotated_lst_sq, if it diverges falls back to corotated_scipy
-        Experimental fitting kinds:
+        Experimental fitting models:
             xy_paraboloid: fitted using scipy.optimize, bending axes are parallel to the x and y axes
             rotated_paraboloid: fitted using scipy.optimize, bending axes can be rotated by an arbitrary angle
             full_paraboloid_lst_sq: Full 9 parameter paraboloid fitted using least_squares method, heavily overfits
         Args:
-            kind: What kind of surface fitting method to be used
+            model: What model of surface fitting method to be used
             label: Panel label
             screws: position of the screws
             center: Panel center
             zeta: panel center angle
         """
-        self.kind = kind
+        self.model = model
         self.solved = False
         self.label = label
         self.screws = screws
         self.samples = []
         self.margins = []
         self.corr = None
-        self.panel_meta = panel_meta
 
         if center is None:
             self.center = [0, 0]
         else:
             self.center = center
         if zeta is None:
             self.zeta = 0
         else:
             self.zeta = zeta
         self._associate()
 
     def _associate(self):
         """
-        Does the fitting method associations according to the kind chosen by the user
+        Does the fitting method associations according to the model chosen by the user
         """
         logger = _get_astrohack_logger()
         try:
-            ikind = panelkinds.index(self.kind)
+            imodel = panel_models.index(self.model)
         except ValueError:
-            logger.error("Unknown panel kind: "+self.kind)
-            raise ValueError('Panel kind not in list')
-        if ikind > icorrob:
+            logger.error("Unknown panel model: "+self.model)
+            raise ValueError('Panel model not in list')
+        if imodel > icorrob:
             self._warn_experimental_method()
-        if ikind == irigid:
+        if imodel == irigid:
             self._associate_rigid()
-        elif ikind == imean:
+        elif imodel == imean:
             self._associate_mean()
-        elif ikind == ixypara:
+        elif imodel == ixypara:
             self._associate_scipy(self._xyaxes_paraboloid, 3)
-        elif ikind == irotpara:
+        elif imodel == irotpara:
             self._associate_scipy(self._rotated_paraboloid, 4)
-        elif ikind == icorscp:
+        elif imodel == icorscp:
             self._associate_scipy(self._corotated_paraboloid, 3)
-        elif ikind == ifulllst:
+        elif imodel == ifulllst:
             self._associate_least_squares()
-        elif ikind == icorlst:
+        elif imodel == icorlst:
             self._associate_corotated_lst_sq()
-        elif ikind == icorrob:
+        elif imodel == icorrob:
             self._associate_robust()
         
     def _warn_experimental_method(self):
         """
         Raises a warning about experimental methods if a warning has not been raised before
         """
         if warned:
             return
         else:
             logger = _get_astrohack_logger()
-            logger.warning("Experimental kind: "+self.kind)
+            logger.warning("Experimental model: "+self.model)
             set_warned(True)
 
     def _associate_scipy(self, fitting_function, NPAR):
         """
         Associate the proper methods to enable scipy fitting
         Args:
             fitting_function: The fitting function to be used by scipy
@@ -130,15 +129,15 @@
         self.NPAR = NPAR
         self._solve_sub = self._solve_scipy
         self.corr_point = self._corr_point_scipy
         self._fitting_function = fitting_function
 
     def _associate_robust(self):
         """
-        Associate fitting method for the corotated_robust kind
+        Associate fitting method for the corotated_robust model
         Returns:
 
         """
         self.NPAR = 3
         self._solve_sub = self._solve_robust
         self.corr_point = self._corr_point_corotated_lst_sq
         self._fitting_function = self._corotated_paraboloid
@@ -190,27 +189,31 @@
             value: tuple/list containing point description [xcoor,ycoor,xidx,yidx,value]
         """
         self.margins.append(value)
 
     def solve(self):
         """
         Wrapping method around fitting to allow for a fallback to mean fitting in the case of an impossible fit
+
+        Returns:
+            True: in case of successful fit
+            False: in case of fallback fit
         """
-        logger = _get_astrohack_logger()
         # fallback behaviour for impossible fits
         if len(self.samples) < self.NPAR:
-            logger.warning("Impossible fit, falling back to mean: " + str(self.panel_meta))
             self._fallback_solve()
+            status = False
         else:
             try:
                 self._solve_sub()
+                status = True
             except np.linalg.LinAlgError:
-                logger.warning("Fit diverged, falling back to mean: " + str(self.panel_meta))
                 self._fallback_solve()
-        return
+                status = False
+        return status
 
     def _fallback_solve(self):
         """
         Changes the method association to mean surface fitting, and fits the panel with it
         """
         self._associate_mean()
         self._solve_sub()
@@ -307,15 +310,15 @@
 
         liminf = [-np.inf, -np.inf, -np.inf]
         limsup = [np.inf, np.inf, np.inf]
         if x0 is None:
             p0 = [1e2, 1e2, np.mean(devia)]
         else:
             p0 = x0
-        if self.kind == panelkinds[irotpara]:
+        if self.model == panel_models[irotpara]:
             liminf.append(0.0)
             limsup.append(np.pi)
             p0.append(0)
 
         maxfevs = [100000, 1000000, 10000000]
         for maxfev in maxfevs:
             try:
@@ -485,29 +488,15 @@
             ycoor: Y coordinate of point
 
         Returns:
         Fitted value at xcoor,ycoor
         """
         return self.par[0]
 
-    def export_adjustments(self, unit='mm'):
-        """
-        Exports panel screw adjustments to a string
-        Args:
-            unit: Unit for screw adjustments ['mm','miliinches']
-        Returns:
-        String with screw adjustments for this panel
-        """
-        fac = _convert_unit('m', unit, 'length')
-        string = self.label
-        for screw in self.screws[:, ]:
-            string += ' {0:10.2f}'.format(fac * self.corr_point(*screw))
-        return string
-
-    def export_screws_float(self, unit='mm'):
+    def export_screws(self, unit='mm'):
         """
         Export screw adjustments to a numpy array in unit
         Args:
             unit: Unit for the screw adjustments
 
         Returns:
             Numpy array with screw adjustments
```

### Comparing `astrohack-0.0.5/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.0.6/src/astrohack/_classes/polygon_panel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from shapely import Polygon, Point
 from shapely.plotting import plot_polygon
-from astrohack._classes.base_panel import BasePanel, panelkinds, icorpara
+from astrohack._classes.base_panel import BasePanel, panel_models, icorpara
 
 
 class PolygonPanel(BasePanel):
 
-    def __init__(self, kind, ipanel, polygon, screws):
+    def __init__(self, model, ipanel, polygon, screws):
         """
         Initializes a polygon based panel based on a polygon shape and the screw positions
         Args:
-            kind: What kind of surface to be used in fitting ["rigid", "mean", "xyparaboloid", "rotatedparaboloid"]
+            model: What model of surface to be used in fitting ["rigid", "mean", "xyparaboloid", "rotatedparaboloid"]
             ipanel: Panel number
             polygon: Polygon describing the panel shape
             screws: Positions of the screw over the panel
         """
-        if kind == panelkinds[icorpara]:
+        if model == panel_models[icorpara]:
             raise Exception('corotatedparaboloid not supported for Polygon based panels')
-        super().__init__(kind, ipanel, screws)
+        super().__init__(model, ipanel, screws)
         self.polygon = Polygon(polygon)
         if not self.polygon.is_simple:
             raise Exception('Polygon must not intersect itself')
         self.center = self.polygon.centroid.x, self.polygon.centroid.y
         return
 
     def is_inside(self, point):
@@ -47,15 +47,15 @@
         """
         Print miscelaneous information about the panel to the terminal
         Args:
             verbose: Include more information in print
         """
         print("########################################")
         print("{0:20s}={1:8d}".format("ipanel", self.ipanel))
-        print("{0:20s}={1:8s}".format("kind", " " + self.kind))
+        print("{0:20s}={1:8s}".format("model", " " + self.model))
         print("{0:20s}={1:8d}".format("nsamp", self.nsamp))
         if verbose:
             for isamp in range(self.nsamp):
                 strg = "{0:20s}=".format("samp{0:d}".format(isamp))
                 for val in self.values[isamp]:
                     strg += str(val) + ", "
                 print(strg)
```

### Comparing `astrohack-0.0.5/src/astrohack/_classes/ring_panel.py` & `astrohack-0.0.6/src/astrohack/_classes/ring_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from astrohack._classes.base_panel import BasePanel
 
 
 class RingPanel(BasePanel):
     # This class describes and treats panels that are arranged in
     # rings on the Antenna surface
 
-    def __init__(self, kind, angle, ipanel, label, inrad, ourad, panel_meta, margin=0.20, screw_scheme=None, screw_offset=None):
+    def __init__(self, kind, angle, ipanel, label, inrad, ourad, margin=0.20, screw_scheme=None, screw_offset=None):
         """
         Initializes a panel that is a section of a ring in a circular antenna
         Fitting method kinds are:
         AIPS fitting kinds:
             mean: The panel is corrected by the mean of its samples
             rigid: The panel samples are fitted to a rigid surface
         Corotated Paraboloids (the two bending axes are parallel and perpendicular to the radius of the antenna crossing
@@ -42,18 +42,17 @@
         self.margin_theta2 = self.theta2 - margin * angle
         self.margin_inrad = inrad + margin * dradius
         self.margin_ourad = ourad - margin * dradius
         self.first = ipanel == 0
         zeta = (ipanel + 0.5) * angle
         rt = (self.inrad + self.ourad) / 2
         self.center = [rt * np.cos(zeta), rt * np.sin(zeta)]
-        self.panel_meta = panel_meta
         screws = self._init_screws(screw_scheme, screw_offset)
         # Now we are ready to initialize the base object
-        super().__init__(kind, screws, label, panel_meta, center=self.center, zeta=zeta)
+        super().__init__(kind, screws, label, center=self.center, zeta=zeta)
 
     def _init_screws(self, scheme, offset):
         """
         Initialize screws according to the scheme
         Args:
             scheme: Tuple of strings containing the positioning of the screws
             offset: How far from the edge of the panel are corner screws (meters)
```

### Comparing `astrohack-0.0.5/src/astrohack/_classes/telescope.py` & `astrohack-0.0.6/src/astrohack/_classes/telescope.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import xarray as xr
 import pkg_resources
 import os
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
-tel_data_path = pkg_resources.resource_filename("astrohack", "../../data/telescopes")
+tel_data_path = pkg_resources.resource_filename("astrohack", "data/telescopes")
 
 
 def _find_cfg_file(name, path):
     """
     Search for the correct telescope configuration file
     Args:
         name: Name of the telescope configuration file
```

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_algorithms.py` & `astrohack-0.0.6/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_constants.py` & `astrohack-0.0.6/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_conversion.py` & `astrohack-0.0.6/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_dio_classes.py` & `astrohack-0.0.6/src/astrohack/_utils/_dio_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 import os
-import dask
-import sys
-
-import xarray as xr
 import numpy as np
-
-from casacore import tables as ctables
-
+from astrohack._utils._io import _load_image_xds
 from prettytable import PrettyTable
-
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
-
-from astrohack._utils._holog import _create_holog_meta_data 
-
-from astrohack._utils._io import _load_pnt_dict 
-from astrohack._utils._io import _extract_holog_chunk
-from astrohack._utils._io import _open_no_dask_zarr
-from astrohack._utils._io import _read_data_from_holog_json
 from astrohack._utils._io import _read_meta_data
 from astrohack._utils._io import _load_holog_file
 from astrohack._utils._io import _load_image_file
 from astrohack._utils._io import _load_panel_file
 
-from memory_profiler import profile
+from astrohack._classes.antenna_surface import AntennaSurface
+from astrohack._classes.telescope import Telescope
+
 
 class AstrohackDataFile:
     def __init__(self, file_stem, path='./'):
                         
         self._image_path = None
         self._holog_path = None
 
@@ -286,7 +274,21 @@
         table.field_names = ["antenna", "ddi"]
         table.align = "l"
         
         for ant in self.keys():
             table.add_row([ant, list(self[ant].keys())])
         
         print(table)
+
+    def review_antenna(self, antenna, ddi):
+        """
+        Return an AntennaSurface object for interaction
+        Args:
+            antenna: Which antenna in to be used
+            ddi: Which ddi is to be used
+
+        Returns:
+            AntennaSurface object contaning relevant information for panel adjustments
+        """
+        xds = _load_image_xds(self.file, antenna, ddi)
+        telescope = Telescope(xds.attrs['telescope_name'])
+        return AntennaSurface(xds, telescope, reread=True)
```

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_holog.py` & `astrohack-0.0.6/src/astrohack/_utils/_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_imaging.py` & `astrohack-0.0.6/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_io.py` & `astrohack-0.0.6/src/astrohack/_utils/_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,17 +66,17 @@
             if 'ant' in ant:
                 ddi_list =  [dir_name for dir_name in os.listdir(file + "/" + str(ant)) if os.path.isdir(file + "/" + str(ant))]
                 panel_data_dict[ant] = {}
                 
                 for ddi in ddi_list:
                     if 'ddi' in ddi:
                         if dask_load:
-                            panel_data_dict[ant][ddi] = xr.open_zarr("{name}/{ant}/{ddi}/xds.zarr".format(name=file, ant=ant, ddi=ddi))
+                            panel_data_dict[ant][ddi] = xr.open_zarr("{name}/{ant}/{ddi}".format(name=file, ant=ant, ddi=ddi))
                         else:
-                            panel_data_dict[ant][ddi] = _open_no_dask_zarr("{name}/{ant}/{ddi}/xds.zarr".format(name=file, ant=ant, ddi=ddi))
+                            panel_data_dict[ant][ddi] = _open_no_dask_zarr("{name}/{ant}/{ddi}".format(name=file, ant=ant, ddi=ddi))
     
     except Exception as e:
             logger.error(str(e))
             raise
 
     
     return panel_data_dict
@@ -831,16 +831,15 @@
                 mode="w",
                 compute=True,
                 consolidated=True,
             )
 
         else:
             logger.warning(
-                "[FLAGGED DATA] scan: {scan} mapping antenna index {index}".format(
-                    scan=scan, index=map_ant_index
+                "[FLAGGED DATA] mapping antenna index {index}".format(index=map_ant_index
                 )
             )
 
 
 def _extract_holog_chunk(extract_holog_params):
     """Perform data query on holography data chunk and get unique time and state_ids/
```

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.0.6/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_panel.py` & `astrohack-0.0.6/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.0.6/src/astrohack/_utils/gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/astrohack_client.py` & `astrohack-0.0.6/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/dio.py` & `astrohack-0.0.6/src/astrohack/dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/extract_holog.py` & `astrohack-0.0.6/src/astrohack/extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/gdown_utils.py` & `astrohack-0.0.6/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/holog.py` & `astrohack-0.0.6/src/astrohack/holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/panel.py` & `astrohack-0.0.6/src/astrohack/panel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 import os
 import dask
 import xarray as xr
 import shutil
 
 from astrohack._classes.antenna_surface import AntennaSurface
 from astrohack._classes.telescope import Telescope
-from astrohack._classes.base_panel import panelkinds
-from astrohack._utils._constants import length_units
+from astrohack._classes.base_panel import panel_models
 from astrohack._utils._io import _load_image_xds, _aips_holog_to_xds, check_if_file_will_be_overwritten, check_if_file_exists
 from astrohack._utils._panel import _external_to_internal_parameters, _correct_phase
 import numpy as np
 
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._utils import _remove_suffix
 
 from astrohack._utils._dio_classes import AstrohackPanelFile
 
-def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, unit='mm', panel_margins=0.2, save_mask=False,
-          save_deviations=True, save_phase=False, parallel=False, sel_ddi=None, overwrite=False):
+
+def panel(image_name, panel_name=None, cutoff=0.2, panel_model=None, panel_margins=0.2, parallel=False, sel_ddi=None,
+          overwrite=False):
     """Analyze holography images to derive panel adjustments
 
     :param image_name: Input holography data file name. Accepted data formats are the output from ``astrohack.holog.holog`` and AIPS holography data prepackaged using ``astrohack.panel.aips_holog_to_astrohack``.
     :type image_name: str
     :param panel_name: Name of output file; File name will be appended with suffix *.panel.zarr*. Defaults to *basename* of input file plus holography panel file suffix.
     :type panel_name: str, optional
     :param cutoff: Relative amplitude cut-off which defines fitting mask. Defaults to 0.2.
     :type cutoff: float, optional
     :param panel_model: Model of surface fitting function used to fit panel surfaces, None will default to "rigid". Possible models are listed below.
     :type panel_model: str, optional
-    :param unit: Unit used in deviation plots and screw adjustments. Several units are available: "m" (meters); "mm" (millimeters); "mils" (milliinches) OR "um" (microns). Defaults to "mm".
-    :type unit: str, optional
     :param panel_margins: Relative margin from the edge of the panel used to decide which points are margin points or internal points of each panel. Defaults to 0.2.
     :type panel_margins: float, optional
-    :param save_mask: Save mask plot derived from the amplitude image and the map of the panels. Defaults to False.
-    :type save_mask: bool, optional
-    :param save_deviations: Save plot with the uncorrected deviation image, applied corrections and the corrected deviation image. Defaults to True.
-    :type save_deviations: bool, optional
-    :param save_phase: Save plot with the uncorrected phase image, applied corrections and the corrected phase image. Defaults to False.
-    :type save_phase: bool, optional
     :param parallel: Run in parallel. Defaults to False.
     :type parallel: bool, optional
     :param sel_ddi: List of DDIs to be processed. None will use all DDIs. Defaults to None.
     :type sel_ddi: list, optional
     :param overwrite: Overwrite files on disk. Defaults to False.
     :type overwrite: bool, optional
 
@@ -60,16 +52,14 @@
         - For each panel:
             * Internal pixels are fitted to a surface model.
             * The fitted surface model is used to derive corrections for all pixels in the panel, internal and margins.
             * The fitted surface model is used to derive corrections for the positions of the screws.
         - A corrected deviation image is produced.
         - RMS is computed for both the corrected and uncorrected deviation images.
         - All images produced are stored in the output *.panel.zarr file*.
-        - Optional plots can be produced (plot production may impact performance).
-        - An ASCII file containing the adjustments to be applied to the panel screws is saved inside the *.panel.zarr* file.
 
         .. rubric:: Available panel surface models:
         * AIPS fitting models:
             - *mean*: The panel is corrected by the mean of its samples.
             - *rigid*: The panel samples are fitted to a rigid surface (DEFAULT model).
         * Corotated Paraboloids: (the two bending axes of the paraboloid are parallel and perpendicular to a radius of the antenna crossing the middle point of the panel):
             - *corotated_scipy*: Paraboloid is fitted using scipy.optimize, robust but slow.
@@ -81,16 +71,16 @@
             - *full_paraboloid_lst_sq*: Full 9 parameter paraboloid fitted using least_squares method, tends to heavily overfit surface irregularities.
 
 
     """
     
     logger = _get_astrohack_logger()
     
-    panel_params = _check_panel_parms(image_name, panel_name, cutoff, panel_model, unit, panel_margins, save_mask,
-                                      save_deviations, save_phase, parallel, sel_ddi, overwrite)
+    panel_params = _check_panel_parms(image_name, panel_name, cutoff, panel_model, panel_margins, parallel, sel_ddi,
+                                      overwrite)
           
     check_if_file_exists(panel_params['image_name'])
     check_if_file_will_be_overwritten(panel_params['panel_name'], panel_params['overwrite'])
 
     if os.path.exists(panel_params['image_name']+'/.aips'):
         panel_params['origin'] = 'AIPS'
         _panel_chunk(panel_params)
@@ -127,15 +117,14 @@
             logger.info("Panel finished processing")
             
             panel_mds = AstrohackPanelFile(panel_chunk_params['panel_name'])
             panel_mds.open()
             return panel_mds
 
 
-
 def _panel_chunk(panel_chunk_params):
     """
     Process a chunk of the holographies, usually a chunk consists of an antenna over a ddi
     Args:
         panel_chunk_params: dictionary of inputs
     """
     if panel_chunk_params['origin'] == 'AIPS':
@@ -163,31 +152,17 @@
     surface = AntennaSurface(inputxds, telescope, panel_chunk_params['cutoff'], panel_chunk_params['panel_kind'],
                              panel_margins=panel_chunk_params['panel_margins'])
 
     surface.compile_panel_points()
     surface.fit_surface()
     surface.correct_surface()
     
-    base_name = panel_chunk_params['panel_name'] + '/' + panel_chunk_params['antenna'] + '/' + panel_chunk_params['ddi']
-
-    os.makedirs(name=base_name, exist_ok=True)
-
-    base_name += "/"
+    xds_name = panel_chunk_params['panel_name'] + '/' + panel_chunk_params['antenna'] + '/' + panel_chunk_params['ddi']
     xds = surface.export_xds()
-    xds.to_zarr(base_name+'xds.zarr', mode='w')
-    surface.export_screw_adjustments(base_name + "screws.txt", unit=panel_chunk_params['unit'])
-    
-    if panel_chunk_params['save_mask']:
-        surface.plot_surface(filename=base_name + "mask.png", mask=True, screws=True)
-    
-    if panel_chunk_params['save_deviations']:
-        surface.plot_surface(filename=base_name + "surface.png")
-    
-    if panel_chunk_params['save_phase']:
-        surface.plot_surface(filename=base_name + "phase.png", plotphase=True)
+    xds.to_zarr(xds_name, mode='w')
 
 
 def _create_phase_model(npix, parameters, wavelength, telescope, cellxy):
     """
     Create a phase model with npix by npix size according to the given parameters
     Args:
         npix: Number of pixels in each size of the model
@@ -232,63 +207,50 @@
     if os.path.exists(holog_name):
         shutil.rmtree(holog_name, ignore_errors=False, onerror=None)
     xds.to_zarr(holog_name, mode='w', compute=True, consolidated=True)
     aips_mark = open(holog_name+'/.aips', 'w')
     aips_mark.close()
 
 
-def _check_panel_parms(image_name, panel_name, cutoff, panel_kind, unit, panel_margins, save_mask, save_deviations,
-                       save_phase, parallel, sel_ddi, overwrite):
+def _check_panel_parms(image_name, panel_name, cutoff, panel_kind, panel_margins, parallel, sel_ddi, overwrite):
     """
     Tests inputs to panel function
     Args:
         image_name: Input holography data, can be from astrohack.holog, but also preprocessed AIPS data
         panel_name: Name for the output directory structure containing the products
 
         cutoff: Cut off in amplitude for the physical deviation fitting, None means 20%
         panel_kind: Type of fitting function used to fit panel surfaces, defaults to corotated_paraboloid for ringed
                     telescopes
-        unit: Unit for panel adjustments
-        save_mask: Save plot of the mask derived from amplitude cutoff to a png file
-        save_deviations: Save plot of physical deviations to a png file
-        save_phase: Save plot of phases to a png file
         parallel: Run chunks of processing in parallel
         panel_margins: Margin to be ignored at edges of panels when fitting
         sel_ddi: Which DDIs are to be processed by panel, None means all of them
         overwrite: Overwrite previous hack_file of same name?
     """
 
     panel_params = {'image_name': image_name,
                     'panel_name': panel_name,
                     'cutoff': cutoff,
                     'panel_kind': panel_kind,
-                    'unit': unit,
                     'panel_margins': panel_margins,
-                    'save_mask': save_mask,
-                    'save_deviations': save_deviations,
-                    'save_phase': save_phase,
                     'parallel': parallel,
                     'sel_ddi': sel_ddi,
                     'overwrite': overwrite
                     }
                           
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(panel_params, 'image_name', [str], default=None)
     base_name = _remove_suffix(panel_params['image_name'], '.image.zarr')
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_name', [str], default=base_name+'.panel.zarr')
     parms_passed = parms_passed and _check_parms(panel_params, 'cutoff', [float], acceptable_range=[0, 1], default=0.2)
-    parms_passed = parms_passed and _check_parms(panel_params, 'panel_kind', [str], acceptable_data=panelkinds, default="rigid")
-    parms_passed = parms_passed and _check_parms(panel_params, 'unit', [str], acceptable_data=length_units, default="mm")
+    parms_passed = parms_passed and _check_parms(panel_params, 'panel_kind', [str], acceptable_data=panel_models, default="rigid")
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_margins', [float], acceptable_range=[0, 0.5], default=0.2)
-    parms_passed = parms_passed and _check_parms(panel_params, 'save_mask', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(panel_params, 'save_deviations', [bool], default=False)
-    parms_passed = parms_passed and _check_parms(panel_params, 'save_phase', [bool], default=False)
     parms_passed = parms_passed and _check_parms(panel_params, 'parallel', [bool], default=False)
     parms_passed = parms_passed and _check_parms(panel_params, 'sel_ddi', [list, np.array], list_acceptable_data_types=[int, np.int], default='all')
     parms_passed = parms_passed and _check_parms(panel_params, 'overwrite', [bool], default=False)
 
     if not parms_passed:
         logger.error("extract_holog parameter checking failed.")
         raise Exception("extract_holog parameter checking failed.")
```

### Comparing `astrohack-0.0.5/src/astrohack/profiling.py` & `astrohack-0.0.6/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack/visualization/viewer.py` & `astrohack-0.0.6/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.0.6/src/astrohack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 # astroHACK
```

### Comparing `astrohack-0.0.5/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.0.6/src/astrohack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,11 +35,12 @@
 src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
 src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
 src/astrohack/_utils/_logger/__init__.py
 src/astrohack/_utils/_logger/_astrohack_logger.py
 src/astrohack/_utils/_parm_utils/__init__.py
 src/astrohack/_utils/_parm_utils/_check_logger_parms.py
 src/astrohack/_utils/_parm_utils/_check_parms.py
+src/astrohack/data/telescopes/__init__.py
 src/astrohack/visualization/__init__.py
 src/astrohack/visualization/viewer.py
 tests/test_class_base_panel.py
 tests/test_class_ring_panel.py
```

### Comparing `astrohack-0.0.5/src/astrohack.egg-info/requires.txt` & `astrohack-0.0.6/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.5/tests/test_class_base_panel.py` & `astrohack-0.0.6/tests/test_class_base_panel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,99 @@
 import pytest
 
 from astrohack._classes.base_panel import _gauss_elimination_numpy, BasePanel, \
-     panelkinds, imean, irigid, icorscp, icorlst, ixypara, icorrob, irotpara, ifulllst
+     panel_models, imean, irigid, icorscp, icorlst, ixypara, icorrob, irotpara, ifulllst
 from astrohack._utils._conversion import _convert_unit
 import numpy as np
 
 
 class TestBasePanel:
     tolerance = 1e-6
-    meta = ['test','test']
 
     def test_gauss_elimination_numpy(self):
         """
         Tests the gaussian elimination routine by using an identity matrix
         """
         size = 3
         identity = np.identity(size)
         vector = np.arange(size)
         for pos in range(size):
             assert _gauss_elimination_numpy(identity, vector)[pos] == vector[pos], 'Gaussian elimination failed'
 
     def test_init(self):
         screws = np.zeros([4, 2])
         label = 'TEST'
-        lepanel = BasePanel(panelkinds[imean], screws, label, self.meta)
+        lepanel = BasePanel(panel_models[imean], screws, label)
         assert lepanel.label == label, "Internal panel label not what expected"
-        assert lepanel.kind == panelkinds[imean], "Internal kind does not match input"
+        assert lepanel.model == panel_models[imean], "Internal model does not match input"
         assert lepanel.samples == [], 'List of samples should be empty'
         assert lepanel.margins == [], 'list of pixels in the margin should be empty'
         assert lepanel.corr is None, 'List of corrections should be None'
         assert not lepanel.solved, 'Panel cannot be solved at creation'
         with pytest.raises(Exception):
-            lepanel = BasePanel('xxx', screws, label, self.meta)
+            lepanel = BasePanel('xxx', screws, label)
 
     def test_add_point(self):
         """
         Test the add point common function
         """
         screws = np.zeros([4, 2])
         ipanel = 0
-        lepanel = BasePanel(panelkinds[imean], ipanel, screws, self.meta)
+        lepanel = BasePanel(panel_models[imean], ipanel, screws)
         nsamp = 30
         point = [0, 0, 0, 0, 0]
         for i in range(nsamp):
             lepanel.add_sample(point)
             lepanel.add_margin(point)
         assert len(lepanel.samples) == nsamp, 'Internal number of samples do not match the expected number of samples'
         assert len(lepanel.margins) == nsamp, 'Internal list of points does not have the expected size'
         for i in range(nsamp):
             assert lepanel.samples[i] == point, '{0:d}-eth point does not match input point'.format(i)
         return
 
-    def test_mean_kind(self):
+    def test_mean_model(self):
         """
-        Tests the whole usage of a panel of the mean kind
+        Tests the whole usage of a panel of the mean model
         """
         expectedmean = 3.5
         point = [0, 0, 0, 0, expectedmean]
         screws = np.zeros([4, 2])
         nsamp = 30
-        meanpanel = BasePanel(panelkinds[imean], screws, 'test', self.meta)
+        meanpanel = BasePanel(panel_models[imean], screws, 'test')
         assert meanpanel._solve_sub == meanpanel._solve_mean, 'Incorrect overloading of mean solving method'
         assert meanpanel.corr_point == meanpanel._corr_point_mean, 'Incorrect overloading of mean point correction ' \
                                                                    'method'
         for i in range(nsamp):
             meanpanel.add_sample(point)
         meanpanel.solve()
         assert abs(meanpanel.par[0] - expectedmean)/expectedmean < self.tolerance, 'Did not recover the expected mean'
         meanpanel.get_corrections()
         assert len(meanpanel.corr) == nsamp, 'Number of corrected points do not match number of samples'
         onecorr = meanpanel.corr_point(0, 0)
         assert abs(onecorr - expectedmean)/expectedmean < self.tolerance, 'Correction for a point did not match the ' \
                                                                           'expected value'
-        mmscrews = meanpanel.export_screws_float(unit='mm')
+        mmscrews = meanpanel.export_screws(unit='mm')
         fac = _convert_unit('m', 'mm', 'length')
         for screw in mmscrews:
             assert abs(screw - fac*expectedmean) < self.tolerance, 'mm screw adjustments not within 0.1% tolerance '\
                                                                       'of the expected value'
-        miscrews = meanpanel.export_screws_float(unit='mils')
+        miscrews = meanpanel.export_screws(unit='mils')
         fac = _convert_unit('m', 'mils', 'length')
         for screw in miscrews:
             assert abs(screw - fac * expectedmean) < 1e-2, 'Miliinches screw adjustments not ' \
                                                                          'within 1% of the expected value'
 
-    def test_rigid_kind(self):
+    def test_rigid_model(self):
         """
-        Tests the whole usage of a panel of the rigid kind
+        Tests the whole usage of a panel of the rigid model
         """
         expectedpar = [3.5, -2, 1]
         screws = np.zeros([4, 2])
         nside = 32
-        rigidpanel = BasePanel(panelkinds[irigid], screws, 'test', self.meta)
+        rigidpanel = BasePanel(panel_models[irigid], screws, 'test')
         assert rigidpanel._solve_sub == rigidpanel._solve_rigid, 'Incorrect overloading of rigid solving method'
         assert rigidpanel.corr_point == rigidpanel._corr_point_rigid, 'Incorrect overloading of rigid point ' \
                                                                       'correction method'
         for ix in range(nside):
             for iy in range(nside):
                 value = ix*expectedpar[0] + iy*expectedpar[1] + expectedpar[2]
                 rigidpanel.add_sample([ix, iy, ix, iy, value])
@@ -103,28 +102,28 @@
             feedback = '{0:d}-eth parameter does not match its expected value'.format(ipar)
             assert abs(rigidpanel.par[ipar]-expectedpar[ipar])/abs(expectedpar[ipar]) < self.tolerance, feedback
         rigidpanel.get_corrections()
         assert len(rigidpanel.corr) == nside**2, 'Number of corrected points do not match number of samples'
         onecorr = rigidpanel.corr_point(0, 0)
         assert abs(onecorr - expectedpar[2])/expectedpar[2] < self.tolerance, 'Correction for a point did not match ' \
                                                                               'the expected value'
-        mmscrews = rigidpanel.export_screws_float()
+        mmscrews = rigidpanel.export_screws()
         fac = _convert_unit('m', 'mm', 'length')
         for screw in mmscrews:
             assert abs(screw - fac*expectedpar[2]) < self.tolerance, 'mm screw adjustments not within 0.1% ' \
                                                                         'tolerance of the expected value'
 
-    def test_xyparaboloid_scipy_kind(self):
+    def test_xyparaboloid_scipy_model(self):
         """
-        Tests the whole usage of a panel of the xyparaboloid kind
+        Tests the whole usage of a panel of the xyparaboloid model
         """
         expectedpar = [150, 10, 2.5]
         screws = np.zeros([4, 2])
         nside = 32
-        xyparapanel = BasePanel(panelkinds[ixypara], screws, 'test', self.meta)
+        xyparapanel = BasePanel(panel_models[ixypara], screws, 'test')
         assert xyparapanel._solve_sub == xyparapanel._solve_scipy, 'Incorrect overloading of scipy solving method'
         assert xyparapanel.corr_point == xyparapanel._corr_point_scipy, 'Incorrect overloading of scipy point ' \
                                                                         'correction method'
         assert xyparapanel._fitting_function == xyparapanel._xyaxes_paraboloid, 'Incorrect overloading of XY '\
                                                                                 'paraboloid function'
         for ix in range(nside):
             for iy in range(nside):
@@ -135,29 +134,29 @@
             feedback = '{0:d}-eth parameter does not match its expected value'.format(ipar)
             assert abs(xyparapanel.par[ipar] - expectedpar[ipar]) / abs(expectedpar[ipar]) < self.tolerance, feedback
         xyparapanel.get_corrections()
         assert len(xyparapanel.corr) == nside ** 2, 'Number of corrected points do not match number of samples'
         onecorr = xyparapanel.corr_point(0, 0)
         assert abs(onecorr - expectedpar[2]) / expectedpar[2] < self.tolerance, 'Correction for a point did not match '\
                                                                                 'the expected value'
-        mmscrews = xyparapanel.export_screws_float()
+        mmscrews = xyparapanel.export_screws()
         fac = _convert_unit('m', 'mm', 'length')
         for screw in mmscrews:
             assert abs(screw - fac*expectedpar[2]) < self.tolerance, 'mm screw adjustments not within 0.1% ' \
                                                                         'tolerance of the expected value'
 
-    def test_rotatedparaboloid_scipy_kind(self):
+    def test_rotatedparaboloid_scipy_model(self):
         """
-        Tests the whole usage of a panel of the rotatedparaboloid kind
+        Tests the whole usage of a panel of the rotatedparaboloid model
         """
         theta = 0
         expectedpar = [39, 10, 2.5, theta]
         screws = np.zeros([4, 2])
         nside = 32
-        rotparapanel = BasePanel(panelkinds[irotpara], screws, 'test', self.meta)
+        rotparapanel = BasePanel(panel_models[irotpara], screws, 'test')
         assert rotparapanel._solve_sub == rotparapanel._solve_scipy, 'Incorrect overloading of scipy solving method'
         assert rotparapanel.corr_point == rotparapanel._corr_point_scipy, 'Incorrect overloading of scipy point ' \
                                                                           'correction method'
         assert rotparapanel._fitting_function == rotparapanel._rotated_paraboloid, 'Incorrect overloading of paraboloid' \
                                                                                    ' function'
         for ix in range(nside):
             for iy in range(nside):
@@ -170,28 +169,28 @@
             feedback = '{0:d}-eth parameter does not match its expected value'.format(ipar)
             assert abs(rotparapanel.par[ipar] - expectedpar[ipar]) / abs(expectedpar[ipar]) < self.tolerance, feedback
         rotparapanel.get_corrections()
         assert len(rotparapanel.corr) == nside ** 2, 'Number of corrected points do not match number of samples'
         onecorr = rotparapanel.corr_point(0, 0)
         assert abs(onecorr - expectedpar[2]) / expectedpar[2] < self.tolerance, 'Correction for a point did not match '\
                                                                                 'the expected value'
-        mmscrews = rotparapanel.export_screws_float()
+        mmscrews = rotparapanel.export_screws()
         fac = _convert_unit('m', 'mm', 'length')
         for screw in mmscrews:
             assert abs(screw - fac*expectedpar[2]) < 1e3*self.tolerance, 'mm screw adjustments not within 0.1% ' \
                                                                         'tolerance of the expected value'
 
-    def test_corotatedparaboloid_scipy_kind(self):
+    def test_corotatedparaboloid_scipy_model(self):
         """
-        Tests the whole usage of a panel of the corotatedparaboloid kind solved with scipy
+        Tests the whole usage of a panel of the corotatedparaboloid model solved with scipy
         """
         expectedpar = [75, 5, -2.0]
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panelkinds[icorscp], screws, 'test', self.meta)
+        corotparapanel = BasePanel(panel_models[icorscp], screws, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_scipy, 'Incorrect overloading of scipy solving method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_scipy, 'Incorrect overloading of scipy point ' \
                                                                               'correction method'
         assert corotparapanel._fitting_function == corotparapanel._corotated_paraboloid, 'Incorrect overloading of ' \
                                                                                          'paraboloid function'
         for ix in range(nside):
             for iy in range(nside):
@@ -202,28 +201,28 @@
             feedback = '{0:d}-eth parameter does not match its expected value'.format(ipar)
             assert abs(corotparapanel.par[ipar] - expectedpar[ipar]) / abs(expectedpar[ipar]) < self.tolerance, feedback
         corotparapanel.get_corrections()
         assert len(corotparapanel.corr) == nside ** 2, 'Number of corrected points do not match number of samples'
         onecorr = corotparapanel.corr_point(0, 0)
         assert abs(onecorr - expectedpar[2]) / expectedpar[2] < self.tolerance, 'Correction for a point did not match ' \
                                                                                 'the expected value'
-        mmscrews = corotparapanel.export_screws_float()
+        mmscrews = corotparapanel.export_screws()
         fac = _convert_unit('m', 'mm', 'length')
         for screw in mmscrews:
             assert abs(screw - fac * expectedpar[2]) < self.tolerance, 'mm screw adjustments not within 0.1% ' \
                                                                        'tolerance of the expected value'
 
-    def test_corotatedparaboloid_lst_kind(self):
+    def test_corotatedparaboloid_lst_model(self):
         """
-        Tests the whole usage of a panel of the corotatedparaboloid kind
+        Tests the whole usage of a panel of the corotatedparaboloid model
         """
         expectedpar = [75, 5, -2.0]
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panelkinds[icorlst], screws, 'test', self.meta)
+        corotparapanel = BasePanel(panel_models[icorlst], screws, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_corotated_lst_sq, 'Incorrect overloading of ' \
                                                                                     'corotated least squares solving ' \
                                                                                     'method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_corotated_lst_sq, 'Incorrect overloading of ' \
                                                                                          'corotated least squares ' \
                                                                                          'point correction method'
         for ix in range(nside):
@@ -235,28 +234,28 @@
             feedback = '{0:d}-eth parameter does not match its expected value'.format(ipar)
             assert abs(corotparapanel.par[ipar] - expectedpar[ipar]) / abs(expectedpar[ipar]) < self.tolerance, feedback
         corotparapanel.get_corrections()
         assert len(corotparapanel.corr) == nside ** 2, 'Number of corrected points do not match number of samples'
         onecorr = corotparapanel.corr_point(0, 0)
         assert abs(onecorr - expectedpar[2]) / expectedpar[2] < self.tolerance, 'Correction for a point did not match ' \
                                                                                 'the expected value'
-        mmscrews = corotparapanel.export_screws_float()
+        mmscrews = corotparapanel.export_screws()
         fac = _convert_unit('m', 'mm', 'length')
         for screw in mmscrews:
             assert abs(screw - fac * expectedpar[2]) < self.tolerance, 'mm screw adjustments not within 0.1% ' \
                                                                        'tolerance of the expected value'
 
-    def test_corotatedparaboloid_robust_kind(self):
+    def test_corotatedparaboloid_robust_model(self):
         """
-        Tests the whole usage of a panel of the corotatedparaboloid kind
+        Tests the whole usage of a panel of the corotatedparaboloid model
         """
         expectedpar = [75, 5, -2.0]
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panelkinds[icorrob], screws, 'test', self.meta)
+        corotparapanel = BasePanel(panel_models[icorrob], screws, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_robust, 'Incorrect overloading of robust solving ' \
                                                                           'method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_corotated_lst_sq, 'Incorrect overloading of ' \
                                                                                          'corotated least squares ' \
                                                                                          'correction method'
         assert corotparapanel._fitting_function == corotparapanel._corotated_paraboloid, 'Incorrect overloading of ' \
                                                                                          'paraboloid function'
@@ -269,29 +268,29 @@
             feedback = '{0:d}-eth parameter does not match its expected value'.format(ipar)
             assert abs(corotparapanel.par[ipar] - expectedpar[ipar]) / abs(expectedpar[ipar]) < self.tolerance, feedback
         corotparapanel.get_corrections()
         assert len(corotparapanel.corr) == nside ** 2, 'Number of corrected points do not match number of samples'
         onecorr = corotparapanel.corr_point(0, 0)
         assert abs(onecorr - expectedpar[2]) / expectedpar[2] < self.tolerance, 'Correction for a point did not match ' \
                                                                                 'the expected value'
-        mmscrews = corotparapanel.export_screws_float()
+        mmscrews = corotparapanel.export_screws()
         fac = _convert_unit('m', 'mm', 'length')
         for screw in mmscrews:
             assert abs(screw - fac * expectedpar[2]) < self.tolerance, 'mm screw adjustments not within 0.1% ' \
                                                                        'tolerance of the expected value'
 
-    def test_fullparaboloid_lst_kind(self):
+    def test_fullparaboloid_lst_model(self):
         """
-        Tests the whole usage of a panel of the corotatedparaboloid kind
+        Tests the whole usage of a panel of the corotatedparaboloid model
         """
         expectedpar = [75, 5, -2.0, 3, -6, 8, 16, -3.5, 8]
         expectedscrew = 8000
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panelkinds[ifulllst], screws, 'test', self.meta)
+        corotparapanel = BasePanel(panel_models[ifulllst], screws, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_least_squares_paraboloid, 'Incorrect overloading of ' \
                                                                                             'full least squares ' \
                                                                                             'solving method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_least_squares_paraboloid, 'Incorrect ' \
                                                                                                  'overloading of full' \
                                                                                                  ' least squares ' \
                                                                                                  'point correction ' \
@@ -309,11 +308,11 @@
             feedback = '{0:d}-eth parameter does not match its expected value'.format(ipar)
             assert abs(corotparapanel.par[ipar] - expectedpar[ipar]) / abs(expectedpar[ipar]) < self.tolerance, feedback
         corotparapanel.get_corrections()
         assert len(corotparapanel.corr) == nside ** 2, 'Number of corrected points do not match number of samples'
         onecorr = corotparapanel.corr_point(0, 0)
         assert abs(onecorr - expectedpar[2]) / expectedpar[2] < self.tolerance, 'Correction for a point did not match ' \
                                                                                 'the expected value'
-        mmscrews = corotparapanel.export_screws_float()
+        mmscrews = corotparapanel.export_screws()
         for screw in mmscrews:
             assert abs(screw - expectedscrew) < 1e3*self.tolerance, 'mm screw adjustments not within 0.1% ' \
                                                                           'tolerance of the expected value'
```

### Comparing `astrohack-0.0.5/tests/test_class_ring_panel.py` & `astrohack-0.0.6/tests/test_class_ring_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,16 @@
     inrad = 2.0
     ourad = 3.0
     angle = np.pi / 2
     ipanel = 1
     deviation = 2.0
     point = [2.5, -2.5, 1, 1, deviation]
     label = 'test'
-    meta  = 'test_ant'
     margin = 0.2
-    panel = RingPanel('rigid', angle, ipanel, label, inrad, ourad, meta, margin=margin)
+    panel = RingPanel('rigid', angle, ipanel, label, inrad, ourad, margin=margin)
 
     def test_init(self):
         """
         Tests the correct initialization of a RingPanel object, not all parameters tested
         """
         theta_margin = self.margin*self.angle
         radius_margin = self.margin*(self.ourad-self.inrad)
```

