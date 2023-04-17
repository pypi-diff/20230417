# Comparing `tmp/dials_data-2.4.8.tar.gz` & `tmp/dials_data-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dials_data-2.4.8.tar", last modified: Mon Mar  7 16:13:36 2022, max compression
+gzip compressed data, was "dials_data-2.4.9.tar", last modified: Tue Mar  8 09:34:37 2022, max compression
```

## Comparing `dials_data-2.4.8.tar` & `dials_data-2.4.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-07 16:13:36.186925 dials_data-2.4.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     3357 2022-03-07 16:13:27.000000 dials_data-2.4.8/CONTRIBUTING.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     2146 2022-03-07 16:13:27.000000 dials_data-2.4.8/HISTORY.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1486 2022-03-07 16:13:27.000000 dials_data-2.4.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      296 2022-03-07 16:13:27.000000 dials_data-2.4.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     5635 2022-03-07 16:13:36.186925 dials_data-2.4.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2491 2022-03-07 16:13:27.000000 dials_data-2.4.8/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-07 16:13:36.174925 dials_data-2.4.8/dials_data/
--rw-r--r--   0 vsts      (1001) docker     (121)      352 2022-03-07 16:13:35.000000 dials_data-2.4.8/dials_data/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4870 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/cli.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5214 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/datasets.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-07 16:13:36.178925 dials_data-2.4.8/dials_data/definitions/
--rw-r--r--   0 vsts      (1001) docker     (121)      987 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/MyD88_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1364 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/aluminium_standard.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2511 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/blend_tutorial.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     4110 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/centroid_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      903 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/cunir_serial.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1279 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/cunir_serial_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2094 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/four_circle_eiger.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    10198 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/fumarase.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      687 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/i19_1_pdteet_index.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2228 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/image_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     3659 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/insulin.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/insulin_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      800 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/isis_sxd_example_data.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1397 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    10657 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/l_cysteine_dials_output.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      725 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/lcls_rayonix_kapton.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/lysozyme_electron_diffraction.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/mpro_x0305_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    11627 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/mpro_x0692.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1761 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/multi_crystal_proteinase_k.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      761 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/pycbf.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      150 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/pychef.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2403 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/quartz_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    20032 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/relion_tutorial_data.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    83017 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/small_molecule_example.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1279 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/spring8_ccp4_2018.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/thaumatin_eiger_screen.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2750 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/thaumatin_grid_scan.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    45846 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/thaumatin_i04.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2479 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/trypsin_multi_lattice.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2459 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/vmxi_proteinase_k_sweeps.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/vmxi_thaumatin.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      645 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/vmxi_thaumatin_grid_index.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     7832 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/x4wide.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      755 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/definitions/x4wide_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    12055 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/download.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-07 16:13:36.182925 dials_data-2.4.8/dials_data/hashinfo/
--rw-r--r--   0 vsts      (1001) docker     (121)      276 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/MyD88_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/aluminium_standard.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2566 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/blend_tutorial.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2642 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/centroid_test_data.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      547 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/cunir_serial.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      624 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/cunir_serial_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      375 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/four_circle_eiger.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    10782 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/fumarase.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      279 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/i19_1_pdteet_index.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1340 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/image_examples.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     4152 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/insulin.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1162 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/insulin_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      642 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/isis_sxd_example_data.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      634 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     7029 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/l_cysteine_dials_output.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      366 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/lcls_rayonix_kapton.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      275 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/lysozyme_electron_diffraction.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/mpro_x0305_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/mpro_x0692.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1502 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/multi_crystal_proteinase_k.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      369 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/pycbf.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/pychef.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/relion_tutorial_data.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    79302 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/small_molecule_example.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/spring8_ccp4_2018.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/thaumatin_eiger_screen.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1793 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/thaumatin_grid_scan.yml
--rw-r--r--   0 vsts      (1001) docker     (121)    48162 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/thaumatin_i04.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     2504 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/trypsin_multi_lattice.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1526 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/vmxi_thaumatin.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      278 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/vmxi_thaumatin_grid_index.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     8112 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/x4wide.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/hashinfo/x4wide_processed.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-03-07 16:13:27.000000 dials_data-2.4.8/dials_data/pytest11.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-07 16:13:36.174925 dials_data-2.4.8/dials_data.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     5635 2022-03-07 16:13:36.000000 dials_data-2.4.8/dials_data.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     3624 2022-03-07 16:13:36.000000 dials_data-2.4.8/dials_data.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-03-07 16:13:36.000000 dials_data-2.4.8/dials_data.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-07 16:13:36.000000 dials_data-2.4.8/dials_data.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-03-07 16:13:36.000000 dials_data-2.4.8/dials_data.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       48 2022-03-07 16:13:36.000000 dials_data-2.4.8/dials_data.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-03-07 16:13:36.000000 dials_data-2.4.8/dials_data.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-07 16:13:36.186925 dials_data-2.4.8/docs/
--rwxr-xr-x   0 vsts      (1001) docker     (121)     4880 2022-03-07 16:13:27.000000 dials_data-2.4.8/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (121)       33 2022-03-07 16:13:27.000000 dials_data-2.4.8/docs/contributing.rst
--rw-r--r--   0 vsts      (1001) docker     (121)       28 2022-03-07 16:13:27.000000 dials_data-2.4.8/docs/history.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1997 2022-03-07 16:13:27.000000 dials_data-2.4.8/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     5127 2022-03-07 16:13:27.000000 dials_data-2.4.8/docs/installation.rst
--rw-r--r--   0 vsts      (1001) docker     (121)       27 2022-03-07 16:13:27.000000 dials_data-2.4.8/docs/readme.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     3976 2022-03-07 16:13:27.000000 dials_data-2.4.8/docs/why.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      217 2022-03-07 16:13:27.000000 dials_data-2.4.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     1618 2022-03-07 16:13:36.186925 dials_data-2.4.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      128 2022-03-07 16:13:27.000000 dials_data-2.4.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-07 16:13:36.186925 dials_data-2.4.8/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)     2468 2022-03-07 16:13:27.000000 dials_data-2.4.8/tests/test_dials_data.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2325 2022-03-07 16:13:27.000000 dials_data-2.4.8/tests/test_yaml_files.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3357 2022-03-08 09:34:30.000000 dials_data-2.4.9/CONTRIBUTING.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     2146 2022-03-08 09:34:30.000000 dials_data-2.4.9/HISTORY.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1486 2022-03-08 09:34:30.000000 dials_data-2.4.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      296 2022-03-08 09:34:30.000000 dials_data-2.4.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     5635 2022-03-08 09:34:37.645043 dials_data-2.4.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     2491 2022-03-08 09:34:30.000000 dials_data-2.4.9/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.633043 dials_data-2.4.9/dials_data/
+-rw-r--r--   0 vsts      (1001) docker     (121)      352 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4870 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5214 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/datasets.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.637043 dials_data-2.4.9/dials_data/definitions/
+-rw-r--r--   0 vsts      (1001) docker     (121)      987 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/MyD88_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1364 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/aluminium_standard.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2511 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/blend_tutorial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     4110 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/centroid_test_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      903 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/cunir_serial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1279 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/cunir_serial_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2094 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/four_circle_eiger.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    10198 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/fumarase.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      687 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/i19_1_pdteet_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2228 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/image_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     3659 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/insulin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/insulin_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      800 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/isis_sxd_example_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1397 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    10657 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/l_cysteine_dials_output.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      725 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/lcls_rayonix_kapton.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/lysozyme_electron_diffraction.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      924 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/mpro_x0305_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    11627 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/mpro_x0692.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1761 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/multi_crystal_proteinase_k.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      761 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/pycbf.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      150 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/pychef.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2403 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/quartz_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    20032 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/relion_tutorial_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    83017 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/small_molecule_example.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1279 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/spring8_ccp4_2018.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/thaumatin_eiger_screen.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2750 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/thaumatin_grid_scan.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    45846 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/thaumatin_i04.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2479 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/trypsin_multi_lattice.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2459 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/vmxi_proteinase_k_sweeps.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      645 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin_grid_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     7832 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/x4wide.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      755 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/definitions/x4wide_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    11892 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/download.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/dials_data/hashinfo/
+-rw-r--r--   0 vsts      (1001) docker     (121)      276 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/MyD88_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/aluminium_standard.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2566 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/blend_tutorial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2642 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/centroid_test_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      547 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/cunir_serial.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      624 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/cunir_serial_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      375 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/four_circle_eiger.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    10782 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/fumarase.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      279 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/i19_1_pdteet_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1340 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/image_examples.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     4152 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/insulin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1162 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/insulin_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      642 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/isis_sxd_example_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      634 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     7029 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/l_cysteine_dials_output.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      366 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/lcls_rayonix_kapton.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      275 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/lysozyme_electron_diffraction.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/mpro_x0305_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/mpro_x0692.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1502 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/multi_crystal_proteinase_k.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      369 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/pycbf.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/pychef.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      191 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/relion_tutorial_data.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    79302 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/small_molecule_example.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/spring8_ccp4_2018.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/thaumatin_eiger_screen.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1793 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/thaumatin_grid_scan.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)    48162 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/thaumatin_i04.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     2504 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/trypsin_multi_lattice.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1526 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/vmxi_thaumatin.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      278 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/vmxi_thaumatin_grid_index.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     8112 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/x4wide.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/hashinfo/x4wide_processed.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-03-08 09:34:30.000000 dials_data-2.4.9/dials_data/pytest11.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.633043 dials_data-2.4.9/dials_data.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5635 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     3624 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)       48 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-03-08 09:34:37.000000 dials_data-2.4.9/dials_data.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/docs/
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     4880 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       33 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/contributing.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)       28 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/history.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     1997 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     5127 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/installation.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)       27 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/readme.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)     3976 2022-03-08 09:34:30.000000 dials_data-2.4.9/docs/why.rst
+-rw-r--r--   0 vsts      (1001) docker     (121)      217 2022-03-08 09:34:30.000000 dials_data-2.4.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)     1618 2022-03-08 09:34:37.645043 dials_data-2.4.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      128 2022-03-08 09:34:30.000000 dials_data-2.4.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-03-08 09:34:37.645043 dials_data-2.4.9/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2468 2022-03-08 09:34:30.000000 dials_data-2.4.9/tests/test_dials_data.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2325 2022-03-08 09:34:30.000000 dials_data-2.4.9/tests/test_yaml_files.py
```

### Comparing `dials_data-2.4.8/CONTRIBUTING.rst` & `dials_data-2.4.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/HISTORY.rst` & `dials_data-2.4.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/LICENSE` & `dials_data-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/PKG-INFO` & `dials_data-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dials_data
-Version: 2.4.8
+Version: 2.4.9
 Summary: DIALS Regression Data Manager
 Home-page: https://github.com/dials/data
 Author: DIALS development team
 Author-email: dials-support@lists.sourceforge.net
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/dials/data/issues
 Project-URL: Documentation, https://dials-data.readthedocs.io/
