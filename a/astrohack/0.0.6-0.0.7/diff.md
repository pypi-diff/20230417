# Comparing `tmp/astrohack-0.0.6.tar.gz` & `tmp/astrohack-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.0.6.tar", last modified: Mon Apr 17 17:07:41 2023, max compression
+gzip compressed data, was "astrohack-0.0.7.tar", last modified: Mon Apr 17 18:01:16 2023, max compression
```

## Comparing `astrohack-0.0.6.tar` & `astrohack-0.0.7.tar`

### file list

```diff
@@ -1,61 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 17:07:41.110303 astrohack-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 17:07:23.000000 astrohack-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:23.000000 astrohack-0.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 17:07:24.000000 astrohack-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:07:41.110303 astrohack-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.102303 astrohack-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.106303 astrohack-0.0.6/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.106303 astrohack-0.0.6/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    27476 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_dio_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    33916 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/astrohack_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.102303 astrohack-0.0.6/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/data/telescopes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-17 17:07:24.000000 astrohack-0.0.6/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.106303 astrohack-0.0.6/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 17:07:41.000000 astrohack-0.0.6/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:07:41.110303 astrohack-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-17 17:07:24.000000 astrohack-0.0.6/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-17 17:07:24.000000 astrohack-0.0.6/tests/test_class_ring_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.481204 astrohack-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 18:00:59.000000 astrohack-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:00:59.000000 astrohack-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 18:01:16.477204 astrohack-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 18:00:59.000000 astrohack-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:00:59.000000 astrohack-0.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-17 18:00:59.000000 astrohack-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:01:16.481204 astrohack-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.469204 astrohack-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    27476 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_dio_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33916 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27130 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/_utils/gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/astrohack_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.469204 astrohack-0.0.7/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15467 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-17 18:00:59.000000 astrohack-0.0.7/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.473204 astrohack-0.0.7/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 18:01:16.000000 astrohack-0.0.7/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:01:16.477204 astrohack-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-17 18:00:59.000000 astrohack-0.0.7/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-17 18:00:59.000000 astrohack-0.0.7/tests/test_class_ring_panel.py
```

### Comparing `astrohack-0.0.6/PKG-INFO` & `astrohack-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.6
+Version: 0.0.7
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENSE
 
 # astroHACK
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `astrohack-0.0.6/README.md` & `astrohack-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/pyproject.toml` & `astrohack-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.0.6"
+version = "0.0.7"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.0.6/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.0.7/src/astrohack/_classes/antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_classes/base_panel.py` & `astrohack-0.0.7/src/astrohack/_classes/base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.0.7/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_classes/ring_panel.py` & `astrohack-0.0.7/src/astrohack/_classes/ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_classes/telescope.py` & `astrohack-0.0.7/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_algorithms.py` & `astrohack-0.0.7/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_constants.py` & `astrohack-0.0.7/src/astrohack/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_conversion.py` & `astrohack-0.0.7/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.0.7/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_dio_classes.py` & `astrohack-0.0.7/src/astrohack/_utils/_dio_classes.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_holog.py` & `astrohack-0.0.7/src/astrohack/_utils/_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_imaging.py` & `astrohack-0.0.7/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_io.py` & `astrohack-0.0.7/src/astrohack/_utils/_io.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.0.7/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_panel.py` & `astrohack-0.0.7/src/astrohack/_utils/_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.0.7/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.0.7/src/astrohack/_utils/gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/astrohack_client.py` & `astrohack-0.0.7/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/dio.py` & `astrohack-0.0.7/src/astrohack/dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/extract_holog.py` & `astrohack-0.0.7/src/astrohack/extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/gdown_utils.py` & `astrohack-0.0.7/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/holog.py` & `astrohack-0.0.7/src/astrohack/holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/panel.py` & `astrohack-0.0.7/src/astrohack/panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/profiling.py` & `astrohack-0.0.7/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack/visualization/viewer.py` & `astrohack-0.0.7/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.0.7/src/astrohack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.0.6
+Version: 0.0.7
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+License-File: LICENSE
 
 # astroHACK
 
 [![Python 3.8 3.9 3.10](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/astrohack/badge/?version=latest)](https://astrohack.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `astrohack-0.0.6/src/astrohack.egg-info/requires.txt` & `astrohack-0.0.7/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/tests/test_class_base_panel.py` & `astrohack-0.0.7/tests/test_class_base_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.0.6/tests/test_class_ring_panel.py` & `astrohack-0.0.7/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

