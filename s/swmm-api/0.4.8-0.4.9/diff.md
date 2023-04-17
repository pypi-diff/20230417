# Comparing `tmp/swmm-api-0.4.8.tar.gz` & `tmp/swmm-api-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swmm-api-0.4.8.tar", last modified: Thu Mar  9 10:04:18 2023, max compression
+gzip compressed data, was "swmm-api-0.4.9.tar", last modified: Thu Mar  9 15:17:50 2023, max compression
```

## Comparing `swmm-api-0.4.8.tar` & `swmm-api-0.4.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.750868 swmm-api-0.4.8/
--rwxrwxrwx   0 mp        (1000) mp        (1000)     1063 2023-03-09 10:04:09.000000 swmm-api-0.4.8/LICENSE
--rw-r--r--   0 mp        (1000) mp        (1000)    14256 2023-03-09 10:04:18.750868 swmm-api-0.4.8/PKG-INFO
--rwxrwxrwx   0 mp        (1000) mp        (1000)    13194 2023-03-09 10:04:09.000000 swmm-api-0.4.8/README.md
--rw-rw-rw-   0 mp        (1000) mp        (1000)     2110 2023-03-09 10:04:10.000000 swmm-api-0.4.8/pyproject.toml
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1527 2023-03-09 10:04:18.751868 swmm-api-0.4.8/setup.cfg
--rw-rw-rw-   0 mp        (1000) mp        (1000)      114 2023-03-09 10:04:10.000000 swmm-api-0.4.8/setup.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.720865 swmm-api-0.4.8/swmm_api/
--rwxrwxrwx   0 mp        (1000) mp        (1000)      509 2023-03-09 10:04:15.000000 swmm-api-0.4.8/swmm_api/__init__.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.725866 swmm-api-0.4.8/swmm_api/_io_helpers/
--rw-rw-rw-   0 mp        (1000) mp        (1000)      161 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/_io_helpers/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)      374 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/_io_helpers/_config.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1950 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/_io_helpers/_encoding.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     3274 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/_io_helpers/_read_bin.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1028 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/_io_helpers/_read_txt.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.726866 swmm-api-0.4.8/swmm_api/hotstart_file/
--rw-rw-rw-   0 mp        (1000) mp        (1000)       44 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/hotstart_file/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     9793 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/hotstart_file/hst.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.729866 swmm-api-0.4.8/swmm_api/input_file/
--rwxrwxrwx   0 mp        (1000) mp        (1000)       93 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     7062 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/_type_converter.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    37329 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/helpers.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     2897 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/helpers_dummy.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    28523 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/inp.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.730866 swmm-api-0.4.8/swmm_api/input_file/macro_snippets/
--rw-rw-rw-   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macro_snippets/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     3028 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macro_snippets/plot_macros_bokeh.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     3891 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macro_snippets/plotly_map.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.739867 swmm-api-0.4.8/swmm_api/input_file/macros/
--rw-rw-rw-   0 mp        (1000) mp        (1000)     3093 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     3258 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/_combined_objects.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)      762 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/_helpers.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     2463 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/_snippets.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     5658 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/check.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     2063 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/collection.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     8957 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/compare.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     6996 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/convert_model.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     4902 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/convert_object.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     4443 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/cross_section_curve.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1724 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/curve.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    22757 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/edit.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     5581 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/filter.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     4880 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/geo.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    16556 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/gis.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     9441 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/graph.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     9647 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/macros.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     9704 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/plotting_longitudinal.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    11475 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/plotting_map.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     6543 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/reduce_unneeded.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1373 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/split_inp_file.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)      615 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/summarize.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     2482 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/macros/tags.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.741867 swmm-api-0.4.8/swmm_api/input_file/misc/
--rwxrwxrwx   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/misc/__init__.py
--rwxrwxrwx   0 mp        (1000) mp        (1000)     2225 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/misc/climate_file.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1366 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/misc/curve_simplification.py
--rwxrwxrwx   0 mp        (1000) mp        (1000)     6450 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/misc/dat_timeseries.py
--rwxrwxrwx   0 mp        (1000) mp        (1000)     2183 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/misc/following_values.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     8296 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/misc/macro_class.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     3699 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/section_labels.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)      392 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/section_lists.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1980 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/section_types.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.745867 swmm-api-0.4.8/swmm_api/input_file/sections/
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1123 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)      321 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/_identifiers.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    56637 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/generic_section.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    25141 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/lid.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    22123 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/link.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    14072 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/link_component.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    27006 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/node.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    15248 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/node_component.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    98676 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/others.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    32886 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/input_file/sections/subcatch.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.747868 swmm-api-0.4.8/swmm_api/output_file/
--rwxrwxrwx   0 mp        (1000) mp        (1000)      131 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/output_file/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     8518 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/output_file/definitions.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     9039 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/output_file/error_codes.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    15547 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/output_file/extract.py
--rwxrwxrwx   0 mp        (1000) mp        (1000)    14885 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/output_file/out.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     3694 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/output_file/parquet_helpers.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.748868 swmm-api-0.4.8/swmm_api/report_file/
--rwxrwxrwx   0 mp        (1000) mp        (1000)       43 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/report_file/__init__.py
--rwxrwxrwx   0 mp        (1000) mp        (1000)     8544 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/report_file/helpers.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)    34371 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/report_file/rpt.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.750868 swmm-api-0.4.8/swmm_api/run_swmm/
--rw-rw-rw-   0 mp        (1000) mp        (1000)      449 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/run_swmm/__init__.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1541 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/run_swmm/_run_helpers.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1576 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/run_swmm/run.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     6692 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/run_swmm/run_epaswmm.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1219 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/run_swmm/run_pyswmm.py
--rw-rw-rw-   0 mp        (1000) mp        (1000)     1752 2023-03-09 10:04:10.000000 swmm-api-0.4.8/swmm_api/run_swmm/run_swmm_toolkit.py
-drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 10:04:18.723866 swmm-api-0.4.8/swmm_api.egg-info/
--rw-r--r--   0 mp        (1000) mp        (1000)    14256 2023-03-09 10:04:18.000000 swmm-api-0.4.8/swmm_api.egg-info/PKG-INFO
--rw-r--r--   0 mp        (1000) mp        (1000)     2986 2023-03-09 10:04:18.000000 swmm-api-0.4.8/swmm_api.egg-info/SOURCES.txt
--rw-r--r--   0 mp        (1000) mp        (1000)        1 2023-03-09 10:04:18.000000 swmm-api-0.4.8/swmm_api.egg-info/dependency_links.txt
--rw-r--r--   0 mp        (1000) mp        (1000)      390 2023-03-09 10:04:18.000000 swmm-api-0.4.8/swmm_api.egg-info/requires.txt
--rw-r--r--   0 mp        (1000) mp        (1000)        9 2023-03-09 10:04:18.000000 swmm-api-0.4.8/swmm_api.egg-info/top_level.txt
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.276741 swmm-api-0.4.9/
+-rwxrwxrwx   0 mp        (1000) mp        (1000)     1063 2023-03-09 15:17:41.000000 swmm-api-0.4.9/LICENSE
+-rw-r--r--   0 mp        (1000) mp        (1000)    14256 2023-03-09 15:17:50.276741 swmm-api-0.4.9/PKG-INFO
+-rwxrwxrwx   0 mp        (1000) mp        (1000)    13194 2023-03-09 15:17:41.000000 swmm-api-0.4.9/README.md
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     2110 2023-03-09 15:17:42.000000 swmm-api-0.4.9/pyproject.toml
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1527 2023-03-09 15:17:50.277741 swmm-api-0.4.9/setup.cfg
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      114 2023-03-09 15:17:42.000000 swmm-api-0.4.9/setup.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.243741 swmm-api-0.4.9/swmm_api/
+-rwxrwxrwx   0 mp        (1000) mp        (1000)      509 2023-03-09 15:17:46.000000 swmm-api-0.4.9/swmm_api/__init__.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.248741 swmm-api-0.4.9/swmm_api/_io_helpers/
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      161 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/_io_helpers/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      374 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/_io_helpers/_config.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1950 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/_io_helpers/_encoding.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     3274 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/_io_helpers/_read_bin.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1028 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/_io_helpers/_read_txt.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.249741 swmm-api-0.4.9/swmm_api/hotstart_file/
+-rw-rw-rw-   0 mp        (1000) mp        (1000)       44 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/hotstart_file/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     9793 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/hotstart_file/hst.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.252741 swmm-api-0.4.9/swmm_api/input_file/
+-rwxrwxrwx   0 mp        (1000) mp        (1000)       93 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     7062 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/_type_converter.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    37329 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/helpers.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     2897 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/helpers_dummy.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    28523 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/inp.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.253741 swmm-api-0.4.9/swmm_api/input_file/macro_snippets/
+-rw-rw-rw-   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macro_snippets/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     3028 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macro_snippets/plot_macros_bokeh.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     3891 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macro_snippets/plotly_map.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.264741 swmm-api-0.4.9/swmm_api/input_file/macros/
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     3093 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     3258 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/_combined_objects.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      762 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/_helpers.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     2463 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/_snippets.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     5658 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/check.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     2063 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/collection.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     8957 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/compare.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     6996 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/convert_model.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     4902 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/convert_object.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     4443 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/cross_section_curve.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1724 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/curve.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    22757 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/edit.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     5581 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/filter.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     4880 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/geo.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    16556 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/gis.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     9441 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/graph.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     9647 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/macros.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     9704 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/plotting_longitudinal.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    11475 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/plotting_map.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     6543 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/reduce_unneeded.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1373 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/split_inp_file.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      615 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/summarize.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     2482 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/macros/tags.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.266741 swmm-api-0.4.9/swmm_api/input_file/misc/
+-rwxrwxrwx   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/misc/__init__.py
+-rwxrwxrwx   0 mp        (1000) mp        (1000)     2225 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/misc/climate_file.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1366 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/misc/curve_simplification.py
+-rwxrwxrwx   0 mp        (1000) mp        (1000)     6450 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/misc/dat_timeseries.py
+-rwxrwxrwx   0 mp        (1000) mp        (1000)     2183 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/misc/following_values.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     8296 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/misc/macro_class.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     3699 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/section_labels.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      392 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/section_lists.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1980 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/section_types.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.270741 swmm-api-0.4.9/swmm_api/input_file/sections/
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1123 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      321 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/_identifiers.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    56637 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/generic_section.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    25141 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/lid.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    22123 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/link.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    14072 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/link_component.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    27006 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/node.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    15248 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/node_component.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    98676 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/others.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    32886 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/input_file/sections/subcatch.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.272741 swmm-api-0.4.9/swmm_api/output_file/
+-rwxrwxrwx   0 mp        (1000) mp        (1000)      131 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/output_file/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     8518 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/output_file/definitions.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     9039 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/output_file/error_codes.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    15776 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/output_file/extract.py
+-rwxrwxrwx   0 mp        (1000) mp        (1000)    15127 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/output_file/out.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     3694 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/output_file/parquet_helpers.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.273741 swmm-api-0.4.9/swmm_api/report_file/
+-rwxrwxrwx   0 mp        (1000) mp        (1000)       43 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/report_file/__init__.py
+-rwxrwxrwx   0 mp        (1000) mp        (1000)     8544 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/report_file/helpers.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)    34371 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/report_file/rpt.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.276741 swmm-api-0.4.9/swmm_api/run_swmm/
+-rw-rw-rw-   0 mp        (1000) mp        (1000)      449 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/run_swmm/__init__.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1541 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/run_swmm/_run_helpers.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1576 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/run_swmm/run.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     6692 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/run_swmm/run_epaswmm.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1219 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/run_swmm/run_pyswmm.py
+-rw-rw-rw-   0 mp        (1000) mp        (1000)     1752 2023-03-09 15:17:42.000000 swmm-api-0.4.9/swmm_api/run_swmm/run_swmm_toolkit.py
+drwxr-xr-x   0 mp        (1000) mp        (1000)        0 2023-03-09 15:17:50.246741 swmm-api-0.4.9/swmm_api.egg-info/
+-rw-r--r--   0 mp        (1000) mp        (1000)    14256 2023-03-09 15:17:50.000000 swmm-api-0.4.9/swmm_api.egg-info/PKG-INFO
+-rw-r--r--   0 mp        (1000) mp        (1000)     2986 2023-03-09 15:17:50.000000 swmm-api-0.4.9/swmm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 mp        (1000) mp        (1000)        1 2023-03-09 15:17:50.000000 swmm-api-0.4.9/swmm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 mp        (1000) mp        (1000)      390 2023-03-09 15:17:50.000000 swmm-api-0.4.9/swmm_api.egg-info/requires.txt
+-rw-r--r--   0 mp        (1000) mp        (1000)        9 2023-03-09 15:17:50.000000 swmm-api-0.4.9/swmm_api.egg-info/top_level.txt
```

### Comparing `swmm-api-0.4.8/LICENSE` & `swmm-api-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/PKG-INFO` & `swmm-api-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swmm-api
-Version: 0.4.8
+Version: 0.4.9
 Summary: US-EPA-SWMM python interface
 Home-page: https://gitlab.com/markuspichler/swmm_api
 Author: Markus Pichler
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspichler.gitlab.io/swmm_api
 Project-URL: Changelog, https://gitlab.com/markuspichler/swmm_api/-/blob/master/CHANGELOG.md
