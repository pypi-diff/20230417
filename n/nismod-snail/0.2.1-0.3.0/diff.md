# Comparing `tmp/nismod-snail-0.2.1.tar.gz` & `tmp/nismod-snail-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nismod-snail-0.2.1.tar", last modified: Thu Nov 11 16:50:52 2021, max compression
+gzip compressed data, was "nismod-snail-0.3.0.tar", last modified: Mon Apr 17 11:19:06 2023, max compression
```

## Comparing `nismod-snail-0.2.1.tar` & `nismod-snail-0.3.0.tar`

### file list

```diff
@@ -1,78 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.852962 nismod-snail-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/.environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.844962 nismod-snail-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.844962 nismod-snail-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-11-11 16:50:52.852962 nismod-snail-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.844962 nismod-snail-0.2.1/images/
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/images/snail.svg
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.844962 nismod-snail-0.2.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/scripts/failure_analysis/
--rw-r--r--   0 runner    (1001) docker     (121)     7868 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/failure_analysis/fragility_damage_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     8230 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/failure_analysis/results_process_vietnam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/scripts/hazard_processing/
--rw-r--r--   0 runner    (1001) docker     (121)    15983 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/hazard_processing/convert_hazard_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/scripts/network_creation/
--rwxr-xr-x   0 runner    (1001) docker     (121)     9057 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/network_creation/spatial_and_network_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/scripts/network_hazard_intersections/
--rw-r--r--   0 runner    (1001) docker     (121)    19444 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py
--rw-r--r--   0 runner    (1001) docker     (121)    14854 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/network_hazard_intersections/hazards_networks_intersections.py
--rw-r--r--   0 runner    (1001) docker     (121)     5534 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/network_hazard_intersections/intersection_networks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5359 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/network_hazard_intersections/intersection_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     5382 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/network_hazard_intersections/intersection_polygons.py
--rw-r--r--   0 runner    (1001) docker     (121)    24129 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/network_hazard_intersections/network_intersections.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/scripts/polygon2raster/
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/scripts/polygon2raster/polygon2raster.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-11 16:50:52.852962 nismod-snail-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2073 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.844962 nismod-snail-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (121)     3902 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/cpp/geometry.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     7137 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/cpp/grid.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4912 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/cpp/intersections.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6924 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/cpp/operations.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      523 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/cpp/operations.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/cpp/transform.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/cpp/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/src/nismod_snail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2021-11-11 16:50:52.000000 nismod-snail-0.2.1/src/nismod_snail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-11-11 16:50:52.000000 nismod-snail-0.2.1/src/nismod_snail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-11 16:50:52.000000 nismod-snail-0.2.1/src/nismod_snail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-11 16:50:52.000000 nismod-snail-0.2.1/src/nismod_snail.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-11 16:50:52.000000 nismod-snail-0.2.1/src/nismod_snail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-11 16:50:52.000000 nismod-snail-0.2.1/src/nismod_snail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-11 16:50:52.000000 nismod-snail-0.2.1/src/nismod_snail.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/src/snail/
--rw-r--r--   0 runner    (1001) docker     (121)      504 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/snail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/snail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4177 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/snail/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.848962 nismod-snail-0.2.1/src/snail/core/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/snail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/snail/multi_intersections.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/snail/routing.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/src/snail/tqdm_standin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.852962 nismod-snail-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.852962 nismod-snail-0.2.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (121)     2143 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/core/test_intersections.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.852962 nismod-snail-0.2.1/tests/cpp/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/cpp/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      206 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/cpp/run_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    14693 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/cpp/tests_intersections.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/cpp/tests_transform.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/split_polygons_rings.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     5610 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/test_multi_intersections.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tests/test_routing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-11 16:50:52.852962 nismod-snail-0.2.1/tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)    15026 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tutorials/01-data-preparation-ghana.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    21919 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tutorials/02-assess-damage-and-disruption.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    20100 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tutorials/03-test-multiple-failures.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    15678 2021-11-11 16:50:42.000000 nismod-snail-0.2.1/tutorials/04-evaluate-adaptation-options.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.305682 nismod-snail-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/.environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.289682 nismod-snail-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.293682 nismod-snail-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-17 11:19:06.305682 nismod-snail-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.293682 nismod-snail-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/_static/theme_tweaks.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/api/snail.core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/api/snail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/docs/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/examples.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/images/snail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.289682 nismod-snail-0.3.0/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/scripts/failure_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/failure_analysis/fragility_damage_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/failure_analysis/results_process_vietnam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/scripts/network_creation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9057 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/network_creation/spatial_and_network_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/scripts/network_hazard_intersections/
+-rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/network_hazard_intersections/hazards_networks_intersections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/network_hazard_intersections/intersection_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/network_hazard_intersections/intersection_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/network_hazard_intersections/intersection_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24129 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/network_hazard_intersections/network_intersections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/scripts/sources_sinks_routing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/sources_sinks_routing/benchmark_shortest_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)   337206 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/sources_sinks_routing/igraph.png
+-rw-r--r--   0 runner    (1001) docker     (123)   367721 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/sources_sinks_routing/pandana.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/sources_sinks_routing/shortest_paths_igraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/scripts/sources_sinks_routing/shortest_paths_pandana.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 11:19:06.305682 nismod-snail-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.289682 nismod-snail-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.297682 nismod-snail-0.3.0/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/cpp/geometry.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/cpp/grid.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/cpp/intersections.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/cpp/operations.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/cpp/operations.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/cpp/transform.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/cpp/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.301682 nismod-snail-0.3.0/src/nismod_snail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-17 11:19:06.000000 nismod-snail-0.3.0/src/nismod_snail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-17 11:19:06.000000 nismod-snail-0.3.0/src/nismod_snail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:19:06.000000 nismod-snail-0.3.0/src/nismod_snail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-17 11:19:06.000000 nismod-snail-0.3.0/src/nismod_snail.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 11:19:06.000000 nismod-snail-0.3.0/src/nismod_snail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 11:19:06.000000 nismod-snail-0.3.0/src/nismod_snail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 11:19:06.000000 nismod-snail-0.3.0/src/nismod_snail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.301682 nismod-snail-0.3.0/src/snail/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.301682 nismod-snail-0.3.0/src/snail/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/src/snail/tqdm_standin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.301682 nismod-snail-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.301682 nismod-snail-0.3.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/core/test_intersections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.301682 nismod-snail-0.3.0/tests/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/cpp/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/cpp/run_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/cpp/tests_intersections.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/cpp/tests_transform.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.305682 nismod-snail-0.3.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)   262568 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/climatology-hd35-annual-mean.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   270586 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/climatology-hd35-historical.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/features.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/inunriver_historical_WATCH_1980_rp01000.tif.aux.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/lines.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/points.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/polygons.geojson
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/range.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/range.tif.aux.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/rasters.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/integration/run_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/split_polygons_rings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/test_multi_intersections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tests/test_routing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 11:19:06.305682 nismod-snail-0.3.0/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    15026 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tutorials/01-data-preparation-ghana.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tutorials/02-assess-damage-and-disruption.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tutorials/03-test-multiple-failures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-04-17 11:18:58.000000 nismod-snail-0.3.0/tutorials/04-evaluate-adaptation-options.ipynb
```

### Comparing `nismod-snail-0.2.1/.github/workflows/build.yml` & `nismod-snail-0.3.0/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       matrix:
         platform: [macos-latest, ubuntu-latest]
 
     runs-on: ${{ matrix.platform }}
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Checkout submodules
         run: git submodule update --init --recursive
 
       - name: Build C++
         run: |
           cmake -Bbuild .