```

### Comparing `dials_data-2.4.8/README.rst` & `dials_data-2.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/cli.py` & `dials_data-2.4.9/dials_data/cli.py`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/datasets.py` & `dials_data-2.4.9/dials_data/datasets.py`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/MyD88_processed.yml` & `dials_data-2.4.9/dials_data/definitions/MyD88_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/aluminium_standard.yml` & `dials_data-2.4.9/dials_data/definitions/aluminium_standard.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/blend_tutorial.yml` & `dials_data-2.4.9/dials_data/definitions/blend_tutorial.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/centroid_test_data.yml` & `dials_data-2.4.9/dials_data/definitions/centroid_test_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/cunir_serial.yml` & `dials_data-2.4.9/dials_data/definitions/cunir_serial.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/cunir_serial_processed.yml` & `dials_data-2.4.9/dials_data/definitions/cunir_serial_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/four_circle_eiger.yml` & `dials_data-2.4.9/dials_data/definitions/four_circle_eiger.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/fumarase.yml` & `dials_data-2.4.9/dials_data/definitions/fumarase.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/i19_1_pdteet_index.yml` & `dials_data-2.4.9/dials_data/definitions/i19_1_pdteet_index.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/image_examples.yml` & `dials_data-2.4.9/dials_data/definitions/image_examples.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/insulin.yml` & `dials_data-2.4.9/dials_data/definitions/insulin.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/insulin_processed.yml` & `dials_data-2.4.9/dials_data/definitions/insulin_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/isis_sxd_example_data.yml` & `dials_data-2.4.9/dials_data/definitions/isis_sxd_example_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml` & `dials_data-2.4.9/dials_data/definitions/l_cysteine_4_sweeps_scaled.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/l_cysteine_dials_output.yml` & `dials_data-2.4.9/dials_data/definitions/l_cysteine_dials_output.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/lcls_rayonix_kapton.yml` & `dials_data-2.4.9/dials_data/definitions/lcls_rayonix_kapton.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/lysozyme_electron_diffraction.yml` & `dials_data-2.4.9/dials_data/definitions/lysozyme_electron_diffraction.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/mpro_x0305_processed.yml` & `dials_data-2.4.9/dials_data/definitions/mpro_x0305_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/mpro_x0692.yml` & `dials_data-2.4.9/dials_data/definitions/mpro_x0692.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/multi_crystal_proteinase_k.yml` & `dials_data-2.4.9/dials_data/definitions/multi_crystal_proteinase_k.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/pycbf.yml` & `dials_data-2.4.9/dials_data/definitions/pycbf.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/quartz_processed.yml` & `dials_data-2.4.9/dials_data/definitions/quartz_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/relion_tutorial_data.yml` & `dials_data-2.4.9/dials_data/definitions/relion_tutorial_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/small_molecule_example.yml` & `dials_data-2.4.9/dials_data/definitions/small_molecule_example.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/spring8_ccp4_2018.yml` & `dials_data-2.4.9/dials_data/definitions/spring8_ccp4_2018.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/thaumatin_eiger_screen.yml` & `dials_data-2.4.9/dials_data/definitions/thaumatin_eiger_screen.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/thaumatin_grid_scan.yml` & `dials_data-2.4.9/dials_data/definitions/thaumatin_grid_scan.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/thaumatin_i04.yml` & `dials_data-2.4.9/dials_data/definitions/thaumatin_i04.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/trypsin_multi_lattice.yml` & `dials_data-2.4.9/dials_data/definitions/trypsin_multi_lattice.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/vmxi_proteinase_k_sweeps.yml` & `dials_data-2.4.9/dials_data/definitions/vmxi_proteinase_k_sweeps.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/vmxi_thaumatin.yml` & `dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/vmxi_thaumatin_grid_index.yml` & `dials_data-2.4.9/dials_data/definitions/vmxi_thaumatin_grid_index.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/x4wide.yml` & `dials_data-2.4.9/dials_data/definitions/x4wide.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/definitions/x4wide_processed.yml` & `dials_data-2.4.9/dials_data/definitions/x4wide_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/download.py` & `dials_data-2.4.9/dials_data/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,27 +70,14 @@
         lock = True
         yield
     finally:
         if lock:
             _platform_unlock(file_handle)
 
 