```

### Comparing `swmm-api-0.4.8/README.md` & `swmm-api-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/pyproject.toml` & `swmm-api-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/setup.cfg` & `swmm-api-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/_io_helpers/_encoding.py` & `swmm-api-0.4.9/swmm_api/_io_helpers/_encoding.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/_io_helpers/_read_bin.py` & `swmm-api-0.4.9/swmm_api/_io_helpers/_read_bin.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/_io_helpers/_read_txt.py` & `swmm-api-0.4.9/swmm_api/_io_helpers/_read_txt.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/hotstart_file/hst.py` & `swmm-api-0.4.9/swmm_api/hotstart_file/hst.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/_type_converter.py` & `swmm-api-0.4.9/swmm_api/input_file/_type_converter.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/helpers.py` & `swmm-api-0.4.9/swmm_api/input_file/helpers.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/helpers_dummy.py` & `swmm-api-0.4.9/swmm_api/input_file/helpers_dummy.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/inp.py` & `swmm-api-0.4.9/swmm_api/input_file/inp.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macro_snippets/plot_macros_bokeh.py` & `swmm-api-0.4.9/swmm_api/input_file/macro_snippets/plot_macros_bokeh.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macro_snippets/plotly_map.py` & `swmm-api-0.4.9/swmm_api/input_file/macro_snippets/plotly_map.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/__init__.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/_combined_objects.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/_combined_objects.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/_helpers.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/_helpers.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/_snippets.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/_snippets.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/check.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/check.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/collection.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/collection.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/compare.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/compare.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/convert_model.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/convert_model.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/convert_object.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/convert_object.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/cross_section_curve.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/cross_section_curve.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/curve.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/curve.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/edit.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/edit.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/filter.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/filter.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/geo.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/geo.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/gis.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/gis.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/graph.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/graph.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/macros.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/macros.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/plotting_longitudinal.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/plotting_longitudinal.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/plotting_map.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/plotting_map.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/reduce_unneeded.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/reduce_unneeded.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/split_inp_file.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/split_inp_file.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/summarize.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/summarize.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/macros/tags.py` & `swmm-api-0.4.9/swmm_api/input_file/macros/tags.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/misc/climate_file.py` & `swmm-api-0.4.9/swmm_api/input_file/misc/climate_file.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/misc/curve_simplification.py` & `swmm-api-0.4.9/swmm_api/input_file/misc/curve_simplification.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/misc/dat_timeseries.py` & `swmm-api-0.4.9/swmm_api/input_file/misc/dat_timeseries.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/misc/following_values.py` & `swmm-api-0.4.9/swmm_api/input_file/misc/following_values.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/misc/macro_class.py` & `swmm-api-0.4.9/swmm_api/input_file/misc/macro_class.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/section_labels.py` & `swmm-api-0.4.9/swmm_api/input_file/section_labels.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/section_types.py` & `swmm-api-0.4.9/swmm_api/input_file/section_types.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/__init__.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/generic_section.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/generic_section.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/lid.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/lid.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/link.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/link.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/link_component.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/link_component.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/node.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/node.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/node_component.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/node_component.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/others.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/others.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/input_file/sections/subcatch.py` & `swmm-api-0.4.9/swmm_api/input_file/sections/subcatch.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/output_file/definitions.py` & `swmm-api-0.4.9/swmm_api/output_file/definitions.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/output_file/error_codes.py` & `swmm-api-0.4.9/swmm_api/output_file/error_codes.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/output_file/extract.py` & `swmm-api-0.4.9/swmm_api/output_file/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 import copy
 
 import datetime
 from io import SEEK_END, SEEK_SET
 from pathlib import Path
 