@@ -28,15 +28,15 @@
 
 
   build-cpp-windows:
     runs-on: windows-latest
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Checkout submodules
         run: git submodule update --init --recursive
 
       - name: Build C++
         run: |
           cmake -Bbuild .
@@ -47,24 +47,24 @@
 
 
   build:
     strategy:
       fail-fast: false
       matrix:
         platform: [macos-latest, ubuntu-latest] # skipping windows-latest
-        python-version: ["3.6", "3.9"]
+        python-version: ["3.8", "3.11"]
 
     runs-on: ${{ matrix.platform }}
 
     steps:
       - name: Checkout repository
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies and build python module
         run: |
           python -m pip install --upgrade pip wheel setuptools
           pip install --verbose .[dev]
```

### Comparing `nismod-snail-0.2.1/.github/workflows/package.yml` & `nismod-snail-0.3.0/.github/workflows/package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,62 +5,62 @@
     types: [published]
 
 jobs:
   build_sdist:
     name: Build SDist
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Build SDist
         run: pipx run build --sdist
 
       - name: Check metadata
         run: pipx run twine check dist/*
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           path: dist/*.tar.gz
 
 
   build_wheels:
     name: Wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest] # skipping windows-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
-      - uses: pypa/cibuildwheel@v2.2.0
+      - uses: pypa/cibuildwheel@v2.12.1
         env:
           CIBW_ARCHS_MACOS: auto universal2
 
       - name: Verify clean directory
         run: git diff --exit-code
         shell: bash
 
       - name: Upload wheels
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           path: wheelhouse/*.whl
 
 
   upload_all:
     name: Upload if release
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
 
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
       - name: Deploy to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
```

### Comparing `nismod-snail-0.2.1/LICENSE` & `nismod-snail-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/PKG-INFO` & `nismod-snail-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: nismod-snail
-Version: 0.2.1
+Version: 0.3.0
 Summary: The spatial networks impact assessment library
 Home-page: https://github.com/nismod/snail
 Author: Tom Russell
 Author-email: tomalrussell@gmail.com
 License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 <p align="center">
 <a href="https://github.com/nismod/snail/tree/master/tutorials">Tutorials</a> |
 <a href="https://github.com/nismod/snail/issues">Issues</a>
 </p>
 
 <p align="center">
 <img src="./images/snail.svg" alt="snail" />
 </p>
 
-
 [![Build](https://github.com/nismod/snail/actions/workflows/build.yml/badge.svg)](https://github.com/nismod/snail/actions/workflows/build.yml)
 
 > This code is under early development
 
 # 🤔 What is this?
 
 This is a Python package to help with analysis of the potential impacts of
@@ -58,14 +57,66 @@
     >>> import snail
     >>> help(snail)
     Help on package snail:
 
     NAME
         snail - snail - the spatial networks impact assessment library
 
+## Using the `snail` command
+
+Once installed, you can use `snail` directly from the command line.
+
+Split features on a grid defined by its transform, width and height:
+
+```bash
+snail split \
+    --features input.shp \
+    --transform 1 0 -180 0 -1 90 \
+    --width 360 \
+    --height 180 \
+    --output split.gpkg
+```
+
+Split features on a grid defined by a GeoTIFF, optionally adding the values from each raster band to each split feature as a new attribute:
+
+```bash
+snail split \
+    --features lines.geojson \
+    --raster gridded_data.tif \
+    --attribute \
+    --output split_lines_with_raster_values.geojson
+```
+
+Split multiple vector feature files along the grids defined by multiple raster files, attributing all raster values:
+
+```bash
+snail process -fs features.csv -rs rasters.csv
+```
+
+Where at a minimum, each CSV has a column `path` with the path to each file.
+
+### Transform
+
+A note on `transform` - these six numbers define the transform from `i,j` cell index (column/row) coordinates in the rectangular grid to `x,y` geographic coordinates, in the coordinate reference system of the input and output files. They effectively form the first two rows of a 3x3 matrix:
+
+```
+| x |   | a  b  c | | i |
+| y | = | d  e  f | | j |
+| 1 |   | 0  0  1 | | 1 |
+```
+
+In cases without shear or rotation, `a` and `e` define scaling or grid cell size, while `c` and `f` define the offset or grid upper-left corner:
+
+```
+| x_scale 0       x_offset |
+| 0       y_scale y_offset |
+| 0       0       1        |
+```
+
+See [`rasterio/affine`](https://github.com/rasterio/affine#usage) and [GDAL Raster Data Model](https://gdal.org/user/raster_data_model.html#affine-geotransform) for more documentation.
 
 ## Development
 
 Clone this repository using [GitHub Desktop](https://desktop.github.com/) or on
 the command line:
 
     git clone git@github.com:nismod/snail.git
@@ -100,15 +151,14 @@
 
 When working on the tutorial notebooks, it is recommended to install and
 configure [nbstripout](https://github.com/kynan/nbstripout) so data and outputs
 are not committed in the notebook files:
 
     nbstripout --install
 
-
 ### C++ library
 
 The C++ library in `src/cpp` contains the core routines to find intersections of
 lines with raster grids.
 
 Before working on the C++ library, fetch source code for Catch2 unit testing
 library (this is included as a git submodule):
@@ -132,22 +182,19 @@
 This may need some includes for `pybind11` - which will vary depending on your
 python installation. For example, with python via miniconda:
 
     clang-tidy --checks 'cppcoreguidelines-*' src/cpp/* -- \
         -I/home/username/miniconda3/include/python3.7m/ \
         -I./pybind11/include/
 
-
 ### Integration of C++ and Python using pybind11
 
-The `snail.core.intersections` module is built using [`pybind11` with
-`setuptools`](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools)
+The `snail.core.intersections` module is built using `pybind11` with
+`setuptools` (see [docs](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools))
 
 - `src/cpp/intersections.cpp` defines the module interface using the
   `PYBIND11_MODULE` macro
 - `pyproject.toml` defines the build requirements for snail, which includes
   pybind11, wheel and setuptools
 - `setup.py` defines the `Pybind11Extension` module to build - both the C++
   files to compile, and the location of the built module within the python
   package
-
-
```

#### html2text {}

```diff
@@ -1,55 +1,76 @@
-Metadata-Version: 2.1 Name: nismod-snail Version: 0.2.1 Summary: The spatial
+Metadata-Version: 2.1 Name: nismod-snail Version: 0.3.0 Summary: The spatial
 networks impact assessment library Home-page: https://github.com/nismod/snail
 Author: Tom Russell Author-email: tomalrussell@gmail.com License: MIT License
-Platform: UNKNOWN Classifier: Development Status :: 1 - Planning Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Utilities Requires-Python: >=3.6 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: GIS Classifier: Topic ::
+Utilities Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: docs License-File: LICENSE
                               Tutorials | Issues
                                     [snail]
 [![Build](https://github.com/nismod/snail/actions/workflows/build.yml/
 badge.svg)](https://github.com/nismod/snail/actions/workflows/build.yml) > This
 code is under early development # ð¤ What is this? This is a Python package
 to help with analysis of the potential impacts of climate hazards and other
 perils on infrastructure networks. ## Installation Install using pip: pip
 install nismod-snail This should bring all dependencies with it. If any of
 these cause difficulties, try using a [conda](https://docs.conda.io/en/latest/
 miniconda.html) environment: conda env create -n snail_env \ python=3.8
 geopandas shapely rasterio python-igraph conda activate snail_env pip install
 nismod-snail If all worked okay, you should be able to run python and import
 snail: $ python >>> import snail >>> help(snail) Help on package snail: NAME
-snail - snail - the spatial networks impact assessment library ## Development
-Clone this repository using [GitHub Desktop](https://desktop.github.com/) or on
-the command line: git clone git@github.com:nismod/snail.git Change directory
-into the root of the project: cd snail To create and activate a conda
-environment with snail's dependencies installed: conda env create -
-f .environment.yml conda activate snail-dev Run this to install the source code
-as a package: pip install . If you're working on snail itself, install it as
-"editable" along with test and development packages: pip install -e .[dev] Run
-tests using [pytest](https://docs.pytest.org/en/latest/) and [pytest-cov]
-(https://pytest-cov.readthedocs.io) to check coverage: pytest --cov=snail --
-cov-report=term-missing Run a formatter ([black](https://github.com/psf/black))
-to fix code formatting: black src/snail When working on the tutorial notebooks,
-it is recommended to install and configure [nbstripout](https://github.com/
-kynan/nbstripout) so data and outputs are not committed in the notebook files:
-nbstripout --install ### C++ library The C++ library in `src/cpp` contains the
-core routines to find intersections of lines with raster grids. Before working
-on the C++ library, fetch source code for Catch2 unit testing library (this is
-included as a git submodule): git submodule update --init --recursive Build the
-library and run tests: cmake -Bbuild . cmake --build build/ ./build/run_tests
-Run code style auto-formatting: clang-format -i src/cpp/*.hpp Run lints and
-checks: clang-tidy --checks 'cppcoreguidelines-*' src/cpp/*.hpp This may need
-some includes for `pybind11` - which will vary depending on your python
-installation. For example, with python via miniconda: clang-tidy --checks
-'cppcoreguidelines-*' src/cpp/* -- \ -I/home/username/miniconda3/include/
-python3.7m/ \ -I./pybind11/include/ ### Integration of C++ and Python using
-pybind11 The `snail.core.intersections` module is built using [`pybind11` with
-`setuptools`](https://pybind11.readthedocs.io/en/stable/
-compiling.html#building-with-setuptools) - `src/cpp/intersections.cpp` defines
-the module interface using the `PYBIND11_MODULE` macro - `pyproject.toml`
-defines the build requirements for snail, which includes pybind11, wheel and
-setuptools - `setup.py` defines the `Pybind11Extension` module to build - both
-the C++ files to compile, and the location of the built module within the
-python package
+snail - snail - the spatial networks impact assessment library ## Using the
+`snail` command Once installed, you can use `snail` directly from the command
+line. Split features on a grid defined by its transform, width and height:
+```bash snail split \ --features input.shp \ --transform 1 0 -180 0 -1 90 \ --
+width 360 \ --height 180 \ --output split.gpkg ``` Split features on a grid
+defined by a GeoTIFF, optionally adding the values from each raster band to
+each split feature as a new attribute: ```bash snail split \ --features
+lines.geojson \ --raster gridded_data.tif \ --attribute \ --output
+split_lines_with_raster_values.geojson ``` Split multiple vector feature files
+along the grids defined by multiple raster files, attributing all raster
+values: ```bash snail process -fs features.csv -rs rasters.csv ``` Where at a
+minimum, each CSV has a column `path` with the path to each file. ### Transform
+A note on `transform` - these six numbers define the transform from `i,j` cell
+index (column/row) coordinates in the rectangular grid to `x,y` geographic
+coordinates, in the coordinate reference system of the input and output files.
+They effectively form the first two rows of a 3x3 matrix: ``` | x | | a b c | |
+i | | y | = | d e f | | j | | 1 | | 0 0 1 | | 1 | ``` In cases without shear or
+rotation, `a` and `e` define scaling or grid cell size, while `c` and `f`
+define the offset or grid upper-left corner: ``` | x_scale 0 x_offset | | 0
+y_scale y_offset | | 0 0 1 | ``` See [`rasterio/affine`](https://github.com/
+rasterio/affine#usage) and [GDAL Raster Data Model](https://gdal.org/user/
+raster_data_model.html#affine-geotransform) for more documentation. ##
+Development Clone this repository using [GitHub Desktop](https://
+desktop.github.com/) or on the command line: git clone git@github.com:nismod/
+snail.git Change directory into the root of the project: cd snail To create and
+activate a conda environment with snail's dependencies installed: conda env
+create -f .environment.yml conda activate snail-dev Run this to install the
+source code as a package: pip install . If you're working on snail itself,
+install it as "editable" along with test and development packages: pip install
+-e .[dev] Run tests using [pytest](https://docs.pytest.org/en/latest/) and
+[pytest-cov](https://pytest-cov.readthedocs.io) to check coverage: pytest --
+cov=snail --cov-report=term-missing Run a formatter ([black](https://
+github.com/psf/black)) to fix code formatting: black src/snail When working on
+the tutorial notebooks, it is recommended to install and configure [nbstripout]
+(https://github.com/kynan/nbstripout) so data and outputs are not committed in
+the notebook files: nbstripout --install ### C++ library The C++ library in
+`src/cpp` contains the core routines to find intersections of lines with raster
+grids. Before working on the C++ library, fetch source code for Catch2 unit
+testing library (this is included as a git submodule): git submodule update --
+init --recursive Build the library and run tests: cmake -Bbuild . cmake --build
+build/ ./build/run_tests Run code style auto-formatting: clang-format -i src/
+cpp/*.hpp Run lints and checks: clang-tidy --checks 'cppcoreguidelines-*' src/
+cpp/*.hpp This may need some includes for `pybind11` - which will vary
+depending on your python installation. For example, with python via miniconda:
+clang-tidy --checks 'cppcoreguidelines-*' src/cpp/* -- \ -I/home/username/
+miniconda3/include/python3.7m/ \ -I./pybind11/include/ ### Integration of C++
+and Python using pybind11 The `snail.core.intersections` module is built using
+`pybind11` with `setuptools` (see [docs](https://pybind11.readthedocs.io/en/
+stable/compiling.html#building-with-setuptools)) - `src/cpp/intersections.cpp`
+defines the module interface using the `PYBIND11_MODULE` macro -
+`pyproject.toml` defines the build requirements for snail, which includes
+pybind11, wheel and setuptools - `setup.py` defines the `Pybind11Extension`
+module to build - both the C++ files to compile, and the location of the built
+module within the python package
```

### Comparing `nismod-snail-0.2.1/README.md` & `nismod-snail-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 <a href="https://github.com/nismod/snail/issues">Issues</a>
 </p>
 
 <p align="center">
 <img src="./images/snail.svg" alt="snail" />
 </p>
 
-
 [![Build](https://github.com/nismod/snail/actions/workflows/build.yml/badge.svg)](https://github.com/nismod/snail/actions/workflows/build.yml)
 
 > This code is under early development
 
 # 🤔 What is this?
 
 This is a Python package to help with analysis of the potential impacts of
@@ -37,14 +36,66 @@
     >>> import snail
     >>> help(snail)
     Help on package snail:
 
     NAME
         snail - snail - the spatial networks impact assessment library
 
+## Using the `snail` command
+
+Once installed, you can use `snail` directly from the command line.
+
+Split features on a grid defined by its transform, width and height:
+
+```bash
+snail split \
+    --features input.shp \
+    --transform 1 0 -180 0 -1 90 \
+    --width 360 \
+    --height 180 \
+    --output split.gpkg
+```
+
+Split features on a grid defined by a GeoTIFF, optionally adding the values from each raster band to each split feature as a new attribute:
+
+```bash
+snail split \
+    --features lines.geojson \
+    --raster gridded_data.tif \
+    --attribute \
+    --output split_lines_with_raster_values.geojson
+```
+
+Split multiple vector feature files along the grids defined by multiple raster files, attributing all raster values:
+
+```bash
+snail process -fs features.csv -rs rasters.csv
+```
+
+Where at a minimum, each CSV has a column `path` with the path to each file.
+
+### Transform
+
+A note on `transform` - these six numbers define the transform from `i,j` cell index (column/row) coordinates in the rectangular grid to `x,y` geographic coordinates, in the coordinate reference system of the input and output files. They effectively form the first two rows of a 3x3 matrix:
+
+```
+| x |   | a  b  c | | i |
+| y | = | d  e  f | | j |
+| 1 |   | 0  0  1 | | 1 |
+```
+
+In cases without shear or rotation, `a` and `e` define scaling or grid cell size, while `c` and `f` define the offset or grid upper-left corner:
+
+```
+| x_scale 0       x_offset |
+| 0       y_scale y_offset |
+| 0       0       1        |
+```
+
+See [`rasterio/affine`](https://github.com/rasterio/affine#usage) and [GDAL Raster Data Model](https://gdal.org/user/raster_data_model.html#affine-geotransform) for more documentation.
 
 ## Development
 
 Clone this repository using [GitHub Desktop](https://desktop.github.com/) or on
 the command line:
 
     git clone git@github.com:nismod/snail.git
@@ -79,15 +130,14 @@
 
 When working on the tutorial notebooks, it is recommended to install and
 configure [nbstripout](https://github.com/kynan/nbstripout) so data and outputs
 are not committed in the notebook files:
 
     nbstripout --install
 
-
 ### C++ library
 
 The C++ library in `src/cpp` contains the core routines to find intersections of
 lines with raster grids.
 
 Before working on the C++ library, fetch source code for Catch2 unit testing
 library (this is included as a git submodule):
@@ -111,19 +161,18 @@
 This may need some includes for `pybind11` - which will vary depending on your
 python installation. For example, with python via miniconda:
 
     clang-tidy --checks 'cppcoreguidelines-*' src/cpp/* -- \
         -I/home/username/miniconda3/include/python3.7m/ \
         -I./pybind11/include/
 
-
 ### Integration of C++ and Python using pybind11
 
-The `snail.core.intersections` module is built using [`pybind11` with
-`setuptools`](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools)
+The `snail.core.intersections` module is built using `pybind11` with
+`setuptools` (see [docs](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools))
 
 - `src/cpp/intersections.cpp` defines the module interface using the
   `PYBIND11_MODULE` macro
 - `pyproject.toml` defines the build requirements for snail, which includes
   pybind11, wheel and setuptools
 - `setup.py` defines the `Pybind11Extension` module to build - both the C++
   files to compile, and the location of the built module within the python
```

#### html2text {}

```diff
@@ -7,40 +7,61 @@
 perils on infrastructure networks. ## Installation Install using pip: pip
 install nismod-snail This should bring all dependencies with it. If any of
 these cause difficulties, try using a [conda](https://docs.conda.io/en/latest/
 miniconda.html) environment: conda env create -n snail_env \ python=3.8
 geopandas shapely rasterio python-igraph conda activate snail_env pip install
 nismod-snail If all worked okay, you should be able to run python and import
 snail: $ python >>> import snail >>> help(snail) Help on package snail: NAME
-snail - snail - the spatial networks impact assessment library ## Development
-Clone this repository using [GitHub Desktop](https://desktop.github.com/) or on
-the command line: git clone git@github.com:nismod/snail.git Change directory
-into the root of the project: cd snail To create and activate a conda
-environment with snail's dependencies installed: conda env create -
-f .environment.yml conda activate snail-dev Run this to install the source code
-as a package: pip install . If you're working on snail itself, install it as
-"editable" along with test and development packages: pip install -e .[dev] Run
-tests using [pytest](https://docs.pytest.org/en/latest/) and [pytest-cov]
-(https://pytest-cov.readthedocs.io) to check coverage: pytest --cov=snail --
-cov-report=term-missing Run a formatter ([black](https://github.com/psf/black))
-to fix code formatting: black src/snail When working on the tutorial notebooks,
-it is recommended to install and configure [nbstripout](https://github.com/
-kynan/nbstripout) so data and outputs are not committed in the notebook files:
-nbstripout --install ### C++ library The C++ library in `src/cpp` contains the
-core routines to find intersections of lines with raster grids. Before working
-on the C++ library, fetch source code for Catch2 unit testing library (this is
-included as a git submodule): git submodule update --init --recursive Build the
-library and run tests: cmake -Bbuild . cmake --build build/ ./build/run_tests
-Run code style auto-formatting: clang-format -i src/cpp/*.hpp Run lints and
-checks: clang-tidy --checks 'cppcoreguidelines-*' src/cpp/*.hpp This may need
-some includes for `pybind11` - which will vary depending on your python
-installation. For example, with python via miniconda: clang-tidy --checks
-'cppcoreguidelines-*' src/cpp/* -- \ -I/home/username/miniconda3/include/
-python3.7m/ \ -I./pybind11/include/ ### Integration of C++ and Python using
-pybind11 The `snail.core.intersections` module is built using [`pybind11` with
-`setuptools`](https://pybind11.readthedocs.io/en/stable/
-compiling.html#building-with-setuptools) - `src/cpp/intersections.cpp` defines
-the module interface using the `PYBIND11_MODULE` macro - `pyproject.toml`
-defines the build requirements for snail, which includes pybind11, wheel and
-setuptools - `setup.py` defines the `Pybind11Extension` module to build - both
-the C++ files to compile, and the location of the built module within the
-python package
+snail - snail - the spatial networks impact assessment library ## Using the
+`snail` command Once installed, you can use `snail` directly from the command
+line. Split features on a grid defined by its transform, width and height:
+```bash snail split \ --features input.shp \ --transform 1 0 -180 0 -1 90 \ --
+width 360 \ --height 180 \ --output split.gpkg ``` Split features on a grid
+defined by a GeoTIFF, optionally adding the values from each raster band to
+each split feature as a new attribute: ```bash snail split \ --features
+lines.geojson \ --raster gridded_data.tif \ --attribute \ --output
+split_lines_with_raster_values.geojson ``` Split multiple vector feature files
+along the grids defined by multiple raster files, attributing all raster
+values: ```bash snail process -fs features.csv -rs rasters.csv ``` Where at a
+minimum, each CSV has a column `path` with the path to each file. ### Transform
+A note on `transform` - these six numbers define the transform from `i,j` cell
+index (column/row) coordinates in the rectangular grid to `x,y` geographic
+coordinates, in the coordinate reference system of the input and output files.
+They effectively form the first two rows of a 3x3 matrix: ``` | x | | a b c | |
+i | | y | = | d e f | | j | | 1 | | 0 0 1 | | 1 | ``` In cases without shear or
+rotation, `a` and `e` define scaling or grid cell size, while `c` and `f`
+define the offset or grid upper-left corner: ``` | x_scale 0 x_offset | | 0
+y_scale y_offset | | 0 0 1 | ``` See [`rasterio/affine`](https://github.com/
+rasterio/affine#usage) and [GDAL Raster Data Model](https://gdal.org/user/
+raster_data_model.html#affine-geotransform) for more documentation. ##
+Development Clone this repository using [GitHub Desktop](https://
+desktop.github.com/) or on the command line: git clone git@github.com:nismod/
+snail.git Change directory into the root of the project: cd snail To create and
+activate a conda environment with snail's dependencies installed: conda env
+create -f .environment.yml conda activate snail-dev Run this to install the
+source code as a package: pip install . If you're working on snail itself,
+install it as "editable" along with test and development packages: pip install
+-e .[dev] Run tests using [pytest](https://docs.pytest.org/en/latest/) and
+[pytest-cov](https://pytest-cov.readthedocs.io) to check coverage: pytest --
+cov=snail --cov-report=term-missing Run a formatter ([black](https://
+github.com/psf/black)) to fix code formatting: black src/snail When working on
+the tutorial notebooks, it is recommended to install and configure [nbstripout]
+(https://github.com/kynan/nbstripout) so data and outputs are not committed in
+the notebook files: nbstripout --install ### C++ library The C++ library in
+`src/cpp` contains the core routines to find intersections of lines with raster
+grids. Before working on the C++ library, fetch source code for Catch2 unit
+testing library (this is included as a git submodule): git submodule update --
+init --recursive Build the library and run tests: cmake -Bbuild . cmake --build
+build/ ./build/run_tests Run code style auto-formatting: clang-format -i src/
+cpp/*.hpp Run lints and checks: clang-tidy --checks 'cppcoreguidelines-*' src/
+cpp/*.hpp This may need some includes for `pybind11` - which will vary
+depending on your python installation. For example, with python via miniconda:
+clang-tidy --checks 'cppcoreguidelines-*' src/cpp/* -- \ -I/home/username/
+miniconda3/include/python3.7m/ \ -I./pybind11/include/ ### Integration of C++
+and Python using pybind11 The `snail.core.intersections` module is built using
+`pybind11` with `setuptools` (see [docs](https://pybind11.readthedocs.io/en/
+stable/compiling.html#building-with-setuptools)) - `src/cpp/intersections.cpp`
+defines the module interface using the `PYBIND11_MODULE` macro -
+`pyproject.toml` defines the build requirements for snail, which includes
+pybind11, wheel and setuptools - `setup.py` defines the `Pybind11Extension`
+module to build - both the C++ files to compile, and the location of the built
+module within the python package
```

### Comparing `nismod-snail-0.2.1/images/snail.svg` & `nismod-snail-0.3.0/images/snail.svg`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/failure_analysis/fragility_damage_analysis.py` & `nismod-snail-0.3.0/scripts/failure_analysis/fragility_damage_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-"""Estimating the fragility and damages to roads 
+"""Estimating the fragility and damages to roads
 """
-
-import os
-import sys
 import pandas as pd
-import geopandas as gpd
 import numpy as np
-import convert_hazard_data as chd
-import network_intersections as ni
 from scipy import integrate
 from tqdm import tqdm
 
 tqdm.pandas()
 
 
 def damage_function_roads_v1(flood_depth, multiplication_factor):
```

### Comparing `nismod-snail-0.2.1/scripts/failure_analysis/results_process_vietnam.py` & `nismod-snail-0.3.0/scripts/failure_analysis/results_process_vietnam.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/network_creation/spatial_and_network_functions.py` & `nismod-snail-0.3.0/scripts/network_creation/spatial_and_network_functions.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py` & `nismod-snail-0.3.0/scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/network_hazard_intersections/hazards_networks_intersections.py` & `nismod-snail-0.3.0/scripts/network_hazard_intersections/hazards_networks_intersections.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/network_hazard_intersections/intersection_networks.py` & `nismod-snail-0.3.0/scripts/network_hazard_intersections/intersection_networks.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/network_hazard_intersections/intersection_points.py` & `nismod-snail-0.3.0/scripts/network_hazard_intersections/intersection_points.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/network_hazard_intersections/intersection_polygons.py` & `nismod-snail-0.3.0/scripts/network_hazard_intersections/intersection_polygons.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/scripts/network_hazard_intersections/network_intersections.py` & `nismod-snail-0.3.0/scripts/network_hazard_intersections/network_intersections.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/setup.py` & `nismod-snail-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,59 +15,69 @@
         "snail.core.intersections",
         sorted(glob("src/cpp/*.cpp")),
     ),
 ]
 
 
 def readme():
-    """Read README contents
-    """
-    with open('README.md', encoding='utf8') as f:
+    """Read README contents"""
+    with open("README.md", encoding="utf8") as f:
         return f.read()
 
 
 setup(
-    name='nismod-snail',
+    name="nismod-snail",
     use_scm_version=True,
-    license='MIT License',
-    description='The spatial networks impact assessment library',
+    license="MIT License",
+    description="The spatial networks impact assessment library",
     long_description=readme(),
     long_description_content_type="text/markdown",
-    author='Tom Russell',
-    author_email='tomalrussell@gmail.com',
-    url='https://github.com/nismod/snail',
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},
+    author="Tom Russell",
+    author_email="tomalrussell@gmail.com",
+    url="https://github.com/nismod/snail",
+    packages=find_packages(where="src"),
+    package_dir={"": "src"},
     ext_modules=ext_modules,
     cmdclass={"build_ext": build_ext},
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'Development Status :: 1 - Planning',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Topic :: Scientific/Engineering :: GIS',
-        'Topic :: Utilities',
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering :: GIS",
+        "Topic :: Utilities",
     ],
     keywords=[
         # eg: 'keyword1', 'keyword2', 'keyword3',
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     install_requires=[
-        'geopandas', 'shapely', 'rasterio', 'python-igraph'
+        "geopandas",
+        "pyarrow",
+        "python-igraph",
+        "rasterio",
+        "shapely",
     ],
     extras_require={
-        'dev': ['affine', 'black', 'nbstripout', 'numpy', 'pytest', 'pytest-cov'],
+        "dev": [
+            "affine",
+            "black",
+            "nbstripout",
+            "numpy",
+            "pytest-cov",
+            "pytest",
+        ],
+        "docs": ["sphinx", "m2r2"]
         # eg:
         #   'rst': ['docutils>=0.11'],
         #   ':python_version=="2.6"': ['argparse'],
     },
     entry_points={
-        'console_scripts': [
-            'snail_split = snail.cli:snail_split',
-            'snail_raster2split = snail.cli:snail_raster2split',
+        "console_scripts": [
+            "snail = snail.cli:snail",
         ]
     },
 )
```

### Comparing `nismod-snail-0.2.1/src/cpp/geometry.hpp` & `nismod-snail-0.3.0/src/cpp/geometry.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/src/cpp/grid.hpp` & `nismod-snail-0.3.0/src/cpp/grid.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/src/cpp/intersections.cpp` & `nismod-snail-0.3.0/src/cpp/intersections.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/src/cpp/operations.cpp` & `nismod-snail-0.3.0/src/cpp/operations.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/src/cpp/operations.hpp` & `nismod-snail-0.3.0/src/cpp/operations.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/src/cpp/transform.hpp` & `nismod-snail-0.3.0/src/cpp/transform.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/src/cpp/utils.hpp` & `nismod-snail-0.3.0/src/cpp/utils.hpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/src/nismod_snail.egg-info/PKG-INFO` & `nismod-snail-0.3.0/src/nismod_snail.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: nismod-snail
-Version: 0.2.1
+Version: 0.3.0
 Summary: The spatial networks impact assessment library
 Home-page: https://github.com/nismod/snail
 Author: Tom Russell
 Author-email: tomalrussell@gmail.com
 License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 <p align="center">
 <a href="https://github.com/nismod/snail/tree/master/tutorials">Tutorials</a> |
 <a href="https://github.com/nismod/snail/issues">Issues</a>
 </p>
 
 <p align="center">
 <img src="./images/snail.svg" alt="snail" />
 </p>
 
-
 [![Build](https://github.com/nismod/snail/actions/workflows/build.yml/badge.svg)](https://github.com/nismod/snail/actions/workflows/build.yml)
 
 > This code is under early development
 
 # 🤔 What is this?
 
 This is a Python package to help with analysis of the potential impacts of
@@ -58,14 +57,66 @@
     >>> import snail
     >>> help(snail)
     Help on package snail:
 
     NAME
         snail - snail - the spatial networks impact assessment library
 
+## Using the `snail` command
+
+Once installed, you can use `snail` directly from the command line.
+
+Split features on a grid defined by its transform, width and height:
+
+```bash
+snail split \
+    --features input.shp \
+    --transform 1 0 -180 0 -1 90 \
+    --width 360 \
+    --height 180 \
+    --output split.gpkg
+```
+
+Split features on a grid defined by a GeoTIFF, optionally adding the values from each raster band to each split feature as a new attribute:
+
+```bash
+snail split \
+    --features lines.geojson \
+    --raster gridded_data.tif \
+    --attribute \
+    --output split_lines_with_raster_values.geojson
+```
+
+Split multiple vector feature files along the grids defined by multiple raster files, attributing all raster values:
+
+```bash
+snail process -fs features.csv -rs rasters.csv
+```
+
+Where at a minimum, each CSV has a column `path` with the path to each file.
+
+### Transform
+
+A note on `transform` - these six numbers define the transform from `i,j` cell index (column/row) coordinates in the rectangular grid to `x,y` geographic coordinates, in the coordinate reference system of the input and output files. They effectively form the first two rows of a 3x3 matrix:
+
+```
+| x |   | a  b  c | | i |
+| y | = | d  e  f | | j |
+| 1 |   | 0  0  1 | | 1 |
+```
+
+In cases without shear or rotation, `a` and `e` define scaling or grid cell size, while `c` and `f` define the offset or grid upper-left corner:
+
+```
+| x_scale 0       x_offset |
+| 0       y_scale y_offset |
+| 0       0       1        |
+```
+
+See [`rasterio/affine`](https://github.com/rasterio/affine#usage) and [GDAL Raster Data Model](https://gdal.org/user/raster_data_model.html#affine-geotransform) for more documentation.
 
 ## Development
 
 Clone this repository using [GitHub Desktop](https://desktop.github.com/) or on
 the command line:
 
     git clone git@github.com:nismod/snail.git
@@ -100,15 +151,14 @@
 
 When working on the tutorial notebooks, it is recommended to install and
 configure [nbstripout](https://github.com/kynan/nbstripout) so data and outputs
 are not committed in the notebook files:
 
     nbstripout --install
 
-
 ### C++ library
 
 The C++ library in `src/cpp` contains the core routines to find intersections of
 lines with raster grids.
 
 Before working on the C++ library, fetch source code for Catch2 unit testing
 library (this is included as a git submodule):
@@ -132,22 +182,19 @@
 This may need some includes for `pybind11` - which will vary depending on your
 python installation. For example, with python via miniconda:
 
     clang-tidy --checks 'cppcoreguidelines-*' src/cpp/* -- \
         -I/home/username/miniconda3/include/python3.7m/ \
         -I./pybind11/include/
 
-
 ### Integration of C++ and Python using pybind11
 
-The `snail.core.intersections` module is built using [`pybind11` with
-`setuptools`](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools)
+The `snail.core.intersections` module is built using `pybind11` with
+`setuptools` (see [docs](https://pybind11.readthedocs.io/en/stable/compiling.html#building-with-setuptools))
 
 - `src/cpp/intersections.cpp` defines the module interface using the
   `PYBIND11_MODULE` macro
 - `pyproject.toml` defines the build requirements for snail, which includes
   pybind11, wheel and setuptools
 - `setup.py` defines the `Pybind11Extension` module to build - both the C++
   files to compile, and the location of the built module within the python
   package
-
-
```

#### html2text {}

```diff
@@ -1,55 +1,76 @@
-Metadata-Version: 2.1 Name: nismod-snail Version: 0.2.1 Summary: The spatial
+Metadata-Version: 2.1 Name: nismod-snail Version: 0.3.0 Summary: The spatial
 networks impact assessment library Home-page: https://github.com/nismod/snail
 Author: Tom Russell Author-email: tomalrussell@gmail.com License: MIT License
-Platform: UNKNOWN Classifier: Development Status :: 1 - Planning Classifier:
-Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Utilities Requires-Python: >=3.6 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE
+Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: GIS Classifier: Topic ::
+Utilities Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: docs License-File: LICENSE
                               Tutorials | Issues
                                     [snail]
 [![Build](https://github.com/nismod/snail/actions/workflows/build.yml/
 badge.svg)](https://github.com/nismod/snail/actions/workflows/build.yml) > This
 code is under early development # ð¤ What is this? This is a Python package
 to help with analysis of the potential impacts of climate hazards and other
 perils on infrastructure networks. ## Installation Install using pip: pip
 install nismod-snail This should bring all dependencies with it. If any of
 these cause difficulties, try using a [conda](https://docs.conda.io/en/latest/
 miniconda.html) environment: conda env create -n snail_env \ python=3.8
 geopandas shapely rasterio python-igraph conda activate snail_env pip install
 nismod-snail If all worked okay, you should be able to run python and import
 snail: $ python >>> import snail >>> help(snail) Help on package snail: NAME
-snail - snail - the spatial networks impact assessment library ## Development
-Clone this repository using [GitHub Desktop](https://desktop.github.com/) or on
-the command line: git clone git@github.com:nismod/snail.git Change directory
-into the root of the project: cd snail To create and activate a conda
-environment with snail's dependencies installed: conda env create -
-f .environment.yml conda activate snail-dev Run this to install the source code
-as a package: pip install . If you're working on snail itself, install it as
-"editable" along with test and development packages: pip install -e .[dev] Run
-tests using [pytest](https://docs.pytest.org/en/latest/) and [pytest-cov]
-(https://pytest-cov.readthedocs.io) to check coverage: pytest --cov=snail --
-cov-report=term-missing Run a formatter ([black](https://github.com/psf/black))
-to fix code formatting: black src/snail When working on the tutorial notebooks,
-it is recommended to install and configure [nbstripout](https://github.com/
-kynan/nbstripout) so data and outputs are not committed in the notebook files:
-nbstripout --install ### C++ library The C++ library in `src/cpp` contains the
-core routines to find intersections of lines with raster grids. Before working
-on the C++ library, fetch source code for Catch2 unit testing library (this is
-included as a git submodule): git submodule update --init --recursive Build the
-library and run tests: cmake -Bbuild . cmake --build build/ ./build/run_tests
-Run code style auto-formatting: clang-format -i src/cpp/*.hpp Run lints and
-checks: clang-tidy --checks 'cppcoreguidelines-*' src/cpp/*.hpp This may need
-some includes for `pybind11` - which will vary depending on your python
-installation. For example, with python via miniconda: clang-tidy --checks
-'cppcoreguidelines-*' src/cpp/* -- \ -I/home/username/miniconda3/include/
-python3.7m/ \ -I./pybind11/include/ ### Integration of C++ and Python using
-pybind11 The `snail.core.intersections` module is built using [`pybind11` with
-`setuptools`](https://pybind11.readthedocs.io/en/stable/
-compiling.html#building-with-setuptools) - `src/cpp/intersections.cpp` defines
-the module interface using the `PYBIND11_MODULE` macro - `pyproject.toml`
-defines the build requirements for snail, which includes pybind11, wheel and
-setuptools - `setup.py` defines the `Pybind11Extension` module to build - both
-the C++ files to compile, and the location of the built module within the
-python package
+snail - snail - the spatial networks impact assessment library ## Using the
+`snail` command Once installed, you can use `snail` directly from the command
+line. Split features on a grid defined by its transform, width and height:
+```bash snail split \ --features input.shp \ --transform 1 0 -180 0 -1 90 \ --
+width 360 \ --height 180 \ --output split.gpkg ``` Split features on a grid
+defined by a GeoTIFF, optionally adding the values from each raster band to
+each split feature as a new attribute: ```bash snail split \ --features
+lines.geojson \ --raster gridded_data.tif \ --attribute \ --output
+split_lines_with_raster_values.geojson ``` Split multiple vector feature files
+along the grids defined by multiple raster files, attributing all raster
+values: ```bash snail process -fs features.csv -rs rasters.csv ``` Where at a
+minimum, each CSV has a column `path` with the path to each file. ### Transform
+A note on `transform` - these six numbers define the transform from `i,j` cell
+index (column/row) coordinates in the rectangular grid to `x,y` geographic
+coordinates, in the coordinate reference system of the input and output files.
+They effectively form the first two rows of a 3x3 matrix: ``` | x | | a b c | |
+i | | y | = | d e f | | j | | 1 | | 0 0 1 | | 1 | ``` In cases without shear or
+rotation, `a` and `e` define scaling or grid cell size, while `c` and `f`
+define the offset or grid upper-left corner: ``` | x_scale 0 x_offset | | 0
+y_scale y_offset | | 0 0 1 | ``` See [`rasterio/affine`](https://github.com/
+rasterio/affine#usage) and [GDAL Raster Data Model](https://gdal.org/user/
+raster_data_model.html#affine-geotransform) for more documentation. ##
+Development Clone this repository using [GitHub Desktop](https://
+desktop.github.com/) or on the command line: git clone git@github.com:nismod/
+snail.git Change directory into the root of the project: cd snail To create and
+activate a conda environment with snail's dependencies installed: conda env
+create -f .environment.yml conda activate snail-dev Run this to install the
+source code as a package: pip install . If you're working on snail itself,
+install it as "editable" along with test and development packages: pip install
+-e .[dev] Run tests using [pytest](https://docs.pytest.org/en/latest/) and
+[pytest-cov](https://pytest-cov.readthedocs.io) to check coverage: pytest --
+cov=snail --cov-report=term-missing Run a formatter ([black](https://
+github.com/psf/black)) to fix code formatting: black src/snail When working on
+the tutorial notebooks, it is recommended to install and configure [nbstripout]
+(https://github.com/kynan/nbstripout) so data and outputs are not committed in
+the notebook files: nbstripout --install ### C++ library The C++ library in
+`src/cpp` contains the core routines to find intersections of lines with raster
+grids. Before working on the C++ library, fetch source code for Catch2 unit
+testing library (this is included as a git submodule): git submodule update --
+init --recursive Build the library and run tests: cmake -Bbuild . cmake --build
+build/ ./build/run_tests Run code style auto-formatting: clang-format -i src/
+cpp/*.hpp Run lints and checks: clang-tidy --checks 'cppcoreguidelines-*' src/
+cpp/*.hpp This may need some includes for `pybind11` - which will vary
+depending on your python installation. For example, with python via miniconda:
+clang-tidy --checks 'cppcoreguidelines-*' src/cpp/* -- \ -I/home/username/
+miniconda3/include/python3.7m/ \ -I./pybind11/include/ ### Integration of C++
+and Python using pybind11 The `snail.core.intersections` module is built using
+`pybind11` with `setuptools` (see [docs](https://pybind11.readthedocs.io/en/
+stable/compiling.html#building-with-setuptools)) - `src/cpp/intersections.cpp`
+defines the module interface using the `PYBIND11_MODULE` macro -
+`pyproject.toml` defines the build requirements for snail, which includes
+pybind11, wheel and setuptools - `setup.py` defines the `Pybind11Extension`
+module to build - both the C++ files to compile, and the location of the built
+module within the python package
```

### Comparing `nismod-snail-0.2.1/src/nismod_snail.egg-info/SOURCES.txt` & `nismod-snail-0.3.0/src/nismod_snail.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 .clang-format
 .environment.yml
 .gitignore
 .gitmodules
 CMakeLists.txt
 LICENSE
 README.md
+examples.sh
 pyproject.toml
 setup.py
 .github/workflows/build.yml
+.github/workflows/docs.yml
 .github/workflows/package.yml
+docs/Makefile
+docs/source/conf.py
+docs/source/getting_started.md
+docs/source/index.rst
+docs/source/license.rst
+docs/source/_static/theme_tweaks.css
+docs/source/api/modules.rst
+docs/source/api/snail.core.rst
+docs/source/api/snail.rst
 images/snail.svg
 scripts/failure_analysis/fragility_damage_analysis.py
 scripts/failure_analysis/results_process_vietnam.py
-scripts/hazard_processing/convert_hazard_data.py
 scripts/network_creation/spatial_and_network_functions.py
 scripts/network_hazard_intersections/hazards_network_intersections_results_collect.py
 scripts/network_hazard_intersections/hazards_networks_intersections.py
 scripts/network_hazard_intersections/intersection_networks.py
 scripts/network_hazard_intersections/intersection_points.py
 scripts/network_hazard_intersections/intersection_polygons.py
 scripts/network_hazard_intersections/network_intersections.py
-scripts/polygon2raster/polygon2raster.py
+scripts/sources_sinks_routing/benchmark_shortest_path.py
+scripts/sources_sinks_routing/igraph.png
+scripts/sources_sinks_routing/pandana.png
+scripts/sources_sinks_routing/shortest_paths_igraph.py
+scripts/sources_sinks_routing/shortest_paths_pandana.py
 src/cpp/geometry.hpp
 src/cpp/grid.hpp
 src/cpp/intersections.cpp
 src/cpp/operations.cpp
 src/cpp/operations.hpp
 src/cpp/transform.hpp
 src/cpp/utils.hpp
@@ -34,24 +48,37 @@
 src/nismod_snail.egg-info/entry_points.txt
 src/nismod_snail.egg-info/not-zip-safe
 src/nismod_snail.egg-info/requires.txt
 src/nismod_snail.egg-info/top_level.txt
 src/snail/__init__.py
 src/snail/__main__.py
 src/snail/cli.py
-src/snail/multi_intersections.py
+src/snail/intersection.py
+src/snail/io.py
 src/snail/routing.py
 src/snail/tqdm_standin.py
 src/snail/core/__init__.py
 tests/split_polygons_rings.py
 tests/test_init.py
 tests/test_multi_intersections.py
 tests/test_routing.py
 tests/core/test_intersections.py
 tests/cpp/README.md
 tests/cpp/run_tests.cpp
 tests/cpp/tests_intersections.cpp
 tests/cpp/tests_transform.cpp
+tests/integration/climatology-hd35-annual-mean.tif
+tests/integration/climatology-hd35-historical.tif
+tests/integration/features.csv
+tests/integration/inunriver_historical_WATCH_1980_rp01000.tif
+tests/integration/inunriver_historical_WATCH_1980_rp01000.tif.aux.xml
+tests/integration/lines.geojson
+tests/integration/points.geojson
+tests/integration/polygons.geojson
+tests/integration/range.tif
+tests/integration/range.tif.aux.xml
+tests/integration/rasters.csv
+tests/integration/run_examples.sh
 tutorials/01-data-preparation-ghana.ipynb
 tutorials/02-assess-damage-and-disruption.ipynb
 tutorials/03-test-multiple-failures.ipynb
 tutorials/04-evaluate-adaptation-options.ipynb
```

### Comparing `nismod-snail-0.2.1/src/snail/routing.py` & `nismod-snail-0.3.0/src/snail/routing.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/tests/core/test_intersections.py` & `nismod-snail-0.3.0/tests/core/test_intersections.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             test_linestring, expected_splits = test_data
             with self.subTest(i=i):
                 splits = snail.core.intersections.split_linestring(
                     test_linestring, self.nrows, self.ncols, self.transform
                 )
                 self.assertTrue(
                     [
-                        split.almost_equals(expected_split)
+                        split.equals_exact(expected_split, 0.5e-6)
                         for split, expected_split in zip(
                             splits, expected_splits
                         )
                     ]
                 )
 
     def test_get_cell_indices(self):
```

### Comparing `nismod-snail-0.2.1/tests/cpp/tests_intersections.cpp` & `nismod-snail-0.3.0/tests/cpp/tests_intersections.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -155,16 +155,50 @@
   };
   case8.expected_splits = {
     {{0.5,1.1}, {1.,1.}},
     {{1.,1.}, {1.5,0.9}, {2.,1.}},
     {{2.,1.}, {2.5,1.1}}
   };
 
+  // Linestring points are marked by o:
+  // Intersection points are marked by (o):
+  // +---------------+--------------+
+  // |               |              |
+  // |               |              |
+  // |               |              |
+  // |               |              |
+  // |               |              |
+  // |               |              |
+  // |               |              |
+  // +---------------+--------------+
+  // |               |              |
+  // |               |              |
+  // |               |              |
+  // |      (o)      |              |
+  // |     /         |              |
+  // |  ---          |              |
+  // | /             |              |
+  //(o)--------------+--------------+
+  // (0,0)         (1,0)          (2,0)
+  Config case9;
+  case9.linestring = {{0, 0}, {0.5, 0.5}};
+  case9.expected_splits = {{{0, 0}, {0.5, 0.5}}};
+
   // TODO case7, case8
-  auto test_data = GENERATE_COPY(case1, case2, case3, case4, case5, case6);
+  auto test_data = GENERATE_COPY(
+    case1,
+    case2,
+    case3,
+    case4,
+    case5,
+    case6,
+    // case7,
+    // case8,
+    case9
+  );
 
 
   std::vector<linestr> expected_splits = test_data.expected_splits;
 
   linestr geom = test_data.linestring;
   snail::geometry::LineString line(geom);
```

### Comparing `nismod-snail-0.2.1/tests/cpp/tests_transform.cpp` & `nismod-snail-0.3.0/tests/cpp/tests_transform.cpp`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/tests/split_polygons_rings.py` & `nismod-snail-0.3.0/tests/split_polygons_rings.py`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/tests/test_routing.py` & `nismod-snail-0.3.0/tests/test_routing.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 from snail.routing import shortest_paths
 
 
 class TestSnailRouting(unittest.TestCase):
     def test_shortest_paths(self):
         """
-               1    e1    2
-               *----------*
-            e0/      1     \e2
-             / 1 	    \
-          0 *    	     *3
-             \     	    /
-            e4\          3 /
-               *---------- e3
-               4
+             e4
+            0--4
+        e0  |  |
+            1  | e3
+        e1  |  |
+            2--3
+             e2
         """
         g = Graph.Ring(n=5, circular=True)
         g.vs["name"] = ["node_" + str(i) for i in range(5)]
         g.es["length_km"] = [1, 1, 1, 3, 1]
-        sps = shortest_paths(["node_0", "node_2"], ["node_4", "node_3"], g, "length_km")
+        sps = shortest_paths(
+            ["node_0", "node_2"], ["node_4", "node_3"], g, "length_km"
+        )
         expected_paths = [
-            [4], [0, 1, 2], [1, 0, 4], [2]
-            ]
+            [4],  # 0 to 4, along edge 4
+            [0, 1, 2],  # 0 to 3, avoids long edge 3
+            [1, 0, 4],  # 2 to 4, avoids long edge 3
+            [2],  # 2 to 3, along edge 2
+        ]
         self.assertEqual(sps, expected_paths)
-
-
```

### Comparing `nismod-snail-0.2.1/tutorials/01-data-preparation-ghana.ipynb` & `nismod-snail-0.3.0/tutorials/01-data-preparation-ghana.ipynb`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/tutorials/02-assess-damage-and-disruption.ipynb` & `nismod-snail-0.3.0/tutorials/02-assess-damage-and-disruption.ipynb`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/tutorials/03-test-multiple-failures.ipynb` & `nismod-snail-0.3.0/tutorials/03-test-multiple-failures.ipynb`

 * *Files identical despite different names*

### Comparing `nismod-snail-0.2.1/tutorials/04-evaluate-adaptation-options.ipynb` & `nismod-snail-0.3.0/tutorials/04-evaluate-adaptation-options.ipynb`

 * *Files identical despite different names*