-@contextlib.contextmanager
-def download_lock(target_dir: Path):
-    """
-    Obtains a (cooperative) lock on a lockfile in a target directory, so only a
-    single (cooperative) process can enter this context manager at any one time.
-    If the lock is held this will block until the existing lock is released.
-    """
-    target_dir.mkdir(parents=True, exist_ok=True)
-    with target_dir.joinpath(".lock").open(mode="w") as fh:
-        with _file_lock(fh):
-            yield
-
-
 def _download_to_file(session: requests.Session, url: str, pyfile: Path):
     """
     Downloads a single URL to a file.
     """
     with session.get(url, stream=True) as r:
         r.raise_for_status()
         pyfile.parent.mkdir(parents=True, exist_ok=True)
@@ -165,17 +152,22 @@
             and item["verify"]["size"] == item["file"].stat().st_size
             for item in filelist
         ):
             return True
         if read_only:
             return False
 
-    # Acquire lock on directory as files may be downloaded/written.
-    with download_lock(target_dir):
-        verification_records = _fetch_filelist(filelist)
+    # Obtain a (cooperative) lock on a dataset-specific lockfile, so only one
+    # (cooperative) process can enter this context at any one time. The lock
+    # file sits in the directory above the dataset directory, as to not
+    # interfere with dataset files.
+    target_dir.mkdir(parents=True, exist_ok=True)
+    with target_dir.with_name(f".lock.{dataset}").open(mode="w") as fh:
+        with _file_lock(fh):
+            verification_records = _fetch_filelist(filelist)
 
     # If any errors occured during download then don't trust the dataset.
     if verify and not all(verification_records):
         return False
 
     integrity_info["verify"] = verification_records
     return integrity_info