-from tqdm.auto import tqdm
 from warnings import warn
 
 from .definitions import OBJECTS, VARIABLES
 from .._io_helpers._read_bin import BinaryReader
 
 VARIABLES_DICT = {
     OBJECTS.SUBCATCHMENT: VARIABLES.SUBCATCHMENT.LIST_,
@@ -265,23 +264,25 @@
         _bytes_per_period = 2  # for the datetime
         for obj in [OBJECTS.SUBCATCHMENT, OBJECTS.NODE, OBJECTS.LINK]:
             _bytes_per_period += len(self.variables[obj]) * len(self.labels[obj])
         _bytes_per_period += len(self.variables[OBJECTS.SYSTEM])
         _bytes_per_period *= _RECORDSIZE
         return _bytes_per_period
 
-    def _get_selective_results(self, columns, processes=1):
+    def _get_selective_results(self, columns, processes=1, show_progress=True):
         """
         get results of selective columns in .out-file
 
         this function is due to its iterative reading slow,
         but has it advantages with out-files with many columns (>1000) and fewer time-steps
 
         Args:
             columns (list[tuple]): list of column identifier tuple with [(kind, label, variable), ...]
+            processes (int): number of parallel processes.
+            show_progress (bool): show a progress bar.
 
         Returns:
             dict[str, list]: dictionary where keys are the column names ('/' as separator) and values are the list of result values
         """
         n_vars_subcatch = len(self.variables[OBJECTS.SUBCATCHMENT])
         n_vars_node = len(self.variables[OBJECTS.NODE])
         n_vars_link = len(self.variables[OBJECTS.LINK])
@@ -336,14 +337,19 @@
         #         self._set_position(offset + period_offset)
         #         values[label].append(self._next_float())
 
         # -------------
         from functools import partial
         from itertools import cycle
 
+        if show_progress:
+            from tqdm.auto import tqdm
+        else:
+            tqdm = lambda _, desc=None: _
+
         if processes == 1:
             for period_offset in tqdm(variable, desc=f'{repr(self)}.get_selective_results(n_cols={len(columns)})'):
                 func(self, period_offset)
 
         else:
             from multiprocessing.dummy import Pool
```

### Comparing `swmm-api-0.4.8/swmm_api/output_file/out.py` & `swmm-api-0.4.9/swmm_api/output_file/out.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __version__ = "0.1"
 __license__ = "MIT"
 
 import datetime
 import warnings
 from itertools import product
 from numpy import dtype, fromfile, frombuffer
-from pandas import date_range, DataFrame, MultiIndex
+from pandas import date_range, DataFrame, MultiIndex, Index
 from pandas._libs import OutOfBoundsDatetime
 
 from .extract import SwmmOutExtract
 from .definitions import OBJECTS, VARIABLES
 
 from . import parquet_helpers as parquet
 
@@ -70,15 +70,15 @@
         if skip_init:
             return
 
         # the main datetime index for the results
         try:
             self.index = date_range(self.start_date, periods=self.n_periods, freq=self.report_interval)
         except OutOfBoundsDatetime:
-            self.index = [self.start_date * i for i in range(self.n_periods)]
+            self.index = Index([self.start_date + self.report_interval * i for i in range(self.n_periods)])
 
     def __repr__(self):
         return f'SwmmOutput(file="{self.filename}")'
 
     def _get_dtypes(self):
         """
         Get the dtypes of the data.
@@ -143,15 +143,15 @@
             pandas.DataFrame: data
         """
         if self._frame is None:
             self._frame = self._to_pandas(self.to_numpy())
             del self._frame['datetime']
         return self._frame
 
-    def get_part(self, kind=None, label=None, variable=None, slim=False, processes=1):
+    def get_part(self, kind=None, label=None, variable=None, slim=False, processes=1, show_progress=True):
         """
         Get specific columns of the data.
 
         .. Important::
             Set the parameter ``slim`` to ``True`` to speedup the code if you just want a few columns and
             there are a lot of objects (many columns) and just few time-steps (fewer rows) in the out-file.
 
@@ -196,22 +196,24 @@
                     - ``flooding`` or :attr:`~swmm_api.output_file.definitions.SYSTEM_VARIABLES.FLOODING`
                     - ``outflow`` or :attr:`~swmm_api.output_file.definitions.SYSTEM_VARIABLES.OUTFLOW`
                     - ``volume`` or :attr:`~swmm_api.output_file.definitions.SYSTEM_VARIABLES.VOLUME`
                     - ``evaporation`` or :attr:`~swmm_api.output_file.definitions.SYSTEM_VARIABLES.EVAPORATION`
                     - ``PET`` or :attr:`~swmm_api.output_file.definitions.SYSTEM_VARIABLES.PET`
 
             slim (bool): set to ``True`` to speedup the code if there are a lot of objects and just few time-steps in the out-file.
+            processes (int): number of parallel processes for the slim-reading.
+            show_progress (bool): show a progress bar for the slim-reading.
 
         Returns:
             pandas.DataFrame | pandas.Series: Filtered data.
                 (return Series if only one column is selected otherwise return a DataFrame)
         """
         columns = self._filter_part_columns(kind, label, variable)
         if slim:
-            values = self._get_selective_results(columns, processes=processes)
+            values = self._get_selective_results(columns, processes=processes, show_progress=show_progress)
         else:
             values = self.to_numpy()[list(map('/'.join, columns))]
 
         return self._to_pandas(values, drop_useless=True)
 
     def _filter_part_columns(self, kind=None, label=None, variable=None):
         """
```

### Comparing `swmm-api-0.4.8/swmm_api/output_file/parquet_helpers.py` & `swmm-api-0.4.9/swmm_api/output_file/parquet_helpers.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/report_file/helpers.py` & `swmm-api-0.4.9/swmm_api/report_file/helpers.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/report_file/rpt.py` & `swmm-api-0.4.9/swmm_api/report_file/rpt.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/run_swmm/_run_helpers.py` & `swmm-api-0.4.9/swmm_api/run_swmm/_run_helpers.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/run_swmm/run.py` & `swmm-api-0.4.9/swmm_api/run_swmm/run.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/run_swmm/run_epaswmm.py` & `swmm-api-0.4.9/swmm_api/run_swmm/run_epaswmm.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/run_swmm/run_pyswmm.py` & `swmm-api-0.4.9/swmm_api/run_swmm/run_pyswmm.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api/run_swmm/run_swmm_toolkit.py` & `swmm-api-0.4.9/swmm_api/run_swmm/run_swmm_toolkit.py`

 * *Files identical despite different names*

### Comparing `swmm-api-0.4.8/swmm_api.egg-info/PKG-INFO` & `swmm-api-0.4.9/swmm_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swmm-api
-Version: 0.4.8
+Version: 0.4.9
 Summary: US-EPA-SWMM python interface
 Home-page: https://gitlab.com/markuspichler/swmm_api
 Author: Markus Pichler
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspichler.gitlab.io/swmm_api
 Project-URL: Changelog, https://gitlab.com/markuspichler/swmm_api/-/blob/master/CHANGELOG.md
```

### Comparing `swmm-api-0.4.8/swmm_api.egg-info/SOURCES.txt` & `swmm-api-0.4.9/swmm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