```

### Comparing `dials_data-2.4.8/dials_data/hashinfo/blend_tutorial.yml` & `dials_data-2.4.9/dials_data/hashinfo/blend_tutorial.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/centroid_test_data.yml` & `dials_data-2.4.9/dials_data/hashinfo/centroid_test_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/cunir_serial.yml` & `dials_data-2.4.9/dials_data/hashinfo/cunir_serial.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/cunir_serial_processed.yml` & `dials_data-2.4.9/dials_data/hashinfo/cunir_serial_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/fumarase.yml` & `dials_data-2.4.9/dials_data/hashinfo/fumarase.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/image_examples.yml` & `dials_data-2.4.9/dials_data/hashinfo/image_examples.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/insulin.yml` & `dials_data-2.4.9/dials_data/hashinfo/insulin.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/insulin_processed.yml` & `dials_data-2.4.9/dials_data/hashinfo/insulin_processed.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/isis_sxd_example_data.yml` & `dials_data-2.4.9/dials_data/hashinfo/isis_sxd_example_data.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml` & `dials_data-2.4.9/dials_data/hashinfo/l_cysteine_4_sweeps_scaled.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/l_cysteine_dials_output.yml` & `dials_data-2.4.9/dials_data/hashinfo/l_cysteine_dials_output.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/multi_crystal_proteinase_k.yml` & `dials_data-2.4.9/dials_data/hashinfo/multi_crystal_proteinase_k.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/small_molecule_example.yml` & `dials_data-2.4.9/dials_data/hashinfo/small_molecule_example.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/thaumatin_grid_scan.yml` & `dials_data-2.4.9/dials_data/hashinfo/thaumatin_grid_scan.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/thaumatin_i04.yml` & `dials_data-2.4.9/dials_data/hashinfo/thaumatin_i04.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/trypsin_multi_lattice.yml` & `dials_data-2.4.9/dials_data/hashinfo/trypsin_multi_lattice.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml` & `dials_data-2.4.9/dials_data/hashinfo/vmxi_proteinase_k_sweeps.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/hashinfo/x4wide.yml` & `dials_data-2.4.9/dials_data/hashinfo/x4wide.yml`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data/pytest11.py` & `dials_data-2.4.9/dials_data/pytest11.py`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/dials_data.egg-info/PKG-INFO` & `dials_data-2.4.9/dials_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dials-data
-Version: 2.4.8
+Version: 2.4.9
 Summary: DIALS Regression Data Manager
 Home-page: https://github.com/dials/data
 Author: DIALS development team
 Author-email: dials-support@lists.sourceforge.net
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/dials/data/issues
 Project-URL: Documentation, https://dials-data.readthedocs.io/
```

### Comparing `dials_data-2.4.8/dials_data.egg-info/SOURCES.txt` & `dials_data-2.4.9/dials_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/docs/conf.py` & `dials_data-2.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/docs/index.rst` & `dials_data-2.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/docs/installation.rst` & `dials_data-2.4.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/docs/why.rst` & `dials_data-2.4.9/docs/why.rst`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/setup.cfg` & `dials_data-2.4.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dials_data
-version = 2.4.8
+version = 2.4.9
 url = https://github.com/dials/data
 project_urls = 
 	Bug Tracker = https://github.com/dials/data/issues
 	Documentation = https://dials-data.readthedocs.io/
 	Source Code = https://github.com/dials/data
 description = DIALS Regression Data Manager
 author = DIALS development team
```

### Comparing `dials_data-2.4.8/tests/test_dials_data.py` & `dials_data-2.4.9/tests/test_dials_data.py`

 * *Files identical despite different names*

### Comparing `dials_data-2.4.8/tests/test_yaml_files.py` & `dials_data-2.4.9/tests/test_yaml_files.py`

 * *Files identical despite different names*

