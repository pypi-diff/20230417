# Comparing `tmp/scikit-rt-0.4.1.tar.gz` & `tmp/scikit-rt-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-rt-0.4.1.tar", last modified: Tue Apr 11 15:52:14 2023, max compression
+gzip compressed data, was "scikit-rt-0.4.2.tar", last modified: Mon Apr 17 10:44:05 2023, max compression
```

## Comparing `scikit-rt-0.4.1.tar` & `scikit-rt-0.4.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.279893 scikit-rt-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-11 15:52:14.279893 scikit-rt-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-11 15:52:14.279893 scikit-rt-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.259893 scikit-rt-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.259893 scikit-rt-0.4.1/src/scikit_rt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-11 15:52:14.000000 scikit-rt-0.4.1/src/scikit_rt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-11 15:52:14.000000 scikit-rt-0.4.1/src/scikit_rt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:52:14.000000 scikit-rt-0.4.1/src/scikit_rt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-11 15:52:14.000000 scikit-rt-0.4.1/src/scikit_rt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 15:52:14.000000 scikit-rt-0.4.1/src/scikit_rt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.267893 scikit-rt-0.4.1/src/skrt/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.267893 scikit-rt-0.4.1/src/skrt/better_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)   131500 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/better_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/better_viewer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    72208 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.259893 scikit-rt-0.4.1/src/skrt/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.267893 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_Affine.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_Translation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.271893 scikit-rt-0.4.1/src/skrt/data/niftyreg_parameter_files/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/niftyreg_parameter_files/Affine.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/data/niftyreg_parameter_files/Rigid.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/dicom_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    35313 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/dose.py
--rw-r--r--   0 runner    (1001) docker     (123)   231542 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)   105267 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/patient.py
--rw-r--r--   0 runner    (1001) docker     (123)   122005 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    51836 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)   349221 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.271893 scikit-rt-0.4.1/src/skrt/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/viewer/core.py
--rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/src/skrt/viewer/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:52:14.279893 scikit-rt-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_01_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_dose.py
--rw-r--r--   0 runner    (1001) docker     (123)    53749 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_patient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_qv_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_qv_quickviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_qv_struct_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_qv_struct_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_qv_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32378 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_roi_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_synthetic_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-11 15:47:39.000000 scikit-rt-0.4.1/tests/test_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.101863 scikit-rt-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-17 10:44:05.101863 scikit-rt-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-17 10:44:05.101863 scikit-rt-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.093862 scikit-rt-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.097863 scikit-rt-0.4.2/src/scikit_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-17 10:44:04.000000 scikit-rt-0.4.2/src/scikit_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-17 10:44:05.000000 scikit-rt-0.4.2/src/scikit_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:44:04.000000 scikit-rt-0.4.2/src/scikit_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-17 10:44:04.000000 scikit-rt-0.4.2/src/scikit_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 10:44:04.000000 scikit-rt-0.4.2/src/scikit_rt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.097863 scikit-rt-0.4.2/src/skrt/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.097863 scikit-rt-0.4.2/src/skrt/better_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)   131500 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/better_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/better_viewer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72208 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.093862 scikit-rt-0.4.2/src/skrt/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.097863 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_Affine.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_Rigid.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_Translation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.101863 scikit-rt-0.4.2/src/skrt/data/niftyreg_parameter_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/niftyreg_parameter_files/Affine.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/niftyreg_parameter_files/BE_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/niftyreg_parameter_files/NMI_BSpline05.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/niftyreg_parameter_files/NMI_BSpline15.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/niftyreg_parameter_files/NMI_BSpline30.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/data/niftyreg_parameter_files/Rigid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23275 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/dicom_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35313 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)   239611 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105267 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122005 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52538 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)   349272 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.101863 scikit-rt-0.4.2/src/skrt/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154795 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/viewer/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113136 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/src/skrt/viewer/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:44:05.101863 scikit-rt-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_01_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_dose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58059 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_patient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_qv_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_qv_quickviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_qv_struct_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_qv_struct_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_qv_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32378 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21138 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_roi_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65888 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_synthetic_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-17 10:40:00.000000 scikit-rt-0.4.2/tests/test_viewer.py
```

### Comparing `scikit-rt-0.4.1/LICENSE` & `scikit-rt-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/PKG-INFO` & `scikit-rt-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.1
+Version: 0.4.2
 Summary: Toolkit for radiotherapy image analysis
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.1/README.md` & `scikit-rt-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/setup.cfg` & `scikit-rt-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-rt
-version = 0.4.1
+version = 0.4.2
 author = H. Pullen, K. Harrison
 author_email = scikit-rt@hep.phy.cam.ac.uk
 description = Toolkit for radiotherapy image analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/scikit-rt/scikit-rt
 project_urls =
```

### Comparing `scikit-rt-0.4.1/src/scikit_rt.egg-info/PKG-INFO` & `scikit-rt-0.4.2/src/scikit_rt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-rt
-Version: 0.4.1
+Version: 0.4.2
 Summary: Toolkit for radiotherapy image analysis
 Home-page: https://github.com/scikit-rt/scikit-rt
 Author: H. Pullen, K. Harrison
 Author-email: scikit-rt@hep.phy.cam.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/scikit-rt/scikit-rt/issues
 Description: # Scikit-rt
```

### Comparing `scikit-rt-0.4.1/src/scikit_rt.egg-info/SOURCES.txt` & `scikit-rt-0.4.2/src/scikit_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/scikit_rt.egg-info/requires.txt` & `scikit-rt-0.4.2/src/scikit_rt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/__init__.py` & `scikit-rt-0.4.2/src/skrt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/application.py` & `scikit-rt-0.4.2/src/skrt/application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/better_viewer/__init__.py` & `scikit-rt-0.4.2/src/skrt/better_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/better_viewer/options.py` & `scikit-rt-0.4.2/src/skrt/better_viewer/options.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/core.py` & `scikit-rt-0.4.2/src/skrt/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt` & `scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/BE_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_Affine.txt` & `scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_Affine.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt` & `scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_BSpline05.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt` & `scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_BSpline15.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt` & `scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_BSpline30.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_Rigid.txt` & `scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_Rigid.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/data/elastix_parameter_files/MI_Translation.txt` & `scikit-rt-0.4.2/src/skrt/data/elastix_parameter_files/MI_Translation.txt`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/dicom_writer.py` & `scikit-rt-0.4.2/src/skrt/dicom_writer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/dose.py` & `scikit-rt-0.4.2/src/skrt/dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/image.py` & `scikit-rt-0.4.2/src/skrt/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1459,14 +1459,43 @@
             return masks[1]
 
         if masks[1] is not None:
             masks[0].data[masks[1].data > 0] = 0
 
         return masks[0]
 
+    def rescale(self, v_min=0.0, v_max=1.0, constant=0.5):
+        '''
+        Linearly rescale image greyscale values,
+        so that they span a specified range.
+
+        **Parameters:**
+
+        v_min: float, default=0.0
+            Minimum greyscale value after rescaling.
+
+        v_max: float, default=1.0
+            Maximum greyscale value after rescaling.
+
+        constant: float, default=0.5
+            Greyscale value to assign after rescaling if all values
+            in the original image are the same.  If None,
+            original value is kept.
+        '''
+        # Perform rescaling.
+        u_min = self.get_min(force=True)
+        u_max = self.get_max(force=True)
+        du = u_max - u_min
+        dv = v_max - v_min
+        if du:
+            self.data = v_min + ((self.data.astype(np.float32) - u_min)
+                                 * (dv / du))
+        elif constant is not None:
+            self.data.fill(constant)
+
     def resize(self, image_size=None, origin=None, voxel_size=None,
             fill_value=None, image_size_unit=None, centre=None,
             keep_centre=False, method='linear'):
         '''
         Resize image to specified image size, voxel size and origin.
 
         **Parameters:**
@@ -1715,19 +1744,22 @@
 
         if not force and hasattr(self, "_min"):
             return self._min
         self.load()
         self._min = self.data.min()
         return self._min
 
-    def get_max(self):
+    def get_max(self, force=False):
         """Get maximum greyscale value of data array."""
 
+        if not force and hasattr(self, "_max"):
+            return self._max
         self.load()
-        return self.data.max()
+        self._max = self.data.max()
+        return self._max
 
     def get_centroid_idx(self, view="x-y", fraction=1):
         """
         Get array index of slice containing centroid of above-threshold voxels.
 
         The centroid coordinate along a given axis is calculated as the
         unweighted mean of the coordinates of voxels with an intensity at
@@ -3888,43 +3920,54 @@
           and higher values by the amounts specified;
         - None : no cropping is performed.
 
         For more details, see documentation of skrt.image.crop_by_amounts().
         """
         crop_by_amounts(self, dx, dy, dz)
 
-    def crop_to_roi(self, roi, crop_margins=None, method=None):
+    def crop_to_roi(self, roi, crop_margins=None, crop_about_centre=False,
+                    method=None):
         """
-        Crop image to region covered by an ROI or StructureSet, plus margins.
+        Crop image to region defined by an ROI or StructureSet, plus margins.
 
         **Parameters:**
 
         rois : skrt.structures.ROI/skirt.structures.StructureSet
             ROI or StructureSet to which image will be cropped.
 
         crop_margins : float/tuple, default=None
             Float or three-element tuple specifying the margins, in mm,
-            to be added to StructureSet extents.  If a float, minus and plus the
-            value specified are added to lower and upper extents respectively
-            along each axis.  If a three-element tuple, elements are
-            taken to specify margins in the order (x, y, z).  Elements
-            can be either floats (minus and plus the value added respectively
-            to lower and upper extents) or two-element tuples (elements 0 and 1
-            added respectively to lower and upper extents).
+            to be added to extents or centre point of ROI or StructureSet.  If
+            a float, minus and plus the value specified are added to lower
+            and upper extents respectively along each axis.  If a
+            three-element tuple, elements are taken to specify margins in
+            the order (x, y, z).  Elements can be either floats (minus and
+            plus the value added respectively to lower and upper extents)
+            or two-element tuples (elements 0 and 1 added respectively
+            to lower and upper extents).
+
+        crop_about_centre : bool, default=False
+            If True, image is cropped to the centre point of ROI or
+            StructureSet plus margins.  If False, image is cropped to 
+            the extents of ROI or StructureSet plus margins.
 
         method : str, default=None
             Method to use for calculating extent of <roi> region. Can be: 
 
                 * "contour": get extent from min/max positions of contour(s).
                 * "mask": get extent from min/max positions of voxels in the 
                   binary mask.
                 * None: use the method set in self.default_geom_method.
         """
-        self.crop(*roi.get_crop_limits(
-            crop_margins=crop_margins, method=method))
+        if crop_about_centre:
+            self.crop_about_point(roi.get_centre(method=method),
+                                  *checked_crop_limits(crop_margins))
+        else:
+            self.crop(*roi.get_crop_limits(
+                crop_margins=crop_margins, method=method))
 
     def crop_to_image(self, image, alignment=None):
         """
         Crop to extents of another image, optionally after image alignment.
 
         **Parameters:**
 
@@ -4317,14 +4360,132 @@
         elif variant in ["iqr", "information_quality_ratio"]:
             return mi / (hxy or small_number)
         if variant in ["rajski", "rajski_distance"]:
             return 1 - mi / (hxy or small_number)
 
         return mi
 
+    def get_relative_structural_content(
+            self, image, v_min=None, v_max=None, constant=None):
+        """
+        Quantify structural content of this image relative to another.
+
+        The calculation of relative structural content is based on
+        the definition of:
+
+        - https://doi.org/10.1364/JOSA.46.000740
+        - https://doi.org/10.1080/713826248
+
+        The result should be from 0 (no agreement) to 1 (perfect agreement).
+
+        The parameters v_min, v_max, constant allow for linear rescaling
+        of image greyscale values prior to calculation of relative
+        structural content.  Any rescaling is performed on clones of
+        the images to be compared, with the originals left unaltered.
+
+        **Parameters:**
+
+        image : skrt.image.Image
+            Image with respect to which relative structural content
+            is to be calculated.
+
+        v_min: float, default=None
+            Minimum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        v_max: float, default=None
+            Maximum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        constant: float, default=None
+            Greyscale value to assign after rescaling if all values
+            in the original image are the same.  If None,
+            original value is kept.
+        """
+        im1, im2 = rescale_images([self, image], v_min, v_max, constant)
+        return ((im1.get_data()**2).sum() / (im2.get_data()**2).sum())
+
+    def get_fidelity(self, image, v_min=None, v_max=None, constant=None):
+        """
+        Calculate fidelity with which this image matches another.
+
+        The calculation of fidelity is based on the definition of:
+
+        - https://doi.org/10.1364/JOSA.46.000740
+        - https://doi.org/10.1080/713826248
+
+        The result should be from 0 (no agreement) to 1 (perfect agreement).
+
+        The parameters v_min, v_max, constant allow for linear rescaling
+        of image greyscale values prior to calculation of fidelity.  Any
+        rescaling is performed on clones of the images to be compared,
+        with the originals left unaltered.
+
+        **Parameters:**
+
+        image : skrt.image.Image
+            Image with respect to which fidelity is to be calculated.
+
+        v_min: float, default=None
+            Minimum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        v_max: float, default=None
+            Maximum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        constant: float, default=None
+            Greyscale value to assign after rescaling if all values
+            in the original image are the same.  If None,
+            original value is kept.
+        """
+        im1, im2 = rescale_images([self, image], v_min, v_max, constant)
+        return (1 - (((im2.get_data() - im1.get_data())**2).sum()
+                / (im2.get_data()**2).sum()))
+
+    def get_correlation_quality(
+            self, image, v_min=None, v_max=None, constant=None):
+        """
+        Calculate quality of correlation between this image and another.
+
+        The calculation of correlation quality is based on the definition of:
+
+        - https://doi.org/10.1364/JOSA.46.000740
+        - https://doi.org/10.1080/713826248
+
+        The result should be from 0 (no agreement) to 1 (perfect agreement).
+
+        The parameters v_min, v_max, constant allow for linear rescaling
+        of image greyscale values prior to calculation of correlation
+        quality.  Any rescaling is performed on clones of the images
+        to be compared, with the originals left unaltered.
+
+        **Parameters:**
+
+        image : skrt.image.Image
+            Image with respect to which correlation quality is to be calculated.
+
+        v_min: float, default=None
+            Minimum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        v_max: float, default=None
+            Maximum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        constant: float, default=None
+            Greyscale value to assign after rescaling if all values
+            in the original image are the same.  If None,
+            original value is kept.
+        """
+        im1, im2 = rescale_images([self, image], v_min, v_max, constant)
+        return ((im2.get_data() * im1.get_data()).sum()
+                / (im2.get_data()**2).sum())
+
+
 class ImageComparison(Image):
     """Plot comparisons of two images and calculate comparison metrics."""
 
     def __init__(self, im1, im2, plot_type="overlay", title=None, **kwargs):
 
         # Load images
         self.ims = []
@@ -6033,26 +6194,27 @@
                 if 1 == len(roi_alignments[idx]):
                     roi_alignments[idx] = [roi_alignments[idx][0], None]
 
     return roi_alignments
 
 def match_images(im1, im2, ss1=None, ss2=None, ss1_index=-1, ss2_index=-1,
                  ss1_name=None, ss2_name=None, roi_names=None,
-                 im2_crop_focus=None, im2_crop_margins=None, alignment=None,
+                 im2_crop_focus=None, im2_crop_margins=None,
+                 im2_crop_about_centre=False, alignment=None,
                  voxel_size=None, bands=None):
     """
     Process pair of images, so that they match in one or more respects.
 
     Matching can be with respect to image size, voxel size,
     grey-level banding, and/or ROI naming in associated structure sets.
     The returned images are created from clones of the input images,
     which are left unchanged.
 
-    The first ROI of the pair may be cropped about a focus (ROI or point).
-    The second ROI of the pair may be cropped to the size of the first.
+    The second ROI of the pair may be cropped about a focus (ROI or point).
+    The first ROI of the pair may be cropped to the size of the first.
 
     **Parameters:**
 
     im1, im2 : skrt.image.Image
         Images to be matched with one another.
 
     ss1, ss2 : skrt.structures.StructureSet, default=None
@@ -6092,14 +6254,20 @@
         im2_crop_focus is the name of an ROI, see documentation for
         method skrt.image.Image.crop_to_roi(). For the case where
         im2_crop_focus is a point coordinate, margins should be
         sepecified by a tuple (xlim, ylim, zlim).  Here, xlim, ylim, zlim
         are two-component tuples specifying lower and upper bounds
         relative to the crop point.
 
+    im2_crop_about_centre: bool, default=False
+        For the case where im2_crop_focus is the name of an ROI:
+        if True, im2 is cropped to the centre point of the ROI plus margins;
+        if False, im2 is cropped to the ROI extents plus margins.
+        Ignored for the case where im2_crop_focus isn't the name of an ROI.
+
     alignment : tuple/dict/str, default=None
         Strategy to be used for aligning images prior to cropping
         so that they have the same size.  For strategy details, see
         documentation of skrt.image.get_alignment_translation().
         After alignment, im1 is cropped to the size of im2, then im2
         is cropped to the size of im1.  To omit cropping to the same
         size, set alginment to False.
@@ -6121,15 +6289,16 @@
     ss2 = im2.structure_sets[0] if im2.structure_sets else None
 
     # Resample images to same voxel size.
     match_image_voxel_sizes(im1, im2, voxel_size)
 
     # Crop im2 to region around focus.
     if ss2 is not None and im2_crop_focus in ss2.get_roi_names():
-        im2.crop_to_roi(ss2[im2_crop_focus], im2_crop_margins)
+        im2.crop_to_roi(ss2[im2_crop_focus], crop_margins=im2_crop_margins,
+                        crop_about_centre=im2_crop_about_centre)
     elif ((skrt.core.is_list(im2_crop_focus) or im2_crop_focus is None)
           and skrt.core.is_list(im2_crop_margins)):
         im2.crop_about_point(im2_crop_focus, *im2_crop_margins)
 
     # Crop images to same size.
     if alignment is not False:
         im1.crop_to_image(im2, alignment)
@@ -6331,7 +6500,55 @@
     base : int/None, default=2
         Base to use when taking logarithms.  If None, use base e.
     """
     if base is None:
         base = math.e
     p_non_zero = (p > 0)
     return -np.sum(p[p_non_zero] * np.log(p[p_non_zero])) /np.log(base)
+
+def rescale_images(images, v_min=0.0, v_max=1.0, constant=0.5, clone=True):
+    """
+    For one or more images, linearly rescale greyscale values
+    so that they span a specified range.
+
+    Returns the input images if no rescaling is performed.  Otherwise
+    returns the input images rescaled (<clone> set to False) or
+    rescaled clones of the input images (<clone> set to True).
+
+    image : list
+        List of skrt.image.Image objects, for which rescaling
+        is to be performed.
+
+        v_min: float, default=0.0
+            Minimum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        v_max: float, default=1.0
+            Maximum greyscale value after rescaling.  If None,
+            no rescaling is performed.
+
+        constant: float, default=0.5
+            Greyscale value to assign after rescaling if all values
+            in the original image are the same.  If None,
+            original value is kept.
+
+    clone : bool, default=True
+        If True, clone each input image before rescaling.
+    """
+    if v_min is None or v_max is None:
+        return images
+
+    # Try to ensure list of images.
+    if not skrt.core.is_list(images):
+        images = [images]
+    elif not isinstance(images, list):
+        images = list(images)
+
+    # Clone if required.
+    if clone:
+        images = [image.clone() for image in images]
+
+    # Perform rescaling.
+    for image in images:
+        image.rescale(v_min=v_min, v_max=v_max, constant=constant)
+
+    return images
```

### Comparing `scikit-rt-0.4.1/src/skrt/multi.py` & `scikit-rt-0.4.2/src/skrt/multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/patient.py` & `scikit-rt-0.4.2/src/skrt/patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/registration.py` & `scikit-rt-0.4.2/src/skrt/registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/segmentation.py` & `scikit-rt-0.4.2/src/skrt/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,23 +518,24 @@
                                 [self.df, df_sas], ignore_index=True)
 
 
 class SingleAtlasSegmentation(Data):
     def __init__(
         self, im1=None, im2=None, ss1=None, ss2=None, log_level=None,
         workdir="segmentation_workdir", overwrite=False,
-        engine=None, engine_dir=None,
-        auto=False, auto_step=None, auto_strategies=None,
-        auto_reg_setup_only=False,
+        engine=None, engine_dir=None, auto=False, auto_step=None,
+        auto_strategies=None, auto_reg_setup_only=False,
         default_step=-1, default_strategy="pull", roi_names=None,
         ss1_index=-1, ss2_index=-1, ss1_name="Filtered1", ss2_name="Filtered2",
         initial_crop_focus=None, initial_crop_margins=None,
-        initial_alignment=None, initial_transform_name=None,
-        crop_to_match_size1=True, voxel_size1=None, bands1=None, pfiles1=None, 
+        initial_crop_about_centre=False, initial_alignment=None,
+        initial_transform_name=None, crop_to_match_size1=True,
+        voxel_size1=None, bands1=None, pfiles1=None, 
         most_points1=True, roi_crop_margins=None, default_roi_crop_margins=10,
+        roi_crop_about_centre=None, default_roi_crop_about_centre=False,
         roi_pfiles=None, crop_to_match_size2=True, voxel_size2=None,
         default_roi_bands=None, roi_bands=None, pfiles2=None,
         most_points2=True, capture_output=False,
         keep_tmp_dir=False, metrics=None, default_slice_stats=None,
         default_by_slice=None):
 
         # Set images and associated structure sets.
@@ -576,24 +577,27 @@
         self.default_strategy = default_strategy or self.auto_strategies[-1]
         self.roi_names = roi_names
 
         # Set parameters for step-1 registration.
         self.initial_alignment = initial_alignment
         self.initial_crop_focus = initial_crop_focus
         self.initial_crop_margins = initial_crop_margins
+        self.initial_crop_about_centre = initial_crop_about_centre
         self.crop_to_match_size1 = crop_to_match_size1
         self.voxel_size1 = voxel_size1
         self.bands1 = bands1
         self.pfiles1 = {reg_step: pfile
                         for reg_step, pfile in (pfiles1 or {}).items() if pfile}
         self.most_points1 = most_points1
 
         # Set parameters for step-2 registration.
         self.roi_crop_margins = roi_crop_margins or {}
         self.default_roi_crop_margins = default_roi_crop_margins
+        self.roi_crop_about_centre = roi_crop_about_centre or {}
+        self.default_roi_crop_about_centre = default_roi_crop_about_centre
         self.crop_to_match_size2 = crop_to_match_size2
         self.voxel_size2 = voxel_size2
         self.roi_bands = roi_bands or {}
         self.default_roi_bands = default_roi_bands
         self.pfiles2 = pfiles2 or pfiles1
         self.pfiles2_non_null = {reg_step: pfile for reg_step, pfile
                                  in (self.pfiles2 or {}).items() if pfile}
@@ -649,14 +653,15 @@
                         ss1=self.ss1,
                         ss2=self.ss2,
                         ss1_name=self.ss1_name,
                         ss2_name=self.ss2_name,
                         roi_names=self.roi_names,
                         im2_crop_focus=self.initial_crop_focus,
                         im2_crop_margins=self.initial_crop_margins,
+                        im2_crop_about_centre=self.initial_crop_about_centre,
                         alignment=(self.initial_alignment
                                    if self.crop_to_match_size1 else False),
                         voxel_size=self.voxel_size1,
                         bands=self.bands1)
 
                 self.ss1_filtered = im1.structure_sets[0]
                 self.ss2_filtered = im2.structure_sets[0]
@@ -705,16 +710,22 @@
                             ss2_index = self.ss2_index,
                             ss1=self.get_segmentation(strategy, 0, -1),
                             ss2=self.ss2,
                             ss1_name=self.ss1_name,
                             ss2_name=self.ss2_name,
                             roi_names={roi_name: self.roi_names[roi_name]},
                             im2_crop_focus=roi_name,
-                            im2_crop_margins=self.roi_crop_margins.get(
-                                roi_name, self.default_roi_crop_margins),
+                            im2_crop_margins=(
+                                self.roi_crop_margins.get(
+                                    roi_name,
+                                    self.default_roi_crop_margins)),
+                            im2_crop_about_centre=(
+                                self.roi_crop_about_centre.get(
+                                    roi_name,
+                                    self.default_roi_crop_about_centre)),
                             alignment=(roi_name if self.crop_to_match_size2
                                        else False),
                             voxel_size=self.voxel_size2,
                             bands=self.roi_bands.get(
                                 roi_name, self.default_roi_bands)
                             )
```

### Comparing `scikit-rt-0.4.1/src/skrt/simulation.py` & `scikit-rt-0.4.2/src/skrt/simulation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/structures.py` & `scikit-rt-0.4.2/src/skrt/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -17702,4126 +17702,4129 @@
 00045250: 6178 6973 2e22 2222 0a0a 2020 2020 2020  axis."""..      
 00045260: 2020 6578 7465 6e74 203d 2073 656c 662e    extent = self.
 00045270: 6765 745f 6578 7465 6e74 2861 783d 6178  get_extent(ax=ax
 00045280: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
 00045290: 2061 6273 2865 7874 656e 745b 315d 202d   abs(extent[1] -
 000452a0: 2065 7874 656e 745b 305d 290a 0a20 2020   extent[0])..   
 000452b0: 2064 6566 2067 6574 5f63 656e 7472 6528   def get_centre(
-000452c0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000452d0: 2222 4765 7420 3344 2063 656e 7472 6520  ""Get 3D centre 
-000452e0: 6f66 2074 6865 2061 7265 6120 636f 7665  of the area cove
-000452f0: 7265 6420 6279 2052 4f49 732e 2222 220a  red by ROIs.""".
-00045300: 0a20 2020 2020 2020 2065 7874 656e 7473  .        extents
-00045310: 203d 205b 7365 6c66 2e67 6574 5f65 7874   = [self.get_ext
-00045320: 656e 7428 6178 3d61 7829 2066 6f72 2061  ent(ax=ax) for a
-00045330: 7820 696e 2073 6b72 742e 696d 6167 652e  x in skrt.image.
-00045340: 5f61 7865 735d 0a20 2020 2020 2020 2072  _axes].        r
-00045350: 6574 7572 6e20 5b6e 702e 6d65 616e 2865  eturn [np.mean(e
-00045360: 7829 2066 6f72 2065 7820 696e 2065 7874  x) for ex in ext
-00045370: 656e 7473 5d0a 0a20 2020 2064 6566 2066  ents]..    def f
-00045380: 696e 645f 6d6f 7374 5f70 6f70 756c 6174  ind_most_populat
-00045390: 6564 5f73 6c69 6365 2873 656c 662c 2076  ed_slice(self, v
-000453a0: 6965 773d 2278 2d79 2229 3a0a 2020 2020  iew="x-y"):.    
-000453b0: 2020 2020 2222 2246 696e 6420 7468 6520      """Find the 
-000453c0: 696e 6465 7820 6f66 2074 6865 2073 6c69  index of the sli
-000453d0: 6365 2077 6974 6820 7468 6520 6d6f 7374  ce with the most
-000453e0: 2052 4f49 7320 6f6e 2069 742e 2222 220a   ROIs on it.""".
-000453f0: 0a20 2020 2020 2020 2069 6e64 6963 6573  .        indices
-00045400: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
-00045410: 7220 726f 6920 696e 2073 656c 662e 6765  r roi in self.ge
-00045420: 745f 726f 6973 2869 676e 6f72 655f 656d  t_rois(ignore_em
-00045430: 7074 793d 5472 7565 293a 0a20 2020 2020  pty=True):.     
-00045440: 2020 2020 2020 2069 6e64 6963 6573 2e65         indices.e
-00045450: 7874 656e 6428 726f 692e 6765 745f 696e  xtend(roi.get_in
-00045460: 6469 6365 7328 7669 6577 2929 0a20 2020  dices(view)).   
-00045470: 2020 2020 2076 616c 732c 2063 6f75 6e74       vals, count
-00045480: 7320 3d20 6e70 2e75 6e69 7175 6528 696e  s = np.unique(in
-00045490: 6469 6365 732c 2072 6574 7572 6e5f 636f  dices, return_co
-000454a0: 756e 7473 3d54 7275 6529 0a20 2020 2020  unts=True).     
-000454b0: 2020 2072 6574 7572 6e20 7661 6c73 5b6e     return vals[n
-000454c0: 702e 6172 676d 6178 2863 6f75 6e74 7329  p.argmax(counts)
-000454d0: 5d0a 0a20 2020 2064 6566 2076 6965 7728  ]..    def view(
-000454e0: 7365 6c66 2c20 696e 636c 7564 655f 696d  self, include_im
-000454f0: 6167 653d 5472 7565 2c20 726f 6973 3d4e  age=True, rois=N
-00045500: 6f6e 652c 2076 6f78 656c 5f73 697a 653d  one, voxel_size=
-00045510: 5b31 2c20 315d 2c20 6275 6666 6572 3d35  [1, 1], buffer=5
-00045520: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00045530: 2020 2020 2022 2222 5669 6577 2074 6865       """View the
-00045540: 2053 7472 7563 7475 7265 5365 742e 0a0a   StructureSet...
-00045550: 2020 2020 2020 2020 2a2a 5061 7261 6d65          **Parame
-00045560: 7465 7273 3a2a 2a0a 2020 2020 2020 2020  ters:**.        
-00045570: 0a20 2020 2020 2020 2069 6e63 6c75 6465  .        include
-00045580: 5f69 6d61 6765 203a 2062 6f6f 6c2c 2064  _image : bool, d
-00045590: 6566 6175 6c74 3d54 7275 650a 2020 2020  efault=True.    
-000455a0: 2020 2020 2020 2020 4966 2054 7275 6520          If True 
-000455b0: 616e 6420 7468 6973 2053 7472 7563 7475  and this Structu
-000455c0: 7265 5365 7420 6861 7320 616e 2061 7373  reSet has an ass
-000455d0: 6f63 6961 7465 6420 696d 6167 6520 0a20  ociated image . 
-000455e0: 2020 2020 2020 2020 2020 2028 696e 2073             (in s
-000455f0: 656c 662e 696d 6167 6529 2c20 7468 6520  elf.image), the 
-00045600: 696d 6167 6520 7769 6c6c 2062 6520 6469  image will be di
-00045610: 7370 6c61 7965 6420 6265 6869 6e64 2074  splayed behind t
-00045620: 6865 2052 4f49 732e 0a0a 2020 2020 2020  he ROIs...      
-00045630: 2020 726f 6973 203a 2053 7472 7563 7475    rois : Structu
-00045640: 7265 5365 742f 6c69 7374 2c20 6465 6661  reSet/list, defa
-00045650: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
-00045660: 2020 2020 2041 6e79 206f 7468 6572 2052       Any other R
-00045670: 4f49 7320 6f72 2053 7472 7563 7475 7265  OIs or Structure
-00045680: 5365 7473 2074 6f20 696e 636c 7564 6520  Sets to include 
-00045690: 696e 2074 6865 2070 6c6f 742e 0a0a 2020  in the plot...  
-000456a0: 2020 2020 2020 766f 7865 6c5f 7369 7a65        voxel_size
-000456b0: 203a 206c 6973 742c 2064 6566 6175 6c74   : list, default
-000456c0: 3d5b 312c 2031 5d0a 2020 2020 2020 2020  =[1, 1].        
-000456d0: 2020 2020 4966 2074 6865 2053 7472 7563      If the Struc
-000456e0: 7475 7265 5365 7420 646f 6573 206e 6f74  tureSet does not
-000456f0: 2068 6176 6520 616e 2061 7373 6f63 6961   have an associa
-00045700: 7465 6420 696d 6167 6520 616e 6420 6861  ted image and ha
-00045710: 7320 524f 4973 200a 2020 2020 2020 2020  s ROIs .        
-00045720: 2020 2020 6465 7363 7269 6265 6420 6f6e      described on
-00045730: 6c79 2062 7920 636f 6e74 6f75 7273 2c20  ly by contours, 
-00045740: 7468 6973 2077 696c 6c20 6265 2074 6865  this will be the
-00045750: 2076 6f78 656c 2073 697a 6573 2075 7365   voxel sizes use
-00045760: 6420 696e 200a 2020 2020 2020 2020 2020  d in .          
-00045770: 2020 7468 6520 782d 7920 6469 7265 6374    the x-y direct
-00045780: 696f 6e20 7768 656e 2063 6f6e 7665 7274  ion when convert
-00045790: 696e 6720 524f 4973 2074 6f20 6d61 736b  ing ROIs to mask
-000457a0: 7320 6966 2061 206d 6173 6b20 706c 6f74  s if a mask plot
-000457b0: 200a 2020 2020 2020 2020 2020 2020 7479   .            ty
-000457c0: 7065 2069 7320 7365 6c65 6374 6564 2e0a  pe is selected..
-000457d0: 0a20 2020 2020 2020 2062 7566 6665 7220  .        buffer 
-000457e0: 3a20 696e 742c 2064 6566 6175 6c74 3d35  : int, default=5
-000457f0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00045800: 7468 6520 5374 7275 6374 7572 6553 6574  the StructureSet
-00045810: 2064 6f65 7320 6e6f 7420 6861 7665 2061   does not have a
-00045820: 6e20 6173 736f 6369 6174 6564 2069 6d61  n associated ima
-00045830: 6765 2061 6e64 2068 6173 2052 4f49 730a  ge and has ROIs.
-00045840: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-00045850: 7269 6265 6420 6f6e 6c79 2062 7920 636f  ribed only by co
-00045860: 6e74 6f75 7273 2c20 7468 6973 2077 696c  ntours, this wil
-00045870: 6c20 6265 2074 6865 206e 756d 6265 7220  l be the number 
-00045880: 6f66 2062 7566 6665 7220 766f 7865 6c73  of buffer voxels
-00045890: 200a 2020 2020 2020 2020 2020 2020 2869   .            (i
-000458a0: 2e65 2e20 7768 6974 6573 7061 6365 2920  .e. whitespace) 
-000458b0: 6469 7370 6c61 7965 6420 6172 6f75 6e64  displayed around
-000458c0: 2074 6865 2065 7874 656e 7420 6f66 2074   the extent of t
-000458d0: 6865 2052 4f49 732e 0a20 2020 2020 2020  he ROIs..       
-000458e0: 2022 2222 0a0a 2020 2020 2020 2020 6672   """..        fr
-000458f0: 6f6d 2073 6b72 742e 6265 7474 6572 5f76  om skrt.better_v
-00045900: 6965 7765 7220 696d 706f 7274 2042 6574  iewer import Bet
-00045910: 7465 7256 6965 7765 720a 2020 2020 2020  terViewer.      
-00045920: 2020 7365 6c66 2e6c 6f61 6428 290a 0a20    self.load().. 
-00045930: 2020 2020 2020 2023 2053 6574 2069 6e69         # Set ini
-00045940: 7469 616c 207a 6f6f 6d20 616d 6f75 6e74  tial zoom amount
-00045950: 2061 6e64 2063 656e 7472 650a 2020 2020   and centre.    
-00045960: 2020 2020 7365 6c66 2e72 6f69 735b 305d      self.rois[0]
-00045970: 2e6c 6f61 6428 290a 2020 2020 2020 2020  .load().        
-00045980: 6966 2073 656c 662e 696d 6167 6520 6973  if self.image is
-00045990: 206e 6f74 204e 6f6e 6520 616e 6420 6e6f   not None and no
-000459a0: 7420 7365 6c66 2e67 6574 5f72 6f69 7328  t self.get_rois(
-000459b0: 6967 6e6f 7265 5f65 6d70 7479 3d54 7275  ignore_empty=Tru
-000459c0: 6529 5b30 5d2e 636f 6e74 6f75 7273 5f6f  e)[0].contours_o
-000459d0: 6e6c 793a 0a20 2020 2020 2020 2020 2020  nly:.           
-000459e0: 2076 6965 7720 3d20 6b77 6172 6773 2e67   view = kwargs.g
-000459f0: 6574 2822 696e 6974 5f76 6965 7722 2c20  et("init_view", 
-00045a00: 2278 2d79 2229 0a20 2020 2020 2020 2020  "x-y").         
-00045a10: 2020 2061 7865 7320 3d20 736b 7274 2e69     axes = skrt.i
-00045a20: 6d61 6765 2e5f 706c 6f74 5f61 7865 735b  mage._plot_axes[
-00045a30: 7669 6577 5d0a 2020 2020 2020 2020 2020  view].          
-00045a40: 2020 6578 7465 6e74 7320 3d20 5b73 656c    extents = [sel
-00045a50: 662e 6765 745f 6c65 6e67 7468 2861 783d  f.get_length(ax=
-00045a60: 6178 2920 666f 7220 6178 2069 6e20 6178  ax) for ax in ax
-00045a70: 6573 5d0a 2020 2020 2020 2020 2020 2020  es].            
-00045a80: 696d 5f6c 696d 7320 3d20 5b73 656c 662e  im_lims = [self.
-00045a90: 696d 6167 652e 6765 745f 6c65 6e67 7468  image.get_length
-00045aa0: 2861 783d 6178 2920 666f 7220 6178 2069  (ax=ax) for ax i
-00045ab0: 6e20 6178 6573 5d0a 2020 2020 2020 2020  n axes].        
-00045ac0: 2020 2020 7a6f 6f6d 203d 206d 696e 285b      zoom = min([
-00045ad0: 696d 5f6c 696d 735b 695d 202f 2065 7874  im_lims[i] / ext
-00045ae0: 656e 7473 5b69 5d20 666f 7220 6920 696e  ents[i] for i in
-00045af0: 2072 616e 6765 2832 295d 2920 2a20 302e   range(2)]) * 0.
-00045b00: 380a 2020 2020 2020 2020 2020 2020 7a6f  8.            zo
-00045b10: 6f6d 5f63 656e 7472 6520 3d20 7365 6c66  om_centre = self
-00045b20: 2e67 6574 5f63 656e 7472 6528 290a 2020  .get_centre().  
-00045b30: 2020 2020 2020 2020 2020 6966 207a 6f6f            if zoo
-00045b40: 6d20 3e20 313a 0a20 2020 2020 2020 2020  m > 1:.         
-00045b50: 2020 2020 2020 206b 7761 7267 732e 7365         kwargs.se
-00045b60: 7464 6566 6175 6c74 2822 7a6f 6f6d 222c  tdefault("zoom",
-00045b70: 207a 6f6f 6d29 0a20 2020 2020 2020 2020   zoom).         
-00045b80: 2020 2020 2020 206b 7761 7267 732e 7365         kwargs.se
-00045b90: 7464 6566 6175 6c74 2822 7a6f 6f6d 5f63  tdefault("zoom_c
-00045ba0: 656e 7472 6522 2c20 7a6f 6f6d 5f63 656e  entre", zoom_cen
-00045bb0: 7472 6529 0a0a 2020 2020 2020 2020 2020  tre)..          
-00045bc0: 2020 2320 5365 7420 696e 6974 6961 6c20    # Set initial 
-00045bd0: 736c 6963 650a 2020 2020 2020 2020 2020  slice.          
-00045be0: 2020 6b77 6172 6773 2e73 6574 6465 6661    kwargs.setdefa
-00045bf0: 756c 7428 0a20 2020 2020 2020 2020 2020  ult(.           
-00045c00: 2020 2020 2022 696e 6974 5f73 6c69 6365       "init_slice
-00045c10: 222c 200a 2020 2020 2020 2020 2020 2020  ", .            
-00045c20: 2020 2020 7365 6c66 2e69 6d61 6765 2e69      self.image.i
-00045c30: 6478 5f74 6f5f 736c 6963 6528 7365 6c66  dx_to_slice(self
-00045c40: 2e66 696e 645f 6d6f 7374 5f70 6f70 756c  .find_most_popul
-00045c50: 6174 6564 5f73 6c69 6365 2876 6965 7729  ated_slice(view)
-00045c60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00045c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00045c80: 2020 2020 2020 2020 2020 736b 7274 2e69            skrt.i
-00045c90: 6d61 6765 2e5f 736c 6963 655f 6178 6573  mage._slice_axes
-00045ca0: 5b76 6965 775d 2929 0a0a 2020 2020 2020  [view]))..      
-00045cb0: 2020 2320 5669 6577 2077 6974 6820 696d    # View with im
-00045cc0: 6167 650a 2020 2020 2020 2020 6966 2069  age.        if i
-00045cd0: 6e63 6c75 6465 5f69 6d61 6765 2061 6e64  nclude_image and
-00045ce0: 2073 656c 662e 696d 6167 6520 6973 206e   self.image is n
-00045cf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00045d00: 2020 2020 2069 6620 726f 6973 2069 7320       if rois is 
-00045d10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00045d20: 2020 2020 2020 726f 6973 203d 2073 656c        rois = sel
-00045d30: 660a 2020 2020 2020 2020 2020 2020 656c  f.            el
-00045d40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00045d50: 2020 2020 6966 2073 6b72 742e 636f 7265      if skrt.core
-00045d60: 2e69 735f 6c69 7374 2872 6f69 7329 3a0a  .is_list(rois):.
-00045d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00045d80: 2020 2020 726f 6973 203d 205b 7365 6c66      rois = [self
-00045d90: 5d20 2b20 726f 6973 0a20 2020 2020 2020  ] + rois.       
-00045da0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00045db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00045dc0: 2020 2072 6f69 7320 3d20 5b73 656c 662c     rois = [self,
-00045dd0: 2072 6f69 735d 0a20 2020 2020 2020 2020   rois].         
-00045de0: 2020 2062 7620 3d20 4265 7474 6572 5669     bv = BetterVi
-00045df0: 6577 6572 2873 656c 662e 696d 6167 652c  ewer(self.image,
-00045e00: 2072 6f69 733d 726f 6973 2c20 2a2a 6b77   rois=rois, **kw
-00045e10: 6172 6773 290a 0a20 2020 2020 2020 2023  args)..        #
-00045e20: 2056 6965 7720 7769 7468 6f75 7420 696d   View without im
-00045e30: 6167 650a 2020 2020 2020 2020 656c 7365  age.        else
-00045e40: 3a0a 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00045e50: 7472 7563 7475 7265 5f73 6574 5f74 6d70  tructure_set_tmp
-00045e60: 203d 2073 656c 660a 0a20 2020 2020 2020   = self..       
-00045e70: 2020 2020 2023 204d 616b 6520 6475 6d6d       # Make dumm
-00045e80: 7920 696d 6167 650a 2020 2020 2020 2020  y image.        
-00045e90: 2020 2020 6966 2073 656c 662e 726f 6973      if self.rois
-00045ea0: 5b30 5d2e 636f 6e74 6f75 7273 5f6f 6e6c  [0].contours_onl
-00045eb0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00045ec0: 2020 2069 6d20 3d20 7365 6c66 2e67 6574     im = self.get
-00045ed0: 5f64 756d 6d79 5f69 6d61 6765 2862 7566  _dummy_image(buf
-00045ee0: 6665 723d 6275 6666 6572 2c20 0a20 2020  fer=buffer, .   
-00045ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00045f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00045f10: 2020 2020 2020 2076 6f78 656c 5f73 697a         voxel_siz
-00045f20: 653d 766f 7865 6c5f 7369 7a65 290a 2020  e=voxel_size).  
-00045f30: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00045f40: 7275 6374 7572 655f 7365 745f 746d 7020  ructure_set_tmp 
-00045f50: 3d20 7365 6c66 2e63 6c6f 6e65 280a 2020  = self.clone(.  
-00045f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00045f70: 2020 636f 7079 5f72 6f69 733d 5472 7565    copy_rois=True
-00045f80: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-00045f90: 2020 2020 2020 2063 6f70 795f 726f 695f         copy_roi_
-00045fa0: 6461 7461 3d46 616c 7365 0a20 2020 2020  data=False.     
-00045fb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00045fc0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00045fd0: 2072 6f69 2069 6e20 7374 7275 6374 7572   roi in structur
-00045fe0: 655f 7365 745f 746d 702e 726f 6973 3a0a  e_set_tmp.rois:.
+000452c0: 7365 6c66 2c20 2a2a 6b77 6172 6773 293a  self, **kwargs):
+000452d0: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+000452e0: 3344 2063 656e 7472 6520 6f66 2074 6865  3D centre of the
+000452f0: 2061 7265 6120 636f 7665 7265 6420 6279   area covered by
+00045300: 2052 4f49 732e 2222 220a 0a20 2020 2020   ROIs."""..     
+00045310: 2020 206b 7761 7267 732e 706f 7028 2261     kwargs.pop("a
+00045320: 7822 2c20 4e6f 6e65 290a 2020 2020 2020  x", None).      
+00045330: 2020 6578 7465 6e74 7320 3d20 5b73 656c    extents = [sel
+00045340: 662e 6765 745f 6578 7465 6e74 2861 783d  f.get_extent(ax=
+00045350: 6178 2c20 2a2a 6b77 6172 6773 2920 666f  ax, **kwargs) fo
+00045360: 7220 6178 2069 6e20 736b 7274 2e69 6d61  r ax in skrt.ima
+00045370: 6765 2e5f 6178 6573 5d0a 2020 2020 2020  ge._axes].      
+00045380: 2020 7265 7475 726e 205b 6e70 2e6d 6561    return [np.mea
+00045390: 6e28 6578 2920 666f 7220 6578 2069 6e20  n(ex) for ex in 
+000453a0: 6578 7465 6e74 735d 0a0a 2020 2020 6465  extents]..    de
+000453b0: 6620 6669 6e64 5f6d 6f73 745f 706f 7075  f find_most_popu
+000453c0: 6c61 7465 645f 736c 6963 6528 7365 6c66  lated_slice(self
+000453d0: 2c20 7669 6577 3d22 782d 7922 293a 0a20  , view="x-y"):. 
+000453e0: 2020 2020 2020 2022 2222 4669 6e64 2074         """Find t
+000453f0: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
+00045400: 736c 6963 6520 7769 7468 2074 6865 206d  slice with the m
+00045410: 6f73 7420 524f 4973 206f 6e20 6974 2e22  ost ROIs on it."
+00045420: 2222 0a0a 2020 2020 2020 2020 696e 6469  ""..        indi
+00045430: 6365 7320 3d20 5b5d 0a20 2020 2020 2020  ces = [].       
+00045440: 2066 6f72 2072 6f69 2069 6e20 7365 6c66   for roi in self
+00045450: 2e67 6574 5f72 6f69 7328 6967 6e6f 7265  .get_rois(ignore
+00045460: 5f65 6d70 7479 3d54 7275 6529 3a0a 2020  _empty=True):.  
+00045470: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+00045480: 732e 6578 7465 6e64 2872 6f69 2e67 6574  s.extend(roi.get
+00045490: 5f69 6e64 6963 6573 2876 6965 7729 290a  _indices(view)).
+000454a0: 2020 2020 2020 2020 7661 6c73 2c20 636f          vals, co
+000454b0: 756e 7473 203d 206e 702e 756e 6971 7565  unts = np.unique
+000454c0: 2869 6e64 6963 6573 2c20 7265 7475 726e  (indices, return
+000454d0: 5f63 6f75 6e74 733d 5472 7565 290a 2020  _counts=True).  
+000454e0: 2020 2020 2020 7265 7475 726e 2076 616c        return val
+000454f0: 735b 6e70 2e61 7267 6d61 7828 636f 756e  s[np.argmax(coun
+00045500: 7473 295d 0a0a 2020 2020 6465 6620 7669  ts)]..    def vi
+00045510: 6577 2873 656c 662c 2069 6e63 6c75 6465  ew(self, include
+00045520: 5f69 6d61 6765 3d54 7275 652c 2072 6f69  _image=True, roi
+00045530: 733d 4e6f 6e65 2c20 766f 7865 6c5f 7369  s=None, voxel_si
+00045540: 7a65 3d5b 312c 2031 5d2c 2062 7566 6665  ze=[1, 1], buffe
+00045550: 723d 352c 202a 2a6b 7761 7267 7329 3a0a  r=5, **kwargs):.
+00045560: 2020 2020 2020 2020 2222 2256 6965 7720          """View 
+00045570: 7468 6520 5374 7275 6374 7572 6553 6574  the StructureSet
+00045580: 2e0a 0a20 2020 2020 2020 202a 2a50 6172  ...        **Par
+00045590: 616d 6574 6572 733a 2a2a 0a20 2020 2020  ameters:**.     
+000455a0: 2020 200a 2020 2020 2020 2020 696e 636c     .        incl
+000455b0: 7564 655f 696d 6167 6520 3a20 626f 6f6c  ude_image : bool
+000455c0: 2c20 6465 6661 756c 743d 5472 7565 0a20  , default=True. 
+000455d0: 2020 2020 2020 2020 2020 2049 6620 5472             If Tr
+000455e0: 7565 2061 6e64 2074 6869 7320 5374 7275  ue and this Stru
+000455f0: 6374 7572 6553 6574 2068 6173 2061 6e20  ctureSet has an 
+00045600: 6173 736f 6369 6174 6564 2069 6d61 6765  associated image
+00045610: 200a 2020 2020 2020 2020 2020 2020 2869   .            (i
+00045620: 6e20 7365 6c66 2e69 6d61 6765 292c 2074  n self.image), t
+00045630: 6865 2069 6d61 6765 2077 696c 6c20 6265  he image will be
+00045640: 2064 6973 706c 6179 6564 2062 6568 696e   displayed behin
+00045650: 6420 7468 6520 524f 4973 2e0a 0a20 2020  d the ROIs...   
+00045660: 2020 2020 2072 6f69 7320 3a20 5374 7275       rois : Stru
+00045670: 6374 7572 6553 6574 2f6c 6973 742c 2064  ctureSet/list, d
+00045680: 6566 6175 6c74 3d4e 6f6e 650a 2020 2020  efault=None.    
+00045690: 2020 2020 2020 2020 416e 7920 6f74 6865          Any othe
+000456a0: 7220 524f 4973 206f 7220 5374 7275 6374  r ROIs or Struct
+000456b0: 7572 6553 6574 7320 746f 2069 6e63 6c75  ureSets to inclu
+000456c0: 6465 2069 6e20 7468 6520 706c 6f74 2e0a  de in the plot..
+000456d0: 0a20 2020 2020 2020 2076 6f78 656c 5f73  .        voxel_s
+000456e0: 697a 6520 3a20 6c69 7374 2c20 6465 6661  ize : list, defa
+000456f0: 756c 743d 5b31 2c20 315d 0a20 2020 2020  ult=[1, 1].     
+00045700: 2020 2020 2020 2049 6620 7468 6520 5374         If the St
+00045710: 7275 6374 7572 6553 6574 2064 6f65 7320  ructureSet does 
+00045720: 6e6f 7420 6861 7665 2061 6e20 6173 736f  not have an asso
+00045730: 6369 6174 6564 2069 6d61 6765 2061 6e64  ciated image and
+00045740: 2068 6173 2052 4f49 7320 0a20 2020 2020   has ROIs .     
+00045750: 2020 2020 2020 2064 6573 6372 6962 6564         described
+00045760: 206f 6e6c 7920 6279 2063 6f6e 746f 7572   only by contour
+00045770: 732c 2074 6869 7320 7769 6c6c 2062 6520  s, this will be 
+00045780: 7468 6520 766f 7865 6c20 7369 7a65 7320  the voxel sizes 
+00045790: 7573 6564 2069 6e20 0a20 2020 2020 2020  used in .       
+000457a0: 2020 2020 2074 6865 2078 2d79 2064 6972       the x-y dir
+000457b0: 6563 7469 6f6e 2077 6865 6e20 636f 6e76  ection when conv
+000457c0: 6572 7469 6e67 2052 4f49 7320 746f 206d  erting ROIs to m
+000457d0: 6173 6b73 2069 6620 6120 6d61 736b 2070  asks if a mask p
+000457e0: 6c6f 7420 0a20 2020 2020 2020 2020 2020  lot .           
+000457f0: 2074 7970 6520 6973 2073 656c 6563 7465   type is selecte
+00045800: 642e 0a0a 2020 2020 2020 2020 6275 6666  d...        buff
+00045810: 6572 203a 2069 6e74 2c20 6465 6661 756c  er : int, defaul
+00045820: 743d 350a 2020 2020 2020 2020 2020 2020  t=5.            
+00045830: 4966 2074 6865 2053 7472 7563 7475 7265  If the Structure
+00045840: 5365 7420 646f 6573 206e 6f74 2068 6176  Set does not hav
+00045850: 6520 616e 2061 7373 6f63 6961 7465 6420  e an associated 
+00045860: 696d 6167 6520 616e 6420 6861 7320 524f  image and has RO
+00045870: 4973 0a20 2020 2020 2020 2020 2020 2064  Is.            d
+00045880: 6573 6372 6962 6564 206f 6e6c 7920 6279  escribed only by
+00045890: 2063 6f6e 746f 7572 732c 2074 6869 7320   contours, this 
+000458a0: 7769 6c6c 2062 6520 7468 6520 6e75 6d62  will be the numb
+000458b0: 6572 206f 6620 6275 6666 6572 2076 6f78  er of buffer vox
+000458c0: 656c 7320 0a20 2020 2020 2020 2020 2020  els .           
+000458d0: 2028 692e 652e 2077 6869 7465 7370 6163   (i.e. whitespac
+000458e0: 6529 2064 6973 706c 6179 6564 2061 726f  e) displayed aro
+000458f0: 756e 6420 7468 6520 6578 7465 6e74 206f  und the extent o
+00045900: 6620 7468 6520 524f 4973 2e0a 2020 2020  f the ROIs..    
+00045910: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00045920: 2066 726f 6d20 736b 7274 2e62 6574 7465   from skrt.bette
+00045930: 725f 7669 6577 6572 2069 6d70 6f72 7420  r_viewer import 
+00045940: 4265 7474 6572 5669 6577 6572 0a20 2020  BetterViewer.   
+00045950: 2020 2020 2073 656c 662e 6c6f 6164 2829       self.load()
+00045960: 0a0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
+00045970: 696e 6974 6961 6c20 7a6f 6f6d 2061 6d6f  initial zoom amo
+00045980: 756e 7420 616e 6420 6365 6e74 7265 0a20  unt and centre. 
+00045990: 2020 2020 2020 2073 656c 662e 726f 6973         self.rois
+000459a0: 5b30 5d2e 6c6f 6164 2829 0a20 2020 2020  [0].load().     
+000459b0: 2020 2069 6620 7365 6c66 2e69 6d61 6765     if self.image
+000459c0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+000459d0: 206e 6f74 2073 656c 662e 6765 745f 726f   not self.get_ro
+000459e0: 6973 2869 676e 6f72 655f 656d 7074 793d  is(ignore_empty=
+000459f0: 5472 7565 295b 305d 2e63 6f6e 746f 7572  True)[0].contour
+00045a00: 735f 6f6e 6c79 3a0a 2020 2020 2020 2020  s_only:.        
+00045a10: 2020 2020 7669 6577 203d 206b 7761 7267      view = kwarg
+00045a20: 732e 6765 7428 2269 6e69 745f 7669 6577  s.get("init_view
+00045a30: 222c 2022 782d 7922 290a 2020 2020 2020  ", "x-y").      
+00045a40: 2020 2020 2020 6178 6573 203d 2073 6b72        axes = skr
+00045a50: 742e 696d 6167 652e 5f70 6c6f 745f 6178  t.image._plot_ax
+00045a60: 6573 5b76 6965 775d 0a20 2020 2020 2020  es[view].       
+00045a70: 2020 2020 2065 7874 656e 7473 203d 205b       extents = [
+00045a80: 7365 6c66 2e67 6574 5f6c 656e 6774 6828  self.get_length(
+00045a90: 6178 3d61 7829 2066 6f72 2061 7820 696e  ax=ax) for ax in
+00045aa0: 2061 7865 735d 0a20 2020 2020 2020 2020   axes].         
+00045ab0: 2020 2069 6d5f 6c69 6d73 203d 205b 7365     im_lims = [se
+00045ac0: 6c66 2e69 6d61 6765 2e67 6574 5f6c 656e  lf.image.get_len
+00045ad0: 6774 6828 6178 3d61 7829 2066 6f72 2061  gth(ax=ax) for a
+00045ae0: 7820 696e 2061 7865 735d 0a20 2020 2020  x in axes].     
+00045af0: 2020 2020 2020 207a 6f6f 6d20 3d20 6d69         zoom = mi
+00045b00: 6e28 5b69 6d5f 6c69 6d73 5b69 5d20 2f20  n([im_lims[i] / 
+00045b10: 6578 7465 6e74 735b 695d 2066 6f72 2069  extents[i] for i
+00045b20: 2069 6e20 7261 6e67 6528 3229 5d29 202a   in range(2)]) *
+00045b30: 2030 2e38 0a20 2020 2020 2020 2020 2020   0.8.           
+00045b40: 207a 6f6f 6d5f 6365 6e74 7265 203d 2073   zoom_centre = s
+00045b50: 656c 662e 6765 745f 6365 6e74 7265 2829  elf.get_centre()
+00045b60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00045b70: 7a6f 6f6d 203e 2031 3a0a 2020 2020 2020  zoom > 1:.      
+00045b80: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+00045b90: 2e73 6574 6465 6661 756c 7428 227a 6f6f  .setdefault("zoo
+00045ba0: 6d22 2c20 7a6f 6f6d 290a 2020 2020 2020  m", zoom).      
+00045bb0: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+00045bc0: 2e73 6574 6465 6661 756c 7428 227a 6f6f  .setdefault("zoo
+00045bd0: 6d5f 6365 6e74 7265 222c 207a 6f6f 6d5f  m_centre", zoom_
+00045be0: 6365 6e74 7265 290a 0a20 2020 2020 2020  centre)..       
+00045bf0: 2020 2020 2023 2053 6574 2069 6e69 7469       # Set initi
+00045c00: 616c 2073 6c69 6365 0a20 2020 2020 2020  al slice.       
+00045c10: 2020 2020 206b 7761 7267 732e 7365 7464       kwargs.setd
+00045c20: 6566 6175 6c74 280a 2020 2020 2020 2020  efault(.        
+00045c30: 2020 2020 2020 2020 2269 6e69 745f 736c          "init_sl
+00045c40: 6963 6522 2c20 0a20 2020 2020 2020 2020  ice", .         
+00045c50: 2020 2020 2020 2073 656c 662e 696d 6167         self.imag
+00045c60: 652e 6964 785f 746f 5f73 6c69 6365 2873  e.idx_to_slice(s
+00045c70: 656c 662e 6669 6e64 5f6d 6f73 745f 706f  elf.find_most_po
+00045c80: 7075 6c61 7465 645f 736c 6963 6528 7669  pulated_slice(vi
+00045c90: 6577 292c 0a20 2020 2020 2020 2020 2020  ew),.           
+00045ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00045cb0: 2020 2020 2020 2020 2020 2020 2073 6b72               skr
+00045cc0: 742e 696d 6167 652e 5f73 6c69 6365 5f61  t.image._slice_a
+00045cd0: 7865 735b 7669 6577 5d29 290a 0a20 2020  xes[view]))..   
+00045ce0: 2020 2020 2023 2056 6965 7720 7769 7468       # View with
+00045cf0: 2069 6d61 6765 0a20 2020 2020 2020 2069   image.        i
+00045d00: 6620 696e 636c 7564 655f 696d 6167 6520  f include_image 
+00045d10: 616e 6420 7365 6c66 2e69 6d61 6765 2069  and self.image i
+00045d20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00045d30: 2020 2020 2020 2020 6966 2072 6f69 7320          if rois 
+00045d40: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00045d50: 2020 2020 2020 2020 2072 6f69 7320 3d20           rois = 
+00045d60: 7365 6c66 0a20 2020 2020 2020 2020 2020  self.           
+00045d70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00045d80: 2020 2020 2020 2069 6620 736b 7274 2e63         if skrt.c
+00045d90: 6f72 652e 6973 5f6c 6973 7428 726f 6973  ore.is_list(rois
+00045da0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00045db0: 2020 2020 2020 2072 6f69 7320 3d20 5b73         rois = [s
+00045dc0: 656c 665d 202b 2072 6f69 730a 2020 2020  elf] + rois.    
+00045dd0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00045de0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00045df0: 2020 2020 2020 726f 6973 203d 205b 7365        rois = [se
+00045e00: 6c66 2c20 726f 6973 5d0a 2020 2020 2020  lf, rois].      
+00045e10: 2020 2020 2020 6276 203d 2042 6574 7465        bv = Bette
+00045e20: 7256 6965 7765 7228 7365 6c66 2e69 6d61  rViewer(self.ima
+00045e30: 6765 2c20 726f 6973 3d72 6f69 732c 202a  ge, rois=rois, *
+00045e40: 2a6b 7761 7267 7329 0a0a 2020 2020 2020  *kwargs)..      
+00045e50: 2020 2320 5669 6577 2077 6974 686f 7574    # View without
+00045e60: 2069 6d61 6765 0a20 2020 2020 2020 2065   image.        e
+00045e70: 6c73 653a 0a0a 2020 2020 2020 2020 2020  lse:..          
+00045e80: 2020 7374 7275 6374 7572 655f 7365 745f    structure_set_
+00045e90: 746d 7020 3d20 7365 6c66 0a0a 2020 2020  tmp = self..    
+00045ea0: 2020 2020 2020 2020 2320 4d61 6b65 2064          # Make d
+00045eb0: 756d 6d79 2069 6d61 6765 0a20 2020 2020  ummy image.     
+00045ec0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+00045ed0: 6f69 735b 305d 2e63 6f6e 746f 7572 735f  ois[0].contours_
+00045ee0: 6f6e 6c79 3a0a 2020 2020 2020 2020 2020  only:.          
+00045ef0: 2020 2020 2020 696d 203d 2073 656c 662e        im = self.
+00045f00: 6765 745f 6475 6d6d 795f 696d 6167 6528  get_dummy_image(
+00045f10: 6275 6666 6572 3d62 7566 6665 722c 200a  buffer=buffer, .
+00045f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00045f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00045f40: 2020 2020 2020 2020 2020 766f 7865 6c5f            voxel_
+00045f50: 7369 7a65 3d76 6f78 656c 5f73 697a 6529  size=voxel_size)
+00045f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00045f70: 2073 7472 7563 7475 7265 5f73 6574 5f74   structure_set_t
+00045f80: 6d70 203d 2073 656c 662e 636c 6f6e 6528  mp = self.clone(
+00045f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00045fa0: 2020 2020 2063 6f70 795f 726f 6973 3d54       copy_rois=T
+00045fb0: 7275 652c 200a 2020 2020 2020 2020 2020  rue, .          
+00045fc0: 2020 2020 2020 2020 2020 636f 7079 5f72            copy_r
+00045fd0: 6f69 5f64 6174 613d 4661 6c73 650a 2020  oi_data=False.  
+00045fe0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
 00045ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00046000: 2020 2020 6966 2072 6f69 2e63 6f6e 746f      if roi.conto
-00046010: 7572 735f 6f6e 6c79 3a0a 2020 2020 2020  urs_only:.      
-00046020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00046030: 2020 726f 692e 7365 745f 696d 6167 6528    roi.set_image(
-00046040: 696d 290a 2020 2020 2020 2020 2020 2020  im).            
-00046050: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00046060: 2020 2020 2020 696d 203d 2073 6b72 742e        im = skrt.
-00046070: 696d 6167 652e 496d 6167 6528 0a20 2020  image.Image(.   
-00046080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00046090: 206e 702e 6f6e 6573 2873 656c 662e 726f   np.ones(self.ro
-000460a0: 6973 5b30 5d2e 7368 6170 6529 202a 2031  is[0].shape) * 1
-000460b0: 6534 2c0a 2020 2020 2020 2020 2020 2020  e4,.            
-000460c0: 2020 2020 2020 2020 6166 6669 6e65 3d73          affine=s
-000460d0: 656c 662e 726f 6973 5b30 5d2e 6166 6669  elf.rois[0].affi
-000460e0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000460f0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00046100: 2020 2069 6620 726f 6973 2069 7320 4e6f     if rois is No
-00046110: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00046120: 2020 2020 726f 6973 203d 2073 7472 7563      rois = struc
-00046130: 7475 7265 5f73 6574 5f74 6d70 0a20 2020  ture_set_tmp.   
-00046140: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00046150: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00046160: 6620 736b 7274 2e63 6f72 652e 6973 5f6c  f skrt.core.is_l
-00046170: 6973 7428 726f 6973 293a 0a20 2020 2020  ist(rois):.     
-00046180: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00046190: 6f69 7320 3d20 5b73 7472 7563 7475 7265  ois = [structure
-000461a0: 5f73 6574 5f74 6d70 5d20 2b20 726f 6973  _set_tmp] + rois
-000461b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000461c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000461d0: 2020 2020 2020 2020 2020 2072 6f69 7320             rois 
-000461e0: 3d20 5b73 7472 7563 7475 7265 5f73 6574  = [structure_set
-000461f0: 5f74 6d70 2c20 726f 6973 5d0a 2020 2020  _tmp, rois].    
-00046200: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-00046210: 7368 6f77 225d 203d 2046 616c 7365 0a20  show"] = False. 
-00046220: 2020 2020 2020 2020 2020 2062 7620 3d20             bv = 
-00046230: 4265 7474 6572 5669 6577 6572 2869 6d2c  BetterViewer(im,
-00046240: 2072 6f69 733d 726f 6973 2c20 2a2a 6b77   rois=rois, **kw
-00046250: 6172 6773 290a 2020 2020 2020 2020 2020  args).          
-00046260: 2020 6276 2e6d 616b 655f 7569 286e 6f5f    bv.make_ui(no_
-00046270: 696e 7465 6e73 6974 793d 5472 7565 290a  intensity=True).
-00046280: 2020 2020 2020 2020 2020 2020 6276 2e73              bv.s
-00046290: 686f 7728 290a 0a20 2020 2020 2020 2072  how()..        r
-000462a0: 6574 7572 6e20 6276 0a0a 2020 2020 6465  eturn bv..    de
-000462b0: 6620 6765 745f 6578 7465 6e74 2873 656c  f get_extent(sel
-000462c0: 662c 202a 2a6b 7761 7267 7329 3a0a 2020  f, **kwargs):.  
-000462d0: 2020 2020 2020 2222 2247 6574 206d 696e        """Get min
-000462e0: 2061 6e64 206d 6178 2065 7874 656e 7420   and max extent 
-000462f0: 6f66 2061 6c6c 2052 4f49 7320 696e 2074  of all ROIs in t
-00046300: 6865 2053 7472 7563 7475 7265 5365 742e  he StructureSet.
-00046310: 2222 220a 0a20 2020 2020 2020 2061 6c6c  """..        all
-00046320: 5f65 7874 656e 7473 203d 205b 5d0a 2020  _extents = [].  
-00046330: 2020 2020 2020 666f 7220 726f 6920 696e        for roi in
-00046340: 2073 656c 662e 6765 745f 726f 6973 2869   self.get_rois(i
-00046350: 676e 6f72 655f 656d 7074 793d 5472 7565  gnore_empty=True
-00046360: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-00046370: 6c6c 5f65 7874 656e 7473 2e65 7874 656e  ll_extents.exten
-00046380: 6428 726f 692e 6765 745f 6578 7465 6e74  d(roi.get_extent
-00046390: 282a 2a6b 7761 7267 7329 290a 2020 2020  (**kwargs)).    
-000463a0: 2020 2020 7265 7475 726e 206d 696e 2861      return min(a
-000463b0: 6c6c 5f65 7874 656e 7473 292c 206d 6178  ll_extents), max
-000463c0: 2861 6c6c 5f65 7874 656e 7473 290a 0a20  (all_extents).. 
-000463d0: 2020 2064 6566 2067 6574 5f65 7874 656e     def get_exten
-000463e0: 7473 2873 656c 662c 2072 6f69 5f6e 616d  ts(self, roi_nam
-000463f0: 6573 3d4e 6f6e 652c 2062 7566 6665 723d  es=None, buffer=
-00046400: 4e6f 6e65 2c20 6275 6666 6572 5f75 6e69  None, buffer_uni
-00046410: 7473 3d22 6d6d 222c 0a20 2020 2020 2020  ts="mm",.       
-00046420: 2020 2020 206d 6574 686f 643d 4e6f 6e65       method=None
-00046430: 2c20 6f72 6967 696e 3d4e 6f6e 6529 3a0a  , origin=None):.
-00046440: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00046450: 2020 2020 4765 7420 6d69 6e69 6d75 6d20      Get minimum 
-00046460: 616e 6420 6d61 7869 6d75 6d20 6578 7465  and maximum exte
-00046470: 6e74 206f 6620 5374 7275 6374 7572 6553  nt of StructureS
-00046480: 6574 2052 4f49 732c 0a20 2020 2020 2020  et ROIs,.       
-00046490: 2069 6e20 6d6d 2061 6c6f 6e67 2061 6c6c   in mm along all
-000464a0: 2074 6872 6565 2061 7865 732c 2072 6574   three axes, ret
-000464b0: 7572 6e65 6420 696e 206f 7264 6572 205b  urned in order [
-000464c0: 782c 2079 2c20 7a5d 2e0a 2020 2020 2020  x, y, z]..      
-000464d0: 2020 4f70 7469 6f6e 616c 6c79 2061 7070    Optionally app
-000464e0: 6c79 2061 2062 7566 6665 7220 746f 2074  ly a buffer to t
-000464f0: 6865 2065 7874 656e 7473 2073 7563 6820  he extents such 
-00046500: 7468 6174 2074 6865 7920 636f 7665 720a  that they cover.
-00046510: 2020 2020 2020 2020 6d6f 7265 2074 6861          more tha
-00046520: 6e20 7468 6520 7265 6769 6f6e 206f 6620  n the region of 
-00046530: 7468 6520 524f 4973 2e0a 0a20 2020 2020  the ROIs...     
-00046540: 2020 202a 2a50 6172 616d 6574 6572 733a     **Parameters:
-00046550: 2a2a 0a0a 2020 2020 2020 2020 726f 695f  **..        roi_
-00046560: 6e61 6d65 7320 3a20 6c69 7374 2c20 6465  names : list, de
-00046570: 6661 756c 743d 4e6f 6e65 0a20 2020 2020  fault=None.     
-00046580: 2020 2020 2020 204c 6973 7420 6f66 206e         List of n
-00046590: 616d 6573 206f 6620 524f 4973 2074 6f20  ames of ROIs to 
-000465a0: 6265 2063 6f6e 7369 6465 7265 642e 2020  be considered.  
-000465b0: 4966 204e 6f6e 652c 2061 6c6c 206f 6620  If None, all of 
-000465c0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-000465d0: 7374 7275 6374 7572 6520 7365 7427 7320  structure set's 
-000465e0: 524f 4973 2061 7265 2063 6f6e 7369 6465  ROIs are conside
-000465f0: 7265 642e 0a0a 2020 2020 2020 2020 6275  red...        bu
-00046600: 6666 6572 203a 2066 6c6f 6174 2c20 6465  ffer : float, de
-00046610: 6661 756c 743d 4e6f 6e65 0a20 2020 2020  fault=None.     
-00046620: 2020 2020 2020 204f 7074 696f 6e61 6c20         Optional 
-00046630: 6275 6666 6572 2074 6f20 6164 6420 746f  buffer to add to
-00046640: 2074 6865 2065 7874 656e 7473 2e20 556e   the extents. Un
-00046650: 6974 7320 7365 7420 6279 2060 6275 6666  its set by `buff
-00046660: 6572 5f75 6e69 7473 602e 0a0a 2020 2020  er_units`...    
-00046670: 2020 2020 6275 6666 6572 5f75 6e69 7473      buffer_units
-00046680: 203a 2073 7472 2c20 6465 6661 756c 743d   : str, default=
-00046690: 226d 6d22 0a20 2020 2020 2020 2020 2020  "mm".           
-000466a0: 2055 6e69 7473 2066 6f72 2062 7566 6665   Units for buffe
-000466b0: 722c 2069 6620 7573 696e 672e 2043 616e  r, if using. Can
-000466c0: 2062 6520 226d 6d22 2c20 2276 6f78 656c   be "mm", "voxel
-000466d0: 7322 2c20 6f72 2022 6672 6163 2220 2877  s", or "frac" (w
-000466e0: 6869 6368 0a20 2020 2020 2020 2020 2020  hich.           
-000466f0: 2061 7070 6c69 6573 2062 7566 6665 7220   applies buffer 
-00046700: 6173 2061 2066 7261 6374 696f 6e20 6f66  as a fraction of
-00046710: 2074 6f74 616c 206c 656e 6774 6820 696e   total length in
-00046720: 2065 6163 6820 6469 6d65 6e73 696f 6e29   each dimension)
-00046730: 2e0a 0a20 2020 2020 2020 206d 6574 686f  ...        metho
-00046740: 6420 3a20 7374 722c 2064 6566 6175 6c74  d : str, default
-00046750: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
-00046760: 2020 4d65 7468 6f64 2074 6f20 7573 6520    Method to use 
-00046770: 666f 7220 6578 7465 6e74 2063 616c 6375  for extent calcu
-00046780: 6c61 7469 6f6e 2e20 4361 6e20 6265 3a20  lation. Can be: 
-00046790: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000467a0: 2020 2a20 2263 6f6e 746f 7572 223a 2067    * "contour": g
-000467b0: 6574 2065 7874 656e 7420 6672 6f6d 206d  et extent from m
-000467c0: 696e 2f6d 6178 2070 6f73 6974 696f 6e73  in/max positions
-000467d0: 206f 6620 636f 6e74 6f75 7228 7329 2e0a   of contour(s)..
-000467e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000467f0: 2a20 226d 6173 6b22 3a20 6765 7420 6578  * "mask": get ex
-00046800: 7465 6e74 2066 726f 6d20 6d69 6e2f 6d61  tent from min/ma
-00046810: 7820 706f 7369 7469 6f6e 7320 6f66 2076  x positions of v
-00046820: 6f78 656c 7320 696e 2074 6865 200a 2020  oxels in the .  
-00046830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00046840: 6269 6e61 7279 206d 6173 6b2e 0a20 2020  binary mask..   
-00046850: 2020 2020 2020 2020 2020 2020 202a 204e               * N
-00046860: 6f6e 653a 2075 7365 2074 6865 206d 6574  one: use the met
-00046870: 686f 6420 7365 7420 696e 2073 656c 662e  hod set in self.
-00046880: 6465 6661 756c 745f 6765 6f6d 5f6d 6574  default_geom_met
-00046890: 686f 642e 0a0a 2020 2020 2020 2020 6f72  hod...        or
-000468a0: 6967 696e 203a 2074 7570 6c65 2c20 6465  igin : tuple, de
-000468b0: 6661 756c 743d 4e6f 6e65 0a20 2020 2020  fault=None.     
-000468c0: 2020 2020 2020 2054 7570 6c65 2073 7065         Tuple spe
-000468d0: 6369 6679 696e 6720 7468 6520 2878 2c20  cifying the (x, 
-000468e0: 792c 207a 2920 636f 6f72 6469 6e61 7465  y, z) coordinate
-000468f0: 7320 6f66 2074 6865 2070 6f69 6e74 0a20  s of the point. 
-00046900: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00046910: 7265 7370 6563 7420 746f 2077 6869 6368  respect to which
-00046920: 2065 7874 656e 7473 2061 7265 2074 6f20   extents are to 
-00046930: 6265 2064 6574 6572 6d69 6e65 642e 0a20  be determined.. 
-00046940: 2020 2020 2020 2020 2020 2049 6620 4e6f             If No
-00046950: 6e65 2c20 7468 656e 2028 302c 2030 2c20  ne, then (0, 0, 
-00046960: 3029 2069 7320 7573 6564 2e0a 2020 2020  0) is used..    
-00046970: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00046980: 7265 7475 726e 2073 656c 662e 636f 6d62  return self.comb
-00046990: 696e 655f 726f 6973 2872 6f69 5f6e 616d  ine_rois(roi_nam
-000469a0: 6573 292e 6765 745f 6578 7465 6e74 7328  es).get_extents(
-000469b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000469c0: 2062 7566 6665 722c 2062 7566 6665 725f   buffer, buffer_
-000469d0: 756e 6974 732c 206d 6574 686f 642c 206f  units, method, o
-000469e0: 7269 6769 6e29 0a0a 2020 2020 6465 6620  rigin)..    def 
-000469f0: 6765 745f 6372 6f70 5f6c 696d 6974 7328  get_crop_limits(
-00046a00: 7365 6c66 2c20 726f 695f 6e61 6d65 733d  self, roi_names=
-00046a10: 4e6f 6e65 2c20 6372 6f70 5f6d 6172 6769  None, crop_margi
-00046a20: 6e73 3d4e 6f6e 652c 206d 6574 686f 643d  ns=None, method=
-00046a30: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
-00046a40: 2222 0a20 2020 2020 2020 2047 6574 2063  "".        Get c
-00046a50: 726f 7020 6c69 6d69 7473 2063 6f72 7265  rop limits corre
-00046a60: 7370 6f6e 6469 6e67 2074 6f20 5374 7275  sponding to Stru
-00046a70: 6374 7572 6553 6574 2052 4f49 2065 7874  ctureSet ROI ext
-00046a80: 656e 7473 2070 6c75 7320 6d61 7267 696e  ents plus margin
-00046a90: 732e 0a0a 2020 2020 2020 2020 5468 6520  s...        The 
-00046aa0: 7475 706c 6573 206f 6620 6c69 6d69 7473  tuples of limits
-00046ab0: 2072 6574 7572 6e65 642c 2069 6e20 7468   returned, in th
-00046ac0: 6520 6f72 6465 7220 2878 2c20 792c 207a  e order (x, y, z
-00046ad0: 2920 6361 6e0a 2020 2020 2020 2020 6265  ) can.        be
-00046ae0: 2075 7365 642c 2066 6f72 2065 7861 6d70   used, for examp
-00046af0: 6c65 2c20 6173 2069 6e70 7574 7320 746f  le, as inputs to
-00046b00: 2073 6b72 742e 696d 6167 652e 496d 6167   skrt.image.Imag
-00046b10: 652e 6372 6f70 2829 2e0a 0a20 2020 2020  e.crop()...     
-00046b20: 2020 2054 6869 7320 6d65 7468 6f64 2069     This method i
-00046b30: 7320 7369 6d69 6c61 7220 746f 2074 6865  s similar to the
-00046b40: 206d 6574 686f 6420 6765 745f 6578 7465   method get_exte
-00046b50: 6e74 7328 292c 2062 7574 2061 6c6c 6f77  nts(), but allow
-00046b60: 730a 2020 2020 2020 2020 6469 6666 6572  s.        differ
-00046b70: 656e 7420 6d61 7267 696e 7320 6f6e 2065  ent margins on e
-00046b80: 6163 6820 7369 6465 206f 6620 7468 6520  ach side of the 
-00046b90: 5374 7275 6374 7572 6553 6574 2e0a 0a20  StructureSet... 
-00046ba0: 2020 2020 2020 202a 2a50 6172 616d 6574         **Paramet
-00046bb0: 6572 733a 2a2a 0a0a 2020 2020 2020 2020  ers:**..        
-00046bc0: 726f 695f 6e61 6d65 7320 3a20 6c69 7374  roi_names : list
-00046bd0: 2c20 6465 6661 756c 743d 4e6f 6e65 0a20  , default=None. 
-00046be0: 2020 2020 2020 2020 2020 204c 6973 7420             List 
-00046bf0: 6f66 206e 616d 6573 206f 6620 524f 4973  of names of ROIs
-00046c00: 2074 6f20 6265 2063 6f6e 7369 6465 7265   to be considere
-00046c10: 642e 2020 4966 204e 6f6e 652c 2061 6c6c  d.  If None, all
-00046c20: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-00046c30: 2020 2020 7374 7275 6374 7572 6520 7365      structure se
-00046c40: 7427 7320 524f 4973 2061 7265 2063 6f6e  t's ROIs are con
-00046c50: 7369 6465 7265 642e 0a0a 2020 2020 2020  sidered...      
-00046c60: 2020 6372 6f70 5f6d 6172 6769 6e73 203a    crop_margins :
-00046c70: 2066 6c6f 6174 2f74 7570 6c65 2c20 6465   float/tuple, de
-00046c80: 6661 756c 743d 4e6f 6e65 0a20 2020 2020  fault=None.     
-00046c90: 2020 2020 2020 2046 6c6f 6174 206f 7220         Float or 
-00046ca0: 7468 7265 652d 656c 656d 656e 7420 7475  three-element tu
-00046cb0: 706c 6520 7370 6563 6966 7969 6e67 2074  ple specifying t
-00046cc0: 6865 206d 6172 6769 6e73 2c20 696e 206d  he margins, in m
-00046cd0: 6d2c 0a20 2020 2020 2020 2020 2020 2074  m,.            t
-00046ce0: 6f20 6265 2061 6464 6564 2074 6f20 5374  o be added to St
-00046cf0: 7275 6374 7572 6553 6574 2065 7874 656e  ructureSet exten
-00046d00: 7473 2e20 2049 6620 6120 666c 6f61 742c  ts.  If a float,
-00046d10: 206d 696e 7573 2061 6e64 2070 6c75 7320   minus and plus 
-00046d20: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00046d30: 7661 6c75 6520 7370 6563 6966 6965 6420  value specified 
-00046d40: 6172 6520 6164 6465 6420 746f 206c 6f77  are added to low
-00046d50: 6572 2061 6e64 2075 7070 6572 2065 7874  er and upper ext
-00046d60: 656e 7473 2072 6573 7065 6374 6976 656c  ents respectivel
-00046d70: 790a 2020 2020 2020 2020 2020 2020 616c  y.            al
-00046d80: 6f6e 6720 6561 6368 2061 7869 732e 2020  ong each axis.  
-00046d90: 4966 2061 2074 6872 6565 2d65 6c65 6d65  If a three-eleme
-00046da0: 6e74 2074 7570 6c65 2c20 656c 656d 656e  nt tuple, elemen
-00046db0: 7473 2061 7265 0a20 2020 2020 2020 2020  ts are.         
-00046dc0: 2020 2074 616b 656e 2074 6f20 7370 6563     taken to spec
-00046dd0: 6966 7920 6d61 7267 696e 7320 696e 2074  ify margins in t
-00046de0: 6865 206f 7264 6572 2028 782c 2079 2c20  he order (x, y, 
-00046df0: 7a29 2e20 2045 6c65 6d65 6e74 730a 2020  z).  Elements.  
-00046e00: 2020 2020 2020 2020 2020 6361 6e20 6265            can be
-00046e10: 2065 6974 6865 7220 666c 6f61 7473 2028   either floats (
-00046e20: 6d69 6e75 7320 616e 6420 706c 7573 2074  minus and plus t
-00046e30: 6865 2076 616c 7565 2061 6464 6564 2072  he value added r
-00046e40: 6573 7065 6374 6976 656c 790a 2020 2020  espectively.    
-00046e50: 2020 2020 2020 2020 746f 206c 6f77 6572          to lower
-00046e60: 2061 6e64 2075 7070 6572 2065 7874 656e   and upper exten
-00046e70: 7473 2920 6f72 2074 776f 2d65 6c65 6d65  ts) or two-eleme
-00046e80: 6e74 2074 7570 6c65 7320 2865 6c65 6d65  nt tuples (eleme
-00046e90: 6e74 7320 3020 616e 6420 310a 2020 2020  nts 0 and 1.    
-00046ea0: 2020 2020 2020 2020 6164 6465 6420 7265          added re
-00046eb0: 7370 6563 7469 7665 6c79 2074 6f20 6c6f  spectively to lo
-00046ec0: 7765 7220 616e 6420 7570 7065 7220 6578  wer and upper ex
-00046ed0: 7465 6e74 7329 2e0a 0a20 2020 2020 2020  tents)...       
-00046ee0: 206d 6574 686f 6420 3a20 7374 722c 2064   method : str, d
-00046ef0: 6566 6175 6c74 3d4e 6f6e 650a 2020 2020  efault=None.    
-00046f00: 2020 2020 2020 2020 4d65 7468 6f64 2074          Method t
-00046f10: 6f20 7573 6520 666f 7220 6578 7465 6e74  o use for extent
-00046f20: 2063 616c 6375 6c61 7469 6f6e 2e20 4361   calculation. Ca
-00046f30: 6e20 6265 3a0a 0a20 2020 2020 2020 2020  n be:..         
-00046f40: 2020 2020 2020 202a 2022 636f 6e74 6f75         * "contou
-00046f50: 7222 3a20 6765 7420 6578 7465 6e74 2066  r": get extent f
-00046f60: 726f 6d20 6d69 6e2f 6d61 7820 706f 7369  rom min/max posi
-00046f70: 7469 6f6e 7320 6f66 2063 6f6e 746f 7572  tions of contour
-00046f80: 2873 292e 0a20 2020 2020 2020 2020 2020  (s)..           
-00046f90: 2020 2020 202a 2022 6d61 736b 223a 2067       * "mask": g
-00046fa0: 6574 2065 7874 656e 7420 6672 6f6d 206d  et extent from m
-00046fb0: 696e 2f6d 6178 2070 6f73 6974 696f 6e73  in/max positions
-00046fc0: 206f 6620 766f 7865 6c73 2069 6e20 7468   of voxels in th
-00046fd0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00046fe0: 2020 2020 6269 6e61 7279 206d 6173 6b2e      binary mask.
-00046ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00047000: 202a 204e 6f6e 653a 2075 7365 2074 6865   * None: use the
-00047010: 206d 6574 686f 6420 7365 7420 696e 2073   method set in s
-00047020: 656c 662e 6465 6661 756c 745f 6765 6f6d  elf.default_geom
-00047030: 5f6d 6574 686f 642e 0a20 2020 2020 2020  _method..       
-00047040: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-00047050: 7572 6e20 7365 6c66 2e63 6f6d 6269 6e65  urn self.combine
-00047060: 5f72 6f69 7328 726f 695f 6e61 6d65 7329  _rois(roi_names)
-00047070: 2e67 6574 5f63 726f 705f 6c69 6d69 7473  .get_crop_limits
-00047080: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00047090: 2020 6372 6f70 5f6d 6172 6769 6e73 2c20    crop_margins, 
-000470a0: 6d65 7468 6f64 290a 0a20 2020 2064 6566  method)..    def
-000470b0: 2067 6574 5f62 626f 785f 6365 6e74 7265   get_bbox_centre
-000470c0: 5f61 6e64 5f77 6964 7468 7328 7365 6c66  _and_widths(self
-000470d0: 2c0a 2020 2020 2020 2020 2020 2020 726f  ,.            ro
-000470e0: 695f 6e61 6d65 733d 4e6f 6e65 2c20 6275  i_names=None, bu
-000470f0: 6666 6572 3d4e 6f6e 652c 2062 7566 6665  ffer=None, buffe
-00047100: 725f 756e 6974 733d 226d 6d22 2c20 6d65  r_units="mm", me
-00047110: 7468 6f64 3d4e 6f6e 6529 3a0a 2020 2020  thod=None):.    
-00047120: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00047130: 4765 7420 6365 6e74 7265 2061 6e64 2077  Get centre and w
-00047140: 6964 7468 7320 696e 206d 6d20 616c 6f6e  idths in mm alon
-00047150: 6720 616c 6c20 7468 7265 6520 6178 6573  g all three axes
-00047160: 206f 6620 6120 626f 756e 6469 6e67 2062   of a bounding b
-00047170: 6f78 0a20 2020 2020 2020 2065 6e63 6c6f  ox.        enclo
-00047180: 7369 6e67 2053 7472 7563 7475 7265 5365  sing StructureSe
-00047190: 7420 524f 4973 2061 6e64 206f 7074 696f  t ROIs and optio
-000471a0: 6e61 6c20 6275 6666 6572 2e20 2043 656e  nal buffer.  Cen
-000471b0: 7472 650a 2020 2020 2020 2020 616e 6420  tre.        and 
-000471c0: 7769 6474 6873 2061 7265 2072 6574 7572  widths are retur
-000471d0: 6e65 6420 6173 2061 2074 7570 6c65 2028  ned as a tuple (
-000471e0: 5b78 2c20 792c 207a 5d2c 205b 6478 2c20  [x, y, z], [dx, 
-000471f0: 6479 2c20 647a 5d29 2e0a 0a20 2020 2020  dy, dz])...     
-00047200: 2020 204d 6574 686f 6420 7061 7261 6d65     Method parame
-00047210: 7465 7273 2061 7265 2070 6173 7365 6420  ters are passed 
-00047220: 746f 0a20 2020 2020 2020 2073 6b72 742e  to.        skrt.
-00047230: 7374 7275 6374 7572 6573 2e53 7472 7563  structures.Struc
-00047240: 7475 7265 5365 742e 6765 745f 6578 7465  tureSet.get_exte
-00047250: 6e74 7328 2920 746f 206f 6274 6169 6e20  nts() to obtain 
-00047260: 5374 7275 6374 7572 6553 6574 0a20 2020  StructureSet.   
-00047270: 2020 2020 2065 7874 656e 7473 2e20 2046       extents.  F
-00047280: 6f72 2070 6172 616d 6574 6572 2065 7870  or parameter exp
-00047290: 6c61 6e61 7469 6f6e 732c 2073 6565 0a20  lanations, see. 
-000472a0: 2020 2020 2020 2073 6b72 742e 7374 7275         skrt.stru
-000472b0: 6374 7572 6573 2e53 7472 7563 7475 7265  ctures.Structure
-000472c0: 5365 742e 6765 745f 6578 7465 6e74 7328  Set.get_extents(
-000472d0: 2920 646f 6375 6d65 6e74 6174 696f 6e2e  ) documentation.
-000472e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000472f0: 2020 2020 2065 7874 656e 7473 203d 2073       extents = s
-00047300: 656c 662e 6765 745f 6578 7465 6e74 7328  elf.get_extents(
-00047310: 726f 695f 6e61 6d65 732c 2062 7566 6665  roi_names, buffe
-00047320: 722c 2062 7566 6665 725f 756e 6974 732c  r, buffer_units,
-00047330: 206d 6574 686f 6429 200a 2020 2020 2020   method) .      
-00047340: 2020 6365 6e74 7265 203d 205b 302e 3520    centre = [0.5 
-00047350: 2a20 2865 7874 656e 745b 305d 202b 2065  * (extent[0] + e
-00047360: 7874 656e 745b 315d 2920 666f 7220 6578  xtent[1]) for ex
-00047370: 7465 6e74 2069 6e20 6578 7465 6e74 735d  tent in extents]
-00047380: 0a20 2020 2020 2020 2077 6964 7468 7320  .        widths 
-00047390: 3d20 5b28 6578 7465 6e74 5b31 5d20 2d20  = [(extent[1] - 
-000473a0: 6578 7465 6e74 5b30 5d29 2066 6f72 2065  extent[0]) for e
-000473b0: 7874 656e 7420 696e 2065 7874 656e 7473  xtent in extents
-000473c0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-000473d0: 2028 6365 6e74 7265 2c20 7769 6474 6873   (centre, widths
-000473e0: 290a 0a20 2020 2064 6566 2067 6574 5f64  )..    def get_d
-000473f0: 756d 6d79 5f69 6d61 6765 2873 656c 662c  ummy_image(self,
-00047400: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00047410: 2020 2020 2222 224d 616b 6520 6120 6475      """Make a du
-00047420: 6d6d 7920 696d 6167 6520 7468 6174 2063  mmy image that c
-00047430: 6f76 6572 7320 7468 6520 6172 6561 2073  overs the area s
-00047440: 7061 6e6e 6564 2062 7920 616c 6c20 524f  panned by all RO
-00047450: 4973 2069 6e20 7468 6973 0a20 2020 2020  Is in this.     
-00047460: 2020 2053 7472 7563 7475 7265 5365 742e     StructureSet.
-00047470: 2052 6574 7572 6e73 2061 6e20 496d 6167   Returns an Imag
-00047480: 6520 6f62 6a65 6374 2e0a 0a20 2020 2020  e object...     
-00047490: 2020 202a 2a50 6172 616d 6574 6572 733a     **Parameters:
-000474a0: 2a2a 0a20 2020 2020 2020 200a 2020 2020  **.        .    
-000474b0: 2020 2020 766f 7865 6c5f 7369 7a65 203a      voxel_size :
-000474c0: 206c 6973 742c 2064 6566 6175 6c74 3d4e   list, default=N
-000474d0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-000474e0: 566f 7865 6c20 7369 7a65 2069 6e20 6d6d  Voxel size in mm
-000474f0: 2069 6e20 7468 6520 6475 6d6d 7920 696d   in the dummy im
-00047500: 6167 6520 696e 2074 6865 2078 2d79 2070  age in the x-y p
-00047510: 6c61 6e65 2c20 6769 7665 6e20 6173 200a  lane, given as .
-00047520: 2020 2020 2020 2020 2020 2020 5b76 782c              [vx,
-00047530: 2076 795d 2e20 4966 203c 7368 6170 653e   vy]. If <shape>
-00047540: 2061 6e64 203c 766f 7865 6c5f 7369 7a65   and <voxel_size
-00047550: 3e20 6172 6520 626f 7468 204e 6f6e 652c  > are both None,
-00047560: 2076 6f78 656c 2073 697a 6573 206f 660a   voxel sizes of.
-00047570: 2020 2020 2020 2020 2020 2020 5b31 2c20              [1, 
-00047580: 315d 2077 696c 6c20 6265 2075 7365 6420  1] will be used 
-00047590: 6279 2064 6566 6175 6c74 2e20 5468 6520  by default. The 
-000475a0: 766f 7865 6c20 7369 7a65 2069 6e20 7468  voxel size in th
-000475b0: 6520 7a20 6469 7265 6374 696f 6e20 0a20  e z direction . 
-000475c0: 2020 2020 2020 2020 2020 2069 7320 6465             is de
-000475d0: 6669 6e65 6420 6279 203c 736c 6963 655f  fined by <slice_
-000475e0: 7468 6963 6b6e 6573 733e 2e0a 0a20 2020  thickness>...   
-000475f0: 2020 2020 2073 6861 7065 203a 206c 6973       shape : lis
-00047600: 742c 2064 6566 6175 6c74 3d4e 6f6e 650a  t, default=None.
-00047610: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
-00047620: 6572 206f 6620 766f 7865 6c73 2069 6e20  er of voxels in 
-00047630: 7468 6520 6475 6d6d 7920 696d 6167 6520  the dummy image 
-00047640: 696e 2074 6865 2078 2d79 2070 6c61 6e65  in the x-y plane
-00047650: 2c20 6769 7665 6e20 6173 0a20 2020 2020  , given as.     
-00047660: 2020 2020 2020 205b 6e78 2c20 6e79 5d2e         [nx, ny].
-00047670: 204f 6e6c 7920 7573 6564 2069 6620 3c76   Only used if <v
-00047680: 6f78 656c 5f73 697a 653e 2069 7320 4e6f  oxel_size> is No
-00047690: 6e65 2e20 0a20 2020 2020 2020 2020 2020  ne. .           
-000476a0: 2054 6865 206e 756d 6265 7220 6f66 2076   The number of v
-000476b0: 6f78 656c 7320 696e 2074 6865 207a 2064  oxels in the z d
-000476c0: 6972 6563 7469 6f6e 2077 696c 6c20 6265  irection will be
-000476d0: 2074 616b 656e 2066 726f 6d20 7468 6520   taken from the 
-000476e0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
-000476f0: 6265 7220 6f66 2073 6c69 6365 7320 696e  ber of slices in
-00047700: 2074 6865 2078 2d79 2063 6f6e 746f 7572   the x-y contour
-00047710: 7320 6469 6374 696f 6e61 7279 2e0a 0a20  s dictionary... 
-00047720: 2020 2020 2020 2066 696c 6c5f 7661 6c20         fill_val 
-00047730: 3a20 696e 742f 666c 6f61 742c 2064 6566  : int/float, def
-00047740: 6175 6c74 3d31 6534 0a20 2020 2020 2020  ault=1e4.       
-00047750: 2020 2020 2056 616c 7565 2077 6974 6820       Value with 
-00047760: 7768 6963 6820 7468 6520 766f 7865 6c73  which the voxels
-00047770: 2069 6e20 7468 6520 6475 6d6d 7920 696d   in the dummy im
-00047780: 6167 6520 7368 6f75 6c64 2062 6520 6669  age should be fi
-00047790: 6c6c 6564 2e20 0a0a 2020 2020 2020 2020  lled. ..        
-000477a0: 6275 6666 6572 203a 2069 6e74 2c20 6465  buffer : int, de
-000477b0: 6661 756c 743d 310a 2020 2020 2020 2020  fault=1.        
-000477c0: 2020 2020 4e75 6d62 6572 206f 6620 656d      Number of em
-000477d0: 7074 7920 6275 6666 6572 2076 6f78 656c  pty buffer voxel
-000477e0: 7320 746f 2061 6464 206f 7574 7369 6465  s to add outside
-000477f0: 2074 6865 2052 4f49 2069 6e20 6561 6368   the ROI in each
-00047800: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-00047810: 6563 7469 6f6e 2e0a 0a20 2020 2020 2020  ection...       
-00047820: 2073 6c69 6365 5f74 6869 636b 6e65 7373   slice_thickness
-00047830: 203a 2066 6c6f 6174 2c20 6465 6661 756c   : float, defaul
-00047840: 743d 4e6f 6e65 0a20 2020 2020 2020 2020  t=None.         
-00047850: 2020 2056 6f78 656c 2073 697a 6520 696e     Voxel size in
-00047860: 206d 6d20 696e 2074 6865 2064 756d 6d79   mm in the dummy
-00047870: 2069 6d61 6765 2069 6e20 7468 6520 7a20   image in the z 
-00047880: 6469 7265 6374 696f 6e2e 2020 4966 204e  direction.  If N
-00047890: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-000478a0: 2074 6865 2076 616c 7565 2075 7365 6420   the value used 
-000478b0: 6973 2074 6865 206d 696e 696d 756d 2064  is the minimum d
-000478c0: 6973 7461 6e63 6520 6265 7477 6565 6e20  istance between 
-000478d0: 736c 6963 6520 706f 7369 7469 6f6e 730a  slice positions.
-000478e0: 2020 2020 2020 2020 2020 2020 696e 2074              in t
-000478f0: 6865 2078 2d79 2063 6f6e 746f 7572 7320  he x-y contours 
-00047900: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
-00047910: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00047920: 6578 7465 6e74 7320 3d20 5b73 656c 662e  extents = [self.
-00047930: 6765 745f 6578 7465 6e74 2861 783d 6178  get_extent(ax=ax
-00047940: 2920 666f 7220 6178 2069 6e20 736b 7274  ) for ax in skrt
-00047950: 2e69 6d61 6765 2e5f 6178 6573 5d0a 2020  .image._axes].  
-00047960: 2020 2020 2020 736c 6963 655f 7468 6963        slice_thic
-00047970: 6b6e 6573 7320 3d20 6b77 6172 6773 2e70  kness = kwargs.p
-00047980: 6f70 2822 736c 6963 655f 7468 6963 6b6e  op("slice_thickn
-00047990: 6573 7322 2c20 4e6f 6e65 290a 2020 2020  ess", None).    
-000479a0: 2020 2020 736c 6963 655f 7468 6963 6b6e      slice_thickn
-000479b0: 6573 7320 3d20 2873 6c69 6365 5f74 6869  ess = (slice_thi
-000479c0: 636b 6e65 7373 206f 720a 2020 2020 2020  ckness or.      
-000479d0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
-000479e0: 6574 5f72 6f69 7328 6967 6e6f 7265 5f65  et_rois(ignore_e
-000479f0: 6d70 7479 3d54 7275 6529 5b30 5d5c 0a20  mpty=True)[0]\. 
-00047a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00047a10: 2020 2020 2020 202e 6765 745f 736c 6963         .get_slic
-00047a20: 655f 7468 6963 6b6e 6573 735f 636f 6e74  e_thickness_cont
-00047a30: 6f75 7273 2829 290a 2020 2020 2020 2020  ours()).        
-00047a40: 7265 7475 726e 2063 7265 6174 655f 6475  return create_du
-00047a50: 6d6d 795f 696d 6167 6528 6578 7465 6e74  mmy_image(extent
-00047a60: 732c 2073 6c69 6365 5f74 6869 636b 6e65  s, slice_thickne
-00047a70: 7373 2c20 2a2a 6b77 6172 6773 290a 0a20  ss, **kwargs).. 
-00047a80: 2020 2064 6566 205f 6765 745f 636f 6d62     def _get_comb
-00047a90: 696e 6174 696f 6e28 7365 6c66 2c20 6e61  ination(self, na
-00047aa0: 6d65 2c20 666f 7263 652c 2065 7863 6c75  me, force, exclu
-00047ab0: 6465 2c20 636f 6d62 6f5f 6d61 6b65 722c  de, combo_maker,
-00047ac0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00047ad0: 2020 2020 2222 2245 6974 6865 7220 6765      """Either ge
-00047ae0: 7420 616e 2061 6c72 6561 6479 2063 616c  t an already cal
-00047af0: 6375 6c61 7465 6420 636f 6d62 696e 6174  culated combinat
-00047b00: 696f 6e20 6672 6f6d 2074 6865 2063 6163  ion from the cac
-00047b10: 6865 0a20 2020 2020 2020 206f 7220 6372  he.        or cr
-00047b20: 6561 7465 2069 742c 2063 6163 6865 2069  eate it, cache i
-00047b30: 742c 2061 6e64 2072 6574 7572 6e20 6974  t, and return it
-00047b40: 2e22 2222 0a0a 2020 2020 2020 2020 2320  ."""..        # 
-00047b50: 5265 7475 726e 2063 6163 6865 6420 7265  Return cached re
-00047b60: 7375 6c74 2069 6620 6974 2065 7869 7374  sult if it exist
-00047b70: 7320 616e 6420 6e6f 7420 666f 7263 696e  s and not forcin
-00047b80: 670a 2020 2020 2020 2020 6174 7472 203d  g.        attr =
-00047b90: 2066 225f 7b6e 616d 657d 220a 2020 2020   f"_{name}".    
-00047ba0: 2020 2020 6966 2065 7863 6c75 6465 3a0a      if exclude:.
-00047bb0: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-00047bc0: 202b 3d20 6622 5f65 7863 6c75 6465 6422   += f"_excluded"
-00047bd0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00047be0: 666f 7263 653a 0a20 2020 2020 2020 2020  force:.         
-00047bf0: 2020 2069 6620 6578 636c 7564 6520 6973     if exclude is
-00047c00: 204e 6f6e 6520 616e 6420 6861 7361 7474   None and hasatt
-00047c10: 7228 7365 6c66 2c20 6174 7472 293a 0a20  r(self, attr):. 
-00047c20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00047c30: 6574 7572 6e20 6765 7461 7474 7228 7365  eturn getattr(se
-00047c40: 6c66 2c20 6174 7472 290a 2020 2020 2020  lf, attr).      
-00047c50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00047c60: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-00047c70: 6173 6174 7472 2873 656c 662c 2061 7474  asattr(self, att
-00047c80: 7229 2061 6e64 2065 7863 6c75 6465 2069  r) and exclude i
-00047c90: 6e20 6765 7461 7474 7228 7365 6c66 2c20  n getattr(self, 
-00047ca0: 6174 7472 293a 0a20 2020 2020 2020 2020  attr):.         
-00047cb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00047cc0: 6e20 6765 7461 7474 7228 7365 6c66 2c20  n getattr(self, 
-00047cd0: 6174 7472 295b 6578 636c 7564 655d 0a0a  attr)[exclude]..
-00047ce0: 2020 2020 2020 2020 2320 4765 7420 6c69          # Get li
-00047cf0: 7374 206f 6620 524f 4973 2074 6f20 696e  st of ROIs to in
-00047d00: 636c 7564 6520 696e 2074 6869 7320 636f  clude in this co
-00047d10: 6d62 696e 6174 696f 6e20 524f 490a 2020  mbination ROI.  
-00047d20: 2020 2020 2020 6966 2065 7863 6c75 6465        if exclude
-00047d30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 0a20   is not None:.. 
-00047d40: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
-00047d50: 636c 7564 6520 6e6f 7420 696e 2073 656c  clude not in sel
-00047d60: 662e 6765 745f 726f 695f 6e61 6d65 7328  f.get_roi_names(
-00047d70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00047d80: 2020 2070 7269 6e74 2866 2252 4f49 2074     print(f"ROI t
-00047d90: 6f20 6578 636c 7564 6520 7b65 7863 6c75  o exclude {exclu
-00047da0: 6465 7d20 6e6f 7420 666f 756e 642e 2229  de} not found.")
-00047db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00047dc0: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-00047dd0: 2020 2020 2072 6f69 735f 746f 5f69 6e63       rois_to_inc
-00047de0: 6c75 6465 203d 205b 726f 6920 666f 7220  lude = [roi for 
-00047df0: 726f 6920 696e 2073 656c 662e 726f 6973  roi in self.rois
-00047e00: 2069 6620 726f 692e 6e61 6d65 2021 3d20   if roi.name != 
-00047e10: 6578 636c 7564 655d 0a0a 2020 2020 2020  exclude]..      
-00047e20: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
-00047e30: 6174 7472 2873 656c 662c 2061 7474 7229  attr(self, attr)
-00047e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00047e50: 2020 7365 7461 7474 7228 7365 6c66 2c20    setattr(self, 
-00047e60: 6174 7472 2c20 7b7d 290a 2020 2020 2020  attr, {}).      
-00047e70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00047e80: 2020 2020 726f 6973 5f74 6f5f 696e 636c      rois_to_incl
-00047e90: 7564 6520 3d20 7365 6c66 2e72 6f69 730a  ude = self.rois.
-00047ea0: 0a20 2020 2020 2020 2023 204d 616b 6520  .        # Make 
-00047eb0: 6b77 6172 6773 2066 6f72 2052 4f49 2063  kwargs for ROI c
-00047ec0: 7265 6174 696f 6e0a 2020 2020 2020 2020  reation.        
-00047ed0: 726f 695f 6b77 6172 6773 203d 2073 656c  roi_kwargs = sel
-00047ee0: 662e 726f 695f 6b77 6172 6773 2e63 6f70  f.roi_kwargs.cop
-00047ef0: 7928 290a 2020 2020 2020 2020 726f 695f  y().        roi_
-00047f00: 6b77 6172 6773 2e75 7064 6174 6528 6b77  kwargs.update(kw
-00047f10: 6172 6773 290a 2020 2020 2020 2020 726f  args).        ro
-00047f20: 695f 6b77 6172 6773 5b22 6e61 6d65 225d  i_kwargs["name"]
-00047f30: 203d 206e 616d 650a 2020 2020 2020 2020   = name.        
-00047f40: 726f 695f 6b77 6172 6773 5b22 696d 6167  roi_kwargs["imag
-00047f50: 6522 5d20 3d20 7365 6c66 2e69 6d61 6765  e"] = self.image
-00047f60: 0a20 2020 2020 2020 2072 6f69 5f6b 7761  .        roi_kwa
-00047f70: 7267 735b 2261 6666 696e 6522 5d20 3d20  rgs["affine"] = 
-00047f80: 726f 6973 5f74 6f5f 696e 636c 7564 655b  rois_to_include[
-00047f90: 305d 2e67 6574 5f61 6666 696e 6528 7374  0].get_affine(st
-00047fa0: 616e 6461 7264 6973 653d 5472 7565 290a  andardise=True).
-00047fb0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
-00047fc0: 6520 7468 6520 524f 490a 2020 2020 2020  e the ROI.      
-00047fd0: 2020 726f 6920 3d20 636f 6d62 6f5f 6d61    roi = combo_ma
-00047fe0: 6b65 7228 726f 6973 5f74 6f5f 696e 636c  ker(rois_to_incl
-00047ff0: 7564 652c 202a 2a72 6f69 5f6b 7761 7267  ude, **roi_kwarg
-00048000: 7329 0a0a 2020 2020 2020 2020 2320 4164  s)..        # Ad
-00048010: 6420 6974 2074 6f20 7468 6520 6361 6368  d it to the cach
-00048020: 6520 616e 6420 7265 7475 726e 0a20 2020  e and return.   
-00048030: 2020 2020 2069 6620 6578 636c 7564 6520       if exclude 
-00048040: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00048050: 2020 2020 2073 6574 6174 7472 2873 656c       setattr(sel
-00048060: 662c 2061 7474 722c 2072 6f69 290a 2020  f, attr, roi).  
-00048070: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00048080: 2020 2020 2020 2020 6765 7461 7474 7228          getattr(
-00048090: 7365 6c66 2c20 6174 7472 295b 6578 636c  self, attr)[excl
-000480a0: 7564 655d 203d 2072 6f69 0a20 2020 2020  ude] = roi.     
-000480b0: 2020 2072 6574 7572 6e20 726f 690a 0a20     return roi.. 
-000480c0: 2020 2064 6566 2067 6574 5f63 6f6e 7365     def get_conse
-000480d0: 6e73 7573 2873 656c 662c 2063 6f6e 7365  nsus(self, conse
-000480e0: 6e73 7573 5f74 7970 652c 2063 6f6c 6f72  nsus_type, color
-000480f0: 3d22 626c 7565 222c 202a 2a6b 7761 7267  ="blue", **kwarg
-00048100: 7329 3a0a 0a20 2020 2020 2020 2023 2047  s):..        # G
-00048110: 6574 2063 6f6e 7365 6e73 7573 2063 616c  et consensus cal
-00048120: 6375 6c61 7469 6f6e 2066 756e 6374 696f  culation functio
-00048130: 6e0a 2020 2020 2020 2020 6966 2063 6f6e  n.        if con
-00048140: 7365 6e73 7573 5f74 7970 6520 3d3d 2022  sensus_type == "
-00048150: 6d61 6a6f 7269 7479 223a 0a20 2020 2020  majority":.     
-00048160: 2020 2020 2020 2063 6f6e 7365 6e73 7573         consensus
-00048170: 5f66 756e 6320 3d20 5374 7275 6374 7572  _func = Structur
-00048180: 6553 6574 2e67 6574 5f6d 616a 6f72 6974  eSet.get_majorit
-00048190: 795f 766f 7465 0a20 2020 2020 2020 2065  y_vote.        e
-000481a0: 6c69 6620 636f 6e73 656e 7375 735f 7479  lif consensus_ty
-000481b0: 7065 203d 3d20 2273 756d 223a 0a20 2020  pe == "sum":.   
-000481c0: 2020 2020 2020 2020 2063 6f6e 7365 6e73           consens
-000481d0: 7573 5f66 756e 6320 3d20 5374 7275 6374  us_func = Struct
-000481e0: 7572 6553 6574 2e67 6574 5f73 756d 0a20  ureSet.get_sum. 
-000481f0: 2020 2020 2020 2065 6c69 6620 636f 6e73         elif cons
-00048200: 656e 7375 735f 7479 7065 203d 3d20 226f  ensus_type == "o
-00048210: 7665 726c 6170 223a 0a20 2020 2020 2020  verlap":.       
-00048220: 2020 2020 2063 6f6e 7365 6e73 7573 5f66       consensus_f
-00048230: 756e 6320 3d20 5374 7275 6374 7572 6553  unc = StructureS
-00048240: 6574 2e67 6574 5f6f 7665 726c 6170 0a20  et.get_overlap. 
-00048250: 2020 2020 2020 2065 6c69 6620 636f 6e73         elif cons
-00048260: 656e 7375 735f 7479 7065 203d 3d20 2273  ensus_type == "s
-00048270: 7461 706c 6522 3a0a 2020 2020 2020 2020  taple":.        
-00048280: 2020 2020 636f 6e73 656e 7375 735f 6675      consensus_fu
-00048290: 6e63 203d 2053 7472 7563 7475 7265 5365  nc = StructureSe
-000482a0: 742e 6765 745f 7374 6170 6c65 0a20 2020  t.get_staple.   
-000482b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000482c0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000482d0: 7565 4572 726f 7228 6622 556e 7265 636f  ueError(f"Unreco
-000482e0: 676e 6973 6564 2063 6f6e 7365 6e73 7573  gnised consensus
-000482f0: 2074 7970 653a 207b 636f 6e73 656e 7375   type: {consensu
-00048300: 735f 7479 7065 7d22 290a 0a20 2020 2020  s_type}")..     
-00048310: 2020 2072 6574 7572 6e20 636f 6e73 656e     return consen
-00048320: 7375 735f 6675 6e63 2873 656c 662c 2063  sus_func(self, c
-00048330: 6f6c 6f72 3d63 6f6c 6f72 2c20 2a2a 6b77  olor=color, **kw
-00048340: 6172 6773 290a 0a20 2020 2064 6566 2067  args)..    def g
-00048350: 6574 5f73 7461 706c 6528 7365 6c66 2c20  et_staple(self, 
-00048360: 666f 7263 653d 4661 6c73 652c 2065 7863  force=False, exc
-00048370: 6c75 6465 3d4e 6f6e 652c 202a 2a6b 7761  lude=None, **kwa
-00048380: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-00048390: 2247 6574 2052 4f49 206f 626a 6563 7420  "Get ROI object 
-000483a0: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
-000483b0: 2053 5441 504c 4520 636f 6d62 696e 6174   STAPLE combinat
-000483c0: 696f 6e20 6f66 2052 4f49 7320 696e 2074  ion of ROIs in t
-000483d0: 6869 7320 0a20 2020 2020 2020 2073 7472  his .        str
-000483e0: 7563 7475 7265 2073 6574 2e20 4966 203c  ucture set. If <
-000483f0: 6578 636c 7564 653e 2069 7320 7365 7420  exclude> is set 
-00048400: 746f 2061 2073 7472 696e 672c 2074 6865  to a string, the
-00048410: 2052 4f49 2077 6974 6820 7468 6174 206e   ROI with that n
-00048420: 616d 6520 0a20 2020 2020 2020 2077 696c  ame .        wil
-00048430: 6c20 6265 2065 7863 6c75 6465 6420 6672  l be excluded fr
-00048440: 6f6d 2074 6865 2063 616c 6375 6c61 7469  om the calculati
-00048450: 6f6e 2e0a 0a20 2020 2020 2020 202a 2a50  on...        **P
-00048460: 6172 616d 6574 6572 733a 2a2a 0a0a 2020  arameters:**..  
-00048470: 2020 2020 2020 666f 7263 6520 3a20 626f        force : bo
-00048480: 6f6c 2c20 6465 6661 756c 743d 4661 6c73  ol, default=Fals
-00048490: 650a 2020 2020 2020 2020 2020 2020 4966  e.            If
-000484a0: 2046 616c 7365 2061 6e64 2053 5441 504c   False and STAPL
-000484b0: 4520 524f 4920 6861 7320 616c 7265 6164  E ROI has alread
-000484c0: 7920 6265 656e 2063 7265 6174 6564 2c20  y been created, 
-000484d0: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
-000484e0: 2070 7265 7669 6f75 736c 7920 636f 6d70   previously comp
-000484f0: 7574 6564 2052 4f49 2077 696c 6c20 6265  uted ROI will be
-00048500: 2072 6574 7572 6e65 642e 2049 6620 466f   returned. If Fo
-00048510: 7263 653d 5472 7565 2c20 7468 6520 0a20  rce=True, the . 
-00048520: 2020 2020 2020 2020 2020 2053 5441 504c             STAPL
-00048530: 4520 524f 4920 7769 6c6c 2062 6520 7265  E ROI will be re
-00048540: 6372 6561 7465 642e 0a0a 2020 2020 2020  created...      
-00048550: 2020 6578 636c 7564 6520 3a20 7374 722c    exclude : str,
-00048560: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
-00048570: 2020 2020 2020 2020 2020 4966 2073 6574            If set
-00048580: 2074 6f20 6120 7374 7269 6e67 2c20 7468   to a string, th
-00048590: 6520 6669 7273 7420 524f 4920 696e 2073  e first ROI in s
-000485a0: 656c 662e 726f 6973 2077 6974 6820 7468  elf.rois with th
-000485b0: 6174 206e 616d 6520 7769 6c6c 200a 2020  at name will .  
-000485c0: 2020 2020 2020 2020 2020 6265 2065 7863            be exc
-000485d0: 6c75 6465 6420 6672 6f6d 2074 6865 2063  luded from the c
-000485e0: 6f6d 6269 6e61 7469 6f6e 2e20 5468 6973  ombination. This
-000485f0: 206d 6179 2062 6520 7573 6566 756c 2069   may be useful i
-00048600: 6620 636f 6d70 6172 6973 6f6e 200a 2020  f comparison .  
-00048610: 2020 2020 2020 2020 2020 6f66 2061 2073            of a s
-00048620: 696e 676c 6520 524f 4920 7769 7468 2074  ingle ROI with t
-00048630: 6865 2063 6f6e 7365 6e73 7573 206f 6620  he consensus of 
-00048640: 616c 6c20 6f74 6865 7273 2069 7320 6465  all others is de
-00048650: 7369 7265 642e 0a0a 2020 2020 2020 2020  sired...        
-00048660: 602a 2a60 6b77 6172 6773 203a 0a20 2020  `**`kwargs :.   
-00048670: 2020 2020 2020 2020 2045 7874 7261 206b           Extra k
-00048680: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-00048690: 2074 6f20 7061 7373 2074 6f20 7468 6520   to pass to the 
-000486a0: 6372 6561 7469 6f6e 206f 6620 7468 6520  creation of the 
-000486b0: 524f 4920 6f62 6a65 6374 0a20 2020 2020  ROI object.     
-000486c0: 2020 2020 2020 2072 6570 7265 7365 6e74         represent
-000486d0: 696e 6720 7468 6520 636f 6d62 696e 6174  ing the combinat
-000486e0: 696f 6e2e 0a20 2020 2020 2020 2022 2222  ion..        """
-000486f0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00048700: 2073 656c 662e 5f67 6574 5f63 6f6d 6269   self._get_combi
-00048710: 6e61 7469 6f6e 2822 7374 6170 6c65 222c  nation("staple",
-00048720: 2066 6f72 6365 2c20 6578 636c 7564 652c   force, exclude,
-00048730: 2063 7265 6174 655f 7374 6170 6c65 2c0a   create_staple,.
-00048740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00048750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00048760: 2020 2020 202a 2a6b 7761 7267 7329 0a0a       **kwargs)..
-00048770: 2020 2020 6465 6620 6765 745f 6d61 6a6f      def get_majo
-00048780: 7269 7479 5f76 6f74 6528 7365 6c66 2c20  rity_vote(self, 
-00048790: 666f 7263 653d 4661 6c73 652c 2065 7863  force=False, exc
-000487a0: 6c75 6465 3d4e 6f6e 652c 202a 2a6b 7761  lude=None, **kwa
-000487b0: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-000487c0: 2247 6574 2052 4f49 206f 626a 6563 7420  "Get ROI object 
-000487d0: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
-000487e0: 206d 616a 6f72 6974 7920 766f 7465 2063   majority vote c
-000487f0: 6f6d 6269 6e61 7469 6f6e 206f 6620 524f  ombination of RO
-00048800: 4973 2069 6e20 0a20 2020 2020 2020 2074  Is in .        t
-00048810: 6869 7320 7374 7275 6374 7572 6520 7365  his structure se
-00048820: 742e 2049 6620 3c65 7863 6c75 6465 3e20  t. If <exclude> 
-00048830: 6973 2073 6574 2074 6f20 6120 7374 7269  is set to a stri
-00048840: 6e67 2c20 7468 6520 524f 4920 7769 7468  ng, the ROI with
-00048850: 2074 6861 7420 0a20 2020 2020 2020 206e   that .        n
-00048860: 616d 6520 7769 6c6c 2062 6520 6578 636c  ame will be excl
-00048870: 7564 6564 2066 726f 6d20 7468 6520 6361  uded from the ca
-00048880: 6c63 756c 6174 696f 6e2e 0a0a 2020 2020  lculation...    
-00048890: 2020 2020 2a2a 5061 7261 6d65 7465 7273      **Parameters
-000488a0: 3a2a 2a0a 0a20 2020 2020 2020 2066 6f72  :**..        for
-000488b0: 6365 203a 2062 6f6f 6c2c 2064 6566 6175  ce : bool, defau
-000488c0: 6c74 3d46 616c 7365 0a20 2020 2020 2020  lt=False.       
-000488d0: 2020 2020 2049 6620 4661 6c73 6520 616e       If False an
-000488e0: 6420 6d61 6a6f 7269 7479 2076 6f74 6520  d majority vote 
-000488f0: 524f 4920 6861 7320 616c 7265 6164 7920  ROI has already 
-00048900: 6265 656e 2063 7265 6174 6564 2c20 7468  been created, th
-00048910: 6520 0a20 2020 2020 2020 2020 2020 2070  e .            p
-00048920: 7265 7669 6f75 736c 7920 636f 6d70 7574  reviously comput
-00048930: 6564 2052 4f49 2077 696c 6c20 6265 2072  ed ROI will be r
-00048940: 6574 7572 6e65 642e 2049 6620 466f 7263  eturned. If Forc
-00048950: 653d 5472 7565 2c20 7468 6520 0a20 2020  e=True, the .   
-00048960: 2020 2020 2020 2020 206d 616a 6f72 6974           majorit
-00048970: 7920 766f 7465 2052 4f49 2077 696c 6c20  y vote ROI will 
-00048980: 6265 2072 6563 7265 6174 6564 2e0a 0a20  be recreated... 
-00048990: 2020 2020 2020 2065 7863 6c75 6465 203a         exclude :
-000489a0: 2073 7472 2c20 6465 6661 756c 743d 4e6f   str, default=No
-000489b0: 6e65 0a20 2020 2020 2020 2020 2020 2049  ne.            I
-000489c0: 6620 7365 7420 746f 2061 2073 7472 696e  f set to a strin
-000489d0: 672c 2074 6865 2066 6972 7374 2052 4f49  g, the first ROI
-000489e0: 2069 6e20 7365 6c66 2e72 6f69 7320 7769   in self.rois wi
-000489f0: 7468 2074 6861 7420 6e61 6d65 2077 696c  th that name wil
-00048a00: 6c20 0a20 2020 2020 2020 2020 2020 2062  l .            b
-00048a10: 6520 6578 636c 7564 6564 2066 726f 6d20  e excluded from 
-00048a20: 7468 6520 636f 6d62 696e 6174 696f 6e2e  the combination.
-00048a30: 2054 6869 7320 6d61 7920 6265 2075 7365   This may be use
-00048a40: 6675 6c20 6966 2063 6f6d 7061 7269 736f  ful if compariso
-00048a50: 6e20 0a20 2020 2020 2020 2020 2020 206f  n .            o
-00048a60: 6620 6120 7369 6e67 6c65 2052 4f49 2077  f a single ROI w
-00048a70: 6974 6820 7468 6520 636f 6e73 656e 7375  ith the consensu
-00048a80: 7320 6f66 2061 6c6c 206f 7468 6572 7320  s of all others 
-00048a90: 6973 2064 6573 6972 6564 2e0a 0a20 2020  is desired...   
-00048aa0: 2020 2020 2060 2a2a 606b 7761 7267 7320       `**`kwargs 
-00048ab0: 3a0a 2020 2020 2020 2020 2020 2020 4578  :.            Ex
-00048ac0: 7472 6120 6b65 7977 6f72 6420 6172 6775  tra keyword argu
-00048ad0: 6d65 6e74 7320 746f 2070 6173 7320 746f  ments to pass to
-00048ae0: 2074 6865 2063 7265 6174 696f 6e20 6f66   the creation of
-00048af0: 2074 6865 2052 4f49 206f 626a 6563 740a   the ROI object.
-00048b00: 2020 2020 2020 2020 2020 2020 7265 7072              repr
-00048b10: 6573 656e 7469 6e67 2074 6865 2063 6f6d  esenting the com
-00048b20: 6269 6e61 7469 6f6e 2e0a 2020 2020 2020  bination..      
-00048b30: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-00048b40: 6574 7572 6e20 7365 6c66 2e5f 6765 745f  eturn self._get_
-00048b50: 636f 6d62 696e 6174 696f 6e28 226d 616a  combination("maj
-00048b60: 6f72 6974 795f 766f 7465 222c 2066 6f72  ority_vote", for
-00048b70: 6365 2c20 6578 636c 7564 652c 200a 2020  ce, exclude, .  
-00048b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00048b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00048ba0: 2020 2063 7265 6174 655f 6d61 6a6f 7269     create_majori
-00048bb0: 7479 5f76 6f74 652c 202a 2a6b 7761 7267  ty_vote, **kwarg
-00048bc0: 7329 0a0a 2020 2020 6465 6620 6765 745f  s)..    def get_
-00048bd0: 7375 6d28 7365 6c66 2c20 666f 7263 653d  sum(self, force=
-00048be0: 4661 6c73 652c 2065 7863 6c75 6465 3d4e  False, exclude=N
-00048bf0: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0a  one, **kwargs):.
-00048c00: 2020 2020 2020 2020 2222 2247 6574 2052          """Get R
-00048c10: 4f49 206f 626a 6563 7420 7265 7072 6573  OI object repres
-00048c20: 656e 7469 6e67 2074 6865 2073 756d 206f  enting the sum o
-00048c30: 6620 524f 4973 2069 6e20 7468 6973 2073  f ROIs in this s
-00048c40: 7472 7563 7475 7265 2073 6574 2e20 0a20  tructure set. . 
-00048c50: 2020 2020 2020 2049 6620 3c65 7863 6c75         If <exclu
-00048c60: 6465 3e20 6973 2073 6574 2074 6f20 6120  de> is set to a 
-00048c70: 7374 7269 6e67 2c20 7468 6520 524f 4920  string, the ROI 
-00048c80: 7769 7468 2074 6861 7420 6e61 6d65 2077  with that name w
-00048c90: 696c 6c20 6265 200a 2020 2020 2020 2020  ill be .        
-00048ca0: 6578 636c 7564 6564 2066 726f 6d20 7468  excluded from th
-00048cb0: 6520 6361 6c63 756c 6174 696f 6e2e 0a0a  e calculation...
-00048cc0: 2020 2020 2020 2020 2a2a 5061 7261 6d65          **Parame
-00048cd0: 7465 7273 3a2a 2a0a 0a20 2020 2020 2020  ters:**..       
-00048ce0: 2066 6f72 6365 203a 2062 6f6f 6c2c 2064   force : bool, d
-00048cf0: 6566 6175 6c74 3d46 616c 7365 0a20 2020  efault=False.   
-00048d00: 2020 2020 2020 2020 2049 6620 4661 6c73           If Fals
-00048d10: 6520 616e 6420 7375 6d20 524f 4920 6861  e and sum ROI ha
-00048d20: 7320 616c 7265 6164 7920 6265 656e 2063  s already been c
-00048d30: 7265 6174 6564 2c20 7468 6520 0a20 2020  reated, the .   
-00048d40: 2020 2020 2020 2020 2070 7265 7669 6f75           previou
-00048d50: 736c 7920 636f 6d70 7574 6564 2052 4f49  sly computed ROI
-00048d60: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
-00048d70: 642e 2049 6620 466f 7263 653d 5472 7565  d. If Force=True
-00048d80: 2c20 7468 6520 0a20 2020 2020 2020 2020  , the .         
-00048d90: 2020 2073 756d 2052 4f49 2077 696c 6c20     sum ROI will 
-00048da0: 6265 2072 6563 7265 6174 6564 2e0a 0a20  be recreated... 
-00048db0: 2020 2020 2020 2065 7863 6c75 6465 203a         exclude :
-00048dc0: 2073 7472 2c20 6465 6661 756c 743d 4e6f   str, default=No
-00048dd0: 6e65 0a20 2020 2020 2020 2020 2020 2049  ne.            I
-00048de0: 6620 7365 7420 746f 2061 2073 7472 696e  f set to a strin
-00048df0: 672c 2074 6865 2066 6972 7374 2052 4f49  g, the first ROI
-00048e00: 2069 6e20 7365 6c66 2e72 6f69 7320 7769   in self.rois wi
-00048e10: 7468 2074 6861 7420 6e61 6d65 2077 696c  th that name wil
-00048e20: 6c20 0a20 2020 2020 2020 2020 2020 2062  l .            b
-00048e30: 6520 6578 636c 7564 6564 2066 726f 6d20  e excluded from 
-00048e40: 7468 6520 636f 6d62 696e 6174 696f 6e2e  the combination.
-00048e50: 2054 6869 7320 6d61 7920 6265 2075 7365   This may be use
-00048e60: 6675 6c20 6966 2063 6f6d 7061 7269 736f  ful if compariso
-00048e70: 6e20 0a20 2020 2020 2020 2020 2020 206f  n .            o
-00048e80: 6620 6120 7369 6e67 6c65 2052 4f49 2077  f a single ROI w
-00048e90: 6974 6820 7468 6520 636f 6e73 656e 7375  ith the consensu
-00048ea0: 7320 6f66 2061 6c6c 206f 7468 6572 7320  s of all others 
-00048eb0: 6973 2064 6573 6972 6564 2e0a 0a20 2020  is desired...   
-00048ec0: 2020 2020 2060 2a2a 606b 7761 7267 7320       `**`kwargs 
-00048ed0: 3a0a 2020 2020 2020 2020 2020 2020 4578  :.            Ex
-00048ee0: 7472 6120 6b65 7977 6f72 6420 6172 6775  tra keyword argu
-00048ef0: 6d65 6e74 7320 746f 2070 6173 7320 746f  ments to pass to
-00048f00: 2074 6865 2063 7265 6174 696f 6e20 6f66   the creation of
-00048f10: 2074 6865 2052 4f49 206f 626a 6563 740a   the ROI object.
-00048f20: 2020 2020 2020 2020 2020 2020 7265 7072              repr
-00048f30: 6573 656e 7469 6e67 2074 6865 2063 6f6d  esenting the com
-00048f40: 6269 6e61 7469 6f6e 2e0a 2020 2020 2020  bination..      
-00048f50: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-00048f60: 6574 7572 6e20 7365 6c66 2e5f 6765 745f  eturn self._get_
-00048f70: 636f 6d62 696e 6174 696f 6e28 2273 756d  combination("sum
-00048f80: 222c 2066 6f72 6365 2c20 6578 636c 7564  ", force, exclud
-00048f90: 652c 200a 2020 2020 2020 2020 2020 2020  e, .            
-00048fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00048fb0: 2020 2020 2020 2020 2063 7265 6174 655f           create_
-00048fc0: 726f 695f 7375 6d2c 202a 2a6b 7761 7267  roi_sum, **kwarg
-00048fd0: 7329 0a0a 2020 2020 6465 6620 6765 745f  s)..    def get_
-00048fe0: 6f76 6572 6c61 7028 7365 6c66 2c20 666f  overlap(self, fo
-00048ff0: 7263 653d 4661 6c73 652c 2065 7863 6c75  rce=False, exclu
-00049000: 6465 3d4e 6f6e 652c 202a 2a6b 7761 7267  de=None, **kwarg
-00049010: 7329 3a0a 2020 2020 2020 2020 2222 2247  s):.        """G
-00049020: 6574 2052 4f49 206f 626a 6563 7420 7265  et ROI object re
-00049030: 7072 6573 656e 7469 6e67 2074 6865 206f  presenting the o
-00049040: 7665 726c 6170 206f 6620 524f 4973 2069  verlap of ROIs i
-00049050: 6e20 7468 6973 200a 2020 2020 2020 2020  n this .        
-00049060: 7374 7275 6374 7572 6520 7365 742e 2049  structure set. I
-00049070: 6620 3c65 7863 6c75 6465 3e20 6973 2073  f <exclude> is s
-00049080: 6574 2074 6f20 6120 7374 7269 6e67 2c20  et to a string, 
-00049090: 7468 6520 524f 4920 7769 7468 2074 6861  the ROI with tha
-000490a0: 7420 6e61 6d65 200a 2020 2020 2020 2020  t name .        
-000490b0: 7769 6c6c 2062 6520 6578 636c 7564 6564  will be excluded
-000490c0: 2066 726f 6d20 7468 6520 6361 6c63 756c   from the calcul
-000490d0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-000490e0: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
-000490f0: 0a20 2020 2020 2020 2066 6f72 6365 203a  .        force :
-00049100: 2062 6f6f 6c2c 2064 6566 6175 6c74 3d46   bool, default=F
-00049110: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00049120: 2049 6620 4661 6c73 6520 616e 6420 6f76   If False and ov
-00049130: 6572 6c61 7020 524f 4920 6861 7320 616c  erlap ROI has al
-00049140: 7265 6164 7920 6265 656e 2063 7265 6174  ready been creat
-00049150: 6564 2c20 7468 6520 0a20 2020 2020 2020  ed, the .       
-00049160: 2020 2020 2070 7265 7669 6f75 736c 7920       previously 
-00049170: 636f 6d70 7574 6564 2052 4f49 2077 696c  computed ROI wil
-00049180: 6c20 6265 2072 6574 7572 6e65 642e 2049  l be returned. I
-00049190: 6620 466f 7263 653d 5472 7565 2c20 7468  f Force=True, th
-000491a0: 6520 0a20 2020 2020 2020 2020 2020 206f  e .            o
-000491b0: 7665 726c 6170 2052 4f49 2077 696c 6c20  verlap ROI will 
-000491c0: 6265 2072 6563 7265 6174 6564 2e0a 0a20  be recreated... 
-000491d0: 2020 2020 2020 2065 7863 6c75 6465 203a         exclude :
-000491e0: 2073 7472 2c20 6465 6661 756c 743d 4e6f   str, default=No
-000491f0: 6e65 0a20 2020 2020 2020 2020 2020 2049  ne.            I
-00049200: 6620 7365 7420 746f 2061 2073 7472 696e  f set to a strin
-00049210: 672c 2074 6865 2066 6972 7374 2052 4f49  g, the first ROI
-00049220: 2069 6e20 7365 6c66 2e72 6f69 7320 7769   in self.rois wi
-00049230: 7468 2074 6861 7420 6e61 6d65 2077 696c  th that name wil
-00049240: 6c20 0a20 2020 2020 2020 2020 2020 2062  l .            b
-00049250: 6520 6578 636c 7564 6564 2066 726f 6d20  e excluded from 
-00049260: 7468 6520 636f 6d62 696e 6174 696f 6e2e  the combination.
-00049270: 2054 6869 7320 6d61 7920 6265 2075 7365   This may be use
-00049280: 6675 6c20 6966 2063 6f6d 7061 7269 736f  ful if compariso
-00049290: 6e20 0a20 2020 2020 2020 2020 2020 206f  n .            o
-000492a0: 6620 6120 7369 6e67 6c65 2052 4f49 2077  f a single ROI w
-000492b0: 6974 6820 7468 6520 636f 6e73 656e 7375  ith the consensu
-000492c0: 7320 6f66 2061 6c6c 206f 7468 6572 7320  s of all others 
-000492d0: 6973 2064 6573 6972 6564 2e0a 0a20 2020  is desired...   
-000492e0: 2020 2020 2060 2a2a 606b 7761 7267 7320       `**`kwargs 
-000492f0: 3a0a 2020 2020 2020 2020 2020 2020 4578  :.            Ex
-00049300: 7472 6120 6b65 7977 6f72 6420 6172 6775  tra keyword argu
-00049310: 6d65 6e74 7320 746f 2070 6173 7320 746f  ments to pass to
-00049320: 2074 6865 2063 7265 6174 696f 6e20 6f66   the creation of
-00049330: 2074 6865 2052 4f49 206f 626a 6563 740a   the ROI object.
-00049340: 2020 2020 2020 2020 2020 2020 7265 7072              repr
-00049350: 6573 656e 7469 6e67 2074 6865 2063 6f6d  esenting the com
-00049360: 6269 6e61 7469 6f6e 2e0a 2020 2020 2020  bination..      
-00049370: 2020 2222 220a 0a20 2020 2020 2020 2072    """..        r
-00049380: 6574 7572 6e20 7365 6c66 2e5f 6765 745f  eturn self._get_
-00049390: 636f 6d62 696e 6174 696f 6e28 226f 7665  combination("ove
-000493a0: 726c 6170 222c 2066 6f72 6365 2c20 6578  rlap", force, ex
-000493b0: 636c 7564 652c 200a 2020 2020 2020 2020  clude, .        
-000493c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000493d0: 2020 2020 2020 2020 2020 2020 2063 7265               cre
-000493e0: 6174 655f 726f 695f 6f76 6572 6c61 702c  ate_roi_overlap,
-000493f0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-00049400: 6465 6620 7472 616e 7366 6f72 6d28 7365  def transform(se
-00049410: 6c66 2c20 7363 616c 653d 312c 2074 7261  lf, scale=1, tra
-00049420: 6e73 6c61 7469 6f6e 3d5b 302c 2030 2c20  nslation=[0, 0, 
-00049430: 305d 2c20 726f 7461 7469 6f6e 3d5b 302c  0], rotation=[0,
-00049440: 2030 2c20 305d 2c0a 2020 2020 2020 2020   0, 0],.        
-00049450: 2020 2020 6365 6e74 7265 3d5b 302c 2030      centre=[0, 0
-00049460: 2c20 305d 2c20 7265 7361 6d70 6c65 3d22  , 0], resample="
-00049470: 6669 6e65 222c 2072 6573 746f 7265 3d54  fine", restore=T
-00049480: 7275 652c 200a 2020 2020 2020 2020 2020  rue, .          
-00049490: 2020 6669 6c6c 5f76 616c 7565 3d4e 6f6e    fill_value=Non
-000494a0: 652c 2066 6f72 6365 5f63 6f6e 746f 7572  e, force_contour
-000494b0: 733d 4661 6c73 652c 206e 616d 6573 3d4e  s=False, names=N
-000494c0: 6f6e 6529 3a0a 2020 2020 2020 2020 2222  one):.        ""
-000494d0: 220a 2020 2020 2020 2020 4170 706c 7920  ".        Apply 
-000494e0: 7468 7265 652d 6469 6d65 6e73 696f 6e61  three-dimensiona
-000494f0: 6c20 7369 6d69 6c61 7269 7479 2074 7261  l similarity tra
-00049500: 6e73 666f 726d 2074 6f20 7374 7275 6374  nsform to struct
-00049510: 7572 652d 7365 7420 524f 4973 2e0a 0a20  ure-set ROIs... 
-00049520: 2020 2020 2020 2049 6620 7468 6520 7472         If the tr
-00049530: 616e 7366 6f72 6d20 636f 7272 6573 706f  ansform correspo
-00049540: 6e64 7320 746f 2061 2074 7261 6e73 6c61  nds to a transla
-00049550: 7469 6f6e 2061 6e64 2f6f 7220 726f 7461  tion and/or rota
-00049560: 7469 6f6e 0a20 2020 2020 2020 2061 626f  tion.        abo
-00049570: 7574 2074 6865 207a 2d61 7869 732c 2061  ut the z-axis, a
-00049580: 6e64 2065 6974 6865 7220 7468 6520 726f  nd either the ro
-00049590: 6920 736f 7572 6365 2074 7970 6520 6973  i source type is
-000495a0: 2022 6469 636f 6d22 0a20 2020 2020 2020   "dicom".       
-000495b0: 206f 7220 666f 7263 652d 636f 6e74 6f75   or force-contou
-000495c0: 7273 2069 7320 5472 7565 2c20 7468 6520  rs is True, the 
-000495d0: 7472 616e 7366 6f72 6d20 6973 2061 7070  transform is app
-000495e0: 6c69 6564 2074 6f20 636f 6e74 6f75 720a  lied to contour.
-000495f0: 2020 2020 2020 2020 706f 696e 7473 2061          points a
-00049600: 6e64 2074 6865 2072 6f69 206d 6173 6b20  nd the roi mask 
-00049610: 6973 2073 6574 2061 7320 756e 6c6f 6164  is set as unload
-00049620: 6564 2e20 204f 7468 6572 7769 7365 2074  ed.  Otherwise t
-00049630: 6865 2074 7261 6e73 666f 726d 0a20 2020  he transform.   
-00049640: 2020 2020 2069 7320 6170 706c 6965 6420       is applied 
-00049650: 746f 2074 6865 206d 6173 6b20 616e 6420  to the mask and 
-00049660: 636f 6e74 6f75 7273 2061 7265 2073 6574  contours are set
-00049670: 2061 7320 756e 6c6f 6164 6564 2e0a 0a20   as unloaded... 
-00049680: 2020 2020 2020 2054 6865 2074 7261 6e73         The trans
-00049690: 666f 726d 2069 7320 6170 706c 6965 6420  form is applied 
-000496a0: 696e 2074 6865 206f 7264 6572 3a20 7472  in the order: tr
-000496b0: 616e 736c 6174 696f 6e2c 2073 6361 6c69  anslation, scali
-000496c0: 6e67 2c0a 2020 2020 2020 2020 726f 7461  ng,.        rota
-000496d0: 7469 6f6e 2e20 2054 6865 206c 6174 7465  tion.  The latte
-000496e0: 7220 7477 6f20 6172 6520 6162 6f75 7420  r two are about 
-000496f0: 7468 6520 6365 6e74 7265 2063 6f6f 7264  the centre coord
-00049700: 696e 6174 6573 2e0a 0a20 2020 2020 2020  inates...       
-00049710: 202a 2a50 6172 616d 6574 6572 733a 2a2a   **Parameters:**
-00049720: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00049730: 2020 666f 7263 655f 636f 6e74 6f75 7273    force_contours
-00049740: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00049750: 3d46 616c 7365 0a20 2020 2020 2020 2020  =False.         
-00049760: 2020 2049 6620 5472 7565 2c20 616e 6420     If True, and 
-00049770: 7468 6520 7472 616e 7366 6f72 6d20 636f  the transform co
-00049780: 7272 6573 706f 6e64 7320 746f 2061 2074  rresponds to a t
-00049790: 7261 6e73 6c61 7469 6f6e 0a20 2020 2020  ranslation.     
-000497a0: 2020 2020 2020 2061 6e64 2f6f 7220 726f         and/or ro
-000497b0: 7461 7469 6f6e 2061 626f 7574 2074 6865  tation about the
-000497c0: 207a 2d61 7869 732c 2061 7070 6c79 2074   z-axis, apply t
-000497d0: 7261 6e73 666f 726d 2074 6f20 636f 6e74  ransform to cont
-000497e0: 6f75 720a 2020 2020 2020 2020 2020 2020  our.            
-000497f0: 706f 696e 7473 2069 6e64 6570 656e 6465  points independe
-00049800: 6e74 6c79 206f 6620 7468 6520 6f72 6967  ntly of the orig
-00049810: 696e 616c 2064 6174 6120 736f 7572 6365  inal data source
-00049820: 2e0a 0a20 2020 2020 2020 206e 616d 6573  ...        names
-00049830: 203a 206c 6973 742f 4e6f 6e65 2c20 6465   : list/None, de
-00049840: 6661 756c 743d 4661 6c73 650a 2020 2020  fault=False.    
-00049850: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
-00049860: 524f 4973 2074 6f20 7768 6963 6820 7472  ROIs to which tr
-00049870: 616e 7366 6f72 6d20 6973 2074 6f20 6265  ansform is to be
-00049880: 2061 7070 6c69 6564 2e20 2049 6620 4e6f   applied.  If No
-00049890: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000498a0: 7472 616e 7366 6f72 6d20 6973 2061 7070  transform is app
-000498b0: 6c69 6564 2074 6f20 616c 6c20 524f 4973  lied to all ROIs
-000498c0: 2e0a 0a20 2020 2020 2020 2046 6f72 206f  ...        For o
-000498d0: 7468 6572 2070 6172 616d 6574 6572 732c  ther parameters,
-000498e0: 2073 6565 2064 6f63 756d 656e 7461 7469   see documentati
-000498f0: 6f6e 2066 6f72 0a20 2020 2020 2020 2073  on for.        s
-00049900: 6b72 742e 696d 6167 652e 496d 6167 652e  krt.image.Image.
-00049910: 7472 616e 7366 6f72 6d28 292e 2020 4e6f  transform().  No
-00049920: 7465 2074 6861 7420 7468 6520 6060 6f72  te that the ``or
-00049930: 6465 7260 600a 2020 2020 2020 2020 7061  der``.        pa
-00049940: 7261 6d65 7465 7220 6973 6e27 7420 6176  rameter isn't av
-00049950: 6169 6c61 626c 6520 666f 7220 7374 7275  ailable for stru
-00049960: 6374 7572 652d 7365 7420 7472 616e 7366  cture-set transf
-00049970: 6f72 6d73 202d 2061 2076 616c 7565 206f  orms - a value o
-00049980: 6620 300a 2020 2020 2020 2020 6973 2075  f 0.        is u
-00049990: 7365 6420 616c 7761 7973 2e0a 2020 2020  sed always..    
-000499a0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-000499b0: 2066 6f72 2072 6f69 2069 6e20 7365 6c66   for roi in self
-000499c0: 2e67 6574 5f72 6f69 7328 6e61 6d65 7329  .get_rois(names)
-000499d0: 3a0a 2020 2020 2020 2020 2020 2020 726f  :.            ro
-000499e0: 692e 7472 616e 7366 6f72 6d28 7363 616c  i.transform(scal
-000499f0: 652c 2074 7261 6e73 6c61 7469 6f6e 2c20  e, translation, 
-00049a00: 726f 7461 7469 6f6e 2c20 6365 6e74 7265  rotation, centre
-00049a10: 2c20 7265 7361 6d70 6c65 2c0a 2020 2020  , resample,.    
-00049a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00049a30: 7265 7374 6f72 652c 2066 696c 6c5f 7661  restore, fill_va
-00049a40: 6c75 652c 2066 6f72 6365 5f63 6f6e 746f  lue, force_conto
-00049a50: 7572 7329 0a0a 2020 2020 2020 2020 7265  urs)..        re
-00049a60: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
-00049a70: 6566 2061 6464 5f70 6c61 6e28 7365 6c66  ef add_plan(self
-00049a80: 2c20 706c 616e 293a 0a20 2020 2020 2020  , plan):.       
-00049a90: 2022 2222 4164 6420 6120 506c 616e 206f   """Add a Plan o
-00049aa0: 626a 6563 7420 746f 2062 6520 6173 736f  bject to be asso
-00049ab0: 6369 6174 6564 2077 6974 6820 7468 6973  ciated with this
-00049ac0: 2073 7472 7563 7475 7265 2073 6574 2061   structure set a
-00049ad0: 6e64 0a20 2020 2020 2020 2069 7473 2052  nd.        its R
-00049ae0: 4f49 732e 2054 6869 7320 646f 6573 206e  OIs. This does n
-00049af0: 6f74 2061 6666 6563 7420 7468 6520 7374  ot affect the st
-00049b00: 7275 6374 7572 6520 7365 7420 6173 736f  ructure set asso
-00049b10: 6369 6174 6564 2077 6974 680a 2020 2020  ciated with.    
-00049b20: 2020 2020 7468 6520 506c 616e 206f 626a      the Plan obj
-00049b30: 6563 742e 0a0a 2020 2020 2020 2020 2a2a  ect...        **
-00049b40: 5061 7261 6d65 7465 7273 3a2a 2a0a 0a20  Parameters:**.. 
-00049b50: 2020 2020 2020 2070 6c61 6e20 3a20 736b         plan : sk
-00049b60: 7274 2e64 6f73 652e 506c 616e 0a20 2020  rt.dose.Plan.   
-00049b70: 2020 2020 2020 2020 2041 2050 6c61 6e20           A Plan 
-00049b80: 6f62 6a65 6374 2074 6f20 6173 7369 676e  object to assign
-00049b90: 2074 6f20 7468 6973 2073 7472 7563 7475   to this structu
-00049ba0: 7265 2073 6574 2e0a 2020 2020 2020 2020  re set..        
-00049bb0: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
-00049bc0: 6e6f 7420 706c 616e 2069 6e20 7365 6c66  not plan in self
-00049bd0: 2e70 6c61 6e73 3a0a 2020 2020 2020 2020  .plans:.        
-00049be0: 2020 2020 7365 6c66 2e70 6c61 6e73 2e61      self.plans.a
-00049bf0: 7070 656e 6428 706c 616e 290a 2020 2020  ppend(plan).    
-00049c00: 2020 2020 2020 2020 7365 6c66 2e70 6c61          self.pla
-00049c10: 6e73 2e73 6f72 7428 290a 0a20 2020 2020  ns.sort()..     
-00049c20: 2020 2020 2020 2066 6f72 2072 6f69 2069         for roi i
-00049c30: 6e20 7365 6c66 2e72 6f69 733a 0a20 2020  n self.rois:.   
-00049c40: 2020 2020 2020 2020 2020 2020 2072 6f69               roi
-00049c50: 2e61 6464 5f70 6c61 6e28 706c 616e 290a  .add_plan(plan).
-00049c60: 0a20 2020 2064 6566 2063 6c65 6172 5f70  .    def clear_p
-00049c70: 6c61 6e73 2873 656c 6629 3a0a 2020 2020  lans(self):.    
-00049c80: 2020 2020 2222 2243 6c65 6172 2061 6c6c      """Clear all
-00049c90: 2070 6c61 6e20 6d61 7073 2061 7373 6f63   plan maps assoc
-00049ca0: 6961 7465 6420 7769 7468 2074 6869 7320  iated with this 
-00049cb0: 7374 7275 6374 7572 6520 7365 742e 2222  structure set.""
-00049cc0: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00049cd0: 706c 616e 7320 3d20 5b5d 0a0a 2020 2020  plans = []..    
-00049ce0: 6465 6620 6765 745f 706c 616e 7328 7365  def get_plans(se
-00049cf0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00049d00: 5265 7475 726e 206c 6973 7420 6f66 2050  Return list of P
-00049d10: 6c61 6e20 6f62 6a65 6374 7320 6173 736f  lan objects asso
-00049d20: 6369 6174 6564 2077 6974 6820 7468 6973  ciated with this
-00049d30: 2073 7472 7563 7475 7265 2073 6574 2e22   structure set."
-00049d40: 2222 0a0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00049d50: 726e 2073 656c 662e 706c 616e 730a 0a20  rn self.plans.. 
-00049d60: 2020 2064 6566 2069 6e74 6572 706f 6c61     def interpola
-00049d70: 7465 5f70 6f69 6e74 7328 7365 6c66 2c20  te_points(self, 
-00049d80: 6e5f 706f 696e 743d 4e6f 6e65 2c20 6478  n_point=None, dx
-00049d90: 793d 4e6f 6e65 2c0a 2020 2020 2020 2020  y=None,.        
-00049da0: 736d 6f6f 7468 6e65 7373 5f70 6572 5f70  smoothness_per_p
-00049db0: 6f69 6e74 3d30 293a 0a20 2020 2020 2020  oint=0):.       
-00049dc0: 2027 2727 0a20 2020 2020 2020 2052 6574   '''.        Ret
-00049dd0: 7572 6e20 6e65 7720 5374 7275 6374 7572  urn new Structur
-00049de0: 6553 6574 206f 626a 6563 742c 2077 6974  eSet object, wit
-00049df0: 6820 696e 7465 7270 6f6c 6174 6564 2063  h interpolated c
-00049e00: 6f6e 746f 7572 2070 6f69 6e74 732e 0a0a  ontour points...
-00049e10: 2020 2020 2020 2020 506f 696e 7473 2061          Points a
-00049e20: 7265 2069 6e74 6572 706f 6c61 7465 6420  re interpolated 
-00049e30: 666f 7220 6561 6368 2063 6f6e 746f 7572  for each contour
-00049e40: 206f 6620 6561 6368 2052 4f49 2e0a 0a20   of each ROI... 
-00049e50: 2020 2020 2020 202a 2a50 6172 616d 6574         **Paramet
-00049e60: 6572 733a 2a2a 0a0a 2020 2020 2020 2020  ers:**..        
-00049e70: 6e5f 706f 696e 7420 3a20 696e 742c 2064  n_point : int, d
-00049e80: 6566 6175 6c74 3d4e 6f6e 650a 2020 2020  efault=None.    
-00049e90: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
-00049ea0: 6620 706f 696e 7473 2070 6572 2063 6f6e  f points per con
-00049eb0: 746f 7572 2c20 6166 7465 7220 696e 7465  tour, after inte
-00049ec0: 7270 6f6c 6174 696f 6e2e 2020 5468 6973  rpolation.  This
-00049ed0: 206d 7573 740a 2020 2020 2020 2020 2020   must.          
-00049ee0: 2020 6265 2073 6574 2074 6f20 4e6f 6e65    be set to None
-00049ef0: 2066 6f72 2064 7879 2074 6f20 6265 2063   for dxy to be c
-00049f00: 6f6e 7369 6465 7265 642e 0a0a 2020 2020  onsidered...    
-00049f10: 2020 2020 6478 7920 3a20 666c 6f61 742c      dxy : float,
-00049f20: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
-00049f30: 2020 2020 2020 2020 2020 4170 7072 6f78            Approx
-00049f40: 696d 6174 6520 6469 7374 616e 6365 2072  imate distance r
-00049f50: 6571 7569 7265 6420 6265 7477 6565 6e20  equired between 
-00049f60: 636f 6e74 6f75 7220 706f 696e 7473 2e20  contour points. 
-00049f70: 2054 6869 7320 6973 2074 616b 656e 0a20   This is taken. 
-00049f80: 2020 2020 2020 2020 2020 2069 6e74 6f20             into 
-00049f90: 6163 636f 756e 7420 6f6e 6c79 2069 6620  account only if 
-00049fa0: 6e5f 706f 696e 7420 6973 2073 6574 2074  n_point is set t
-00049fb0: 6f20 4e6f 6e65 2e20 2046 6f72 2061 2063  o None.  For a c
-00049fc0: 6f6e 746f 7572 206f 660a 2020 2020 2020  ontour of.      
-00049fd0: 2020 2020 2020 6c65 6e67 7468 2063 6f6e        length con
-00049fe0: 746f 7572 5f6c 656e 6774 682c 2074 6865  tour_length, the
-00049ff0: 206e 756d 6265 7220 6f66 2063 6f6e 746f   number of conto
-0004a000: 7572 2070 6f69 6e74 7320 6973 2074 6865  ur points is the
-0004a010: 6e20 7461 6b65 6e0a 2020 2020 2020 2020  n taken.        
-0004a020: 2020 2020 746f 2062 6520 6d61 7828 696e      to be max(in
-0004a030: 7428 636f 6e74 6f75 725f 6c65 6e67 7468  t(contour_length
-0004a040: 202f 2064 7879 292c 2033 292e 2020 0a0a   / dxy), 3).  ..
-0004a050: 2020 2020 2020 2020 736d 6f6f 7468 6e65          smoothne
-0004a060: 7373 5f70 6572 5f70 6f69 6e74 203a 2066  ss_per_point : f
-0004a070: 6c6f 6174 2c20 6465 6661 756c 743d 300a  loat, default=0.
-0004a080: 2020 2020 2020 2020 2020 2020 5061 7261              Para
-0004a090: 6d65 7465 7220 6465 7465 726d 696e 696e  meter determinin
-0004a0a0: 6720 7468 6520 736d 6f6f 7468 6e65 7373  g the smoothness
-0004a0b0: 206f 6620 7468 6520 422d 7370 6c69 6e65   of the B-spline
-0004a0c0: 2063 7572 7665 2075 7365 640a 2020 2020   curve used.    
-0004a0d0: 2020 2020 2020 2020 696e 2063 6f6e 746f          in conto
-0004a0e0: 7572 2061 7070 726f 7869 6d61 7469 6f6e  ur approximation
-0004a0f0: 2066 6f72 2069 6e74 6572 706f 6c61 7469   for interpolati
-0004a100: 6f6e 2e20 2054 6865 2070 726f 6475 6374  on.  The product
-0004a110: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
-0004a120: 736d 6f6f 7468 6e65 7373 5f70 6572 5f70  smoothness_per_p
-0004a130: 6f69 6e74 2061 6e64 2074 6865 206e 756d  oint and the num
-0004a140: 6265 7220 6f66 2063 6f6e 746f 7572 2070  ber of contour p
-0004a150: 6f69 6e74 7320 2873 7065 6369 6669 6564  oints (specified
-0004a160: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-0004a170: 6563 746c 7920 7669 6120 6e5f 706f 696e  ectly via n_poin
-0004a180: 742c 206f 7220 696e 6469 7265 6374 6c79  t, or indirectly
-0004a190: 2076 6961 2064 7879 2920 636f 7272 6573   via dxy) corres
-0004a1a0: 706f 6e64 7320 746f 2074 6865 0a20 2020  ponds to the.   
-0004a1b0: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
-0004a1c0: 6572 2073 206f 6620 7363 6970 792e 696e  er s of scipy.in
-0004a1d0: 7465 7270 6f6c 6174 652e 7370 6c70 7265  terpolate.splpre
-0004a1e0: 7020 2d20 7365 6520 646f 6375 6d65 6e74  p - see document
-0004a1f0: 6174 696f 6e20 6174 3a0a 2020 2020 2020  ation at:.      
-0004a200: 2020 0a20 2020 2020 2020 2020 2020 2068    .            h
-0004a210: 7474 7073 3a2f 2f73 6369 7079 2e67 6974  ttps://scipy.git
-0004a220: 6875 622e 696f 2f64 6576 646f 6373 2f72  hub.io/devdocs/r
-0004a230: 6566 6572 656e 6365 2f67 656e 6572 6174  eference/generat
-0004a240: 6564 2f73 6369 7079 2e69 6e74 6572 706f  ed/scipy.interpo
-0004a250: 6c61 7465 2e73 706c 7072 6570 2e68 746d  late.splprep.htm
-0004a260: 6c23 7363 6970 792e 696e 7465 7270 6f6c  l#scipy.interpol
-0004a270: 6174 652e 7370 6c70 7265 700a 0a20 2020  ate.splprep..   
-0004a280: 2020 2020 2020 2020 2041 2073 6d6f 6f74           A smoot
-0004a290: 686e 6573 735f 7065 725f 706f 696e 7420  hness_per_point 
-0004a2a0: 6f66 2030 2066 6f72 6365 7320 7468 6520  of 0 forces the 
-0004a2b0: 422d 7370 6c69 6e65 2074 6f20 7061 7373  B-spline to pass
-0004a2c0: 2074 6872 6f75 6768 0a20 2020 2020 2020   through.       
-0004a2d0: 2020 2020 2061 6c6c 206f 6620 7468 6520       all of the 
-0004a2e0: 7072 652d 696e 7465 7270 6f6c 6174 696f  pre-interpolatio
-0004a2f0: 6e20 636f 6e74 6f75 7220 706f 696e 7473  n contour points
-0004a300: 2e0a 2020 2020 2020 2020 2727 270a 0a20  ..        '''.. 
-0004a310: 2020 2020 2020 2023 2049 6e74 6572 706f         # Interpo
-0004a320: 6c61 7465 2070 6f69 6e74 7320 666f 7220  late points for 
-0004a330: 7468 6520 726f 6973 0a20 2020 2020 2020  the rois.       
-0004a340: 2072 6f69 7320 3d20 5b5d 0a20 2020 2020   rois = [].     
-0004a350: 2020 2066 6f72 2072 6f69 2069 6e20 7365     for roi in se
-0004a360: 6c66 2e67 6574 5f72 6f69 7328 293a 0a20  lf.get_rois():. 
-0004a370: 2020 2020 2020 2020 2020 2072 6f69 732e             rois.
-0004a380: 6170 7065 6e64 2872 6f69 2e69 6e74 6572  append(roi.inter
-0004a390: 706f 6c61 7465 5f70 6f69 6e74 7328 0a20  polate_points(. 
-0004a3a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0004a3b0: 5f70 6f69 6e74 2c20 6478 792c 2073 6d6f  _point, dxy, smo
-0004a3c0: 6f74 686e 6573 735f 7065 725f 706f 696e  othness_per_poin
-0004a3d0: 7429 290a 0a20 2020 2020 2020 2023 2043  t))..        # C
-0004a3e0: 6c6f 6e65 2073 656c 662c 2074 6865 6e20  lone self, then 
-0004a3f0: 7265 7365 7420 736f 7572 6365 2061 6e64  reset source and
-0004a400: 2072 6f69 730a 2020 2020 2020 2020 7373   rois.        ss
-0004a410: 203d 2053 7472 7563 7475 7265 5365 7428   = StructureSet(
-0004a420: 7365 6c66 290a 2020 2020 2020 2020 7373  self).        ss
-0004a430: 2e73 6f75 7263 6573 203d 2072 6f69 730a  .sources = rois.
-0004a440: 2020 2020 2020 2020 7373 2e72 6f69 7320          ss.rois 
-0004a450: 3d20 726f 6973 0a0a 2020 2020 2020 2020  = rois..        
-0004a460: 7265 7475 726e 2073 730a 0a20 2020 2064  return ss..    d
-0004a470: 6566 206f 7264 6572 5f72 6f69 7328 7365  ef order_rois(se
-0004a480: 6c66 2c20 6f72 6465 723d 2778 2b27 293a  lf, order='x+'):
-0004a490: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-0004a4a0: 2020 2020 204f 7264 6572 2052 4f49 7320       Order ROIs 
-0004a4b0: 6279 206f 6e65 206f 6620 7468 6569 7220  by one of their 
-0004a4c0: 6365 6e74 726f 6964 2063 6f6f 7264 696e  centroid coordin
-0004a4d0: 6174 6573 2e0a 0a20 2020 2020 2020 202a  ates...        *
-0004a4e0: 2a50 6172 616d 6574 6572 3a2a 2a0a 0a20  *Parameter:**.. 
-0004a4f0: 2020 2020 2020 206f 7264 6572 203a 2073         order : s
-0004a500: 7472 2c20 6465 6661 756c 743d 2778 2b27  tr, default='x+'
-0004a510: 0a20 2020 2020 2020 2020 2020 2053 7065  .            Spe
-0004a520: 6369 6669 6361 7469 6f6e 206f 6620 7761  cification of wa
-0004a530: 7920 6974 2077 6869 6368 2052 4f49 7320  y it which ROIs 
-0004a540: 6172 6520 746f 2062 6520 6f72 6465 7264  are to be orderd
-0004a550: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
-0004a560: 2778 2b27 203a 2069 6e20 6f72 6465 7220  'x+' : in order 
-0004a570: 6f66 2069 6e63 7265 6173 696e 6720 7820  of increasing x 
-0004a580: 7661 6c75 652e 0a20 2020 2020 2020 2020  value..         
-0004a590: 2020 202d 2027 782d 2720 3a20 696e 206f     - 'x-' : in o
-0004a5a0: 7264 6572 206f 6620 6465 6372 6561 7369  rder of decreasi
-0004a5b0: 6e67 2078 2076 616c 7565 2e0a 2020 2020  ng x value..    
-0004a5c0: 2020 2020 2020 2020 2d20 2779 2b27 203a          - 'y+' :
-0004a5d0: 2069 6e20 6f72 6465 7220 6f66 2069 6e63   in order of inc
-0004a5e0: 7265 6173 696e 6720 7920 7661 6c75 652e  reasing y value.
-0004a5f0: 0a20 2020 2020 2020 2020 2020 202d 2027  .            - '
-0004a600: 792d 2720 3a20 696e 206f 7264 6572 206f  y-' : in order o
-0004a610: 6620 6465 6372 6561 7369 6e67 2079 2076  f decreasing y v
-0004a620: 616c 7565 2e0a 2020 2020 2020 2020 2020  alue..          
-0004a630: 2020 2d20 277a 2b27 203a 2069 6e20 6f72    - 'z+' : in or
-0004a640: 6465 7220 6f66 2069 6e63 7265 6173 696e  der of increasin
-0004a650: 6720 7a20 7661 6c75 652e 0a20 2020 2020  g z value..     
-0004a660: 2020 2020 2020 202d 2027 7a2d 2720 3a20         - 'z-' : 
-0004a670: 696e 206f 7264 6572 206f 6620 6465 6372  in order of decr
-0004a680: 6561 7369 6e67 207a 2076 616c 7565 2e0a  easing z value..
-0004a690: 2020 2020 2020 2020 2727 270a 0a20 2020          '''..   
-0004a6a0: 2020 2020 2069 6620 6f72 6465 7220 6e6f       if order no
-0004a6b0: 7420 696e 205b 2778 2b27 2c20 2778 2d27  t in ['x+', 'x-'
-0004a6c0: 2c20 2779 2b27 2c20 2779 2d27 2c20 277a  , 'y+', 'y-', 'z
-0004a6d0: 2b27 2c20 277a 2d27 5d3a 0a20 2020 2020  +', 'z-']:.     
-0004a6e0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-0004a6f0: 2020 2020 2020 2023 2044 6574 6572 6d69         # Determi
-0004a700: 6e65 2061 7869 7320 666f 7220 6f72 6465  ne axis for orde
-0004a710: 7269 6e67 2c20 616e 6420 6469 7265 6374  ring, and direct
-0004a720: 696f 6e2e 0a20 2020 2020 2020 2061 7869  ion..        axi
-0004a730: 7320 3d20 2778 797a 272e 6669 6e64 286f  s = 'xyz'.find(o
-0004a740: 7264 6572 5b30 5d29 0a20 2020 2020 2020  rder[0]).       
-0004a750: 2072 6576 6572 7365 203d 2028 272d 2720   reverse = ('-' 
-0004a760: 696e 206f 7264 6572 290a 0a20 2020 2020  in order)..     
-0004a770: 2020 2023 2043 7265 6174 6520 6469 6374     # Create dict
-0004a780: 696f 6e61 7279 2077 6865 7265 206b 6579  ionary where key
-0004a790: 7320 6172 6520 6365 6e74 726f 6964 2063  s are centroid c
-0004a7a0: 6f6f 7264 696e 6174 6573 0a20 2020 2020  oordinates.     
-0004a7b0: 2020 2023 2061 6e64 2076 616c 7565 7320     # and values 
-0004a7c0: 6172 6520 6c69 7374 7320 6f66 2052 4f49  are lists of ROI
-0004a7d0: 2069 6e64 6963 6965 7320 6174 2074 6865   indicies at the
-0004a7e0: 7365 2063 6f6f 7264 696e 6174 6573 2e0a  se coordinates..
-0004a7f0: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
-0004a800: 7320 3d20 7b7d 0a20 2020 2020 2020 2066  s = {}.        f
-0004a810: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-0004a820: 6e28 7365 6c66 2e72 6f69 7329 293a 0a20  n(self.rois)):. 
-0004a830: 2020 2020 2020 2020 2020 2078 797a 203d             xyz =
-0004a840: 2073 656c 662e 726f 6973 5b69 5d2e 6765   self.rois[i].ge
-0004a850: 745f 6365 6e74 726f 6964 2829 5b61 7869  t_centroid()[axi
-0004a860: 735d 0a20 2020 2020 2020 2020 2020 2069  s].            i
-0004a870: 6620 7879 7a20 6e6f 7420 696e 2063 656e  f xyz not in cen
-0004a880: 7472 6f69 6473 3a0a 2020 2020 2020 2020  troids:.        
-0004a890: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
-0004a8a0: 735b 7879 7a5d 203d 205b 5d0a 2020 2020  s[xyz] = [].    
-0004a8b0: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
-0004a8c0: 735b 7879 7a5d 2e61 7070 656e 6428 6929  s[xyz].append(i)
-0004a8d0: 0a0a 2020 2020 2020 2020 2320 4372 6561  ..        # Crea
-0004a8e0: 7465 206c 6973 7420 6f66 2052 4f49 7320  te list of ROIs 
-0004a8f0: 6f72 6465 7265 6420 6279 2063 656e 7472  ordered by centr
-0004a900: 6f69 6420 636f 6f72 6469 6e61 7465 2e0a  oid coordinate..
-0004a910: 2020 2020 2020 2020 726f 6973 203d 205b          rois = [
-0004a920: 5d0a 2020 2020 2020 2020 666f 7220 6365  ].        for ce
-0004a930: 6e74 726f 6964 2069 6e20 736f 7274 6564  ntroid in sorted
-0004a940: 2863 656e 7472 6f69 6473 2c20 7265 7665  (centroids, reve
-0004a950: 7273 653d 7265 7665 7273 6529 3a0a 2020  rse=reverse):.  
-0004a960: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
-0004a970: 696e 2063 656e 7472 6f69 6473 5b63 656e  in centroids[cen
-0004a980: 7472 6f69 645d 3a0a 2020 2020 2020 2020  troid]:.        
-0004a990: 2020 2020 2020 2020 726f 6973 2e61 7070          rois.app
-0004a9a0: 656e 6428 7365 6c66 2e72 6f69 735b 695d  end(self.rois[i]
-0004a9b0: 290a 0a20 2020 2020 2020 2023 2053 746f  )..        # Sto
-0004a9c0: 7265 2074 6865 206e 6577 206f 7264 6572  re the new order
-0004a9d0: 206f 6620 524f 4973 2e0a 2020 2020 2020   of ROIs..      
-0004a9e0: 2020 7365 6c66 2e72 6f69 7320 3d20 726f    self.rois = ro
-0004a9f0: 6973 0a0a 2020 2020 6465 6620 636f 6d62  is..    def comb
-0004aa00: 696e 655f 726f 6973 2873 656c 662c 206e  ine_rois(self, n
-0004aa10: 616d 653d 4e6f 6e65 2c20 726f 695f 6e61  ame=None, roi_na
-0004aa20: 6d65 733d 4e6f 6e65 2c20 696d 6167 653d  mes=None, image=
-0004aa30: 4e6f 6e65 2c20 6d65 7468 6f64 3d4e 6f6e  None, method=Non
-0004aa40: 6529 3a0a 2020 2020 2020 2020 2727 270a  e):.        '''.
-0004aa50: 2020 2020 2020 2020 436f 6d62 696e 6520          Combine 
-0004aa60: 7477 6f20 6f72 206d 6f72 6520 524f 4973  two or more ROIs
-0004aa70: 2061 7320 6120 7369 6e67 6c65 2052 4f49   as a single ROI
-0004aa80: 2e0a 0a20 2020 2020 2020 202a 2a50 6172  ...        **Par
-0004aa90: 616d 6574 6572 733a 2a2a 0a0a 2020 2020  ameters:**..    
-0004aaa0: 2020 2020 6e61 6d65 203a 2073 7472 2c20      name : str, 
-0004aab0: 6465 6661 756c 743d 4e6f 6e65 0a20 2020  default=None.   
-0004aac0: 2020 2020 2020 2020 204e 616d 6520 746f           Name to
-0004aad0: 2062 6520 6769 7665 6e20 746f 2074 6865   be given to the
-0004aae0: 2063 6f6d 706f 7369 7465 2052 4f49 2e20   composite ROI. 
-0004aaf0: 2049 6620 4e6f 6e65 2c20 7468 650a 2020   If None, the.  
-0004ab00: 2020 2020 2020 2020 2020 6e61 6d65 2061            name a
-0004ab10: 7373 6967 6e65 6420 6973 2066 6f72 6d65  ssigned is forme
-0004ab20: 6420 6279 206a 6f69 6e69 6e67 2074 6f67  d by joining tog
-0004ab30: 6574 6865 7220 7468 6520 6e61 6d65 730a  ether the names.
-0004ab40: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
-0004ab50: 6865 206f 7269 6769 6e61 6c20 524f 4973  he original ROIs
-0004ab60: 2e0a 0a20 2020 2020 2020 2072 6f69 5f6e  ...        roi_n
-0004ab70: 616d 6573 203a 206c 6973 742c 2064 6566  ames : list, def
-0004ab80: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
-0004ab90: 2020 2020 2020 4c69 7374 206f 6620 6e61        List of na
-0004aba0: 6d65 7320 6f66 2052 4f49 7320 746f 2062  mes of ROIs to b
-0004abb0: 6520 636f 6d62 696e 6564 2e20 2049 6620  e combined.  If 
-0004abc0: 4e6f 6e65 2c20 616c 6c20 6f66 2074 6865  None, all of the
-0004abd0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-0004abe0: 7563 7475 7265 2073 6574 2773 2052 4f49  ucture set's ROI
-0004abf0: 7320 6172 6520 636f 6d62 696e 6564 2e0a  s are combined..
-0004ac00: 0a20 2020 2020 2020 2069 6d61 6765 203a  .        image :
-0004ac10: 2073 6b72 742e 696d 6167 652e 496d 6167   skrt.image.Imag
-0004ac20: 652c 2064 6566 6175 6c74 3d4e 6f6e 650a  e, default=None.
-0004ac30: 2020 2020 2020 2020 2020 2020 496d 6167              Imag
-0004ac40: 6520 746f 2073 6574 2066 6f72 2074 6865  e to set for the
-0004ac50: 2063 6f6d 706f 7369 7465 2052 4f49 2e20   composite ROI. 
-0004ac60: 2049 6620 4e6f 6e65 2c20 7573 6520 7468   If None, use th
-0004ac70: 6520 696d 6167 650a 2020 2020 2020 2020  e image.        
-0004ac80: 2020 2020 6f66 2074 6865 2052 4f49 2077      of the ROI w
-0004ac90: 6974 6820 7468 6520 6669 7273 7420 696e  ith the first in
-0004aca0: 203c 726f 695f 6e61 6d65 733e 2e0a 0a20   <roi_names>... 
-0004acb0: 2020 2020 2020 206d 6574 686f 6420 3a20         method : 
-0004acc0: 7374 722c 2064 6566 6175 6c74 3d4e 6f6e  str, default=Non
-0004acd0: 650a 2020 2020 2020 2020 2020 2020 4d65  e.            Me
-0004ace0: 7468 6f64 2074 6f20 7573 6520 666f 7220  thod to use for 
-0004acf0: 636f 6d62 696e 696e 6720 524f 4973 2e20  combining ROIs. 
-0004ad00: 2043 616e 2062 653a 200a 0a20 2020 2020   Can be: ..     
-0004ad10: 2020 2020 2020 2020 2020 202d 2022 636f             - "co
-0004ad20: 6e74 6f75 7222 3a20 7461 6b65 2075 6e61  ntour": take una
-0004ad30: 7279 2075 6e69 6f6e 206f 6620 7368 6170  ry union of shap
-0004ad40: 656c 7920 706f 6c79 676f 6e73 2e0a 2020  ely polygons..  
-0004ad50: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-0004ad60: 226d 6173 6b22 3a20 7375 6d20 6269 6e61  "mask": sum bina
-0004ad70: 7279 206d 6173 6b73 2e0a 2020 2020 2020  ry masks..      
-0004ad80: 2020 2020 2020 2020 2020 2d20 2261 7574            - "aut
-0004ad90: 6f22 3a20 7573 6520 7468 6520 6465 6661  o": use the defa
-0004ada0: 756c 745f 6765 6f6d 5f6d 6574 686f 6420  ult_geom_method 
-0004adb0: 6f66 2074 6865 2052 4f49 2077 6974 6820  of the ROI with 
-0004adc0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-0004add0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0004ade0: 7273 7420 6e61 6d65 2069 6e20 3c72 6f69  rst name in <roi
-0004adf0: 5f6e 616d 6573 3e2e 0a0a 2020 2020 2020  _names>...      
-0004ae00: 2020 2020 2020 4966 204e 6f6e 652c 2022        If None, "
-0004ae10: 6175 746f 2220 6973 2075 7365 642e 0a20  auto" is used.. 
-0004ae20: 2020 2020 2020 2027 2727 0a0a 2020 2020         '''..    
-0004ae30: 2020 2020 2320 4966 204e 6f6e 6520 7661      # If None va
-0004ae40: 6c75 6573 2070 6173 7365 642c 2073 6574  lues passed, set
-0004ae50: 2064 6566 6175 6c74 2062 6568 6176 696f   default behavio
-0004ae60: 7572 2e0a 2020 2020 2020 2020 6966 2072  ur..        if r
-0004ae70: 6f69 5f6e 616d 6573 2069 7320 4e6f 6e65  oi_names is None
-0004ae80: 3a0a 2020 2020 2020 2020 2020 2020 726f  :.            ro
-0004ae90: 695f 6e61 6d65 7320 3d20 7365 6c66 2e67  i_names = self.g
-0004aea0: 6574 5f72 6f69 5f6e 616d 6573 2829 0a20  et_roi_names(). 
-0004aeb0: 2020 2020 2020 2069 6620 6e61 6d65 2069         if name i
-0004aec0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0004aed0: 2020 2020 6e61 6d65 203d 2027 2b27 2e6a      name = '+'.j
-0004aee0: 6f69 6e28 726f 695f 6e61 6d65 7329 0a20  oin(roi_names). 
-0004aef0: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
-0004af00: 2069 6e20 5b4e 6f6e 652c 2022 6175 746f   in [None, "auto
-0004af10: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0004af20: 6d65 7468 6f64 203d 2073 656c 665b 726f  method = self[ro
-0004af30: 695f 6e61 6d65 735b 305d 5d2e 6465 6661  i_names[0]].defa
-0004af40: 756c 745f 6765 6f6d 5f6d 6574 686f 640a  ult_geom_method.
-0004af50: 2020 2020 2020 2020 6966 2069 6d61 6765          if image
-0004af60: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0004af70: 2020 2020 2020 696d 6167 6520 3d20 7365        image = se
-0004af80: 6c66 5b72 6f69 5f6e 616d 6573 5b30 5d5d  lf[roi_names[0]]
-0004af90: 2e69 6d61 6765 0a0a 2020 2020 2020 2020  .image..        
-0004afa0: 6966 2022 636f 6e74 6f75 7222 203d 3d20  if "contour" == 
-0004afb0: 6d65 7468 6f64 3a0a 2020 2020 2020 2020  method:.        
-0004afc0: 2020 2020 2320 4372 6561 7465 2061 2064      # Create a d
-0004afd0: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
-0004afe0: 6e69 6e67 2070 6f6c 7967 6f6e 7320 666f  ning polygons fo
-0004aff0: 7220 616c 6c20 524f 4973 2e0a 2020 2020  r all ROIs..    
-0004b000: 2020 2020 2020 2020 616c 6c5f 706f 6c79          all_poly
-0004b010: 676f 6e73 203d 207b 7d0a 2020 2020 2020  gons = {}.      
-0004b020: 2020 2020 2020 666f 7220 726f 6920 696e        for roi in
-0004b030: 2073 656c 662e 6765 745f 726f 6973 2872   self.get_rois(r
-0004b040: 6f69 5f6e 616d 6573 293a 0a20 2020 2020  oi_names):.     
-0004b050: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0004b060: 6579 2c20 706f 6c79 676f 6e73 2069 6e20  ey, polygons in 
-0004b070: 726f 692e 6765 745f 706f 6c79 676f 6e73  roi.get_polygons
-0004b080: 2829 2e69 7465 6d73 2829 3a0a 2020 2020  ().items():.    
-0004b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004b0a0: 6966 206e 6f74 206b 6579 2069 6e20 616c  if not key in al
-0004b0b0: 6c5f 706f 6c79 676f 6e73 3a0a 2020 2020  l_polygons:.    
+00046000: 666f 7220 726f 6920 696e 2073 7472 7563  for roi in struc
+00046010: 7475 7265 5f73 6574 5f74 6d70 2e72 6f69  ture_set_tmp.roi
+00046020: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00046030: 2020 2020 2020 2069 6620 726f 692e 636f         if roi.co
+00046040: 6e74 6f75 7273 5f6f 6e6c 793a 0a20 2020  ntours_only:.   
+00046050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00046060: 2020 2020 2072 6f69 2e73 6574 5f69 6d61       roi.set_ima
+00046070: 6765 2869 6d29 0a20 2020 2020 2020 2020  ge(im).         
+00046080: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00046090: 2020 2020 2020 2020 2069 6d20 3d20 736b           im = sk
+000460a0: 7274 2e69 6d61 6765 2e49 6d61 6765 280a  rt.image.Image(.
+000460b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000460c0: 2020 2020 6e70 2e6f 6e65 7328 7365 6c66      np.ones(self
+000460d0: 2e72 6f69 735b 305d 2e73 6861 7065 2920  .rois[0].shape) 
+000460e0: 2a20 3165 342c 0a20 2020 2020 2020 2020  * 1e4,.         
+000460f0: 2020 2020 2020 2020 2020 2061 6666 696e             affin
+00046100: 653d 7365 6c66 2e72 6f69 735b 305d 2e61  e=self.rois[0].a
+00046110: 6666 696e 652c 0a20 2020 2020 2020 2020  ffine,.         
+00046120: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00046130: 2020 2020 2020 6966 2072 6f69 7320 6973        if rois is
+00046140: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00046150: 2020 2020 2020 2072 6f69 7320 3d20 7374         rois = st
+00046160: 7275 6374 7572 655f 7365 745f 746d 700a  ructure_set_tmp.
+00046170: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00046180: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00046190: 2020 6966 2073 6b72 742e 636f 7265 2e69    if skrt.core.i
+000461a0: 735f 6c69 7374 2872 6f69 7329 3a0a 2020  s_list(rois):.  
+000461b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000461c0: 2020 726f 6973 203d 205b 7374 7275 6374    rois = [struct
+000461d0: 7572 655f 7365 745f 746d 705d 202b 2072  ure_set_tmp] + r
+000461e0: 6f69 730a 2020 2020 2020 2020 2020 2020  ois.            
+000461f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00046200: 2020 2020 2020 2020 2020 2020 2020 726f                ro
+00046210: 6973 203d 205b 7374 7275 6374 7572 655f  is = [structure_
+00046220: 7365 745f 746d 702c 2072 6f69 735d 0a20  set_tmp, rois]. 
+00046230: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00046240: 735b 2273 686f 7722 5d20 3d20 4661 6c73  s["show"] = Fals
+00046250: 650a 2020 2020 2020 2020 2020 2020 6276  e.            bv
+00046260: 203d 2042 6574 7465 7256 6965 7765 7228   = BetterViewer(
+00046270: 696d 2c20 726f 6973 3d72 6f69 732c 202a  im, rois=rois, *
+00046280: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+00046290: 2020 2020 2062 762e 6d61 6b65 5f75 6928       bv.make_ui(
+000462a0: 6e6f 5f69 6e74 656e 7369 7479 3d54 7275  no_intensity=Tru
+000462b0: 6529 0a20 2020 2020 2020 2020 2020 2062  e).            b
+000462c0: 762e 7368 6f77 2829 0a0a 2020 2020 2020  v.show()..      
+000462d0: 2020 7265 7475 726e 2062 760a 0a20 2020    return bv..   
+000462e0: 2064 6566 2067 6574 5f65 7874 656e 7428   def get_extent(
+000462f0: 7365 6c66 2c20 2a2a 6b77 6172 6773 293a  self, **kwargs):
+00046300: 0a20 2020 2020 2020 2022 2222 4765 7420  .        """Get 
+00046310: 6d69 6e20 616e 6420 6d61 7820 6578 7465  min and max exte
+00046320: 6e74 206f 6620 616c 6c20 524f 4973 2069  nt of all ROIs i
+00046330: 6e20 7468 6520 5374 7275 6374 7572 6553  n the StructureS
+00046340: 6574 2e22 2222 0a0a 2020 2020 2020 2020  et."""..        
+00046350: 616c 6c5f 6578 7465 6e74 7320 3d20 5b5d  all_extents = []
+00046360: 0a20 2020 2020 2020 2066 6f72 2072 6f69  .        for roi
+00046370: 2069 6e20 7365 6c66 2e67 6574 5f72 6f69   in self.get_roi
+00046380: 7328 6967 6e6f 7265 5f65 6d70 7479 3d54  s(ignore_empty=T
+00046390: 7275 6529 3a0a 2020 2020 2020 2020 2020  rue):.          
+000463a0: 2020 616c 6c5f 6578 7465 6e74 732e 6578    all_extents.ex
+000463b0: 7465 6e64 2872 6f69 2e67 6574 5f65 7874  tend(roi.get_ext
+000463c0: 656e 7428 2a2a 6b77 6172 6773 2929 0a20  ent(**kwargs)). 
+000463d0: 2020 2020 2020 2072 6574 7572 6e20 6d69         return mi
+000463e0: 6e28 616c 6c5f 6578 7465 6e74 7329 2c20  n(all_extents), 
+000463f0: 6d61 7828 616c 6c5f 6578 7465 6e74 7329  max(all_extents)
+00046400: 0a0a 2020 2020 6465 6620 6765 745f 6578  ..    def get_ex
+00046410: 7465 6e74 7328 7365 6c66 2c20 726f 695f  tents(self, roi_
+00046420: 6e61 6d65 733d 4e6f 6e65 2c20 6275 6666  names=None, buff
+00046430: 6572 3d4e 6f6e 652c 2062 7566 6665 725f  er=None, buffer_
+00046440: 756e 6974 733d 226d 6d22 2c0a 2020 2020  units="mm",.    
+00046450: 2020 2020 2020 2020 6d65 7468 6f64 3d4e          method=N
+00046460: 6f6e 652c 206f 7269 6769 6e3d 4e6f 6e65  one, origin=None
+00046470: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00046480: 2020 2020 2020 2047 6574 206d 696e 696d         Get minim
+00046490: 756d 2061 6e64 206d 6178 696d 756d 2065  um and maximum e
+000464a0: 7874 656e 7420 6f66 2053 7472 7563 7475  xtent of Structu
+000464b0: 7265 5365 7420 524f 4973 2c0a 2020 2020  reSet ROIs,.    
+000464c0: 2020 2020 696e 206d 6d20 616c 6f6e 6720      in mm along 
+000464d0: 616c 6c20 7468 7265 6520 6178 6573 2c20  all three axes, 
+000464e0: 7265 7475 726e 6564 2069 6e20 6f72 6465  returned in orde
+000464f0: 7220 5b78 2c20 792c 207a 5d2e 0a20 2020  r [x, y, z]..   
+00046500: 2020 2020 204f 7074 696f 6e61 6c6c 7920       Optionally 
+00046510: 6170 706c 7920 6120 6275 6666 6572 2074  apply a buffer t
+00046520: 6f20 7468 6520 6578 7465 6e74 7320 7375  o the extents su
+00046530: 6368 2074 6861 7420 7468 6579 2063 6f76  ch that they cov
+00046540: 6572 0a20 2020 2020 2020 206d 6f72 6520  er.        more 
+00046550: 7468 616e 2074 6865 2072 6567 696f 6e20  than the region 
+00046560: 6f66 2074 6865 2052 4f49 732e 0a0a 2020  of the ROIs...  
+00046570: 2020 2020 2020 2a2a 5061 7261 6d65 7465        **Paramete
+00046580: 7273 3a2a 2a0a 0a20 2020 2020 2020 2072  rs:**..        r
+00046590: 6f69 5f6e 616d 6573 203a 206c 6973 742c  oi_names : list,
+000465a0: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
+000465b0: 2020 2020 2020 2020 2020 4c69 7374 206f            List o
+000465c0: 6620 6e61 6d65 7320 6f66 2052 4f49 7320  f names of ROIs 
+000465d0: 746f 2062 6520 636f 6e73 6964 6572 6564  to be considered
+000465e0: 2e20 2049 6620 4e6f 6e65 2c20 616c 6c20  .  If None, all 
+000465f0: 6f66 2074 6865 0a20 2020 2020 2020 2020  of the.         
+00046600: 2020 2073 7472 7563 7475 7265 2073 6574     structure set
+00046610: 2773 2052 4f49 7320 6172 6520 636f 6e73  's ROIs are cons
+00046620: 6964 6572 6564 2e0a 0a20 2020 2020 2020  idered...       
+00046630: 2062 7566 6665 7220 3a20 666c 6f61 742c   buffer : float,
+00046640: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
+00046650: 2020 2020 2020 2020 2020 4f70 7469 6f6e            Option
+00046660: 616c 2062 7566 6665 7220 746f 2061 6464  al buffer to add
+00046670: 2074 6f20 7468 6520 6578 7465 6e74 732e   to the extents.
+00046680: 2055 6e69 7473 2073 6574 2062 7920 6062   Units set by `b
+00046690: 7566 6665 725f 756e 6974 7360 2e0a 0a20  uffer_units`... 
+000466a0: 2020 2020 2020 2062 7566 6665 725f 756e         buffer_un
+000466b0: 6974 7320 3a20 7374 722c 2064 6566 6175  its : str, defau
+000466c0: 6c74 3d22 6d6d 220a 2020 2020 2020 2020  lt="mm".        
+000466d0: 2020 2020 556e 6974 7320 666f 7220 6275      Units for bu
+000466e0: 6666 6572 2c20 6966 2075 7369 6e67 2e20  ffer, if using. 
+000466f0: 4361 6e20 6265 2022 6d6d 222c 2022 766f  Can be "mm", "vo
+00046700: 7865 6c73 222c 206f 7220 2266 7261 6322  xels", or "frac"
+00046710: 2028 7768 6963 680a 2020 2020 2020 2020   (which.        
+00046720: 2020 2020 6170 706c 6965 7320 6275 6666      applies buff
+00046730: 6572 2061 7320 6120 6672 6163 7469 6f6e  er as a fraction
+00046740: 206f 6620 746f 7461 6c20 6c65 6e67 7468   of total length
+00046750: 2069 6e20 6561 6368 2064 696d 656e 7369   in each dimensi
+00046760: 6f6e 292e 0a0a 2020 2020 2020 2020 6d65  on)...        me
+00046770: 7468 6f64 203a 2073 7472 2c20 6465 6661  thod : str, defa
+00046780: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
+00046790: 2020 2020 204d 6574 686f 6420 746f 2075       Method to u
+000467a0: 7365 2066 6f72 2065 7874 656e 7420 6361  se for extent ca
+000467b0: 6c63 756c 6174 696f 6e2e 2043 616e 2062  lculation. Can b
+000467c0: 653a 200a 0a20 2020 2020 2020 2020 2020  e: ..           
+000467d0: 2020 2020 202a 2022 636f 6e74 6f75 7222       * "contour"
+000467e0: 3a20 6765 7420 6578 7465 6e74 2066 726f  : get extent fro
+000467f0: 6d20 6d69 6e2f 6d61 7820 706f 7369 7469  m min/max positi
+00046800: 6f6e 7320 6f66 2063 6f6e 746f 7572 2873  ons of contour(s
+00046810: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+00046820: 2020 202a 2022 6d61 736b 223a 2067 6574     * "mask": get
+00046830: 2065 7874 656e 7420 6672 6f6d 206d 696e   extent from min
+00046840: 2f6d 6178 2070 6f73 6974 696f 6e73 206f  /max positions o
+00046850: 6620 766f 7865 6c73 2069 6e20 7468 6520  f voxels in the 
+00046860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00046870: 2020 2062 696e 6172 7920 6d61 736b 2e0a     binary mask..
+00046880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00046890: 2a20 4e6f 6e65 3a20 7573 6520 7468 6520  * None: use the 
+000468a0: 6d65 7468 6f64 2073 6574 2069 6e20 7365  method set in se
+000468b0: 6c66 2e64 6566 6175 6c74 5f67 656f 6d5f  lf.default_geom_
+000468c0: 6d65 7468 6f64 2e0a 0a20 2020 2020 2020  method...       
+000468d0: 206f 7269 6769 6e20 3a20 7475 706c 652c   origin : tuple,
+000468e0: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
+000468f0: 2020 2020 2020 2020 2020 5475 706c 6520            Tuple 
+00046900: 7370 6563 6966 7969 6e67 2074 6865 2028  specifying the (
+00046910: 782c 2079 2c20 7a29 2063 6f6f 7264 696e  x, y, z) coordin
+00046920: 6174 6573 206f 6620 7468 6520 706f 696e  ates of the poin
+00046930: 740a 2020 2020 2020 2020 2020 2020 7769  t.            wi
+00046940: 7468 2072 6573 7065 6374 2074 6f20 7768  th respect to wh
+00046950: 6963 6820 6578 7465 6e74 7320 6172 6520  ich extents are 
+00046960: 746f 2062 6520 6465 7465 726d 696e 6564  to be determined
+00046970: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00046980: 204e 6f6e 652c 2074 6865 6e20 2830 2c20   None, then (0, 
+00046990: 302c 2030 2920 6973 2075 7365 642e 0a20  0, 0) is used.. 
+000469a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000469b0: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
+000469c0: 6f6d 6269 6e65 5f72 6f69 7328 726f 695f  ombine_rois(roi_
+000469d0: 6e61 6d65 7329 2e67 6574 5f65 7874 656e  names).get_exten
+000469e0: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
+000469f0: 2020 2020 6275 6666 6572 2c20 6275 6666      buffer, buff
+00046a00: 6572 5f75 6e69 7473 2c20 6d65 7468 6f64  er_units, method
+00046a10: 2c20 6f72 6967 696e 290a 0a20 2020 2064  , origin)..    d
+00046a20: 6566 2067 6574 5f63 726f 705f 6c69 6d69  ef get_crop_limi
+00046a30: 7473 2873 656c 662c 2072 6f69 5f6e 616d  ts(self, roi_nam
+00046a40: 6573 3d4e 6f6e 652c 2063 726f 705f 6d61  es=None, crop_ma
+00046a50: 7267 696e 733d 4e6f 6e65 2c20 6d65 7468  rgins=None, meth
+00046a60: 6f64 3d4e 6f6e 6529 3a0a 2020 2020 2020  od=None):.      
+00046a70: 2020 2222 220a 2020 2020 2020 2020 4765    """.        Ge
+00046a80: 7420 6372 6f70 206c 696d 6974 7320 636f  t crop limits co
+00046a90: 7272 6573 706f 6e64 696e 6720 746f 2053  rresponding to S
+00046aa0: 7472 7563 7475 7265 5365 7420 524f 4920  tructureSet ROI 
+00046ab0: 6578 7465 6e74 7320 706c 7573 206d 6172  extents plus mar
+00046ac0: 6769 6e73 2e0a 0a20 2020 2020 2020 2054  gins...        T
+00046ad0: 6865 2074 7570 6c65 7320 6f66 206c 696d  he tuples of lim
+00046ae0: 6974 7320 7265 7475 726e 6564 2c20 696e  its returned, in
+00046af0: 2074 6865 206f 7264 6572 2028 782c 2079   the order (x, y
+00046b00: 2c20 7a29 2063 616e 0a20 2020 2020 2020  , z) can.       
+00046b10: 2062 6520 7573 6564 2c20 666f 7220 6578   be used, for ex
+00046b20: 616d 706c 652c 2061 7320 696e 7075 7473  ample, as inputs
+00046b30: 2074 6f20 736b 7274 2e69 6d61 6765 2e49   to skrt.image.I
+00046b40: 6d61 6765 2e63 726f 7028 292e 0a0a 2020  mage.crop()...  
+00046b50: 2020 2020 2020 5468 6973 206d 6574 686f        This metho
+00046b60: 6420 6973 2073 696d 696c 6172 2074 6f20  d is similar to 
+00046b70: 7468 6520 6d65 7468 6f64 2067 6574 5f65  the method get_e
+00046b80: 7874 656e 7473 2829 2c20 6275 7420 616c  xtents(), but al
+00046b90: 6c6f 7773 0a20 2020 2020 2020 2064 6966  lows.        dif
+00046ba0: 6665 7265 6e74 206d 6172 6769 6e73 206f  ferent margins o
+00046bb0: 6e20 6561 6368 2073 6964 6520 6f66 2074  n each side of t
+00046bc0: 6865 2053 7472 7563 7475 7265 5365 742e  he StructureSet.
+00046bd0: 0a0a 2020 2020 2020 2020 2a2a 5061 7261  ..        **Para
+00046be0: 6d65 7465 7273 3a2a 2a0a 0a20 2020 2020  meters:**..     
+00046bf0: 2020 2072 6f69 5f6e 616d 6573 203a 206c     roi_names : l
+00046c00: 6973 742c 2064 6566 6175 6c74 3d4e 6f6e  ist, default=Non
+00046c10: 650a 2020 2020 2020 2020 2020 2020 4c69  e.            Li
+00046c20: 7374 206f 6620 6e61 6d65 7320 6f66 2052  st of names of R
+00046c30: 4f49 7320 746f 2062 6520 636f 6e73 6964  OIs to be consid
+00046c40: 6572 6564 2e20 2049 6620 4e6f 6e65 2c20  ered.  If None, 
+00046c50: 616c 6c20 6f66 2074 6865 0a20 2020 2020  all of the.     
+00046c60: 2020 2020 2020 2073 7472 7563 7475 7265         structure
+00046c70: 2073 6574 2773 2052 4f49 7320 6172 6520   set's ROIs are 
+00046c80: 636f 6e73 6964 6572 6564 2e0a 0a20 2020  considered...   
+00046c90: 2020 2020 2063 726f 705f 6d61 7267 696e       crop_margin
+00046ca0: 7320 3a20 666c 6f61 742f 7475 706c 652c  s : float/tuple,
+00046cb0: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
+00046cc0: 2020 2020 2020 2020 2020 466c 6f61 7420            Float 
+00046cd0: 6f72 2074 6872 6565 2d65 6c65 6d65 6e74  or three-element
+00046ce0: 2074 7570 6c65 2073 7065 6369 6679 696e   tuple specifyin
+00046cf0: 6720 7468 6520 6d61 7267 696e 732c 2069  g the margins, i
+00046d00: 6e20 6d6d 2c0a 2020 2020 2020 2020 2020  n mm,.          
+00046d10: 2020 746f 2062 6520 6164 6465 6420 746f    to be added to
+00046d20: 2053 7472 7563 7475 7265 5365 7420 6578   StructureSet ex
+00046d30: 7465 6e74 732e 2020 4966 2061 2066 6c6f  tents.  If a flo
+00046d40: 6174 2c20 6d69 6e75 7320 616e 6420 706c  at, minus and pl
+00046d50: 7573 2074 6865 0a20 2020 2020 2020 2020  us the.         
+00046d60: 2020 2076 616c 7565 2073 7065 6369 6669     value specifi
+00046d70: 6564 2061 7265 2061 6464 6564 2074 6f20  ed are added to 
+00046d80: 6c6f 7765 7220 616e 6420 7570 7065 7220  lower and upper 
+00046d90: 6578 7465 6e74 7320 7265 7370 6563 7469  extents respecti
+00046da0: 7665 6c79 0a20 2020 2020 2020 2020 2020  vely.           
+00046db0: 2061 6c6f 6e67 2065 6163 6820 6178 6973   along each axis
+00046dc0: 2e20 2049 6620 6120 7468 7265 652d 656c  .  If a three-el
+00046dd0: 656d 656e 7420 7475 706c 652c 2065 6c65  ement tuple, ele
+00046de0: 6d65 6e74 7320 6172 650a 2020 2020 2020  ments are.      
+00046df0: 2020 2020 2020 7461 6b65 6e20 746f 2073        taken to s
+00046e00: 7065 6369 6679 206d 6172 6769 6e73 2069  pecify margins i
+00046e10: 6e20 7468 6520 6f72 6465 7220 2878 2c20  n the order (x, 
+00046e20: 792c 207a 292e 2020 456c 656d 656e 7473  y, z).  Elements
+00046e30: 0a20 2020 2020 2020 2020 2020 2063 616e  .            can
+00046e40: 2062 6520 6569 7468 6572 2066 6c6f 6174   be either float
+00046e50: 7320 286d 696e 7573 2061 6e64 2070 6c75  s (minus and plu
+00046e60: 7320 7468 6520 7661 6c75 6520 6164 6465  s the value adde
+00046e70: 6420 7265 7370 6563 7469 7665 6c79 0a20  d respectively. 
+00046e80: 2020 2020 2020 2020 2020 2074 6f20 6c6f             to lo
+00046e90: 7765 7220 616e 6420 7570 7065 7220 6578  wer and upper ex
+00046ea0: 7465 6e74 7329 206f 7220 7477 6f2d 656c  tents) or two-el
+00046eb0: 656d 656e 7420 7475 706c 6573 2028 656c  ement tuples (el
+00046ec0: 656d 656e 7473 2030 2061 6e64 2031 0a20  ements 0 and 1. 
+00046ed0: 2020 2020 2020 2020 2020 2061 6464 6564             added
+00046ee0: 2072 6573 7065 6374 6976 656c 7920 746f   respectively to
+00046ef0: 206c 6f77 6572 2061 6e64 2075 7070 6572   lower and upper
+00046f00: 2065 7874 656e 7473 292e 0a0a 2020 2020   extents)...    
+00046f10: 2020 2020 6d65 7468 6f64 203a 2073 7472      method : str
+00046f20: 2c20 6465 6661 756c 743d 4e6f 6e65 0a20  , default=None. 
+00046f30: 2020 2020 2020 2020 2020 204d 6574 686f             Metho
+00046f40: 6420 746f 2075 7365 2066 6f72 2065 7874  d to use for ext
+00046f50: 656e 7420 6361 6c63 756c 6174 696f 6e2e  ent calculation.
+00046f60: 2043 616e 2062 653a 0a0a 2020 2020 2020   Can be:..      
+00046f70: 2020 2020 2020 2020 2020 2a20 2263 6f6e            * "con
+00046f80: 746f 7572 223a 2067 6574 2065 7874 656e  tour": get exten
+00046f90: 7420 6672 6f6d 206d 696e 2f6d 6178 2070  t from min/max p
+00046fa0: 6f73 6974 696f 6e73 206f 6620 636f 6e74  ositions of cont
+00046fb0: 6f75 7228 7329 2e0a 2020 2020 2020 2020  our(s)..        
+00046fc0: 2020 2020 2020 2020 2a20 226d 6173 6b22          * "mask"
+00046fd0: 3a20 6765 7420 6578 7465 6e74 2066 726f  : get extent fro
+00046fe0: 6d20 6d69 6e2f 6d61 7820 706f 7369 7469  m min/max positi
+00046ff0: 6f6e 7320 6f66 2076 6f78 656c 7320 696e  ons of voxels in
+00047000: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00047010: 2020 2020 2020 2062 696e 6172 7920 6d61         binary ma
+00047020: 736b 2e0a 2020 2020 2020 2020 2020 2020  sk..            
+00047030: 2020 2020 2a20 4e6f 6e65 3a20 7573 6520      * None: use 
+00047040: 7468 6520 6d65 7468 6f64 2073 6574 2069  the method set i
+00047050: 6e20 7365 6c66 2e64 6566 6175 6c74 5f67  n self.default_g
+00047060: 656f 6d5f 6d65 7468 6f64 2e0a 2020 2020  eom_method..    
+00047070: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00047080: 7265 7475 726e 2073 656c 662e 636f 6d62  return self.comb
+00047090: 696e 655f 726f 6973 2872 6f69 5f6e 616d  ine_rois(roi_nam
+000470a0: 6573 292e 6765 745f 6372 6f70 5f6c 696d  es).get_crop_lim
+000470b0: 6974 7328 0a20 2020 2020 2020 2020 2020  its(.           
+000470c0: 2020 2020 2063 726f 705f 6d61 7267 696e       crop_margin
+000470d0: 732c 206d 6574 686f 6429 0a0a 2020 2020  s, method)..    
+000470e0: 6465 6620 6765 745f 6262 6f78 5f63 656e  def get_bbox_cen
+000470f0: 7472 655f 616e 645f 7769 6474 6873 2873  tre_and_widths(s
+00047100: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00047110: 2072 6f69 5f6e 616d 6573 3d4e 6f6e 652c   roi_names=None,
+00047120: 2062 7566 6665 723d 4e6f 6e65 2c20 6275   buffer=None, bu
+00047130: 6666 6572 5f75 6e69 7473 3d22 6d6d 222c  ffer_units="mm",
+00047140: 206d 6574 686f 643d 4e6f 6e65 293a 0a20   method=None):. 
+00047150: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00047160: 2020 2047 6574 2063 656e 7472 6520 616e     Get centre an
+00047170: 6420 7769 6474 6873 2069 6e20 6d6d 2061  d widths in mm a
+00047180: 6c6f 6e67 2061 6c6c 2074 6872 6565 2061  long all three a
+00047190: 7865 7320 6f66 2061 2062 6f75 6e64 696e  xes of a boundin
+000471a0: 6720 626f 780a 2020 2020 2020 2020 656e  g box.        en
+000471b0: 636c 6f73 696e 6720 5374 7275 6374 7572  closing Structur
+000471c0: 6553 6574 2052 4f49 7320 616e 6420 6f70  eSet ROIs and op
+000471d0: 7469 6f6e 616c 2062 7566 6665 722e 2020  tional buffer.  
+000471e0: 4365 6e74 7265 0a20 2020 2020 2020 2061  Centre.        a
+000471f0: 6e64 2077 6964 7468 7320 6172 6520 7265  nd widths are re
+00047200: 7475 726e 6564 2061 7320 6120 7475 706c  turned as a tupl
+00047210: 6520 285b 782c 2079 2c20 7a5d 2c20 5b64  e ([x, y, z], [d
+00047220: 782c 2064 792c 2064 7a5d 292e 0a0a 2020  x, dy, dz])...  
+00047230: 2020 2020 2020 4d65 7468 6f64 2070 6172        Method par
+00047240: 616d 6574 6572 7320 6172 6520 7061 7373  ameters are pass
+00047250: 6564 2074 6f0a 2020 2020 2020 2020 736b  ed to.        sk
+00047260: 7274 2e73 7472 7563 7475 7265 732e 5374  rt.structures.St
+00047270: 7275 6374 7572 6553 6574 2e67 6574 5f65  ructureSet.get_e
+00047280: 7874 656e 7473 2829 2074 6f20 6f62 7461  xtents() to obta
+00047290: 696e 2053 7472 7563 7475 7265 5365 740a  in StructureSet.
+000472a0: 2020 2020 2020 2020 6578 7465 6e74 732e          extents.
+000472b0: 2020 466f 7220 7061 7261 6d65 7465 7220    For parameter 
+000472c0: 6578 706c 616e 6174 696f 6e73 2c20 7365  explanations, se
+000472d0: 650a 2020 2020 2020 2020 736b 7274 2e73  e.        skrt.s
+000472e0: 7472 7563 7475 7265 732e 5374 7275 6374  tructures.Struct
+000472f0: 7572 6553 6574 2e67 6574 5f65 7874 656e  ureSet.get_exten
+00047300: 7473 2829 2064 6f63 756d 656e 7461 7469  ts() documentati
+00047310: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
+00047320: 2020 2020 2020 2020 6578 7465 6e74 7320          extents 
+00047330: 3d20 7365 6c66 2e67 6574 5f65 7874 656e  = self.get_exten
+00047340: 7473 2872 6f69 5f6e 616d 6573 2c20 6275  ts(roi_names, bu
+00047350: 6666 6572 2c20 6275 6666 6572 5f75 6e69  ffer, buffer_uni
+00047360: 7473 2c20 6d65 7468 6f64 2920 0a20 2020  ts, method) .   
+00047370: 2020 2020 2063 656e 7472 6520 3d20 5b30       centre = [0
+00047380: 2e35 202a 2028 6578 7465 6e74 5b30 5d20  .5 * (extent[0] 
+00047390: 2b20 6578 7465 6e74 5b31 5d29 2066 6f72  + extent[1]) for
+000473a0: 2065 7874 656e 7420 696e 2065 7874 656e   extent in exten
+000473b0: 7473 5d0a 2020 2020 2020 2020 7769 6474  ts].        widt
+000473c0: 6873 203d 205b 2865 7874 656e 745b 315d  hs = [(extent[1]
+000473d0: 202d 2065 7874 656e 745b 305d 2920 666f   - extent[0]) fo
+000473e0: 7220 6578 7465 6e74 2069 6e20 6578 7465  r extent in exte
+000473f0: 6e74 735d 0a20 2020 2020 2020 2072 6574  nts].        ret
+00047400: 7572 6e20 2863 656e 7472 652c 2077 6964  urn (centre, wid
+00047410: 7468 7329 0a0a 2020 2020 6465 6620 6765  ths)..    def ge
+00047420: 745f 6475 6d6d 795f 696d 6167 6528 7365  t_dummy_image(se
+00047430: 6c66 2c20 2a2a 6b77 6172 6773 293a 0a20  lf, **kwargs):. 
+00047440: 2020 2020 2020 2022 2222 4d61 6b65 2061         """Make a
+00047450: 2064 756d 6d79 2069 6d61 6765 2074 6861   dummy image tha
+00047460: 7420 636f 7665 7273 2074 6865 2061 7265  t covers the are
+00047470: 6120 7370 616e 6e65 6420 6279 2061 6c6c  a spanned by all
+00047480: 2052 4f49 7320 696e 2074 6869 730a 2020   ROIs in this.  
+00047490: 2020 2020 2020 5374 7275 6374 7572 6553        StructureS
+000474a0: 6574 2e20 5265 7475 726e 7320 616e 2049  et. Returns an I
+000474b0: 6d61 6765 206f 626a 6563 742e 0a0a 2020  mage object...  
+000474c0: 2020 2020 2020 2a2a 5061 7261 6d65 7465        **Paramete
+000474d0: 7273 3a2a 2a0a 2020 2020 2020 2020 0a20  rs:**.        . 
+000474e0: 2020 2020 2020 2076 6f78 656c 5f73 697a         voxel_siz
+000474f0: 6520 3a20 6c69 7374 2c20 6465 6661 756c  e : list, defaul
+00047500: 743d 4e6f 6e65 0a20 2020 2020 2020 2020  t=None.         
+00047510: 2020 2056 6f78 656c 2073 697a 6520 696e     Voxel size in
+00047520: 206d 6d20 696e 2074 6865 2064 756d 6d79   mm in the dummy
+00047530: 2069 6d61 6765 2069 6e20 7468 6520 782d   image in the x-
+00047540: 7920 706c 616e 652c 2067 6976 656e 2061  y plane, given a
+00047550: 7320 0a20 2020 2020 2020 2020 2020 205b  s .            [
+00047560: 7678 2c20 7679 5d2e 2049 6620 3c73 6861  vx, vy]. If <sha
+00047570: 7065 3e20 616e 6420 3c76 6f78 656c 5f73  pe> and <voxel_s
+00047580: 697a 653e 2061 7265 2062 6f74 6820 4e6f  ize> are both No
+00047590: 6e65 2c20 766f 7865 6c20 7369 7a65 7320  ne, voxel sizes 
+000475a0: 6f66 0a20 2020 2020 2020 2020 2020 205b  of.            [
+000475b0: 312c 2031 5d20 7769 6c6c 2062 6520 7573  1, 1] will be us
+000475c0: 6564 2062 7920 6465 6661 756c 742e 2054  ed by default. T
+000475d0: 6865 2076 6f78 656c 2073 697a 6520 696e  he voxel size in
+000475e0: 2074 6865 207a 2064 6972 6563 7469 6f6e   the z direction
+000475f0: 200a 2020 2020 2020 2020 2020 2020 6973   .            is
+00047600: 2064 6566 696e 6564 2062 7920 3c73 6c69   defined by <sli
+00047610: 6365 5f74 6869 636b 6e65 7373 3e2e 0a0a  ce_thickness>...
+00047620: 2020 2020 2020 2020 7368 6170 6520 3a20          shape : 
+00047630: 6c69 7374 2c20 6465 6661 756c 743d 4e6f  list, default=No
+00047640: 6e65 0a20 2020 2020 2020 2020 2020 204e  ne.            N
+00047650: 756d 6265 7220 6f66 2076 6f78 656c 7320  umber of voxels 
+00047660: 696e 2074 6865 2064 756d 6d79 2069 6d61  in the dummy ima
+00047670: 6765 2069 6e20 7468 6520 782d 7920 706c  ge in the x-y pl
+00047680: 616e 652c 2067 6976 656e 2061 730a 2020  ane, given as.  
+00047690: 2020 2020 2020 2020 2020 5b6e 782c 206e            [nx, n
+000476a0: 795d 2e20 4f6e 6c79 2075 7365 6420 6966  y]. Only used if
+000476b0: 203c 766f 7865 6c5f 7369 7a65 3e20 6973   <voxel_size> is
+000476c0: 204e 6f6e 652e 200a 2020 2020 2020 2020   None. .        
+000476d0: 2020 2020 5468 6520 6e75 6d62 6572 206f      The number o
+000476e0: 6620 766f 7865 6c73 2069 6e20 7468 6520  f voxels in the 
+000476f0: 7a20 6469 7265 6374 696f 6e20 7769 6c6c  z direction will
+00047700: 2062 6520 7461 6b65 6e20 6672 6f6d 2074   be taken from t
+00047710: 6865 200a 2020 2020 2020 2020 2020 2020  he .            
+00047720: 6e75 6d62 6572 206f 6620 736c 6963 6573  number of slices
+00047730: 2069 6e20 7468 6520 782d 7920 636f 6e74   in the x-y cont
+00047740: 6f75 7273 2064 6963 7469 6f6e 6172 792e  ours dictionary.
+00047750: 0a0a 2020 2020 2020 2020 6669 6c6c 5f76  ..        fill_v
+00047760: 616c 203a 2069 6e74 2f66 6c6f 6174 2c20  al : int/float, 
+00047770: 6465 6661 756c 743d 3165 340a 2020 2020  default=1e4.    
+00047780: 2020 2020 2020 2020 5661 6c75 6520 7769          Value wi
+00047790: 7468 2077 6869 6368 2074 6865 2076 6f78  th which the vox
+000477a0: 656c 7320 696e 2074 6865 2064 756d 6d79  els in the dummy
+000477b0: 2069 6d61 6765 2073 686f 756c 6420 6265   image should be
+000477c0: 2066 696c 6c65 642e 200a 0a20 2020 2020   filled. ..     
+000477d0: 2020 2062 7566 6665 7220 3a20 696e 742c     buffer : int,
+000477e0: 2064 6566 6175 6c74 3d31 0a20 2020 2020   default=1.     
+000477f0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+00047800: 2065 6d70 7479 2062 7566 6665 7220 766f   empty buffer vo
+00047810: 7865 6c73 2074 6f20 6164 6420 6f75 7473  xels to add outs
+00047820: 6964 6520 7468 6520 524f 4920 696e 2065  ide the ROI in e
+00047830: 6163 680a 2020 2020 2020 2020 2020 2020  ach.            
+00047840: 6469 7265 6374 696f 6e2e 0a0a 2020 2020  direction...    
+00047850: 2020 2020 736c 6963 655f 7468 6963 6b6e      slice_thickn
+00047860: 6573 7320 3a20 666c 6f61 742c 2064 6566  ess : float, def
+00047870: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
+00047880: 2020 2020 2020 566f 7865 6c20 7369 7a65        Voxel size
+00047890: 2069 6e20 6d6d 2069 6e20 7468 6520 6475   in mm in the du
+000478a0: 6d6d 7920 696d 6167 6520 696e 2074 6865  mmy image in the
+000478b0: 207a 2064 6972 6563 7469 6f6e 2e20 2049   z direction.  I
+000478c0: 6620 4e6f 6e65 2c0a 2020 2020 2020 2020  f None,.        
+000478d0: 2020 2020 7468 6520 7661 6c75 6520 7573      the value us
+000478e0: 6564 2069 7320 7468 6520 6d69 6e69 6d75  ed is the minimu
+000478f0: 6d20 6469 7374 616e 6365 2062 6574 7765  m distance betwe
+00047900: 656e 2073 6c69 6365 2070 6f73 6974 696f  en slice positio
+00047910: 6e73 0a20 2020 2020 2020 2020 2020 2069  ns.            i
+00047920: 6e20 7468 6520 782d 7920 636f 6e74 6f75  n the x-y contou
+00047930: 7273 2064 6963 7469 6f6e 6172 792e 0a20  rs dictionary.. 
+00047940: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00047950: 2020 2065 7874 656e 7473 203d 205b 7365     extents = [se
+00047960: 6c66 2e67 6574 5f65 7874 656e 7428 6178  lf.get_extent(ax
+00047970: 3d61 7829 2066 6f72 2061 7820 696e 2073  =ax) for ax in s
+00047980: 6b72 742e 696d 6167 652e 5f61 7865 735d  krt.image._axes]
+00047990: 0a20 2020 2020 2020 2073 6c69 6365 5f74  .        slice_t
+000479a0: 6869 636b 6e65 7373 203d 206b 7761 7267  hickness = kwarg
+000479b0: 732e 706f 7028 2273 6c69 6365 5f74 6869  s.pop("slice_thi
+000479c0: 636b 6e65 7373 222c 204e 6f6e 6529 0a20  ckness", None). 
+000479d0: 2020 2020 2020 2073 6c69 6365 5f74 6869         slice_thi
+000479e0: 636b 6e65 7373 203d 2028 736c 6963 655f  ckness = (slice_
+000479f0: 7468 6963 6b6e 6573 7320 6f72 0a20 2020  thickness or.   
+00047a00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00047a10: 662e 6765 745f 726f 6973 2869 676e 6f72  f.get_rois(ignor
+00047a20: 655f 656d 7074 793d 5472 7565 295b 305d  e_empty=True)[0]
+00047a30: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
+00047a40: 2020 2020 2020 2020 2020 2e67 6574 5f73            .get_s
+00047a50: 6c69 6365 5f74 6869 636b 6e65 7373 5f63  lice_thickness_c
+00047a60: 6f6e 746f 7572 7328 2929 0a20 2020 2020  ontours()).     
+00047a70: 2020 2072 6574 7572 6e20 6372 6561 7465     return create
+00047a80: 5f64 756d 6d79 5f69 6d61 6765 2865 7874  _dummy_image(ext
+00047a90: 656e 7473 2c20 736c 6963 655f 7468 6963  ents, slice_thic
+00047aa0: 6b6e 6573 732c 202a 2a6b 7761 7267 7329  kness, **kwargs)
+00047ab0: 0a0a 2020 2020 6465 6620 5f67 6574 5f63  ..    def _get_c
+00047ac0: 6f6d 6269 6e61 7469 6f6e 2873 656c 662c  ombination(self,
+00047ad0: 206e 616d 652c 2066 6f72 6365 2c20 6578   name, force, ex
+00047ae0: 636c 7564 652c 2063 6f6d 626f 5f6d 616b  clude, combo_mak
+00047af0: 6572 2c20 2a2a 6b77 6172 6773 293a 0a20  er, **kwargs):. 
+00047b00: 2020 2020 2020 2022 2222 4569 7468 6572         """Either
+00047b10: 2067 6574 2061 6e20 616c 7265 6164 7920   get an already 
+00047b20: 6361 6c63 756c 6174 6564 2063 6f6d 6269  calculated combi
+00047b30: 6e61 7469 6f6e 2066 726f 6d20 7468 6520  nation from the 
+00047b40: 6361 6368 650a 2020 2020 2020 2020 6f72  cache.        or
+00047b50: 2063 7265 6174 6520 6974 2c20 6361 6368   create it, cach
+00047b60: 6520 6974 2c20 616e 6420 7265 7475 726e  e it, and return
+00047b70: 2069 742e 2222 220a 0a20 2020 2020 2020   it."""..       
+00047b80: 2023 2052 6574 7572 6e20 6361 6368 6564   # Return cached
+00047b90: 2072 6573 756c 7420 6966 2069 7420 6578   result if it ex
+00047ba0: 6973 7473 2061 6e64 206e 6f74 2066 6f72  ists and not for
+00047bb0: 6369 6e67 0a20 2020 2020 2020 2061 7474  cing.        att
+00047bc0: 7220 3d20 6622 5f7b 6e61 6d65 7d22 0a20  r = f"_{name}". 
+00047bd0: 2020 2020 2020 2069 6620 6578 636c 7564         if exclud
+00047be0: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+00047bf0: 7474 7220 2b3d 2066 225f 6578 636c 7564  ttr += f"_exclud
+00047c00: 6564 220a 2020 2020 2020 2020 6966 206e  ed".        if n
+00047c10: 6f74 2066 6f72 6365 3a0a 2020 2020 2020  ot force:.      
+00047c20: 2020 2020 2020 6966 2065 7863 6c75 6465        if exclude
+00047c30: 2069 7320 4e6f 6e65 2061 6e64 2068 6173   is None and has
+00047c40: 6174 7472 2873 656c 662c 2061 7474 7229  attr(self, attr)
+00047c50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00047c60: 2020 7265 7475 726e 2067 6574 6174 7472    return getattr
+00047c70: 2873 656c 662c 2061 7474 7229 0a20 2020  (self, attr).   
+00047c80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00047c90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00047ca0: 6620 6861 7361 7474 7228 7365 6c66 2c20  f hasattr(self, 
+00047cb0: 6174 7472 2920 616e 6420 6578 636c 7564  attr) and exclud
+00047cc0: 6520 696e 2067 6574 6174 7472 2873 656c  e in getattr(sel
+00047cd0: 662c 2061 7474 7229 3a0a 2020 2020 2020  f, attr):.      
+00047ce0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00047cf0: 7475 726e 2067 6574 6174 7472 2873 656c  turn getattr(sel
+00047d00: 662c 2061 7474 7229 5b65 7863 6c75 6465  f, attr)[exclude
+00047d10: 5d0a 0a20 2020 2020 2020 2023 2047 6574  ]..        # Get
+00047d20: 206c 6973 7420 6f66 2052 4f49 7320 746f   list of ROIs to
+00047d30: 2069 6e63 6c75 6465 2069 6e20 7468 6973   include in this
+00047d40: 2063 6f6d 6269 6e61 7469 6f6e 2052 4f49   combination ROI
+00047d50: 0a20 2020 2020 2020 2069 6620 6578 636c  .        if excl
+00047d60: 7564 6520 6973 206e 6f74 204e 6f6e 653a  ude is not None:
+00047d70: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00047d80: 2065 7863 6c75 6465 206e 6f74 2069 6e20   exclude not in 
+00047d90: 7365 6c66 2e67 6574 5f72 6f69 5f6e 616d  self.get_roi_nam
+00047da0: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
+00047db0: 2020 2020 2020 7072 696e 7428 6622 524f        print(f"RO
+00047dc0: 4920 746f 2065 7863 6c75 6465 207b 6578  I to exclude {ex
+00047dd0: 636c 7564 657d 206e 6f74 2066 6f75 6e64  clude} not found
+00047de0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00047df0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00047e00: 2020 2020 2020 2020 726f 6973 5f74 6f5f          rois_to_
+00047e10: 696e 636c 7564 6520 3d20 5b72 6f69 2066  include = [roi f
+00047e20: 6f72 2072 6f69 2069 6e20 7365 6c66 2e72  or roi in self.r
+00047e30: 6f69 7320 6966 2072 6f69 2e6e 616d 6520  ois if roi.name 
+00047e40: 213d 2065 7863 6c75 6465 5d0a 0a20 2020  != exclude]..   
+00047e50: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00047e60: 6861 7361 7474 7228 7365 6c66 2c20 6174  hasattr(self, at
+00047e70: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+00047e80: 2020 2020 2073 6574 6174 7472 2873 656c       setattr(sel
+00047e90: 662c 2061 7474 722c 207b 7d29 0a20 2020  f, attr, {}).   
+00047ea0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00047eb0: 2020 2020 2020 2072 6f69 735f 746f 5f69         rois_to_i
+00047ec0: 6e63 6c75 6465 203d 2073 656c 662e 726f  nclude = self.ro
+00047ed0: 6973 0a0a 2020 2020 2020 2020 2320 4d61  is..        # Ma
+00047ee0: 6b65 206b 7761 7267 7320 666f 7220 524f  ke kwargs for RO
+00047ef0: 4920 6372 6561 7469 6f6e 0a20 2020 2020  I creation.     
+00047f00: 2020 2072 6f69 5f6b 7761 7267 7320 3d20     roi_kwargs = 
+00047f10: 7365 6c66 2e72 6f69 5f6b 7761 7267 732e  self.roi_kwargs.
+00047f20: 636f 7079 2829 0a20 2020 2020 2020 2072  copy().        r
+00047f30: 6f69 5f6b 7761 7267 732e 7570 6461 7465  oi_kwargs.update
+00047f40: 286b 7761 7267 7329 0a20 2020 2020 2020  (kwargs).       
+00047f50: 2072 6f69 5f6b 7761 7267 735b 226e 616d   roi_kwargs["nam
+00047f60: 6522 5d20 3d20 6e61 6d65 0a20 2020 2020  e"] = name.     
+00047f70: 2020 2072 6f69 5f6b 7761 7267 735b 2269     roi_kwargs["i
+00047f80: 6d61 6765 225d 203d 2073 656c 662e 696d  mage"] = self.im
+00047f90: 6167 650a 2020 2020 2020 2020 726f 695f  age.        roi_
+00047fa0: 6b77 6172 6773 5b22 6166 6669 6e65 225d  kwargs["affine"]
+00047fb0: 203d 2072 6f69 735f 746f 5f69 6e63 6c75   = rois_to_inclu
+00047fc0: 6465 5b30 5d2e 6765 745f 6166 6669 6e65  de[0].get_affine
+00047fd0: 2873 7461 6e64 6172 6469 7365 3d54 7275  (standardise=Tru
+00047fe0: 6529 0a0a 2020 2020 2020 2020 2320 4372  e)..        # Cr
+00047ff0: 6561 7465 2074 6865 2052 4f49 0a20 2020  eate the ROI.   
+00048000: 2020 2020 2072 6f69 203d 2063 6f6d 626f       roi = combo
+00048010: 5f6d 616b 6572 2872 6f69 735f 746f 5f69  _maker(rois_to_i
+00048020: 6e63 6c75 6465 2c20 2a2a 726f 695f 6b77  nclude, **roi_kw
+00048030: 6172 6773 290a 0a20 2020 2020 2020 2023  args)..        #
+00048040: 2041 6464 2069 7420 746f 2074 6865 2063   Add it to the c
+00048050: 6163 6865 2061 6e64 2072 6574 7572 6e0a  ache and return.
+00048060: 2020 2020 2020 2020 6966 2065 7863 6c75          if exclu
+00048070: 6465 2069 7320 4e6f 6e65 3a0a 2020 2020  de is None:.    
+00048080: 2020 2020 2020 2020 7365 7461 7474 7228          setattr(
+00048090: 7365 6c66 2c20 6174 7472 2c20 726f 6929  self, attr, roi)
+000480a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000480b0: 2020 2020 2020 2020 2020 2067 6574 6174             getat
+000480c0: 7472 2873 656c 662c 2061 7474 7229 5b65  tr(self, attr)[e
+000480d0: 7863 6c75 6465 5d20 3d20 726f 690a 2020  xclude] = roi.  
+000480e0: 2020 2020 2020 7265 7475 726e 2072 6f69        return roi
+000480f0: 0a0a 2020 2020 6465 6620 6765 745f 636f  ..    def get_co
+00048100: 6e73 656e 7375 7328 7365 6c66 2c20 636f  nsensus(self, co
+00048110: 6e73 656e 7375 735f 7479 7065 2c20 636f  nsensus_type, co
+00048120: 6c6f 723d 2262 6c75 6522 2c20 2a2a 6b77  lor="blue", **kw
+00048130: 6172 6773 293a 0a0a 2020 2020 2020 2020  args):..        
+00048140: 2320 4765 7420 636f 6e73 656e 7375 7320  # Get consensus 
+00048150: 6361 6c63 756c 6174 696f 6e20 6675 6e63  calculation func
+00048160: 7469 6f6e 0a20 2020 2020 2020 2069 6620  tion.        if 
+00048170: 636f 6e73 656e 7375 735f 7479 7065 203d  consensus_type =
+00048180: 3d20 226d 616a 6f72 6974 7922 3a0a 2020  = "majority":.  
+00048190: 2020 2020 2020 2020 2020 636f 6e73 656e            consen
+000481a0: 7375 735f 6675 6e63 203d 2053 7472 7563  sus_func = Struc
+000481b0: 7475 7265 5365 742e 6765 745f 6d61 6a6f  tureSet.get_majo
+000481c0: 7269 7479 5f76 6f74 650a 2020 2020 2020  rity_vote.      
+000481d0: 2020 656c 6966 2063 6f6e 7365 6e73 7573    elif consensus
+000481e0: 5f74 7970 6520 3d3d 2022 7375 6d22 3a0a  _type == "sum":.
+000481f0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00048200: 656e 7375 735f 6675 6e63 203d 2053 7472  ensus_func = Str
+00048210: 7563 7475 7265 5365 742e 6765 745f 7375  uctureSet.get_su
+00048220: 6d0a 2020 2020 2020 2020 656c 6966 2063  m.        elif c
+00048230: 6f6e 7365 6e73 7573 5f74 7970 6520 3d3d  onsensus_type ==
+00048240: 2022 6f76 6572 6c61 7022 3a0a 2020 2020   "overlap":.    
+00048250: 2020 2020 2020 2020 636f 6e73 656e 7375          consensu
+00048260: 735f 6675 6e63 203d 2053 7472 7563 7475  s_func = Structu
+00048270: 7265 5365 742e 6765 745f 6f76 6572 6c61  reSet.get_overla
+00048280: 700a 2020 2020 2020 2020 656c 6966 2063  p.        elif c
+00048290: 6f6e 7365 6e73 7573 5f74 7970 6520 3d3d  onsensus_type ==
+000482a0: 2022 7374 6170 6c65 223a 0a20 2020 2020   "staple":.     
+000482b0: 2020 2020 2020 2063 6f6e 7365 6e73 7573         consensus
+000482c0: 5f66 756e 6320 3d20 5374 7275 6374 7572  _func = Structur
+000482d0: 6553 6574 2e67 6574 5f73 7461 706c 650a  eSet.get_staple.
+000482e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000482f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00048300: 5661 6c75 6545 7272 6f72 2866 2255 6e72  ValueError(f"Unr
+00048310: 6563 6f67 6e69 7365 6420 636f 6e73 656e  ecognised consen
+00048320: 7375 7320 7479 7065 3a20 7b63 6f6e 7365  sus type: {conse
+00048330: 6e73 7573 5f74 7970 657d 2229 0a0a 2020  nsus_type}")..  
+00048340: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
+00048350: 7365 6e73 7573 5f66 756e 6328 7365 6c66  sensus_func(self
+00048360: 2c20 636f 6c6f 723d 636f 6c6f 722c 202a  , color=color, *
+00048370: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+00048380: 6620 6765 745f 7374 6170 6c65 2873 656c  f get_staple(sel
+00048390: 662c 2066 6f72 6365 3d46 616c 7365 2c20  f, force=False, 
+000483a0: 6578 636c 7564 653d 4e6f 6e65 2c20 2a2a  exclude=None, **
+000483b0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+000483c0: 2022 2222 4765 7420 524f 4920 6f62 6a65   """Get ROI obje
+000483d0: 6374 2072 6570 7265 7365 6e74 696e 6720  ct representing 
+000483e0: 7468 6520 5354 4150 4c45 2063 6f6d 6269  the STAPLE combi
+000483f0: 6e61 7469 6f6e 206f 6620 524f 4973 2069  nation of ROIs i
+00048400: 6e20 7468 6973 200a 2020 2020 2020 2020  n this .        
+00048410: 7374 7275 6374 7572 6520 7365 742e 2049  structure set. I
+00048420: 6620 3c65 7863 6c75 6465 3e20 6973 2073  f <exclude> is s
+00048430: 6574 2074 6f20 6120 7374 7269 6e67 2c20  et to a string, 
+00048440: 7468 6520 524f 4920 7769 7468 2074 6861  the ROI with tha
+00048450: 7420 6e61 6d65 200a 2020 2020 2020 2020  t name .        
+00048460: 7769 6c6c 2062 6520 6578 636c 7564 6564  will be excluded
+00048470: 2066 726f 6d20 7468 6520 6361 6c63 756c   from the calcul
+00048480: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
+00048490: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
+000484a0: 0a20 2020 2020 2020 2066 6f72 6365 203a  .        force :
+000484b0: 2062 6f6f 6c2c 2064 6566 6175 6c74 3d46   bool, default=F
+000484c0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+000484d0: 2049 6620 4661 6c73 6520 616e 6420 5354   If False and ST
+000484e0: 4150 4c45 2052 4f49 2068 6173 2061 6c72  APLE ROI has alr
+000484f0: 6561 6479 2062 6565 6e20 6372 6561 7465  eady been create
+00048500: 642c 2074 6865 200a 2020 2020 2020 2020  d, the .        
+00048510: 2020 2020 7072 6576 696f 7573 6c79 2063      previously c
+00048520: 6f6d 7075 7465 6420 524f 4920 7769 6c6c  omputed ROI will
+00048530: 2062 6520 7265 7475 726e 6564 2e20 4966   be returned. If
+00048540: 2046 6f72 6365 3d54 7275 652c 2074 6865   Force=True, the
+00048550: 200a 2020 2020 2020 2020 2020 2020 5354   .            ST
+00048560: 4150 4c45 2052 4f49 2077 696c 6c20 6265  APLE ROI will be
+00048570: 2072 6563 7265 6174 6564 2e0a 0a20 2020   recreated...   
+00048580: 2020 2020 2065 7863 6c75 6465 203a 2073       exclude : s
+00048590: 7472 2c20 6465 6661 756c 743d 4e6f 6e65  tr, default=None
+000485a0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000485b0: 7365 7420 746f 2061 2073 7472 696e 672c  set to a string,
+000485c0: 2074 6865 2066 6972 7374 2052 4f49 2069   the first ROI i
+000485d0: 6e20 7365 6c66 2e72 6f69 7320 7769 7468  n self.rois with
+000485e0: 2074 6861 7420 6e61 6d65 2077 696c 6c20   that name will 
+000485f0: 0a20 2020 2020 2020 2020 2020 2062 6520  .            be 
+00048600: 6578 636c 7564 6564 2066 726f 6d20 7468  excluded from th
+00048610: 6520 636f 6d62 696e 6174 696f 6e2e 2054  e combination. T
+00048620: 6869 7320 6d61 7920 6265 2075 7365 6675  his may be usefu
+00048630: 6c20 6966 2063 6f6d 7061 7269 736f 6e20  l if comparison 
+00048640: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
+00048650: 6120 7369 6e67 6c65 2052 4f49 2077 6974  a single ROI wit
+00048660: 6820 7468 6520 636f 6e73 656e 7375 7320  h the consensus 
+00048670: 6f66 2061 6c6c 206f 7468 6572 7320 6973  of all others is
+00048680: 2064 6573 6972 6564 2e0a 0a20 2020 2020   desired...     
+00048690: 2020 2060 2a2a 606b 7761 7267 7320 3a0a     `**`kwargs :.
+000486a0: 2020 2020 2020 2020 2020 2020 4578 7472              Extr
+000486b0: 6120 6b65 7977 6f72 6420 6172 6775 6d65  a keyword argume
+000486c0: 6e74 7320 746f 2070 6173 7320 746f 2074  nts to pass to t
+000486d0: 6865 2063 7265 6174 696f 6e20 6f66 2074  he creation of t
+000486e0: 6865 2052 4f49 206f 626a 6563 740a 2020  he ROI object.  
+000486f0: 2020 2020 2020 2020 2020 7265 7072 6573            repres
+00048700: 656e 7469 6e67 2074 6865 2063 6f6d 6269  enting the combi
+00048710: 6e61 7469 6f6e 2e0a 2020 2020 2020 2020  nation..        
+00048720: 2222 220a 0a20 2020 2020 2020 2072 6574  """..        ret
+00048730: 7572 6e20 7365 6c66 2e5f 6765 745f 636f  urn self._get_co
+00048740: 6d62 696e 6174 696f 6e28 2273 7461 706c  mbination("stapl
+00048750: 6522 2c20 666f 7263 652c 2065 7863 6c75  e", force, exclu
+00048760: 6465 2c20 6372 6561 7465 5f73 7461 706c  de, create_stapl
+00048770: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00048780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00048790: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+000487a0: 290a 0a20 2020 2064 6566 2067 6574 5f6d  )..    def get_m
+000487b0: 616a 6f72 6974 795f 766f 7465 2873 656c  ajority_vote(sel
+000487c0: 662c 2066 6f72 6365 3d46 616c 7365 2c20  f, force=False, 
+000487d0: 6578 636c 7564 653d 4e6f 6e65 2c20 2a2a  exclude=None, **
+000487e0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+000487f0: 2022 2222 4765 7420 524f 4920 6f62 6a65   """Get ROI obje
+00048800: 6374 2072 6570 7265 7365 6e74 696e 6720  ct representing 
+00048810: 7468 6520 6d61 6a6f 7269 7479 2076 6f74  the majority vot
+00048820: 6520 636f 6d62 696e 6174 696f 6e20 6f66  e combination of
+00048830: 2052 4f49 7320 696e 200a 2020 2020 2020   ROIs in .      
+00048840: 2020 7468 6973 2073 7472 7563 7475 7265    this structure
+00048850: 2073 6574 2e20 4966 203c 6578 636c 7564   set. If <exclud
+00048860: 653e 2069 7320 7365 7420 746f 2061 2073  e> is set to a s
+00048870: 7472 696e 672c 2074 6865 2052 4f49 2077  tring, the ROI w
+00048880: 6974 6820 7468 6174 200a 2020 2020 2020  ith that .      
+00048890: 2020 6e61 6d65 2077 696c 6c20 6265 2065    name will be e
+000488a0: 7863 6c75 6465 6420 6672 6f6d 2074 6865  xcluded from the
+000488b0: 2063 616c 6375 6c61 7469 6f6e 2e0a 0a20   calculation... 
+000488c0: 2020 2020 2020 202a 2a50 6172 616d 6574         **Paramet
+000488d0: 6572 733a 2a2a 0a0a 2020 2020 2020 2020  ers:**..        
+000488e0: 666f 7263 6520 3a20 626f 6f6c 2c20 6465  force : bool, de
+000488f0: 6661 756c 743d 4661 6c73 650a 2020 2020  fault=False.    
+00048900: 2020 2020 2020 2020 4966 2046 616c 7365          If False
+00048910: 2061 6e64 206d 616a 6f72 6974 7920 766f   and majority vo
+00048920: 7465 2052 4f49 2068 6173 2061 6c72 6561  te ROI has alrea
+00048930: 6479 2062 6565 6e20 6372 6561 7465 642c  dy been created,
+00048940: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
+00048950: 2020 7072 6576 696f 7573 6c79 2063 6f6d    previously com
+00048960: 7075 7465 6420 524f 4920 7769 6c6c 2062  puted ROI will b
+00048970: 6520 7265 7475 726e 6564 2e20 4966 2046  e returned. If F
+00048980: 6f72 6365 3d54 7275 652c 2074 6865 200a  orce=True, the .
+00048990: 2020 2020 2020 2020 2020 2020 6d61 6a6f              majo
+000489a0: 7269 7479 2076 6f74 6520 524f 4920 7769  rity vote ROI wi
+000489b0: 6c6c 2062 6520 7265 6372 6561 7465 642e  ll be recreated.
+000489c0: 0a0a 2020 2020 2020 2020 6578 636c 7564  ..        exclud
+000489d0: 6520 3a20 7374 722c 2064 6566 6175 6c74  e : str, default
+000489e0: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
+000489f0: 2020 4966 2073 6574 2074 6f20 6120 7374    If set to a st
+00048a00: 7269 6e67 2c20 7468 6520 6669 7273 7420  ring, the first 
+00048a10: 524f 4920 696e 2073 656c 662e 726f 6973  ROI in self.rois
+00048a20: 2077 6974 6820 7468 6174 206e 616d 6520   with that name 
+00048a30: 7769 6c6c 200a 2020 2020 2020 2020 2020  will .          
+00048a40: 2020 6265 2065 7863 6c75 6465 6420 6672    be excluded fr
+00048a50: 6f6d 2074 6865 2063 6f6d 6269 6e61 7469  om the combinati
+00048a60: 6f6e 2e20 5468 6973 206d 6179 2062 6520  on. This may be 
+00048a70: 7573 6566 756c 2069 6620 636f 6d70 6172  useful if compar
+00048a80: 6973 6f6e 200a 2020 2020 2020 2020 2020  ison .          
+00048a90: 2020 6f66 2061 2073 696e 676c 6520 524f    of a single RO
+00048aa0: 4920 7769 7468 2074 6865 2063 6f6e 7365  I with the conse
+00048ab0: 6e73 7573 206f 6620 616c 6c20 6f74 6865  nsus of all othe
+00048ac0: 7273 2069 7320 6465 7369 7265 642e 0a0a  rs is desired...
+00048ad0: 2020 2020 2020 2020 602a 2a60 6b77 6172          `**`kwar
+00048ae0: 6773 203a 0a20 2020 2020 2020 2020 2020  gs :.           
+00048af0: 2045 7874 7261 206b 6579 776f 7264 2061   Extra keyword a
+00048b00: 7267 756d 656e 7473 2074 6f20 7061 7373  rguments to pass
+00048b10: 2074 6f20 7468 6520 6372 6561 7469 6f6e   to the creation
+00048b20: 206f 6620 7468 6520 524f 4920 6f62 6a65   of the ROI obje
+00048b30: 6374 0a20 2020 2020 2020 2020 2020 2072  ct.            r
+00048b40: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00048b50: 636f 6d62 696e 6174 696f 6e2e 0a20 2020  combination..   
+00048b60: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00048b70: 2020 7265 7475 726e 2073 656c 662e 5f67    return self._g
+00048b80: 6574 5f63 6f6d 6269 6e61 7469 6f6e 2822  et_combination("
+00048b90: 6d61 6a6f 7269 7479 5f76 6f74 6522 2c20  majority_vote", 
+00048ba0: 666f 7263 652c 2065 7863 6c75 6465 2c20  force, exclude, 
+00048bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00048bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00048bd0: 2020 2020 2020 6372 6561 7465 5f6d 616a        create_maj
+00048be0: 6f72 6974 795f 766f 7465 2c20 2a2a 6b77  ority_vote, **kw
+00048bf0: 6172 6773 290a 0a20 2020 2064 6566 2067  args)..    def g
+00048c00: 6574 5f73 756d 2873 656c 662c 2066 6f72  et_sum(self, for
+00048c10: 6365 3d46 616c 7365 2c20 6578 636c 7564  ce=False, exclud
+00048c20: 653d 4e6f 6e65 2c20 2a2a 6b77 6172 6773  e=None, **kwargs
+00048c30: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+00048c40: 7420 524f 4920 6f62 6a65 6374 2072 6570  t ROI object rep
+00048c50: 7265 7365 6e74 696e 6720 7468 6520 7375  resenting the su
+00048c60: 6d20 6f66 2052 4f49 7320 696e 2074 6869  m of ROIs in thi
+00048c70: 7320 7374 7275 6374 7572 6520 7365 742e  s structure set.
+00048c80: 200a 2020 2020 2020 2020 4966 203c 6578   .        If <ex
+00048c90: 636c 7564 653e 2069 7320 7365 7420 746f  clude> is set to
+00048ca0: 2061 2073 7472 696e 672c 2074 6865 2052   a string, the R
+00048cb0: 4f49 2077 6974 6820 7468 6174 206e 616d  OI with that nam
+00048cc0: 6520 7769 6c6c 2062 6520 0a20 2020 2020  e will be .     
+00048cd0: 2020 2065 7863 6c75 6465 6420 6672 6f6d     excluded from
+00048ce0: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
+00048cf0: 2e0a 0a20 2020 2020 2020 202a 2a50 6172  ...        **Par
+00048d00: 616d 6574 6572 733a 2a2a 0a0a 2020 2020  ameters:**..    
+00048d10: 2020 2020 666f 7263 6520 3a20 626f 6f6c      force : bool
+00048d20: 2c20 6465 6661 756c 743d 4661 6c73 650a  , default=False.
+00048d30: 2020 2020 2020 2020 2020 2020 4966 2046              If F
+00048d40: 616c 7365 2061 6e64 2073 756d 2052 4f49  alse and sum ROI
+00048d50: 2068 6173 2061 6c72 6561 6479 2062 6565   has already bee
+00048d60: 6e20 6372 6561 7465 642c 2074 6865 200a  n created, the .
+00048d70: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00048d80: 696f 7573 6c79 2063 6f6d 7075 7465 6420  iously computed 
+00048d90: 524f 4920 7769 6c6c 2062 6520 7265 7475  ROI will be retu
+00048da0: 726e 6564 2e20 4966 2046 6f72 6365 3d54  rned. If Force=T
+00048db0: 7275 652c 2074 6865 200a 2020 2020 2020  rue, the .      
+00048dc0: 2020 2020 2020 7375 6d20 524f 4920 7769        sum ROI wi
+00048dd0: 6c6c 2062 6520 7265 6372 6561 7465 642e  ll be recreated.
+00048de0: 0a0a 2020 2020 2020 2020 6578 636c 7564  ..        exclud
+00048df0: 6520 3a20 7374 722c 2064 6566 6175 6c74  e : str, default
+00048e00: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
+00048e10: 2020 4966 2073 6574 2074 6f20 6120 7374    If set to a st
+00048e20: 7269 6e67 2c20 7468 6520 6669 7273 7420  ring, the first 
+00048e30: 524f 4920 696e 2073 656c 662e 726f 6973  ROI in self.rois
+00048e40: 2077 6974 6820 7468 6174 206e 616d 6520   with that name 
+00048e50: 7769 6c6c 200a 2020 2020 2020 2020 2020  will .          
+00048e60: 2020 6265 2065 7863 6c75 6465 6420 6672    be excluded fr
+00048e70: 6f6d 2074 6865 2063 6f6d 6269 6e61 7469  om the combinati
+00048e80: 6f6e 2e20 5468 6973 206d 6179 2062 6520  on. This may be 
+00048e90: 7573 6566 756c 2069 6620 636f 6d70 6172  useful if compar
+00048ea0: 6973 6f6e 200a 2020 2020 2020 2020 2020  ison .          
+00048eb0: 2020 6f66 2061 2073 696e 676c 6520 524f    of a single RO
+00048ec0: 4920 7769 7468 2074 6865 2063 6f6e 7365  I with the conse
+00048ed0: 6e73 7573 206f 6620 616c 6c20 6f74 6865  nsus of all othe
+00048ee0: 7273 2069 7320 6465 7369 7265 642e 0a0a  rs is desired...
+00048ef0: 2020 2020 2020 2020 602a 2a60 6b77 6172          `**`kwar
+00048f00: 6773 203a 0a20 2020 2020 2020 2020 2020  gs :.           
+00048f10: 2045 7874 7261 206b 6579 776f 7264 2061   Extra keyword a
+00048f20: 7267 756d 656e 7473 2074 6f20 7061 7373  rguments to pass
+00048f30: 2074 6f20 7468 6520 6372 6561 7469 6f6e   to the creation
+00048f40: 206f 6620 7468 6520 524f 4920 6f62 6a65   of the ROI obje
+00048f50: 6374 0a20 2020 2020 2020 2020 2020 2072  ct.            r
+00048f60: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00048f70: 636f 6d62 696e 6174 696f 6e2e 0a20 2020  combination..   
+00048f80: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00048f90: 2020 7265 7475 726e 2073 656c 662e 5f67    return self._g
+00048fa0: 6574 5f63 6f6d 6269 6e61 7469 6f6e 2822  et_combination("
+00048fb0: 7375 6d22 2c20 666f 7263 652c 2065 7863  sum", force, exc
+00048fc0: 6c75 6465 2c20 0a20 2020 2020 2020 2020  lude, .         
+00048fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00048fe0: 2020 2020 2020 2020 2020 2020 6372 6561              crea
+00048ff0: 7465 5f72 6f69 5f73 756d 2c20 2a2a 6b77  te_roi_sum, **kw
+00049000: 6172 6773 290a 0a20 2020 2064 6566 2067  args)..    def g
+00049010: 6574 5f6f 7665 726c 6170 2873 656c 662c  et_overlap(self,
+00049020: 2066 6f72 6365 3d46 616c 7365 2c20 6578   force=False, ex
+00049030: 636c 7564 653d 4e6f 6e65 2c20 2a2a 6b77  clude=None, **kw
+00049040: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
+00049050: 2222 4765 7420 524f 4920 6f62 6a65 6374  ""Get ROI object
+00049060: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+00049070: 6520 6f76 6572 6c61 7020 6f66 2052 4f49  e overlap of ROI
+00049080: 7320 696e 2074 6869 7320 0a20 2020 2020  s in this .     
+00049090: 2020 2073 7472 7563 7475 7265 2073 6574     structure set
+000490a0: 2e20 4966 203c 6578 636c 7564 653e 2069  . If <exclude> i
+000490b0: 7320 7365 7420 746f 2061 2073 7472 696e  s set to a strin
+000490c0: 672c 2074 6865 2052 4f49 2077 6974 6820  g, the ROI with 
+000490d0: 7468 6174 206e 616d 6520 0a20 2020 2020  that name .     
+000490e0: 2020 2077 696c 6c20 6265 2065 7863 6c75     will be exclu
+000490f0: 6465 6420 6672 6f6d 2074 6865 2063 616c  ded from the cal
+00049100: 6375 6c61 7469 6f6e 2e0a 0a20 2020 2020  culation...     
+00049110: 2020 202a 2a50 6172 616d 6574 6572 733a     **Parameters:
+00049120: 2a2a 0a0a 2020 2020 2020 2020 666f 7263  **..        forc
+00049130: 6520 3a20 626f 6f6c 2c20 6465 6661 756c  e : bool, defaul
+00049140: 743d 4661 6c73 650a 2020 2020 2020 2020  t=False.        
+00049150: 2020 2020 4966 2046 616c 7365 2061 6e64      If False and
+00049160: 206f 7665 726c 6170 2052 4f49 2068 6173   overlap ROI has
+00049170: 2061 6c72 6561 6479 2062 6565 6e20 6372   already been cr
+00049180: 6561 7465 642c 2074 6865 200a 2020 2020  eated, the .    
+00049190: 2020 2020 2020 2020 7072 6576 696f 7573          previous
+000491a0: 6c79 2063 6f6d 7075 7465 6420 524f 4920  ly computed ROI 
+000491b0: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
+000491c0: 2e20 4966 2046 6f72 6365 3d54 7275 652c  . If Force=True,
+000491d0: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
+000491e0: 2020 6f76 6572 6c61 7020 524f 4920 7769    overlap ROI wi
+000491f0: 6c6c 2062 6520 7265 6372 6561 7465 642e  ll be recreated.
+00049200: 0a0a 2020 2020 2020 2020 6578 636c 7564  ..        exclud
+00049210: 6520 3a20 7374 722c 2064 6566 6175 6c74  e : str, default
+00049220: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
+00049230: 2020 4966 2073 6574 2074 6f20 6120 7374    If set to a st
+00049240: 7269 6e67 2c20 7468 6520 6669 7273 7420  ring, the first 
+00049250: 524f 4920 696e 2073 656c 662e 726f 6973  ROI in self.rois
+00049260: 2077 6974 6820 7468 6174 206e 616d 6520   with that name 
+00049270: 7769 6c6c 200a 2020 2020 2020 2020 2020  will .          
+00049280: 2020 6265 2065 7863 6c75 6465 6420 6672    be excluded fr
+00049290: 6f6d 2074 6865 2063 6f6d 6269 6e61 7469  om the combinati
+000492a0: 6f6e 2e20 5468 6973 206d 6179 2062 6520  on. This may be 
+000492b0: 7573 6566 756c 2069 6620 636f 6d70 6172  useful if compar
+000492c0: 6973 6f6e 200a 2020 2020 2020 2020 2020  ison .          
+000492d0: 2020 6f66 2061 2073 696e 676c 6520 524f    of a single RO
+000492e0: 4920 7769 7468 2074 6865 2063 6f6e 7365  I with the conse
+000492f0: 6e73 7573 206f 6620 616c 6c20 6f74 6865  nsus of all othe
+00049300: 7273 2069 7320 6465 7369 7265 642e 0a0a  rs is desired...
+00049310: 2020 2020 2020 2020 602a 2a60 6b77 6172          `**`kwar
+00049320: 6773 203a 0a20 2020 2020 2020 2020 2020  gs :.           
+00049330: 2045 7874 7261 206b 6579 776f 7264 2061   Extra keyword a
+00049340: 7267 756d 656e 7473 2074 6f20 7061 7373  rguments to pass
+00049350: 2074 6f20 7468 6520 6372 6561 7469 6f6e   to the creation
+00049360: 206f 6620 7468 6520 524f 4920 6f62 6a65   of the ROI obje
+00049370: 6374 0a20 2020 2020 2020 2020 2020 2072  ct.            r
+00049380: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+00049390: 636f 6d62 696e 6174 696f 6e2e 0a20 2020  combination..   
+000493a0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+000493b0: 2020 7265 7475 726e 2073 656c 662e 5f67    return self._g
+000493c0: 6574 5f63 6f6d 6269 6e61 7469 6f6e 2822  et_combination("
+000493d0: 6f76 6572 6c61 7022 2c20 666f 7263 652c  overlap", force,
+000493e0: 2065 7863 6c75 6465 2c20 0a20 2020 2020   exclude, .     
+000493f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00049400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00049410: 6372 6561 7465 5f72 6f69 5f6f 7665 726c  create_roi_overl
+00049420: 6170 2c20 2a2a 6b77 6172 6773 290a 0a20  ap, **kwargs).. 
+00049430: 2020 2064 6566 2074 7261 6e73 666f 726d     def transform
+00049440: 2873 656c 662c 2073 6361 6c65 3d31 2c20  (self, scale=1, 
+00049450: 7472 616e 736c 6174 696f 6e3d 5b30 2c20  translation=[0, 
+00049460: 302c 2030 5d2c 2072 6f74 6174 696f 6e3d  0, 0], rotation=
+00049470: 5b30 2c20 302c 2030 5d2c 0a20 2020 2020  [0, 0, 0],.     
+00049480: 2020 2020 2020 2063 656e 7472 653d 5b30         centre=[0
+00049490: 2c20 302c 2030 5d2c 2072 6573 616d 706c  , 0, 0], resampl
+000494a0: 653d 2266 696e 6522 2c20 7265 7374 6f72  e="fine", restor
+000494b0: 653d 5472 7565 2c20 0a20 2020 2020 2020  e=True, .       
+000494c0: 2020 2020 2066 696c 6c5f 7661 6c75 653d       fill_value=
+000494d0: 4e6f 6e65 2c20 666f 7263 655f 636f 6e74  None, force_cont
+000494e0: 6f75 7273 3d46 616c 7365 2c20 6e61 6d65  ours=False, name
+000494f0: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
+00049500: 2022 2222 0a20 2020 2020 2020 2041 7070   """.        App
+00049510: 6c79 2074 6872 6565 2d64 696d 656e 7369  ly three-dimensi
+00049520: 6f6e 616c 2073 696d 696c 6172 6974 7920  onal similarity 
+00049530: 7472 616e 7366 6f72 6d20 746f 2073 7472  transform to str
+00049540: 7563 7475 7265 2d73 6574 2052 4f49 732e  ucture-set ROIs.
+00049550: 0a0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
+00049560: 2074 7261 6e73 666f 726d 2063 6f72 7265   transform corre
+00049570: 7370 6f6e 6473 2074 6f20 6120 7472 616e  sponds to a tran
+00049580: 736c 6174 696f 6e20 616e 642f 6f72 2072  slation and/or r
+00049590: 6f74 6174 696f 6e0a 2020 2020 2020 2020  otation.        
+000495a0: 6162 6f75 7420 7468 6520 7a2d 6178 6973  about the z-axis
+000495b0: 2c20 616e 6420 6569 7468 6572 2074 6865  , and either the
+000495c0: 2072 6f69 2073 6f75 7263 6520 7479 7065   roi source type
+000495d0: 2069 7320 2264 6963 6f6d 220a 2020 2020   is "dicom".    
+000495e0: 2020 2020 6f72 2066 6f72 6365 2d63 6f6e      or force-con
+000495f0: 746f 7572 7320 6973 2054 7275 652c 2074  tours is True, t
+00049600: 6865 2074 7261 6e73 666f 726d 2069 7320  he transform is 
+00049610: 6170 706c 6965 6420 746f 2063 6f6e 746f  applied to conto
+00049620: 7572 0a20 2020 2020 2020 2070 6f69 6e74  ur.        point
+00049630: 7320 616e 6420 7468 6520 726f 6920 6d61  s and the roi ma
+00049640: 736b 2069 7320 7365 7420 6173 2075 6e6c  sk is set as unl
+00049650: 6f61 6465 642e 2020 4f74 6865 7277 6973  oaded.  Otherwis
+00049660: 6520 7468 6520 7472 616e 7366 6f72 6d0a  e the transform.
+00049670: 2020 2020 2020 2020 6973 2061 7070 6c69          is appli
+00049680: 6564 2074 6f20 7468 6520 6d61 736b 2061  ed to the mask a
+00049690: 6e64 2063 6f6e 746f 7572 7320 6172 6520  nd contours are 
+000496a0: 7365 7420 6173 2075 6e6c 6f61 6465 642e  set as unloaded.
+000496b0: 0a0a 2020 2020 2020 2020 5468 6520 7472  ..        The tr
+000496c0: 616e 7366 6f72 6d20 6973 2061 7070 6c69  ansform is appli
+000496d0: 6564 2069 6e20 7468 6520 6f72 6465 723a  ed in the order:
+000496e0: 2074 7261 6e73 6c61 7469 6f6e 2c20 7363   translation, sc
+000496f0: 616c 696e 672c 0a20 2020 2020 2020 2072  aling,.        r
+00049700: 6f74 6174 696f 6e2e 2020 5468 6520 6c61  otation.  The la
+00049710: 7474 6572 2074 776f 2061 7265 2061 626f  tter two are abo
+00049720: 7574 2074 6865 2063 656e 7472 6520 636f  ut the centre co
+00049730: 6f72 6469 6e61 7465 732e 0a0a 2020 2020  ordinates...    
+00049740: 2020 2020 2a2a 5061 7261 6d65 7465 7273      **Parameters
+00049750: 3a2a 2a0a 2020 2020 2020 2020 0a20 2020  :**.        .   
+00049760: 2020 2020 2066 6f72 6365 5f63 6f6e 746f       force_conto
+00049770: 7572 7320 3a20 626f 6f6c 2c20 6465 6661  urs : bool, defa
+00049780: 756c 743d 4661 6c73 650a 2020 2020 2020  ult=False.      
+00049790: 2020 2020 2020 4966 2054 7275 652c 2061        If True, a
+000497a0: 6e64 2074 6865 2074 7261 6e73 666f 726d  nd the transform
+000497b0: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+000497c0: 6120 7472 616e 736c 6174 696f 6e0a 2020  a translation.  
+000497d0: 2020 2020 2020 2020 2020 616e 642f 6f72            and/or
+000497e0: 2072 6f74 6174 696f 6e20 6162 6f75 7420   rotation about 
+000497f0: 7468 6520 7a2d 6178 6973 2c20 6170 706c  the z-axis, appl
+00049800: 7920 7472 616e 7366 6f72 6d20 746f 2063  y transform to c
+00049810: 6f6e 746f 7572 0a20 2020 2020 2020 2020  ontour.         
+00049820: 2020 2070 6f69 6e74 7320 696e 6465 7065     points indepe
+00049830: 6e64 656e 746c 7920 6f66 2074 6865 206f  ndently of the o
+00049840: 7269 6769 6e61 6c20 6461 7461 2073 6f75  riginal data sou
+00049850: 7263 652e 0a0a 2020 2020 2020 2020 6e61  rce...        na
+00049860: 6d65 7320 3a20 6c69 7374 2f4e 6f6e 652c  mes : list/None,
+00049870: 2064 6566 6175 6c74 3d46 616c 7365 0a20   default=False. 
+00049880: 2020 2020 2020 2020 2020 204c 6973 7420             List 
+00049890: 6f66 2052 4f49 7320 746f 2077 6869 6368  of ROIs to which
+000498a0: 2074 7261 6e73 666f 726d 2069 7320 746f   transform is to
+000498b0: 2062 6520 6170 706c 6965 642e 2020 4966   be applied.  If
+000498c0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000498d0: 2020 2074 7261 6e73 666f 726d 2069 7320     transform is 
+000498e0: 6170 706c 6965 6420 746f 2061 6c6c 2052  applied to all R
+000498f0: 4f49 732e 0a0a 2020 2020 2020 2020 466f  OIs...        Fo
+00049900: 7220 6f74 6865 7220 7061 7261 6d65 7465  r other paramete
+00049910: 7273 2c20 7365 6520 646f 6375 6d65 6e74  rs, see document
+00049920: 6174 696f 6e20 666f 720a 2020 2020 2020  ation for.      
+00049930: 2020 736b 7274 2e69 6d61 6765 2e49 6d61    skrt.image.Ima
+00049940: 6765 2e74 7261 6e73 666f 726d 2829 2e20  ge.transform(). 
+00049950: 204e 6f74 6520 7468 6174 2074 6865 2060   Note that the `
+00049960: 606f 7264 6572 6060 0a20 2020 2020 2020  `order``.       
+00049970: 2070 6172 616d 6574 6572 2069 736e 2774   parameter isn't
+00049980: 2061 7661 696c 6162 6c65 2066 6f72 2073   available for s
+00049990: 7472 7563 7475 7265 2d73 6574 2074 7261  tructure-set tra
+000499a0: 6e73 666f 726d 7320 2d20 6120 7661 6c75  nsforms - a valu
+000499b0: 6520 6f66 2030 0a20 2020 2020 2020 2069  e of 0.        i
+000499c0: 7320 7573 6564 2061 6c77 6179 732e 0a20  s used always.. 
+000499d0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+000499e0: 2020 2020 666f 7220 726f 6920 696e 2073      for roi in s
+000499f0: 656c 662e 6765 745f 726f 6973 286e 616d  elf.get_rois(nam
+00049a00: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+00049a10: 2072 6f69 2e74 7261 6e73 666f 726d 2873   roi.transform(s
+00049a20: 6361 6c65 2c20 7472 616e 736c 6174 696f  cale, translatio
+00049a30: 6e2c 2072 6f74 6174 696f 6e2c 2063 656e  n, rotation, cen
+00049a40: 7472 652c 2072 6573 616d 706c 652c 0a20  tre, resample,. 
+00049a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00049a60: 2020 2072 6573 746f 7265 2c20 6669 6c6c     restore, fill
+00049a70: 5f76 616c 7565 2c20 666f 7263 655f 636f  _value, force_co
+00049a80: 6e74 6f75 7273 290a 0a20 2020 2020 2020  ntours)..       
+00049a90: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00049aa0: 2020 6465 6620 6164 645f 706c 616e 2873    def add_plan(s
+00049ab0: 656c 662c 2070 6c61 6e29 3a0a 2020 2020  elf, plan):.    
+00049ac0: 2020 2020 2222 2241 6464 2061 2050 6c61      """Add a Pla
+00049ad0: 6e20 6f62 6a65 6374 2074 6f20 6265 2061  n object to be a
+00049ae0: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
+00049af0: 6869 7320 7374 7275 6374 7572 6520 7365  his structure se
+00049b00: 7420 616e 640a 2020 2020 2020 2020 6974  t and.        it
+00049b10: 7320 524f 4973 2e20 5468 6973 2064 6f65  s ROIs. This doe
+00049b20: 7320 6e6f 7420 6166 6665 6374 2074 6865  s not affect the
+00049b30: 2073 7472 7563 7475 7265 2073 6574 2061   structure set a
+00049b40: 7373 6f63 6961 7465 6420 7769 7468 0a20  ssociated with. 
+00049b50: 2020 2020 2020 2074 6865 2050 6c61 6e20         the Plan 
+00049b60: 6f62 6a65 6374 2e0a 0a20 2020 2020 2020  object...       
+00049b70: 202a 2a50 6172 616d 6574 6572 733a 2a2a   **Parameters:**
+00049b80: 0a0a 2020 2020 2020 2020 706c 616e 203a  ..        plan :
+00049b90: 2073 6b72 742e 646f 7365 2e50 6c61 6e0a   skrt.dose.Plan.
+00049ba0: 2020 2020 2020 2020 2020 2020 4120 506c              A Pl
+00049bb0: 616e 206f 626a 6563 7420 746f 2061 7373  an object to ass
+00049bc0: 6967 6e20 746f 2074 6869 7320 7374 7275  ign to this stru
+00049bd0: 6374 7572 6520 7365 742e 0a20 2020 2020  cture set..     
+00049be0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+00049bf0: 6966 206e 6f74 2070 6c61 6e20 696e 2073  if not plan in s
+00049c00: 656c 662e 706c 616e 733a 0a20 2020 2020  elf.plans:.     
+00049c10: 2020 2020 2020 2073 656c 662e 706c 616e         self.plan
+00049c20: 732e 6170 7065 6e64 2870 6c61 6e29 0a20  s.append(plan). 
+00049c30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00049c40: 706c 616e 732e 736f 7274 2829 0a0a 2020  plans.sort()..  
+00049c50: 2020 2020 2020 2020 2020 666f 7220 726f            for ro
+00049c60: 6920 696e 2073 656c 662e 726f 6973 3a0a  i in self.rois:.
+00049c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00049c80: 726f 692e 6164 645f 706c 616e 2870 6c61  roi.add_plan(pla
+00049c90: 6e29 0a0a 2020 2020 6465 6620 636c 6561  n)..    def clea
+00049ca0: 725f 706c 616e 7328 7365 6c66 293a 0a20  r_plans(self):. 
+00049cb0: 2020 2020 2020 2022 2222 436c 6561 7220         """Clear 
+00049cc0: 616c 6c20 706c 616e 206d 6170 7320 6173  all plan maps as
+00049cd0: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
+00049ce0: 6973 2073 7472 7563 7475 7265 2073 6574  is structure set
+00049cf0: 2e22 2222 0a0a 2020 2020 2020 2020 7365  ."""..        se
+00049d00: 6c66 2e70 6c61 6e73 203d 205b 5d0a 0a20  lf.plans = [].. 
+00049d10: 2020 2064 6566 2067 6574 5f70 6c61 6e73     def get_plans
+00049d20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00049d30: 2222 2252 6574 7572 6e20 6c69 7374 206f  """Return list o
+00049d40: 6620 506c 616e 206f 626a 6563 7473 2061  f Plan objects a
+00049d50: 7373 6f63 6961 7465 6420 7769 7468 2074  ssociated with t
+00049d60: 6869 7320 7374 7275 6374 7572 6520 7365  his structure se
+00049d70: 742e 2222 220a 0a20 2020 2020 2020 2072  t."""..        r
+00049d80: 6574 7572 6e20 7365 6c66 2e70 6c61 6e73  eturn self.plans
+00049d90: 0a0a 2020 2020 6465 6620 696e 7465 7270  ..    def interp
+00049da0: 6f6c 6174 655f 706f 696e 7473 2873 656c  olate_points(sel
+00049db0: 662c 206e 5f70 6f69 6e74 3d4e 6f6e 652c  f, n_point=None,
+00049dc0: 2064 7879 3d4e 6f6e 652c 0a20 2020 2020   dxy=None,.     
+00049dd0: 2020 2073 6d6f 6f74 686e 6573 735f 7065     smoothness_pe
+00049de0: 725f 706f 696e 743d 3029 3a0a 2020 2020  r_point=0):.    
+00049df0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00049e00: 5265 7475 726e 206e 6577 2053 7472 7563  Return new Struc
+00049e10: 7475 7265 5365 7420 6f62 6a65 6374 2c20  tureSet object, 
+00049e20: 7769 7468 2069 6e74 6572 706f 6c61 7465  with interpolate
+00049e30: 6420 636f 6e74 6f75 7220 706f 696e 7473  d contour points
+00049e40: 2e0a 0a20 2020 2020 2020 2050 6f69 6e74  ...        Point
+00049e50: 7320 6172 6520 696e 7465 7270 6f6c 6174  s are interpolat
+00049e60: 6564 2066 6f72 2065 6163 6820 636f 6e74  ed for each cont
+00049e70: 6f75 7220 6f66 2065 6163 6820 524f 492e  our of each ROI.
+00049e80: 0a0a 2020 2020 2020 2020 2a2a 5061 7261  ..        **Para
+00049e90: 6d65 7465 7273 3a2a 2a0a 0a20 2020 2020  meters:**..     
+00049ea0: 2020 206e 5f70 6f69 6e74 203a 2069 6e74     n_point : int
+00049eb0: 2c20 6465 6661 756c 743d 4e6f 6e65 0a20  , default=None. 
+00049ec0: 2020 2020 2020 2020 2020 204e 756d 6265             Numbe
+00049ed0: 7220 6f66 2070 6f69 6e74 7320 7065 7220  r of points per 
+00049ee0: 636f 6e74 6f75 722c 2061 6674 6572 2069  contour, after i
+00049ef0: 6e74 6572 706f 6c61 7469 6f6e 2e20 2054  nterpolation.  T
+00049f00: 6869 7320 6d75 7374 0a20 2020 2020 2020  his must.       
+00049f10: 2020 2020 2062 6520 7365 7420 746f 204e       be set to N
+00049f20: 6f6e 6520 666f 7220 6478 7920 746f 2062  one for dxy to b
+00049f30: 6520 636f 6e73 6964 6572 6564 2e0a 0a20  e considered... 
+00049f40: 2020 2020 2020 2064 7879 203a 2066 6c6f         dxy : flo
+00049f50: 6174 2c20 6465 6661 756c 743d 4e6f 6e65  at, default=None
+00049f60: 0a20 2020 2020 2020 2020 2020 2041 7070  .            App
+00049f70: 726f 7869 6d61 7465 2064 6973 7461 6e63  roximate distanc
+00049f80: 6520 7265 7175 6972 6564 2062 6574 7765  e required betwe
+00049f90: 656e 2063 6f6e 746f 7572 2070 6f69 6e74  en contour point
+00049fa0: 732e 2020 5468 6973 2069 7320 7461 6b65  s.  This is take
+00049fb0: 6e0a 2020 2020 2020 2020 2020 2020 696e  n.            in
+00049fc0: 746f 2061 6363 6f75 6e74 206f 6e6c 7920  to account only 
+00049fd0: 6966 206e 5f70 6f69 6e74 2069 7320 7365  if n_point is se
+00049fe0: 7420 746f 204e 6f6e 652e 2020 466f 7220  t to None.  For 
+00049ff0: 6120 636f 6e74 6f75 7220 6f66 0a20 2020  a contour of.   
+0004a000: 2020 2020 2020 2020 206c 656e 6774 6820           length 
+0004a010: 636f 6e74 6f75 725f 6c65 6e67 7468 2c20  contour_length, 
+0004a020: 7468 6520 6e75 6d62 6572 206f 6620 636f  the number of co
+0004a030: 6e74 6f75 7220 706f 696e 7473 2069 7320  ntour points is 
+0004a040: 7468 656e 2074 616b 656e 0a20 2020 2020  then taken.     
+0004a050: 2020 2020 2020 2074 6f20 6265 206d 6178         to be max
+0004a060: 2869 6e74 2863 6f6e 746f 7572 5f6c 656e  (int(contour_len
+0004a070: 6774 6820 2f20 6478 7929 2c20 3329 2e20  gth / dxy), 3). 
+0004a080: 200a 0a20 2020 2020 2020 2073 6d6f 6f74   ..        smoot
+0004a090: 686e 6573 735f 7065 725f 706f 696e 7420  hness_per_point 
+0004a0a0: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
+0004a0b0: 3d30 0a20 2020 2020 2020 2020 2020 2050  =0.            P
+0004a0c0: 6172 616d 6574 6572 2064 6574 6572 6d69  arameter determi
+0004a0d0: 6e69 6e67 2074 6865 2073 6d6f 6f74 686e  ning the smoothn
+0004a0e0: 6573 7320 6f66 2074 6865 2042 2d73 706c  ess of the B-spl
+0004a0f0: 696e 6520 6375 7276 6520 7573 6564 0a20  ine curve used. 
+0004a100: 2020 2020 2020 2020 2020 2069 6e20 636f             in co
+0004a110: 6e74 6f75 7220 6170 7072 6f78 696d 6174  ntour approximat
+0004a120: 696f 6e20 666f 7220 696e 7465 7270 6f6c  ion for interpol
+0004a130: 6174 696f 6e2e 2020 5468 6520 7072 6f64  ation.  The prod
+0004a140: 7563 7420 6f66 0a20 2020 2020 2020 2020  uct of.         
+0004a150: 2020 2073 6d6f 6f74 686e 6573 735f 7065     smoothness_pe
+0004a160: 725f 706f 696e 7420 616e 6420 7468 6520  r_point and the 
+0004a170: 6e75 6d62 6572 206f 6620 636f 6e74 6f75  number of contou
+0004a180: 7220 706f 696e 7473 2028 7370 6563 6966  r points (specif
+0004a190: 6965 640a 2020 2020 2020 2020 2020 2020  ied.            
+0004a1a0: 6469 7265 6374 6c79 2076 6961 206e 5f70  directly via n_p
+0004a1b0: 6f69 6e74 2c20 6f72 2069 6e64 6972 6563  oint, or indirec
+0004a1c0: 746c 7920 7669 6120 6478 7929 2063 6f72  tly via dxy) cor
+0004a1d0: 7265 7370 6f6e 6473 2074 6f20 7468 650a  responds to the.
+0004a1e0: 2020 2020 2020 2020 2020 2020 7061 7261              para
+0004a1f0: 6d65 7465 7220 7320 6f66 2073 6369 7079  meter s of scipy
+0004a200: 2e69 6e74 6572 706f 6c61 7465 2e73 706c  .interpolate.spl
+0004a210: 7072 6570 202d 2073 6565 2064 6f63 756d  prep - see docum
+0004a220: 656e 7461 7469 6f6e 2061 743a 0a20 2020  entation at:.   
+0004a230: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+0004a240: 2020 6874 7470 733a 2f2f 7363 6970 792e    https://scipy.
+0004a250: 6769 7468 7562 2e69 6f2f 6465 7664 6f63  github.io/devdoc
+0004a260: 732f 7265 6665 7265 6e63 652f 6765 6e65  s/reference/gene
+0004a270: 7261 7465 642f 7363 6970 792e 696e 7465  rated/scipy.inte
+0004a280: 7270 6f6c 6174 652e 7370 6c70 7265 702e  rpolate.splprep.
+0004a290: 6874 6d6c 2373 6369 7079 2e69 6e74 6572  html#scipy.inter
+0004a2a0: 706f 6c61 7465 2e73 706c 7072 6570 0a0a  polate.splprep..
+0004a2b0: 2020 2020 2020 2020 2020 2020 4120 736d              A sm
+0004a2c0: 6f6f 7468 6e65 7373 5f70 6572 5f70 6f69  oothness_per_poi
+0004a2d0: 6e74 206f 6620 3020 666f 7263 6573 2074  nt of 0 forces t
+0004a2e0: 6865 2042 2d73 706c 696e 6520 746f 2070  he B-spline to p
+0004a2f0: 6173 7320 7468 726f 7567 680a 2020 2020  ass through.    
+0004a300: 2020 2020 2020 2020 616c 6c20 6f66 2074          all of t
+0004a310: 6865 2070 7265 2d69 6e74 6572 706f 6c61  he pre-interpola
+0004a320: 7469 6f6e 2063 6f6e 746f 7572 2070 6f69  tion contour poi
+0004a330: 6e74 732e 0a20 2020 2020 2020 2027 2727  nts..        '''
+0004a340: 0a0a 2020 2020 2020 2020 2320 496e 7465  ..        # Inte
+0004a350: 7270 6f6c 6174 6520 706f 696e 7473 2066  rpolate points f
+0004a360: 6f72 2074 6865 2072 6f69 730a 2020 2020  or the rois.    
+0004a370: 2020 2020 726f 6973 203d 205b 5d0a 2020      rois = [].  
+0004a380: 2020 2020 2020 666f 7220 726f 6920 696e        for roi in
+0004a390: 2073 656c 662e 6765 745f 726f 6973 2829   self.get_rois()
+0004a3a0: 3a0a 2020 2020 2020 2020 2020 2020 726f  :.            ro
+0004a3b0: 6973 2e61 7070 656e 6428 726f 692e 696e  is.append(roi.in
+0004a3c0: 7465 7270 6f6c 6174 655f 706f 696e 7473  terpolate_points
+0004a3d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0004a3e0: 2020 6e5f 706f 696e 742c 2064 7879 2c20    n_point, dxy, 
+0004a3f0: 736d 6f6f 7468 6e65 7373 5f70 6572 5f70  smoothness_per_p
+0004a400: 6f69 6e74 2929 0a0a 2020 2020 2020 2020  oint))..        
+0004a410: 2320 436c 6f6e 6520 7365 6c66 2c20 7468  # Clone self, th
+0004a420: 656e 2072 6573 6574 2073 6f75 7263 6520  en reset source 
+0004a430: 616e 6420 726f 6973 0a20 2020 2020 2020  and rois.       
+0004a440: 2073 7320 3d20 5374 7275 6374 7572 6553   ss = StructureS
+0004a450: 6574 2873 656c 6629 0a20 2020 2020 2020  et(self).       
+0004a460: 2073 732e 736f 7572 6365 7320 3d20 726f   ss.sources = ro
+0004a470: 6973 0a20 2020 2020 2020 2073 732e 726f  is.        ss.ro
+0004a480: 6973 203d 2072 6f69 730a 0a20 2020 2020  is = rois..     
+0004a490: 2020 2072 6574 7572 6e20 7373 0a0a 2020     return ss..  
+0004a4a0: 2020 6465 6620 6f72 6465 725f 726f 6973    def order_rois
+0004a4b0: 2873 656c 662c 206f 7264 6572 3d27 782b  (self, order='x+
+0004a4c0: 2729 3a0a 2020 2020 2020 2020 2727 270a  '):.        '''.
+0004a4d0: 2020 2020 2020 2020 4f72 6465 7220 524f          Order RO
+0004a4e0: 4973 2062 7920 6f6e 6520 6f66 2074 6865  Is by one of the
+0004a4f0: 6972 2063 656e 7472 6f69 6420 636f 6f72  ir centroid coor
+0004a500: 6469 6e61 7465 732e 0a0a 2020 2020 2020  dinates...      
+0004a510: 2020 2a2a 5061 7261 6d65 7465 723a 2a2a    **Parameter:**
+0004a520: 0a0a 2020 2020 2020 2020 6f72 6465 7220  ..        order 
+0004a530: 3a20 7374 722c 2064 6566 6175 6c74 3d27  : str, default='
+0004a540: 782b 270a 2020 2020 2020 2020 2020 2020  x+'.            
+0004a550: 5370 6563 6966 6963 6174 696f 6e20 6f66  Specification of
+0004a560: 2077 6179 2069 7420 7768 6963 6820 524f   way it which RO
+0004a570: 4973 2061 7265 2074 6f20 6265 206f 7264  Is are to be ord
+0004a580: 6572 643a 0a20 2020 2020 2020 2020 2020  erd:.           
+0004a590: 202d 2027 782b 2720 3a20 696e 206f 7264   - 'x+' : in ord
+0004a5a0: 6572 206f 6620 696e 6372 6561 7369 6e67  er of increasing
+0004a5b0: 2078 2076 616c 7565 2e0a 2020 2020 2020   x value..      
+0004a5c0: 2020 2020 2020 2d20 2778 2d27 203a 2069        - 'x-' : i
+0004a5d0: 6e20 6f72 6465 7220 6f66 2064 6563 7265  n order of decre
+0004a5e0: 6173 696e 6720 7820 7661 6c75 652e 0a20  asing x value.. 
+0004a5f0: 2020 2020 2020 2020 2020 202d 2027 792b             - 'y+
+0004a600: 2720 3a20 696e 206f 7264 6572 206f 6620  ' : in order of 
+0004a610: 696e 6372 6561 7369 6e67 2079 2076 616c  increasing y val
+0004a620: 7565 2e0a 2020 2020 2020 2020 2020 2020  ue..            
+0004a630: 2d20 2779 2d27 203a 2069 6e20 6f72 6465  - 'y-' : in orde
+0004a640: 7220 6f66 2064 6563 7265 6173 696e 6720  r of decreasing 
+0004a650: 7920 7661 6c75 652e 0a20 2020 2020 2020  y value..       
+0004a660: 2020 2020 202d 2027 7a2b 2720 3a20 696e       - 'z+' : in
+0004a670: 206f 7264 6572 206f 6620 696e 6372 6561   order of increa
+0004a680: 7369 6e67 207a 2076 616c 7565 2e0a 2020  sing z value..  
+0004a690: 2020 2020 2020 2020 2020 2d20 277a 2d27            - 'z-'
+0004a6a0: 203a 2069 6e20 6f72 6465 7220 6f66 2064   : in order of d
+0004a6b0: 6563 7265 6173 696e 6720 7a20 7661 6c75  ecreasing z valu
+0004a6c0: 652e 0a20 2020 2020 2020 2027 2727 0a0a  e..        '''..
+0004a6d0: 2020 2020 2020 2020 6966 206f 7264 6572          if order
+0004a6e0: 206e 6f74 2069 6e20 5b27 782b 272c 2027   not in ['x+', '
+0004a6f0: 782d 272c 2027 792b 272c 2027 792d 272c  x-', 'y+', 'y-',
+0004a700: 2027 7a2b 272c 2027 7a2d 275d 3a0a 2020   'z+', 'z-']:.  
+0004a710: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0004a720: 0a0a 2020 2020 2020 2020 2320 4465 7465  ..        # Dete
+0004a730: 726d 696e 6520 6178 6973 2066 6f72 206f  rmine axis for o
+0004a740: 7264 6572 696e 672c 2061 6e64 2064 6972  rdering, and dir
+0004a750: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
+0004a760: 6178 6973 203d 2027 7879 7a27 2e66 696e  axis = 'xyz'.fin
+0004a770: 6428 6f72 6465 725b 305d 290a 2020 2020  d(order[0]).    
+0004a780: 2020 2020 7265 7665 7273 6520 3d20 2827      reverse = ('
+0004a790: 2d27 2069 6e20 6f72 6465 7229 0a0a 2020  -' in order)..  
+0004a7a0: 2020 2020 2020 2320 4372 6561 7465 2064        # Create d
+0004a7b0: 6963 7469 6f6e 6172 7920 7768 6572 6520  ictionary where 
+0004a7c0: 6b65 7973 2061 7265 2063 656e 7472 6f69  keys are centroi
+0004a7d0: 6420 636f 6f72 6469 6e61 7465 730a 2020  d coordinates.  
+0004a7e0: 2020 2020 2020 2320 616e 6420 7661 6c75        # and valu
+0004a7f0: 6573 2061 7265 206c 6973 7473 206f 6620  es are lists of 
+0004a800: 524f 4920 696e 6469 6369 6573 2061 7420  ROI indicies at 
+0004a810: 7468 6573 6520 636f 6f72 6469 6e61 7465  these coordinate
+0004a820: 732e 0a20 2020 2020 2020 2063 656e 7472  s..        centr
+0004a830: 6f69 6473 203d 207b 7d0a 2020 2020 2020  oids = {}.      
+0004a840: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0004a850: 286c 656e 2873 656c 662e 726f 6973 2929  (len(self.rois))
+0004a860: 3a0a 2020 2020 2020 2020 2020 2020 7879  :.            xy
+0004a870: 7a20 3d20 7365 6c66 2e72 6f69 735b 695d  z = self.rois[i]
+0004a880: 2e67 6574 5f63 656e 7472 6f69 6428 295b  .get_centroid()[
+0004a890: 6178 6973 5d0a 2020 2020 2020 2020 2020  axis].          
+0004a8a0: 2020 6966 2078 797a 206e 6f74 2069 6e20    if xyz not in 
+0004a8b0: 6365 6e74 726f 6964 733a 0a20 2020 2020  centroids:.     
+0004a8c0: 2020 2020 2020 2020 2020 2063 656e 7472             centr
+0004a8d0: 6f69 6473 5b78 797a 5d20 3d20 5b5d 0a20  oids[xyz] = []. 
+0004a8e0: 2020 2020 2020 2020 2020 2063 656e 7472             centr
+0004a8f0: 6f69 6473 5b78 797a 5d2e 6170 7065 6e64  oids[xyz].append
+0004a900: 2869 290a 0a20 2020 2020 2020 2023 2043  (i)..        # C
+0004a910: 7265 6174 6520 6c69 7374 206f 6620 524f  reate list of RO
+0004a920: 4973 206f 7264 6572 6564 2062 7920 6365  Is ordered by ce
+0004a930: 6e74 726f 6964 2063 6f6f 7264 696e 6174  ntroid coordinat
+0004a940: 652e 0a20 2020 2020 2020 2072 6f69 7320  e..        rois 
+0004a950: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+0004a960: 2063 656e 7472 6f69 6420 696e 2073 6f72   centroid in sor
+0004a970: 7465 6428 6365 6e74 726f 6964 732c 2072  ted(centroids, r
+0004a980: 6576 6572 7365 3d72 6576 6572 7365 293a  everse=reverse):
+0004a990: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0004a9a0: 2069 2069 6e20 6365 6e74 726f 6964 735b   i in centroids[
+0004a9b0: 6365 6e74 726f 6964 5d3a 0a20 2020 2020  centroid]:.     
+0004a9c0: 2020 2020 2020 2020 2020 2072 6f69 732e             rois.
+0004a9d0: 6170 7065 6e64 2873 656c 662e 726f 6973  append(self.rois
+0004a9e0: 5b69 5d29 0a0a 2020 2020 2020 2020 2320  [i])..        # 
+0004a9f0: 5374 6f72 6520 7468 6520 6e65 7720 6f72  Store the new or
+0004aa00: 6465 7220 6f66 2052 4f49 732e 0a20 2020  der of ROIs..   
+0004aa10: 2020 2020 2073 656c 662e 726f 6973 203d       self.rois =
+0004aa20: 2072 6f69 730a 0a20 2020 2064 6566 2063   rois..    def c
+0004aa30: 6f6d 6269 6e65 5f72 6f69 7328 7365 6c66  ombine_rois(self
+0004aa40: 2c20 6e61 6d65 3d4e 6f6e 652c 2072 6f69  , name=None, roi
+0004aa50: 5f6e 616d 6573 3d4e 6f6e 652c 2069 6d61  _names=None, ima
+0004aa60: 6765 3d4e 6f6e 652c 206d 6574 686f 643d  ge=None, method=
+0004aa70: 4e6f 6e65 293a 0a20 2020 2020 2020 2027  None):.        '
+0004aa80: 2727 0a20 2020 2020 2020 2043 6f6d 6269  ''.        Combi
+0004aa90: 6e65 2074 776f 206f 7220 6d6f 7265 2052  ne two or more R
+0004aaa0: 4f49 7320 6173 2061 2073 696e 676c 6520  OIs as a single 
+0004aab0: 524f 492e 0a0a 2020 2020 2020 2020 2a2a  ROI...        **
+0004aac0: 5061 7261 6d65 7465 7273 3a2a 2a0a 0a20  Parameters:**.. 
+0004aad0: 2020 2020 2020 206e 616d 6520 3a20 7374         name : st
+0004aae0: 722c 2064 6566 6175 6c74 3d4e 6f6e 650a  r, default=None.
+0004aaf0: 2020 2020 2020 2020 2020 2020 4e61 6d65              Name
+0004ab00: 2074 6f20 6265 2067 6976 656e 2074 6f20   to be given to 
+0004ab10: 7468 6520 636f 6d70 6f73 6974 6520 524f  the composite RO
+0004ab20: 492e 2020 4966 204e 6f6e 652c 2074 6865  I.  If None, the
+0004ab30: 0a20 2020 2020 2020 2020 2020 206e 616d  .            nam
+0004ab40: 6520 6173 7369 676e 6564 2069 7320 666f  e assigned is fo
+0004ab50: 726d 6564 2062 7920 6a6f 696e 696e 6720  rmed by joining 
+0004ab60: 746f 6765 7468 6572 2074 6865 206e 616d  together the nam
+0004ab70: 6573 0a20 2020 2020 2020 2020 2020 206f  es.            o
+0004ab80: 6620 7468 6520 6f72 6967 696e 616c 2052  f the original R
+0004ab90: 4f49 732e 0a0a 2020 2020 2020 2020 726f  OIs...        ro
+0004aba0: 695f 6e61 6d65 7320 3a20 6c69 7374 2c20  i_names : list, 
+0004abb0: 6465 6661 756c 743d 4e6f 6e65 0a20 2020  default=None.   
+0004abc0: 2020 2020 2020 2020 204c 6973 7420 6f66           List of
+0004abd0: 206e 616d 6573 206f 6620 524f 4973 2074   names of ROIs t
+0004abe0: 6f20 6265 2063 6f6d 6269 6e65 642e 2020  o be combined.  
+0004abf0: 4966 204e 6f6e 652c 2061 6c6c 206f 6620  If None, all of 
+0004ac00: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0004ac10: 7374 7275 6374 7572 6520 7365 7427 7320  structure set's 
+0004ac20: 524f 4973 2061 7265 2063 6f6d 6269 6e65  ROIs are combine
+0004ac30: 642e 0a0a 2020 2020 2020 2020 696d 6167  d...        imag
+0004ac40: 6520 3a20 736b 7274 2e69 6d61 6765 2e49  e : skrt.image.I
+0004ac50: 6d61 6765 2c20 6465 6661 756c 743d 4e6f  mage, default=No
+0004ac60: 6e65 0a20 2020 2020 2020 2020 2020 2049  ne.            I
+0004ac70: 6d61 6765 2074 6f20 7365 7420 666f 7220  mage to set for 
+0004ac80: 7468 6520 636f 6d70 6f73 6974 6520 524f  the composite RO
+0004ac90: 492e 2020 4966 204e 6f6e 652c 2075 7365  I.  If None, use
+0004aca0: 2074 6865 2069 6d61 6765 0a20 2020 2020   the image.     
+0004acb0: 2020 2020 2020 206f 6620 7468 6520 524f         of the RO
+0004acc0: 4920 7769 7468 2074 6865 2066 6972 7374  I with the first
+0004acd0: 2069 6e20 3c72 6f69 5f6e 616d 6573 3e2e   in <roi_names>.
+0004ace0: 0a0a 2020 2020 2020 2020 6d65 7468 6f64  ..        method
+0004acf0: 203a 2073 7472 2c20 6465 6661 756c 743d   : str, default=
+0004ad00: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0004ad10: 204d 6574 686f 6420 746f 2075 7365 2066   Method to use f
+0004ad20: 6f72 2063 6f6d 6269 6e69 6e67 2052 4f49  or combining ROI
+0004ad30: 732e 2020 4361 6e20 6265 3a20 0a0a 2020  s.  Can be: ..  
+0004ad40: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+0004ad50: 2263 6f6e 746f 7572 223a 2074 616b 6520  "contour": take 
+0004ad60: 756e 6172 7920 756e 696f 6e20 6f66 2073  unary union of s
+0004ad70: 6861 7065 6c79 2070 6f6c 7967 6f6e 732e  hapely polygons.
+0004ad80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0004ad90: 202d 2022 6d61 736b 223a 2073 756d 2062   - "mask": sum b
+0004ada0: 696e 6172 7920 6d61 736b 732e 0a20 2020  inary masks..   
+0004adb0: 2020 2020 2020 2020 2020 2020 202d 2022               - "
+0004adc0: 6175 746f 223a 2075 7365 2074 6865 2064  auto": use the d
+0004add0: 6566 6175 6c74 5f67 656f 6d5f 6d65 7468  efault_geom_meth
+0004ade0: 6f64 206f 6620 7468 6520 524f 4920 7769  od of the ROI wi
+0004adf0: 7468 2074 6865 0a20 2020 2020 2020 2020  th the.         
+0004ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004ae10: 2066 6972 7374 206e 616d 6520 696e 203c   first name in <
+0004ae20: 726f 695f 6e61 6d65 733e 2e0a 0a20 2020  roi_names>...   
+0004ae30: 2020 2020 2020 2020 2049 6620 4e6f 6e65           If None
+0004ae40: 2c20 2261 7574 6f22 2069 7320 7573 6564  , "auto" is used
+0004ae50: 2e0a 2020 2020 2020 2020 2727 270a 0a20  ..        '''.. 
+0004ae60: 2020 2020 2020 2023 2049 6620 4e6f 6e65         # If None
+0004ae70: 2076 616c 7565 7320 7061 7373 6564 2c20   values passed, 
+0004ae80: 7365 7420 6465 6661 756c 7420 6265 6861  set default beha
+0004ae90: 7669 6f75 722e 0a20 2020 2020 2020 2069  viour..        i
+0004aea0: 6620 726f 695f 6e61 6d65 7320 6973 204e  f roi_names is N
+0004aeb0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0004aec0: 2072 6f69 5f6e 616d 6573 203d 2073 656c   roi_names = sel
+0004aed0: 662e 6765 745f 726f 695f 6e61 6d65 7328  f.get_roi_names(
+0004aee0: 290a 2020 2020 2020 2020 6966 206e 616d  ).        if nam
+0004aef0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+0004af00: 2020 2020 2020 206e 616d 6520 3d20 272b         name = '+
+0004af10: 272e 6a6f 696e 2872 6f69 5f6e 616d 6573  '.join(roi_names
+0004af20: 290a 2020 2020 2020 2020 6966 206d 6574  ).        if met
+0004af30: 686f 6420 696e 205b 4e6f 6e65 2c20 2261  hod in [None, "a
+0004af40: 7574 6f22 5d3a 0a20 2020 2020 2020 2020  uto"]:.         
+0004af50: 2020 206d 6574 686f 6420 3d20 7365 6c66     method = self
+0004af60: 5b72 6f69 5f6e 616d 6573 5b30 5d5d 2e64  [roi_names[0]].d
+0004af70: 6566 6175 6c74 5f67 656f 6d5f 6d65 7468  efault_geom_meth
+0004af80: 6f64 0a20 2020 2020 2020 2069 6620 696d  od.        if im
+0004af90: 6167 6520 6973 204e 6f6e 653a 0a20 2020  age is None:.   
+0004afa0: 2020 2020 2020 2020 2069 6d61 6765 203d           image =
+0004afb0: 2073 656c 665b 726f 695f 6e61 6d65 735b   self[roi_names[
+0004afc0: 305d 5d2e 696d 6167 650a 0a20 2020 2020  0]].image..     
+0004afd0: 2020 2069 6620 2263 6f6e 746f 7572 2220     if "contour" 
+0004afe0: 3d3d 206d 6574 686f 643a 0a20 2020 2020  == method:.     
+0004aff0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+0004b000: 6120 6469 6374 696f 6e61 7279 2063 6f6e  a dictionary con
+0004b010: 7461 696e 696e 6720 706f 6c79 676f 6e73  taining polygons
+0004b020: 2066 6f72 2061 6c6c 2052 4f49 732e 0a20   for all ROIs.. 
+0004b030: 2020 2020 2020 2020 2020 2061 6c6c 5f70             all_p
+0004b040: 6f6c 7967 6f6e 7320 3d20 7b7d 0a20 2020  olygons = {}.   
+0004b050: 2020 2020 2020 2020 2066 6f72 2072 6f69           for roi
+0004b060: 2069 6e20 7365 6c66 2e67 6574 5f72 6f69   in self.get_roi
+0004b070: 7328 726f 695f 6e61 6d65 7329 3a0a 2020  s(roi_names):.  
+0004b080: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0004b090: 7220 6b65 792c 2070 6f6c 7967 6f6e 7320  r key, polygons 
+0004b0a0: 696e 2072 6f69 2e67 6574 5f70 6f6c 7967  in roi.get_polyg
+0004b0b0: 6f6e 7328 292e 6974 656d 7328 293a 0a20  ons().items():. 
 0004b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004b0d0: 2020 2020 616c 6c5f 706f 6c79 676f 6e73      all_polygons
-0004b0e0: 5b6b 6579 5d20 3d20 5b5d 0a20 2020 2020  [key] = [].     
-0004b0f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0004b100: 6c6c 5f70 6f6c 7967 6f6e 735b 6b65 795d  ll_polygons[key]
-0004b110: 2e65 7874 656e 6428 706f 6c79 676f 6e73  .extend(polygons
-0004b120: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-0004b130: 2045 7661 6c75 6174 6520 7468 6520 756e   Evaluate the un
-0004b140: 6172 7920 756e 696f 6e20 6f66 2070 6f6c  ary union of pol
-0004b150: 7967 6f6e 7320 666f 7220 6561 6368 2073  ygons for each s
-0004b160: 6c69 6365 2e0a 2020 2020 2020 2020 2020  lice..          
-0004b170: 2020 616c 6c5f 706f 6c79 676f 6e73 203d    all_polygons =
-0004b180: 207b 6b65 793a 205b 6f70 732e 756e 6172   {key: [ops.unar
-0004b190: 795f 756e 696f 6e28 616c 6c5f 706f 6c79  y_union(all_poly
-0004b1a0: 676f 6e73 5b6b 6579 5d29 5d0a 2020 2020  gons[key])].    
-0004b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004b1c0: 2066 6f72 206b 6579 2069 6e20 616c 6c5f   for key in all_
-0004b1d0: 706f 6c79 676f 6e73 7d0a 0a20 2020 2020  polygons}..     
-0004b1e0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-0004b1f0: 7468 6520 636f 6d70 6f73 6974 6520 524f  the composite RO
-0004b200: 492e 0a20 2020 2020 2020 2020 2020 2072  I..            r
-0004b210: 6f69 5f6e 6577 203d 2052 4f49 2873 6f75  oi_new = ROI(sou
-0004b220: 7263 653d 616c 6c5f 706f 6c79 676f 6e73  rce=all_polygons
-0004b230: 2c20 696d 6167 653d 696d 6167 652c 206e  , image=image, n
-0004b240: 616d 653d 6e61 6d65 290a 0a20 2020 2020  ame=name)..     
-0004b250: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0004b260: 2020 2020 2023 2055 7365 2064 6174 6120       # Use data 
-0004b270: 6672 6f6d 206f 6e65 206f 6620 7468 6520  from one of the 
-0004b280: 524f 4973 2061 7320 6120 7374 6172 7469  ROIs as a starti
-0004b290: 6e67 2070 6f69 6e74 2e0a 2020 2020 2020  ng point..      
-0004b2a0: 2020 2020 2020 726f 6930 203d 2073 656c        roi0 = sel
-0004b2b0: 662e 6765 745f 726f 6928 726f 695f 6e61  f.get_roi(roi_na
-0004b2c0: 6d65 735b 305d 290a 2020 2020 2020 2020  mes[0]).        
-0004b2d0: 2020 2020 726f 695f 6e65 7720 3d20 524f      roi_new = RO
-0004b2e0: 4928 736f 7572 6365 3d72 6f69 302e 6765  I(source=roi0.ge
-0004b2f0: 745f 6d61 736b 2829 2c20 6166 6669 6e65  t_mask(), affine
-0004b300: 3d72 6f69 302e 6166 6669 6e65 2c0a 2020  =roi0.affine,.  
-0004b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004b320: 2020 6e61 6d65 3d6e 616d 652c 2069 6d61    name=name, ima
-0004b330: 6765 3d69 6d61 6765 290a 0a20 2020 2020  ge=image)..     
-0004b340: 2020 2020 2020 2023 2043 6f6d 6269 6e65         # Combine
-0004b350: 2077 6974 6820 6461 7461 2066 726f 6d20   with data from 
-0004b360: 7468 6520 6f74 6865 7220 524f 4973 2e0a  the other ROIs..
-0004b370: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0004b380: 6920 696e 2072 616e 6765 2831 2c20 6c65  i in range(1, le
-0004b390: 6e28 726f 695f 6e61 6d65 7329 293a 0a20  n(roi_names)):. 
-0004b3a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0004b3b0: 6f69 5f6e 6577 2e6d 6173 6b2e 6461 7461  oi_new.mask.data
-0004b3c0: 202b 3d20 7365 6c66 2e67 6574 5f72 6f69   += self.get_roi
-0004b3d0: 2872 6f69 5f6e 616d 6573 5b69 5d29 2e67  (roi_names[i]).g
-0004b3e0: 6574 5f6d 6173 6b28 290a 0a20 2020 2020  et_mask()..     
-0004b3f0: 2020 2072 6574 7572 6e20 726f 695f 6e65     return roi_ne
-0004b400: 770a 0a20 2020 2064 6566 2067 6574 5f6d  w..    def get_m
-0004b410: 6173 6b5f 696d 6167 6528 7365 6c66 2c20  ask_image(self, 
-0004b420: 6e61 6d65 3d4e 6f6e 6529 3a0a 2020 2020  name=None):.    
-0004b430: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0004b440: 4765 7420 696d 6167 6520 6f62 6a65 6374  Get image object
-0004b450: 2072 6570 7265 7365 6e74 696e 6720 6d61   representing ma
-0004b460: 736b 2066 6f72 2061 6c6c 2052 4f49 7320  sk for all ROIs 
-0004b470: 6f66 2073 7472 7563 7475 7265 2073 6574  of structure set
-0004b480: 2e0a 0a20 2020 2020 2020 202a 2a50 6172  ...        **Par
-0004b490: 616d 6574 6572 733a 2a2a 0a0a 2020 2020  ameters:**..    
-0004b4a0: 2020 2020 6e61 6d65 203a 2073 7472 2c20      name : str, 
-0004b4b0: 6465 6661 756c 743d 4e6f 6e65 0a20 2020  default=None.   
-0004b4c0: 2020 2020 2020 2020 204e 616d 6520 746f           Name to
-0004b4d0: 2062 6520 6769 7665 6e20 746f 2074 6865   be given to the
-0004b4e0: 206d 6173 6b20 696d 6167 652e 2020 4966   mask image.  If
-0004b4f0: 204e 6f6e 652c 2074 6865 0a20 2020 2020   None, the.     
-0004b500: 2020 2020 2020 206e 616d 6520 6173 7369         name assi
-0004b510: 676e 6564 2069 7320 7468 6520 6e61 6d65  gned is the name
-0004b520: 206f 6620 7468 6520 7374 7275 6374 7572   of the structur
-0004b530: 6520 7365 742c 2077 6974 6820 7375 6666  e set, with suff
-0004b540: 6978 0a20 2020 2020 2020 2020 2020 2022  ix.            "
-0004b550: 5f6d 6173 6b22 2061 7070 656e 6465 642e  _mask" appended.
-0004b560: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0004b570: 2020 2020 206e 616d 6520 3d20 6e61 6d65       name = name
-0004b580: 206f 7220 6622 7b73 656c 662e 6e61 6d65   or f"{self.name
-0004b590: 7d5f 6d61 736b 220a 2020 2020 2020 2020  }_mask".        
-0004b5a0: 726f 695f 636f 6d62 696e 6564 203d 2073  roi_combined = s
-0004b5b0: 656c 662e 636f 6d62 696e 655f 726f 6973  elf.combine_rois
-0004b5c0: 286e 616d 653d 6e61 6d65 290a 2020 2020  (name=name).    
-0004b5d0: 2020 2020 6d61 736b 5f69 6d61 6765 203d      mask_image =
-0004b5e0: 2072 6f69 5f63 6f6d 6269 6e65 642e 6765   roi_combined.ge
-0004b5f0: 745f 6d61 736b 5f69 6d61 6765 2829 0a20  t_mask_image(). 
-0004b600: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
-0004b610: 736b 5f69 6d61 6765 0a0a 2020 2020 6465  sk_image..    de
-0004b620: 6620 6372 6f70 2873 656c 662c 2078 6c69  f crop(self, xli
-0004b630: 6d3d 4e6f 6e65 2c20 796c 696d 3d4e 6f6e  m=None, ylim=Non
-0004b640: 652c 207a 6c69 6d3d 4e6f 6e65 293a 0a20  e, zlim=None):. 
-0004b650: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0004b660: 2020 2043 726f 7020 616c 6c20 524f 4973     Crop all ROIs
-0004b670: 206f 6620 5374 7275 6374 7572 6553 6574   of StructureSet
-0004b680: 2074 6f20 7370 6563 6966 6965 6420 7261   to specified ra
-0004b690: 6e67 6520 696e 2078 2c20 792c 207a 2e0a  nge in x, y, z..
-0004b6a0: 0a20 2020 2020 2020 2054 6865 2070 6172  .        The par
-0004b6b0: 616d 6574 6572 7320 786c 696d 2c20 796c  ameters xlim, yl
-0004b6c0: 696d 2c20 7a6c 696d 2061 7265 2070 6173  im, zlim are pas
-0004b6d0: 7365 6420 746f 2065 6163 6820 524f 4927  sed to each ROI'
-0004b6e0: 7320 6372 6f70 2829 206d 6574 686f 642e  s crop() method.
-0004b6f0: 0a20 2020 2020 2020 2046 6f72 2065 7870  .        For exp
-0004b700: 6c61 6e61 7469 6f6e 206f 6620 7468 6573  lanation of thes
-0004b710: 6520 7061 7261 6d65 7465 7273 2c20 7365  e parameters, se
-0004b720: 6520 646f 6375 6d65 6e74 6174 696f 6e20  e documentation 
-0004b730: 666f 720a 2020 2020 2020 2020 736b 7274  for.        skrt
-0004b740: 2e73 7472 7563 7475 7265 732e 524f 492e  .structures.ROI.
-0004b750: 6372 6f70 2829 2e0a 2020 2020 2020 2020  crop()..        
-0004b760: 2222 220a 2020 2020 2020 2020 666f 7220  """.        for 
-0004b770: 726f 6920 696e 2073 656c 662e 6765 745f  roi in self.get_
-0004b780: 726f 6973 2829 3a0a 2020 2020 2020 2020  rois():.        
-0004b790: 2020 2020 726f 692e 6372 6f70 2878 6c69      roi.crop(xli
-0004b7a0: 6d2c 2079 6c69 6d2c 207a 6c69 6d29 0a0a  m, ylim, zlim)..
-0004b7b0: 636c 6173 7320 5374 7275 6374 7572 6553  class StructureS
-0004b7c0: 6574 4974 6572 6174 6f72 3a0a 0a20 2020  etIterator:..   
-0004b7d0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-0004b7e0: 6c66 2c20 7374 7275 6374 7572 655f 7365  lf, structure_se
-0004b7f0: 7429 3a0a 2020 2020 2020 2020 7365 6c66  t):.        self
-0004b800: 2e69 6478 203d 202d 310a 2020 2020 2020  .idx = -1.      
-0004b810: 2020 7365 6c66 2e73 7472 7563 7475 7265    self.structure
-0004b820: 5f73 6574 203d 2073 7472 7563 7475 7265  _set = structure
-0004b830: 5f73 6574 0a0a 2020 2020 6465 6620 5f5f  _set..    def __
-0004b840: 6e65 7874 5f5f 2873 656c 6629 3a0a 2020  next__(self):.  
-0004b850: 2020 2020 2020 7365 6c66 2e69 6478 202b        self.idx +
-0004b860: 3d20 310a 2020 2020 2020 2020 6966 2073  = 1.        if s
-0004b870: 656c 662e 6964 7820 3c20 6c65 6e28 7365  elf.idx < len(se
-0004b880: 6c66 2e73 7472 7563 7475 7265 5f73 6574  lf.structure_set
-0004b890: 2e67 6574 5f72 6f69 7328 2929 3a0a 2020  .get_rois()):.  
-0004b8a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0004b8b0: 2073 656c 662e 7374 7275 6374 7572 655f   self.structure_
-0004b8c0: 7365 742e 6765 745f 726f 6973 2829 5b73  set.get_rois()[s
-0004b8d0: 656c 662e 6964 785d 0a20 2020 2020 2020  elf.idx].       
-0004b8e0: 2072 6169 7365 2053 746f 7049 7465 7261   raise StopItera
-0004b8f0: 7469 6f6e 0a0a 0a64 6566 206c 6f61 645f  tion...def load_
-0004b900: 726f 6973 5f64 6963 6f6d 2870 6174 682c  rois_dicom(path,
-0004b910: 206e 616d 6573 3d4e 6f6e 6529 3a0a 2020   names=None):.  
-0004b920: 2020 2222 224c 6f61 6420 524f 4928 7329    """Load ROI(s)
-0004b930: 2066 726f 6d20 6120 6469 636f 6d20 7374   from a dicom st
-0004b940: 7275 6374 7572 6520 7365 7420 6669 6c65  ructure set file
-0004b950: 2e20 3c6e 616d 653e 2063 616e 2062 6520  . <name> can be 
-0004b960: 6120 7369 6e67 6c65 0a20 2020 206e 616d  a single.    nam
-0004b970: 6520 6f72 206c 6973 7420 6f66 206e 616d  e or list of nam
-0004b980: 6573 206f 6620 524f 4973 2074 6f20 6c6f  es of ROIs to lo
-0004b990: 6164 2e22 2222 0a0a 2020 2020 2320 4c6f  ad."""..    # Lo
-0004b9a0: 6164 2064 6963 6f6d 206f 626a 6563 740a  ad dicom object.
-0004b9b0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0004b9c0: 2064 7320 3d20 7079 6469 636f 6d2e 6463   ds = pydicom.dc
-0004b9d0: 6d72 6561 6428 7061 7468 2c20 666f 7263  mread(path, forc
-0004b9e0: 653d 5472 7565 290a 2020 2020 6578 6365  e=True).    exce
-0004b9f0: 7074 2070 7964 6963 6f6d 2e65 7272 6f72  pt pydicom.error
-0004ba00: 732e 496e 7661 6c69 6444 6963 6f6d 4572  s.InvalidDicomEr
-0004ba10: 726f 723a 0a20 2020 2020 2020 2072 6574  ror:.        ret
-0004ba20: 7572 6e20 5b5d 2c20 4e6f 6e65 0a20 2020  urn [], None.   
-0004ba30: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
-0004ba40: 6473 2c20 2253 4f50 436c 6173 7355 4944  ds, "SOPClassUID
-0004ba50: 2229 3a0a 2020 2020 2020 2020 7265 7475  "):.        retu
-0004ba60: 726e 205b 5d2c 204e 6f6e 650a 2020 2020  rn [], None.    
-0004ba70: 6966 206e 6f74 2028 6473 2e53 4f50 436c  if not (ds.SOPCl
-0004ba80: 6173 7355 4944 203d 3d20 2231 2e32 2e38  assUID == "1.2.8
-0004ba90: 3430 2e31 3030 3038 2e35 2e31 2e34 2e31  40.10008.5.1.4.1
-0004baa0: 2e31 2e34 3831 2e33 2229 3a0a 2020 2020  .1.481.3"):.    
-0004bab0: 2020 2020 7072 696e 7428 6622 5761 726e      print(f"Warn
-0004bac0: 696e 673a 207b 7061 7468 7d20 6973 206e  ing: {path} is n
-0004bad0: 6f74 2061 2044 4943 4f4d 2073 7472 7563  ot a DICOM struc
-0004bae0: 7475 7265 2073 6574 2066 696c 6521 2229  ture set file!")
-0004baf0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0004bb00: 5b5d 2c20 4e6f 6e65 0a0a 2020 2020 2320  [], None..    # 
-0004bb10: 4765 7420 524f 4920 6e61 6d65 730a 2020  Get ROI names.  
-0004bb20: 2020 7365 7120 3d20 6765 745f 6469 636f    seq = get_dico
-0004bb30: 6d5f 7365 7175 656e 6365 2864 732c 2022  m_sequence(ds, "
-0004bb40: 5374 7275 6374 7572 6553 6574 524f 4922  StructureSetROI"
-0004bb50: 290a 2020 2020 726f 6973 203d 207b 7d0a  ).    rois = {}.
-0004bb60: 2020 2020 666f 7220 726f 6920 696e 2073      for roi in s
-0004bb70: 6571 3a0a 2020 2020 2020 2020 726f 6973  eq:.        rois
-0004bb80: 5b69 6e74 2872 6f69 2e52 4f49 4e75 6d62  [int(roi.ROINumb
-0004bb90: 6572 295d 203d 207b 226e 616d 6522 3a20  er)] = {"name": 
-0004bba0: 726f 692e 524f 494e 616d 657d 0a0a 2020  roi.ROIName}..  
-0004bbb0: 2020 2320 4669 6e64 2052 4f49 7320 6d61    # Find ROIs ma
-0004bbc0: 7463 6869 6e67 2072 6571 7565 7374 6564  tching requested
-0004bbd0: 206e 616d 6573 0a20 2020 206e 616d 6573   names.    names
-0004bbe0: 5f74 6f5f 6c6f 6164 203d 204e 6f6e 650a  _to_load = None.
-0004bbf0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0004bc00: 6528 6e61 6d65 732c 2073 7472 293a 0a20  e(names, str):. 
-0004bc10: 2020 2020 2020 206e 616d 6573 5f74 6f5f         names_to_
-0004bc20: 6c6f 6164 203d 205b 6e61 6d65 735d 0a20  load = [names]. 
-0004bc30: 2020 2065 6c69 6620 736b 7274 2e63 6f72     elif skrt.cor
-0004bc40: 652e 6973 5f6c 6973 7428 6e61 6d65 7329  e.is_list(names)
-0004bc50: 3a0a 2020 2020 2020 2020 6e61 6d65 735f  :.        names_
-0004bc60: 746f 5f6c 6f61 6420 3d20 6e61 6d65 730a  to_load = names.
-0004bc70: 2020 2020 6966 206e 616d 6573 5f74 6f5f      if names_to_
-0004bc80: 6c6f 6164 3a0a 2020 2020 2020 2020 726f  load:.        ro
-0004bc90: 6973 203d 207b 0a20 2020 2020 2020 2020  is = {.         
-0004bca0: 2020 2069 3a20 730a 2020 2020 2020 2020     i: s.        
-0004bcb0: 2020 2020 666f 7220 692c 2073 2069 6e20      for i, s in 
-0004bcc0: 726f 6973 2e69 7465 6d73 2829 0a20 2020  rois.items().   
-0004bcd0: 2020 2020 2020 2020 2069 6620 616e 7928           if any(
-0004bce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0004bcf0: 205b 666e 6d61 7463 682e 666e 6d61 7463   [fnmatch.fnmatc
-0004bd00: 6828 735b 226e 616d 6522 5d2e 6c6f 7765  h(s["name"].lowe
-0004bd10: 7228 292c 206e 2e6c 6f77 6572 2829 2920  r(), n.lower()) 
-0004bd20: 666f 7220 6e20 696e 206e 616d 6573 5f74  for n in names_t
-0004bd30: 6f5f 6c6f 6164 5d0a 2020 2020 2020 2020  o_load].        
-0004bd40: 2020 2020 290a 2020 2020 2020 2020 7d0a      ).        }.
-0004bd50: 2020 2020 2020 2020 6966 206e 6f74 206c          if not l
-0004bd60: 656e 2872 6f69 7329 3a0a 2020 2020 2020  en(rois):.      
-0004bd70: 2020 2020 2020 7072 696e 7428 6622 5761        print(f"Wa
-0004bd80: 726e 696e 673a 206e 6f20 524f 4973 2066  rning: no ROIs f
-0004bd90: 6f75 6e64 206d 6174 6368 696e 6720 6e61  ound matching na
-0004bda0: 6d65 2873 293a 207b 6e61 6d65 737d 2229  me(s): {names}")
-0004bdb0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0004bdc0: 7572 6e20 5b5d 2c20 4e6f 6e65 0a0a 2020  urn [], None..  
-0004bdd0: 2020 2320 4765 7420 524f 4920 6465 7461    # Get ROI deta
-0004bde0: 696c 730a 2020 2020 726f 695f 7365 7120  ils.    roi_seq 
-0004bdf0: 3d20 6765 745f 6469 636f 6d5f 7365 7175  = get_dicom_sequ
-0004be00: 656e 6365 2864 732c 2022 524f 4943 6f6e  ence(ds, "ROICon
-0004be10: 746f 7572 2229 0a20 2020 2066 6f72 2072  tour").    for r
-0004be20: 6f69 2069 6e20 726f 695f 7365 713a 0a0a  oi in roi_seq:..
-0004be30: 2020 2020 2020 2020 6e75 6d62 6572 203d          number =
-0004be40: 2072 6f69 2e52 6566 6572 656e 6365 6452   roi.ReferencedR
-0004be50: 4f49 4e75 6d62 6572 0a20 2020 2020 2020  OINumber.       
-0004be60: 2069 6620 6e75 6d62 6572 206e 6f74 2069   if number not i
-0004be70: 6e20 726f 6973 3a0a 2020 2020 2020 2020  n rois:.        
-0004be80: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-0004be90: 2020 2020 2064 6174 6120 3d20 7b22 636f       data = {"co
-0004bea0: 6e74 6f75 7273 223a 207b 7d7d 0a0a 2020  ntours": {}}..  
-0004beb0: 2020 2020 2020 2320 4765 7420 524f 4920        # Get ROI 
-0004bec0: 636f 6c6f 7572 0a20 2020 2020 2020 2069  colour.        i
-0004bed0: 6620 2252 4f49 4469 7370 6c61 7943 6f6c  f "ROIDisplayCol
-0004bee0: 6f72 2220 696e 2072 6f69 3a0a 2020 2020  or" in roi:.    
-0004bef0: 2020 2020 2020 2020 6461 7461 5b22 636f          data["co
-0004bf00: 6c6f 7222 5d20 3d20 5b69 6e74 2863 2920  lor"] = [int(c) 
-0004bf10: 2f20 3235 3520 666f 7220 6320 696e 206c  / 255 for c in l
-0004bf20: 6973 7428 726f 692e 524f 4944 6973 706c  ist(roi.ROIDispl
-0004bf30: 6179 436f 6c6f 7229 5d0a 2020 2020 2020  ayColor)].      
-0004bf40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0004bf50: 2020 2020 6461 7461 5b22 636f 6c6f 7222      data["color"
-0004bf60: 5d20 3d20 4e6f 6e65 0a0a 2020 2020 2020  ] = None..      
-0004bf70: 2020 2320 4765 7420 636f 6e74 6f75 7273    # Get contours
-0004bf80: 0a20 2020 2020 2020 2063 6f6e 746f 7572  .        contour
-0004bf90: 5f73 6571 203d 2067 6574 5f64 6963 6f6d  _seq = get_dicom
-0004bfa0: 5f73 6571 7565 6e63 6528 726f 692c 2022  _sequence(roi, "
-0004bfb0: 436f 6e74 6f75 7222 290a 2020 2020 2020  Contour").      
-0004bfc0: 2020 6966 2063 6f6e 746f 7572 5f73 6571    if contour_seq
-0004bfd0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0004bfe0: 7220 6320 696e 2063 6f6e 746f 7572 5f73  r c in contour_s
-0004bff0: 6571 3a0a 2020 2020 2020 2020 2020 2020  eq:.            
-0004c000: 2020 2020 706c 616e 655f 6461 7461 203d      plane_data =
-0004c010: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-0004c020: 2020 2020 2020 205b 666c 6f61 7428 7029         [float(p)
-0004c030: 2066 6f72 2070 2069 6e20 632e 436f 6e74   for p in c.Cont
-0004c040: 6f75 7244 6174 615b 6920 2a20 3320 3a20  ourData[i * 3 : 
-0004c050: 6920 2a20 3320 2b20 335d 5d0a 2020 2020  i * 3 + 3]].    
-0004c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004c070: 666f 7220 6920 696e 2072 616e 6765 2863  for i in range(c
-0004c080: 2e4e 756d 6265 724f 6643 6f6e 746f 7572  .NumberOfContour
-0004c090: 506f 696e 7473 290a 2020 2020 2020 2020  Points).        
-0004c0a0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-0004c0b0: 2020 2020 2020 2020 2020 7a20 3d20 666c            z = fl
-0004c0c0: 6f61 7428 632e 436f 6e74 6f75 7244 6174  oat(c.ContourDat
-0004c0d0: 615b 325d 290a 2020 2020 2020 2020 2020  a[2]).          
-0004c0e0: 2020 2020 2020 6966 207a 206e 6f74 2069        if z not i
-0004c0f0: 6e20 6461 7461 5b22 636f 6e74 6f75 7273  n data["contours
-0004c100: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0004c110: 2020 2020 2020 2020 6461 7461 5b22 636f          data["co
-0004c120: 6e74 6f75 7273 225d 5b7a 5d20 3d20 5b5d  ntours"][z] = []
-0004c130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0004c140: 2064 6174 615b 2263 6f6e 746f 7572 7322   data["contours"
-0004c150: 5d5b 7a5d 2e61 7070 656e 6428 6e70 2e61  ][z].append(np.a
-0004c160: 7272 6179 2870 6c61 6e65 5f64 6174 6129  rray(plane_data)
-0004c170: 290a 0a20 2020 2020 2020 2072 6f69 735b  )..        rois[
-0004c180: 6e75 6d62 6572 5d2e 7570 6461 7465 2864  number].update(d
-0004c190: 6174 6129 0a0a 2020 2020 7265 7475 726e  ata)..    return
-0004c1a0: 2072 6f69 732c 2064 730a 0a0a 6465 6620   rois, ds...def 
-0004c1b0: 6765 745f 6469 636f 6d5f 7365 7175 656e  get_dicom_sequen
-0004c1c0: 6365 2864 733d 4e6f 6e65 2c20 6261 7365  ce(ds=None, base
-0004c1d0: 6e61 6d65 3d22 2229 3a0a 0a20 2020 2073  name=""):..    s
-0004c1e0: 6571 7565 6e63 6520 3d20 5b5d 0a20 2020  equence = [].   
-0004c1f0: 2066 6f72 2073 7566 6669 7820 696e 205b   for suffix in [
-0004c200: 2253 6571 7565 6e63 6522 2c20 2273 225d  "Sequence", "s"]
-0004c210: 3a0a 2020 2020 2020 2020 6174 7472 6962  :.        attrib
-0004c220: 7574 6520 3d20 6622 7b62 6173 656e 616d  ute = f"{basenam
-0004c230: 657d 7b73 7566 6669 787d 220a 2020 2020  e}{suffix}".    
-0004c240: 2020 2020 6966 2068 6173 6174 7472 2864      if hasattr(d
-0004c250: 732c 2061 7474 7269 6275 7465 293a 0a20  s, attribute):. 
-0004c260: 2020 2020 2020 2020 2020 2073 6571 7565             seque
-0004c270: 6e63 6520 3d20 6765 7461 7474 7228 6473  nce = getattr(ds
-0004c280: 2c20 6174 7472 6962 7574 6529 0a20 2020  , attribute).   
-0004c290: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-0004c2a0: 2020 2072 6574 7572 6e20 7365 7175 656e     return sequen
-0004c2b0: 6365 0a0a 6465 6620 636f 6e74 6f75 725f  ce..def contour_
-0004c2c0: 746f 5f70 6f6c 7967 6f6e 2863 6f6e 746f  to_polygon(conto
-0004c2d0: 7572 293a 0a20 2020 2022 2222 436f 6e76  ur):.    """Conv
-0004c2e0: 6572 7420 6120 6c69 7374 206f 6620 636f  ert a list of co
-0004c2f0: 6e74 6f75 7220 706f 696e 7473 2074 6f20  ntour points to 
-0004c300: 6120 5368 6170 656c 7920 706f 6c79 676f  a Shapely polygo
-0004c310: 6e2c 2065 6e73 7572 696e 6720 7468 6174  n, ensuring that
-0004c320: 200a 2020 2020 7468 6520 706f 6c79 676f   .    the polygo
-0004c330: 6e20 6973 2076 616c 6964 2e22 2222 0a0a  n is valid."""..
-0004c340: 2020 2020 706f 6c79 676f 6e20 3d20 6765      polygon = ge
-0004c350: 6f6d 6574 7279 2e50 6f6c 7967 6f6e 2863  ometry.Polygon(c
-0004c360: 6f6e 746f 7572 290a 0a20 2020 2064 656c  ontour)..    del
-0004c370: 7461 203d 2030 2e30 3035 0a20 2020 2069  ta = 0.005.    i
-0004c380: 6620 6e6f 7420 706f 6c79 676f 6e2e 6973  f not polygon.is
-0004c390: 5f76 616c 6964 3a0a 2020 2020 2020 2020  _valid:.        
-0004c3a0: 746d 7020 3d20 6765 6f6d 6574 7279 2e50  tmp = geometry.P
-0004c3b0: 6f6c 7967 6f6e 2870 6f6c 7967 6f6e 290a  olygon(polygon).
-0004c3c0: 2020 2020 2020 2020 6275 6666 6572 203d          buffer =
-0004c3d0: 2030 2e0a 2020 2020 2020 2020 2320 5468   0..        # Th
-0004c3e0: 6520 6964 6561 2068 6572 6520 6973 2074  e idea here is t
-0004c3f0: 6f20 696e 6372 6561 7365 2074 6865 2062  o increase the b
-0004c400: 7566 6665 7220 6469 7374 616e 6365 2075  uffer distance u
-0004c410: 6e74 696c 0a20 2020 2020 2020 2023 2061  ntil.        # a
-0004c420: 2076 616c 6964 2070 6f6c 7967 6f6e 2069   valid polygon i
-0004c430: 7320 6f62 7461 696e 6564 2e20 2054 6869  s obtained.  Thi
-0004c440: 7320 6765 6e65 7261 6c6c 7920 7365 656d  s generally seem
-0004c450: 7320 746f 2077 6f72 6b2e 2e2e 0a20 2020  s to work....   
-0004c460: 2020 2020 2077 6869 6c65 2028 6973 696e       while (isin
-0004c470: 7374 616e 6365 2870 6f6c 7967 6f6e 2c20  stance(polygon, 
-0004c480: 6765 6f6d 6574 7279 2e4d 756c 7469 506f  geometry.MultiPo
-0004c490: 6c79 676f 6e29 0a20 2020 2020 2020 2020  lygon).         
-0004c4a0: 2020 2020 2020 206f 7220 6e6f 7420 706f         or not po
-0004c4b0: 6c79 676f 6e2e 6973 5f76 616c 6964 293a  lygon.is_valid):
-0004c4c0: 0a20 2020 2020 2020 2020 2020 2062 7566  .            buf
-0004c4d0: 6665 7220 2b3d 2064 656c 7461 0a20 2020  fer += delta.   
-0004c4e0: 2020 2020 2020 2020 2070 6f6c 7967 6f6e           polygon
-0004c4f0: 203d 2074 6d70 2e62 7566 6665 7228 6275   = tmp.buffer(bu
-0004c500: 6666 6572 290a 2020 2020 2020 2020 706f  ffer).        po
-0004c510: 696e 7473 203d 205b 5d0a 2020 2020 2020  ints = [].      
-0004c520: 2020 666f 7220 782c 2079 2069 6e20 706f    for x, y in po
-0004c530: 6c79 676f 6e2e 6578 7465 7269 6f72 2e63  lygon.exterior.c
-0004c540: 6f6f 7264 733a 0a20 2020 2020 2020 2020  oords:.         
-0004c550: 2020 2070 6f69 6e74 732e 6170 7065 6e64     points.append
-0004c560: 2828 782c 2079 2929 0a20 2020 2020 2020  ((x, y)).       
-0004c570: 2070 6f6c 7967 6f6e 203d 2067 656f 6d65   polygon = geome
-0004c580: 7472 792e 506f 6c79 676f 6e28 706f 696e  try.Polygon(poin
-0004c590: 7473 290a 0a20 2020 2072 6574 7572 6e20  ts)..    return 
-0004c5a0: 706f 6c79 676f 6e0a 0a64 6566 2070 6f6c  polygon..def pol
-0004c5b0: 7967 6f6e 5f74 6f5f 636f 6e74 6f75 7228  ygon_to_contour(
-0004c5c0: 706f 6c79 676f 6e29 3a0a 2020 2020 2727  polygon):.    ''
-0004c5d0: 270a 2020 2020 436f 6e76 6572 7420 6120  '.    Convert a 
-0004c5e0: 5368 6170 656c 7920 706f 6c79 676f 6e20  Shapely polygon 
-0004c5f0: 746f 2061 206c 6973 7420 6f66 2063 6f6e  to a list of con
-0004c600: 746f 7572 2070 6f69 6e74 732e 0a0a 2020  tour points...  
-0004c610: 2020 2a2a 5061 7261 6d65 7465 723a 2a2a    **Parameter:**
-0004c620: 0a0a 2020 2020 706f 6c79 676f 6e3a 2073  ..    polygon: s
-0004c630: 6861 7065 6c79 2e67 656f 6d65 7472 792e  hapely.geometry.
-0004c640: 706f 6c79 676f 6e0a 2020 2020 2020 2020  polygon.        
-0004c650: 5368 6170 656c 7920 706f 6c79 676f 6e2e  Shapely polygon.
-0004c660: 0a0a 2020 2020 7a5f 706f 6c79 676f 6e3a  ..    z_polygon:
-0004c670: 207a 2063 6f6f 7264 696e 6174 6520 6174   z coordinate at
-0004c680: 2077 6869 6368 2070 6f6c 7967 6f6e 2069   which polygon i
-0004c690: 7320 6465 6669 6e65 642e 0a20 2020 2027  s defined..    '
-0004c6a0: 2727 0a20 2020 2063 6f6e 746f 7572 5f70  ''.    contour_p
-0004c6b0: 6f69 6e74 7320 3d20 5b5d 0a20 2020 2066  oints = [].    f
-0004c6c0: 6f72 2078 2c20 7920 696e 206c 6973 7428  or x, y in list(
-0004c6d0: 706f 6c79 676f 6e2e 6578 7465 7269 6f72  polygon.exterior
-0004c6e0: 2e63 6f6f 7264 7329 3a0a 2020 2020 2020  .coords):.      
-0004c6f0: 2020 636f 6e74 6f75 725f 706f 696e 7473    contour_points
-0004c700: 2e61 7070 656e 6428 5b78 2c20 795d 290a  .append([x, y]).
-0004c710: 2020 2020 636f 6e74 6f75 7220 3d20 6e70      contour = np
-0004c720: 2e61 7272 6179 2863 6f6e 746f 7572 5f70  .array(contour_p
-0004c730: 6f69 6e74 7329 0a0a 2020 2020 7265 7475  oints)..    retu
-0004c740: 726e 2063 6f6e 746f 7572 0a0a 6465 6620  rn contour..def 
-0004c750: 696e 7465 7270 6f6c 6174 655f 706f 696e  interpolate_poin
-0004c760: 7473 5f73 696e 676c 655f 636f 6e74 6f75  ts_single_contou
-0004c770: 7228 736f 7572 6365 3d4e 6f6e 652c 206e  r(source=None, n
-0004c780: 5f70 6f69 6e74 3d4e 6f6e 652c 2064 7879  _point=None, dxy
-0004c790: 3d4e 6f6e 652c 0a20 2020 2020 2020 2073  =None,.        s
-0004c7a0: 6d6f 6f74 686e 6573 735f 7065 725f 706f  moothness_per_po
-0004c7b0: 696e 743d 3029 3a0a 2020 2020 2727 270a  int=0):.    '''.
-0004c7c0: 2020 2020 496e 7465 7270 6f6c 6174 6520      Interpolate 
-0004c7d0: 706f 696e 7473 2066 6f72 2061 2073 696e  points for a sin
-0004c7e0: 676c 6520 636f 6e74 6f75 722e 0a0a 2020  gle contour...  
-0004c7f0: 2020 2a2a 5061 7261 6d65 7465 7273 3a2a    **Parameters:*
-0004c800: 2a0a 0a20 2020 2073 6f75 7263 6520 3a20  *..    source : 
-0004c810: 7368 6170 656c 792e 706f 6c79 676f 6e2e  shapely.polygon.
-0004c820: 506f 6c79 676f 6e2f 6e70 2e6e 6461 7272  Polygon/np.ndarr
-0004c830: 6179 2f6c 6973 742c 2064 6566 6175 6c74  ay/list, default
-0004c840: 3d4e 6f6e 650a 2020 2020 2020 2020 436f  =None.        Co
-0004c850: 6e74 6f75 7220 7265 7072 6573 656e 7461  ntour representa
-0004c860: 7469 6f6e 2061 7320 6569 7468 6572 2061  tion as either a
-0004c870: 2073 6861 7065 6c79 2050 6f6c 7967 6f6e   shapely Polygon
-0004c880: 2c20 6120 6e75 6d70 790a 2020 2020 2020  , a numpy.      
-0004c890: 2020 6172 7261 7920 6f66 205b 782c 2079    array of [x, y
-0004c8a0: 5d20 7061 6972 7320 6f72 2061 206c 6973  ] pairs or a lis
-0004c8b0: 7420 6f66 205b 782c 2079 5d20 7061 6972  t of [x, y] pair
-0004c8c0: 732e 2020 5468 650a 2020 2020 2020 2020  s.  The.        
-0004c8d0: 7265 7475 726e 6564 2063 6f6e 746f 7572  returned contour
-0004c8e0: 2068 6173 2074 6865 2073 616d 6520 7265   has the same re
-0004c8f0: 7072 6573 656e 7461 7469 6f6e 2e0a 0a20  presentation... 
-0004c900: 2020 206e 5f70 6f69 6e74 203a 2069 6e74     n_point : int
-0004c910: 2c20 6465 6661 756c 743d 4e6f 6e65 0a20  , default=None. 
-0004c920: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
-0004c930: 2070 6f69 6e74 7320 746f 2064 6566 696e   points to defin
-0004c940: 6520 636f 6e74 6f75 722c 2061 6674 6572  e contour, after
-0004c950: 2069 6e74 6572 706f 6c61 7469 6f6e 2e20   interpolation. 
-0004c960: 2054 6869 7320 6d75 7374 0a20 2020 2020   This must.     
-0004c970: 2020 2062 6520 7365 7420 746f 204e 6f6e     be set to Non
-0004c980: 6520 666f 7220 6478 7920 746f 2062 6520  e for dxy to be 
-0004c990: 636f 6e73 6964 6572 6564 2e0a 0a20 2020  considered...   
-0004c9a0: 2064 7879 203a 2066 6c6f 6174 2c20 6465   dxy : float, de
-0004c9b0: 6661 756c 743d 4e6f 6e65 0a20 2020 2020  fault=None.     
-0004c9c0: 2020 2041 7070 726f 7869 6d61 7465 2064     Approximate d
-0004c9d0: 6973 7461 6e63 6520 7265 7175 6972 6564  istance required
-0004c9e0: 2062 6574 7765 656e 2063 6f6e 746f 7572   between contour
-0004c9f0: 2070 6f69 6e74 732e 2020 5468 6973 2069   points.  This i
-0004ca00: 7320 7461 6b65 6e0a 2020 2020 2020 2020  s taken.        
-0004ca10: 696e 746f 2061 6363 6f75 6e74 206f 6e6c  into account onl
-0004ca20: 7920 6966 206e 5f70 6f69 6e74 2069 7320  y if n_point is 
-0004ca30: 7365 7420 746f 204e 6f6e 652e 2020 466f  set to None.  Fo
-0004ca40: 7220 6120 636f 6e74 6f75 7220 6f66 0a20  r a contour of. 
-0004ca50: 2020 2020 2020 206c 656e 6774 6820 636f         length co
-0004ca60: 6e74 6f75 725f 6c65 6e67 7468 2c20 7468  ntour_length, th
-0004ca70: 6520 6e75 6d62 6572 206f 6620 636f 6e74  e number of cont
-0004ca80: 6f75 7220 706f 696e 7473 2069 7320 7468  our points is th
-0004ca90: 656e 2074 616b 656e 0a20 2020 2020 2020  en taken.       
-0004caa0: 2074 6f20 6265 206d 6178 2869 6e74 2863   to be max(int(c
-0004cab0: 6f6e 746f 7572 5f6c 656e 6774 6820 2f20  ontour_length / 
-0004cac0: 6478 7929 2c20 3329 2e20 200a 0a20 2020  dxy), 3).  ..   
-0004cad0: 2073 6d6f 6f74 686e 6573 735f 7065 725f   smoothness_per_
-0004cae0: 706f 696e 7420 3a20 666c 6f61 742c 2064  point : float, d
-0004caf0: 6566 6175 6c74 3d30 0a20 2020 2020 2020  efault=0.       
-0004cb00: 2050 6172 616d 6574 6572 2064 6574 6572   Parameter deter
-0004cb10: 6d69 6e69 6e67 2074 6865 2073 6d6f 6f74  mining the smoot
-0004cb20: 686e 6573 7320 6f66 2074 6865 2042 2d73  hness of the B-s
-0004cb30: 706c 696e 6520 6375 7276 6520 7573 6564  pline curve used
-0004cb40: 0a20 2020 2020 2020 2069 6e20 636f 6e74  .        in cont
-0004cb50: 6f75 7220 6170 7072 6f78 696d 6174 696f  our approximatio
-0004cb60: 6e20 666f 7220 696e 7465 7270 6f6c 6174  n for interpolat
-0004cb70: 696f 6e2e 2020 5468 6520 7072 6f64 7563  ion.  The produc
-0004cb80: 7420 6f66 0a20 2020 2020 2020 2073 6d6f  t of.        smo
-0004cb90: 6f74 686e 6573 735f 7065 725f 706f 696e  othness_per_poin
-0004cba0: 7420 616e 6420 7468 6520 6e75 6d62 6572  t and the number
-0004cbb0: 206f 6620 636f 6e74 6f75 7220 706f 696e   of contour poin
-0004cbc0: 7473 2028 7370 6563 6966 6965 640a 2020  ts (specified.  
-0004cbd0: 2020 2020 2020 6469 7265 6374 6c79 2076        directly v
-0004cbe0: 6961 206e 5f70 6f69 6e74 2c20 6f72 2069  ia n_point, or i
-0004cbf0: 6e64 6972 6563 746c 7920 7669 6120 6478  ndirectly via dx
-0004cc00: 7929 2063 6f72 7265 7370 6f6e 6473 2074  y) corresponds t
-0004cc10: 6f20 7468 650a 2020 2020 2020 2020 7061  o the.        pa
-0004cc20: 7261 6d65 7465 7220 7320 6f66 2073 6369  rameter s of sci
-0004cc30: 7079 2e69 6e74 6572 706f 6c61 7465 2e73  py.interpolate.s
-0004cc40: 706c 7072 6570 202d 2073 6565 2064 6f63  plprep - see doc
-0004cc50: 756d 656e 7461 7469 6f6e 2061 743a 0a20  umentation at:. 
-0004cc60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-0004cc70: 6874 7470 733a 2f2f 7363 6970 792e 6769  https://scipy.gi
-0004cc80: 7468 7562 2e69 6f2f 6465 7664 6f63 732f  thub.io/devdocs/
-0004cc90: 7265 6665 7265 6e63 652f 6765 6e65 7261  reference/genera
-0004cca0: 7465 642f 7363 6970 792e 696e 7465 7270  ted/scipy.interp
-0004ccb0: 6f6c 6174 652e 7370 6c70 7265 702e 6874  olate.splprep.ht
-0004ccc0: 6d6c 2373 6369 7079 2e69 6e74 6572 706f  ml#scipy.interpo
-0004ccd0: 6c61 7465 2e73 706c 7072 6570 0a0a 2020  late.splprep..  
-0004cce0: 2020 2020 2020 4120 736d 6f6f 7468 6e65        A smoothne
-0004ccf0: 7373 5f70 6572 5f70 6f69 6e74 206f 6620  ss_per_point of 
-0004cd00: 3020 666f 7263 6573 2074 6865 2042 2d73  0 forces the B-s
-0004cd10: 706c 696e 6520 746f 2070 6173 7320 7468  pline to pass th
-0004cd20: 726f 7567 680a 2020 2020 2020 2020 616c  rough.        al
-0004cd30: 6c20 6f66 2074 6865 2070 7265 2d69 6e74  l of the pre-int
-0004cd40: 6572 706f 6c61 7469 6f6e 2063 6f6e 746f  erpolation conto
-0004cd50: 7572 2070 6f69 6e74 732e 0a20 2020 2027  ur points..    '
-0004cd60: 2727 0a0a 2020 2020 2320 4578 7472 6163  ''..    # Extrac
-0004cd70: 7420 6c69 7374 206f 6620 636f 6e74 6f75  t list of contou
-0004cd80: 7220 706f 696e 7473 2066 726f 6d20 736f  r points from so
-0004cd90: 7572 6365 2e0a 2020 2020 636f 6e74 6f75  urce..    contou
-0004cda0: 725f 6c65 6e67 7468 203d 204e 6f6e 650a  r_length = None.
-0004cdb0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0004cdc0: 6528 736f 7572 6365 2c20 6765 6f6d 6574  e(source, geomet
-0004cdd0: 7279 2e70 6f6c 7967 6f6e 2e50 6f6c 7967  ry.polygon.Polyg
-0004cde0: 6f6e 293a 0a20 2020 2020 2020 2070 6f69  on):.        poi
-0004cdf0: 6e74 7320 3d20 6c69 7374 2870 6f6c 7967  nts = list(polyg
-0004ce00: 6f6e 5f74 6f5f 636f 6e74 6f75 7228 736f  on_to_contour(so
-0004ce10: 7572 6365 2929 0a20 2020 2020 2020 2063  urce)).        c
-0004ce20: 6f6e 746f 7572 5f6c 656e 6774 6820 3d20  ontour_length = 
-0004ce30: 736f 7572 6365 2e6c 656e 6774 680a 2020  source.length.  
-0004ce40: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-0004ce50: 6528 736f 7572 6365 2c20 6e70 2e6e 6461  e(source, np.nda
-0004ce60: 7272 6179 2920 6f72 2069 7369 6e73 7461  rray) or isinsta
-0004ce70: 6e63 6528 736f 7572 6365 2c20 6c69 7374  nce(source, list
-0004ce80: 293a 0a20 2020 2020 2020 2070 6f69 6e74  ):.        point
-0004ce90: 7320 3d20 6c69 7374 2873 6f75 7263 6529  s = list(source)
-0004cea0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0004ceb0: 2020 2070 6f69 6e74 7320 3d20 4e6f 6e65     points = None
-0004cec0: 0a0a 2020 2020 6966 2070 6f69 6e74 7320  ..    if points 
-0004ced0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0004cee0: 2070 7269 6e74 2827 556e 7265 636f 676e   print('Unrecogn
-0004cef0: 6973 6564 2073 6f75 7263 6520 7061 7373  ised source pass
-0004cf00: 6564 2074 6f20 270a 2020 2020 2020 2020  ed to '.        
-0004cf10: 2020 2020 2020 2020 275c 2769 6e74 6572          '\'inter
-0004cf20: 706f 6c61 7465 5f70 6f69 6e74 735f 7369  polate_points_si
-0004cf30: 6e67 6c65 5f63 6f6e 746f 7572 2829 5c27  ngle_contour()\'
-0004cf40: 2729 0a20 2020 2020 2020 2070 7269 6e74  ').        print
-0004cf50: 2827 536f 7572 6365 206d 7573 7420 6265  ('Source must be
-0004cf60: 2073 6861 7065 6c79 2050 6f6c 7967 6f6e   shapely Polygon
-0004cf70: 206f 7220 636f 6e74 6f75 7227 290a 2020   or contour').  
-0004cf80: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-0004cf90: 650a 0a20 2020 2023 2049 6620 6e75 6d62  e..    # If numb
-0004cfa0: 6572 206f 6620 636f 6e74 6f75 7220 706f  er of contour po
-0004cfb0: 696e 7473 206e 6f74 2070 6173 7365 6420  ints not passed 
-0004cfc0: 6469 7265 6374 6c79 2c0a 2020 2020 2320  directly,.    # 
-0004cfd0: 7472 7920 746f 2064 6574 6572 6d69 6e65  try to determine
-0004cfe0: 2069 7473 2076 616c 7565 2066 726f 6d20   its value from 
-0004cff0: 7468 6520 6469 7374 616e 6365 2062 6574  the distance bet
-0004d000: 7765 656e 2063 6f6e 746f 7572 2070 6f69  ween contour poi
-0004d010: 6e74 732e 0a20 2020 2069 6620 6e5f 706f  nts..    if n_po
-0004d020: 696e 7420 6973 204e 6f6e 6520 616e 6420  int is None and 
-0004d030: 6478 793a 0a20 2020 2020 2020 2069 6620  dxy:.        if 
-0004d040: 636f 6e74 6f75 725f 6c65 6e67 7468 2069  contour_length i
-0004d050: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0004d060: 2020 2020 636f 6e74 6f75 725f 6c65 6e67      contour_leng
-0004d070: 7468 203d 2063 6f6e 746f 7572 5f74 6f5f  th = contour_to_
-0004d080: 706f 6c79 676f 6e28 736f 7572 6365 292e  polygon(source).
-0004d090: 6c65 6e67 7468 0a20 2020 2020 2020 206e  length.        n
-0004d0a0: 5f70 6f69 6e74 203d 206d 6178 2869 6e74  _point = max(int
-0004d0b0: 2863 6f6e 746f 7572 5f6c 656e 6774 6820  (contour_length 
-0004d0c0: 2f20 6478 7929 2c20 3329 0a20 2020 2069  / dxy), 3).    i
-0004d0d0: 6620 6e5f 706f 696e 7420 6973 204e 6f6e  f n_point is Non
-0004d0e0: 653a 0a20 2020 2020 2020 2070 7269 6e74  e:.        print
-0004d0f0: 2827 4e6f 2069 6e74 6572 706f 6c61 7469  ('No interpolati
-0004d100: 6f6e 2070 6572 666f 726d 6564 2729 0a20  on performed'). 
-0004d110: 2020 2020 2020 2070 7269 6e74 2827 4e75         print('Nu
-0004d120: 6d62 6572 206f 6620 636f 6e74 6f75 7220  mber of contour 
-0004d130: 706f 696e 7473 2028 6e5f 706f 696e 7429  points (n_point)
-0004d140: 206f 7220 6469 7374 616e 6365 2062 6574   or distance bet
-0004d150: 7765 656e 2070 6f69 6e74 7327 0a20 2020  ween points'.   
-0004d160: 2020 2020 2020 2020 2020 2020 2027 6d75               'mu
-0004d170: 7374 2062 6520 7370 6563 6966 6965 642e  st be specified.
-0004d180: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0004d190: 6e20 4e6f 6e65 0a0a 2020 2020 2320 4d61  n None..    # Ma
-0004d1a0: 6b65 206c 6173 7420 706f 696e 7420 7468  ke last point th
-0004d1b0: 6520 7361 6d65 2061 7320 7468 6520 6669  e same as the fi
-0004d1c0: 7273 742c 2074 6f20 656e 7375 7265 2063  rst, to ensure c
-0004d1d0: 6c6f 7365 6420 6375 7276 652e 0a20 2020  losed curve..   
-0004d1e0: 2070 6f69 6e74 732e 6170 7065 6e64 2870   points.append(p
-0004d1f0: 6f69 6e74 735b 305d 290a 0a20 2020 2023  oints[0])..    #
-0004d200: 2044 6973 6361 7264 2070 6f69 6e74 7320   Discard points 
-0004d210: 7468 6174 2061 7265 6e27 7420 7365 7061  that aren't sepa
-0004d220: 7261 7465 6420 6672 6f6d 2074 6865 2070  rated from the p
-0004d230: 7265 6365 6564 696e 6720 706f 696e 740a  receeding point.
-0004d240: 2020 2020 2320 6279 2061 7420 6c65 6173      # by at leas
-0004d250: 7420 736f 6d65 206d 696e 696d 756d 2064  t some minimum d
-0004d260: 6973 7461 6e63 652e 0a20 2020 2064 7879  istance..    dxy
-0004d270: 5f6d 696e 203d 2030 2e30 3031 0a20 2020  _min = 0.001.   
-0004d280: 2078 5f6c 6173 742c 2079 5f6c 6173 7420   x_last, y_last 
-0004d290: 3d20 706f 696e 7473 5b30 5d0a 2020 2020  = points[0].    
-0004d2a0: 785f 7661 6c75 6573 2c20 795f 7661 6c75  x_values, y_valu
-0004d2b0: 6573 203d 2028 5b78 5f6c 6173 745d 2c20  es = ([x_last], 
-0004d2c0: 5b79 5f6c 6173 745d 290a 2020 2020 666f  [y_last]).    fo
-0004d2d0: 7220 6920 696e 2072 616e 6765 2831 2c20  r i in range(1, 
-0004d2e0: 6c65 6e28 706f 696e 7473 2929 3a0a 2020  len(points)):.  
-0004d2f0: 2020 2020 2020 782c 2079 203d 2070 6f69        x, y = poi
-0004d300: 6e74 735b 695d 0a20 2020 2020 2020 2069  nts[i].        i
-0004d310: 6620 2861 6273 2878 202d 2078 5f6c 6173  f (abs(x - x_las
-0004d320: 7429 203e 2064 7879 5f6d 696e 2920 6f72  t) > dxy_min) or
-0004d330: 2028 6162 7328 7920 2d20 795f 6c61 7374   (abs(y - y_last
-0004d340: 2920 3e20 6478 795f 6d69 6e29 3a0a 2020  ) > dxy_min):.  
-0004d350: 2020 2020 2020 2020 2020 785f 7661 6c75            x_valu
-0004d360: 6573 2e61 7070 656e 6428 706f 696e 7473  es.append(points
-0004d370: 5b69 5d5b 305d 290a 2020 2020 2020 2020  [i][0]).        
-0004d380: 2020 2020 795f 7661 6c75 6573 2e61 7070      y_values.app
-0004d390: 656e 6428 706f 696e 7473 5b69 5d5b 315d  end(points[i][1]
-0004d3a0: 290a 2020 2020 2020 2020 785f 6c61 7374  ).        x_last
-0004d3b0: 2c20 795f 6c61 7374 203d 2070 6f69 6e74  , y_last = point
-0004d3c0: 735b 695d 0a0a 2020 2020 785f 7661 6c75  s[i]..    x_valu
-0004d3d0: 6573 203d 206e 702e 6172 7261 7928 785f  es = np.array(x_
-0004d3e0: 7661 6c75 6573 290a 2020 2020 795f 7661  values).    y_va
-0004d3f0: 6c75 6573 203d 206e 702e 6172 7261 7928  lues = np.array(
-0004d400: 795f 7661 6c75 6573 290a 0a20 2020 2023  y_values)..    #
-0004d410: 2049 6e74 6572 706f 6c61 7465 2063 6f6e   Interpolate con
-0004d420: 746f 7572 2070 6f69 6e74 732e 0a20 2020  tour points..   
-0004d430: 2073 6d6f 6f74 686e 6573 7320 3d20 736d   smoothness = sm
-0004d440: 6f6f 7468 6e65 7373 5f70 6572 5f70 6f69  oothness_per_poi
-0004d450: 6e74 202a 206c 656e 2878 5f76 616c 7565  nt * len(x_value
-0004d460: 7329 0a20 2020 2074 7279 3a0a 2320 2020  s).    try:.#   
-0004d470: 2020 2020 2077 6974 6820 7761 726e 696e       with warnin
-0004d480: 6773 2e63 6174 6368 5f77 6172 6e69 6e67  gs.catch_warning
-0004d490: 7328 293a 0a23 2020 2020 2020 2020 2020  s():.#          
-0004d4a0: 2020 7761 726e 696e 6773 2e66 696c 7465    warnings.filte
-0004d4b0: 7277 6172 6e69 6e67 7328 2269 676e 6f72  rwarnings("ignor
-0004d4c0: 6522 2c20 6d65 7373 6167 653d 2253 6574  e", message="Set
-0004d4d0: 7469 6e67 2078 2229 0a20 2020 2020 2020  ting x").       
-0004d4e0: 2020 2020 2074 636b 2c20 7520 3d20 696e       tck, u = in
-0004d4f0: 7465 7270 6f6c 6174 652e 7370 6c70 7265  terpolate.splpre
-0004d500: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-0004d510: 2020 2020 2020 205b 785f 7661 6c75 6573         [x_values
-0004d520: 2c20 795f 7661 6c75 6573 5d2c 2073 3d73  , y_values], s=s
-0004d530: 6d6f 6f74 686e 6573 732c 2070 6572 3d54  moothness, per=T
-0004d540: 7275 6529 0a20 2020 2065 7863 6570 7420  rue).    except 
-0004d550: 5479 7065 4572 726f 7220 6173 2070 726f  TypeError as pro
-0004d560: 626c 656d 3a0a 2020 2020 2020 2020 7072  blem:.        pr
-0004d570: 696e 7428 2257 4152 4e49 4e47 3a20 5072  int("WARNING: Pr
-0004d580: 6f62 6c65 6d20 696e 2069 6e74 6572 706f  oblem in interpo
-0004d590: 6c61 7465 5f63 6f6e 746f 7572 5f70 6f69  late_contour_poi
-0004d5a0: 6e74 7328 293a 222c 2070 726f 626c 656d  nts():", problem
-0004d5b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0004d5c0: 204e 6f6e 650a 0a20 2020 2078 695f 7661   None..    xi_va
-0004d5d0: 6c75 6573 2c20 7969 5f76 616c 7565 7320  lues, yi_values 
-0004d5e0: 3d20 696e 7465 7270 6f6c 6174 652e 7370  = interpolate.sp
-0004d5f0: 6c65 7628 0a20 2020 2020 2020 206e 702e  lev(.        np.
-0004d600: 6c69 6e73 7061 6365 2830 2e2c 2031 2e2c  linspace(0., 1.,
-0004d610: 206e 5f70 6f69 6e74 202b 2031 292c 2074   n_point + 1), t
-0004d620: 636b 290a 0a20 2020 2023 2053 746f 7265  ck)..    # Store
-0004d630: 2070 6f69 6e74 7320 696e 2061 2066 6f72   points in a for
-0004d640: 6d20 7468 6174 206d 6179 2062 6520 636f  m that may be co
-0004d650: 6e76 6572 7465 6420 746f 2061 206e 756d  nverted to a num
-0004d660: 7079 2061 7272 6179 2e0a 2020 2020 706f  py array..    po
-0004d670: 696e 7473 5f69 6e74 6572 706f 6c61 7465  ints_interpolate
-0004d680: 6420 3d20 6c69 7374 287a 6970 2878 695f  d = list(zip(xi_
-0004d690: 7661 6c75 6573 2c20 7969 5f76 616c 7565  values, yi_value
-0004d6a0: 7329 290a 2020 2020 706f 696e 7473 5f69  s)).    points_i
-0004d6b0: 6e74 6572 706f 6c61 7465 6420 3d20 5b78  nterpolated = [x
-0004d6c0: 7920 666f 7220 7879 2069 6e20 706f 696e  y for xy in poin
-0004d6d0: 7473 5f69 6e74 6572 706f 6c61 7465 645d  ts_interpolated]
-0004d6e0: 0a0a 2020 2020 2320 5265 7475 726e 2069  ..    # Return i
-0004d6f0: 6e74 6572 706f 6c61 7465 6420 636f 6e74  nterpolated cont
-0004d700: 6f75 7220 696e 2074 6865 2073 616d 6520  our in the same 
-0004d710: 7265 7072 6573 656e 7461 7469 6f6e 2061  representation a
-0004d720: 7320 7468 6520 736f 7572 6365 2e0a 2020  s the source..  
-0004d730: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0004d740: 736f 7572 6365 2c20 6765 6f6d 6574 7279  source, geometry
-0004d750: 2e70 6f6c 7967 6f6e 2e50 6f6c 7967 6f6e  .polygon.Polygon
-0004d760: 293a 0a20 2020 2020 2020 206f 7574 5f6f  ):.        out_o
-0004d770: 626a 6563 7420 3d20 6765 6f6d 6574 7279  bject = geometry
-0004d780: 2e70 6f6c 7967 6f6e 2e50 6f6c 7967 6f6e  .polygon.Polygon
-0004d790: 2870 6f69 6e74 735f 696e 7465 7270 6f6c  (points_interpol
-0004d7a0: 6174 6564 290a 2020 2020 656c 6966 2069  ated).    elif i
-0004d7b0: 7369 6e73 7461 6e63 6528 736f 7572 6365  sinstance(source
-0004d7c0: 2c20 6e70 2e6e 6461 7272 6179 293a 0a20  , np.ndarray):. 
-0004d7d0: 2020 2020 2020 206f 7574 5f6f 626a 6563         out_objec
-0004d7e0: 7420 3d20 6e70 2e61 7272 6179 2870 6f69  t = np.array(poi
-0004d7f0: 6e74 735f 696e 7465 7270 6f6c 6174 6564  nts_interpolated
-0004d800: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-0004d810: 2020 2020 6f75 745f 6f62 6a65 6374 203d      out_object =
-0004d820: 2070 6f69 6e74 735f 696e 7465 7270 6f6c   points_interpol
-0004d830: 6174 6564 0a0a 2020 2020 7265 7475 726e  ated..    return
-0004d840: 206f 7574 5f6f 626a 6563 740a 0a64 6566   out_object..def
-0004d850: 2077 7269 7465 5f73 7472 7563 7475 7265   write_structure
-0004d860: 5f73 6574 5f64 6963 6f6d 280a 2020 2020  _set_dicom(.    
-0004d870: 6f75 746e 616d 652c 200a 2020 2020 726f  outname, .    ro
-0004d880: 6973 2c20 0a20 2020 2069 6d61 6765 3d4e  is, .    image=N
-0004d890: 6f6e 652c 200a 2020 2020 6166 6669 6e65  one, .    affine
-0004d8a0: 3d4e 6f6e 652c 200a 2020 2020 7368 6170  =None, .    shap
-0004d8b0: 653d 4e6f 6e65 2c0a 2020 2020 6f72 6965  e=None,.    orie
-0004d8c0: 6e74 6174 696f 6e3d 4e6f 6e65 2c20 0a20  ntation=None, . 
-0004d8d0: 2020 2068 6561 6465 725f 736f 7572 6365     header_source
-0004d8e0: 3d4e 6f6e 652c 200a 2020 2020 7061 7469  =None, .    pati
-0004d8f0: 656e 745f 6964 3d4e 6f6e 652c 0a20 2020  ent_id=None,.   
-0004d900: 206d 6f64 616c 6974 793d 4e6f 6e65 2c20   modality=None, 
-0004d910: 0a20 2020 2072 6f6f 745f 7569 643d 4e6f  .    root_uid=No
-0004d920: 6e65 0a29 3a0a 0a20 2020 2023 2043 6865  ne.):..    # Che
-0004d930: 636b 2077 6520 6861 7665 2074 6865 2072  ck we have the r
-0004d940: 656c 6576 616e 7420 696e 666f 0a20 2020  elevant info.   
-0004d950: 2069 6620 6e6f 7420 696d 6167 6520 616e   if not image an
-0004d960: 6420 286e 6f74 2061 6666 696e 6520 6f72  d (not affine or
-0004d970: 206e 6f74 2073 6861 7065 293a 0a20 2020   not shape):.   
-0004d980: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
-0004d990: 6d65 4572 726f 7228 224d 7573 7420 7072  meError("Must pr
-0004d9a0: 6f76 6964 6520 6569 7468 6572 2061 6e20  ovide either an 
-0004d9b0: 696d 6167 6520 6f72 2061 6e20 6166 6669  image or an affi
-0004d9c0: 6e65 206d 6174 7269 7820 220a 2020 2020  ne matrix ".    
-0004d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004d9e0: 2020 2020 2020 2022 616e 6420 7368 6170         "and shap
-0004d9f0: 6521 2229 0a0a 2020 2020 2320 5472 7920  e!")..    # Try 
-0004da00: 6765 7474 696e 6720 6469 636f 6d20 6461  getting dicom da
-0004da10: 7461 7365 7420 6672 6f6d 2069 6d61 6765  taset from image
-0004da20: 0a20 2020 2064 7320 3d20 4e6f 6e65 0a20  .    ds = None. 
-0004da30: 2020 2069 6620 696d 6167 653a 0a20 2020     if image:.   
-0004da40: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-0004da50: 696d 6167 652c 2022 6469 636f 6d5f 6461  image, "dicom_da
-0004da60: 7461 7365 7422 293a 0a20 2020 2020 2020  taset"):.       
-0004da70: 2020 2020 2064 7320 3d20 696d 6167 652e       ds = image.
-0004da80: 6469 636f 6d5f 6461 7461 7365 740a 2020  dicom_dataset.  
-0004da90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0004daa0: 2020 2020 2020 2020 6473 203d 2073 6b72          ds = skr
-0004dab0: 742e 696d 6167 652e 6372 6561 7465 5f64  t.image.create_d
-0004dac0: 6963 6f6d 2829 0a20 2020 2020 2020 2020  icom().         
-0004dad0: 2020 2064 732e 7365 745f 6765 6f6d 6574     ds.set_geomet
-0004dae0: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
-0004daf0: 2020 2020 696d 6167 652e 6765 745f 6166      image.get_af
-0004db00: 6669 6e65 2829 2c20 696d 6167 652e 6765  fine(), image.ge
-0004db10: 745f 6461 7461 2829 2e73 6861 7065 2c0a  t_data().shape,.
-0004db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004db30: 696d 6167 652e 6765 745f 6f72 6965 6e74  image.get_orient
-0004db40: 6174 696f 6e5f 7665 6374 6f72 2869 6d61  ation_vector(ima
-0004db50: 6765 2e67 6574 5f61 6666 696e 652c 2022  ge.get_affine, "
-0004db60: 6469 636f 6d22 290a 2020 2020 2020 2020  dicom").        
-0004db70: 2020 2020 290a 0a20 2020 2023 204f 7468      )..    # Oth
-0004db80: 6572 7769 7365 2c20 6372 6561 7465 2066  erwise, create f
-0004db90: 7265 7368 2064 6963 6f6d 2064 6174 6173  resh dicom datas
-0004dba0: 6574 0a20 2020 2065 6c73 653a 0a20 2020  et.    else:.   
-0004dbb0: 2020 2020 2064 7320 3d20 736b 7274 2e69       ds = skrt.i
-0004dbc0: 6d61 6765 2e63 7265 6174 655f 6469 636f  mage.create_dico
-0004dbd0: 6d28 7061 7469 656e 745f 6964 2c20 6d6f  m(patient_id, mo
-0004dbe0: 6461 6c69 7479 2c20 726f 6f74 5f75 6964  dality, root_uid
-0004dbf0: 290a 2020 2020 2020 2020 6473 2e73 6574  ).        ds.set
-0004dc00: 5f67 656f 6d65 7472 7928 6166 6669 6e65  _geometry(affine
-0004dc10: 2c20 7368 6170 652c 206f 7269 656e 7461  , shape, orienta
-0004dc20: 7469 6f6e 290a 0a20 2020 2023 2041 646a  tion)..    # Adj
-0004dc30: 7573 7420 6461 7461 7365 7420 746f 2062  ust dataset to b
-0004dc40: 6520 666f 7220 5374 7275 6374 7572 6553  e for StructureS
-0004dc50: 6574 2069 6e73 7465 6164 206f 6620 696d  et instead of im
-0004dc60: 6167 650a 0a0a 6465 6620 6469 636f 6d5f  age...def dicom_
-0004dc70: 6461 7461 7365 745f 746f 5f73 7472 7563  dataset_to_struc
-0004dc80: 7475 7265 5f73 6574 2864 7329 3a0a 2020  ture_set(ds):.  
-0004dc90: 2020 2727 2743 6f6e 7665 7274 2061 6e20    '''Convert an 
-0004dca0: 6578 6973 7469 6e67 2069 6d61 6765 2064  existing image d
-0004dcb0: 6963 6f6d 2064 6174 6173 6574 2074 6f20  icom dataset to 
-0004dcc0: 6120 5374 7275 6374 7572 6553 6574 2064  a StructureSet d
-0004dcd0: 6174 6173 6574 2e27 2727 0a0a 2020 2020  ataset.'''..    
-0004dce0: 2320 4164 6a75 7374 2063 6c61 7373 2055  # Adjust class U
-0004dcf0: 4944 730a 2020 2020 6473 2e66 696c 655f  IDs.    ds.file_
-0004dd00: 6d65 7461 2e49 6d70 6c65 6d65 6e74 6174  meta.Implementat
-0004dd10: 696f 6e43 6c61 7373 5549 4420 3d20 2239  ionClassUID = "9
-0004dd20: 2e39 2e39 2e31 3030 2e30 2e30 2e31 2e30  .9.9.100.0.0.1.0
-0004dd30: 2e39 2e36 2e30 2e30 2e31 220a 2020 2020  .9.6.0.0.1".    
-0004dd40: 6473 2e66 696c 655f 6d65 7461 2e4d 6564  ds.file_meta.Med
-0004dd50: 6961 5374 6f72 6167 6553 4f50 436c 6173  iaStorageSOPClas
-0004dd60: 7355 4944 203d 2022 312e 322e 3834 302e  sUID = "1.2.840.
-0004dd70: 3130 3030 382e 352e 312e 342e 312e 312e  10008.5.1.4.1.1.
-0004dd80: 3438 312e 3322 0a0a 2020 2020 2320 4173  481.3"..    # As
-0004dd90: 7369 676e 2065 6d70 7479 2073 6571 7565  sign empty seque
-0004dda0: 6e63 6573 0a20 2020 2064 732e 5265 6665  nces.    ds.Refe
-0004ddb0: 7265 6e63 6564 4672 616d 656f 6652 6566  rencedFrameofRef
-0004ddc0: 6572 656e 6365 5365 7175 656e 6365 203d  erenceSequence =
-0004ddd0: 2053 6571 7565 6e63 6528 290a 2020 2020   Sequence().    
-0004dde0: 6473 2e53 7472 7563 7475 7265 5365 7452  ds.StructureSetR
-0004ddf0: 4f49 5365 7175 656e 6365 203d 2053 6571  OISequence = Seq
-0004de00: 7565 6e63 6528 290a 2020 2020 6473 2e52  uence().    ds.R
-0004de10: 5452 4f49 4f62 7365 7276 6174 696f 6e73  TROIObservations
-0004de20: 5365 7175 656e 6365 203d 2053 6571 7565  Sequence = Seque
-0004de30: 6e63 6528 290a 2020 2020 6473 2e52 4f49  nce().    ds.ROI
-0004de40: 436f 6e74 6f75 7253 6571 7565 6e63 6520  ContourSequence 
-0004de50: 3d20 5365 7175 656e 6365 2829 0a0a 2020  = Sequence()..  
-0004de60: 2020 2320 4173 7369 676e 2073 7472 7563    # Assign struc
-0004de70: 7475 7265 2073 6574 2070 726f 7065 7274  ture set propert
-0004de80: 6965 730a 2020 2020 6473 2e53 7472 7563  ies.    ds.Struc
-0004de90: 7475 7265 5365 744c 6162 656c 203d 2022  tureSetLabel = "
-0004dea0: 220a 2020 2020 6473 2e53 7472 7563 7475  ".    ds.Structu
-0004deb0: 7265 5365 7444 6174 6520 3d20 6473 2e49  reSetDate = ds.I
-0004dec0: 6e73 7461 6e63 6543 7265 6174 696f 6e44  nstanceCreationD
-0004ded0: 6174 650a 2020 2020 6473 2e53 7472 7563  ate.    ds.Struc
-0004dee0: 7475 7265 5365 7454 696d 6520 3d20 6473  tureSetTime = ds
-0004def0: 2e49 6e73 7461 6e63 6543 7265 6174 696f  .InstanceCreatio
-0004df00: 6e54 696d 650a 0a20 2020 2023 2041 7373  nTime..    # Ass
-0004df10: 6967 6e20 6672 616d 6520 6f66 2072 6566  ign frame of ref
-0004df20: 6572 656e 6365 0a0a 0a64 6566 2063 7265  erence...def cre
-0004df30: 6174 655f 6475 6d6d 795f 696d 6167 6528  ate_dummy_image(
-0004df40: 0a20 2020 2065 7874 656e 7473 2c20 0a20  .    extents, . 
-0004df50: 2020 2073 6c69 6365 5f74 6869 636b 6e65     slice_thickne
-0004df60: 7373 2c0a 2020 2020 7368 6170 653d 4e6f  ss,.    shape=No
-0004df70: 6e65 2c20 0a20 2020 2076 6f78 656c 5f73  ne, .    voxel_s
-0004df80: 697a 653d 4e6f 6e65 2c0a 2020 2020 6669  ize=None,.    fi
-0004df90: 6c6c 5f76 616c 3d31 6534 2c0a 2020 2020  ll_val=1e4,.    
-0004dfa0: 6275 6666 6572 3d32 0a29 3a0a 2020 2020  buffer=2.):.    
-0004dfb0: 2222 224d 616b 6520 6120 6475 6d6d 7920  """Make a dummy 
-0004dfc0: 696d 6167 6520 7468 6174 2063 6f76 6572  image that cover
-0004dfd0: 7320 7468 6520 6172 6561 2073 7061 6e6e  s the area spann
-0004dfe0: 6564 2062 7920 3c65 7874 656e 7473 3e20  ed by <extents> 
-0004dff0: 706c 7573 2061 200a 2020 2020 6275 6666  plus a .    buff
-0004e000: 6572 2e0a 0a20 2020 202a 2a50 6172 616d  er...    **Param
-0004e010: 6574 6572 733a 2a2a 0a20 2020 200a 2020  eters:**.    .  
-0004e020: 2020 6578 7465 6e74 7320 3a20 6c69 7374    extents : list
-0004e030: 0a20 2020 2020 2020 204c 6973 7420 6f66  .        List of
-0004e040: 205b 6d69 6e2c 206d 6178 5d20 6578 7465   [min, max] exte
-0004e050: 6e74 7320 696e 206d 6d20 616c 6f6e 6720  nts in mm along 
-0004e060: 6561 6368 206f 6620 7468 6520 7468 7265  each of the thre
-0004e070: 6520 6178 6573 2069 6e20 0a20 2020 2020  e axes in .     
-0004e080: 2020 206f 7264 6572 205b 782c 2079 2c20     order [x, y, 
-0004e090: 7a5d 2e0a 0a20 2020 2073 6c69 6365 5f74  z]...    slice_t
-0004e0a0: 6869 636b 6e65 7373 203a 2066 6c6f 6174  hickness : float
-0004e0b0: 0a20 2020 2020 2020 2053 6c69 6365 2074  .        Slice t
-0004e0c0: 6869 636b 6e65 7373 2069 6e20 6d6d 2e0a  hickness in mm..
-0004e0d0: 0a20 2020 2076 6f78 656c 5f73 697a 6520  .    voxel_size 
-0004e0e0: 3a20 6c69 7374 2c20 6465 6661 756c 743d  : list, default=
-0004e0f0: 4e6f 6e65 0a20 2020 2020 2020 2056 6f78  None.        Vox
-0004e100: 656c 2073 697a 6520 696e 206d 6d20 696e  el size in mm in
-0004e110: 2074 6865 2064 756d 6d79 2069 6d61 6765   the dummy image
-0004e120: 2069 6e20 7468 6520 782d 7920 706c 616e   in the x-y plan
-0004e130: 652c 2067 6976 656e 2061 7320 0a20 2020  e, given as .   
-0004e140: 2020 2020 205b 7678 2c20 7679 5d2e 2049       [vx, vy]. I
-0004e150: 6620 3c73 6861 7065 3e20 616e 6420 3c76  f <shape> and <v
-0004e160: 6f78 656c 5f73 697a 653e 2061 7265 2062  oxel_size> are b
-0004e170: 6f74 6820 4e6f 6e65 2c20 766f 7865 6c20  oth None, voxel 
-0004e180: 7369 7a65 7320 6f66 0a20 2020 2020 2020  sizes of.       
-0004e190: 205b 312c 2031 5d20 7769 6c6c 2062 6520   [1, 1] will be 
-0004e1a0: 7573 6564 2062 7920 6465 6661 756c 742e  used by default.
-0004e1b0: 2054 6865 2076 6f78 656c 2073 697a 6520   The voxel size 
-0004e1c0: 696e 2074 6865 207a 2064 6972 6563 7469  in the z directi
-0004e1d0: 6f6e 200a 2020 2020 2020 2020 7769 6c6c  on .        will
-0004e1e0: 2062 6520 7461 6b65 6e20 6672 6f6d 2074   be taken from t
-0004e1f0: 6865 206d 696e 696d 756d 2064 6973 7461  he minimum dista
-0004e200: 6e63 6520 6265 7477 6565 6e20 736c 6963  nce between slic
-0004e210: 6520 706f 7369 7469 6f6e 7320 696e 200a  e positions in .
-0004e220: 2020 2020 2020 2020 7468 6520 782d 7920          the x-y 
-0004e230: 636f 6e74 6f75 7273 2064 6963 7469 6f6e  contours diction
-0004e240: 6172 792e 0a0a 2020 2020 7368 6170 6520  ary...    shape 
-0004e250: 3a20 6c69 7374 2c20 6465 6661 756c 743d  : list, default=
-0004e260: 4e6f 6e65 0a20 2020 2020 2020 204e 756d  None.        Num
-0004e270: 6265 7220 6f66 2076 6f78 656c 7320 696e  ber of voxels in
-0004e280: 2074 6865 2064 756d 6d79 2069 6d61 6765   the dummy image
-0004e290: 2069 6e20 7468 6520 782d 7920 706c 616e   in the x-y plan
-0004e2a0: 652c 2067 6976 656e 2061 730a 2020 2020  e, given as.    
-0004e2b0: 2020 2020 5b6e 782c 206e 795d 2e20 4f6e      [nx, ny]. On
-0004e2c0: 6c79 2075 7365 6420 6966 203c 766f 7865  ly used if <voxe
-0004e2d0: 6c5f 7369 7a65 3e20 6973 204e 6f6e 652e  l_size> is None.
-0004e2e0: 200a 2020 2020 2020 2020 5468 6520 6e75   .        The nu
-0004e2f0: 6d62 6572 206f 6620 766f 7865 6c73 2069  mber of voxels i
-0004e300: 6e20 7468 6520 7a20 6469 7265 6374 696f  n the z directio
-0004e310: 6e20 7769 6c6c 2062 6520 7461 6b65 6e20  n will be taken 
-0004e320: 6672 6f6d 2074 6865 200a 2020 2020 2020  from the .      
-0004e330: 2020 6e75 6d62 6572 206f 6620 736c 6963    number of slic
-0004e340: 6573 2069 6e20 7468 6520 782d 7920 636f  es in the x-y co
-0004e350: 6e74 6f75 7273 2064 6963 7469 6f6e 6172  ntours dictionar
-0004e360: 792e 0a0a 2020 2020 6669 6c6c 5f76 616c  y...    fill_val
-0004e370: 203a 2069 6e74 2f66 6c6f 6174 2c20 6465   : int/float, de
-0004e380: 6661 756c 743d 3165 340a 2020 2020 2020  fault=1e4.      
-0004e390: 2020 5661 6c75 6520 7769 7468 2077 6869    Value with whi
-0004e3a0: 6368 2074 6865 2076 6f78 656c 7320 696e  ch the voxels in
-0004e3b0: 2074 6865 2064 756d 6d79 2069 6d61 6765   the dummy image
-0004e3c0: 2073 686f 756c 6420 6265 2066 696c 6c65   should be fille
-0004e3d0: 642e 200a 0a20 2020 2062 7566 6665 7220  d. ..    buffer 
-0004e3e0: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
-0004e3f0: 3d32 0a20 2020 2020 2020 2042 7566 6665  =2.        Buffe
-0004e400: 7220 616d 6f75 6e74 206f 6620 7768 6974  r amount of whit
-0004e410: 6573 7061 6365 2069 6e20 6d6d 2074 6f20  espace in mm to 
-0004e420: 6164 6420 6f75 7473 6964 6520 7468 6520  add outside the 
-0004e430: 524f 4920 696e 2065 6163 6820 0a20 2020  ROI in each .   
-0004e440: 2020 2020 2064 6972 6563 7469 6f6e 2e0a       direction..
-0004e450: 2020 2020 2222 220a 0a20 2020 2023 2041      """..    # A
-0004e460: 7373 6967 6e20 6465 6661 756c 7420 766f  ssign default vo
-0004e470: 7865 6c20 7369 7a65 0a20 2020 2069 6620  xel size.    if 
-0004e480: 7368 6170 6520 6973 204e 6f6e 6520 616e  shape is None an
-0004e490: 6420 766f 7865 6c5f 7369 7a65 2069 7320  d voxel_size is 
-0004e4a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 766f  None:.        vo
-0004e4b0: 7865 6c5f 7369 7a65 203d 205b 312c 2031  xel_size = [1, 1
-0004e4c0: 5d0a 2020 2020 6966 206e 6f74 2073 6b72  ].    if not skr
-0004e4d0: 742e 636f 7265 2e69 735f 6c69 7374 2876  t.core.is_list(v
-0004e4e0: 6f78 656c 5f73 697a 6529 3a0a 2020 2020  oxel_size):.    
-0004e4f0: 2020 2020 766f 7865 6c5f 7369 7a65 203d      voxel_size =
-0004e500: 205b 766f 7865 6c5f 7369 7a65 5d20 2a20   [voxel_size] * 
-0004e510: 320a 0a20 2020 2023 2043 616c 6375 6c61  2..    # Calcula
-0004e520: 7465 2076 6f78 656c 2073 697a 6573 2066  te voxel sizes f
-0004e530: 726f 6d20 7368 6170 650a 2020 2020 6966  rom shape.    if
-0004e540: 2073 6861 7065 2069 7320 6e6f 7420 4e6f   shape is not No
-0004e550: 6e65 3a0a 2020 2020 2020 2020 7368 6170  ne:.        shap
-0004e560: 6520 3d20 6c69 7374 2873 6861 7065 290a  e = list(shape).
-0004e570: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
-0004e580: 6861 7065 2920 213d 2032 3a0a 2020 2020  hape) != 2:.    
-0004e590: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
-0004e5a0: 7065 4572 726f 7228 2253 6861 7065 2073  peError("Shape s
-0004e5b0: 686f 756c 6420 6265 2061 206c 6973 7420  hould be a list 
-0004e5c0: 6f66 2074 776f 2076 616c 7565 7320 220a  of two values ".
-0004e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004e5e0: 2020 2020 2020 2020 2020 2020 2273 7065              "spe
-0004e5f0: 6369 6679 696e 6720 6475 6d6d 7920 696d  cifying dummy im
-0004e600: 6167 6520 7368 6170 6520 696e 2074 6865  age shape in the
-0004e610: 205b 782c 2079 5d20 220a 2020 2020 2020   [x, y] ".      
-0004e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004e630: 2020 2020 2020 2264 6972 6563 7469 6f6e        "direction
-0004e640: 732e 2229 0a0a 2020 2020 2020 2020 2320  s.")..        # 
-0004e650: 4361 6c63 756c 6174 6520 766f 7865 6c20  Calculate voxel 
-0004e660: 7369 7a65 2069 6620 524f 4920 6578 7465  size if ROI exte
-0004e670: 6e74 2070 6c75 7320 6275 6666 6572 2069  nt plus buffer i
-0004e680: 7320 6469 7669 6465 6420 6279 2073 6861  s divided by sha
-0004e690: 7065 0a20 2020 2020 2020 2076 6f78 656c  pe.        voxel
-0004e6a0: 5f73 697a 6520 3d20 5b28 6d61 7828 6578  _size = [(max(ex
-0004e6b0: 2920 2d20 6d69 6e28 6578 2920 2b20 3220  ) - min(ex) + 2 
-0004e6c0: 2a20 6275 6666 6572 2920 2f20 7368 6170  * buffer) / shap
-0004e6d0: 655b 695d 0a20 2020 2020 2020 2020 2020  e[i].           
-0004e6e0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0004e6f0: 2c20 6578 2069 6e20 656e 756d 6572 6174  , ex in enumerat
-0004e700: 6528 6578 7465 6e74 735b 3a32 5d29 5d0a  e(extents[:2])].
-0004e710: 0a20 2020 2023 204f 7468 6572 7769 7365  .    # Otherwise
-0004e720: 2c20 6361 6c63 756c 6174 6520 7368 6170  , calculate shap
-0004e730: 6520 6672 6f6d 2076 6f78 656c 2073 697a  e from voxel siz
-0004e740: 6573 0a20 2020 2065 6c73 653a 0a20 2020  es.    else:.   
-0004e750: 2020 2020 2076 6f78 656c 5f73 697a 6520       voxel_size 
-0004e760: 3d20 6c69 7374 2876 6f78 656c 5f73 697a  = list(voxel_siz
-0004e770: 6529 0a20 2020 2020 2020 200a 2020 2020  e).        .    
-0004e780: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
-0004e790: 6e75 6d62 6572 206f 6620 766f 7865 6c73  number of voxels
-0004e7a0: 206e 6565 6465 6420 746f 2063 6f76 6572   needed to cover
-0004e7b0: 2052 4f49 2070 6c75 7320 6275 6666 6572   ROI plus buffer
-0004e7c0: 2065 6163 6820 7369 6465 0a20 2020 2020   each side.     
-0004e7d0: 2020 2073 6861 7065 203d 205b 286e 702e     shape = [(np.
-0004e7e0: 6365 696c 2828 6d61 7828 6578 2920 2d20  ceil((max(ex) - 
-0004e7f0: 6d69 6e28 6578 2929 202b 2032 202a 2062  min(ex)) + 2 * b
-0004e800: 7566 6665 7229 202f 2076 6f78 656c 5f73  uffer) / voxel_s
-0004e810: 697a 655b 695d 2920 0a20 2020 2020 2020  ize[i]) .       
-0004e820: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
-0004e830: 2065 7820 696e 2065 6e75 6d65 7261 7465   ex in enumerate
-0004e840: 2865 7874 656e 7473 5b3a 325d 295d 0a0a  (extents[:2])]..
-0004e850: 2020 2020 2320 4765 7420 7a20 766f 7865      # Get z voxe
-0004e860: 6c20 7369 7a65 2061 6e64 2073 6861 7065  l size and shape
-0004e870: 0a20 2020 2076 6f78 656c 5f73 697a 652e  .    voxel_size.
-0004e880: 6170 7065 6e64 2873 6c69 6365 5f74 6869  append(slice_thi
-0004e890: 636b 6e65 7373 290a 2020 2020 7368 6170  ckness).    shap
-0004e8a0: 655f 7a20 3d20 286d 6178 2865 7874 656e  e_z = (max(exten
-0004e8b0: 7473 5b32 5d29 202d 206d 696e 2865 7874  ts[2]) - min(ext
-0004e8c0: 656e 7473 5b32 5d29 2920 2f20 736c 6963  ents[2])) / slic
-0004e8d0: 655f 7468 6963 6b6e 6573 730a 0a20 2020  e_thickness..   
-0004e8e0: 2023 2041 6464 206e 6561 7265 7374 2069   # Add nearest i
-0004e8f0: 6e74 6567 6572 206e 756d 6265 7220 6f66  nteger number of
-0004e900: 2062 7566 6665 7220 766f 7865 6c73 0a20   buffer voxels. 
-0004e910: 2020 206e 5f62 7566 665f 7a20 3d20 6e70     n_buff_z = np
-0004e920: 2e63 6569 6c28 6275 6666 6572 202f 2073  .ceil(buffer / s
-0004e930: 6c69 6365 5f74 6869 636b 6e65 7373 290a  lice_thickness).
-0004e940: 2020 2020 7368 6170 652e 6170 7065 6e64      shape.append
-0004e950: 2873 6861 7065 5f7a 202b 2032 202a 206e  (shape_z + 2 * n
-0004e960: 5f62 7566 665f 7a29 0a20 2020 2073 6861  _buff_z).    sha
-0004e970: 7065 203d 205b 696e 7428 7329 2066 6f72  pe = [int(s) for
-0004e980: 2073 2069 6e20 7368 6170 655d 0a0a 2020   s in shape]..  
-0004e990: 2020 2320 4765 7420 6f72 6967 696e 2070    # Get origin p
-0004e9a0: 6f73 6974 696f 6e3b 2065 6e73 7572 6520  osition; ensure 
-0004e9b0: 7468 6174 206f 7269 6769 6e20 706f 696e  that origin poin
-0004e9c0: 7473 2074 6f20 6365 6e74 7265 206f 6620  ts to centre of 
-0004e9d0: 6275 6666 6572 2076 6f78 656c 200a 2020  buffer voxel .  
-0004e9e0: 2020 2320 6f75 7473 6964 6520 524f 490a    # outside ROI.
-0004e9f0: 2020 2020 6f72 6967 696e 203d 205b 6d69      origin = [mi
-0004ea00: 6e28 6578 2920 2b20 6162 7328 766f 7865  n(ex) + abs(voxe
-0004ea10: 6c5f 7369 7a65 5b69 5d29 202a 2030 2e35  l_size[i]) * 0.5
-0004ea20: 202d 2062 7566 6665 720a 2020 2020 2020   - buffer.      
-0004ea30: 2020 2020 2020 2020 666f 7220 692c 2065          for i, e
-0004ea40: 7820 696e 2065 6e75 6d65 7261 7465 2865  x in enumerate(e
-0004ea50: 7874 656e 7473 5b3a 325d 295d 0a20 2020  xtents[:2])].   
-0004ea60: 206f 7269 6769 6e2e 6170 7065 6e64 286d   origin.append(m
-0004ea70: 696e 2865 7874 656e 7473 5b32 5d29 202d  in(extents[2]) -
-0004ea80: 2061 6273 2873 6c69 6365 5f74 6869 636b   abs(slice_thick
-0004ea90: 6e65 7373 2920 2a20 286e 5f62 7566 665f  ness) * (n_buff_
-0004eaa0: 7a20 2d20 302e 3529 290a 0a20 2020 2023  z - 0.5))..    #
-0004eab0: 2043 7265 6174 6520 696d 6167 650a 2020   Create image.  
-0004eac0: 2020 7265 7475 726e 2073 6b72 742e 696d    return skrt.im
-0004ead0: 6167 652e 496d 6167 6528 0a20 2020 2020  age.Image(.     
-0004eae0: 2020 206e 702e 6f6e 6573 2828 7368 6170     np.ones((shap
-0004eaf0: 655b 315d 2c20 7368 6170 655b 305d 2c20  e[1], shape[0], 
-0004eb00: 7368 6170 655b 325d 2929 202a 2066 696c  shape[2])) * fil
-0004eb10: 6c5f 7661 6c2c 0a20 2020 2020 2020 2076  l_val,.        v
-0004eb20: 6f78 656c 5f73 697a 653d 766f 7865 6c5f  oxel_size=voxel_
-0004eb30: 7369 7a65 2c0a 2020 2020 2020 2020 6f72  size,.        or
-0004eb40: 6967 696e 3d6f 7269 6769 6e0a 2020 2020  igin=origin.    
-0004eb50: 290a 0a0a 6465 6620 6372 6561 7465 5f73  )...def create_s
-0004eb60: 7461 706c 6528 726f 6973 2c20 2a2a 6b77  taple(rois, **kw
-0004eb70: 6172 6773 293a 0a20 2020 2022 2222 4372  args):.    """Cr
-0004eb80: 6561 7465 2053 5441 504c 4520 524f 4920  eate STAPLE ROI 
-0004eb90: 6672 6f6d 206c 6973 7420 6f66 2052 4f49  from list of ROI
-0004eba0: 732e 2222 220a 0a20 2020 2023 2054 7279  s."""..    # Try
-0004ebb0: 2069 6d70 6f72 7420 5369 6d70 6c65 4954   import SimpleIT
-0004ebc0: 4b0a 2020 2020 7472 793a 0a20 2020 2020  K.    try:.     
-0004ebd0: 2020 2069 6d70 6f72 7420 5369 6d70 6c65     import Simple
-0004ebe0: 4954 4b20 6173 2073 6974 6b0a 2020 2020  ITK as sitk.    
-0004ebf0: 6578 6365 7074 204d 6f64 756c 654e 6f74  except ModuleNot
-0004ec00: 466f 756e 6445 7272 6f72 3a0a 2020 2020  FoundError:.    
-0004ec10: 2020 2020 7261 6973 6520 4d6f 6475 6c65      raise Module
-0004ec20: 4e6f 7446 6f75 6e64 4572 726f 7228 2253  NotFoundError("S
-0004ec30: 696d 706c 6549 544b 2069 7320 7265 7175  impleITK is requ
-0004ec40: 6972 6564 2074 6f20 6361 6c63 756c 6174  ired to calculat
-0004ec50: 6520 5354 4150 4c45 2063 6f6e 746f 7572  e STAPLE contour
-0004ec60: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
-0004ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004ec80: 2020 2020 2020 2254 7279 2069 6e73 7461        "Try insta
-0004ec90: 6c6c 696e 6720 7669 613a 2070 6970 2069  lling via: pip i
-0004eca0: 6e73 7461 6c6c 2073 696d 706c 6569 746b  nstall simpleitk
-0004ecb0: 2229 0a0a 2020 2020 2320 4765 7420 5354  ")..    # Get ST
-0004ecc0: 4150 4c45 206d 6173 6b0a 2020 2020 726f  APLE mask.    ro
-0004ecd0: 695f 6172 7261 7973 203d 205b 5d0a 2020  i_arrays = [].  
-0004ece0: 2020 666f 7220 726f 6920 696e 2072 6f69    for roi in roi
-0004ecf0: 733a 0a20 2020 2020 2020 2072 6f69 5f61  s:.        roi_a
-0004ed00: 7272 6179 732e 6170 7065 6e64 2873 6974  rrays.append(sit
-0004ed10: 6b2e 4765 7449 6d61 6765 4672 6f6d 4172  k.GetImageFromAr
-0004ed20: 7261 7928 726f 692e 6765 745f 6d61 736b  ray(roi.get_mask
-0004ed30: 280a 2020 2020 2020 2020 2020 2020 7374  (.            st
-0004ed40: 616e 6461 7264 6973 653d 5472 7565 292e  andardise=True).
-0004ed50: 6173 7479 7065 2869 6e74 2929 290a 2020  astype(int))).  
-0004ed60: 2020 7072 6f62 7320 3d20 7369 746b 2e47    probs = sitk.G
-0004ed70: 6574 4172 7261 7946 726f 6d49 6d61 6765  etArrayFromImage
-0004ed80: 2873 6974 6b2e 5354 4150 4c45 2872 6f69  (sitk.STAPLE(roi
-0004ed90: 5f61 7272 6179 732c 2031 2929 0a20 2020  _arrays, 1)).   
-0004eda0: 206d 6173 6b20 3d20 7072 6f62 7320 3e20   mask = probs > 
-0004edb0: 302e 3935 0a0a 2020 2020 2320 4372 6561  0.95..    # Crea
-0004edc0: 7465 2053 5441 504c 4520 524f 4920 6f62  te STAPLE ROI ob
-0004edd0: 6a65 6374 0a20 2020 2072 6574 7572 6e20  ject.    return 
-0004ede0: 524f 4928 6d61 736b 2c20 2a2a 6b77 6172  ROI(mask, **kwar
-0004edf0: 6773 290a 0a0a 6465 6620 6372 6561 7465  gs)...def create
-0004ee00: 5f6d 616a 6f72 6974 795f 766f 7465 2872  _majority_vote(r
-0004ee10: 6f69 732c 202a 2a6b 7761 7267 7329 3a0a  ois, **kwargs):.
-0004ee20: 2020 2020 2222 2243 7265 6174 6520 6d61      """Create ma
-0004ee30: 6a6f 7269 7479 2076 6f74 6520 524f 4920  jority vote ROI 
-0004ee40: 6672 6f6d 206c 6973 7420 6f66 2052 4f49  from list of ROI
-0004ee50: 732e 2222 220a 0a20 2020 206d 6173 6b20  s."""..    mask 
-0004ee60: 3d20 726f 6973 5b30 5d2e 6765 745f 6d61  = rois[0].get_ma
-0004ee70: 736b 2873 7461 6e64 6172 6469 7365 3d54  sk(standardise=T
-0004ee80: 7275 6529 2e61 7374 7970 6528 696e 7429  rue).astype(int)
-0004ee90: 0a20 2020 2066 6f72 2072 6f69 2069 6e20  .    for roi in 
-0004eea0: 726f 6973 5b31 3a5d 3a0a 2020 2020 2020  rois[1:]:.      
-0004eeb0: 2020 6d61 736b 202b 3d20 726f 692e 6765    mask += roi.ge
-0004eec0: 745f 6d61 736b 2873 7461 6e64 6172 6469  t_mask(standardi
-0004eed0: 7365 3d54 7275 6529 2e61 7374 7970 6528  se=True).astype(
-0004eee0: 696e 7429 0a20 2020 206d 6173 6b20 3d20  int).    mask = 
-0004eef0: 6d61 736b 203e 3d20 6c65 6e28 726f 6973  mask >= len(rois
-0004ef00: 2920 2f20 320a 2020 2020 7265 7475 726e  ) / 2.    return
-0004ef10: 2052 4f49 286d 6173 6b2c 202a 2a6b 7761   ROI(mask, **kwa
-0004ef20: 7267 7329 0a0a 0a64 6566 2063 7265 6174  rgs)...def creat
-0004ef30: 655f 726f 695f 7375 6d28 726f 6973 2c20  e_roi_sum(rois, 
-0004ef40: 2a2a 6b77 6172 6773 293a 0a20 2020 2022  **kwargs):.    "
-0004ef50: 2222 4372 6561 7465 2052 4f49 2066 726f  ""Create ROI fro
-0004ef60: 6d20 7375 6d20 6f66 206c 6973 7420 6f66  m sum of list of
-0004ef70: 2052 4f49 732e 2222 220a 0a20 2020 206d   ROIs."""..    m
-0004ef80: 6173 6b20 3d20 726f 6973 5b30 5d2e 6765  ask = rois[0].ge
-0004ef90: 745f 6d61 736b 2873 7461 6e64 6172 6469  t_mask(standardi
-0004efa0: 7365 3d54 7275 6529 2e63 6f70 7928 290a  se=True).copy().
-0004efb0: 2020 2020 666f 7220 726f 6920 696e 2072      for roi in r
-0004efc0: 6f69 735b 313a 5d3a 0a20 2020 2020 2020  ois[1:]:.       
-0004efd0: 206d 6173 6b20 2b3d 2072 6f69 2e67 6574   mask += roi.get
-0004efe0: 5f6d 6173 6b28 7374 616e 6461 7264 6973  _mask(standardis
-0004eff0: 653d 5472 7565 290a 2020 2020 7265 7475  e=True).    retu
-0004f000: 726e 2052 4f49 286d 6173 6b2c 202a 2a6b  rn ROI(mask, **k
-0004f010: 7761 7267 7329 0a0a 0a64 6566 2063 7265  wargs)...def cre
-0004f020: 6174 655f 726f 695f 6f76 6572 6c61 7028  ate_roi_overlap(
-0004f030: 726f 6973 2c20 2a2a 6b77 6172 6773 293a  rois, **kwargs):
-0004f040: 0a20 2020 2022 2222 4372 6561 7465 2052  .    """Create R
-0004f050: 4f49 2066 726f 6d20 6f76 6572 6c61 7020  OI from overlap 
-0004f060: 6f66 206c 6973 7420 6f66 2052 4f49 732e  of list of ROIs.
-0004f070: 2222 220a 0a20 2020 206d 6173 6b20 3d20  """..    mask = 
-0004f080: 726f 6973 5b30 5d2e 6765 745f 6d61 736b  rois[0].get_mask
-0004f090: 2873 7461 6e64 6172 6469 7365 3d54 7275  (standardise=Tru
-0004f0a0: 6529 2e63 6f70 7928 290a 2020 2020 666f  e).copy().    fo
-0004f0b0: 7220 726f 6920 696e 2072 6f69 735b 313a  r roi in rois[1:
-0004f0c0: 5d3a 0a20 2020 2020 2020 206d 6173 6b20  ]:.        mask 
-0004f0d0: 2a3d 2072 6f69 2e67 6574 5f6d 6173 6b28  *= roi.get_mask(
-0004f0e0: 7374 616e 6461 7264 6973 653d 5472 7565  standardise=True
-0004f0f0: 290a 2020 2020 7265 7475 726e 2052 4f49  ).    return ROI
-0004f100: 286d 6173 6b2c 202a 2a6b 7761 7267 7329  (mask, **kwargs)
-0004f110: 0a0a 0a64 6566 2064 665f 746f 5f68 746d  ...def df_to_htm
-0004f120: 6c28 6466 293a 0a20 2020 2022 2222 436f  l(df):.    """Co
-0004f130: 6e76 6572 7420 6120 7061 6e64 6173 2044  nvert a pandas D
-0004f140: 6174 6146 7261 6d65 2074 6f20 6874 6d6c  ataFrame to html
-0004f150: 2e22 2222 0a0a 2020 2020 2320 436f 6e76  ."""..    # Conv
-0004f160: 6572 7420 6461 7461 6672 616d 6520 746f  ert dataframe to
-0004f170: 2048 544d 4c0a 2020 2020 6874 6d6c 203d   HTML.    html =
-0004f180: 2064 662e 6669 6c6c 6e61 2827 e280 9427   df.fillna('...'
-0004f190: 292e 746f 5f68 746d 6c28 696e 6465 783d  ).to_html(index=
-0004f1a0: 4661 6c73 6529 0a20 2020 2068 746d 6c20  False).    html 
-0004f1b0: 3d20 6874 6d6c 2e72 6570 6c61 6365 2822  = html.replace("
-0004f1c0: 5e33 222c 2022 3c73 7570 3e33 3c2f 7375  ^3", "<sup>3</su
-0004f1d0: 703e 2229 2e72 6570 6c61 6365 2822 5e32  p>").replace("^2
-0004f1e0: 222c 2022 3c73 7570 3e32 3c2f 7375 703e  ", "<sup>2</sup>
-0004f1f0: 2229 0a0a 2020 2020 2320 4164 6420 6865  ")..    # Add he
-0004f200: 6164 6572 2077 6974 6820 7374 796c 6520  ader with style 
-0004f210: 6465 7461 696c 730a 2020 2020 6865 6164  details.    head
-0004f220: 6572 203d 2022 2222 0a20 2020 2020 2020  er = """.       
-0004f230: 203c 6865 6164 3e0a 2020 2020 2020 2020   <head>.        
-0004f240: 2020 2020 3c73 7479 6c65 3e0a 2020 2020      <style>.    
-0004f250: 2020 2020 2020 2020 2020 2020 7468 2c20              th, 
-0004f260: 7464 207b 0a20 2020 2020 2020 2020 2020  td {.           
-0004f270: 2020 2020 2020 2020 2070 6164 6469 6e67           padding
-0004f280: 3a20 3270 7820 3270 783b 0a20 2020 2020  : 2px 2px;.     
-0004f290: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0004f2a0: 2020 2020 2020 2020 2020 2020 2074 6820               th 
-0004f2b0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0004f2c0: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-0004f2d0: 2d63 6f6c 6f72 3a20 7472 616e 7370 6172  -color: transpar
-0004f2e0: 656e 743b 0a20 2020 2020 2020 2020 2020  ent;.           
-0004f2f0: 2020 2020 2020 2020 2074 6578 742d 616c           text-al
-0004f300: 6967 6e3a 2063 656e 7465 723b 0a20 2020  ign: center;.   
-0004f310: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-0004f320: 2020 2020 2020 2020 2020 203c 2f73 7479             </sty
-0004f330: 6c65 3e0a 2020 2020 2020 2020 3c2f 6865  le>.        </he
-0004f340: 6164 3e0a 2020 2020 2222 220a 2020 2020  ad>.    """.    
-0004f350: 7461 626c 655f 6874 6d6c 203d 2028 0a20  table_html = (. 
-0004f360: 2020 2020 2020 2028 6865 6164 6572 202b         (header +
-0004f370: 2068 746d 6c29 0a20 2020 2020 2020 202e   html).        .
-0004f380: 7265 706c 6163 6528 2226 6774 3b22 2c20  replace("&gt;", 
-0004f390: 223e 2229 0a20 2020 2020 2020 202e 7265  ">").        .re
-0004f3a0: 706c 6163 6528 2226 6c74 3b22 2c20 223c  place("&lt;", "<
-0004f3b0: 2229 0a20 2020 2020 2020 202e 7265 706c  ").        .repl
-0004f3c0: 6163 6528 2226 616d 703b 222c 2022 2622  ace("&amp;", "&"
-0004f3d0: 290a 2020 2020 290a 2020 2020 7265 7475  ).    ).    retu
-0004f3e0: 726e 2074 6162 6c65 5f68 746d 6c0a 0a0a  rn table_html...
-0004f3f0: 6465 6620 6265 7374 5f74 6578 745f 636f  def best_text_co
-0004f400: 6c6f 7228 7265 642c 2067 7265 656e 2c20  lor(red, green, 
-0004f410: 626c 7565 293a 0a20 2020 2069 6620 2872  blue):.    if (r
-0004f420: 6564 202a 2030 2e32 3939 202b 2067 7265  ed * 0.299 + gre
-0004f430: 656e 202a 2030 2e35 3837 202b 2062 6c75  en * 0.587 + blu
-0004f440: 6520 2a20 302e 3131 3429 203e 2031 3836  e * 0.114) > 186
-0004f450: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0004f460: 2022 626c 6163 6b22 0a20 2020 2072 6574   "black".    ret
-0004f470: 7572 6e20 2277 6869 7465 220a 0a0a 6465  urn "white"...de
-0004f480: 6620 6765 745f 636f 6c6f 7265 645f 726f  f get_colored_ro
-0004f490: 695f 7374 7269 6e67 2872 6f69 2c20 6772  i_string(roi, gr
-0004f4a0: 6579 3d46 616c 7365 2c20 636f 6c6f 723d  ey=False, color=
-0004f4b0: 4e6f 6e65 293a 0a20 2020 2022 2222 4765  None):.    """Ge
-0004f4c0: 7420 524f 4920 6e61 6d65 2069 6e20 4854  t ROI name in HT
-0004f4d0: 4d4c 2077 6974 6820 6261 636b 6772 6f75  ML with backgrou
-0004f4e0: 6e64 2063 6f6c 6f72 2066 726f 6d20 726f  nd color from ro
-0004f4f0: 692e 636f 6c6f 722e 2049 6620 6772 6579  i.color. If grey
-0004f500: 3d54 7275 652c 0a20 2020 2074 6865 2062  =True,.    the b
-0004f510: 6163 6b67 726f 756e 6420 636f 6c6f 7220  ackground color 
-0004f520: 7769 6c6c 2062 6520 6772 6579 2e22 2222  will be grey."""
-0004f530: 0a0a 2020 2020 6966 2063 6f6c 6f72 2069  ..    if color i
-0004f540: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0004f550: 636f 6c6f 7220 3d20 726f 692e 636f 6c6f  color = roi.colo
-0004f560: 720a 2020 2020 6966 2067 7265 793a 0a20  r.    if grey:. 
-0004f570: 2020 2020 2020 2072 6564 2c20 6772 6565         red, gree
-0004f580: 6e2c 2062 6c75 6520 3d20 3235 352c 2032  n, blue = 255, 2
-0004f590: 3535 2c20 3235 350a 2020 2020 2020 2020  55, 255.        
-0004f5a0: 7265 642c 2067 7265 656e 2c20 626c 7565  red, green, blue
-0004f5b0: 203d 2031 3238 2c20 3132 382c 2031 3238   = 128, 128, 128
-0004f5c0: 0a20 2020 2020 2020 2074 6578 745f 636f  .        text_co
-0004f5d0: 6c20 3d20 3230 302c 2032 3030 2c20 3230  l = 200, 200, 20
-0004f5e0: 300a 2020 2020 2020 2020 2320 4176 6f69  0.        # Avoi
-0004f5f0: 6420 7365 7474 696e 6720 636f 6c6f 7572  d setting colour
-0004f600: 2066 6f72 2067 7265 7965 6420 6f75 7420   for greyed out 
-0004f610: 524f 4973 2e0a 2020 2020 2020 2020 2320  ROIs..        # 
-0004f620: 5468 6973 2067 6976 6573 2067 6f6f 6420  This gives good 
-0004f630: 7265 6164 6162 696c 6974 7920 666f 7220  readability for 
-0004f640: 626f 7468 2064 6172 6b20 616e 6420 6c69  both dark and li
-0004f650: 6768 7420 7468 656d 6573 2e0a 2020 2020  ght themes..    
-0004f660: 2020 2020 7265 7475 726e 2028 273c 703e      return ('<p>
-0004f670: 266e 6273 703b 7b7d 266e 6273 703b 3c2f  &nbsp;{}&nbsp;</
-0004f680: 703e 2729 2e66 6f72 6d61 7428 726f 692e  p>').format(roi.
-0004f690: 6e61 6d65 290a 2020 2020 656c 7365 3a0a  name).    else:.
-0004f6a0: 2020 2020 2020 2020 7265 642c 2067 7265          red, gre
-0004f6b0: 656e 2c20 626c 7565 203d 205b 6320 2a20  en, blue = [c * 
-0004f6c0: 3235 3520 666f 7220 6320 696e 2063 6f6c  255 for c in col
-0004f6d0: 6f72 5b3a 335d 5d0a 2020 2020 2020 2020  or[:3]].        
-0004f6e0: 7465 7874 5f63 6f6c 203d 2062 6573 745f  text_col = best_
-0004f6f0: 7465 7874 5f63 6f6c 6f72 2872 6564 2c20  text_color(red, 
-0004f700: 6772 6565 6e2c 2062 6c75 6529 0a20 2020  green, blue).   
-0004f710: 2072 6574 7572 6e20 280a 2020 2020 2020   return (.      
-0004f720: 2020 273c 7020 7374 796c 653d 2262 6163    '<p style="bac
-0004f730: 6b67 726f 756e 642d 636f 6c6f 723a 2072  kground-color: r
-0004f740: 6762 287b 7d2c 207b 7d2c 207b 7d29 3b20  gb({}, {}, {}); 
-0004f750: 270a 2020 2020 2020 2020 2763 6f6c 6f72  '.        'color
-0004f760: 3a20 7b7d 3b22 3e26 6e62 7370 3b7b 7d26  : {};">&nbsp;{}&
-0004f770: 6e62 7370 3b3c 2f70 3e27 0a20 2020 2029  nbsp;</p>'.    )
-0004f780: 2e66 6f72 6d61 7428 7265 642c 2067 7265  .format(red, gre
-0004f790: 656e 2c20 626c 7565 2c20 7465 7874 5f63  en, blue, text_c
-0004f7a0: 6f6c 2c20 726f 692e 6e61 6d65 290a 0a64  ol, roi.name)..d
-0004f7b0: 6566 2063 6f6d 7061 7265 5f72 6f69 5f70  ef compare_roi_p
-0004f7c0: 6169 7273 280a 2020 2020 7061 6972 732c  airs(.    pairs,
-0004f7d0: 200a 2020 2020 6874 6d6c 3d46 616c 7365   .    html=False
-0004f7e0: 2c0a 2020 2020 6e61 6d65 5f61 735f 696e  ,.    name_as_in
-0004f7f0: 6465 783d 5472 7565 2c0a 2020 2020 6772  dex=True,.    gr
-0004f800: 6579 6564 5f6f 7574 3d4e 6f6e 652c 0a20  eyed_out=None,. 
-0004f810: 2020 2063 6f6c 6f72 6564 3d46 616c 7365     colored=False
-0004f820: 2c0a 2020 2020 726f 695f 6b77 6172 6773  ,.    roi_kwargs
-0004f830: 3d7b 7d2c 0a20 2020 202a 2a6b 7761 7267  ={},.    **kwarg
-0004f840: 730a 293a 0a20 2020 2069 6620 6874 6d6c  s.):.    if html
-0004f850: 3a0a 2020 2020 2020 2020 6e61 6d65 5f61  :.        name_a
-0004f860: 735f 696e 6465 7820 3d20 4661 6c73 650a  s_index = False.
-0004f870: 2020 2020 6966 2067 7265 7965 645f 6f75      if greyed_ou
-0004f880: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
-0004f890: 2020 2067 7265 7965 645f 6f75 7420 3d20     greyed_out = 
-0004f8a0: 5b5d 0a20 2020 2064 6673 203d 205b 5d0a  [].    dfs = [].
-0004f8b0: 2020 2020 666f 7220 726f 6931 2c20 726f      for roi1, ro
-0004f8c0: 6932 2069 6e20 7061 6972 733a 0a0a 2020  i2 in pairs:..  
-0004f8d0: 2020 2020 2020 2320 4765 7420 4461 7461        # Get Data
-0004f8e0: 4672 616d 6520 666f 7220 7468 6973 2070  Frame for this p
-0004f8f0: 6169 720a 2020 2020 2020 2020 6466 5f72  air.        df_r
-0004f900: 6f77 203d 2072 6f69 312e 6765 745f 636f  ow = roi1.get_co
-0004f910: 6d70 6172 6973 6f6e 2872 6f69 322c 206e  mparison(roi2, n
-0004f920: 616d 655f 6173 5f69 6e64 6578 3d6e 616d  ame_as_index=nam
-0004f930: 655f 6173 5f69 6e64 6578 2c0a 2020 2020  e_as_index,.    
-0004f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004f960: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-0004f970: 2020 2020 2320 5265 706c 6163 6520 7661      # Replace va
-0004f980: 6c75 6573 2077 6974 6820 222d 2d22 2069  lues with "--" i
-0004f990: 6620 6569 7468 6572 2052 4f49 2069 7320  f either ROI is 
-0004f9a0: 6772 6579 6564 206f 7574 0a20 2020 2020  greyed out.     
-0004f9b0: 2020 2067 7265 7920 3d20 726f 6931 2069     grey = roi1 i
-0004f9c0: 6e20 6772 6579 6564 5f6f 7574 206f 7220  n greyed_out or 
-0004f9d0: 726f 6932 2069 6e20 6772 6579 6564 5f6f  roi2 in greyed_o
-0004f9e0: 7574 0a20 2020 2020 2020 2069 6620 6772  ut.        if gr
-0004f9f0: 6579 3a0a 2020 2020 2020 2020 2020 2020  ey:.            
-0004fa00: 666f 7220 636f 6c20 696e 2064 665f 726f  for col in df_ro
-0004fa10: 772e 636f 6c75 6d6e 733a 0a20 2020 2020  w.columns:.     
-0004fa20: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-0004fa30: 6c20 3d3d 2022 524f 4922 3a20 0a20 2020  l == "ROI": .   
-0004fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0004fa50: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-0004fa60: 2020 2020 2020 2020 2020 6466 5f72 6f77            df_row
-0004fa70: 5b63 6f6c 5d20 3d20 222d 2d22 0a0a 2020  [col] = "--"..  
-0004fa80: 2020 2020 2020 2320 4164 6a75 7374 2063        # Adjust c
-0004fa90: 6f6d 7061 7269 736f 6e20 6e61 6d65 0a20  omparison name. 
-0004faa0: 2020 2020 2020 2063 6f6d 705f 6e61 6d65         comp_name
-0004fab0: 203d 2072 6f69 312e 6765 745f 636f 6d70   = roi1.get_comp
-0004fac0: 6172 6973 6f6e 5f6e 616d 6528 726f 6932  arison_name(roi2
-0004fad0: 2c20 636f 6c6f 7265 643d 636f 6c6f 7265  , colored=colore
-0004fae0: 642c 2067 7265 793d 6772 6579 2c0a 2020  d, grey=grey,.  
-0004faf0: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-0004fb00: 695f 6b77 6172 6773 3d72 6f69 5f6b 7761  i_kwargs=roi_kwa
-0004fb10: 7267 7329 0a20 2020 2020 2020 2069 6620  rgs).        if 
-0004fb20: 6e61 6d65 5f61 735f 696e 6465 783a 0a20  name_as_index:. 
-0004fb30: 2020 2020 2020 2020 2020 2064 665f 726f             df_ro
-0004fb40: 772e 7265 6e61 6d65 287b 6466 5f72 6f77  w.rename({df_row
-0004fb50: 2e69 6e64 6578 5b30 5d3a 2063 6f6d 705f  .index[0]: comp_
-0004fb60: 6e61 6d65 7d2c 2069 6e70 6c61 6365 3d54  name}, inplace=T
-0004fb70: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
-0004fb80: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-0004fb90: 665f 726f 772e 696c 6f63 5b30 2c20 305d  f_row.iloc[0, 0]
-0004fba0: 203d 2063 6f6d 705f 6e61 6d65 0a0a 2020   = comp_name..  
-0004fbb0: 2020 2020 2020 6466 732e 6170 7065 6e64        dfs.append
-0004fbc0: 2864 665f 726f 7729 0a0a 2020 2020 6967  (df_row)..    ig
-0004fbd0: 6e6f 7265 5f69 6e64 6578 203d 2046 616c  nore_index = Fal
-0004fbe0: 7365 2069 6620 6e61 6d65 5f61 735f 696e  se if name_as_in
-0004fbf0: 6465 7820 656c 7365 2054 7275 650a 2020  dex else True.  
-0004fc00: 2020 6466 203d 2070 642e 636f 6e63 6174    df = pd.concat
-0004fc10: 2864 6673 2c20 6967 6e6f 7265 5f69 6e64  (dfs, ignore_ind
-0004fc20: 6578 3d69 676e 6f72 655f 696e 6465 7829  ex=ignore_index)
-0004fc30: 2069 6620 6466 7320 656c 7365 204e 6f6e   if dfs else Non
-0004fc40: 650a 2020 2020 6966 2068 746d 6c3a 0a20  e.    if html:. 
-0004fc50: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-0004fc60: 5f74 6f5f 6874 6d6c 2864 6629 0a20 2020  _to_html(df).   
-0004fc70: 2072 6574 7572 6e20 6466 0a0a 6465 6620   return df..def 
-0004fc80: 6765 745f 636f 6e66 6f72 6d69 7479 5f69  get_conformity_i
-0004fc90: 6e64 6578 280a 2020 2020 726f 6973 2c0a  ndex(.    rois,.
-0004fca0: 2020 2020 6369 5f74 7970 653d 2267 656e      ci_type="gen
-0004fcb0: 222c 0a20 2020 2073 696e 676c 655f 736c  ",.    single_sl
-0004fcc0: 6963 653d 4661 6c73 652c 0a20 2020 2076  ice=False,.    v
-0004fcd0: 6965 773d 2278 2d79 222c 200a 2020 2020  iew="x-y", .    
-0004fce0: 736c 3d4e 6f6e 652c 200a 2020 2020 6964  sl=None, .    id
-0004fcf0: 783d 4e6f 6e65 2c20 0a20 2020 2070 6f73  x=None, .    pos
-0004fd00: 3d4e 6f6e 652c 200a 2020 2020 6d65 7468  =None, .    meth
-0004fd10: 6f64 3d4e 6f6e 652c 0a20 2020 2066 6c61  od=None,.    fla
-0004fd20: 7474 656e 3d46 616c 7365 2c0a 2020 2020  tten=False,.    
-0004fd30: 293a 0a20 2020 2022 2222 0a20 2020 2047  ):.    """.    G
-0004fd40: 6574 2063 6f6e 666f 726d 6974 7920 696e  et conformity in
-0004fd50: 6465 7820 666f 7220 7477 6f20 6f72 206d  dex for two or m
-0004fd60: 6f72 6520 524f 4973 2e0a 0a20 2020 2054  ore ROIs...    T
-0004fd70: 6865 2063 6f6e 666f 726d 6974 7920 696e  he conformity in
-0004fd80: 6465 7820 6d61 7920 6265 2063 616c 6375  dex may be calcu
-0004fd90: 6c61 7465 6420 676c 6f62 616c 6c79 206f  lated globally o
-0004fda0: 7220 666f 7220 6120 7369 6e67 6c65 2073  r for a single s
-0004fdb0: 6c69 6365 2e0a 0a20 2020 2054 6869 7320  lice...    This 
-0004fdc0: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-0004fdd0: 2065 6974 6865 7220 7468 6520 7661 6c75   either the valu
-0004fde0: 6520 6f66 206f 6e65 206f 6620 7468 6520  e of one of the 
-0004fdf0: 7468 7265 6520 7479 7065 730a 2020 2020  three types.    
-0004fe00: 6f66 2063 6f6e 666f 726d 6974 7920 696e  of conformity in
-0004fe10: 6465 7820 2822 6765 6e22 2028 666f 7220  dex ("gen" (for 
-0004fe20: 6765 6e65 7261 6c69 7365 6429 2c20 2270  generalised), "p
-0004fe30: 6169 7273 222c 2022 636f 6d6d 6f6e 2229  airs", "common")
-0004fe40: 0a20 2020 2072 6566 6572 7265 6420 746f  .    referred to
-0004fe50: 2069 6e3a 0a20 2020 2068 7474 7073 3a2f   in:.    https:/
-0004fe60: 2f64 6f69 2e6f 7267 2f31 302e 3130 3838  /doi.org/10.1088
-0004fe70: 2f30 3033 312d 3931 3535 2f35 342f 392f  /0031-9155/54/9/
-0004fe80: 3031 380a 2020 2020 6f72 2061 2073 6b72  018.    or a skr
-0004fe90: 742e 636f 7265 2e44 6174 6120 6f62 6a65  t.core.Data obje
-0004fea0: 6374 2077 6974 6820 7468 6520 7661 6c75  ct with the valu
-0004feb0: 6573 206f 6620 616c 6c20 7468 7265 652e  es of all three.
-0004fec0: 0a20 2020 2046 6f72 2074 6865 2063 6173  .    For the cas
-0004fed0: 6520 6f66 2074 776f 2052 4f49 732c 2074  e of two ROIs, t
-0004fee0: 6865 2074 6872 6565 206d 6574 7269 6373  he three metrics
-0004fef0: 2061 7265 2061 6c6c 2065 7175 6976 616c   are all equival
-0004ff00: 656e 740a 2020 2020 746f 2074 6865 204a  ent.    to the J
-0004ff10: 6163 6361 7264 2063 6f6e 666f 726d 6974  accard conformit
-0004ff20: 7920 696e 6465 782e 0a0a 2020 2020 2a2a  y index...    **
-0004ff30: 5061 7261 6d65 7465 7273 3a2a 2a0a 2020  Parameters:**.  
-0004ff40: 2020 2020 2020 0a20 2020 2072 6f69 7320        .    rois 
-0004ff50: 3a20 6c69 7374 0a20 2020 2020 2020 204c  : list.        L
-0004ff60: 6973 7420 6f66 2074 776f 206f 7220 6d6f  ist of two or mo
-0004ff70: 7265 2073 6b72 742e 7374 7275 6374 7572  re skrt.structur
-0004ff80: 6573 2e52 4f49 206f 626a 6563 7473 2066  es.ROI objects f
-0004ff90: 6f72 2077 6869 6368 2063 6f6e 666f 726d  or which conform
-0004ffa0: 6974 790a 2020 2020 2020 2020 696e 6465  ity.        inde
-0004ffb0: 7820 6973 2074 6f20 6265 2063 616c 6375  x is to be calcu
-0004ffc0: 6c61 7465 642e 0a0a 2020 2020 6369 5f74  lated...    ci_t
-0004ffd0: 7970 653a 2073 7472 2c20 6465 6661 756c  ype: str, defaul
-0004ffe0: 743d 2267 656e 220a 2020 2020 2020 2020  t="gen".        
-0004fff0: 5479 7065 206f 6620 636f 6e66 6f72 6d69  Type of conformi
-00050000: 7479 2069 6e64 6578 2074 6f20 6265 2072  ty index to be r
-00050010: 6574 7572 6e65 642c 2066 726f 6d20 2267  eturned, from "g
-00050020: 656e 2220 2866 6f72 2067 656e 6572 616c  en" (for general
-00050030: 6973 6564 292c 0a20 2020 2020 2020 2022  ised),.        "
-00050040: 7061 6972 7322 2c20 2263 6f6d 6d6f 6e22  pairs", "common"
-00050050: 2e20 2049 6620 7365 7420 746f 2022 616c  .  If set to "al
-00050060: 6c22 2c20 6120 736b 7274 2e63 6f72 652e  l", a skrt.core.
-00050070: 4461 7461 206f 626a 6563 7420 7769 7468  Data object with
-00050080: 0a20 2020 2020 2020 2076 616c 7565 7320  .        values 
-00050090: 666f 7220 7468 6520 7468 7265 6520 7479  for the three ty
-000500a0: 7065 7320 6f66 2063 6f6e 666f 726d 6974  pes of conformit
-000500b0: 7920 696e 6465 7820 6973 2072 6574 7572  y index is retur
-000500c0: 6e65 642e 0a0a 2020 2020 7369 6e67 6c65  ned...    single
-000500d0: 5f73 6c69 6365 203a 2062 6f6f 6c2c 2064  _slice : bool, d
-000500e0: 6566 6175 6c74 3d46 616c 7365 0a20 2020  efault=False.   
-000500f0: 2020 2020 2049 6620 4661 6c73 652c 2074       If False, t
-00050100: 6865 2067 6c6f 6261 6c20 3344 2044 6963  he global 3D Dic
-00050110: 6520 7363 6f72 6520 6f66 2074 6865 2066  e score of the f
-00050120: 756c 6c20 524f 4973 2077 696c 6c20 6265  ull ROIs will be
-00050130: 2072 6574 7572 6e65 643b 0a20 2020 2020   returned;.     
-00050140: 2020 206f 7468 6572 7769 7365 2c20 7468     otherwise, th
-00050150: 6520 3244 2044 6963 6520 7363 6f72 6520  e 2D Dice score 
-00050160: 6f6e 2061 2073 696e 676c 6520 736c 6963  on a single slic
-00050170: 6520 7769 6c6c 2062 6520 7265 7475 726e  e will be return
-00050180: 6564 2e0a 0a20 2020 2076 6965 7720 3a20  ed...    view : 
-00050190: 7374 722c 2064 6566 6175 6c74 3d22 782d  str, default="x-
-000501a0: 7922 0a20 2020 2020 2020 204f 7269 656e  y".        Orien
-000501b0: 7461 7469 6f6e 206f 6620 736c 6963 6520  tation of slice 
-000501c0: 6f6e 2077 6869 6368 2074 6f20 6765 7420  on which to get 
-000501d0: 4469 6365 2073 636f 7265 2e20 4f6e 6c79  Dice score. Only
-000501e0: 2075 7365 6420 6966 200a 2020 2020 2020   used if .      
-000501f0: 2020 7369 6e67 6c65 5f73 6c69 6365 3d54    single_slice=T
-00050200: 7275 652e 2049 6620 7573 696e 672c 203c  rue. If using, <
-00050210: 6178 3e20 6d75 7374 2062 6520 616e 2061  ax> must be an a
-00050220: 7869 7320 7468 6174 206c 6965 7320 616c  xis that lies al
-00050230: 6f6e 670a 2020 2020 2020 2020 7468 6520  ong.        the 
-00050240: 736c 6963 6520 696e 2074 6869 7320 6f72  slice in this or
-00050250: 6965 6e74 6174 696f 6e2e 0a0a 2020 2020  ientation...    
-00050260: 736c 203a 2069 6e74 2c20 6465 6661 756c  sl : int, defaul
-00050270: 743d 4e6f 6e65 0a20 2020 2020 2020 2053  t=None.        S
-00050280: 6c69 6365 206e 756d 6265 722e 2049 6620  lice number. If 
-00050290: 6e6f 6e65 206f 6620 3c73 6c3e 2c20 3c69  none of <sl>, <i
-000502a0: 6478 3e20 6f72 203c 706f 733e 2061 7265  dx> or <pos> are
-000502b0: 2073 7570 706c 6965 6420 6275 740a 2020   supplied but.  
-000502c0: 2020 2020 2020 3c73 696e 676c 655f 736c        <single_sl
-000502d0: 6963 653e 2069 7320 5472 7565 2c20 7468  ice> is True, th
-000502e0: 6520 6365 6e74 7261 6c20 736c 6963 6520  e central slice 
-000502f0: 6f66 2074 6869 7320 524f 4920 7769 6c6c  of this ROI will
-00050300: 2062 6520 7573 6564 2e0a 0a20 2020 2069   be used...    i
-00050310: 6478 203a 2069 6e74 2c20 6465 6661 756c  dx : int, defaul
-00050320: 743d 4e6f 6e65 0a20 2020 2020 2020 2041  t=None.        A
-00050330: 7272 6179 2069 6e64 6578 206f 6620 736c  rray index of sl
-00050340: 6963 652e 2049 6620 6e6f 6e65 206f 6620  ice. If none of 
-00050350: 3c73 6c3e 2c20 3c69 6478 3e20 6f72 203c  <sl>, <idx> or <
-00050360: 706f 733e 2061 7265 2073 7570 706c 6965  pos> are supplie
-00050370: 6420 6275 740a 2020 2020 2020 2020 3c73  d but.        <s
-00050380: 696e 676c 655f 736c 6963 653e 2069 7320  ingle_slice> is 
-00050390: 5472 7565 2c20 7468 6520 6365 6e74 7261  True, the centra
-000503a0: 6c20 736c 6963 6520 6f66 2074 6869 7320  l slice of this 
-000503b0: 524f 4920 7769 6c6c 2062 6520 7573 6564  ROI will be used
-000503c0: 2e0a 0a20 2020 2070 6f73 203a 2066 6c6f  ...    pos : flo
-000503d0: 6174 2c20 6465 6661 756c 743d 4e6f 6e65  at, default=None
-000503e0: 0a20 2020 2020 2020 2053 6c69 6365 2070  .        Slice p
-000503f0: 6f73 6974 696f 6e20 696e 206d 6d2e 2049  osition in mm. I
-00050400: 6620 6e6f 6e65 206f 6620 3c73 6c3e 2c20  f none of <sl>, 
-00050410: 3c69 6478 3e20 6f72 203c 706f 733e 2061  <idx> or <pos> a
-00050420: 7265 2073 7570 706c 6965 6420 6275 740a  re supplied but.
-00050430: 2020 2020 2020 2020 3c73 696e 676c 655f          <single_
-00050440: 736c 6963 653e 2069 7320 5472 7565 2c20  slice> is True, 
-00050450: 7468 6520 6365 6e74 7261 6c20 736c 6963  the central slic
-00050460: 6520 6f66 2074 6869 7320 524f 4920 7769  e of this ROI wi
-00050470: 6c6c 2062 6520 7573 6564 2e0a 0a20 2020  ll be used...   
-00050480: 206d 6574 686f 6420 3a20 7374 722c 2064   method : str, d
-00050490: 6566 6175 6c74 3d4e 6f6e 650a 2020 2020  efault=None.    
-000504a0: 2020 2020 4d65 7468 6f64 2074 6f20 7573      Method to us
-000504b0: 6520 666f 7220 4469 6365 2073 636f 7265  e for Dice score
-000504c0: 2063 616c 6375 6c61 7469 6f6e 2e20 4361   calculation. Ca
-000504d0: 6e20 6265 3a20 0a20 2020 2020 2020 202d  n be: .        -
-000504e0: 2022 636f 6e74 6f75 7222 3a20 6765 7420   "contour": get 
-000504f0: 696e 7465 7273 6563 7469 6f6e 7320 616e  intersections an
-00050500: 6420 6172 6561 7320 6f66 2073 6861 7065  d areas of shape
-00050510: 6c79 2063 6f6e 746f 7572 732e 0a20 2020  ly contours..   
-00050520: 2020 2020 202d 2022 6d61 736b 223a 2063       - "mask": c
-00050530: 6f75 6e74 2069 6e74 6572 7365 6374 696e  ount intersectin
-00050540: 6720 766f 7865 6c73 2069 6e20 6269 6e61  g voxels in bina
-00050550: 7279 206d 6173 6b73 2e0a 2020 2020 2020  ry masks..      
-00050560: 2020 2d20 4e6f 6e65 3a20 7573 6520 7468    - None: use th
-00050570: 6520 6d65 7468 6f64 2073 6574 2069 6e20  e method set in 
-00050580: 7365 6c66 2e64 6566 6175 6c74 5f67 656f  self.default_geo
-00050590: 6d5f 6d65 7468 6f64 2e0a 2020 2020 2020  m_method..      
-000505a0: 2020 466f 7220 6d6f 7265 2074 6861 6e20    For more than 
-000505b0: 7477 6f20 524f 4973 2061 6e64 203c 6369  two ROIs and <ci
-000505c0: 5f74 7970 653e 2022 636f 6d6d 6f6e 222c  _type> "common",
-000505d0: 206f 6e6c 7920 7468 6520 226d 6173 6b22   only the "mask"
-000505e0: 0a20 2020 2020 2020 206d 6574 686f 6420  .        method 
-000505f0: 6973 2069 6d70 6c65 6d65 6e74 6564 2e0a  is implemented..
-00050600: 0a20 2020 2066 6c61 7474 656e 203a 2062  .    flatten : b
-00050610: 6f6f 6c2c 2064 6566 6175 6c74 3d46 616c  ool, default=Fal
-00050620: 7365 0a20 2020 2020 2020 2049 6620 5472  se.        If Tr
-00050630: 7565 2c20 616c 6c20 736c 6963 6573 2077  ue, all slices w
-00050640: 696c 6c20 6265 2066 6c61 7474 656e 6564  ill be flattened
-00050650: 2069 6e20 7468 6520 6769 7665 6e20 6f72   in the given or
-00050660: 6965 6e74 6174 696f 6e20 616e 640a 2020  ientation and.  
-00050670: 2020 2020 2020 7468 6520 4469 6365 2073        the Dice s
-00050680: 636f 7265 206f 6620 7468 6520 666c 6174  core of the flat
-00050690: 7465 6e65 6420 736c 6963 6573 2077 696c  tened slices wil
-000506a0: 6c20 6265 2072 6574 7572 6e65 642e 204f  l be returned. O
-000506b0: 6e6c 7920 0a20 2020 2020 2020 2061 7661  nly .        ava
-000506c0: 696c 6162 6c65 2069 6620 6d65 7468 6f64  ilable if method
-000506d0: 3d22 6d61 736b 222e 0a20 2020 2022 2222  ="mask"..    """
-000506e0: 0a0a 2020 2020 2320 5265 7175 6972 6520  ..    # Require 
-000506f0: 7661 6c69 6420 696e 7075 7473 2e0a 2020  valid inputs..  
-00050700: 2020 6966 206c 656e 2872 6f69 7329 203c    if len(rois) <
-00050710: 2032 206f 7220 6369 5f74 7970 6520 6e6f   2 or ci_type no
-00050720: 7420 696e 205b 2263 6f6d 6d6f 6e22 2c20  t in ["common", 
-00050730: 2267 656e 222c 2022 7061 6972 7322 2c20  "gen", "pairs", 
-00050740: 2261 6c6c 225d 3a0a 2020 2020 2020 2020  "all"]:.        
-00050750: 7265 7475 726e 0a0a 2020 2020 2320 496e  return..    # In
-00050760: 6974 6961 6c69 7365 2044 6174 6120 6f62  itialise Data ob
-00050770: 6a65 6374 2066 6f72 2063 6f6e 666f 726d  ject for conform
-00050780: 6974 7920 696e 6469 6365 732e 0a20 2020  ity indices..   
-00050790: 2063 6920 3d20 736b 7274 2e63 6f72 652e   ci = skrt.core.
-000507a0: 4461 7461 287b 2263 6f6d 6d6f 6e22 3a20  Data({"common": 
-000507b0: 302c 2022 6765 6e22 3a30 2c20 2270 6169  0, "gen":0, "pai
-000507c0: 7273 223a 307d 290a 0a20 2020 2023 2044  rs":0})..    # D
-000507d0: 6561 6c20 7769 7468 2063 6173 6573 2022  eal with cases "
-000507e0: 6765 6e22 2061 6e64 2022 7061 6972 7322  gen" and "pairs"
-000507f0: 2e0a 2020 2020 230a 2020 2020 2320 466f  ..    #.    # Fo
-00050800: 7220 2267 656e 222c 2074 6865 2063 6f6e  r "gen", the con
-00050810: 666f 726d 6974 7920 696e 6465 7820 6973  formity index is
-00050820: 2063 616c 6375 6c61 7465 6420 6173 2074   calculated as t
-00050830: 6865 2072 6174 696f 206f 660a 2020 2020  he ratio of.    
-00050840: 2320 2831 2920 7468 6520 7375 6d20 6f66  # (1) the sum of
-00050850: 2074 6865 2069 6e74 6572 7365 6374 696f   the intersectio
-00050860: 6e73 2066 6f72 2061 6c6c 2070 6169 7273  ns for all pairs
-00050870: 2074 6f20 2832 2920 7468 6520 7375 6d20   to (2) the sum 
-00050880: 6f66 0a20 2020 2023 2074 6865 2075 6e69  of.    # the uni
-00050890: 6f6e 7320 666f 7220 616c 6c20 7061 6972  ons for all pair
-000508a0: 732e 0a20 2020 2023 0a20 2020 2023 2046  s..    #.    # F
-000508b0: 6f72 2022 7061 6972 732c 2074 6865 2063  or "pairs, the c
-000508c0: 6f6e 666f 726d 6974 7920 696e 6465 7820  onformity index 
-000508d0: 6973 2063 616c 6375 616c 7465 6420 6173  is calcualted as
-000508e0: 2074 6865 206d 6561 6e20 6f66 2074 6865   the mean of the
-000508f0: 0a20 2020 2023 204a 6163 6361 7264 2063  .    # Jaccard c
-00050900: 6f6e 666f 726d 6974 7920 696e 6469 6365  onformity indice
-00050910: 7320 666f 7220 616c 6c20 7061 6972 732e  s for all pairs.
-00050920: 0a0a 2020 2020 6e75 6d65 7261 746f 7220  ..    numerator 
-00050930: 3d20 300a 2020 2020 6465 6e6f 6d69 6e61  = 0.    denomina
-00050940: 746f 7220 3d20 300a 2020 2020 6e5f 7061  tor = 0.    n_pa
-00050950: 6972 203d 2030 0a20 2020 2066 6f72 2069  ir = 0.    for i
-00050960: 6478 3120 696e 2072 616e 6765 286c 656e  dx1 in range(len
-00050970: 2872 6f69 7329 202d 2031 293a 0a20 2020  (rois) - 1):.   
-00050980: 2020 2020 2066 6f72 2069 6478 3220 696e       for idx2 in
-00050990: 2072 616e 6765 2869 6478 3120 2b20 312c   range(idx1 + 1,
-000509a0: 206c 656e 2872 6f69 7329 293a 0a20 2020   len(rois)):.   
-000509b0: 2020 2020 2020 2020 2072 6f69 3120 3d20           roi1 = 
-000509c0: 726f 6973 5b69 6478 315d 0a20 2020 2020  rois[idx1].     
-000509d0: 2020 2020 2020 2072 6f69 3220 3d20 726f         roi2 = ro
-000509e0: 6973 5b69 6478 325d 0a20 2020 2020 2020  is[idx2].       
-000509f0: 2020 2020 2069 6e74 6572 7365 6374 696f       intersectio
-00050a00: 6e2c 2075 6e69 6f6e 2c20 6d65 616e 5f73  n, union, mean_s
-00050a10: 697a 6520 3d20 280a 2020 2020 2020 2020  ize = (.        
-00050a20: 2020 2020 2020 2020 2020 2020 726f 6931              roi1
-00050a30: 2e67 6574 5f69 6e74 6572 7365 6374 696f  .get_intersectio
-00050a40: 6e5f 756e 696f 6e5f 7369 7a65 2872 6f69  n_union_size(roi
-00050a50: 322c 2073 696e 676c 655f 736c 6963 652c  2, single_slice,
-00050a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00050a70: 2020 2020 2020 2020 2076 6965 772c 2073           view, s
-00050a80: 6c2c 2069 6478 2c20 706f 732c 206d 6574  l, idx, pos, met
-00050a90: 686f 642c 2066 6c61 7474 656e 2929 0a20  hod, flatten)). 
-00050aa0: 2020 2020 2020 2020 2020 206e 756d 6572             numer
-00050ab0: 6174 6f72 202b 3d20 696e 7465 7273 6563  ator += intersec
-00050ac0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00050ad0: 2064 656e 6f6d 696e 6174 6f72 202b 3d20   denominator += 
-00050ae0: 756e 696f 6e0a 2020 2020 2020 2020 2020  union.          
-00050af0: 2020 6369 2e70 6169 7273 202b 3d20 696e    ci.pairs += in
-00050b00: 7465 7273 6563 7469 6f6e 202f 2075 6e69  tersection / uni
-00050b10: 6f6e 0a20 2020 2020 2020 2020 2020 206e  on.            n
-00050b20: 5f70 6169 7220 2b3d 2031 0a0a 2020 2020  _pair += 1..    
-00050b30: 6369 2e67 656e 203d 206e 756d 6572 6174  ci.gen = numerat
-00050b40: 6f72 202f 2064 656e 6f6d 696e 6174 6f72  or / denominator
-00050b50: 0a20 2020 2063 692e 7061 6972 7320 2f3d  .    ci.pairs /=
-00050b60: 206e 5f70 6169 720a 0a20 2020 2023 2044   n_pair..    # D
-00050b70: 6561 6c20 7769 7468 2063 6173 6520 2263  eal with case "c
-00050b80: 6f6d 6d6f 6e22 2e0a 2020 2020 230a 2020  ommon"..    #.  
-00050b90: 2020 2320 5468 6520 636f 6e66 6f72 6d69    # The conformi
-00050ba0: 7479 2069 6e64 6578 2069 7320 6361 6c63  ty index is calc
-00050bb0: 756c 6174 6564 2061 7320 7468 6520 7261  ulated as the ra
-00050bc0: 7469 6f20 6f66 0a20 2020 2023 2028 3129  tio of.    # (1)
-00050bd0: 2074 6865 2063 6f6d 6d6f 6e20 696e 7465   the common inte
-00050be0: 7273 6563 7469 6f6e 206f 6620 616c 6c20  rsection of all 
-00050bf0: 524f 4973 2074 6f20 2832 2920 7468 6520  ROIs to (2) the 
-00050c00: 636f 6d62 696e 6564 2075 6e69 6f6e 0a20  combined union. 
-00050c10: 2020 2023 206f 6620 616c 6c20 524f 4973     # of all ROIs
-00050c20: 2e0a 2020 2020 6966 2032 203d 3d20 6c65  ..    if 2 == le
-00050c30: 6e28 726f 6973 293a 0a20 2020 2020 2020  n(rois):.       
-00050c40: 2069 6e74 6572 7365 6374 696f 6e2c 2075   intersection, u
-00050c50: 6e69 6f6e 2c20 6d65 616e 5f73 697a 6520  nion, mean_size 
-00050c60: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00050c70: 2020 2020 726f 6973 5b30 5d2e 6765 745f      rois[0].get_
-00050c80: 696e 7465 7273 6563 7469 6f6e 5f75 6e69  intersection_uni
-00050c90: 6f6e 5f73 697a 6528 726f 6973 5b31 5d2c  on_size(rois[1],
-00050ca0: 2073 696e 676c 655f 736c 6963 652c 0a20   single_slice,. 
-00050cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00050cc0: 2020 2020 2020 2076 6965 772c 2073 6c2c         view, sl,
-00050cd0: 2069 6478 2c20 706f 732c 206d 6574 686f   idx, pos, metho
-00050ce0: 642c 2066 6c61 7474 656e 2929 0a20 2020  d, flatten)).   
-00050cf0: 2020 2020 2063 692e 636f 6d6d 6f6e 203d       ci.common =
-00050d00: 2069 6e74 6572 7365 6374 696f 6e20 2f20   intersection / 
-00050d10: 756e 696f 6e0a 2020 2020 656c 7365 3a0a  union.    else:.
-00050d20: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00050d30: 696e 676c 655f 736c 6963 653a 0a20 2020  ingle_slice:.   
-00050d40: 2020 2020 2020 2020 206d 6173 6b5f 696e           mask_in
-00050d50: 7465 7273 6563 7469 6f6e 203d 2072 6f69  tersection = roi
-00050d60: 735b 305d 2e63 6c6f 6e65 2829 2e67 6574  s[0].clone().get
-00050d70: 5f6d 6173 6b28 0a20 2020 2020 2020 2020  _mask(.         
-00050d80: 2020 2020 2020 2020 2020 2076 6965 772c             view,
-00050d90: 2066 6c61 7474 656e 2c20 7374 616e 6461   flatten, standa
-00050da0: 7264 6973 653d 5472 7565 290a 2020 2020  rdise=True).    
-00050db0: 2020 2020 2020 2020 6d61 736b 5f75 6e69          mask_uni
-00050dc0: 6f6e 203d 2072 6f69 735b 305d 2e63 6c6f  on = rois[0].clo
-00050dd0: 6e65 2829 2e67 6574 5f6d 6173 6b28 0a20  ne().get_mask(. 
-00050de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00050df0: 2020 2076 6965 772c 2066 6c61 7474 656e     view, flatten
-00050e00: 2c20 7374 616e 6461 7264 6973 653d 5472  , standardise=Tr
-00050e10: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
-00050e20: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-00050e30: 736b 5f69 6e74 6572 7365 6374 696f 6e20  sk_intersection 
-00050e40: 3d20 726f 6973 5b30 5d2e 636c 6f6e 6528  = rois[0].clone(
-00050e50: 292e 6765 745f 736c 6963 6528 0a20 2020  ).get_slice(.   
-00050e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00050e70: 2076 6965 772c 2073 6c2c 2069 6478 2c20   view, sl, idx, 
-00050e80: 706f 7329 0a20 2020 2020 2020 2020 2020  pos).           
-00050e90: 206d 6173 6b5f 756e 696f 6e20 3d20 726f   mask_union = ro
-00050ea0: 6973 5b30 5d2e 636c 6f6e 6528 292e 6765  is[0].clone().ge
-00050eb0: 745f 736c 6963 6528 7669 6577 2c20 736c  t_slice(view, sl
-00050ec0: 2c20 6964 782c 2070 6f73 290a 0a20 2020  , idx, pos)..   
-00050ed0: 2020 2020 2066 6f72 2072 6f69 2069 6e20       for roi in 
-00050ee0: 726f 6973 5b31 3a5d 3a0a 2020 2020 2020  rois[1:]:.      
-00050ef0: 2020 2020 2020 6966 206e 6f74 2073 696e        if not sin
-00050f00: 676c 655f 736c 6963 653a 0a20 2020 2020  gle_slice:.     
-00050f10: 2020 2020 2020 2020 2020 206d 6173 6b20             mask 
-00050f20: 3d20 726f 692e 6765 745f 6d61 736b 2876  = roi.get_mask(v
-00050f30: 6965 772c 2066 6c61 7474 656e 2c20 7374  iew, flatten, st
-00050f40: 616e 6461 7264 6973 653d 5472 7565 290a  andardise=True).
-00050f50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00050f60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00050f70: 2020 6d61 736b 203d 2072 6f69 2e67 6574    mask = roi.get
-00050f80: 5f73 6c69 6365 2876 6965 772c 2073 6c2c  _slice(view, sl,
-00050f90: 2069 6478 2c20 706f 7329 0a0a 2020 2020   idx, pos)..    
-00050fa0: 2020 2020 2020 2020 6d61 736b 5f69 6e74          mask_int
-00050fb0: 6572 7365 6374 696f 6e20 3d20 286d 6173  ersection = (mas
-00050fc0: 6b5f 696e 7465 7273 6563 7469 6f6e 2026  k_intersection &
-00050fd0: 206d 6173 6b29 0a20 2020 2020 2020 2020   mask).         
-00050fe0: 2020 206d 6173 6b5f 756e 696f 6e20 3d20     mask_union = 
-00050ff0: 286d 6173 6b5f 756e 696f 6e20 7c20 6d61  (mask_union | ma
-00051000: 736b 290a 0a20 2020 2020 2020 2063 692e  sk)..        ci.
-00051010: 636f 6d6d 6f6e 203d 206d 6173 6b5f 696e  common = mask_in
-00051020: 7465 7273 6563 7469 6f6e 2e73 756d 2829  tersection.sum()
-00051030: 202f 206d 6173 6b5f 756e 696f 6e2e 7375   / mask_union.su
-00051040: 6d28 290a 0a20 2020 2072 6574 7572 6e20  m()..    return 
-00051050: 6765 7461 7474 7228 6369 2c20 6369 5f74  getattr(ci, ci_t
-00051060: 7970 652c 2063 6929 0a0a 6465 6620 6765  ype, ci)..def ge
-00051070: 745f 726f 695f 736c 6963 6528 726f 692c  t_roi_slice(roi,
-00051080: 207a 5f66 7261 6374 696f 6e3d 312c 2073   z_fraction=1, s
-00051090: 7566 6669 783d 4e6f 6e65 293a 0a20 2020  uffix=None):.   
-000510a0: 2022 2222 0a20 2020 2047 6574 2052 4f49   """.    Get ROI
-000510b0: 206f 626a 6563 7420 636f 7272 6573 706f   object correspo
-000510c0: 6e64 696e 6720 746f 2078 2d79 2073 6c69  nding to x-y sli
-000510d0: 6365 2074 6872 6f75 6768 2069 6e70 7574  ce through input
-000510e0: 2052 4f49 2e0a 0a20 2020 202a 2a50 6172   ROI...    **Par
-000510f0: 616d 6574 6572 733a 2a2a 0a0a 2020 2020  ameters:**..    
-00051100: 726f 6920 3a20 736b 7274 2e73 7472 7563  roi : skrt.struc
-00051110: 7475 7265 732e 524f 490a 2020 2020 2020  tures.ROI.      
-00051120: 2020 524f 4920 6f62 6a65 6374 2066 6f72    ROI object for
-00051130: 2077 6869 6368 2073 6c69 6365 2069 7320   which slice is 
-00051140: 746f 2062 6520 6f62 7461 696e 6564 2e0a  to be obtained..
-00051150: 0a20 2020 207a 5f66 7261 6374 696f 6e20  .    z_fraction 
-00051160: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
-00051170: 3d31 0a20 2020 2020 2020 2050 6f73 6974  =1.        Posit
-00051180: 696f 6e20 616c 6f6e 6720 7a20 6178 6973  ion along z axis
-00051190: 2061 7420 7768 6963 6820 746f 2074 616b   at which to tak
-000511a0: 6520 736c 6963 6520 7468 726f 7567 6820  e slice through 
-000511b0: 524f 492e 0a20 2020 2020 2020 2054 6865  ROI..        The
-000511c0: 2070 6f73 6974 696f 6e20 6973 2073 7065   position is spe
-000511d0: 6369 6669 6564 2061 7320 7468 6520 6672  cified as the fr
-000511e0: 6163 7469 6f6e 616c 2064 6973 7461 6e63  actional distanc
-000511f0: 650a 2020 2020 2020 2020 6672 6f6d 2074  e.        from t
-00051200: 6865 2052 4f49 2773 206d 6f73 742d 696e  he ROI's most-in
-00051210: 6665 7269 6f72 2070 6f69 6e74 3a20 3020  ferior point: 0 
-00051220: 636f 7272 6573 706f 6e64 7320 746f 0a20  corresponds to. 
-00051230: 2020 2020 2020 2074 6865 206d 6f73 742d         the most-
-00051240: 696e 6665 7269 6f72 2070 6f69 6e74 2028  inferior point (
-00051250: 6c6f 7765 7374 207a 293b 2031 2063 6f72  lowest z); 1 cor
-00051260: 7265 7370 6f6e 6473 2074 6f20 7468 650a  responds to the.
-00051270: 2020 2020 2020 2020 6d6f 7374 2d73 7570          most-sup
-00051280: 6572 696f 7220 706f 696e 7420 2868 6967  erior point (hig
-00051290: 6865 7374 207a 292e 2020 5661 6c75 6573  hest z).  Values
-000512a0: 2066 6f72 207a 5f66 7261 6374 696f 6e0a   for z_fraction.
-000512b0: 2020 2020 2020 2020 6f75 7473 6964 6520          outside 
-000512c0: 7468 6520 696e 7465 7276 616c 205b 302c  the interval [0,
-000512d0: 2031 5d20 7265 7375 6c74 2069 6e20 6120   1] result in a 
-000512e0: 5275 6e74 696d 6545 7272 6f72 2e0a 0a20  RuntimeError... 
-000512f0: 2020 2073 7566 6669 7820 3a20 7374 722c     suffix : str,
-00051300: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
-00051310: 2020 2020 2020 5375 6666 6978 2074 6f20        Suffix to 
-00051320: 6170 7065 6e64 2074 6f20 6e61 6d65 206f  append to name o
-00051330: 6620 696e 7075 7420 524f 492c 2074 6f20  f input ROI, to 
-00051340: 666f 726d 206e 616d 650a 2020 2020 2020  form name.      
-00051350: 2020 6f66 206f 7574 7075 7420 524f 492e    of output ROI.
-00051360: 2020 4966 204e 6f6e 652c 2061 7070 656e    If None, appen
-00051370: 6420 7a5f 6672 6163 7469 6f6e 2c20 7769  d z_fraction, wi
-00051380: 7468 2076 616c 7565 0a20 2020 2020 2020  th value.       
-00051390: 2067 6976 656e 2074 6f20 7477 6f20 6465   given to two de
-000513a0: 6369 6d61 6c20 706c 6163 6573 2e0a 2020  cimal places..  
-000513b0: 2020 2222 220a 2020 2020 2320 4368 6563    """.    # Chec
-000513c0: 6b20 7468 6174 207a 5f66 7261 6374 696f  k that z_fractio
-000513d0: 6e20 6973 2069 6e20 616c 6c6f 7765 6420  n is in allowed 
-000513e0: 696e 7465 7276 616c 2e0a 2020 2020 6966  interval..    if
-000513f0: 207a 5f66 7261 6374 696f 6e20 3c20 3020   z_fraction < 0 
-00051400: 6f72 207a 5f66 7261 6374 696f 6e20 3e20  or z_fraction > 
-00051410: 313a 0a20 2020 2020 2020 2072 6169 7365  1:.        raise
-00051420: 2052 756e 7469 6d65 4572 726f 7228 6622   RuntimeError(f"
-00051430: 7a5f 6672 6163 7469 6f6e 3d7b 7a5f 6672  z_fraction={z_fr
-00051440: 6163 7469 6f6e 7d22 0a20 2020 2020 2020  action}".       
-00051450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00051460: 2020 2020 2022 206f 7574 7369 6465 2061       " outside a
-00051470: 6c6c 6f77 6564 2069 6e74 6572 7661 6c20  llowed interval 
-00051480: 5b30 2c20 315d 2229 0a0a 2020 2020 2320  [0, 1]")..    # 
-00051490: 4465 7465 726d 696e 6520 7468 6520 696e  Determine the in
-000514a0: 6465 7820 6f66 2074 6865 2069 6d61 6765  dex of the image
-000514b0: 2073 6c69 6365 2061 7420 7768 6963 6820   slice at which 
-000514c0: 746f 2074 616b 6520 524f 4920 736c 6963  to take ROI slic
-000514d0: 652e 0a20 2020 2070 6f73 312c 2070 6f73  e..    pos1, pos
-000514e0: 3220 3d20 726f 692e 6765 745f 6578 7465  2 = roi.get_exte
-000514f0: 6e74 2829 0a20 2020 2070 6f73 203d 2070  nt().    pos = p
-00051500: 6f73 3120 2b20 7a5f 6672 6163 7469 6f6e  os1 + z_fraction
-00051510: 202a 2028 706f 7332 202d 2070 6f73 3129   * (pos2 - pos1)
-00051520: 0a20 2020 2069 6478 203d 2072 6f69 2e70  .    idx = roi.p
-00051530: 6f73 5f74 6f5f 6964 7828 706f 732c 2022  os_to_idx(pos, "
-00051540: 7a22 290a 0a20 2020 2023 204f 6274 6169  z")..    # Obtai
-00051550: 6e20 636f 6e74 6f75 7273 2066 6f72 2072  n contours for r
-00051560: 6571 7569 7265 6420 736c 6963 652c 2061  equired slice, a
-00051570: 6e64 2063 6f6e 7665 7274 2074 6f20 524f  nd convert to RO
-00051580: 4920 6f62 6a65 6374 2e0a 2020 2020 636f  I object..    co
-00051590: 6e74 6f75 7273 203d 2072 6f69 2e67 6574  ntours = roi.get
-000515a0: 5f63 6f6e 746f 7572 7328 6964 785f 6173  _contours(idx_as
-000515b0: 5f6b 6579 3d54 7275 6529 5b69 6478 5d0a  _key=True)[idx].
-000515c0: 2020 2020 726f 695f 736c 6963 6520 3d20      roi_slice = 
-000515d0: 524f 4928 7b72 6f69 2e69 6478 5f74 6f5f  ROI({roi.idx_to_
-000515e0: 706f 7328 6964 782c 2022 7a22 293a 2063  pos(idx, "z"): c
-000515f0: 6f6e 746f 7572 737d 290a 0a20 2020 2073  ontours})..    s
-00051600: 7566 6669 7820 3d20 6622 7b7a 5f66 7261  uffix = f"{z_fra
-00051610: 6374 696f 6e3a 2e32 667d 2220 6966 2073  ction:.2f}" if s
-00051620: 7566 6669 7820 6973 204e 6f6e 6520 656c  uffix is None el
-00051630: 7365 2073 7566 6669 780a 2020 2020 6966  se suffix.    if
-00051640: 2073 7566 6669 783a 0a20 2020 2020 2020   suffix:.       
-00051650: 2072 6f69 5f73 6c69 6365 2e6e 616d 6520   roi_slice.name 
-00051660: 3d20 6622 7b72 6f69 2e6e 616d 657d 5f7b  = f"{roi.name}_{
-00051670: 7375 6666 6978 7d22 0a20 2020 2065 6c73  suffix}".    els
-00051680: 653a 0a20 2020 2020 2020 2072 6f69 5f73  e:.        roi_s
-00051690: 6c69 6365 2e6e 616d 6520 3d20 7374 7228  lice.name = str(
-000516a0: 726f 692e 6e61 6d65 290a 0a20 2020 2072  roi.name)..    r
-000516b0: 6574 7572 6e20 726f 695f 736c 6963 650a  eturn roi_slice.
-000516c0: 0a64 6566 2067 6574 5f6d 6574 7269 635f  .def get_metric_
-000516d0: 6d65 7468 6f64 286d 6574 7269 6329 3a0a  method(metric):.
-000516e0: 2020 2020 2222 220a 2020 2020 4d61 7020      """.    Map 
-000516f0: 6265 7477 6565 6e20 6d65 7472 6963 2069  between metric i
-00051700: 6465 6e74 6966 6965 7220 6173 206c 6973  dentifier as lis
-00051710: 7465 6420 696e 2067 6574 5f63 6f6d 7061  ted in get_compa
-00051720: 7269 736f 6e5f 6d65 7472 6963 7328 290a  rison_metrics().
-00051730: 2020 2020 616e 6420 6e61 6d65 206f 6620      and name of 
-00051740: 524f 4920 6d65 7468 6f64 2066 6f72 2063  ROI method for c
-00051750: 616c 6375 6c61 7469 6e67 2074 6865 206d  alculating the m
-00051760: 6574 7269 632e 0a20 2020 200a 2020 2020  etric..    .    
-00051770: 5468 6973 2066 756e 6374 696f 6e20 6973  This function is
-00051780: 2075 7365 6420 696e 2052 4f49 2e67 6574   used in ROI.get
-00051790: 5f6d 6574 7269 635f 6279 5f73 6c69 6365  _metric_by_slice
-000517a0: 2829 2074 6f20 6465 7465 726d 696e 650a  () to determine.
-000517b0: 2020 2020 7468 6520 6d65 7468 6f64 2074      the method t
-000517c0: 6f20 6265 2063 616c 6c65 6420 666f 7220  o be called for 
-000517d0: 6561 6368 206d 6574 7269 632e 0a20 2020  each metric..   
-000517e0: 2022 2222 0a20 2020 2023 204b 6579 7320   """.    # Keys 
-000517f0: 6172 6520 6d65 7472 6963 2069 6465 6e74  are metric ident
-00051800: 6966 6965 7273 3b20 7661 6c75 6573 2061  ifiers; values a
-00051810: 7265 206e 616d 6573 206f 6620 524f 4920  re names of ROI 
-00051820: 6d65 7468 6f64 730a 2020 2020 2320 666f  methods.    # fo
-00051830: 7220 6d65 7472 6963 2063 616c 6375 6c61  r metric calcula
-00051840: 7469 6f6e 2e0a 2020 2020 2320 4d65 7472  tion..    # Metr
-00051850: 6963 7320 6172 6520 696e 636c 7564 6564  ics are included
-00051860: 2069 6e20 7468 6520 6469 6374 696f 6e61   in the dictiona
-00051870: 7279 206f 6e6c 7920 6966 2069 6465 6e74  ry only if ident
-00051880: 6966 6965 7220 616e 6420 6d65 7468 6f64  ifier and method
-00051890: 0a20 2020 2023 206e 616d 6520 6172 6520  .    # name are 
-000518a0: 6469 6666 6572 656e 742e 0a20 2020 206d  different..    m
-000518b0: 6170 7069 6e67 7320 3d20 7b0a 2020 2020  appings = {.    
-000518c0: 2020 2020 2020 2020 2261 6273 5f63 656e          "abs_cen
-000518d0: 7472 6f69 6422 3a20 2261 6273 5f63 656e  troid": "abs_cen
-000518e0: 7472 6f69 645f 6469 7374 616e 6365 222c  troid_distance",
-000518f0: 0a20 2020 2020 2020 2020 2020 2022 6365  .            "ce
-00051900: 6e74 726f 6964 223a 2022 6365 6e74 726f  ntroid": "centro
-00051910: 6964 5f64 6973 7461 6e63 6522 2c0a 2020  id_distance",.  
-00051920: 2020 2020 2020 2020 2020 2272 656c 5f61            "rel_a
-00051930: 7265 615f 6469 6666 223a 2022 7265 6c61  rea_diff": "rela
-00051940: 7469 7665 5f61 7265 615f 6469 6666 222c  tive_area_diff",
-00051950: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00051960: 2020 2072 6574 7572 6e20 6d61 7070 696e     return mappin
-00051970: 6773 2e67 6574 286d 6574 7269 632c 206d  gs.get(metric, m
-00051980: 6574 7269 6329 0a0a 6465 6620 6765 745f  etric)..def get_
-00051990: 636f 6d70 6172 6973 6f6e 5f6d 6574 7269  comparison_metri
-000519a0: 6373 2863 656e 7472 6f69 645f 636f 6d70  cs(centroid_comp
-000519b0: 6f6e 656e 7473 3d46 616c 7365 2c20 736c  onents=False, sl
-000519c0: 6963 655f 7374 6174 733d 4e6f 6e65 2c0a  ice_stats=None,.
-000519d0: 2020 2020 2020 2020 6465 6661 756c 745f          default_
-000519e0: 6279 5f73 6c69 6365 3d4e 6f6e 652c 2076  by_slice=None, v
-000519f0: 6965 773d 2278 2d79 2229 3a0a 2020 2020  iew="x-y"):.    
-00051a00: 2222 220a 2020 2020 4765 7420 6c69 7374  """.    Get list
-00051a10: 206f 6620 636f 6d70 6172 6973 6f6e 206d   of comparison m
-00051a20: 6574 7269 6373 2e0a 0a20 2020 2041 6c6c  etrics...    All
-00051a30: 206d 6574 7269 6373 206c 6973 7465 6420   metrics listed 
-00051a40: 6865 7265 2073 686f 756c 6420 6265 2072  here should be r
-00051a50: 6563 6f67 6e69 7365 6420 6279 2052 4f49  ecognised by ROI
-00051a60: 2e67 6574 5f63 6f6d 7061 7269 736f 6e28  .get_comparison(
-00051a70: 292c 0a20 2020 2061 6e64 2061 6c6c 206d  ),.    and all m
-00051a80: 6574 7269 6373 2072 6563 6f67 6e69 7365  etrics recognise
-00051a90: 6420 6279 2052 4f49 2e67 6574 5f63 6f6d  d by ROI.get_com
-00051aa0: 7061 7269 736f 6e28 2920 7368 6f75 6c64  parison() should
-00051ab0: 2062 6520 6c69 7374 6564 2068 6572 652e   be listed here.
-00051ac0: 0a0a 2020 2020 2a2a 5061 7261 6d65 7465  ..    **Paramete
-00051ad0: 7273 3a2a 2a0a 0a20 2020 2063 656e 7472  rs:**..    centr
-00051ae0: 6f69 645f 636f 6d70 6f6e 656e 7473 203a  oid_components :
-00051af0: 2062 6f6f 6c2c 2064 6566 6175 6c74 3d46   bool, default=F
-00051b00: 616c 7365 0a20 2020 2020 2020 2049 6620  alse.        If 
-00051b10: 5472 7565 2c20 7265 706c 6163 6520 6d65  True, replace me
-00051b20: 7472 6963 7320 2263 656e 7472 6f69 6422  trics "centroid"
-00051b30: 2061 6e64 2022 6365 6e74 726f 6964 5f73   and "centroid_s
-00051b40: 6c69 6365 2220 6279 2074 6865 0a20 2020  lice" by the.   
-00051b50: 2020 2020 206d 6574 7269 6373 2066 6f72       metrics for
-00051b60: 2074 6865 6972 2063 6f6d 706f 6e65 6e74   their component
-00051b70: 732e 0a0a 2020 2020 736c 6963 655f 7374  s...    slice_st
-00051b80: 6174 7320 3a20 7374 722f 6c69 7374 2f64  ats : str/list/d
-00051b90: 6963 742c 2064 6566 6175 6c74 3d4e 6f6e  ict, default=Non
-00051ba0: 650a 2020 2020 2020 2020 5370 6563 6966  e.        Specif
-00051bb0: 6963 6174 696f 6e20 6f66 2073 7461 7469  ication of stati
-00051bc0: 7374 6963 7320 746f 2062 6520 6361 6c63  stics to be calc
-00051bd0: 756c 6174 6564 2072 656c 6174 6976 650a  ulated relative.
-00051be0: 2020 2020 2020 2020 746f 2073 6c69 6365          to slice
-00051bf0: 2d62 792d 736c 6963 6520 6d65 7472 6963  -by-slice metric
-00051c00: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
-00051c10: 2020 4120 7374 6174 6973 7469 6320 6973    A statistic is
-00051c20: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
-00051c30: 6520 6e61 6d65 206f 6620 7468 6520 6675  e name of the fu
-00051c40: 6e63 7469 6f6e 2066 6f72 0a20 2020 2020  nction for.     
-00051c50: 2020 2069 7473 2063 616c 6375 6c61 7469     its calculati
-00051c60: 6f6e 2069 6e20 7468 6520 5079 7468 6f6e  on in the Python
-00051c70: 2073 7461 7469 7374 6963 7320 6d6f 6475   statistics modu
-00051c80: 6c65 3a0a 0a20 2020 2020 2020 2068 7474  le:..        htt
-00051c90: 7073 3a2f 2f64 6f63 732e 7079 7468 6f6e  ps://docs.python
-00051ca0: 2e6f 7267 2f33 2f6c 6962 7261 7279 2f73  .org/3/library/s
-00051cb0: 7461 7469 7374 6963 732e 6874 6d6c 0a0a  tatistics.html..
-00051cc0: 2020 2020 2020 2020 466f 7220 6974 7320          For its 
-00051cd0: 7573 6520 6865 7265 2c20 7468 6520 7265  use here, the re
-00051ce0: 6c65 7661 6e74 2066 756e 6374 696f 6e20  levant function 
-00051cf0: 6d75 7374 2072 6571 7569 7265 0a20 2020  must require.   
-00051d00: 2020 2020 2061 2073 696e 676c 652d 7661       a single-va
-00051d10: 7269 6162 6c65 2069 6e70 7574 2c20 6d75  riable input, mu
-00051d20: 7374 206e 6f74 2072 6571 7569 7265 2061  st not require a
-00051d30: 6e79 206b 6579 776f 7264 0a20 2020 2020  ny keyword.     
-00051d40: 2020 2061 7267 756d 656e 7473 2c20 616e     arguments, an
-00051d50: 6420 6d75 7374 2072 6574 7572 6e20 6120  d must return a 
-00051d60: 7369 6e67 6c65 206e 756d 6265 722e 0a0a  single number...
-00051d70: 2020 2020 2020 2020 4176 6169 6c61 626c          Availabl
-00051d80: 6520 6f70 7469 6f6e 7320 696e 636c 7564  e options includ
-00051d90: 653a 2022 6d65 616e 222c 2022 6d65 6469  e: "mean", "medi
-00051da0: 616e 222c 2022 6d6f 6465 222c 0a20 2020  an", "mode",.   
-00051db0: 2020 2020 2022 7374 6465 7622 2e0a 0a20       "stdev"... 
-00051dc0: 2020 2020 2020 5374 6174 6973 7469 6373        Statistics
-00051dd0: 2074 6f20 6265 2063 616c 6375 6c61 7465   to be calculate
-00051de0: 6420 6361 6e20 6265 2073 7065 6369 6669  d can be specifi
-00051df0: 6564 2075 7369 6e67 2061 6e79 206f 660a  ed using any of.
-00051e00: 2020 2020 2020 2074 6865 2066 6f6c 6c6f         the follo
-00051e10: 7769 6e67 3a0a 0a20 2020 2020 2020 2d20  wing:..       - 
-00051e20: 5374 7269 6e67 2073 7065 6369 6679 696e  String specifyin
-00051e30: 6720 7369 6e67 6c65 2073 7461 7469 7374  g single statist
-00051e40: 6963 2074 6f20 6265 2063 616c 6375 6c61  ic to be calcula
-00051e50: 7465 642c 0a20 2020 2020 2020 2020 7769  ted,.         wi
-00051e60: 7468 2073 6c69 6365 7320 636f 6e73 6964  th slices consid
-00051e70: 6572 6564 2061 7320 6769 7665 6e20 6279  ered as given by
-00051e80: 203c 6465 6661 756c 745f 6279 5f73 6c69   <default_by_sli
-00051e90: 6365 3e2c 0a20 2020 2020 2020 2020 666f  ce>,.         fo
-00051ea0: 7220 6578 616d 706c 653a 2022 6d65 616e  r example: "mean
-00051eb0: 223b 0a20 2020 2020 2020 2d20 4c69 7374  ";.       - List
-00051ec0: 2073 7065 6369 6679 696e 6720 6d75 6c74   specifying mult
-00051ed0: 6970 6c65 2073 7461 7469 7374 6963 7320  iple statistics 
-00051ee0: 746f 2062 6520 6361 6c63 756c 6174 6564  to be calculated
-00051ef0: 2c0a 2020 2020 2020 2020 2077 6974 6820  ,.         with 
-00051f00: 736c 6963 6573 2063 6f6e 7369 6465 7265  slices considere
-00051f10: 6420 6173 2067 6976 656e 2062 7920 3c64  d as given by <d
-00051f20: 6566 6175 6c74 5f62 795f 736c 6963 653e  efault_by_slice>
-00051f30: 2c0a 2020 2020 2020 2020 2066 6f72 2065  ,.         for e
-00051f40: 7861 6d70 6c65 3a20 5b22 6d65 616e 222c  xample: ["mean",
-00051f50: 2022 7374 6465 7622 5d3b 0a20 2020 2020   "stdev"];.     
-00051f60: 2020 2d20 4469 6374 696f 6e61 7279 2077    - Dictionary w
-00051f70: 6865 7265 206b 6579 7320 7370 6563 6966  here keys specif
-00051f80: 7920 736c 6963 6573 2074 6f20 6265 2063  y slices to be c
-00051f90: 6f6e 7369 6465 7265 642c 0a20 2020 2020  onsidered,.     
-00051fa0: 2020 2020 616e 6420 7661 6c75 6573 2073      and values s
-00051fb0: 7065 6369 6679 2073 7461 7469 7374 6963  pecify statistic
-00051fc0: 7320 2873 7472 696e 6720 6f72 206c 6973  s (string or lis
-00051fd0: 7429 2c20 666f 720a 2020 2020 2020 2020  t), for.        
-00051fe0: 2065 7861 6d70 6c65 3a20 7b22 756e 696f   example: {"unio
-00051ff0: 6e22 3a20 5b22 6d65 616e 222c 2022 7374  n": ["mean", "st
-00052000: 6465 7622 5d7d 2e20 2056 616c 6964 2073  dev"]}.  Valid s
-00052010: 6c69 6365 0a20 2020 2020 2020 2020 7370  lice.         sp
-00052020: 6563 6966 6963 6174 696f 6e73 2061 7265  ecifications are
-00052030: 2061 7320 6c69 7374 6564 2066 6f72 203c   as listed for <
-00052040: 6465 6661 756c 745f 6279 5f73 6c69 6365  default_by_slice
-00052050: 3e2e 0a0a 2020 2020 6465 6661 756c 745f  >...    default_
-00052060: 6279 5f73 6c69 6365 3a20 7374 722c 2064  by_slice: str, d
-00052070: 6566 6175 6c74 3d4e 6f6e 650a 2020 2020  efault=None.    
-00052080: 2020 2020 4465 6661 756c 7420 7370 6563      Default spec
-00052090: 6966 6963 6174 696f 6e20 6f66 2073 6c69  ification of sli
-000520a0: 6365 7320 746f 2062 6520 636f 6e73 6964  ces to be consid
-000520b0: 6572 6564 2077 6865 6e0a 2020 2020 2020  ered when.      
-000520c0: 2020 6361 6c63 756c 6174 696e 6720 736c    calculating sl
-000520d0: 6963 652d 6279 2d73 6c69 6365 2073 7461  ice-by-slice sta
-000520e0: 7469 7374 6963 7320 666f 7220 6120 6d65  tistics for a me
-000520f0: 7472 6963 2063 6f6d 7061 7269 6e67 0a20  tric comparing. 
-00052100: 2020 2020 2020 2074 776f 2052 4f49 732c         two ROIs,
-00052110: 2072 6f69 3120 616e 6420 726f 6932 2e20   roi1 and roi2. 
-00052120: 2054 6865 2076 616c 6964 2073 7065 6369   The valid speci
-00052130: 6669 6361 7469 6f6e 7320 6172 653a 0a0a  fications are:..
-00052140: 2020 2020 2020 2020 2d20 226c 6566 7422          - "left"
-00052150: 3a20 636f 6e73 6964 6572 206f 6e6c 7920  : consider only 
-00052160: 736c 6963 6573 2063 6f6e 7461 696e 696e  slices containin
-00052170: 6720 726f 6931 3b0a 2020 2020 2020 2020  g roi1;.        
-00052180: 2d20 2272 6967 6874 223a 2063 6f6e 7369  - "right": consi
-00052190: 6465 7220 6f6e 6c79 2073 6c69 6365 7320  der only slices 
-000521a0: 636f 6e74 6169 6e69 6e67 2072 6f69 323b  containing roi2;
-000521b0: 0a20 2020 2020 2020 202d 2022 756e 696f  .        - "unio
-000521c0: 6e22 3a20 636f 6e73 6964 6572 2073 6c69  n": consider sli
-000521d0: 6365 7320 636f 6e74 6169 6e69 6e67 2065  ces containing e
-000521e0: 6974 6865 7220 6f66 2072 6f69 3120 616e  ither of roi1 an
-000521f0: 6420 726f 6932 3b0a 2020 2020 2020 2020  d roi2;.        
-00052200: 2d20 2269 6e74 6572 7365 6374 696f 6e22  - "intersection"
-00052210: 3a20 636f 6e73 6964 6572 2073 6c69 6365  : consider slice
-00052220: 7320 636f 6e74 6169 6e69 6e67 2062 6f74  s containing bot
-00052230: 6820 726f 6931 2061 6e64 2072 6f69 322e  h roi1 and roi2.
-00052240: 0a0a 2020 2020 2020 2020 4966 204e 6f6e  ..        If Non
-00052250: 652c 2075 7365 2073 6b72 742e 636f 7265  e, use skrt.core
-00052260: 2e44 6566 6175 6c74 7328 292e 6279 5f73  .Defaults().by_s
-00052270: 6c69 6365 0a0a 2020 2020 2020 2020 7669  lice..        vi
-00052280: 6577 203a 2073 7472 2c20 6465 6661 756c  ew : str, defaul
-00052290: 743d 2278 2d79 220a 2020 2020 2020 2020  t="x-y".        
-000522a0: 2020 2020 4f72 6965 6e74 6174 696f 6e20      Orientation 
-000522b0: 746f 2063 6f6e 7369 6465 7220 7768 656e  to consider when
-000522c0: 2074 616b 696e 6720 6365 6e74 726f 6964   taking centroid
-000522d0: 2063 6f6d 706f 6e65 6e74 7320 7265 6c61   components rela
-000522e0: 7469 7665 0a20 2020 2020 2020 2020 2020  tive.           
-000522f0: 2074 6f20 6120 736c 6963 652e 2020 4361   to a slice.  Ca
-00052300: 6e20 6265 2022 782d 7922 2c20 2279 2d7a  n be "x-y", "y-z
-00052310: 222c 206f 7220 2278 2d7a 222e 0a20 2020  ", or "x-z"..   
-00052320: 2022 2222 0a20 2020 206d 6574 7269 6373   """.    metrics
-00052330: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00052340: 2022 6162 735f 6365 6e74 726f 6964 222c   "abs_centroid",
-00052350: 0a20 2020 2020 2020 2020 2020 2022 6162  .            "ab
-00052360: 735f 6365 6e74 726f 6964 5f66 6c61 7422  s_centroid_flat"
-00052370: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
-00052380: 6273 5f63 656e 7472 6f69 645f 736c 6963  bs_centroid_slic
-00052390: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-000523a0: 2261 6273 5f63 656e 7472 6f69 645f 736c  "abs_centroid_sl
-000523b0: 6963 655f 7374 6174 7322 2c0a 2020 2020  ice_stats",.    
-000523c0: 2020 2020 2020 2020 2261 7265 615f 6469          "area_di
-000523d0: 6666 222c 0a20 2020 2020 2020 2020 2020  ff",.           
-000523e0: 2022 6172 6561 5f64 6966 665f 666c 6174   "area_diff_flat
-000523f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00052400: 6172 6561 5f64 6966 665f 736c 6963 655f  area_diff_slice_
-00052410: 7374 6174 7322 2c0a 2020 2020 2020 2020  stats",.        
-00052420: 2020 2020 2261 7265 615f 7261 7469 6f22      "area_ratio"
-00052430: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
-00052440: 7265 615f 7261 7469 6f5f 666c 6174 222c  rea_ratio_flat",
-00052450: 0a20 2020 2020 2020 2020 2020 2022 6172  .            "ar
-00052460: 6561 5f72 6174 696f 5f73 6c69 6365 5f73  ea_ratio_slice_s
-00052470: 7461 7473 222c 0a20 2020 2020 2020 2020  tats",.         
-00052480: 2020 2022 6365 6e74 726f 6964 222c 0a20     "centroid",. 
-00052490: 2020 2020 2020 2020 2020 2022 6365 6e74             "cent
-000524a0: 726f 6964 5f73 6c69 6365 222c 0a20 2020  roid_slice",.   
-000524b0: 2020 2020 2020 2020 2022 6365 6e74 726f           "centro
-000524c0: 6964 5f73 6c69 6365 5f73 7461 7473 222c  id_slice_stats",
-000524d0: 0a20 2020 2020 2020 2020 2020 2022 6469  .            "di
-000524e0: 6365 222c 0a20 2020 2020 2020 2020 2020  ce",.           
-000524f0: 2022 6469 6365 5f66 6c61 7422 2c0a 2020   "dice_flat",.  
-00052500: 2020 2020 2020 2020 2020 2264 6963 655f            "dice_
-00052510: 736c 6963 6522 2c0a 2020 2020 2020 2020  slice",.        
-00052520: 2020 2020 2264 6963 655f 736c 6963 655f      "dice_slice_
-00052530: 7374 6174 7322 2c0a 2020 2020 2020 2020  stats",.        
-00052540: 2020 2020 2268 6175 7364 6f72 6666 5f64      "hausdorff_d
-00052550: 6973 7461 6e63 6522 2c0a 2020 2020 2020  istance",.      
-00052560: 2020 2020 2020 2268 6175 7364 6f72 6666        "hausdorff
-00052570: 5f64 6973 7461 6e63 655f 666c 6174 222c  _distance_flat",
-00052580: 0a20 2020 2020 2020 2020 2020 2022 6a61  .            "ja
-00052590: 6363 6172 6422 2c0a 2020 2020 2020 2020  ccard",.        
-000525a0: 2020 2020 226a 6163 6361 7264 5f66 6c61      "jaccard_fla
+0004b0d0: 2020 2069 6620 6e6f 7420 6b65 7920 696e     if not key in
+0004b0e0: 2061 6c6c 5f70 6f6c 7967 6f6e 733a 0a20   all_polygons:. 
+0004b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004b100: 2020 2020 2020 2061 6c6c 5f70 6f6c 7967         all_polyg
+0004b110: 6f6e 735b 6b65 795d 203d 205b 5d0a 2020  ons[key] = [].  
+0004b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004b130: 2020 616c 6c5f 706f 6c79 676f 6e73 5b6b    all_polygons[k
+0004b140: 6579 5d2e 6578 7465 6e64 2870 6f6c 7967  ey].extend(polyg
+0004b150: 6f6e 7329 0a0a 2020 2020 2020 2020 2020  ons)..          
+0004b160: 2020 2320 4576 616c 7561 7465 2074 6865    # Evaluate the
+0004b170: 2075 6e61 7279 2075 6e69 6f6e 206f 6620   unary union of 
+0004b180: 706f 6c79 676f 6e73 2066 6f72 2065 6163  polygons for eac
+0004b190: 6820 736c 6963 652e 0a20 2020 2020 2020  h slice..       
+0004b1a0: 2020 2020 2061 6c6c 5f70 6f6c 7967 6f6e       all_polygon
+0004b1b0: 7320 3d20 7b6b 6579 3a20 5b6f 7073 2e75  s = {key: [ops.u
+0004b1c0: 6e61 7279 5f75 6e69 6f6e 2861 6c6c 5f70  nary_union(all_p
+0004b1d0: 6f6c 7967 6f6e 735b 6b65 795d 295d 0a20  olygons[key])]. 
+0004b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004b1f0: 2020 2020 666f 7220 6b65 7920 696e 2061      for key in a
+0004b200: 6c6c 5f70 6f6c 7967 6f6e 737d 0a0a 2020  ll_polygons}..  
+0004b210: 2020 2020 2020 2020 2020 2320 4372 6561            # Crea
+0004b220: 7465 2074 6865 2063 6f6d 706f 7369 7465  te the composite
+0004b230: 2052 4f49 2e0a 2020 2020 2020 2020 2020   ROI..          
+0004b240: 2020 726f 695f 6e65 7720 3d20 524f 4928    roi_new = ROI(
+0004b250: 736f 7572 6365 3d61 6c6c 5f70 6f6c 7967  source=all_polyg
+0004b260: 6f6e 732c 2069 6d61 6765 3d69 6d61 6765  ons, image=image
+0004b270: 2c20 6e61 6d65 3d6e 616d 6529 0a0a 2020  , name=name)..  
+0004b280: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0004b290: 2020 2020 2020 2020 2320 5573 6520 6461          # Use da
+0004b2a0: 7461 2066 726f 6d20 6f6e 6520 6f66 2074  ta from one of t
+0004b2b0: 6865 2052 4f49 7320 6173 2061 2073 7461  he ROIs as a sta
+0004b2c0: 7274 696e 6720 706f 696e 742e 0a20 2020  rting point..   
+0004b2d0: 2020 2020 2020 2020 2072 6f69 3020 3d20           roi0 = 
+0004b2e0: 7365 6c66 2e67 6574 5f72 6f69 2872 6f69  self.get_roi(roi
+0004b2f0: 5f6e 616d 6573 5b30 5d29 0a20 2020 2020  _names[0]).     
+0004b300: 2020 2020 2020 2072 6f69 5f6e 6577 203d         roi_new =
+0004b310: 2052 4f49 2873 6f75 7263 653d 726f 6930   ROI(source=roi0
+0004b320: 2e67 6574 5f6d 6173 6b28 292c 2061 6666  .get_mask(), aff
+0004b330: 696e 653d 726f 6930 2e61 6666 696e 652c  ine=roi0.affine,
+0004b340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0004b350: 2020 2020 206e 616d 653d 6e61 6d65 2c20       name=name, 
+0004b360: 696d 6167 653d 696d 6167 6529 0a0a 2020  image=image)..  
+0004b370: 2020 2020 2020 2020 2020 2320 436f 6d62            # Comb
+0004b380: 696e 6520 7769 7468 2064 6174 6120 6672  ine with data fr
+0004b390: 6f6d 2074 6865 206f 7468 6572 2052 4f49  om the other ROI
+0004b3a0: 732e 0a20 2020 2020 2020 2020 2020 2066  s..            f
+0004b3b0: 6f72 2069 2069 6e20 7261 6e67 6528 312c  or i in range(1,
+0004b3c0: 206c 656e 2872 6f69 5f6e 616d 6573 2929   len(roi_names))
+0004b3d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0004b3e0: 2020 726f 695f 6e65 772e 6d61 736b 2e64    roi_new.mask.d
+0004b3f0: 6174 6120 2b3d 2073 656c 662e 6765 745f  ata += self.get_
+0004b400: 726f 6928 726f 695f 6e61 6d65 735b 695d  roi(roi_names[i]
+0004b410: 292e 6765 745f 6d61 736b 2829 0a0a 2020  ).get_mask()..  
+0004b420: 2020 2020 2020 7265 7475 726e 2072 6f69        return roi
+0004b430: 5f6e 6577 0a0a 2020 2020 6465 6620 6765  _new..    def ge
+0004b440: 745f 6d61 736b 5f69 6d61 6765 2873 656c  t_mask_image(sel
+0004b450: 662c 206e 616d 653d 4e6f 6e65 293a 0a20  f, name=None):. 
+0004b460: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0004b470: 2020 2047 6574 2069 6d61 6765 206f 626a     Get image obj
+0004b480: 6563 7420 7265 7072 6573 656e 7469 6e67  ect representing
+0004b490: 206d 6173 6b20 666f 7220 616c 6c20 524f   mask for all RO
+0004b4a0: 4973 206f 6620 7374 7275 6374 7572 6520  Is of structure 
+0004b4b0: 7365 742e 0a0a 2020 2020 2020 2020 2a2a  set...        **
+0004b4c0: 5061 7261 6d65 7465 7273 3a2a 2a0a 0a20  Parameters:**.. 
+0004b4d0: 2020 2020 2020 206e 616d 6520 3a20 7374         name : st
+0004b4e0: 722c 2064 6566 6175 6c74 3d4e 6f6e 650a  r, default=None.
+0004b4f0: 2020 2020 2020 2020 2020 2020 4e61 6d65              Name
+0004b500: 2074 6f20 6265 2067 6976 656e 2074 6f20   to be given to 
+0004b510: 7468 6520 6d61 736b 2069 6d61 6765 2e20  the mask image. 
+0004b520: 2049 6620 4e6f 6e65 2c20 7468 650a 2020   If None, the.  
+0004b530: 2020 2020 2020 2020 2020 6e61 6d65 2061            name a
+0004b540: 7373 6967 6e65 6420 6973 2074 6865 206e  ssigned is the n
+0004b550: 616d 6520 6f66 2074 6865 2073 7472 7563  ame of the struc
+0004b560: 7475 7265 2073 6574 2c20 7769 7468 2073  ture set, with s
+0004b570: 7566 6669 780a 2020 2020 2020 2020 2020  uffix.          
+0004b580: 2020 225f 6d61 736b 2220 6170 7065 6e64    "_mask" append
+0004b590: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
+0004b5a0: 2020 2020 2020 2020 6e61 6d65 203d 206e          name = n
+0004b5b0: 616d 6520 6f72 2066 227b 7365 6c66 2e6e  ame or f"{self.n
+0004b5c0: 616d 657d 5f6d 6173 6b22 0a20 2020 2020  ame}_mask".     
+0004b5d0: 2020 2072 6f69 5f63 6f6d 6269 6e65 6420     roi_combined 
+0004b5e0: 3d20 7365 6c66 2e63 6f6d 6269 6e65 5f72  = self.combine_r
+0004b5f0: 6f69 7328 6e61 6d65 3d6e 616d 6529 0a20  ois(name=name). 
+0004b600: 2020 2020 2020 206d 6173 6b5f 696d 6167         mask_imag
+0004b610: 6520 3d20 726f 695f 636f 6d62 696e 6564  e = roi_combined
+0004b620: 2e67 6574 5f6d 6173 6b5f 696d 6167 6528  .get_mask_image(
+0004b630: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0004b640: 206d 6173 6b5f 696d 6167 650a 0a20 2020   mask_image..   
+0004b650: 2064 6566 2063 726f 7028 7365 6c66 2c20   def crop(self, 
+0004b660: 786c 696d 3d4e 6f6e 652c 2079 6c69 6d3d  xlim=None, ylim=
+0004b670: 4e6f 6e65 2c20 7a6c 696d 3d4e 6f6e 6529  None, zlim=None)
+0004b680: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0004b690: 2020 2020 2020 4372 6f70 2061 6c6c 2052        Crop all R
+0004b6a0: 4f49 7320 6f66 2053 7472 7563 7475 7265  OIs of Structure
+0004b6b0: 5365 7420 746f 2073 7065 6369 6669 6564  Set to specified
+0004b6c0: 2072 616e 6765 2069 6e20 782c 2079 2c20   range in x, y, 
+0004b6d0: 7a2e 0a0a 2020 2020 2020 2020 5468 6520  z...        The 
+0004b6e0: 7061 7261 6d65 7465 7273 2078 6c69 6d2c  parameters xlim,
+0004b6f0: 2079 6c69 6d2c 207a 6c69 6d20 6172 6520   ylim, zlim are 
+0004b700: 7061 7373 6564 2074 6f20 6561 6368 2052  passed to each R
+0004b710: 4f49 2773 2063 726f 7028 2920 6d65 7468  OI's crop() meth
+0004b720: 6f64 2e0a 2020 2020 2020 2020 466f 7220  od..        For 
+0004b730: 6578 706c 616e 6174 696f 6e20 6f66 2074  explanation of t
+0004b740: 6865 7365 2070 6172 616d 6574 6572 732c  hese parameters,
+0004b750: 2073 6565 2064 6f63 756d 656e 7461 7469   see documentati
+0004b760: 6f6e 2066 6f72 0a20 2020 2020 2020 2073  on for.        s
+0004b770: 6b72 742e 7374 7275 6374 7572 6573 2e52  krt.structures.R
+0004b780: 4f49 2e63 726f 7028 292e 0a20 2020 2020  OI.crop()..     
+0004b790: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+0004b7a0: 6f72 2072 6f69 2069 6e20 7365 6c66 2e67  or roi in self.g
+0004b7b0: 6574 5f72 6f69 7328 293a 0a20 2020 2020  et_rois():.     
+0004b7c0: 2020 2020 2020 2072 6f69 2e63 726f 7028         roi.crop(
+0004b7d0: 786c 696d 2c20 796c 696d 2c20 7a6c 696d  xlim, ylim, zlim
+0004b7e0: 290a 0a63 6c61 7373 2053 7472 7563 7475  )..class Structu
+0004b7f0: 7265 5365 7449 7465 7261 746f 723a 0a0a  reSetIterator:..
+0004b800: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0004b810: 2873 656c 662c 2073 7472 7563 7475 7265  (self, structure
+0004b820: 5f73 6574 293a 0a20 2020 2020 2020 2073  _set):.        s
+0004b830: 656c 662e 6964 7820 3d20 2d31 0a20 2020  elf.idx = -1.   
+0004b840: 2020 2020 2073 656c 662e 7374 7275 6374       self.struct
+0004b850: 7572 655f 7365 7420 3d20 7374 7275 6374  ure_set = struct
+0004b860: 7572 655f 7365 740a 0a20 2020 2064 6566  ure_set..    def
+0004b870: 205f 5f6e 6578 745f 5f28 7365 6c66 293a   __next__(self):
+0004b880: 0a20 2020 2020 2020 2073 656c 662e 6964  .        self.id
+0004b890: 7820 2b3d 2031 0a20 2020 2020 2020 2069  x += 1.        i
+0004b8a0: 6620 7365 6c66 2e69 6478 203c 206c 656e  f self.idx < len
+0004b8b0: 2873 656c 662e 7374 7275 6374 7572 655f  (self.structure_
+0004b8c0: 7365 742e 6765 745f 726f 6973 2829 293a  set.get_rois()):
+0004b8d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0004b8e0: 7572 6e20 7365 6c66 2e73 7472 7563 7475  urn self.structu
+0004b8f0: 7265 5f73 6574 2e67 6574 5f72 6f69 7328  re_set.get_rois(
+0004b900: 295b 7365 6c66 2e69 6478 5d0a 2020 2020  )[self.idx].    
+0004b910: 2020 2020 7261 6973 6520 5374 6f70 4974      raise StopIt
+0004b920: 6572 6174 696f 6e0a 0a0a 6465 6620 6c6f  eration...def lo
+0004b930: 6164 5f72 6f69 735f 6469 636f 6d28 7061  ad_rois_dicom(pa
+0004b940: 7468 2c20 6e61 6d65 733d 4e6f 6e65 293a  th, names=None):
+0004b950: 0a20 2020 2022 2222 4c6f 6164 2052 4f49  .    """Load ROI
+0004b960: 2873 2920 6672 6f6d 2061 2064 6963 6f6d  (s) from a dicom
+0004b970: 2073 7472 7563 7475 7265 2073 6574 2066   structure set f
+0004b980: 696c 652e 203c 6e61 6d65 3e20 6361 6e20  ile. <name> can 
+0004b990: 6265 2061 2073 696e 676c 650a 2020 2020  be a single.    
+0004b9a0: 6e61 6d65 206f 7220 6c69 7374 206f 6620  name or list of 
+0004b9b0: 6e61 6d65 7320 6f66 2052 4f49 7320 746f  names of ROIs to
+0004b9c0: 206c 6f61 642e 2222 220a 0a20 2020 2023   load."""..    #
+0004b9d0: 204c 6f61 6420 6469 636f 6d20 6f62 6a65   Load dicom obje
+0004b9e0: 6374 0a20 2020 2074 7279 3a0a 2020 2020  ct.    try:.    
+0004b9f0: 2020 2020 6473 203d 2070 7964 6963 6f6d      ds = pydicom
+0004ba00: 2e64 636d 7265 6164 2870 6174 682c 2066  .dcmread(path, f
+0004ba10: 6f72 6365 3d54 7275 6529 0a20 2020 2065  orce=True).    e
+0004ba20: 7863 6570 7420 7079 6469 636f 6d2e 6572  xcept pydicom.er
+0004ba30: 726f 7273 2e49 6e76 616c 6964 4469 636f  rors.InvalidDico
+0004ba40: 6d45 7272 6f72 3a0a 2020 2020 2020 2020  mError:.        
+0004ba50: 7265 7475 726e 205b 5d2c 204e 6f6e 650a  return [], None.
+0004ba60: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
+0004ba70: 7472 2864 732c 2022 534f 5043 6c61 7373  tr(ds, "SOPClass
+0004ba80: 5549 4422 293a 0a20 2020 2020 2020 2072  UID"):.        r
+0004ba90: 6574 7572 6e20 5b5d 2c20 4e6f 6e65 0a20  eturn [], None. 
+0004baa0: 2020 2069 6620 6e6f 7420 2864 732e 534f     if not (ds.SO
+0004bab0: 5043 6c61 7373 5549 4420 3d3d 2022 312e  PClassUID == "1.
+0004bac0: 322e 3834 302e 3130 3030 382e 352e 312e  2.840.10008.5.1.
+0004bad0: 342e 312e 312e 3438 312e 3322 293a 0a20  4.1.1.481.3"):. 
+0004bae0: 2020 2020 2020 2070 7269 6e74 2866 2257         print(f"W
+0004baf0: 6172 6e69 6e67 3a20 7b70 6174 687d 2069  arning: {path} i
+0004bb00: 7320 6e6f 7420 6120 4449 434f 4d20 7374  s not a DICOM st
+0004bb10: 7275 6374 7572 6520 7365 7420 6669 6c65  ructure set file
+0004bb20: 2122 290a 2020 2020 2020 2020 7265 7475  !").        retu
+0004bb30: 726e 205b 5d2c 204e 6f6e 650a 0a20 2020  rn [], None..   
+0004bb40: 2023 2047 6574 2052 4f49 206e 616d 6573   # Get ROI names
+0004bb50: 0a20 2020 2073 6571 203d 2067 6574 5f64  .    seq = get_d
+0004bb60: 6963 6f6d 5f73 6571 7565 6e63 6528 6473  icom_sequence(ds
+0004bb70: 2c20 2253 7472 7563 7475 7265 5365 7452  , "StructureSetR
+0004bb80: 4f49 2229 0a20 2020 2072 6f69 7320 3d20  OI").    rois = 
+0004bb90: 7b7d 0a20 2020 2066 6f72 2072 6f69 2069  {}.    for roi i
+0004bba0: 6e20 7365 713a 0a20 2020 2020 2020 2072  n seq:.        r
+0004bbb0: 6f69 735b 696e 7428 726f 692e 524f 494e  ois[int(roi.ROIN
+0004bbc0: 756d 6265 7229 5d20 3d20 7b22 6e61 6d65  umber)] = {"name
+0004bbd0: 223a 2072 6f69 2e52 4f49 4e61 6d65 7d0a  ": roi.ROIName}.
+0004bbe0: 0a20 2020 2023 2046 696e 6420 524f 4973  .    # Find ROIs
+0004bbf0: 206d 6174 6368 696e 6720 7265 7175 6573   matching reques
+0004bc00: 7465 6420 6e61 6d65 730a 2020 2020 6e61  ted names.    na
+0004bc10: 6d65 735f 746f 5f6c 6f61 6420 3d20 4e6f  mes_to_load = No
+0004bc20: 6e65 0a20 2020 2069 6620 6973 696e 7374  ne.    if isinst
+0004bc30: 616e 6365 286e 616d 6573 2c20 7374 7229  ance(names, str)
+0004bc40: 3a0a 2020 2020 2020 2020 6e61 6d65 735f  :.        names_
+0004bc50: 746f 5f6c 6f61 6420 3d20 5b6e 616d 6573  to_load = [names
+0004bc60: 5d0a 2020 2020 656c 6966 2073 6b72 742e  ].    elif skrt.
+0004bc70: 636f 7265 2e69 735f 6c69 7374 286e 616d  core.is_list(nam
+0004bc80: 6573 293a 0a20 2020 2020 2020 206e 616d  es):.        nam
+0004bc90: 6573 5f74 6f5f 6c6f 6164 203d 206e 616d  es_to_load = nam
+0004bca0: 6573 0a20 2020 2069 6620 6e61 6d65 735f  es.    if names_
+0004bcb0: 746f 5f6c 6f61 643a 0a20 2020 2020 2020  to_load:.       
+0004bcc0: 2072 6f69 7320 3d20 7b0a 2020 2020 2020   rois = {.      
+0004bcd0: 2020 2020 2020 693a 2073 0a20 2020 2020        i: s.     
+0004bce0: 2020 2020 2020 2066 6f72 2069 2c20 7320         for i, s 
+0004bcf0: 696e 2072 6f69 732e 6974 656d 7328 290a  in rois.items().
+0004bd00: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0004bd10: 6e79 280a 2020 2020 2020 2020 2020 2020  ny(.            
+0004bd20: 2020 2020 5b66 6e6d 6174 6368 2e66 6e6d      [fnmatch.fnm
+0004bd30: 6174 6368 2873 5b22 6e61 6d65 225d 2e6c  atch(s["name"].l
+0004bd40: 6f77 6572 2829 2c20 6e2e 6c6f 7765 7228  ower(), n.lower(
+0004bd50: 2929 2066 6f72 206e 2069 6e20 6e61 6d65  )) for n in name
+0004bd60: 735f 746f 5f6c 6f61 645d 0a20 2020 2020  s_to_load].     
+0004bd70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0004bd80: 207d 0a20 2020 2020 2020 2069 6620 6e6f   }.        if no
+0004bd90: 7420 6c65 6e28 726f 6973 293a 0a20 2020  t len(rois):.   
+0004bda0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+0004bdb0: 2257 6172 6e69 6e67 3a20 6e6f 2052 4f49  "Warning: no ROI
+0004bdc0: 7320 666f 756e 6420 6d61 7463 6869 6e67  s found matching
+0004bdd0: 206e 616d 6528 7329 3a20 7b6e 616d 6573   name(s): {names
+0004bde0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+0004bdf0: 7265 7475 726e 205b 5d2c 204e 6f6e 650a  return [], None.
+0004be00: 0a20 2020 2023 2047 6574 2052 4f49 2064  .    # Get ROI d
+0004be10: 6574 6169 6c73 0a20 2020 2072 6f69 5f73  etails.    roi_s
+0004be20: 6571 203d 2067 6574 5f64 6963 6f6d 5f73  eq = get_dicom_s
+0004be30: 6571 7565 6e63 6528 6473 2c20 2252 4f49  equence(ds, "ROI
+0004be40: 436f 6e74 6f75 7222 290a 2020 2020 666f  Contour").    fo
+0004be50: 7220 726f 6920 696e 2072 6f69 5f73 6571  r roi in roi_seq
+0004be60: 3a0a 0a20 2020 2020 2020 206e 756d 6265  :..        numbe
+0004be70: 7220 3d20 726f 692e 5265 6665 7265 6e63  r = roi.Referenc
+0004be80: 6564 524f 494e 756d 6265 720a 2020 2020  edROINumber.    
+0004be90: 2020 2020 6966 206e 756d 6265 7220 6e6f      if number no
+0004bea0: 7420 696e 2072 6f69 733a 0a20 2020 2020  t in rois:.     
+0004beb0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0004bec0: 2020 2020 2020 2020 6461 7461 203d 207b          data = {
+0004bed0: 2263 6f6e 746f 7572 7322 3a20 7b7d 7d0a  "contours": {}}.
+0004bee0: 0a20 2020 2020 2020 2023 2047 6574 2052  .        # Get R
+0004bef0: 4f49 2063 6f6c 6f75 720a 2020 2020 2020  OI colour.      
+0004bf00: 2020 6966 2022 524f 4944 6973 706c 6179    if "ROIDisplay
+0004bf10: 436f 6c6f 7222 2069 6e20 726f 693a 0a20  Color" in roi:. 
+0004bf20: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0004bf30: 2263 6f6c 6f72 225d 203d 205b 696e 7428  "color"] = [int(
+0004bf40: 6329 202f 2032 3535 2066 6f72 2063 2069  c) / 255 for c i
+0004bf50: 6e20 6c69 7374 2872 6f69 2e52 4f49 4469  n list(roi.ROIDi
+0004bf60: 7370 6c61 7943 6f6c 6f72 295d 0a20 2020  splayColor)].   
+0004bf70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0004bf80: 2020 2020 2020 2064 6174 615b 2263 6f6c         data["col
+0004bf90: 6f72 225d 203d 204e 6f6e 650a 0a20 2020  or"] = None..   
+0004bfa0: 2020 2020 2023 2047 6574 2063 6f6e 746f       # Get conto
+0004bfb0: 7572 730a 2020 2020 2020 2020 636f 6e74  urs.        cont
+0004bfc0: 6f75 725f 7365 7120 3d20 6765 745f 6469  our_seq = get_di
+0004bfd0: 636f 6d5f 7365 7175 656e 6365 2872 6f69  com_sequence(roi
+0004bfe0: 2c20 2243 6f6e 746f 7572 2229 0a20 2020  , "Contour").   
+0004bff0: 2020 2020 2069 6620 636f 6e74 6f75 725f       if contour_
+0004c000: 7365 713a 0a20 2020 2020 2020 2020 2020  seq:.           
+0004c010: 2066 6f72 2063 2069 6e20 636f 6e74 6f75   for c in contou
+0004c020: 725f 7365 713a 0a20 2020 2020 2020 2020  r_seq:.         
+0004c030: 2020 2020 2020 2070 6c61 6e65 5f64 6174         plane_dat
+0004c040: 6120 3d20 5b0a 2020 2020 2020 2020 2020  a = [.          
+0004c050: 2020 2020 2020 2020 2020 5b66 6c6f 6174            [float
+0004c060: 2870 2920 666f 7220 7020 696e 2063 2e43  (p) for p in c.C
+0004c070: 6f6e 746f 7572 4461 7461 5b69 202a 2033  ontourData[i * 3
+0004c080: 203a 2069 202a 2033 202b 2033 5d5d 0a20   : i * 3 + 3]]. 
+0004c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004c0a0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0004c0b0: 6528 632e 4e75 6d62 6572 4f66 436f 6e74  e(c.NumberOfCont
+0004c0c0: 6f75 7250 6f69 6e74 7329 0a20 2020 2020  ourPoints).     
+0004c0d0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+0004c0e0: 2020 2020 2020 2020 2020 2020 207a 203d               z =
+0004c0f0: 2066 6c6f 6174 2863 2e43 6f6e 746f 7572   float(c.Contour
+0004c100: 4461 7461 5b32 5d29 0a20 2020 2020 2020  Data[2]).       
+0004c110: 2020 2020 2020 2020 2069 6620 7a20 6e6f           if z no
+0004c120: 7420 696e 2064 6174 615b 2263 6f6e 746f  t in data["conto
+0004c130: 7572 7322 5d3a 0a20 2020 2020 2020 2020  urs"]:.         
+0004c140: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0004c150: 2263 6f6e 746f 7572 7322 5d5b 7a5d 203d  "contours"][z] =
+0004c160: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+0004c170: 2020 2020 6461 7461 5b22 636f 6e74 6f75      data["contou
+0004c180: 7273 225d 5b7a 5d2e 6170 7065 6e64 286e  rs"][z].append(n
+0004c190: 702e 6172 7261 7928 706c 616e 655f 6461  p.array(plane_da
+0004c1a0: 7461 2929 0a0a 2020 2020 2020 2020 726f  ta))..        ro
+0004c1b0: 6973 5b6e 756d 6265 725d 2e75 7064 6174  is[number].updat
+0004c1c0: 6528 6461 7461 290a 0a20 2020 2072 6574  e(data)..    ret
+0004c1d0: 7572 6e20 726f 6973 2c20 6473 0a0a 0a64  urn rois, ds...d
+0004c1e0: 6566 2067 6574 5f64 6963 6f6d 5f73 6571  ef get_dicom_seq
+0004c1f0: 7565 6e63 6528 6473 3d4e 6f6e 652c 2062  uence(ds=None, b
+0004c200: 6173 656e 616d 653d 2222 293a 0a0a 2020  asename=""):..  
+0004c210: 2020 7365 7175 656e 6365 203d 205b 5d0a    sequence = [].
+0004c220: 2020 2020 666f 7220 7375 6666 6978 2069      for suffix i
+0004c230: 6e20 5b22 5365 7175 656e 6365 222c 2022  n ["Sequence", "
+0004c240: 7322 5d3a 0a20 2020 2020 2020 2061 7474  s"]:.        att
+0004c250: 7269 6275 7465 203d 2066 227b 6261 7365  ribute = f"{base
+0004c260: 6e61 6d65 7d7b 7375 6666 6978 7d22 0a20  name}{suffix}". 
+0004c270: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+0004c280: 7228 6473 2c20 6174 7472 6962 7574 6529  r(ds, attribute)
+0004c290: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0004c2a0: 7175 656e 6365 203d 2067 6574 6174 7472  quence = getattr
+0004c2b0: 2864 732c 2061 7474 7269 6275 7465 290a  (ds, attribute).
+0004c2c0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+0004c2d0: 6b0a 2020 2020 7265 7475 726e 2073 6571  k.    return seq
+0004c2e0: 7565 6e63 650a 0a64 6566 2063 6f6e 746f  uence..def conto
+0004c2f0: 7572 5f74 6f5f 706f 6c79 676f 6e28 636f  ur_to_polygon(co
+0004c300: 6e74 6f75 7229 3a0a 2020 2020 2222 2243  ntour):.    """C
+0004c310: 6f6e 7665 7274 2061 206c 6973 7420 6f66  onvert a list of
+0004c320: 2063 6f6e 746f 7572 2070 6f69 6e74 7320   contour points 
+0004c330: 746f 2061 2053 6861 7065 6c79 2070 6f6c  to a Shapely pol
+0004c340: 7967 6f6e 2c20 656e 7375 7269 6e67 2074  ygon, ensuring t
+0004c350: 6861 7420 0a20 2020 2074 6865 2070 6f6c  hat .    the pol
+0004c360: 7967 6f6e 2069 7320 7661 6c69 642e 2222  ygon is valid.""
+0004c370: 220a 0a20 2020 2070 6f6c 7967 6f6e 203d  "..    polygon =
+0004c380: 2067 656f 6d65 7472 792e 506f 6c79 676f   geometry.Polygo
+0004c390: 6e28 636f 6e74 6f75 7229 0a0a 2020 2020  n(contour)..    
+0004c3a0: 6465 6c74 6120 3d20 302e 3030 350a 2020  delta = 0.005.  
+0004c3b0: 2020 6966 206e 6f74 2070 6f6c 7967 6f6e    if not polygon
+0004c3c0: 2e69 735f 7661 6c69 643a 0a20 2020 2020  .is_valid:.     
+0004c3d0: 2020 2074 6d70 203d 2067 656f 6d65 7472     tmp = geometr
+0004c3e0: 792e 506f 6c79 676f 6e28 706f 6c79 676f  y.Polygon(polygo
+0004c3f0: 6e29 0a20 2020 2020 2020 2062 7566 6665  n).        buffe
+0004c400: 7220 3d20 302e 0a20 2020 2020 2020 2023  r = 0..        #
+0004c410: 2054 6865 2069 6465 6120 6865 7265 2069   The idea here i
+0004c420: 7320 746f 2069 6e63 7265 6173 6520 7468  s to increase th
+0004c430: 6520 6275 6666 6572 2064 6973 7461 6e63  e buffer distanc
+0004c440: 6520 756e 7469 6c0a 2020 2020 2020 2020  e until.        
+0004c450: 2320 6120 7661 6c69 6420 706f 6c79 676f  # a valid polygo
+0004c460: 6e20 6973 206f 6274 6169 6e65 642e 2020  n is obtained.  
+0004c470: 5468 6973 2067 656e 6572 616c 6c79 2073  This generally s
+0004c480: 6565 6d73 2074 6f20 776f 726b 2e2e 2e0a  eems to work....
+0004c490: 2020 2020 2020 2020 7768 696c 6520 2869          while (i
+0004c4a0: 7369 6e73 7461 6e63 6528 706f 6c79 676f  sinstance(polygo
+0004c4b0: 6e2c 2067 656f 6d65 7472 792e 4d75 6c74  n, geometry.Mult
+0004c4c0: 6950 6f6c 7967 6f6e 290a 2020 2020 2020  iPolygon).      
+0004c4d0: 2020 2020 2020 2020 2020 6f72 206e 6f74            or not
+0004c4e0: 2070 6f6c 7967 6f6e 2e69 735f 7661 6c69   polygon.is_vali
+0004c4f0: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
+0004c500: 6275 6666 6572 202b 3d20 6465 6c74 610a  buffer += delta.
+0004c510: 2020 2020 2020 2020 2020 2020 706f 6c79              poly
+0004c520: 676f 6e20 3d20 746d 702e 6275 6666 6572  gon = tmp.buffer
+0004c530: 2862 7566 6665 7229 0a20 2020 2020 2020  (buffer).       
+0004c540: 2070 6f69 6e74 7320 3d20 5b5d 0a20 2020   points = [].   
+0004c550: 2020 2020 2066 6f72 2078 2c20 7920 696e       for x, y in
+0004c560: 2070 6f6c 7967 6f6e 2e65 7874 6572 696f   polygon.exterio
+0004c570: 722e 636f 6f72 6473 3a0a 2020 2020 2020  r.coords:.      
+0004c580: 2020 2020 2020 706f 696e 7473 2e61 7070        points.app
+0004c590: 656e 6428 2878 2c20 7929 290a 2020 2020  end((x, y)).    
+0004c5a0: 2020 2020 706f 6c79 676f 6e20 3d20 6765      polygon = ge
+0004c5b0: 6f6d 6574 7279 2e50 6f6c 7967 6f6e 2870  ometry.Polygon(p
+0004c5c0: 6f69 6e74 7329 0a0a 2020 2020 7265 7475  oints)..    retu
+0004c5d0: 726e 2070 6f6c 7967 6f6e 0a0a 6465 6620  rn polygon..def 
+0004c5e0: 706f 6c79 676f 6e5f 746f 5f63 6f6e 746f  polygon_to_conto
+0004c5f0: 7572 2870 6f6c 7967 6f6e 293a 0a20 2020  ur(polygon):.   
+0004c600: 2027 2727 0a20 2020 2043 6f6e 7665 7274   '''.    Convert
+0004c610: 2061 2053 6861 7065 6c79 2070 6f6c 7967   a Shapely polyg
+0004c620: 6f6e 2074 6f20 6120 6c69 7374 206f 6620  on to a list of 
+0004c630: 636f 6e74 6f75 7220 706f 696e 7473 2e0a  contour points..
+0004c640: 0a20 2020 202a 2a50 6172 616d 6574 6572  .    **Parameter
+0004c650: 3a2a 2a0a 0a20 2020 2070 6f6c 7967 6f6e  :**..    polygon
+0004c660: 3a20 7368 6170 656c 792e 6765 6f6d 6574  : shapely.geomet
+0004c670: 7279 2e70 6f6c 7967 6f6e 0a20 2020 2020  ry.polygon.     
+0004c680: 2020 2053 6861 7065 6c79 2070 6f6c 7967     Shapely polyg
+0004c690: 6f6e 2e0a 0a20 2020 207a 5f70 6f6c 7967  on...    z_polyg
+0004c6a0: 6f6e 3a20 7a20 636f 6f72 6469 6e61 7465  on: z coordinate
+0004c6b0: 2061 7420 7768 6963 6820 706f 6c79 676f   at which polygo
+0004c6c0: 6e20 6973 2064 6566 696e 6564 2e0a 2020  n is defined..  
+0004c6d0: 2020 2727 270a 2020 2020 636f 6e74 6f75    '''.    contou
+0004c6e0: 725f 706f 696e 7473 203d 205b 5d0a 2020  r_points = [].  
+0004c6f0: 2020 666f 7220 782c 2079 2069 6e20 6c69    for x, y in li
+0004c700: 7374 2870 6f6c 7967 6f6e 2e65 7874 6572  st(polygon.exter
+0004c710: 696f 722e 636f 6f72 6473 293a 0a20 2020  ior.coords):.   
+0004c720: 2020 2020 2063 6f6e 746f 7572 5f70 6f69       contour_poi
+0004c730: 6e74 732e 6170 7065 6e64 285b 782c 2079  nts.append([x, y
+0004c740: 5d29 0a20 2020 2063 6f6e 746f 7572 203d  ]).    contour =
+0004c750: 206e 702e 6172 7261 7928 636f 6e74 6f75   np.array(contou
+0004c760: 725f 706f 696e 7473 290a 0a20 2020 2072  r_points)..    r
+0004c770: 6574 7572 6e20 636f 6e74 6f75 720a 0a64  eturn contour..d
+0004c780: 6566 2069 6e74 6572 706f 6c61 7465 5f70  ef interpolate_p
+0004c790: 6f69 6e74 735f 7369 6e67 6c65 5f63 6f6e  oints_single_con
+0004c7a0: 746f 7572 2873 6f75 7263 653d 4e6f 6e65  tour(source=None
+0004c7b0: 2c20 6e5f 706f 696e 743d 4e6f 6e65 2c20  , n_point=None, 
+0004c7c0: 6478 793d 4e6f 6e65 2c0a 2020 2020 2020  dxy=None,.      
+0004c7d0: 2020 736d 6f6f 7468 6e65 7373 5f70 6572    smoothness_per
+0004c7e0: 5f70 6f69 6e74 3d30 293a 0a20 2020 2027  _point=0):.    '
+0004c7f0: 2727 0a20 2020 2049 6e74 6572 706f 6c61  ''.    Interpola
+0004c800: 7465 2070 6f69 6e74 7320 666f 7220 6120  te points for a 
+0004c810: 7369 6e67 6c65 2063 6f6e 746f 7572 2e0a  single contour..
+0004c820: 0a20 2020 202a 2a50 6172 616d 6574 6572  .    **Parameter
+0004c830: 733a 2a2a 0a0a 2020 2020 736f 7572 6365  s:**..    source
+0004c840: 203a 2073 6861 7065 6c79 2e70 6f6c 7967   : shapely.polyg
+0004c850: 6f6e 2e50 6f6c 7967 6f6e 2f6e 702e 6e64  on.Polygon/np.nd
+0004c860: 6172 7261 792f 6c69 7374 2c20 6465 6661  array/list, defa
+0004c870: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
+0004c880: 2043 6f6e 746f 7572 2072 6570 7265 7365   Contour represe
+0004c890: 6e74 6174 696f 6e20 6173 2065 6974 6865  ntation as eithe
+0004c8a0: 7220 6120 7368 6170 656c 7920 506f 6c79  r a shapely Poly
+0004c8b0: 676f 6e2c 2061 206e 756d 7079 0a20 2020  gon, a numpy.   
+0004c8c0: 2020 2020 2061 7272 6179 206f 6620 5b78       array of [x
+0004c8d0: 2c20 795d 2070 6169 7273 206f 7220 6120  , y] pairs or a 
+0004c8e0: 6c69 7374 206f 6620 5b78 2c20 795d 2070  list of [x, y] p
+0004c8f0: 6169 7273 2e20 2054 6865 0a20 2020 2020  airs.  The.     
+0004c900: 2020 2072 6574 7572 6e65 6420 636f 6e74     returned cont
+0004c910: 6f75 7220 6861 7320 7468 6520 7361 6d65  our has the same
+0004c920: 2072 6570 7265 7365 6e74 6174 696f 6e2e   representation.
+0004c930: 0a0a 2020 2020 6e5f 706f 696e 7420 3a20  ..    n_point : 
+0004c940: 696e 742c 2064 6566 6175 6c74 3d4e 6f6e  int, default=Non
+0004c950: 650a 2020 2020 2020 2020 4e75 6d62 6572  e.        Number
+0004c960: 206f 6620 706f 696e 7473 2074 6f20 6465   of points to de
+0004c970: 6669 6e65 2063 6f6e 746f 7572 2c20 6166  fine contour, af
+0004c980: 7465 7220 696e 7465 7270 6f6c 6174 696f  ter interpolatio
+0004c990: 6e2e 2020 5468 6973 206d 7573 740a 2020  n.  This must.  
+0004c9a0: 2020 2020 2020 6265 2073 6574 2074 6f20        be set to 
+0004c9b0: 4e6f 6e65 2066 6f72 2064 7879 2074 6f20  None for dxy to 
+0004c9c0: 6265 2063 6f6e 7369 6465 7265 642e 0a0a  be considered...
+0004c9d0: 2020 2020 6478 7920 3a20 666c 6f61 742c      dxy : float,
+0004c9e0: 2064 6566 6175 6c74 3d4e 6f6e 650a 2020   default=None.  
+0004c9f0: 2020 2020 2020 4170 7072 6f78 696d 6174        Approximat
+0004ca00: 6520 6469 7374 616e 6365 2072 6571 7569  e distance requi
+0004ca10: 7265 6420 6265 7477 6565 6e20 636f 6e74  red between cont
+0004ca20: 6f75 7220 706f 696e 7473 2e20 2054 6869  our points.  Thi
+0004ca30: 7320 6973 2074 616b 656e 0a20 2020 2020  s is taken.     
+0004ca40: 2020 2069 6e74 6f20 6163 636f 756e 7420     into account 
+0004ca50: 6f6e 6c79 2069 6620 6e5f 706f 696e 7420  only if n_point 
+0004ca60: 6973 2073 6574 2074 6f20 4e6f 6e65 2e20  is set to None. 
+0004ca70: 2046 6f72 2061 2063 6f6e 746f 7572 206f   For a contour o
+0004ca80: 660a 2020 2020 2020 2020 6c65 6e67 7468  f.        length
+0004ca90: 2063 6f6e 746f 7572 5f6c 656e 6774 682c   contour_length,
+0004caa0: 2074 6865 206e 756d 6265 7220 6f66 2063   the number of c
+0004cab0: 6f6e 746f 7572 2070 6f69 6e74 7320 6973  ontour points is
+0004cac0: 2074 6865 6e20 7461 6b65 6e0a 2020 2020   then taken.    
+0004cad0: 2020 2020 746f 2062 6520 6d61 7828 696e      to be max(in
+0004cae0: 7428 636f 6e74 6f75 725f 6c65 6e67 7468  t(contour_length
+0004caf0: 202f 2064 7879 292c 2033 292e 2020 0a0a   / dxy), 3).  ..
+0004cb00: 2020 2020 736d 6f6f 7468 6e65 7373 5f70      smoothness_p
+0004cb10: 6572 5f70 6f69 6e74 203a 2066 6c6f 6174  er_point : float
+0004cb20: 2c20 6465 6661 756c 743d 300a 2020 2020  , default=0.    
+0004cb30: 2020 2020 5061 7261 6d65 7465 7220 6465      Parameter de
+0004cb40: 7465 726d 696e 696e 6720 7468 6520 736d  termining the sm
+0004cb50: 6f6f 7468 6e65 7373 206f 6620 7468 6520  oothness of the 
+0004cb60: 422d 7370 6c69 6e65 2063 7572 7665 2075  B-spline curve u
+0004cb70: 7365 640a 2020 2020 2020 2020 696e 2063  sed.        in c
+0004cb80: 6f6e 746f 7572 2061 7070 726f 7869 6d61  ontour approxima
+0004cb90: 7469 6f6e 2066 6f72 2069 6e74 6572 706f  tion for interpo
+0004cba0: 6c61 7469 6f6e 2e20 2054 6865 2070 726f  lation.  The pro
+0004cbb0: 6475 6374 206f 660a 2020 2020 2020 2020  duct of.        
+0004cbc0: 736d 6f6f 7468 6e65 7373 5f70 6572 5f70  smoothness_per_p
+0004cbd0: 6f69 6e74 2061 6e64 2074 6865 206e 756d  oint and the num
+0004cbe0: 6265 7220 6f66 2063 6f6e 746f 7572 2070  ber of contour p
+0004cbf0: 6f69 6e74 7320 2873 7065 6369 6669 6564  oints (specified
+0004cc00: 0a20 2020 2020 2020 2064 6972 6563 746c  .        directl
+0004cc10: 7920 7669 6120 6e5f 706f 696e 742c 206f  y via n_point, o
+0004cc20: 7220 696e 6469 7265 6374 6c79 2076 6961  r indirectly via
+0004cc30: 2064 7879 2920 636f 7272 6573 706f 6e64   dxy) correspond
+0004cc40: 7320 746f 2074 6865 0a20 2020 2020 2020  s to the.       
+0004cc50: 2070 6172 616d 6574 6572 2073 206f 6620   parameter s of 
+0004cc60: 7363 6970 792e 696e 7465 7270 6f6c 6174  scipy.interpolat
+0004cc70: 652e 7370 6c70 7265 7020 2d20 7365 6520  e.splprep - see 
+0004cc80: 646f 6375 6d65 6e74 6174 696f 6e20 6174  documentation at
+0004cc90: 3a0a 2020 2020 2020 2020 0a20 2020 2020  :.        .     
+0004cca0: 2020 2068 7474 7073 3a2f 2f73 6369 7079     https://scipy
+0004ccb0: 2e67 6974 6875 622e 696f 2f64 6576 646f  .github.io/devdo
+0004ccc0: 6373 2f72 6566 6572 656e 6365 2f67 656e  cs/reference/gen
+0004ccd0: 6572 6174 6564 2f73 6369 7079 2e69 6e74  erated/scipy.int
+0004cce0: 6572 706f 6c61 7465 2e73 706c 7072 6570  erpolate.splprep
+0004ccf0: 2e68 746d 6c23 7363 6970 792e 696e 7465  .html#scipy.inte
+0004cd00: 7270 6f6c 6174 652e 7370 6c70 7265 700a  rpolate.splprep.
+0004cd10: 0a20 2020 2020 2020 2041 2073 6d6f 6f74  .        A smoot
+0004cd20: 686e 6573 735f 7065 725f 706f 696e 7420  hness_per_point 
+0004cd30: 6f66 2030 2066 6f72 6365 7320 7468 6520  of 0 forces the 
+0004cd40: 422d 7370 6c69 6e65 2074 6f20 7061 7373  B-spline to pass
+0004cd50: 2074 6872 6f75 6768 0a20 2020 2020 2020   through.       
+0004cd60: 2061 6c6c 206f 6620 7468 6520 7072 652d   all of the pre-
+0004cd70: 696e 7465 7270 6f6c 6174 696f 6e20 636f  interpolation co
+0004cd80: 6e74 6f75 7220 706f 696e 7473 2e0a 2020  ntour points..  
+0004cd90: 2020 2727 270a 0a20 2020 2023 2045 7874    '''..    # Ext
+0004cda0: 7261 6374 206c 6973 7420 6f66 2063 6f6e  ract list of con
+0004cdb0: 746f 7572 2070 6f69 6e74 7320 6672 6f6d  tour points from
+0004cdc0: 2073 6f75 7263 652e 0a20 2020 2063 6f6e   source..    con
+0004cdd0: 746f 7572 5f6c 656e 6774 6820 3d20 4e6f  tour_length = No
+0004cde0: 6e65 0a20 2020 2069 6620 6973 696e 7374  ne.    if isinst
+0004cdf0: 616e 6365 2873 6f75 7263 652c 2067 656f  ance(source, geo
+0004ce00: 6d65 7472 792e 706f 6c79 676f 6e2e 506f  metry.polygon.Po
+0004ce10: 6c79 676f 6e29 3a0a 2020 2020 2020 2020  lygon):.        
+0004ce20: 706f 696e 7473 203d 206c 6973 7428 706f  points = list(po
+0004ce30: 6c79 676f 6e5f 746f 5f63 6f6e 746f 7572  lygon_to_contour
+0004ce40: 2873 6f75 7263 6529 290a 2020 2020 2020  (source)).      
+0004ce50: 2020 636f 6e74 6f75 725f 6c65 6e67 7468    contour_length
+0004ce60: 203d 2073 6f75 7263 652e 6c65 6e67 7468   = source.length
+0004ce70: 0a20 2020 2065 6c69 6620 6973 696e 7374  .    elif isinst
+0004ce80: 616e 6365 2873 6f75 7263 652c 206e 702e  ance(source, np.
+0004ce90: 6e64 6172 7261 7929 206f 7220 6973 696e  ndarray) or isin
+0004cea0: 7374 616e 6365 2873 6f75 7263 652c 206c  stance(source, l
+0004ceb0: 6973 7429 3a0a 2020 2020 2020 2020 706f  ist):.        po
+0004cec0: 696e 7473 203d 206c 6973 7428 736f 7572  ints = list(sour
+0004ced0: 6365 290a 2020 2020 656c 7365 3a0a 2020  ce).    else:.  
+0004cee0: 2020 2020 2020 706f 696e 7473 203d 204e        points = N
+0004cef0: 6f6e 650a 0a20 2020 2069 6620 706f 696e  one..    if poin
+0004cf00: 7473 2069 7320 4e6f 6e65 3a0a 2020 2020  ts is None:.    
+0004cf10: 2020 2020 7072 696e 7428 2755 6e72 6563      print('Unrec
+0004cf20: 6f67 6e69 7365 6420 736f 7572 6365 2070  ognised source p
+0004cf30: 6173 7365 6420 746f 2027 0a20 2020 2020  assed to '.     
+0004cf40: 2020 2020 2020 2020 2020 2027 5c27 696e             '\'in
+0004cf50: 7465 7270 6f6c 6174 655f 706f 696e 7473  terpolate_points
+0004cf60: 5f73 696e 676c 655f 636f 6e74 6f75 7228  _single_contour(
+0004cf70: 295c 2727 290a 2020 2020 2020 2020 7072  )\'').        pr
+0004cf80: 696e 7428 2753 6f75 7263 6520 6d75 7374  int('Source must
+0004cf90: 2062 6520 7368 6170 656c 7920 506f 6c79   be shapely Poly
+0004cfa0: 676f 6e20 6f72 2063 6f6e 746f 7572 2729  gon or contour')
+0004cfb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0004cfc0: 4e6f 6e65 0a0a 2020 2020 2320 4966 206e  None..    # If n
+0004cfd0: 756d 6265 7220 6f66 2063 6f6e 746f 7572  umber of contour
+0004cfe0: 2070 6f69 6e74 7320 6e6f 7420 7061 7373   points not pass
+0004cff0: 6564 2064 6972 6563 746c 792c 0a20 2020  ed directly,.   
+0004d000: 2023 2074 7279 2074 6f20 6465 7465 726d   # try to determ
+0004d010: 696e 6520 6974 7320 7661 6c75 6520 6672  ine its value fr
+0004d020: 6f6d 2074 6865 2064 6973 7461 6e63 6520  om the distance 
+0004d030: 6265 7477 6565 6e20 636f 6e74 6f75 7220  between contour 
+0004d040: 706f 696e 7473 2e0a 2020 2020 6966 206e  points..    if n
+0004d050: 5f70 6f69 6e74 2069 7320 4e6f 6e65 2061  _point is None a
+0004d060: 6e64 2064 7879 3a0a 2020 2020 2020 2020  nd dxy:.        
+0004d070: 6966 2063 6f6e 746f 7572 5f6c 656e 6774  if contour_lengt
+0004d080: 6820 6973 204e 6f6e 653a 0a20 2020 2020  h is None:.     
+0004d090: 2020 2020 2020 2063 6f6e 746f 7572 5f6c         contour_l
+0004d0a0: 656e 6774 6820 3d20 636f 6e74 6f75 725f  ength = contour_
+0004d0b0: 746f 5f70 6f6c 7967 6f6e 2873 6f75 7263  to_polygon(sourc
+0004d0c0: 6529 2e6c 656e 6774 680a 2020 2020 2020  e).length.      
+0004d0d0: 2020 6e5f 706f 696e 7420 3d20 6d61 7828    n_point = max(
+0004d0e0: 696e 7428 636f 6e74 6f75 725f 6c65 6e67  int(contour_leng
+0004d0f0: 7468 202f 2064 7879 292c 2033 290a 2020  th / dxy), 3).  
+0004d100: 2020 6966 206e 5f70 6f69 6e74 2069 7320    if n_point is 
+0004d110: 4e6f 6e65 3a0a 2020 2020 2020 2020 7072  None:.        pr
+0004d120: 696e 7428 274e 6f20 696e 7465 7270 6f6c  int('No interpol
+0004d130: 6174 696f 6e20 7065 7266 6f72 6d65 6427  ation performed'
+0004d140: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+0004d150: 274e 756d 6265 7220 6f66 2063 6f6e 746f  'Number of conto
+0004d160: 7572 2070 6f69 6e74 7320 286e 5f70 6f69  ur points (n_poi
+0004d170: 6e74 2920 6f72 2064 6973 7461 6e63 6520  nt) or distance 
+0004d180: 6265 7477 6565 6e20 706f 696e 7473 270a  between points'.
+0004d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004d1a0: 276d 7573 7420 6265 2073 7065 6369 6669  'must be specifi
+0004d1b0: 6564 2e27 290a 2020 2020 2020 2020 7265  ed.').        re
+0004d1c0: 7475 726e 204e 6f6e 650a 0a20 2020 2023  turn None..    #
+0004d1d0: 204d 616b 6520 6c61 7374 2070 6f69 6e74   Make last point
+0004d1e0: 2074 6865 2073 616d 6520 6173 2074 6865   the same as the
+0004d1f0: 2066 6972 7374 2c20 746f 2065 6e73 7572   first, to ensur
+0004d200: 6520 636c 6f73 6564 2063 7572 7665 2e0a  e closed curve..
+0004d210: 2020 2020 706f 696e 7473 2e61 7070 656e      points.appen
+0004d220: 6428 706f 696e 7473 5b30 5d29 0a0a 2020  d(points[0])..  
+0004d230: 2020 2320 4469 7363 6172 6420 706f 696e    # Discard poin
+0004d240: 7473 2074 6861 7420 6172 656e 2774 2073  ts that aren't s
+0004d250: 6570 6172 6174 6564 2066 726f 6d20 7468  eparated from th
+0004d260: 6520 7072 6563 6565 6469 6e67 2070 6f69  e preceeding poi
+0004d270: 6e74 0a20 2020 2023 2062 7920 6174 206c  nt.    # by at l
+0004d280: 6561 7374 2073 6f6d 6520 6d69 6e69 6d75  east some minimu
+0004d290: 6d20 6469 7374 616e 6365 2e0a 2020 2020  m distance..    
+0004d2a0: 6478 795f 6d69 6e20 3d20 302e 3030 310a  dxy_min = 0.001.
+0004d2b0: 2020 2020 785f 6c61 7374 2c20 795f 6c61      x_last, y_la
+0004d2c0: 7374 203d 2070 6f69 6e74 735b 305d 0a20  st = points[0]. 
+0004d2d0: 2020 2078 5f76 616c 7565 732c 2079 5f76     x_values, y_v
+0004d2e0: 616c 7565 7320 3d20 285b 785f 6c61 7374  alues = ([x_last
+0004d2f0: 5d2c 205b 795f 6c61 7374 5d29 0a20 2020  ], [y_last]).   
+0004d300: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0004d310: 312c 206c 656e 2870 6f69 6e74 7329 293a  1, len(points)):
+0004d320: 0a20 2020 2020 2020 2078 2c20 7920 3d20  .        x, y = 
+0004d330: 706f 696e 7473 5b69 5d0a 2020 2020 2020  points[i].      
+0004d340: 2020 6966 2028 6162 7328 7820 2d20 785f    if (abs(x - x_
+0004d350: 6c61 7374 2920 3e20 6478 795f 6d69 6e29  last) > dxy_min)
+0004d360: 206f 7220 2861 6273 2879 202d 2079 5f6c   or (abs(y - y_l
+0004d370: 6173 7429 203e 2064 7879 5f6d 696e 293a  ast) > dxy_min):
+0004d380: 0a20 2020 2020 2020 2020 2020 2078 5f76  .            x_v
+0004d390: 616c 7565 732e 6170 7065 6e64 2870 6f69  alues.append(poi
+0004d3a0: 6e74 735b 695d 5b30 5d29 0a20 2020 2020  nts[i][0]).     
+0004d3b0: 2020 2020 2020 2079 5f76 616c 7565 732e         y_values.
+0004d3c0: 6170 7065 6e64 2870 6f69 6e74 735b 695d  append(points[i]
+0004d3d0: 5b31 5d29 0a20 2020 2020 2020 2078 5f6c  [1]).        x_l
+0004d3e0: 6173 742c 2079 5f6c 6173 7420 3d20 706f  ast, y_last = po
+0004d3f0: 696e 7473 5b69 5d0a 0a20 2020 2078 5f76  ints[i]..    x_v
+0004d400: 616c 7565 7320 3d20 6e70 2e61 7272 6179  alues = np.array
+0004d410: 2878 5f76 616c 7565 7329 0a20 2020 2079  (x_values).    y
+0004d420: 5f76 616c 7565 7320 3d20 6e70 2e61 7272  _values = np.arr
+0004d430: 6179 2879 5f76 616c 7565 7329 0a0a 2020  ay(y_values)..  
+0004d440: 2020 2320 496e 7465 7270 6f6c 6174 6520    # Interpolate 
+0004d450: 636f 6e74 6f75 7220 706f 696e 7473 2e0a  contour points..
+0004d460: 2020 2020 736d 6f6f 7468 6e65 7373 203d      smoothness =
+0004d470: 2073 6d6f 6f74 686e 6573 735f 7065 725f   smoothness_per_
+0004d480: 706f 696e 7420 2a20 6c65 6e28 785f 7661  point * len(x_va
+0004d490: 6c75 6573 290a 2020 2020 7472 793a 0a23  lues).    try:.#
+0004d4a0: 2020 2020 2020 2020 7769 7468 2077 6172          with war
+0004d4b0: 6e69 6e67 732e 6361 7463 685f 7761 726e  nings.catch_warn
+0004d4c0: 696e 6773 2829 3a0a 2320 2020 2020 2020  ings():.#       
+0004d4d0: 2020 2020 2077 6172 6e69 6e67 732e 6669       warnings.fi
+0004d4e0: 6c74 6572 7761 726e 696e 6773 2822 6967  lterwarnings("ig
+0004d4f0: 6e6f 7265 222c 206d 6573 7361 6765 3d22  nore", message="
+0004d500: 5365 7474 696e 6720 7822 290a 2020 2020  Setting x").    
+0004d510: 2020 2020 2020 2020 7463 6b2c 2075 203d          tck, u =
+0004d520: 2069 6e74 6572 706f 6c61 7465 2e73 706c   interpolate.spl
+0004d530: 7072 6570 280a 2020 2020 2020 2020 2020  prep(.          
+0004d540: 2020 2020 2020 2020 2020 5b78 5f76 616c            [x_val
+0004d550: 7565 732c 2079 5f76 616c 7565 735d 2c20  ues, y_values], 
+0004d560: 733d 736d 6f6f 7468 6e65 7373 2c20 7065  s=smoothness, pe
+0004d570: 723d 5472 7565 290a 2020 2020 6578 6365  r=True).    exce
+0004d580: 7074 2054 7970 6545 7272 6f72 2061 7320  pt TypeError as 
+0004d590: 7072 6f62 6c65 6d3a 0a20 2020 2020 2020  problem:.       
+0004d5a0: 2070 7269 6e74 2822 5741 524e 494e 473a   print("WARNING:
+0004d5b0: 2050 726f 626c 656d 2069 6e20 696e 7465   Problem in inte
+0004d5c0: 7270 6f6c 6174 655f 636f 6e74 6f75 725f  rpolate_contour_
+0004d5d0: 706f 696e 7473 2829 3a22 2c20 7072 6f62  points():", prob
+0004d5e0: 6c65 6d29 0a20 2020 2020 2020 2072 6574  lem).        ret
+0004d5f0: 7572 6e20 4e6f 6e65 0a0a 2020 2020 7869  urn None..    xi
+0004d600: 5f76 616c 7565 732c 2079 695f 7661 6c75  _values, yi_valu
+0004d610: 6573 203d 2069 6e74 6572 706f 6c61 7465  es = interpolate
+0004d620: 2e73 706c 6576 280a 2020 2020 2020 2020  .splev(.        
+0004d630: 6e70 2e6c 696e 7370 6163 6528 302e 2c20  np.linspace(0., 
+0004d640: 312e 2c20 6e5f 706f 696e 7420 2b20 3129  1., n_point + 1)
+0004d650: 2c20 7463 6b29 0a0a 2020 2020 2320 5374  , tck)..    # St
+0004d660: 6f72 6520 706f 696e 7473 2069 6e20 6120  ore points in a 
+0004d670: 666f 726d 2074 6861 7420 6d61 7920 6265  form that may be
+0004d680: 2063 6f6e 7665 7274 6564 2074 6f20 6120   converted to a 
+0004d690: 6e75 6d70 7920 6172 7261 792e 0a20 2020  numpy array..   
+0004d6a0: 2070 6f69 6e74 735f 696e 7465 7270 6f6c   points_interpol
+0004d6b0: 6174 6564 203d 206c 6973 7428 7a69 7028  ated = list(zip(
+0004d6c0: 7869 5f76 616c 7565 732c 2079 695f 7661  xi_values, yi_va
+0004d6d0: 6c75 6573 2929 0a20 2020 2070 6f69 6e74  lues)).    point
+0004d6e0: 735f 696e 7465 7270 6f6c 6174 6564 203d  s_interpolated =
+0004d6f0: 205b 7879 2066 6f72 2078 7920 696e 2070   [xy for xy in p
+0004d700: 6f69 6e74 735f 696e 7465 7270 6f6c 6174  oints_interpolat
+0004d710: 6564 5d0a 0a20 2020 2023 2052 6574 7572  ed]..    # Retur
+0004d720: 6e20 696e 7465 7270 6f6c 6174 6564 2063  n interpolated c
+0004d730: 6f6e 746f 7572 2069 6e20 7468 6520 7361  ontour in the sa
+0004d740: 6d65 2072 6570 7265 7365 6e74 6174 696f  me representatio
+0004d750: 6e20 6173 2074 6865 2073 6f75 7263 652e  n as the source.
+0004d760: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+0004d770: 6365 2873 6f75 7263 652c 2067 656f 6d65  ce(source, geome
+0004d780: 7472 792e 706f 6c79 676f 6e2e 506f 6c79  try.polygon.Poly
+0004d790: 676f 6e29 3a0a 2020 2020 2020 2020 6f75  gon):.        ou
+0004d7a0: 745f 6f62 6a65 6374 203d 2067 656f 6d65  t_object = geome
+0004d7b0: 7472 792e 706f 6c79 676f 6e2e 506f 6c79  try.polygon.Poly
+0004d7c0: 676f 6e28 706f 696e 7473 5f69 6e74 6572  gon(points_inter
+0004d7d0: 706f 6c61 7465 6429 0a20 2020 2065 6c69  polated).    eli
+0004d7e0: 6620 6973 696e 7374 616e 6365 2873 6f75  f isinstance(sou
+0004d7f0: 7263 652c 206e 702e 6e64 6172 7261 7929  rce, np.ndarray)
+0004d800: 3a0a 2020 2020 2020 2020 6f75 745f 6f62  :.        out_ob
+0004d810: 6a65 6374 203d 206e 702e 6172 7261 7928  ject = np.array(
+0004d820: 706f 696e 7473 5f69 6e74 6572 706f 6c61  points_interpola
+0004d830: 7465 6429 0a20 2020 2065 6c73 653a 0a20  ted).    else:. 
+0004d840: 2020 2020 2020 206f 7574 5f6f 626a 6563         out_objec
+0004d850: 7420 3d20 706f 696e 7473 5f69 6e74 6572  t = points_inter
+0004d860: 706f 6c61 7465 640a 0a20 2020 2072 6574  polated..    ret
+0004d870: 7572 6e20 6f75 745f 6f62 6a65 6374 0a0a  urn out_object..
+0004d880: 6465 6620 7772 6974 655f 7374 7275 6374  def write_struct
+0004d890: 7572 655f 7365 745f 6469 636f 6d28 0a20  ure_set_dicom(. 
+0004d8a0: 2020 206f 7574 6e61 6d65 2c20 0a20 2020     outname, .   
+0004d8b0: 2072 6f69 732c 200a 2020 2020 696d 6167   rois, .    imag
+0004d8c0: 653d 4e6f 6e65 2c20 0a20 2020 2061 6666  e=None, .    aff
+0004d8d0: 696e 653d 4e6f 6e65 2c20 0a20 2020 2073  ine=None, .    s
+0004d8e0: 6861 7065 3d4e 6f6e 652c 0a20 2020 206f  hape=None,.    o
+0004d8f0: 7269 656e 7461 7469 6f6e 3d4e 6f6e 652c  rientation=None,
+0004d900: 200a 2020 2020 6865 6164 6572 5f73 6f75   .    header_sou
+0004d910: 7263 653d 4e6f 6e65 2c20 0a20 2020 2070  rce=None, .    p
+0004d920: 6174 6965 6e74 5f69 643d 4e6f 6e65 2c0a  atient_id=None,.
+0004d930: 2020 2020 6d6f 6461 6c69 7479 3d4e 6f6e      modality=Non
+0004d940: 652c 200a 2020 2020 726f 6f74 5f75 6964  e, .    root_uid
+0004d950: 3d4e 6f6e 650a 293a 0a0a 2020 2020 2320  =None.):..    # 
+0004d960: 4368 6563 6b20 7765 2068 6176 6520 7468  Check we have th
+0004d970: 6520 7265 6c65 7661 6e74 2069 6e66 6f0a  e relevant info.
+0004d980: 2020 2020 6966 206e 6f74 2069 6d61 6765      if not image
+0004d990: 2061 6e64 2028 6e6f 7420 6166 6669 6e65   and (not affine
+0004d9a0: 206f 7220 6e6f 7420 7368 6170 6529 3a0a   or not shape):.
+0004d9b0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+0004d9c0: 6e74 696d 6545 7272 6f72 2822 4d75 7374  ntimeError("Must
+0004d9d0: 2070 726f 7669 6465 2065 6974 6865 7220   provide either 
+0004d9e0: 616e 2069 6d61 6765 206f 7220 616e 2061  an image or an a
+0004d9f0: 6666 696e 6520 6d61 7472 6978 2022 0a20  ffine matrix ". 
+0004da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004da10: 2020 2020 2020 2020 2020 2261 6e64 2073            "and s
+0004da20: 6861 7065 2122 290a 0a20 2020 2023 2054  hape!")..    # T
+0004da30: 7279 2067 6574 7469 6e67 2064 6963 6f6d  ry getting dicom
+0004da40: 2064 6174 6173 6574 2066 726f 6d20 696d   dataset from im
+0004da50: 6167 650a 2020 2020 6473 203d 204e 6f6e  age.    ds = Non
+0004da60: 650a 2020 2020 6966 2069 6d61 6765 3a0a  e.    if image:.
+0004da70: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+0004da80: 7472 2869 6d61 6765 2c20 2264 6963 6f6d  tr(image, "dicom
+0004da90: 5f64 6174 6173 6574 2229 3a0a 2020 2020  _dataset"):.    
+0004daa0: 2020 2020 2020 2020 6473 203d 2069 6d61          ds = ima
+0004dab0: 6765 2e64 6963 6f6d 5f64 6174 6173 6574  ge.dicom_dataset
+0004dac0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0004dad0: 2020 2020 2020 2020 2020 2064 7320 3d20             ds = 
+0004dae0: 736b 7274 2e69 6d61 6765 2e63 7265 6174  skrt.image.creat
+0004daf0: 655f 6469 636f 6d28 290a 2020 2020 2020  e_dicom().      
+0004db00: 2020 2020 2020 6473 2e73 6574 5f67 656f        ds.set_geo
+0004db10: 6d65 7472 7928 0a20 2020 2020 2020 2020  metry(.         
+0004db20: 2020 2020 2020 2069 6d61 6765 2e67 6574         image.get
+0004db30: 5f61 6666 696e 6528 292c 2069 6d61 6765  _affine(), image
+0004db40: 2e67 6574 5f64 6174 6128 292e 7368 6170  .get_data().shap
+0004db50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0004db60: 2020 2069 6d61 6765 2e67 6574 5f6f 7269     image.get_ori
+0004db70: 656e 7461 7469 6f6e 5f76 6563 746f 7228  entation_vector(
+0004db80: 696d 6167 652e 6765 745f 6166 6669 6e65  image.get_affine
+0004db90: 2c20 2264 6963 6f6d 2229 0a20 2020 2020  , "dicom").     
+0004dba0: 2020 2020 2020 2029 0a0a 2020 2020 2320         )..    # 
+0004dbb0: 4f74 6865 7277 6973 652c 2063 7265 6174  Otherwise, creat
+0004dbc0: 6520 6672 6573 6820 6469 636f 6d20 6461  e fresh dicom da
+0004dbd0: 7461 7365 740a 2020 2020 656c 7365 3a0a  taset.    else:.
+0004dbe0: 2020 2020 2020 2020 6473 203d 2073 6b72          ds = skr
+0004dbf0: 742e 696d 6167 652e 6372 6561 7465 5f64  t.image.create_d
+0004dc00: 6963 6f6d 2870 6174 6965 6e74 5f69 642c  icom(patient_id,
+0004dc10: 206d 6f64 616c 6974 792c 2072 6f6f 745f   modality, root_
+0004dc20: 7569 6429 0a20 2020 2020 2020 2064 732e  uid).        ds.
+0004dc30: 7365 745f 6765 6f6d 6574 7279 2861 6666  set_geometry(aff
+0004dc40: 696e 652c 2073 6861 7065 2c20 6f72 6965  ine, shape, orie
+0004dc50: 6e74 6174 696f 6e29 0a0a 2020 2020 2320  ntation)..    # 
+0004dc60: 4164 6a75 7374 2064 6174 6173 6574 2074  Adjust dataset t
+0004dc70: 6f20 6265 2066 6f72 2053 7472 7563 7475  o be for Structu
+0004dc80: 7265 5365 7420 696e 7374 6561 6420 6f66  reSet instead of
+0004dc90: 2069 6d61 6765 0a0a 0a64 6566 2064 6963   image...def dic
+0004dca0: 6f6d 5f64 6174 6173 6574 5f74 6f5f 7374  om_dataset_to_st
+0004dcb0: 7275 6374 7572 655f 7365 7428 6473 293a  ructure_set(ds):
+0004dcc0: 0a20 2020 2027 2727 436f 6e76 6572 7420  .    '''Convert 
+0004dcd0: 616e 2065 7869 7374 696e 6720 696d 6167  an existing imag
+0004dce0: 6520 6469 636f 6d20 6461 7461 7365 7420  e dicom dataset 
+0004dcf0: 746f 2061 2053 7472 7563 7475 7265 5365  to a StructureSe
+0004dd00: 7420 6461 7461 7365 742e 2727 270a 0a20  t dataset.'''.. 
+0004dd10: 2020 2023 2041 646a 7573 7420 636c 6173     # Adjust clas
+0004dd20: 7320 5549 4473 0a20 2020 2064 732e 6669  s UIDs.    ds.fi
+0004dd30: 6c65 5f6d 6574 612e 496d 706c 656d 656e  le_meta.Implemen
+0004dd40: 7461 7469 6f6e 436c 6173 7355 4944 203d  tationClassUID =
+0004dd50: 2022 392e 392e 392e 3130 302e 302e 302e   "9.9.9.100.0.0.
+0004dd60: 312e 302e 392e 362e 302e 302e 3122 0a20  1.0.9.6.0.0.1". 
+0004dd70: 2020 2064 732e 6669 6c65 5f6d 6574 612e     ds.file_meta.
+0004dd80: 4d65 6469 6153 746f 7261 6765 534f 5043  MediaStorageSOPC
+0004dd90: 6c61 7373 5549 4420 3d20 2231 2e32 2e38  lassUID = "1.2.8
+0004dda0: 3430 2e31 3030 3038 2e35 2e31 2e34 2e31  40.10008.5.1.4.1
+0004ddb0: 2e31 2e34 3831 2e33 220a 0a20 2020 2023  .1.481.3"..    #
+0004ddc0: 2041 7373 6967 6e20 656d 7074 7920 7365   Assign empty se
+0004ddd0: 7175 656e 6365 730a 2020 2020 6473 2e52  quences.    ds.R
+0004dde0: 6566 6572 656e 6365 6446 7261 6d65 6f66  eferencedFrameof
+0004ddf0: 5265 6665 7265 6e63 6553 6571 7565 6e63  ReferenceSequenc
+0004de00: 6520 3d20 5365 7175 656e 6365 2829 0a20  e = Sequence(). 
+0004de10: 2020 2064 732e 5374 7275 6374 7572 6553     ds.StructureS
+0004de20: 6574 524f 4953 6571 7565 6e63 6520 3d20  etROISequence = 
+0004de30: 5365 7175 656e 6365 2829 0a20 2020 2064  Sequence().    d
+0004de40: 732e 5254 524f 494f 6273 6572 7661 7469  s.RTROIObservati
+0004de50: 6f6e 7353 6571 7565 6e63 6520 3d20 5365  onsSequence = Se
+0004de60: 7175 656e 6365 2829 0a20 2020 2064 732e  quence().    ds.
+0004de70: 524f 4943 6f6e 746f 7572 5365 7175 656e  ROIContourSequen
+0004de80: 6365 203d 2053 6571 7565 6e63 6528 290a  ce = Sequence().
+0004de90: 0a20 2020 2023 2041 7373 6967 6e20 7374  .    # Assign st
+0004dea0: 7275 6374 7572 6520 7365 7420 7072 6f70  ructure set prop
+0004deb0: 6572 7469 6573 0a20 2020 2064 732e 5374  erties.    ds.St
+0004dec0: 7275 6374 7572 6553 6574 4c61 6265 6c20  ructureSetLabel 
+0004ded0: 3d20 2222 0a20 2020 2064 732e 5374 7275  = "".    ds.Stru
+0004dee0: 6374 7572 6553 6574 4461 7465 203d 2064  ctureSetDate = d
+0004def0: 732e 496e 7374 616e 6365 4372 6561 7469  s.InstanceCreati
+0004df00: 6f6e 4461 7465 0a20 2020 2064 732e 5374  onDate.    ds.St
+0004df10: 7275 6374 7572 6553 6574 5469 6d65 203d  ructureSetTime =
+0004df20: 2064 732e 496e 7374 616e 6365 4372 6561   ds.InstanceCrea
+0004df30: 7469 6f6e 5469 6d65 0a0a 2020 2020 2320  tionTime..    # 
+0004df40: 4173 7369 676e 2066 7261 6d65 206f 6620  Assign frame of 
+0004df50: 7265 6665 7265 6e63 650a 0a0a 6465 6620  reference...def 
+0004df60: 6372 6561 7465 5f64 756d 6d79 5f69 6d61  create_dummy_ima
+0004df70: 6765 280a 2020 2020 6578 7465 6e74 732c  ge(.    extents,
+0004df80: 200a 2020 2020 736c 6963 655f 7468 6963   .    slice_thic
+0004df90: 6b6e 6573 732c 0a20 2020 2073 6861 7065  kness,.    shape
+0004dfa0: 3d4e 6f6e 652c 200a 2020 2020 766f 7865  =None, .    voxe
+0004dfb0: 6c5f 7369 7a65 3d4e 6f6e 652c 0a20 2020  l_size=None,.   
+0004dfc0: 2066 696c 6c5f 7661 6c3d 3165 342c 0a20   fill_val=1e4,. 
+0004dfd0: 2020 2062 7566 6665 723d 320a 293a 0a20     buffer=2.):. 
+0004dfe0: 2020 2022 2222 4d61 6b65 2061 2064 756d     """Make a dum
+0004dff0: 6d79 2069 6d61 6765 2074 6861 7420 636f  my image that co
+0004e000: 7665 7273 2074 6865 2061 7265 6120 7370  vers the area sp
+0004e010: 616e 6e65 6420 6279 203c 6578 7465 6e74  anned by <extent
+0004e020: 733e 2070 6c75 7320 6120 0a20 2020 2062  s> plus a .    b
+0004e030: 7566 6665 722e 0a0a 2020 2020 2a2a 5061  uffer...    **Pa
+0004e040: 7261 6d65 7465 7273 3a2a 2a0a 2020 2020  rameters:**.    
+0004e050: 0a20 2020 2065 7874 656e 7473 203a 206c  .    extents : l
+0004e060: 6973 740a 2020 2020 2020 2020 4c69 7374  ist.        List
+0004e070: 206f 6620 5b6d 696e 2c20 6d61 785d 2065   of [min, max] e
+0004e080: 7874 656e 7473 2069 6e20 6d6d 2061 6c6f  xtents in mm alo
+0004e090: 6e67 2065 6163 6820 6f66 2074 6865 2074  ng each of the t
+0004e0a0: 6872 6565 2061 7865 7320 696e 200a 2020  hree axes in .  
+0004e0b0: 2020 2020 2020 6f72 6465 7220 5b78 2c20        order [x, 
+0004e0c0: 792c 207a 5d2e 0a0a 2020 2020 736c 6963  y, z]...    slic
+0004e0d0: 655f 7468 6963 6b6e 6573 7320 3a20 666c  e_thickness : fl
+0004e0e0: 6f61 740a 2020 2020 2020 2020 536c 6963  oat.        Slic
+0004e0f0: 6520 7468 6963 6b6e 6573 7320 696e 206d  e thickness in m
+0004e100: 6d2e 0a0a 2020 2020 766f 7865 6c5f 7369  m...    voxel_si
+0004e110: 7a65 203a 206c 6973 742c 2064 6566 6175  ze : list, defau
+0004e120: 6c74 3d4e 6f6e 650a 2020 2020 2020 2020  lt=None.        
+0004e130: 566f 7865 6c20 7369 7a65 2069 6e20 6d6d  Voxel size in mm
+0004e140: 2069 6e20 7468 6520 6475 6d6d 7920 696d   in the dummy im
+0004e150: 6167 6520 696e 2074 6865 2078 2d79 2070  age in the x-y p
+0004e160: 6c61 6e65 2c20 6769 7665 6e20 6173 200a  lane, given as .
+0004e170: 2020 2020 2020 2020 5b76 782c 2076 795d          [vx, vy]
+0004e180: 2e20 4966 203c 7368 6170 653e 2061 6e64  . If <shape> and
+0004e190: 203c 766f 7865 6c5f 7369 7a65 3e20 6172   <voxel_size> ar
+0004e1a0: 6520 626f 7468 204e 6f6e 652c 2076 6f78  e both None, vox
+0004e1b0: 656c 2073 697a 6573 206f 660a 2020 2020  el sizes of.    
+0004e1c0: 2020 2020 5b31 2c20 315d 2077 696c 6c20      [1, 1] will 
+0004e1d0: 6265 2075 7365 6420 6279 2064 6566 6175  be used by defau
+0004e1e0: 6c74 2e20 5468 6520 766f 7865 6c20 7369  lt. The voxel si
+0004e1f0: 7a65 2069 6e20 7468 6520 7a20 6469 7265  ze in the z dire
+0004e200: 6374 696f 6e20 0a20 2020 2020 2020 2077  ction .        w
+0004e210: 696c 6c20 6265 2074 616b 656e 2066 726f  ill be taken fro
+0004e220: 6d20 7468 6520 6d69 6e69 6d75 6d20 6469  m the minimum di
+0004e230: 7374 616e 6365 2062 6574 7765 656e 2073  stance between s
+0004e240: 6c69 6365 2070 6f73 6974 696f 6e73 2069  lice positions i
+0004e250: 6e20 0a20 2020 2020 2020 2074 6865 2078  n .        the x
+0004e260: 2d79 2063 6f6e 746f 7572 7320 6469 6374  -y contours dict
+0004e270: 696f 6e61 7279 2e0a 0a20 2020 2073 6861  ionary...    sha
+0004e280: 7065 203a 206c 6973 742c 2064 6566 6175  pe : list, defau
+0004e290: 6c74 3d4e 6f6e 650a 2020 2020 2020 2020  lt=None.        
+0004e2a0: 4e75 6d62 6572 206f 6620 766f 7865 6c73  Number of voxels
+0004e2b0: 2069 6e20 7468 6520 6475 6d6d 7920 696d   in the dummy im
+0004e2c0: 6167 6520 696e 2074 6865 2078 2d79 2070  age in the x-y p
+0004e2d0: 6c61 6e65 2c20 6769 7665 6e20 6173 0a20  lane, given as. 
+0004e2e0: 2020 2020 2020 205b 6e78 2c20 6e79 5d2e         [nx, ny].
+0004e2f0: 204f 6e6c 7920 7573 6564 2069 6620 3c76   Only used if <v
+0004e300: 6f78 656c 5f73 697a 653e 2069 7320 4e6f  oxel_size> is No
+0004e310: 6e65 2e20 0a20 2020 2020 2020 2054 6865  ne. .        The
+0004e320: 206e 756d 6265 7220 6f66 2076 6f78 656c   number of voxel
+0004e330: 7320 696e 2074 6865 207a 2064 6972 6563  s in the z direc
+0004e340: 7469 6f6e 2077 696c 6c20 6265 2074 616b  tion will be tak
+0004e350: 656e 2066 726f 6d20 7468 6520 0a20 2020  en from the .   
+0004e360: 2020 2020 206e 756d 6265 7220 6f66 2073       number of s
+0004e370: 6c69 6365 7320 696e 2074 6865 2078 2d79  lices in the x-y
+0004e380: 2063 6f6e 746f 7572 7320 6469 6374 696f   contours dictio
+0004e390: 6e61 7279 2e0a 0a20 2020 2066 696c 6c5f  nary...    fill_
+0004e3a0: 7661 6c20 3a20 696e 742f 666c 6f61 742c  val : int/float,
+0004e3b0: 2064 6566 6175 6c74 3d31 6534 0a20 2020   default=1e4.   
+0004e3c0: 2020 2020 2056 616c 7565 2077 6974 6820       Value with 
+0004e3d0: 7768 6963 6820 7468 6520 766f 7865 6c73  which the voxels
+0004e3e0: 2069 6e20 7468 6520 6475 6d6d 7920 696d   in the dummy im
+0004e3f0: 6167 6520 7368 6f75 6c64 2062 6520 6669  age should be fi
+0004e400: 6c6c 6564 2e20 0a0a 2020 2020 6275 6666  lled. ..    buff
+0004e410: 6572 203a 2066 6c6f 6174 2c20 6465 6661  er : float, defa
+0004e420: 756c 743d 320a 2020 2020 2020 2020 4275  ult=2.        Bu
+0004e430: 6666 6572 2061 6d6f 756e 7420 6f66 2077  ffer amount of w
+0004e440: 6869 7465 7370 6163 6520 696e 206d 6d20  hitespace in mm 
+0004e450: 746f 2061 6464 206f 7574 7369 6465 2074  to add outside t
+0004e460: 6865 2052 4f49 2069 6e20 6561 6368 200a  he ROI in each .
+0004e470: 2020 2020 2020 2020 6469 7265 6374 696f          directio
+0004e480: 6e2e 0a20 2020 2022 2222 0a0a 2020 2020  n..    """..    
+0004e490: 2320 4173 7369 676e 2064 6566 6175 6c74  # Assign default
+0004e4a0: 2076 6f78 656c 2073 697a 650a 2020 2020   voxel size.    
+0004e4b0: 6966 2073 6861 7065 2069 7320 4e6f 6e65  if shape is None
+0004e4c0: 2061 6e64 2076 6f78 656c 5f73 697a 6520   and voxel_size 
+0004e4d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0004e4e0: 2076 6f78 656c 5f73 697a 6520 3d20 5b31   voxel_size = [1
+0004e4f0: 2c20 315d 0a20 2020 2069 6620 6e6f 7420  , 1].    if not 
+0004e500: 736b 7274 2e63 6f72 652e 6973 5f6c 6973  skrt.core.is_lis
+0004e510: 7428 766f 7865 6c5f 7369 7a65 293a 0a20  t(voxel_size):. 
+0004e520: 2020 2020 2020 2076 6f78 656c 5f73 697a         voxel_siz
+0004e530: 6520 3d20 5b76 6f78 656c 5f73 697a 655d  e = [voxel_size]
+0004e540: 202a 2032 0a0a 2020 2020 2320 4361 6c63   * 2..    # Calc
+0004e550: 756c 6174 6520 766f 7865 6c20 7369 7a65  ulate voxel size
+0004e560: 7320 6672 6f6d 2073 6861 7065 0a20 2020  s from shape.   
+0004e570: 2069 6620 7368 6170 6520 6973 206e 6f74   if shape is not
+0004e580: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
+0004e590: 6861 7065 203d 206c 6973 7428 7368 6170  hape = list(shap
+0004e5a0: 6529 0a20 2020 2020 2020 2069 6620 6c65  e).        if le
+0004e5b0: 6e28 7368 6170 6529 2021 3d20 323a 0a20  n(shape) != 2:. 
+0004e5c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0004e5d0: 2054 7970 6545 7272 6f72 2822 5368 6170   TypeError("Shap
+0004e5e0: 6520 7368 6f75 6c64 2062 6520 6120 6c69  e should be a li
+0004e5f0: 7374 206f 6620 7477 6f20 7661 6c75 6573  st of two values
+0004e600: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0004e610: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0004e620: 7370 6563 6966 7969 6e67 2064 756d 6d79  specifying dummy
+0004e630: 2069 6d61 6765 2073 6861 7065 2069 6e20   image shape in 
+0004e640: 7468 6520 5b78 2c20 795d 2022 0a20 2020  the [x, y] ".   
+0004e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004e660: 2020 2020 2020 2020 2022 6469 7265 6374           "direct
+0004e670: 696f 6e73 2e22 290a 0a20 2020 2020 2020  ions.")..       
+0004e680: 2023 2043 616c 6375 6c61 7465 2076 6f78   # Calculate vox
+0004e690: 656c 2073 697a 6520 6966 2052 4f49 2065  el size if ROI e
+0004e6a0: 7874 656e 7420 706c 7573 2062 7566 6665  xtent plus buffe
+0004e6b0: 7220 6973 2064 6976 6964 6564 2062 7920  r is divided by 
+0004e6c0: 7368 6170 650a 2020 2020 2020 2020 766f  shape.        vo
+0004e6d0: 7865 6c5f 7369 7a65 203d 205b 286d 6178  xel_size = [(max
+0004e6e0: 2865 7829 202d 206d 696e 2865 7829 202b  (ex) - min(ex) +
+0004e6f0: 2032 202a 2062 7566 6665 7229 202f 2073   2 * buffer) / s
+0004e700: 6861 7065 5b69 5d0a 2020 2020 2020 2020  hape[i].        
+0004e710: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0004e720: 7220 692c 2065 7820 696e 2065 6e75 6d65  r i, ex in enume
+0004e730: 7261 7465 2865 7874 656e 7473 5b3a 325d  rate(extents[:2]
+0004e740: 295d 0a0a 2020 2020 2320 4f74 6865 7277  )]..    # Otherw
+0004e750: 6973 652c 2063 616c 6375 6c61 7465 2073  ise, calculate s
+0004e760: 6861 7065 2066 726f 6d20 766f 7865 6c20  hape from voxel 
+0004e770: 7369 7a65 730a 2020 2020 656c 7365 3a0a  sizes.    else:.
+0004e780: 2020 2020 2020 2020 766f 7865 6c5f 7369          voxel_si
+0004e790: 7a65 203d 206c 6973 7428 766f 7865 6c5f  ze = list(voxel_
+0004e7a0: 7369 7a65 290a 2020 2020 2020 2020 0a20  size).        . 
+0004e7b0: 2020 2020 2020 2023 2043 616c 6375 6c61         # Calcula
+0004e7c0: 7465 206e 756d 6265 7220 6f66 2076 6f78  te number of vox
+0004e7d0: 656c 7320 6e65 6564 6564 2074 6f20 636f  els needed to co
+0004e7e0: 7665 7220 524f 4920 706c 7573 2062 7566  ver ROI plus buf
+0004e7f0: 6665 7220 6561 6368 2073 6964 650a 2020  fer each side.  
+0004e800: 2020 2020 2020 7368 6170 6520 3d20 5b28        shape = [(
+0004e810: 6e70 2e63 6569 6c28 286d 6178 2865 7829  np.ceil((max(ex)
+0004e820: 202d 206d 696e 2865 7829 2920 2b20 3220   - min(ex)) + 2 
+0004e830: 2a20 6275 6666 6572 2920 2f20 766f 7865  * buffer) / voxe
+0004e840: 6c5f 7369 7a65 5b69 5d29 200a 2020 2020  l_size[i]) .    
+0004e850: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0004e860: 2069 2c20 6578 2069 6e20 656e 756d 6572   i, ex in enumer
+0004e870: 6174 6528 6578 7465 6e74 735b 3a32 5d29  ate(extents[:2])
+0004e880: 5d0a 0a20 2020 2023 2047 6574 207a 2076  ]..    # Get z v
+0004e890: 6f78 656c 2073 697a 6520 616e 6420 7368  oxel size and sh
+0004e8a0: 6170 650a 2020 2020 766f 7865 6c5f 7369  ape.    voxel_si
+0004e8b0: 7a65 2e61 7070 656e 6428 736c 6963 655f  ze.append(slice_
+0004e8c0: 7468 6963 6b6e 6573 7329 0a20 2020 2073  thickness).    s
+0004e8d0: 6861 7065 5f7a 203d 2028 6d61 7828 6578  hape_z = (max(ex
+0004e8e0: 7465 6e74 735b 325d 2920 2d20 6d69 6e28  tents[2]) - min(
+0004e8f0: 6578 7465 6e74 735b 325d 2929 202f 2073  extents[2])) / s
+0004e900: 6c69 6365 5f74 6869 636b 6e65 7373 0a0a  lice_thickness..
+0004e910: 2020 2020 2320 4164 6420 6e65 6172 6573      # Add neares
+0004e920: 7420 696e 7465 6765 7220 6e75 6d62 6572  t integer number
+0004e930: 206f 6620 6275 6666 6572 2076 6f78 656c   of buffer voxel
+0004e940: 730a 2020 2020 6e5f 6275 6666 5f7a 203d  s.    n_buff_z =
+0004e950: 206e 702e 6365 696c 2862 7566 6665 7220   np.ceil(buffer 
+0004e960: 2f20 736c 6963 655f 7468 6963 6b6e 6573  / slice_thicknes
+0004e970: 7329 0a20 2020 2073 6861 7065 2e61 7070  s).    shape.app
+0004e980: 656e 6428 7368 6170 655f 7a20 2b20 3220  end(shape_z + 2 
+0004e990: 2a20 6e5f 6275 6666 5f7a 290a 2020 2020  * n_buff_z).    
+0004e9a0: 7368 6170 6520 3d20 5b69 6e74 2873 2920  shape = [int(s) 
+0004e9b0: 666f 7220 7320 696e 2073 6861 7065 5d0a  for s in shape].
+0004e9c0: 0a20 2020 2023 2047 6574 206f 7269 6769  .    # Get origi
+0004e9d0: 6e20 706f 7369 7469 6f6e 3b20 656e 7375  n position; ensu
+0004e9e0: 7265 2074 6861 7420 6f72 6967 696e 2070  re that origin p
+0004e9f0: 6f69 6e74 7320 746f 2063 656e 7472 6520  oints to centre 
+0004ea00: 6f66 2062 7566 6665 7220 766f 7865 6c20  of buffer voxel 
+0004ea10: 0a20 2020 2023 206f 7574 7369 6465 2052  .    # outside R
+0004ea20: 4f49 0a20 2020 206f 7269 6769 6e20 3d20  OI.    origin = 
+0004ea30: 5b6d 696e 2865 7829 202b 2061 6273 2876  [min(ex) + abs(v
+0004ea40: 6f78 656c 5f73 697a 655b 695d 2920 2a20  oxel_size[i]) * 
+0004ea50: 302e 3520 2d20 6275 6666 6572 0a20 2020  0.5 - buffer.   
+0004ea60: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0004ea70: 2c20 6578 2069 6e20 656e 756d 6572 6174  , ex in enumerat
+0004ea80: 6528 6578 7465 6e74 735b 3a32 5d29 5d0a  e(extents[:2])].
+0004ea90: 2020 2020 6f72 6967 696e 2e61 7070 656e      origin.appen
+0004eaa0: 6428 6d69 6e28 6578 7465 6e74 735b 325d  d(min(extents[2]
+0004eab0: 2920 2d20 6162 7328 736c 6963 655f 7468  ) - abs(slice_th
+0004eac0: 6963 6b6e 6573 7329 202a 2028 6e5f 6275  ickness) * (n_bu
+0004ead0: 6666 5f7a 202d 2030 2e35 2929 0a0a 2020  ff_z - 0.5))..  
+0004eae0: 2020 2320 4372 6561 7465 2069 6d61 6765    # Create image
+0004eaf0: 0a20 2020 2072 6574 7572 6e20 736b 7274  .    return skrt
+0004eb00: 2e69 6d61 6765 2e49 6d61 6765 280a 2020  .image.Image(.  
+0004eb10: 2020 2020 2020 6e70 2e6f 6e65 7328 2873        np.ones((s
+0004eb20: 6861 7065 5b31 5d2c 2073 6861 7065 5b30  hape[1], shape[0
+0004eb30: 5d2c 2073 6861 7065 5b32 5d29 2920 2a20  ], shape[2])) * 
+0004eb40: 6669 6c6c 5f76 616c 2c0a 2020 2020 2020  fill_val,.      
+0004eb50: 2020 766f 7865 6c5f 7369 7a65 3d76 6f78    voxel_size=vox
+0004eb60: 656c 5f73 697a 652c 0a20 2020 2020 2020  el_size,.       
+0004eb70: 206f 7269 6769 6e3d 6f72 6967 696e 0a20   origin=origin. 
+0004eb80: 2020 2029 0a0a 0a64 6566 2063 7265 6174     )...def creat
+0004eb90: 655f 7374 6170 6c65 2872 6f69 732c 202a  e_staple(rois, *
+0004eba0: 2a6b 7761 7267 7329 3a0a 2020 2020 2222  *kwargs):.    ""
+0004ebb0: 2243 7265 6174 6520 5354 4150 4c45 2052  "Create STAPLE R
+0004ebc0: 4f49 2066 726f 6d20 6c69 7374 206f 6620  OI from list of 
+0004ebd0: 524f 4973 2e22 2222 0a0a 2020 2020 2320  ROIs."""..    # 
+0004ebe0: 5472 7920 696d 706f 7274 2053 696d 706c  Try import Simpl
+0004ebf0: 6549 544b 0a20 2020 2074 7279 3a0a 2020  eITK.    try:.  
+0004ec00: 2020 2020 2020 696d 706f 7274 2053 696d        import Sim
+0004ec10: 706c 6549 544b 2061 7320 7369 746b 0a20  pleITK as sitk. 
+0004ec20: 2020 2065 7863 6570 7420 4d6f 6475 6c65     except Module
+0004ec30: 4e6f 7446 6f75 6e64 4572 726f 723a 0a20  NotFoundError:. 
+0004ec40: 2020 2020 2020 2072 6169 7365 204d 6f64         raise Mod
+0004ec50: 756c 654e 6f74 466f 756e 6445 7272 6f72  uleNotFoundError
+0004ec60: 2822 5369 6d70 6c65 4954 4b20 6973 2072  ("SimpleITK is r
+0004ec70: 6571 7569 7265 6420 746f 2063 616c 6375  equired to calcu
+0004ec80: 6c61 7465 2053 5441 504c 4520 636f 6e74  late STAPLE cont
+0004ec90: 6f75 722e 2022 0a20 2020 2020 2020 2020  our. ".         
+0004eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004ecb0: 2020 2020 2020 2020 2022 5472 7920 696e           "Try in
+0004ecc0: 7374 616c 6c69 6e67 2076 6961 3a20 7069  stalling via: pi
+0004ecd0: 7020 696e 7374 616c 6c20 7369 6d70 6c65  p install simple
+0004ece0: 6974 6b22 290a 0a20 2020 2023 2047 6574  itk")..    # Get
+0004ecf0: 2053 5441 504c 4520 6d61 736b 0a20 2020   STAPLE mask.   
+0004ed00: 2072 6f69 5f61 7272 6179 7320 3d20 5b5d   roi_arrays = []
+0004ed10: 0a20 2020 2066 6f72 2072 6f69 2069 6e20  .    for roi in 
+0004ed20: 726f 6973 3a0a 2020 2020 2020 2020 726f  rois:.        ro
+0004ed30: 695f 6172 7261 7973 2e61 7070 656e 6428  i_arrays.append(
+0004ed40: 7369 746b 2e47 6574 496d 6167 6546 726f  sitk.GetImageFro
+0004ed50: 6d41 7272 6179 2872 6f69 2e67 6574 5f6d  mArray(roi.get_m
+0004ed60: 6173 6b28 0a20 2020 2020 2020 2020 2020  ask(.           
+0004ed70: 2073 7461 6e64 6172 6469 7365 3d54 7275   standardise=Tru
+0004ed80: 6529 2e61 7374 7970 6528 696e 7429 2929  e).astype(int)))
+0004ed90: 0a20 2020 2070 726f 6273 203d 2073 6974  .    probs = sit
+0004eda0: 6b2e 4765 7441 7272 6179 4672 6f6d 496d  k.GetArrayFromIm
+0004edb0: 6167 6528 7369 746b 2e53 5441 504c 4528  age(sitk.STAPLE(
+0004edc0: 726f 695f 6172 7261 7973 2c20 3129 290a  roi_arrays, 1)).
+0004edd0: 2020 2020 6d61 736b 203d 2070 726f 6273      mask = probs
+0004ede0: 203e 2030 2e39 350a 0a20 2020 2023 2043   > 0.95..    # C
+0004edf0: 7265 6174 6520 5354 4150 4c45 2052 4f49  reate STAPLE ROI
+0004ee00: 206f 626a 6563 740a 2020 2020 7265 7475   object.    retu
+0004ee10: 726e 2052 4f49 286d 6173 6b2c 202a 2a6b  rn ROI(mask, **k
+0004ee20: 7761 7267 7329 0a0a 0a64 6566 2063 7265  wargs)...def cre
+0004ee30: 6174 655f 6d61 6a6f 7269 7479 5f76 6f74  ate_majority_vot
+0004ee40: 6528 726f 6973 2c20 2a2a 6b77 6172 6773  e(rois, **kwargs
+0004ee50: 293a 0a20 2020 2022 2222 4372 6561 7465  ):.    """Create
+0004ee60: 206d 616a 6f72 6974 7920 766f 7465 2052   majority vote R
+0004ee70: 4f49 2066 726f 6d20 6c69 7374 206f 6620  OI from list of 
+0004ee80: 524f 4973 2e22 2222 0a0a 2020 2020 6d61  ROIs."""..    ma
+0004ee90: 736b 203d 2072 6f69 735b 305d 2e67 6574  sk = rois[0].get
+0004eea0: 5f6d 6173 6b28 7374 616e 6461 7264 6973  _mask(standardis
+0004eeb0: 653d 5472 7565 292e 6173 7479 7065 2869  e=True).astype(i
+0004eec0: 6e74 290a 2020 2020 666f 7220 726f 6920  nt).    for roi 
+0004eed0: 696e 2072 6f69 735b 313a 5d3a 0a20 2020  in rois[1:]:.   
+0004eee0: 2020 2020 206d 6173 6b20 2b3d 2072 6f69       mask += roi
+0004eef0: 2e67 6574 5f6d 6173 6b28 7374 616e 6461  .get_mask(standa
+0004ef00: 7264 6973 653d 5472 7565 292e 6173 7479  rdise=True).asty
+0004ef10: 7065 2869 6e74 290a 2020 2020 6d61 736b  pe(int).    mask
+0004ef20: 203d 206d 6173 6b20 3e3d 206c 656e 2872   = mask >= len(r
+0004ef30: 6f69 7329 202f 2032 0a20 2020 2072 6574  ois) / 2.    ret
+0004ef40: 7572 6e20 524f 4928 6d61 736b 2c20 2a2a  urn ROI(mask, **
+0004ef50: 6b77 6172 6773 290a 0a0a 6465 6620 6372  kwargs)...def cr
+0004ef60: 6561 7465 5f72 6f69 5f73 756d 2872 6f69  eate_roi_sum(roi
+0004ef70: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
+0004ef80: 2020 2222 2243 7265 6174 6520 524f 4920    """Create ROI 
+0004ef90: 6672 6f6d 2073 756d 206f 6620 6c69 7374  from sum of list
+0004efa0: 206f 6620 524f 4973 2e22 2222 0a0a 2020   of ROIs."""..  
+0004efb0: 2020 6d61 736b 203d 2072 6f69 735b 305d    mask = rois[0]
+0004efc0: 2e67 6574 5f6d 6173 6b28 7374 616e 6461  .get_mask(standa
+0004efd0: 7264 6973 653d 5472 7565 292e 636f 7079  rdise=True).copy
+0004efe0: 2829 0a20 2020 2066 6f72 2072 6f69 2069  ().    for roi i
+0004eff0: 6e20 726f 6973 5b31 3a5d 3a0a 2020 2020  n rois[1:]:.    
+0004f000: 2020 2020 6d61 736b 202b 3d20 726f 692e      mask += roi.
+0004f010: 6765 745f 6d61 736b 2873 7461 6e64 6172  get_mask(standar
+0004f020: 6469 7365 3d54 7275 6529 0a20 2020 2072  dise=True).    r
+0004f030: 6574 7572 6e20 524f 4928 6d61 736b 2c20  eturn ROI(mask, 
+0004f040: 2a2a 6b77 6172 6773 290a 0a0a 6465 6620  **kwargs)...def 
+0004f050: 6372 6561 7465 5f72 6f69 5f6f 7665 726c  create_roi_overl
+0004f060: 6170 2872 6f69 732c 202a 2a6b 7761 7267  ap(rois, **kwarg
+0004f070: 7329 3a0a 2020 2020 2222 2243 7265 6174  s):.    """Creat
+0004f080: 6520 524f 4920 6672 6f6d 206f 7665 726c  e ROI from overl
+0004f090: 6170 206f 6620 6c69 7374 206f 6620 524f  ap of list of RO
+0004f0a0: 4973 2e22 2222 0a0a 2020 2020 6d61 736b  Is."""..    mask
+0004f0b0: 203d 2072 6f69 735b 305d 2e67 6574 5f6d   = rois[0].get_m
+0004f0c0: 6173 6b28 7374 616e 6461 7264 6973 653d  ask(standardise=
+0004f0d0: 5472 7565 292e 636f 7079 2829 0a20 2020  True).copy().   
+0004f0e0: 2066 6f72 2072 6f69 2069 6e20 726f 6973   for roi in rois
+0004f0f0: 5b31 3a5d 3a0a 2020 2020 2020 2020 6d61  [1:]:.        ma
+0004f100: 736b 202a 3d20 726f 692e 6765 745f 6d61  sk *= roi.get_ma
+0004f110: 736b 2873 7461 6e64 6172 6469 7365 3d54  sk(standardise=T
+0004f120: 7275 6529 0a20 2020 2072 6574 7572 6e20  rue).    return 
+0004f130: 524f 4928 6d61 736b 2c20 2a2a 6b77 6172  ROI(mask, **kwar
+0004f140: 6773 290a 0a0a 6465 6620 6466 5f74 6f5f  gs)...def df_to_
+0004f150: 6874 6d6c 2864 6629 3a0a 2020 2020 2222  html(df):.    ""
+0004f160: 2243 6f6e 7665 7274 2061 2070 616e 6461  "Convert a panda
+0004f170: 7320 4461 7461 4672 616d 6520 746f 2068  s DataFrame to h
+0004f180: 746d 6c2e 2222 220a 0a20 2020 2023 2043  tml."""..    # C
+0004f190: 6f6e 7665 7274 2064 6174 6166 7261 6d65  onvert dataframe
+0004f1a0: 2074 6f20 4854 4d4c 0a20 2020 2068 746d   to HTML.    htm
+0004f1b0: 6c20 3d20 6466 2e66 696c 6c6e 6128 27e2  l = df.fillna('.
+0004f1c0: 8094 2729 2e74 6f5f 6874 6d6c 2869 6e64  ..').to_html(ind
+0004f1d0: 6578 3d46 616c 7365 290a 2020 2020 6874  ex=False).    ht
+0004f1e0: 6d6c 203d 2068 746d 6c2e 7265 706c 6163  ml = html.replac
+0004f1f0: 6528 225e 3322 2c20 223c 7375 703e 333c  e("^3", "<sup>3<
+0004f200: 2f73 7570 3e22 292e 7265 706c 6163 6528  /sup>").replace(
+0004f210: 225e 3222 2c20 223c 7375 703e 323c 2f73  "^2", "<sup>2</s
+0004f220: 7570 3e22 290a 0a20 2020 2023 2041 6464  up>")..    # Add
+0004f230: 2068 6561 6465 7220 7769 7468 2073 7479   header with sty
+0004f240: 6c65 2064 6574 6169 6c73 0a20 2020 2068  le details.    h
+0004f250: 6561 6465 7220 3d20 2222 220a 2020 2020  eader = """.    
+0004f260: 2020 2020 3c68 6561 643e 0a20 2020 2020      <head>.     
+0004f270: 2020 2020 2020 203c 7374 796c 653e 0a20         <style>. 
+0004f280: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0004f290: 682c 2074 6420 7b0a 2020 2020 2020 2020  h, td {.        
+0004f2a0: 2020 2020 2020 2020 2020 2020 7061 6464              padd
+0004f2b0: 696e 673a 2032 7078 2032 7078 3b0a 2020  ing: 2px 2px;.  
+0004f2c0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+0004f2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004f2e0: 7468 207b 0a20 2020 2020 2020 2020 2020  th {.           
+0004f2f0: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
+0004f300: 756e 642d 636f 6c6f 723a 2074 7261 6e73  und-color: trans
+0004f310: 7061 7265 6e74 3b0a 2020 2020 2020 2020  parent;.        
+0004f320: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0004f330: 2d61 6c69 676e 3a20 6365 6e74 6572 3b0a  -align: center;.
+0004f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004f350: 7d0a 2020 2020 2020 2020 2020 2020 3c2f  }.            </
+0004f360: 7374 796c 653e 0a20 2020 2020 2020 203c  style>.        <
+0004f370: 2f68 6561 643e 0a20 2020 2022 2222 0a20  /head>.    """. 
+0004f380: 2020 2074 6162 6c65 5f68 746d 6c20 3d20     table_html = 
+0004f390: 280a 2020 2020 2020 2020 2868 6561 6465  (.        (heade
+0004f3a0: 7220 2b20 6874 6d6c 290a 2020 2020 2020  r + html).      
+0004f3b0: 2020 2e72 6570 6c61 6365 2822 2667 743b    .replace("&gt;
+0004f3c0: 222c 2022 3e22 290a 2020 2020 2020 2020  ", ">").        
+0004f3d0: 2e72 6570 6c61 6365 2822 266c 743b 222c  .replace("&lt;",
+0004f3e0: 2022 3c22 290a 2020 2020 2020 2020 2e72   "<").        .r
+0004f3f0: 6570 6c61 6365 2822 2661 6d70 3b22 2c20  eplace("&amp;", 
+0004f400: 2226 2229 0a20 2020 2029 0a20 2020 2072  "&").    ).    r
+0004f410: 6574 7572 6e20 7461 626c 655f 6874 6d6c  eturn table_html
+0004f420: 0a0a 0a64 6566 2062 6573 745f 7465 7874  ...def best_text
+0004f430: 5f63 6f6c 6f72 2872 6564 2c20 6772 6565  _color(red, gree
+0004f440: 6e2c 2062 6c75 6529 3a0a 2020 2020 6966  n, blue):.    if
+0004f450: 2028 7265 6420 2a20 302e 3239 3920 2b20   (red * 0.299 + 
+0004f460: 6772 6565 6e20 2a20 302e 3538 3720 2b20  green * 0.587 + 
+0004f470: 626c 7565 202a 2030 2e31 3134 2920 3e20  blue * 0.114) > 
+0004f480: 3138 363a 0a20 2020 2020 2020 2072 6574  186:.        ret
+0004f490: 7572 6e20 2262 6c61 636b 220a 2020 2020  urn "black".    
+0004f4a0: 7265 7475 726e 2022 7768 6974 6522 0a0a  return "white"..
+0004f4b0: 0a64 6566 2067 6574 5f63 6f6c 6f72 6564  .def get_colored
+0004f4c0: 5f72 6f69 5f73 7472 696e 6728 726f 692c  _roi_string(roi,
+0004f4d0: 2067 7265 793d 4661 6c73 652c 2063 6f6c   grey=False, col
+0004f4e0: 6f72 3d4e 6f6e 6529 3a0a 2020 2020 2222  or=None):.    ""
+0004f4f0: 2247 6574 2052 4f49 206e 616d 6520 696e  "Get ROI name in
+0004f500: 2048 544d 4c20 7769 7468 2062 6163 6b67   HTML with backg
+0004f510: 726f 756e 6420 636f 6c6f 7220 6672 6f6d  round color from
+0004f520: 2072 6f69 2e63 6f6c 6f72 2e20 4966 2067   roi.color. If g
+0004f530: 7265 793d 5472 7565 2c0a 2020 2020 7468  rey=True,.    th
+0004f540: 6520 6261 636b 6772 6f75 6e64 2063 6f6c  e background col
+0004f550: 6f72 2077 696c 6c20 6265 2067 7265 792e  or will be grey.
+0004f560: 2222 220a 0a20 2020 2069 6620 636f 6c6f  """..    if colo
+0004f570: 7220 6973 204e 6f6e 653a 0a20 2020 2020  r is None:.     
+0004f580: 2020 2063 6f6c 6f72 203d 2072 6f69 2e63     color = roi.c
+0004f590: 6f6c 6f72 0a20 2020 2069 6620 6772 6579  olor.    if grey
+0004f5a0: 3a0a 2020 2020 2020 2020 7265 642c 2067  :.        red, g
+0004f5b0: 7265 656e 2c20 626c 7565 203d 2032 3535  reen, blue = 255
+0004f5c0: 2c20 3235 352c 2032 3535 0a20 2020 2020  , 255, 255.     
+0004f5d0: 2020 2072 6564 2c20 6772 6565 6e2c 2062     red, green, b
+0004f5e0: 6c75 6520 3d20 3132 382c 2031 3238 2c20  lue = 128, 128, 
+0004f5f0: 3132 380a 2020 2020 2020 2020 7465 7874  128.        text
+0004f600: 5f63 6f6c 203d 2032 3030 2c20 3230 302c  _col = 200, 200,
+0004f610: 2032 3030 0a20 2020 2020 2020 2023 2041   200.        # A
+0004f620: 766f 6964 2073 6574 7469 6e67 2063 6f6c  void setting col
+0004f630: 6f75 7220 666f 7220 6772 6579 6564 206f  our for greyed o
+0004f640: 7574 2052 4f49 732e 0a20 2020 2020 2020  ut ROIs..       
+0004f650: 2023 2054 6869 7320 6769 7665 7320 676f   # This gives go
+0004f660: 6f64 2072 6561 6461 6269 6c69 7479 2066  od readability f
+0004f670: 6f72 2062 6f74 6820 6461 726b 2061 6e64  or both dark and
+0004f680: 206c 6967 6874 2074 6865 6d65 732e 0a20   light themes.. 
+0004f690: 2020 2020 2020 2072 6574 7572 6e20 2827         return ('
+0004f6a0: 3c70 3e26 6e62 7370 3b7b 7d26 6e62 7370  <p>&nbsp;{}&nbsp
+0004f6b0: 3b3c 2f70 3e27 292e 666f 726d 6174 2872  ;</p>').format(r
+0004f6c0: 6f69 2e6e 616d 6529 0a20 2020 2065 6c73  oi.name).    els
+0004f6d0: 653a 0a20 2020 2020 2020 2072 6564 2c20  e:.        red, 
+0004f6e0: 6772 6565 6e2c 2062 6c75 6520 3d20 5b63  green, blue = [c
+0004f6f0: 202a 2032 3535 2066 6f72 2063 2069 6e20   * 255 for c in 
+0004f700: 636f 6c6f 725b 3a33 5d5d 0a20 2020 2020  color[:3]].     
+0004f710: 2020 2074 6578 745f 636f 6c20 3d20 6265     text_col = be
+0004f720: 7374 5f74 6578 745f 636f 6c6f 7228 7265  st_text_color(re
+0004f730: 642c 2067 7265 656e 2c20 626c 7565 290a  d, green, blue).
+0004f740: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+0004f750: 2020 2020 2027 3c70 2073 7479 6c65 3d22       '<p style="
+0004f760: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
+0004f770: 3a20 7267 6228 7b7d 2c20 7b7d 2c20 7b7d  : rgb({}, {}, {}
+0004f780: 293b 2027 0a20 2020 2020 2020 2027 636f  ); '.        'co
+0004f790: 6c6f 723a 207b 7d3b 223e 266e 6273 703b  lor: {};">&nbsp;
+0004f7a0: 7b7d 266e 6273 703b 3c2f 703e 270a 2020  {}&nbsp;</p>'.  
+0004f7b0: 2020 292e 666f 726d 6174 2872 6564 2c20    ).format(red, 
+0004f7c0: 6772 6565 6e2c 2062 6c75 652c 2074 6578  green, blue, tex
+0004f7d0: 745f 636f 6c2c 2072 6f69 2e6e 616d 6529  t_col, roi.name)
+0004f7e0: 0a0a 6465 6620 636f 6d70 6172 655f 726f  ..def compare_ro
+0004f7f0: 695f 7061 6972 7328 0a20 2020 2070 6169  i_pairs(.    pai
+0004f800: 7273 2c20 0a20 2020 2068 746d 6c3d 4661  rs, .    html=Fa
+0004f810: 6c73 652c 0a20 2020 206e 616d 655f 6173  lse,.    name_as
+0004f820: 5f69 6e64 6578 3d54 7275 652c 0a20 2020  _index=True,.   
+0004f830: 2067 7265 7965 645f 6f75 743d 4e6f 6e65   greyed_out=None
+0004f840: 2c0a 2020 2020 636f 6c6f 7265 643d 4661  ,.    colored=Fa
+0004f850: 6c73 652c 0a20 2020 2072 6f69 5f6b 7761  lse,.    roi_kwa
+0004f860: 7267 733d 7b7d 2c0a 2020 2020 2a2a 6b77  rgs={},.    **kw
+0004f870: 6172 6773 0a29 3a0a 2020 2020 6966 2068  args.):.    if h
+0004f880: 746d 6c3a 0a20 2020 2020 2020 206e 616d  tml:.        nam
+0004f890: 655f 6173 5f69 6e64 6578 203d 2046 616c  e_as_index = Fal
+0004f8a0: 7365 0a20 2020 2069 6620 6772 6579 6564  se.    if greyed
+0004f8b0: 5f6f 7574 2069 7320 4e6f 6e65 3a0a 2020  _out is None:.  
+0004f8c0: 2020 2020 2020 6772 6579 6564 5f6f 7574        greyed_out
+0004f8d0: 203d 205b 5d0a 2020 2020 6466 7320 3d20   = [].    dfs = 
+0004f8e0: 5b5d 0a20 2020 2066 6f72 2072 6f69 312c  [].    for roi1,
+0004f8f0: 2072 6f69 3220 696e 2070 6169 7273 3a0a   roi2 in pairs:.
+0004f900: 0a20 2020 2020 2020 2023 2047 6574 2044  .        # Get D
+0004f910: 6174 6146 7261 6d65 2066 6f72 2074 6869  ataFrame for thi
+0004f920: 7320 7061 6972 0a20 2020 2020 2020 2064  s pair.        d
+0004f930: 665f 726f 7720 3d20 726f 6931 2e67 6574  f_row = roi1.get
+0004f940: 5f63 6f6d 7061 7269 736f 6e28 726f 6932  _comparison(roi2
+0004f950: 2c20 6e61 6d65 5f61 735f 696e 6465 783d  , name_as_index=
+0004f960: 6e61 6d65 5f61 735f 696e 6465 782c 0a20  name_as_index,. 
+0004f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004f990: 2020 2020 2a2a 6b77 6172 6773 290a 0a20      **kwargs).. 
+0004f9a0: 2020 2020 2020 2023 2052 6570 6c61 6365         # Replace
+0004f9b0: 2076 616c 7565 7320 7769 7468 2022 2d2d   values with "--
+0004f9c0: 2220 6966 2065 6974 6865 7220 524f 4920  " if either ROI 
+0004f9d0: 6973 2067 7265 7965 6420 6f75 740a 2020  is greyed out.  
+0004f9e0: 2020 2020 2020 6772 6579 203d 2072 6f69        grey = roi
+0004f9f0: 3120 696e 2067 7265 7965 645f 6f75 7420  1 in greyed_out 
+0004fa00: 6f72 2072 6f69 3220 696e 2067 7265 7965  or roi2 in greye
+0004fa10: 645f 6f75 740a 2020 2020 2020 2020 6966  d_out.        if
+0004fa20: 2067 7265 793a 0a20 2020 2020 2020 2020   grey:.         
+0004fa30: 2020 2066 6f72 2063 6f6c 2069 6e20 6466     for col in df
+0004fa40: 5f72 6f77 2e63 6f6c 756d 6e73 3a0a 2020  _row.columns:.  
+0004fa50: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0004fa60: 2063 6f6c 203d 3d20 2252 4f49 223a 200a   col == "ROI": .
+0004fa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0004fa80: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+0004fa90: 2020 2020 2020 2020 2020 2020 2064 665f               df_
+0004faa0: 726f 775b 636f 6c5d 203d 2022 2d2d 220a  row[col] = "--".
+0004fab0: 0a20 2020 2020 2020 2023 2041 646a 7573  .        # Adjus
+0004fac0: 7420 636f 6d70 6172 6973 6f6e 206e 616d  t comparison nam
+0004fad0: 650a 2020 2020 2020 2020 636f 6d70 5f6e  e.        comp_n
+0004fae0: 616d 6520 3d20 726f 6931 2e67 6574 5f63  ame = roi1.get_c
+0004faf0: 6f6d 7061 7269 736f 6e5f 6e61 6d65 2872  omparison_name(r
+0004fb00: 6f69 322c 2063 6f6c 6f72 6564 3d63 6f6c  oi2, colored=col
+0004fb10: 6f72 6564 2c20 6772 6579 3d67 7265 792c  ored, grey=grey,
+0004fb20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0004fb30: 2072 6f69 5f6b 7761 7267 733d 726f 695f   roi_kwargs=roi_
+0004fb40: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
+0004fb50: 6966 206e 616d 655f 6173 5f69 6e64 6578  if name_as_index
+0004fb60: 3a0a 2020 2020 2020 2020 2020 2020 6466  :.            df
+0004fb70: 5f72 6f77 2e72 656e 616d 6528 7b64 665f  _row.rename({df_
+0004fb80: 726f 772e 696e 6465 785b 305d 3a20 636f  row.index[0]: co
+0004fb90: 6d70 5f6e 616d 657d 2c20 696e 706c 6163  mp_name}, inplac
+0004fba0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+0004fbb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0004fbc0: 2020 6466 5f72 6f77 2e69 6c6f 635b 302c    df_row.iloc[0,
+0004fbd0: 2030 5d20 3d20 636f 6d70 5f6e 616d 650a   0] = comp_name.
+0004fbe0: 0a20 2020 2020 2020 2064 6673 2e61 7070  .        dfs.app
+0004fbf0: 656e 6428 6466 5f72 6f77 290a 0a20 2020  end(df_row)..   
+0004fc00: 2069 676e 6f72 655f 696e 6465 7820 3d20   ignore_index = 
+0004fc10: 4661 6c73 6520 6966 206e 616d 655f 6173  False if name_as
+0004fc20: 5f69 6e64 6578 2065 6c73 6520 5472 7565  _index else True
+0004fc30: 0a20 2020 2064 6620 3d20 7064 2e63 6f6e  .    df = pd.con
+0004fc40: 6361 7428 6466 732c 2069 676e 6f72 655f  cat(dfs, ignore_
+0004fc50: 696e 6465 783d 6967 6e6f 7265 5f69 6e64  index=ignore_ind
+0004fc60: 6578 2920 6966 2064 6673 2065 6c73 6520  ex) if dfs else 
+0004fc70: 4e6f 6e65 0a20 2020 2069 6620 6874 6d6c  None.    if html
+0004fc80: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0004fc90: 2064 665f 746f 5f68 746d 6c28 6466 290a   df_to_html(df).
+0004fca0: 2020 2020 7265 7475 726e 2064 660a 0a64      return df..d
+0004fcb0: 6566 2067 6574 5f63 6f6e 666f 726d 6974  ef get_conformit
+0004fcc0: 795f 696e 6465 7828 0a20 2020 2072 6f69  y_index(.    roi
+0004fcd0: 732c 0a20 2020 2063 695f 7479 7065 3d22  s,.    ci_type="
+0004fce0: 6765 6e22 2c0a 2020 2020 7369 6e67 6c65  gen",.    single
+0004fcf0: 5f73 6c69 6365 3d46 616c 7365 2c0a 2020  _slice=False,.  
+0004fd00: 2020 7669 6577 3d22 782d 7922 2c20 0a20    view="x-y", . 
+0004fd10: 2020 2073 6c3d 4e6f 6e65 2c20 0a20 2020     sl=None, .   
+0004fd20: 2069 6478 3d4e 6f6e 652c 200a 2020 2020   idx=None, .    
+0004fd30: 706f 733d 4e6f 6e65 2c20 0a20 2020 206d  pos=None, .    m
+0004fd40: 6574 686f 643d 4e6f 6e65 2c0a 2020 2020  ethod=None,.    
+0004fd50: 666c 6174 7465 6e3d 4661 6c73 652c 0a20  flatten=False,. 
+0004fd60: 2020 2029 3a0a 2020 2020 2222 220a 2020     ):.    """.  
+0004fd70: 2020 4765 7420 636f 6e66 6f72 6d69 7479    Get conformity
+0004fd80: 2069 6e64 6578 2066 6f72 2074 776f 206f   index for two o
+0004fd90: 7220 6d6f 7265 2052 4f49 732e 0a0a 2020  r more ROIs...  
+0004fda0: 2020 5468 6520 636f 6e66 6f72 6d69 7479    The conformity
+0004fdb0: 2069 6e64 6578 206d 6179 2062 6520 6361   index may be ca
+0004fdc0: 6c63 756c 6174 6564 2067 6c6f 6261 6c6c  lculated globall
+0004fdd0: 7920 6f72 2066 6f72 2061 2073 696e 676c  y or for a singl
+0004fde0: 6520 736c 6963 652e 0a0a 2020 2020 5468  e slice...    Th
+0004fdf0: 6973 2066 756e 6374 696f 6e20 7265 7475  is function retu
+0004fe00: 726e 7320 6569 7468 6572 2074 6865 2076  rns either the v
+0004fe10: 616c 7565 206f 6620 6f6e 6520 6f66 2074  alue of one of t
+0004fe20: 6865 2074 6872 6565 2074 7970 6573 0a20  he three types. 
+0004fe30: 2020 206f 6620 636f 6e66 6f72 6d69 7479     of conformity
+0004fe40: 2069 6e64 6578 2028 2267 656e 2220 2866   index ("gen" (f
+0004fe50: 6f72 2067 656e 6572 616c 6973 6564 292c  or generalised),
+0004fe60: 2022 7061 6972 7322 2c20 2263 6f6d 6d6f   "pairs", "commo
+0004fe70: 6e22 290a 2020 2020 7265 6665 7272 6564  n").    referred
+0004fe80: 2074 6f20 696e 3a0a 2020 2020 6874 7470   to in:.    http
+0004fe90: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
+0004fea0: 3038 382f 3030 3331 2d39 3135 352f 3534  088/0031-9155/54
+0004feb0: 2f39 2f30 3138 0a20 2020 206f 7220 6120  /9/018.    or a 
+0004fec0: 736b 7274 2e63 6f72 652e 4461 7461 206f  skrt.core.Data o
+0004fed0: 626a 6563 7420 7769 7468 2074 6865 2076  bject with the v
+0004fee0: 616c 7565 7320 6f66 2061 6c6c 2074 6872  alues of all thr
+0004fef0: 6565 2e0a 2020 2020 466f 7220 7468 6520  ee..    For the 
+0004ff00: 6361 7365 206f 6620 7477 6f20 524f 4973  case of two ROIs
+0004ff10: 2c20 7468 6520 7468 7265 6520 6d65 7472  , the three metr
+0004ff20: 6963 7320 6172 6520 616c 6c20 6571 7569  ics are all equi
+0004ff30: 7661 6c65 6e74 0a20 2020 2074 6f20 7468  valent.    to th
+0004ff40: 6520 4a61 6363 6172 6420 636f 6e66 6f72  e Jaccard confor
+0004ff50: 6d69 7479 2069 6e64 6578 2e0a 0a20 2020  mity index...   
+0004ff60: 202a 2a50 6172 616d 6574 6572 733a 2a2a   **Parameters:**
+0004ff70: 0a20 2020 2020 2020 200a 2020 2020 726f  .        .    ro
+0004ff80: 6973 203a 206c 6973 740a 2020 2020 2020  is : list.      
+0004ff90: 2020 4c69 7374 206f 6620 7477 6f20 6f72    List of two or
+0004ffa0: 206d 6f72 6520 736b 7274 2e73 7472 7563   more skrt.struc
+0004ffb0: 7475 7265 732e 524f 4920 6f62 6a65 6374  tures.ROI object
+0004ffc0: 7320 666f 7220 7768 6963 6820 636f 6e66  s for which conf
+0004ffd0: 6f72 6d69 7479 0a20 2020 2020 2020 2069  ormity.        i
+0004ffe0: 6e64 6578 2069 7320 746f 2062 6520 6361  ndex is to be ca
+0004fff0: 6c63 756c 6174 6564 2e0a 0a20 2020 2063  lculated...    c
+00050000: 695f 7479 7065 3a20 7374 722c 2064 6566  i_type: str, def
+00050010: 6175 6c74 3d22 6765 6e22 0a20 2020 2020  ault="gen".     
+00050020: 2020 2054 7970 6520 6f66 2063 6f6e 666f     Type of confo
+00050030: 726d 6974 7920 696e 6465 7820 746f 2062  rmity index to b
+00050040: 6520 7265 7475 726e 6564 2c20 6672 6f6d  e returned, from
+00050050: 2022 6765 6e22 2028 666f 7220 6765 6e65   "gen" (for gene
+00050060: 7261 6c69 7365 6429 2c0a 2020 2020 2020  ralised),.      
+00050070: 2020 2270 6169 7273 222c 2022 636f 6d6d    "pairs", "comm
+00050080: 6f6e 222e 2020 4966 2073 6574 2074 6f20  on".  If set to 
+00050090: 2261 6c6c 222c 2061 2073 6b72 742e 636f  "all", a skrt.co
+000500a0: 7265 2e44 6174 6120 6f62 6a65 6374 2077  re.Data object w
+000500b0: 6974 680a 2020 2020 2020 2020 7661 6c75  ith.        valu
+000500c0: 6573 2066 6f72 2074 6865 2074 6872 6565  es for the three
+000500d0: 2074 7970 6573 206f 6620 636f 6e66 6f72   types of confor
+000500e0: 6d69 7479 2069 6e64 6578 2069 7320 7265  mity index is re
+000500f0: 7475 726e 6564 2e0a 0a20 2020 2073 696e  turned...    sin
+00050100: 676c 655f 736c 6963 6520 3a20 626f 6f6c  gle_slice : bool
+00050110: 2c20 6465 6661 756c 743d 4661 6c73 650a  , default=False.
+00050120: 2020 2020 2020 2020 4966 2046 616c 7365          If False
+00050130: 2c20 7468 6520 676c 6f62 616c 2033 4420  , the global 3D 
+00050140: 4469 6365 2073 636f 7265 206f 6620 7468  Dice score of th
+00050150: 6520 6675 6c6c 2052 4f49 7320 7769 6c6c  e full ROIs will
+00050160: 2062 6520 7265 7475 726e 6564 3b0a 2020   be returned;.  
+00050170: 2020 2020 2020 6f74 6865 7277 6973 652c        otherwise,
+00050180: 2074 6865 2032 4420 4469 6365 2073 636f   the 2D Dice sco
+00050190: 7265 206f 6e20 6120 7369 6e67 6c65 2073  re on a single s
+000501a0: 6c69 6365 2077 696c 6c20 6265 2072 6574  lice will be ret
+000501b0: 7572 6e65 642e 0a0a 2020 2020 7669 6577  urned...    view
+000501c0: 203a 2073 7472 2c20 6465 6661 756c 743d   : str, default=
+000501d0: 2278 2d79 220a 2020 2020 2020 2020 4f72  "x-y".        Or
+000501e0: 6965 6e74 6174 696f 6e20 6f66 2073 6c69  ientation of sli
+000501f0: 6365 206f 6e20 7768 6963 6820 746f 2067  ce on which to g
+00050200: 6574 2044 6963 6520 7363 6f72 652e 204f  et Dice score. O
+00050210: 6e6c 7920 7573 6564 2069 6620 0a20 2020  nly used if .   
+00050220: 2020 2020 2073 696e 676c 655f 736c 6963       single_slic
+00050230: 653d 5472 7565 2e20 4966 2075 7369 6e67  e=True. If using
+00050240: 2c20 3c61 783e 206d 7573 7420 6265 2061  , <ax> must be a
+00050250: 6e20 6178 6973 2074 6861 7420 6c69 6573  n axis that lies
+00050260: 2061 6c6f 6e67 0a20 2020 2020 2020 2074   along.        t
+00050270: 6865 2073 6c69 6365 2069 6e20 7468 6973  he slice in this
+00050280: 206f 7269 656e 7461 7469 6f6e 2e0a 0a20   orientation... 
+00050290: 2020 2073 6c20 3a20 696e 742c 2064 6566     sl : int, def
+000502a0: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
+000502b0: 2020 536c 6963 6520 6e75 6d62 6572 2e20    Slice number. 
+000502c0: 4966 206e 6f6e 6520 6f66 203c 736c 3e2c  If none of <sl>,
+000502d0: 203c 6964 783e 206f 7220 3c70 6f73 3e20   <idx> or <pos> 
+000502e0: 6172 6520 7375 7070 6c69 6564 2062 7574  are supplied but
+000502f0: 0a20 2020 2020 2020 203c 7369 6e67 6c65  .        <single
+00050300: 5f73 6c69 6365 3e20 6973 2054 7275 652c  _slice> is True,
+00050310: 2074 6865 2063 656e 7472 616c 2073 6c69   the central sli
+00050320: 6365 206f 6620 7468 6973 2052 4f49 2077  ce of this ROI w
+00050330: 696c 6c20 6265 2075 7365 642e 0a0a 2020  ill be used...  
+00050340: 2020 6964 7820 3a20 696e 742c 2064 6566    idx : int, def
+00050350: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
+00050360: 2020 4172 7261 7920 696e 6465 7820 6f66    Array index of
+00050370: 2073 6c69 6365 2e20 4966 206e 6f6e 6520   slice. If none 
+00050380: 6f66 203c 736c 3e2c 203c 6964 783e 206f  of <sl>, <idx> o
+00050390: 7220 3c70 6f73 3e20 6172 6520 7375 7070  r <pos> are supp
+000503a0: 6c69 6564 2062 7574 0a20 2020 2020 2020  lied but.       
+000503b0: 203c 7369 6e67 6c65 5f73 6c69 6365 3e20   <single_slice> 
+000503c0: 6973 2054 7275 652c 2074 6865 2063 656e  is True, the cen
+000503d0: 7472 616c 2073 6c69 6365 206f 6620 7468  tral slice of th
+000503e0: 6973 2052 4f49 2077 696c 6c20 6265 2075  is ROI will be u
+000503f0: 7365 642e 0a0a 2020 2020 706f 7320 3a20  sed...    pos : 
+00050400: 666c 6f61 742c 2064 6566 6175 6c74 3d4e  float, default=N
+00050410: 6f6e 650a 2020 2020 2020 2020 536c 6963  one.        Slic
+00050420: 6520 706f 7369 7469 6f6e 2069 6e20 6d6d  e position in mm
+00050430: 2e20 4966 206e 6f6e 6520 6f66 203c 736c  . If none of <sl
+00050440: 3e2c 203c 6964 783e 206f 7220 3c70 6f73  >, <idx> or <pos
+00050450: 3e20 6172 6520 7375 7070 6c69 6564 2062  > are supplied b
+00050460: 7574 0a20 2020 2020 2020 203c 7369 6e67  ut.        <sing
+00050470: 6c65 5f73 6c69 6365 3e20 6973 2054 7275  le_slice> is Tru
+00050480: 652c 2074 6865 2063 656e 7472 616c 2073  e, the central s
+00050490: 6c69 6365 206f 6620 7468 6973 2052 4f49  lice of this ROI
+000504a0: 2077 696c 6c20 6265 2075 7365 642e 0a0a   will be used...
+000504b0: 2020 2020 6d65 7468 6f64 203a 2073 7472      method : str
+000504c0: 2c20 6465 6661 756c 743d 4e6f 6e65 0a20  , default=None. 
+000504d0: 2020 2020 2020 204d 6574 686f 6420 746f         Method to
+000504e0: 2075 7365 2066 6f72 2044 6963 6520 7363   use for Dice sc
+000504f0: 6f72 6520 6361 6c63 756c 6174 696f 6e2e  ore calculation.
+00050500: 2043 616e 2062 653a 200a 2020 2020 2020   Can be: .      
+00050510: 2020 2d20 2263 6f6e 746f 7572 223a 2067    - "contour": g
+00050520: 6574 2069 6e74 6572 7365 6374 696f 6e73  et intersections
+00050530: 2061 6e64 2061 7265 6173 206f 6620 7368   and areas of sh
+00050540: 6170 656c 7920 636f 6e74 6f75 7273 2e0a  apely contours..
+00050550: 2020 2020 2020 2020 2d20 226d 6173 6b22          - "mask"
+00050560: 3a20 636f 756e 7420 696e 7465 7273 6563  : count intersec
+00050570: 7469 6e67 2076 6f78 656c 7320 696e 2062  ting voxels in b
+00050580: 696e 6172 7920 6d61 736b 732e 0a20 2020  inary masks..   
+00050590: 2020 2020 202d 204e 6f6e 653a 2075 7365       - None: use
+000505a0: 2074 6865 206d 6574 686f 6420 7365 7420   the method set 
+000505b0: 696e 2073 656c 662e 6465 6661 756c 745f  in self.default_
+000505c0: 6765 6f6d 5f6d 6574 686f 642e 0a20 2020  geom_method..   
+000505d0: 2020 2020 2046 6f72 206d 6f72 6520 7468       For more th
+000505e0: 616e 2074 776f 2052 4f49 7320 616e 6420  an two ROIs and 
+000505f0: 3c63 695f 7479 7065 3e20 2263 6f6d 6d6f  <ci_type> "commo
+00050600: 6e22 2c20 6f6e 6c79 2074 6865 2022 6d61  n", only the "ma
+00050610: 736b 220a 2020 2020 2020 2020 6d65 7468  sk".        meth
+00050620: 6f64 2069 7320 696d 706c 656d 656e 7465  od is implemente
+00050630: 642e 0a0a 2020 2020 666c 6174 7465 6e20  d...    flatten 
+00050640: 3a20 626f 6f6c 2c20 6465 6661 756c 743d  : bool, default=
+00050650: 4661 6c73 650a 2020 2020 2020 2020 4966  False.        If
+00050660: 2054 7275 652c 2061 6c6c 2073 6c69 6365   True, all slice
+00050670: 7320 7769 6c6c 2062 6520 666c 6174 7465  s will be flatte
+00050680: 6e65 6420 696e 2074 6865 2067 6976 656e  ned in the given
+00050690: 206f 7269 656e 7461 7469 6f6e 2061 6e64   orientation and
+000506a0: 0a20 2020 2020 2020 2074 6865 2044 6963  .        the Dic
+000506b0: 6520 7363 6f72 6520 6f66 2074 6865 2066  e score of the f
+000506c0: 6c61 7474 656e 6564 2073 6c69 6365 7320  lattened slices 
+000506d0: 7769 6c6c 2062 6520 7265 7475 726e 6564  will be returned
+000506e0: 2e20 4f6e 6c79 200a 2020 2020 2020 2020  . Only .        
+000506f0: 6176 6169 6c61 626c 6520 6966 206d 6574  available if met
+00050700: 686f 643d 226d 6173 6b22 2e0a 2020 2020  hod="mask"..    
+00050710: 2222 220a 0a20 2020 2023 2052 6571 7569  """..    # Requi
+00050720: 7265 2076 616c 6964 2069 6e70 7574 732e  re valid inputs.
+00050730: 0a20 2020 2069 6620 6c65 6e28 726f 6973  .    if len(rois
+00050740: 2920 3c20 3220 6f72 2063 695f 7479 7065  ) < 2 or ci_type
+00050750: 206e 6f74 2069 6e20 5b22 636f 6d6d 6f6e   not in ["common
+00050760: 222c 2022 6765 6e22 2c20 2270 6169 7273  ", "gen", "pairs
+00050770: 222c 2022 616c 6c22 5d3a 0a20 2020 2020  ", "all"]:.     
+00050780: 2020 2072 6574 7572 6e0a 0a20 2020 2023     return..    #
+00050790: 2049 6e69 7469 616c 6973 6520 4461 7461   Initialise Data
+000507a0: 206f 626a 6563 7420 666f 7220 636f 6e66   object for conf
+000507b0: 6f72 6d69 7479 2069 6e64 6963 6573 2e0a  ormity indices..
+000507c0: 2020 2020 6369 203d 2073 6b72 742e 636f      ci = skrt.co
+000507d0: 7265 2e44 6174 6128 7b22 636f 6d6d 6f6e  re.Data({"common
+000507e0: 223a 2030 2c20 2267 656e 223a 302c 2022  ": 0, "gen":0, "
+000507f0: 7061 6972 7322 3a30 7d29 0a0a 2020 2020  pairs":0})..    
+00050800: 2320 4465 616c 2077 6974 6820 6361 7365  # Deal with case
+00050810: 7320 2267 656e 2220 616e 6420 2270 6169  s "gen" and "pai
+00050820: 7273 222e 0a20 2020 2023 0a20 2020 2023  rs"..    #.    #
+00050830: 2046 6f72 2022 6765 6e22 2c20 7468 6520   For "gen", the 
+00050840: 636f 6e66 6f72 6d69 7479 2069 6e64 6578  conformity index
+00050850: 2069 7320 6361 6c63 756c 6174 6564 2061   is calculated a
+00050860: 7320 7468 6520 7261 7469 6f20 6f66 0a20  s the ratio of. 
+00050870: 2020 2023 2028 3129 2074 6865 2073 756d     # (1) the sum
+00050880: 206f 6620 7468 6520 696e 7465 7273 6563   of the intersec
+00050890: 7469 6f6e 7320 666f 7220 616c 6c20 7061  tions for all pa
+000508a0: 6972 7320 746f 2028 3229 2074 6865 2073  irs to (2) the s
+000508b0: 756d 206f 660a 2020 2020 2320 7468 6520  um of.    # the 
+000508c0: 756e 696f 6e73 2066 6f72 2061 6c6c 2070  unions for all p
+000508d0: 6169 7273 2e0a 2020 2020 230a 2020 2020  airs..    #.    
+000508e0: 2320 466f 7220 2270 6169 7273 2c20 7468  # For "pairs, th
+000508f0: 6520 636f 6e66 6f72 6d69 7479 2069 6e64  e conformity ind
+00050900: 6578 2069 7320 6361 6c63 7561 6c74 6564  ex is calcualted
+00050910: 2061 7320 7468 6520 6d65 616e 206f 6620   as the mean of 
+00050920: 7468 650a 2020 2020 2320 4a61 6363 6172  the.    # Jaccar
+00050930: 6420 636f 6e66 6f72 6d69 7479 2069 6e64  d conformity ind
+00050940: 6963 6573 2066 6f72 2061 6c6c 2070 6169  ices for all pai
+00050950: 7273 2e0a 0a20 2020 206e 756d 6572 6174  rs...    numerat
+00050960: 6f72 203d 2030 0a20 2020 2064 656e 6f6d  or = 0.    denom
+00050970: 696e 6174 6f72 203d 2030 0a20 2020 206e  inator = 0.    n
+00050980: 5f70 6169 7220 3d20 300a 2020 2020 666f  _pair = 0.    fo
+00050990: 7220 6964 7831 2069 6e20 7261 6e67 6528  r idx1 in range(
+000509a0: 6c65 6e28 726f 6973 2920 2d20 3129 3a0a  len(rois) - 1):.
+000509b0: 2020 2020 2020 2020 666f 7220 6964 7832          for idx2
+000509c0: 2069 6e20 7261 6e67 6528 6964 7831 202b   in range(idx1 +
+000509d0: 2031 2c20 6c65 6e28 726f 6973 2929 3a0a   1, len(rois)):.
+000509e0: 2020 2020 2020 2020 2020 2020 726f 6931              roi1
+000509f0: 203d 2072 6f69 735b 6964 7831 5d0a 2020   = rois[idx1].  
+00050a00: 2020 2020 2020 2020 2020 726f 6932 203d            roi2 =
+00050a10: 2072 6f69 735b 6964 7832 5d0a 2020 2020   rois[idx2].    
+00050a20: 2020 2020 2020 2020 696e 7465 7273 6563          intersec
+00050a30: 7469 6f6e 2c20 756e 696f 6e2c 206d 6561  tion, union, mea
+00050a40: 6e5f 7369 7a65 203d 2028 0a20 2020 2020  n_size = (.     
+00050a50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00050a60: 6f69 312e 6765 745f 696e 7465 7273 6563  oi1.get_intersec
+00050a70: 7469 6f6e 5f75 6e69 6f6e 5f73 697a 6528  tion_union_size(
+00050a80: 726f 6932 2c20 7369 6e67 6c65 5f73 6c69  roi2, single_sli
+00050a90: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+00050aa0: 2020 2020 2020 2020 2020 2020 7669 6577              view
+00050ab0: 2c20 736c 2c20 6964 782c 2070 6f73 2c20  , sl, idx, pos, 
+00050ac0: 6d65 7468 6f64 2c20 666c 6174 7465 6e29  method, flatten)
+00050ad0: 290a 2020 2020 2020 2020 2020 2020 6e75  ).            nu
+00050ae0: 6d65 7261 746f 7220 2b3d 2069 6e74 6572  merator += inter
+00050af0: 7365 6374 696f 6e0a 2020 2020 2020 2020  section.        
+00050b00: 2020 2020 6465 6e6f 6d69 6e61 746f 7220      denominator 
+00050b10: 2b3d 2075 6e69 6f6e 0a20 2020 2020 2020  += union.       
+00050b20: 2020 2020 2063 692e 7061 6972 7320 2b3d       ci.pairs +=
+00050b30: 2069 6e74 6572 7365 6374 696f 6e20 2f20   intersection / 
+00050b40: 756e 696f 6e0a 2020 2020 2020 2020 2020  union.          
+00050b50: 2020 6e5f 7061 6972 202b 3d20 310a 0a20    n_pair += 1.. 
+00050b60: 2020 2063 692e 6765 6e20 3d20 6e75 6d65     ci.gen = nume
+00050b70: 7261 746f 7220 2f20 6465 6e6f 6d69 6e61  rator / denomina
+00050b80: 746f 720a 2020 2020 6369 2e70 6169 7273  tor.    ci.pairs
+00050b90: 202f 3d20 6e5f 7061 6972 0a0a 2020 2020   /= n_pair..    
+00050ba0: 2320 4465 616c 2077 6974 6820 6361 7365  # Deal with case
+00050bb0: 2022 636f 6d6d 6f6e 222e 0a20 2020 2023   "common"..    #
+00050bc0: 0a20 2020 2023 2054 6865 2063 6f6e 666f  .    # The confo
+00050bd0: 726d 6974 7920 696e 6465 7820 6973 2063  rmity index is c
+00050be0: 616c 6375 6c61 7465 6420 6173 2074 6865  alculated as the
+00050bf0: 2072 6174 696f 206f 660a 2020 2020 2320   ratio of.    # 
+00050c00: 2831 2920 7468 6520 636f 6d6d 6f6e 2069  (1) the common i
+00050c10: 6e74 6572 7365 6374 696f 6e20 6f66 2061  ntersection of a
+00050c20: 6c6c 2052 4f49 7320 746f 2028 3229 2074  ll ROIs to (2) t
+00050c30: 6865 2063 6f6d 6269 6e65 6420 756e 696f  he combined unio
+00050c40: 6e0a 2020 2020 2320 6f66 2061 6c6c 2052  n.    # of all R
+00050c50: 4f49 732e 0a20 2020 2069 6620 3220 3d3d  OIs..    if 2 ==
+00050c60: 206c 656e 2872 6f69 7329 3a0a 2020 2020   len(rois):.    
+00050c70: 2020 2020 696e 7465 7273 6563 7469 6f6e      intersection
+00050c80: 2c20 756e 696f 6e2c 206d 6561 6e5f 7369  , union, mean_si
+00050c90: 7a65 203d 2028 0a20 2020 2020 2020 2020  ze = (.         
+00050ca0: 2020 2020 2020 2072 6f69 735b 305d 2e67         rois[0].g
+00050cb0: 6574 5f69 6e74 6572 7365 6374 696f 6e5f  et_intersection_
+00050cc0: 756e 696f 6e5f 7369 7a65 2872 6f69 735b  union_size(rois[
+00050cd0: 315d 2c20 7369 6e67 6c65 5f73 6c69 6365  1], single_slice
+00050ce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00050cf0: 2020 2020 2020 2020 2020 7669 6577 2c20            view, 
+00050d00: 736c 2c20 6964 782c 2070 6f73 2c20 6d65  sl, idx, pos, me
+00050d10: 7468 6f64 2c20 666c 6174 7465 6e29 290a  thod, flatten)).
+00050d20: 2020 2020 2020 2020 6369 2e63 6f6d 6d6f          ci.commo
+00050d30: 6e20 3d20 696e 7465 7273 6563 7469 6f6e  n = intersection
+00050d40: 202f 2075 6e69 6f6e 0a20 2020 2065 6c73   / union.    els
+00050d50: 653a 0a20 2020 2020 2020 2069 6620 6e6f  e:.        if no
+00050d60: 7420 7369 6e67 6c65 5f73 6c69 6365 3a0a  t single_slice:.
+00050d70: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
+00050d80: 5f69 6e74 6572 7365 6374 696f 6e20 3d20  _intersection = 
+00050d90: 726f 6973 5b30 5d2e 636c 6f6e 6528 292e  rois[0].clone().
+00050da0: 6765 745f 6d61 736b 280a 2020 2020 2020  get_mask(.      
+00050db0: 2020 2020 2020 2020 2020 2020 2020 7669                vi
+00050dc0: 6577 2c20 666c 6174 7465 6e2c 2073 7461  ew, flatten, sta
+00050dd0: 6e64 6172 6469 7365 3d54 7275 6529 0a20  ndardise=True). 
+00050de0: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
+00050df0: 756e 696f 6e20 3d20 726f 6973 5b30 5d2e  union = rois[0].
+00050e00: 636c 6f6e 6528 292e 6765 745f 6d61 736b  clone().get_mask
+00050e10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00050e20: 2020 2020 2020 7669 6577 2c20 666c 6174        view, flat
+00050e30: 7465 6e2c 2073 7461 6e64 6172 6469 7365  ten, standardise
+00050e40: 3d54 7275 6529 0a20 2020 2020 2020 2065  =True).        e
+00050e50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00050e60: 206d 6173 6b5f 696e 7465 7273 6563 7469   mask_intersecti
+00050e70: 6f6e 203d 2072 6f69 735b 305d 2e63 6c6f  on = rois[0].clo
+00050e80: 6e65 2829 2e67 6574 5f73 6c69 6365 280a  ne().get_slice(.
+00050e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00050ea0: 2020 2020 7669 6577 2c20 736c 2c20 6964      view, sl, id
+00050eb0: 782c 2070 6f73 290a 2020 2020 2020 2020  x, pos).        
+00050ec0: 2020 2020 6d61 736b 5f75 6e69 6f6e 203d      mask_union =
+00050ed0: 2072 6f69 735b 305d 2e63 6c6f 6e65 2829   rois[0].clone()
+00050ee0: 2e67 6574 5f73 6c69 6365 2876 6965 772c  .get_slice(view,
+00050ef0: 2073 6c2c 2069 6478 2c20 706f 7329 0a0a   sl, idx, pos)..
+00050f00: 2020 2020 2020 2020 666f 7220 726f 6920          for roi 
+00050f10: 696e 2072 6f69 735b 313a 5d3a 0a20 2020  in rois[1:]:.   
+00050f20: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00050f30: 7369 6e67 6c65 5f73 6c69 6365 3a0a 2020  single_slice:.  
+00050f40: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00050f50: 736b 203d 2072 6f69 2e67 6574 5f6d 6173  sk = roi.get_mas
+00050f60: 6b28 7669 6577 2c20 666c 6174 7465 6e2c  k(view, flatten,
+00050f70: 2073 7461 6e64 6172 6469 7365 3d54 7275   standardise=Tru
+00050f80: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
+00050f90: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00050fa0: 2020 2020 206d 6173 6b20 3d20 726f 692e       mask = roi.
+00050fb0: 6765 745f 736c 6963 6528 7669 6577 2c20  get_slice(view, 
+00050fc0: 736c 2c20 6964 782c 2070 6f73 290a 0a20  sl, idx, pos).. 
+00050fd0: 2020 2020 2020 2020 2020 206d 6173 6b5f             mask_
+00050fe0: 696e 7465 7273 6563 7469 6f6e 203d 2028  intersection = (
+00050ff0: 6d61 736b 5f69 6e74 6572 7365 6374 696f  mask_intersectio
+00051000: 6e20 2620 6d61 736b 290a 2020 2020 2020  n & mask).      
+00051010: 2020 2020 2020 6d61 736b 5f75 6e69 6f6e        mask_union
+00051020: 203d 2028 6d61 736b 5f75 6e69 6f6e 207c   = (mask_union |
+00051030: 206d 6173 6b29 0a0a 2020 2020 2020 2020   mask)..        
+00051040: 6369 2e63 6f6d 6d6f 6e20 3d20 6d61 736b  ci.common = mask
+00051050: 5f69 6e74 6572 7365 6374 696f 6e2e 7375  _intersection.su
+00051060: 6d28 2920 2f20 6d61 736b 5f75 6e69 6f6e  m() / mask_union
+00051070: 2e73 756d 2829 0a0a 2020 2020 7265 7475  .sum()..    retu
+00051080: 726e 2067 6574 6174 7472 2863 692c 2063  rn getattr(ci, c
+00051090: 695f 7479 7065 2c20 6369 290a 0a64 6566  i_type, ci)..def
+000510a0: 2067 6574 5f72 6f69 5f73 6c69 6365 2872   get_roi_slice(r
+000510b0: 6f69 2c20 7a5f 6672 6163 7469 6f6e 3d31  oi, z_fraction=1
+000510c0: 2c20 7375 6666 6978 3d4e 6f6e 6529 3a0a  , suffix=None):.
+000510d0: 2020 2020 2222 220a 2020 2020 4765 7420      """.    Get 
+000510e0: 524f 4920 6f62 6a65 6374 2063 6f72 7265  ROI object corre
+000510f0: 7370 6f6e 6469 6e67 2074 6f20 782d 7920  sponding to x-y 
+00051100: 736c 6963 6520 7468 726f 7567 6820 696e  slice through in
+00051110: 7075 7420 524f 492e 0a0a 2020 2020 2a2a  put ROI...    **
+00051120: 5061 7261 6d65 7465 7273 3a2a 2a0a 0a20  Parameters:**.. 
+00051130: 2020 2072 6f69 203a 2073 6b72 742e 7374     roi : skrt.st
+00051140: 7275 6374 7572 6573 2e52 4f49 0a20 2020  ructures.ROI.   
+00051150: 2020 2020 2052 4f49 206f 626a 6563 7420       ROI object 
+00051160: 666f 7220 7768 6963 6820 736c 6963 6520  for which slice 
+00051170: 6973 2074 6f20 6265 206f 6274 6169 6e65  is to be obtaine
+00051180: 642e 0a0a 2020 2020 7a5f 6672 6163 7469  d...    z_fracti
+00051190: 6f6e 203a 2066 6c6f 6174 2c20 6465 6661  on : float, defa
+000511a0: 756c 743d 310a 2020 2020 2020 2020 506f  ult=1.        Po
+000511b0: 7369 7469 6f6e 2061 6c6f 6e67 207a 2061  sition along z a
+000511c0: 7869 7320 6174 2077 6869 6368 2074 6f20  xis at which to 
+000511d0: 7461 6b65 2073 6c69 6365 2074 6872 6f75  take slice throu
+000511e0: 6768 2052 4f49 2e0a 2020 2020 2020 2020  gh ROI..        
+000511f0: 5468 6520 706f 7369 7469 6f6e 2069 7320  The position is 
+00051200: 7370 6563 6966 6965 6420 6173 2074 6865  specified as the
+00051210: 2066 7261 6374 696f 6e61 6c20 6469 7374   fractional dist
+00051220: 616e 6365 0a20 2020 2020 2020 2066 726f  ance.        fro
+00051230: 6d20 7468 6520 524f 4927 7320 6d6f 7374  m the ROI's most
+00051240: 2d69 6e66 6572 696f 7220 706f 696e 743a  -inferior point:
+00051250: 2030 2063 6f72 7265 7370 6f6e 6473 2074   0 corresponds t
+00051260: 6f0a 2020 2020 2020 2020 7468 6520 6d6f  o.        the mo
+00051270: 7374 2d69 6e66 6572 696f 7220 706f 696e  st-inferior poin
+00051280: 7420 286c 6f77 6573 7420 7a29 3b20 3120  t (lowest z); 1 
+00051290: 636f 7272 6573 706f 6e64 7320 746f 2074  corresponds to t
+000512a0: 6865 0a20 2020 2020 2020 206d 6f73 742d  he.        most-
+000512b0: 7375 7065 7269 6f72 2070 6f69 6e74 2028  superior point (
+000512c0: 6869 6768 6573 7420 7a29 2e20 2056 616c  highest z).  Val
+000512d0: 7565 7320 666f 7220 7a5f 6672 6163 7469  ues for z_fracti
+000512e0: 6f6e 0a20 2020 2020 2020 206f 7574 7369  on.        outsi
+000512f0: 6465 2074 6865 2069 6e74 6572 7661 6c20  de the interval 
+00051300: 5b30 2c20 315d 2072 6573 756c 7420 696e  [0, 1] result in
+00051310: 2061 2052 756e 7469 6d65 4572 726f 722e   a RuntimeError.
+00051320: 0a0a 2020 2020 7375 6666 6978 203a 2073  ..    suffix : s
+00051330: 7472 2c20 6465 6661 756c 743d 4e6f 6e65  tr, default=None
+00051340: 0a20 2020 2020 2020 2053 7566 6669 7820  .        Suffix 
+00051350: 746f 2061 7070 656e 6420 746f 206e 616d  to append to nam
+00051360: 6520 6f66 2069 6e70 7574 2052 4f49 2c20  e of input ROI, 
+00051370: 746f 2066 6f72 6d20 6e61 6d65 0a20 2020  to form name.   
+00051380: 2020 2020 206f 6620 6f75 7470 7574 2052       of output R
+00051390: 4f49 2e20 2049 6620 4e6f 6e65 2c20 6170  OI.  If None, ap
+000513a0: 7065 6e64 207a 5f66 7261 6374 696f 6e2c  pend z_fraction,
+000513b0: 2077 6974 6820 7661 6c75 650a 2020 2020   with value.    
+000513c0: 2020 2020 6769 7665 6e20 746f 2074 776f      given to two
+000513d0: 2064 6563 696d 616c 2070 6c61 6365 732e   decimal places.
+000513e0: 0a20 2020 2022 2222 0a20 2020 2023 2043  .    """.    # C
+000513f0: 6865 636b 2074 6861 7420 7a5f 6672 6163  heck that z_frac
+00051400: 7469 6f6e 2069 7320 696e 2061 6c6c 6f77  tion is in allow
+00051410: 6564 2069 6e74 6572 7661 6c2e 0a20 2020  ed interval..   
+00051420: 2069 6620 7a5f 6672 6163 7469 6f6e 203c   if z_fraction <
+00051430: 2030 206f 7220 7a5f 6672 6163 7469 6f6e   0 or z_fraction
+00051440: 203e 2031 3a0a 2020 2020 2020 2020 7261   > 1:.        ra
+00051450: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
+00051460: 2866 227a 5f66 7261 6374 696f 6e3d 7b7a  (f"z_fraction={z
+00051470: 5f66 7261 6374 696f 6e7d 220a 2020 2020  _fraction}".    
+00051480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00051490: 2020 2020 2020 2020 2220 6f75 7473 6964          " outsid
+000514a0: 6520 616c 6c6f 7765 6420 696e 7465 7276  e allowed interv
+000514b0: 616c 205b 302c 2031 5d22 290a 0a20 2020  al [0, 1]")..   
+000514c0: 2023 2044 6574 6572 6d69 6e65 2074 6865   # Determine the
+000514d0: 2069 6e64 6578 206f 6620 7468 6520 696d   index of the im
+000514e0: 6167 6520 736c 6963 6520 6174 2077 6869  age slice at whi
+000514f0: 6368 2074 6f20 7461 6b65 2052 4f49 2073  ch to take ROI s
+00051500: 6c69 6365 2e0a 2020 2020 706f 7331 2c20  lice..    pos1, 
+00051510: 706f 7332 203d 2072 6f69 2e67 6574 5f65  pos2 = roi.get_e
+00051520: 7874 656e 7428 290a 2020 2020 706f 7320  xtent().    pos 
+00051530: 3d20 706f 7331 202b 207a 5f66 7261 6374  = pos1 + z_fract
+00051540: 696f 6e20 2a20 2870 6f73 3220 2d20 706f  ion * (pos2 - po
+00051550: 7331 290a 2020 2020 6964 7820 3d20 726f  s1).    idx = ro
+00051560: 692e 706f 735f 746f 5f69 6478 2870 6f73  i.pos_to_idx(pos
+00051570: 2c20 227a 2229 0a0a 2020 2020 2320 4f62  , "z")..    # Ob
+00051580: 7461 696e 2063 6f6e 746f 7572 7320 666f  tain contours fo
+00051590: 7220 7265 7175 6972 6564 2073 6c69 6365  r required slice
+000515a0: 2c20 616e 6420 636f 6e76 6572 7420 746f  , and convert to
+000515b0: 2052 4f49 206f 626a 6563 742e 0a20 2020   ROI object..   
+000515c0: 2063 6f6e 746f 7572 7320 3d20 726f 692e   contours = roi.
+000515d0: 6765 745f 636f 6e74 6f75 7273 2869 6478  get_contours(idx
+000515e0: 5f61 735f 6b65 793d 5472 7565 295b 6964  _as_key=True)[id
+000515f0: 785d 0a20 2020 2072 6f69 5f73 6c69 6365  x].    roi_slice
+00051600: 203d 2052 4f49 287b 726f 692e 6964 785f   = ROI({roi.idx_
+00051610: 746f 5f70 6f73 2869 6478 2c20 227a 2229  to_pos(idx, "z")
+00051620: 3a20 636f 6e74 6f75 7273 7d29 0a0a 2020  : contours})..  
+00051630: 2020 7375 6666 6978 203d 2066 227b 7a5f    suffix = f"{z_
+00051640: 6672 6163 7469 6f6e 3a2e 3266 7d22 2069  fraction:.2f}" i
+00051650: 6620 7375 6666 6978 2069 7320 4e6f 6e65  f suffix is None
+00051660: 2065 6c73 6520 7375 6666 6978 0a20 2020   else suffix.   
+00051670: 2069 6620 7375 6666 6978 3a0a 2020 2020   if suffix:.    
+00051680: 2020 2020 726f 695f 736c 6963 652e 6e61      roi_slice.na
+00051690: 6d65 203d 2066 227b 726f 692e 6e61 6d65  me = f"{roi.name
+000516a0: 7d5f 7b73 7566 6669 787d 220a 2020 2020  }_{suffix}".    
+000516b0: 656c 7365 3a0a 2020 2020 2020 2020 726f  else:.        ro
+000516c0: 695f 736c 6963 652e 6e61 6d65 203d 2073  i_slice.name = s
+000516d0: 7472 2872 6f69 2e6e 616d 6529 0a0a 2020  tr(roi.name)..  
+000516e0: 2020 7265 7475 726e 2072 6f69 5f73 6c69    return roi_sli
+000516f0: 6365 0a0a 6465 6620 6765 745f 6d65 7472  ce..def get_metr
+00051700: 6963 5f6d 6574 686f 6428 6d65 7472 6963  ic_method(metric
+00051710: 293a 0a20 2020 2022 2222 0a20 2020 204d  ):.    """.    M
+00051720: 6170 2062 6574 7765 656e 206d 6574 7269  ap between metri
+00051730: 6320 6964 656e 7469 6669 6572 2061 7320  c identifier as 
+00051740: 6c69 7374 6564 2069 6e20 6765 745f 636f  listed in get_co
+00051750: 6d70 6172 6973 6f6e 5f6d 6574 7269 6373  mparison_metrics
+00051760: 2829 0a20 2020 2061 6e64 206e 616d 6520  ().    and name 
+00051770: 6f66 2052 4f49 206d 6574 686f 6420 666f  of ROI method fo
+00051780: 7220 6361 6c63 756c 6174 696e 6720 7468  r calculating th
+00051790: 6520 6d65 7472 6963 2e0a 2020 2020 0a20  e metric..    . 
+000517a0: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+000517b0: 2069 7320 7573 6564 2069 6e20 524f 492e   is used in ROI.
+000517c0: 6765 745f 6d65 7472 6963 5f62 795f 736c  get_metric_by_sl
+000517d0: 6963 6528 2920 746f 2064 6574 6572 6d69  ice() to determi
+000517e0: 6e65 0a20 2020 2074 6865 206d 6574 686f  ne.    the metho
+000517f0: 6420 746f 2062 6520 6361 6c6c 6564 2066  d to be called f
+00051800: 6f72 2065 6163 6820 6d65 7472 6963 2e0a  or each metric..
+00051810: 2020 2020 2222 220a 2020 2020 2320 4b65      """.    # Ke
+00051820: 7973 2061 7265 206d 6574 7269 6320 6964  ys are metric id
+00051830: 656e 7469 6669 6572 733b 2076 616c 7565  entifiers; value
+00051840: 7320 6172 6520 6e61 6d65 7320 6f66 2052  s are names of R
+00051850: 4f49 206d 6574 686f 6473 0a20 2020 2023  OI methods.    #
+00051860: 2066 6f72 206d 6574 7269 6320 6361 6c63   for metric calc
+00051870: 756c 6174 696f 6e2e 0a20 2020 2023 204d  ulation..    # M
+00051880: 6574 7269 6373 2061 7265 2069 6e63 6c75  etrics are inclu
+00051890: 6465 6420 696e 2074 6865 2064 6963 7469  ded in the dicti
+000518a0: 6f6e 6172 7920 6f6e 6c79 2069 6620 6964  onary only if id
+000518b0: 656e 7469 6669 6572 2061 6e64 206d 6574  entifier and met
+000518c0: 686f 640a 2020 2020 2320 6e61 6d65 2061  hod.    # name a
+000518d0: 7265 2064 6966 6665 7265 6e74 2e0a 2020  re different..  
+000518e0: 2020 6d61 7070 696e 6773 203d 207b 0a20    mappings = {. 
+000518f0: 2020 2020 2020 2020 2020 2022 6162 735f             "abs_
+00051900: 6365 6e74 726f 6964 223a 2022 6162 735f  centroid": "abs_
+00051910: 6365 6e74 726f 6964 5f64 6973 7461 6e63  centroid_distanc
+00051920: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00051930: 2263 656e 7472 6f69 6422 3a20 2263 656e  "centroid": "cen
+00051940: 7472 6f69 645f 6469 7374 616e 6365 222c  troid_distance",
+00051950: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00051960: 6c5f 6172 6561 5f64 6966 6622 3a20 2272  l_area_diff": "r
+00051970: 656c 6174 6976 655f 6172 6561 5f64 6966  elative_area_dif
+00051980: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
+00051990: 7d0a 2020 2020 7265 7475 726e 206d 6170  }.    return map
+000519a0: 7069 6e67 732e 6765 7428 6d65 7472 6963  pings.get(metric
+000519b0: 2c20 6d65 7472 6963 290a 0a64 6566 2067  , metric)..def g
+000519c0: 6574 5f63 6f6d 7061 7269 736f 6e5f 6d65  et_comparison_me
+000519d0: 7472 6963 7328 6365 6e74 726f 6964 5f63  trics(centroid_c
+000519e0: 6f6d 706f 6e65 6e74 733d 4661 6c73 652c  omponents=False,
+000519f0: 2073 6c69 6365 5f73 7461 7473 3d4e 6f6e   slice_stats=Non
+00051a00: 652c 0a20 2020 2020 2020 2064 6566 6175  e,.        defau
+00051a10: 6c74 5f62 795f 736c 6963 653d 4e6f 6e65  lt_by_slice=None
+00051a20: 2c20 7669 6577 3d22 782d 7922 293a 0a20  , view="x-y"):. 
+00051a30: 2020 2022 2222 0a20 2020 2047 6574 206c     """.    Get l
+00051a40: 6973 7420 6f66 2063 6f6d 7061 7269 736f  ist of compariso
+00051a50: 6e20 6d65 7472 6963 732e 0a0a 2020 2020  n metrics...    
+00051a60: 416c 6c20 6d65 7472 6963 7320 6c69 7374  All metrics list
+00051a70: 6564 2068 6572 6520 7368 6f75 6c64 2062  ed here should b
+00051a80: 6520 7265 636f 676e 6973 6564 2062 7920  e recognised by 
+00051a90: 524f 492e 6765 745f 636f 6d70 6172 6973  ROI.get_comparis
+00051aa0: 6f6e 2829 2c0a 2020 2020 616e 6420 616c  on(),.    and al
+00051ab0: 6c20 6d65 7472 6963 7320 7265 636f 676e  l metrics recogn
+00051ac0: 6973 6564 2062 7920 524f 492e 6765 745f  ised by ROI.get_
+00051ad0: 636f 6d70 6172 6973 6f6e 2829 2073 686f  comparison() sho
+00051ae0: 756c 6420 6265 206c 6973 7465 6420 6865  uld be listed he
+00051af0: 7265 2e0a 0a20 2020 202a 2a50 6172 616d  re...    **Param
+00051b00: 6574 6572 733a 2a2a 0a0a 2020 2020 6365  eters:**..    ce
+00051b10: 6e74 726f 6964 5f63 6f6d 706f 6e65 6e74  ntroid_component
+00051b20: 7320 3a20 626f 6f6c 2c20 6465 6661 756c  s : bool, defaul
+00051b30: 743d 4661 6c73 650a 2020 2020 2020 2020  t=False.        
+00051b40: 4966 2054 7275 652c 2072 6570 6c61 6365  If True, replace
+00051b50: 206d 6574 7269 6373 2022 6365 6e74 726f   metrics "centro
+00051b60: 6964 2220 616e 6420 2263 656e 7472 6f69  id" and "centroi
+00051b70: 645f 736c 6963 6522 2062 7920 7468 650a  d_slice" by the.
+00051b80: 2020 2020 2020 2020 6d65 7472 6963 7320          metrics 
+00051b90: 666f 7220 7468 6569 7220 636f 6d70 6f6e  for their compon
+00051ba0: 656e 7473 2e0a 0a20 2020 2073 6c69 6365  ents...    slice
+00051bb0: 5f73 7461 7473 203a 2073 7472 2f6c 6973  _stats : str/lis
+00051bc0: 742f 6469 6374 2c20 6465 6661 756c 743d  t/dict, default=
+00051bd0: 4e6f 6e65 0a20 2020 2020 2020 2053 7065  None.        Spe
+00051be0: 6369 6669 6361 7469 6f6e 206f 6620 7374  cification of st
+00051bf0: 6174 6973 7469 6373 2074 6f20 6265 2063  atistics to be c
+00051c00: 616c 6375 6c61 7465 6420 7265 6c61 7469  alculated relati
+00051c10: 7665 0a20 2020 2020 2020 2074 6f20 736c  ve.        to sl
+00051c20: 6963 652d 6279 2d73 6c69 6365 206d 6574  ice-by-slice met
+00051c30: 7269 6320 7661 6c75 6573 2e0a 0a20 2020  ric values...   
+00051c40: 2020 2020 2041 2073 7461 7469 7374 6963       A statistic
+00051c50: 2069 7320 7370 6563 6966 6965 6420 6279   is specified by
+00051c60: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+00051c70: 2066 756e 6374 696f 6e20 666f 720a 2020   function for.  
+00051c80: 2020 2020 2020 6974 7320 6361 6c63 756c        its calcul
+00051c90: 6174 696f 6e20 696e 2074 6865 2050 7974  ation in the Pyt
+00051ca0: 686f 6e20 7374 6174 6973 7469 6373 206d  hon statistics m
+00051cb0: 6f64 756c 653a 0a0a 2020 2020 2020 2020  odule:..        
+00051cc0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+00051cd0: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
+00051ce0: 792f 7374 6174 6973 7469 6373 2e68 746d  y/statistics.htm
+00051cf0: 6c0a 0a20 2020 2020 2020 2046 6f72 2069  l..        For i
+00051d00: 7473 2075 7365 2068 6572 652c 2074 6865  ts use here, the
+00051d10: 2072 656c 6576 616e 7420 6675 6e63 7469   relevant functi
+00051d20: 6f6e 206d 7573 7420 7265 7175 6972 650a  on must require.
+00051d30: 2020 2020 2020 2020 6120 7369 6e67 6c65          a single
+00051d40: 2d76 6172 6961 626c 6520 696e 7075 742c  -variable input,
+00051d50: 206d 7573 7420 6e6f 7420 7265 7175 6972   must not requir
+00051d60: 6520 616e 7920 6b65 7977 6f72 640a 2020  e any keyword.  
+00051d70: 2020 2020 2020 6172 6775 6d65 6e74 732c        arguments,
+00051d80: 2061 6e64 206d 7573 7420 7265 7475 726e   and must return
+00051d90: 2061 2073 696e 676c 6520 6e75 6d62 6572   a single number
+00051da0: 2e0a 0a20 2020 2020 2020 2041 7661 696c  ...        Avail
+00051db0: 6162 6c65 206f 7074 696f 6e73 2069 6e63  able options inc
+00051dc0: 6c75 6465 3a20 226d 6561 6e22 2c20 226d  lude: "mean", "m
+00051dd0: 6564 6961 6e22 2c20 226d 6f64 6522 2c0a  edian", "mode",.
+00051de0: 2020 2020 2020 2020 2273 7464 6576 222e          "stdev".
+00051df0: 0a0a 2020 2020 2020 2053 7461 7469 7374  ..       Statist
+00051e00: 6963 7320 746f 2062 6520 6361 6c63 756c  ics to be calcul
+00051e10: 6174 6564 2063 616e 2062 6520 7370 6563  ated can be spec
+00051e20: 6966 6965 6420 7573 696e 6720 616e 7920  ified using any 
+00051e30: 6f66 0a20 2020 2020 2020 7468 6520 666f  of.       the fo
+00051e40: 6c6c 6f77 696e 673a 0a0a 2020 2020 2020  llowing:..      
+00051e50: 202d 2053 7472 696e 6720 7370 6563 6966   - String specif
+00051e60: 7969 6e67 2073 696e 676c 6520 7374 6174  ying single stat
+00051e70: 6973 7469 6320 746f 2062 6520 6361 6c63  istic to be calc
+00051e80: 756c 6174 6564 2c0a 2020 2020 2020 2020  ulated,.        
+00051e90: 2077 6974 6820 736c 6963 6573 2063 6f6e   with slices con
+00051ea0: 7369 6465 7265 6420 6173 2067 6976 656e  sidered as given
+00051eb0: 2062 7920 3c64 6566 6175 6c74 5f62 795f   by <default_by_
+00051ec0: 736c 6963 653e 2c0a 2020 2020 2020 2020  slice>,.        
+00051ed0: 2066 6f72 2065 7861 6d70 6c65 3a20 226d   for example: "m
+00051ee0: 6561 6e22 3b0a 2020 2020 2020 202d 204c  ean";.       - L
+00051ef0: 6973 7420 7370 6563 6966 7969 6e67 206d  ist specifying m
+00051f00: 756c 7469 706c 6520 7374 6174 6973 7469  ultiple statisti
+00051f10: 6373 2074 6f20 6265 2063 616c 6375 6c61  cs to be calcula
+00051f20: 7465 642c 0a20 2020 2020 2020 2020 7769  ted,.         wi
+00051f30: 7468 2073 6c69 6365 7320 636f 6e73 6964  th slices consid
+00051f40: 6572 6564 2061 7320 6769 7665 6e20 6279  ered as given by
+00051f50: 203c 6465 6661 756c 745f 6279 5f73 6c69   <default_by_sli
+00051f60: 6365 3e2c 0a20 2020 2020 2020 2020 666f  ce>,.         fo
+00051f70: 7220 6578 616d 706c 653a 205b 226d 6561  r example: ["mea
+00051f80: 6e22 2c20 2273 7464 6576 225d 3b0a 2020  n", "stdev"];.  
+00051f90: 2020 2020 202d 2044 6963 7469 6f6e 6172       - Dictionar
+00051fa0: 7920 7768 6572 6520 6b65 7973 2073 7065  y where keys spe
+00051fb0: 6369 6679 2073 6c69 6365 7320 746f 2062  cify slices to b
+00051fc0: 6520 636f 6e73 6964 6572 6564 2c0a 2020  e considered,.  
+00051fd0: 2020 2020 2020 2061 6e64 2076 616c 7565         and value
+00051fe0: 7320 7370 6563 6966 7920 7374 6174 6973  s specify statis
+00051ff0: 7469 6373 2028 7374 7269 6e67 206f 7220  tics (string or 
+00052000: 6c69 7374 292c 2066 6f72 0a20 2020 2020  list), for.     
+00052010: 2020 2020 6578 616d 706c 653a 207b 2275      example: {"u
+00052020: 6e69 6f6e 223a 205b 226d 6561 6e22 2c20  nion": ["mean", 
+00052030: 2273 7464 6576 225d 7d2e 2020 5661 6c69  "stdev"]}.  Vali
+00052040: 6420 736c 6963 650a 2020 2020 2020 2020  d slice.        
+00052050: 2073 7065 6369 6669 6361 7469 6f6e 7320   specifications 
+00052060: 6172 6520 6173 206c 6973 7465 6420 666f  are as listed fo
+00052070: 7220 3c64 6566 6175 6c74 5f62 795f 736c  r <default_by_sl
+00052080: 6963 653e 2e0a 0a20 2020 2064 6566 6175  ice>...    defau
+00052090: 6c74 5f62 795f 736c 6963 653a 2073 7472  lt_by_slice: str
+000520a0: 2c20 6465 6661 756c 743d 4e6f 6e65 0a20  , default=None. 
+000520b0: 2020 2020 2020 2044 6566 6175 6c74 2073         Default s
+000520c0: 7065 6369 6669 6361 7469 6f6e 206f 6620  pecification of 
+000520d0: 736c 6963 6573 2074 6f20 6265 2063 6f6e  slices to be con
+000520e0: 7369 6465 7265 6420 7768 656e 0a20 2020  sidered when.   
+000520f0: 2020 2020 2063 616c 6375 6c61 7469 6e67       calculating
+00052100: 2073 6c69 6365 2d62 792d 736c 6963 6520   slice-by-slice 
+00052110: 7374 6174 6973 7469 6373 2066 6f72 2061  statistics for a
+00052120: 206d 6574 7269 6320 636f 6d70 6172 696e   metric comparin
+00052130: 670a 2020 2020 2020 2020 7477 6f20 524f  g.        two RO
+00052140: 4973 2c20 726f 6931 2061 6e64 2072 6f69  Is, roi1 and roi
+00052150: 322e 2020 5468 6520 7661 6c69 6420 7370  2.  The valid sp
+00052160: 6563 6966 6963 6174 696f 6e73 2061 7265  ecifications are
+00052170: 3a0a 0a20 2020 2020 2020 202d 2022 6c65  :..        - "le
+00052180: 6674 223a 2063 6f6e 7369 6465 7220 6f6e  ft": consider on
+00052190: 6c79 2073 6c69 6365 7320 636f 6e74 6169  ly slices contai
+000521a0: 6e69 6e67 2072 6f69 313b 0a20 2020 2020  ning roi1;.     
+000521b0: 2020 202d 2022 7269 6768 7422 3a20 636f     - "right": co
+000521c0: 6e73 6964 6572 206f 6e6c 7920 736c 6963  nsider only slic
+000521d0: 6573 2063 6f6e 7461 696e 696e 6720 726f  es containing ro
+000521e0: 6932 3b0a 2020 2020 2020 2020 2d20 2275  i2;.        - "u
+000521f0: 6e69 6f6e 223a 2063 6f6e 7369 6465 7220  nion": consider 
+00052200: 736c 6963 6573 2063 6f6e 7461 696e 696e  slices containin
+00052210: 6720 6569 7468 6572 206f 6620 726f 6931  g either of roi1
+00052220: 2061 6e64 2072 6f69 323b 0a20 2020 2020   and roi2;.     
+00052230: 2020 202d 2022 696e 7465 7273 6563 7469     - "intersecti
+00052240: 6f6e 223a 2063 6f6e 7369 6465 7220 736c  on": consider sl
+00052250: 6963 6573 2063 6f6e 7461 696e 696e 6720  ices containing 
+00052260: 626f 7468 2072 6f69 3120 616e 6420 726f  both roi1 and ro
+00052270: 6932 2e0a 0a20 2020 2020 2020 2049 6620  i2...        If 
+00052280: 4e6f 6e65 2c20 7573 6520 736b 7274 2e63  None, use skrt.c
+00052290: 6f72 652e 4465 6661 756c 7473 2829 2e62  ore.Defaults().b
+000522a0: 795f 736c 6963 650a 0a20 2020 2020 2020  y_slice..       
+000522b0: 2076 6965 7720 3a20 7374 722c 2064 6566   view : str, def
+000522c0: 6175 6c74 3d22 782d 7922 0a20 2020 2020  ault="x-y".     
+000522d0: 2020 2020 2020 204f 7269 656e 7461 7469         Orientati
+000522e0: 6f6e 2074 6f20 636f 6e73 6964 6572 2077  on to consider w
+000522f0: 6865 6e20 7461 6b69 6e67 2063 656e 7472  hen taking centr
+00052300: 6f69 6420 636f 6d70 6f6e 656e 7473 2072  oid components r
+00052310: 656c 6174 6976 650a 2020 2020 2020 2020  elative.        
+00052320: 2020 2020 746f 2061 2073 6c69 6365 2e20      to a slice. 
+00052330: 2043 616e 2062 6520 2278 2d79 222c 2022   Can be "x-y", "
+00052340: 792d 7a22 2c20 6f72 2022 782d 7a22 2e0a  y-z", or "x-z"..
+00052350: 2020 2020 2222 220a 2020 2020 6d65 7472      """.    metr
+00052360: 6963 7320 3d20 5b0a 2020 2020 2020 2020  ics = [.        
+00052370: 2020 2020 2261 6273 5f63 656e 7472 6f69      "abs_centroi
+00052380: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+00052390: 2261 6273 5f63 656e 7472 6f69 645f 666c  "abs_centroid_fl
+000523a0: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
+000523b0: 2022 6162 735f 6365 6e74 726f 6964 5f73   "abs_centroid_s
+000523c0: 6c69 6365 222c 0a20 2020 2020 2020 2020  lice",.         
+000523d0: 2020 2022 6162 735f 6365 6e74 726f 6964     "abs_centroid
+000523e0: 5f73 6c69 6365 5f73 7461 7473 222c 0a20  _slice_stats",. 
+000523f0: 2020 2020 2020 2020 2020 2022 6172 6561             "area
+00052400: 5f64 6966 6622 2c0a 2020 2020 2020 2020  _diff",.        
+00052410: 2020 2020 2261 7265 615f 6469 6666 5f66      "area_diff_f
+00052420: 6c61 7422 2c0a 2020 2020 2020 2020 2020  lat",.          
+00052430: 2020 2261 7265 615f 6469 6666 5f73 6c69    "area_diff_sli
+00052440: 6365 5f73 7461 7473 222c 0a20 2020 2020  ce_stats",.     
+00052450: 2020 2020 2020 2022 6172 6561 5f72 6174         "area_rat
+00052460: 696f 222c 0a20 2020 2020 2020 2020 2020  io",.           
+00052470: 2022 6172 6561 5f72 6174 696f 5f66 6c61   "area_ratio_fla
+00052480: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00052490: 2261 7265 615f 7261 7469 6f5f 736c 6963  "area_ratio_slic
+000524a0: 655f 7374 6174 7322 2c0a 2020 2020 2020  e_stats",.      
+000524b0: 2020 2020 2020 2263 656e 7472 6f69 6422        "centroid"
+000524c0: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
+000524d0: 656e 7472 6f69 645f 736c 6963 6522 2c0a  entroid_slice",.
+000524e0: 2020 2020 2020 2020 2020 2020 2263 656e              "cen
+000524f0: 7472 6f69 645f 736c 6963 655f 7374 6174  troid_slice_stat
+00052500: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00052510: 2264 6963 6522 2c0a 2020 2020 2020 2020  "dice",.        
+00052520: 2020 2020 2264 6963 655f 666c 6174 222c      "dice_flat",
+00052530: 0a20 2020 2020 2020 2020 2020 2022 6469  .            "di
+00052540: 6365 5f73 6c69 6365 222c 0a20 2020 2020  ce_slice",.     
+00052550: 2020 2020 2020 2022 6469 6365 5f73 6c69         "dice_sli
+00052560: 6365 5f73 7461 7473 222c 0a20 2020 2020  ce_stats",.     
+00052570: 2020 2020 2020 2022 6861 7573 646f 7266         "hausdorf
+00052580: 665f 6469 7374 616e 6365 222c 0a20 2020  f_distance",.   
+00052590: 2020 2020 2020 2020 2022 6861 7573 646f           "hausdo
+000525a0: 7266 665f 6469 7374 616e 6365 5f66 6c61  rff_distance_fla
 000525b0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-000525c0: 226a 6163 6361 7264 5f73 6c69 6365 222c  "jaccard_slice",
-000525d0: 0a20 2020 2020 2020 2020 2020 2022 6a61  .            "ja
-000525e0: 6363 6172 645f 736c 6963 655f 7374 6174  ccard_slice_stat
-000525f0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00052600: 226d 6561 6e5f 6469 7374 616e 6365 5f74  "mean_distance_t
-00052610: 6f5f 636f 6e66 6f72 6d69 7479 222c 0a20  o_conformity",. 
-00052620: 2020 2020 2020 2020 2020 2022 6d65 616e             "mean
-00052630: 5f64 6973 7461 6e63 655f 746f 5f63 6f6e  _distance_to_con
-00052640: 666f 726d 6974 795f 666c 6174 222c 0a20  formity_flat",. 
-00052650: 2020 2020 2020 2020 2020 2022 6d65 616e             "mean
-00052660: 5f73 6967 6e65 645f 7375 7266 6163 655f  _signed_surface_
-00052670: 6469 7374 616e 6365 222c 0a20 2020 2020  distance",.     
-00052680: 2020 2020 2020 2022 6d65 616e 5f73 6967         "mean_sig
-00052690: 6e65 645f 7375 7266 6163 655f 6469 7374  ned_surface_dist
-000526a0: 616e 6365 5f66 6c61 7422 2c0a 2020 2020  ance_flat",.    
-000526b0: 2020 2020 2020 2020 226d 6561 6e5f 7375          "mean_su
-000526c0: 7266 6163 655f 6469 7374 616e 6365 222c  rface_distance",
-000526d0: 0a20 2020 2020 2020 2020 2020 2022 6d65  .            "me
-000526e0: 616e 5f73 7572 6661 6365 5f64 6973 7461  an_surface_dista
-000526f0: 6e63 655f 666c 6174 222c 0a20 2020 2020  nce_flat",.     
-00052700: 2020 2020 2020 2022 6d65 616e 5f6f 7665         "mean_ove
-00052710: 725f 636f 6e74 6f75 7269 6e67 222c 0a20  r_contouring",. 
-00052720: 2020 2020 2020 2020 2020 2022 6d65 616e             "mean
-00052730: 5f6f 7665 725f 636f 6e74 6f75 7269 6e67  _over_contouring
-00052740: 5f66 6c61 7422 2c0a 2020 2020 2020 2020  _flat",.        
-00052750: 2020 2020 226d 6561 6e5f 756e 6465 725f      "mean_under_
-00052760: 636f 6e74 6f75 7269 6e67 222c 0a20 2020  contouring",.   
-00052770: 2020 2020 2020 2020 2022 6d65 616e 5f75           "mean_u
-00052780: 6e64 6572 5f63 6f6e 746f 7572 696e 675f  nder_contouring_
-00052790: 666c 6174 222c 0a20 2020 2020 2020 2020  flat",.         
-000527a0: 2020 2022 7265 6c5f 6172 6561 5f64 6966     "rel_area_dif
-000527b0: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
-000527c0: 2272 656c 5f61 7265 615f 6469 6666 5f66  "rel_area_diff_f
-000527d0: 6c61 7422 2c0a 2020 2020 2020 2020 2020  lat",.          
-000527e0: 2020 2272 656c 5f61 7265 615f 6469 6666    "rel_area_diff
-000527f0: 5f73 6c69 6365 5f73 7461 7473 222c 0a20  _slice_stats",. 
-00052800: 2020 2020 2020 2020 2020 2022 7265 6c5f             "rel_
-00052810: 766f 6c75 6d65 5f64 6966 6622 2c0a 2020  volume_diff",.  
-00052820: 2020 2020 2020 2020 2020 2272 6d73 5f73            "rms_s
-00052830: 6967 6e65 645f 7375 7266 6163 655f 6469  igned_surface_di
-00052840: 7374 616e 6365 222c 0a20 2020 2020 2020  stance",.       
-00052850: 2020 2020 2022 726d 735f 7369 676e 6564       "rms_signed
-00052860: 5f73 7572 6661 6365 5f64 6973 7461 6e63  _surface_distanc
-00052870: 655f 666c 6174 222c 0a20 2020 2020 2020  e_flat",.       
-00052880: 2020 2020 2022 726d 735f 7375 7266 6163       "rms_surfac
-00052890: 655f 6469 7374 616e 6365 222c 0a20 2020  e_distance",.   
-000528a0: 2020 2020 2020 2020 2022 726d 735f 7375           "rms_su
-000528b0: 7266 6163 655f 6469 7374 616e 6365 5f66  rface_distance_f
-000528c0: 6c61 7422 2c0a 2020 2020 2020 2020 2020  lat",.          
-000528d0: 2020 2276 6f6c 756d 655f 6469 6666 222c    "volume_diff",
-000528e0: 0a20 2020 2020 2020 2020 2020 2022 766f  .            "vo
-000528f0: 6c75 6d65 5f72 6174 696f 222c 0a20 2020  lume_ratio",.   
-00052900: 2020 2020 2020 2020 205d 0a0a 2020 2020           ]..    
-00052910: 2320 5265 706c 6163 6520 6365 6e74 726f  # Replace centro
-00052920: 6964 2076 6563 746f 7273 2062 7920 636f  id vectors by co
-00052930: 6d70 6f6e 656e 7473 2e0a 2020 2020 6966  mponents..    if
-00052940: 2063 656e 7472 6f69 645f 636f 6d70 6f6e   centroid_compon
-00052950: 656e 7473 3a0a 2020 2020 2020 2020 6365  ents:.        ce
-00052960: 6e74 726f 6964 7320 3d20 7b0a 2020 2020  ntroids = {.    
-00052970: 2020 2020 2020 2020 2020 2020 2263 656e              "cen
-00052980: 7472 6f69 6422 3a20 5b22 6365 6e74 726f  troid": ["centro
-00052990: 6964 5f78 222c 2022 6365 6e74 726f 6964  id_x", "centroid
-000529a0: 5f79 222c 2022 6365 6e74 726f 6964 5f7a  _y", "centroid_z
-000529b0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-000529c0: 2020 2020 2263 656e 7472 6f69 645f 736c      "centroid_sl
-000529d0: 6963 6522 3a20 5b5d 0a20 2020 2020 2020  ice": [].       
-000529e0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000529f0: 2020 2069 6620 736c 6963 655f 7374 6174     if slice_stat
-00052a00: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-00052a10: 2020 2020 2020 2020 2020 2063 656e 7472             centr
-00052a20: 6f69 6473 5b22 6365 6e74 726f 6964 5f73  oids["centroid_s
-00052a30: 6c69 6365 5f73 7461 7473 225d 203d 205b  lice_stats"] = [
-00052a40: 5d0a 0a20 2020 2020 2020 2066 6f72 2069  ]..        for i
-00052a50: 5f61 7820 696e 2073 6b72 742e 696d 6167  _ax in skrt.imag
-00052a60: 652e 5f70 6c6f 745f 6178 6573 5b76 6965  e._plot_axes[vie
-00052a70: 775d 3a0a 2020 2020 2020 2020 2020 2020  w]:.            
-00052a80: 6178 203d 2073 6b72 742e 696d 6167 652e  ax = skrt.image.
-00052a90: 5f61 7865 735b 695f 6178 5d0a 2020 2020  _axes[i_ax].    
-00052aa0: 2020 2020 2020 2020 6365 6e74 726f 6964          centroid
-00052ab0: 735b 2263 656e 7472 6f69 645f 736c 6963  s["centroid_slic
-00052ac0: 6522 5d2e 6170 7065 6e64 2866 2263 656e  e"].append(f"cen
-00052ad0: 7472 6f69 645f 736c 6963 655f 7b61 787d  troid_slice_{ax}
-00052ae0: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-00052af0: 6966 2073 6c69 6365 5f73 7461 7473 2069  if slice_stats i
-00052b00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00052b10: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
-00052b20: 726f 6964 735b 2263 656e 7472 6f69 645f  roids["centroid_
-00052b30: 736c 6963 655f 7374 6174 7322 5d2e 6170  slice_stats"].ap
-00052b40: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
-00052b50: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00052b60: 6365 6e74 726f 6964 5f7b 6178 7d5f 736c  centroid_{ax}_sl
-00052b70: 6963 655f 7374 6174 7322 290a 0a20 2020  ice_stats")..   
-00052b80: 2020 2020 2066 6f72 2076 6563 746f 722c       for vector,
-00052b90: 2063 6f6d 706f 6e65 6e74 7320 696e 2063   components in c
-00052ba0: 656e 7472 6f69 6473 2e69 7465 6d73 2829  entroids.items()
-00052bb0: 3a0a 2020 2020 2020 2020 2020 2020 6964  :.            id
-00052bc0: 7820 3d20 6d65 7472 6963 732e 696e 6465  x = metrics.inde
-00052bd0: 7828 7665 6374 6f72 290a 2020 2020 2020  x(vector).      
-00052be0: 2020 2020 2020 6d65 7472 6963 735b 6964        metrics[id
-00052bf0: 7820 3a20 6964 7820 2b20 315d 203d 2063  x : idx + 1] = c
-00052c00: 6f6d 706f 6e65 6e74 730a 0a20 2020 2023  omponents..    #
-00052c10: 2052 656d 6f76 6520 6d65 7472 6963 7320   Remove metrics 
-00052c20: 7769 7468 2073 7566 6669 7820 2273 6c69  with suffix "sli
-00052c30: 6365 5f73 7461 7473 222c 0a20 2020 2023  ce_stats",.    #
-00052c40: 2061 6e64 2072 6570 6c61 6365 2077 6974   and replace wit
-00052c50: 6820 7370 6563 6966 6963 206d 6574 7269  h specific metri
-00052c60: 6373 2072 656c 6174 696e 6720 746f 2073  cs relating to s
-00052c70: 6c69 6365 2d62 792d 736c 6963 6520 7374  lice-by-slice st
-00052c80: 6174 6973 7469 6373 2e0a 2020 2020 6966  atistics..    if
-00052c90: 2073 6c69 6365 5f73 7461 7473 2069 7320   slice_stats is 
-00052ca0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00052cb0: 2020 736c 6963 655f 7374 6174 735f 6d65    slice_stats_me
-00052cc0: 7472 6963 7320 3d20 5b5d 0a20 2020 2020  trics = [].     
-00052cd0: 2020 206d 6574 7269 6373 3220 3d20 5b5d     metrics2 = []
-00052ce0: 0a20 2020 2020 2020 2066 6f72 206d 6574  .        for met
-00052cf0: 7269 6320 696e 206d 6574 7269 6373 3a0a  ric in metrics:.
-00052d00: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-00052d10: 736c 6963 655f 7374 6174 7322 2069 6e20  slice_stats" in 
-00052d20: 6d65 7472 6963 3a0a 2020 2020 2020 2020  metric:.        
-00052d30: 2020 2020 2020 2020 736c 6963 655f 7374          slice_st
-00052d40: 6174 735f 6d65 7472 6963 732e 6170 7065  ats_metrics.appe
-00052d50: 6e64 286d 6574 7269 632e 7370 6c69 7428  nd(metric.split(
-00052d60: 225f 736c 6963 655f 7374 6174 7322 295b  "_slice_stats")[
-00052d70: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00052d80: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00052d90: 2020 2020 2020 6d65 7472 6963 7332 2e61        metrics2.a
-00052da0: 7070 656e 6428 6d65 7472 6963 290a 0a20  ppend(metric).. 
-00052db0: 2020 2020 2020 2066 6f72 2062 795f 736c         for by_sl
-00052dc0: 6963 652c 2073 7461 7473 2069 6e20 280a  ice, stats in (.
-00052dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00052de0: 6578 7061 6e64 5f73 6c69 6365 5f73 7461  expand_slice_sta
-00052df0: 7473 2873 6c69 6365 5f73 7461 7473 2c20  ts(slice_stats, 
-00052e00: 6465 6661 756c 745f 6279 5f73 6c69 6365  default_by_slice
-00052e10: 292e 6974 656d 7328 2929 3a0a 2020 2020  ).items()):.    
-00052e20: 2020 2020 2020 2020 666f 7220 6d65 7472          for metr
-00052e30: 6963 2069 6e20 736c 6963 655f 7374 6174  ic in slice_stat
-00052e40: 735f 6d65 7472 6963 733a 0a20 2020 2020  s_metrics:.     
-00052e50: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00052e60: 7461 7420 696e 2073 7461 7473 3a0a 2020  tat in stats:.  
-00052e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00052e80: 2020 6d65 7472 6963 7332 2e61 7070 656e    metrics2.appen
-00052e90: 6428 6622 7b6d 6574 7269 637d 5f73 6c69  d(f"{metric}_sli
-00052ea0: 6365 5f7b 6279 5f73 6c69 6365 7d5f 7b73  ce_{by_slice}_{s
-00052eb0: 7461 747d 2229 0a20 2020 2020 2020 206d  tat}").        m
-00052ec0: 6574 7269 6373 203d 206d 6574 7269 6373  etrics = metrics
-00052ed0: 320a 0a20 2020 2072 6574 7572 6e20 736f  2..    return so
-00052ee0: 7274 6564 286d 6574 7269 6373 290a 0a64  rted(metrics)..d
-00052ef0: 6566 2067 6574 5f63 6f6e 7365 6e73 7573  ef get_consensus
-00052f00: 5f74 7970 6573 2829 3a0a 2020 2020 2222  _types():.    ""
-00052f10: 220a 2020 2020 4765 7420 6c69 7374 206f  ".    Get list o
-00052f20: 6620 636f 6e73 656e 7375 7320 7479 7065  f consensus type
-00052f30: 732e 0a0a 2020 2020 416c 6c20 636f 6e73  s...    All cons
-00052f40: 656e 7375 7320 7479 7065 7320 6c69 7374  ensus types list
-00052f50: 6564 2068 6572 6520 7368 6f75 6c64 2062  ed here should b
-00052f60: 6520 7265 636f 676e 6973 6564 2062 790a  e recognised by.
-00052f70: 2020 2020 5374 7275 6374 7572 6553 6574      StructureSet
-00052f80: 2e67 6574 5f63 6f6e 7365 6e73 7573 2829  .get_consensus()
-00052f90: 2c20 616e 6420 616c 6c20 636f 6e73 656e  , and all consen
-00052fa0: 7375 7320 7479 7065 7320 7265 636f 676e  sus types recogn
-00052fb0: 6973 6564 0a20 2020 2062 7920 5374 7275  ised.    by Stru
-00052fc0: 6374 7572 6553 6574 2e67 6574 5f63 6f6e  ctureSet.get_con
-00052fd0: 7365 6e73 7573 2073 686f 756c 6420 6265  sensus should be
-00052fe0: 206c 6973 7465 6420 6865 7265 2e0a 2020   listed here..  
-00052ff0: 2020 2222 220a 2020 2020 7265 7475 726e    """.    return
-00053000: 205b 0a20 2020 2020 2020 2020 2020 2022   [.            "
-00053010: 6d61 6a6f 7269 7479 222c 0a20 2020 2020  majority",.     
-00053020: 2020 2020 2020 2022 6f76 6572 6c61 7022         "overlap"
-00053030: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
-00053040: 7461 706c 6522 2c0a 2020 2020 2020 2020  taple",.        
-00053050: 2020 2020 2273 756d 222c 0a20 2020 2020      "sum",.     
-00053060: 2020 2020 2020 205d 0a0a 6465 6620 6765         ]..def ge
-00053070: 745f 6279 5f73 6c69 6365 5f6d 6574 686f  t_by_slice_metho
-00053080: 6473 2829 3a0a 2020 2020 2222 220a 2020  ds():.    """.  
-00053090: 2020 4765 7420 6c69 7374 206f 6620 6d65    Get list of me
-000530a0: 7468 6f64 7320 666f 7220 6465 6669 6e69  thods for defini
-000530b0: 6e67 2073 6c69 6365 7320 746f 2062 6520  ng slices to be 
-000530c0: 636f 6e73 6964 6572 6564 0a20 2020 2066  considered.    f
-000530d0: 6f72 2073 6c69 6365 2d62 792d 736c 6963  or slice-by-slic
-000530e0: 6520 524f 4920 636f 6d70 6172 6973 6f6e  e ROI comparison
-000530f0: 732e 0a20 2020 2022 2222 0a20 2020 2072  s..    """.    r
-00053100: 6574 7572 6e20 5b22 6c65 6674 222c 2022  eturn ["left", "
-00053110: 7269 6768 7422 2c20 2275 6e69 6f6e 222c  right", "union",
-00053120: 2022 696e 7465 7273 6563 7469 6f6e 225d   "intersection"]
-00053130: 0a0a 6465 6620 6765 745f 616c 6c5f 726f  ..def get_all_ro
-00053140: 6973 286f 626a 733d 4e6f 6e65 293a 0a20  is(objs=None):. 
-00053150: 2020 2022 2222 0a20 2020 2043 7265 6174     """.    Creat
-00053160: 6520 6c69 7374 206f 6620 524f 4973 2066  e list of ROIs f
-00053170: 726f 6d20 6172 6269 7472 6172 7920 636f  rom arbitrary co
-00053180: 6d62 696e 6174 696f 6e20 6f66 2052 4f49  mbination of ROI
-00053190: 7320 616e 6420 5374 7275 6374 7572 6553  s and StructureS
-000531a0: 6574 732e 0a0a 2020 2020 2a2a 5061 7261  ets...    **Para
-000531b0: 6d65 7465 7273 3a2a 2a0a 0a20 2020 206f  meters:**..    o
-000531c0: 626a 7320 3a20 524f 492f 5374 7275 6374  bjs : ROI/Struct
-000531d0: 7572 6553 6574 2f6c 6973 742c 2064 6566  ureSet/list, def
-000531e0: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
-000531f0: 2020 4f62 6a65 6374 2873 2920 6672 6f6d    Object(s) from
-00053200: 2077 6869 6368 2061 206c 6973 7420 6f66   which a list of
-00053210: 2052 4f49 7320 6973 2074 6f20 6265 2063   ROIs is to be c
-00053220: 7265 6174 6564 2e20 2054 6865 0a20 2020  reated.  The.   
-00053230: 2020 2020 206f 626a 6563 7428 7329 2063       object(s) c
-00053240: 616e 2062 6520 6120 7369 6e67 6c65 2073  an be a single s
-00053250: 6b72 742e 7374 7275 6374 7572 6573 2e52  krt.structures.R
-00053260: 4f49 206f 626a 6563 742c 2061 2073 696e  OI object, a sin
-00053270: 676c 650a 2020 2020 2020 2020 736b 7274  gle.        skrt
-00053280: 2e73 7472 7563 7475 7265 732e 5374 7275  .structures.Stru
-00053290: 6374 7572 6553 6574 206f 626a 6563 742c  ctureSet object,
-000532a0: 206f 7220 6120 6c69 7374 2063 6f6e 7461   or a list conta
-000532b0: 696e 696e 6720 616e 790a 2020 2020 2020  ining any.      
-000532c0: 2020 636f 6d62 696e 6174 696f 6e20 6f66    combination of
-000532d0: 2052 4f49 2061 6e64 2053 7472 7563 7475   ROI and Structu
-000532e0: 7265 5365 7420 6f62 6a65 6374 732e 0a20  reSet objects.. 
-000532f0: 2020 2022 2222 0a20 2020 2023 2045 6e73     """.    # Ens
-00053300: 7572 6520 7468 6174 206f 626a 7320 6973  ure that objs is
-00053310: 2061 206c 6973 740a 2020 2020 6966 2069   a list.    if i
-00053320: 7373 7562 636c 6173 7328 7479 7065 286f  ssubclass(type(o
-00053330: 626a 7329 2c20 2852 4f49 2c20 5374 7275  bjs), (ROI, Stru
-00053340: 6374 7572 6553 6574 2929 3a0a 2020 2020  ctureSet)):.    
-00053350: 2020 2020 6f62 6a73 203d 205b 6f62 6a73      objs = [objs
-00053360: 5d0a 2020 2020 656c 6966 206f 626a 7320  ].    elif objs 
-00053370: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00053380: 206f 626a 7320 3d20 5b5d 0a0a 2020 2020   objs = []..    
-00053390: 2320 4372 6561 7465 2061 206c 6973 7420  # Create a list 
-000533a0: 636f 6e74 6169 6e69 6e67 2061 6c6c 2075  containing all u
-000533b0: 6e69 7175 6520 726f 6973 2e0a 2020 2020  nique rois..    
-000533c0: 616c 6c5f 726f 6973 203d 205b 5d0a 2020  all_rois = [].  
-000533d0: 2020 666f 7220 6974 656d 2069 6e20 6f62    for item in ob
-000533e0: 6a73 3a0a 2020 2020 2020 2020 6966 2069  js:.        if i
-000533f0: 7373 7562 636c 6173 7328 7479 7065 2869  ssubclass(type(i
-00053400: 7465 6d29 2c20 524f 4929 3a0a 2020 2020  tem), ROI):.    
-00053410: 2020 2020 2020 2020 6361 6e64 6964 6174          candidat
-00053420: 655f 726f 6973 203d 205b 6974 656d 5d0a  e_rois = [item].
-00053430: 2020 2020 2020 2020 656c 6966 2069 7373          elif iss
-00053440: 7562 636c 6173 7328 7479 7065 2869 7465  ubclass(type(ite
-00053450: 6d29 2c20 5374 7275 6374 7572 6553 6574  m), StructureSet
-00053460: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00053470: 616e 6469 6461 7465 5f72 6f69 7320 3d20  andidate_rois = 
-00053480: 6974 656d 2e67 6574 5f72 6f69 7328 290a  item.get_rois().
-00053490: 2020 2020 2020 2020 666f 7220 726f 6920          for roi 
-000534a0: 696e 2063 616e 6469 6461 7465 5f72 6f69  in candidate_roi
-000534b0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-000534c0: 6620 6e6f 7420 726f 6920 696e 2061 6c6c  f not roi in all
-000534d0: 5f72 6f69 733a 0a20 2020 2020 2020 2020  _rois:.         
-000534e0: 2020 2020 2020 2061 6c6c 5f72 6f69 732e         all_rois.
-000534f0: 6170 7065 6e64 2872 6f69 290a 0a20 2020  append(roi)..   
-00053500: 2072 6574 7572 6e20 616c 6c5f 726f 6973   return all_rois
-00053510: 0a0a 6465 6620 6765 745f 7472 616e 736c  ..def get_transl
-00053520: 6174 696f 6e5f 746f 5f61 6c69 676e 2872  ation_to_align(r
-00053530: 6f69 312c 2072 6f69 322c 207a 5f66 7261  oi1, roi2, z_fra
-00053540: 6374 696f 6e31 3d4e 6f6e 652c 207a 5f66  ction1=None, z_f
-00053550: 7261 6374 696f 6e32 3d4e 6f6e 6529 3a0a  raction2=None):.
-00053560: 2020 2020 2222 220a 2020 2020 4465 7465      """.    Dete
-00053570: 726d 696e 6520 7472 616e 736c 6174 696f  rmine translatio
-00053580: 6e20 666f 7220 616c 6967 6e69 6e67 203c  n for aligning <
-00053590: 726f 6931 3e20 746f 203c 726f 6932 3e2e  roi1> to <roi2>.
-000535a0: 0a0a 2020 2020 2a2a 5061 7261 6d65 7465  ..    **Paramete
-000535b0: 7273 3a2a 2a0a 0a20 2020 2072 6f69 3120  rs:**..    roi1 
-000535c0: 3a20 524f 492f 5374 7275 6374 7572 6553  : ROI/StructureS
-000535d0: 6574 2f6c 6973 740a 2020 2020 2020 2020  et/list.        
-000535e0: 524f 4920 7468 6174 2069 7320 746f 2062  ROI that is to b
-000535f0: 6520 7472 616e 736c 6174 696f 6e20 746f  e translation to
-00053600: 2061 6368 6965 7665 2074 6865 2061 6c69   achieve the ali
-00053610: 676e 6d65 6e74 2e20 2054 6869 730a 2020  gnment.  This.  
-00053620: 2020 2020 2020 6361 6e20 6265 2073 7065        can be spe
-00053630: 6369 6669 6564 2064 6972 6563 746c 7920  cified directly 
-00053640: 6173 2061 2073 696e 676c 6520 524f 492e  as a single ROI.
-00053650: 2020 416c 7465 726e 6174 6976 656c 792c    Alternatively,
-00053660: 0a20 2020 2020 2020 2069 7420 6361 6e20  .        it can 
-00053670: 6265 2061 2053 7472 7563 7475 7265 5365  be a StructureSe
-00053680: 742c 206f 7220 6120 6c69 7374 206f 7220  t, or a list or 
-00053690: 524f 492f 5374 7275 6374 7572 6553 6574  ROI/StructureSet
-000536a0: 206f 626a 6563 7473 2c0a 2020 2020 2020   objects,.      
-000536b0: 2020 696e 2077 6869 6368 2063 6173 6520    in which case 
-000536c0: 7468 6520 696e 6469 7669 6475 616c 2052  the individual R
-000536d0: 4f49 7320 7769 6c6c 2062 6520 636f 6d62  OIs will be comb
-000536e0: 696e 6564 2e0a 0a20 2020 2072 6f69 3220  ined...    roi2 
-000536f0: 3a20 524f 492f 5374 7275 6374 7572 6553  : ROI/StructureS
-00053700: 6574 2f6c 6973 740a 2020 2020 2020 2020  et/list.        
-00053710: 524f 4920 7769 7468 2077 6869 6368 2061  ROI with which a
-00053720: 6c69 676e 6d65 6e74 2069 7320 746f 2062  lignment is to b
-00053730: 6520 7065 7266 6f72 6d65 642e 2020 5468  e performed.  Th
-00053740: 6973 2063 616e 2062 650a 2020 2020 2020  is can be.      
-00053750: 2020 7370 6563 6966 6965 6420 6469 7265    specified dire
-00053760: 6374 6c79 2061 7320 6120 7369 6e67 6c65  ctly as a single
-00053770: 2052 4f49 2e20 2041 6c74 6572 6e61 7469   ROI.  Alternati
-00053780: 7665 6c79 2c20 6974 2063 616e 0a20 2020  vely, it can.   
-00053790: 2020 2020 2062 6520 6120 5374 7275 6374       be a Struct
-000537a0: 7572 6553 6574 2c20 6f72 2061 206c 6973  ureSet, or a lis
-000537b0: 7420 6f72 2052 4f49 2f53 7472 7563 7475  t or ROI/Structu
-000537c0: 7265 5365 7420 6f62 6a65 6374 732c 0a20  reSet objects,. 
-000537d0: 2020 2020 2020 2069 6e20 7768 6963 6820         in which 
-000537e0: 6361 7365 2074 6865 2069 6e64 6976 6964  case the individ
-000537f0: 7561 6c20 524f 4973 2077 696c 6c20 6265  ual ROIs will be
-00053800: 2063 6f6d 6269 6e65 642e 0a0a 2020 2020   combined...    
-00053810: 7a5f 6672 6163 7469 6f6e 3120 3a20 666c  z_fraction1 : fl
-00053820: 6f61 742c 2064 6566 6175 6c74 3d4e 6f6e  oat, default=Non
-00053830: 650a 2020 2020 2020 2020 506f 7369 7469  e.        Positi
-00053840: 6f6e 2061 6c6f 6e67 207a 2061 7869 7320  on along z axis 
-00053850: 6f66 2073 6c69 6365 2074 6872 6f75 6768  of slice through
-00053860: 203c 726f 6931 3e20 6f6e 2077 6869 6368   <roi1> on which
-00053870: 0a20 2020 2020 2020 2074 6f20 616c 6967  .        to alig
-00053880: 6e2e 2020 4966 204e 6f6e 652c 2061 6c69  n.  If None, ali
-00053890: 676e 6d65 6e74 2069 7320 746f 2074 6865  gnment is to the
-000538a0: 2063 656e 7472 6f69 6420 6f66 2074 6865   centroid of the
-000538b0: 0a20 2020 2020 2020 2077 686f 6c65 2052  .        whole R
-000538c0: 4f49 2076 6f6c 756d 652e 2020 4f74 6865  OI volume.  Othe
-000538d0: 7277 6973 652c 2061 6c69 676e 6d65 6e74  rwise, alignment
-000538e0: 2069 7320 746f 2074 6865 0a20 2020 2020   is to the.     
-000538f0: 2020 2063 656e 7472 6f69 6420 6f66 2074     centroid of t
-00053900: 6865 2073 6c69 6365 2061 7420 7468 6520  he slice at the 
-00053910: 7370 6563 6966 6965 6420 6469 7374 616e  specified distan
-00053920: 6365 0a20 2020 2020 2020 2066 726f 6d20  ce.        from 
-00053930: 7468 6520 524f 4927 7320 6d6f 7374 2d69  the ROI's most-i
-00053940: 6e66 6572 696f 7220 706f 696e 743a 2030  nferior point: 0
-00053950: 2063 6f72 7265 7370 6f6e 6473 2074 6f0a   corresponds to.
-00053960: 2020 2020 2020 2020 7468 6520 6d6f 7374          the most
-00053970: 2d69 6e66 6572 696f 7220 706f 696e 7420  -inferior point 
-00053980: 286c 6f77 6573 7420 7a29 3b20 3120 636f  (lowest z); 1 co
-00053990: 7272 6573 706f 6e64 7320 746f 2074 6865  rresponds to the
-000539a0: 0a20 2020 2020 2020 206d 6f73 742d 7375  .        most-su
-000539b0: 7065 7269 6f72 2070 6f69 6e74 2028 6869  perior point (hi
-000539c0: 6768 6573 7420 7a29 2e20 2056 616c 7565  ghest z).  Value
-000539d0: 7320 666f 7220 7a5f 6672 6163 7469 6f6e  s for z_fraction
-000539e0: 0a20 2020 2020 2020 206f 7574 7369 6465  .        outside
-000539f0: 2074 6865 2069 6e74 6572 7661 6c20 5b30   the interval [0
-00053a00: 2c20 315d 2072 6573 756c 7420 696e 2061  , 1] result in a
-00053a10: 2052 756e 7469 6d65 4572 726f 722e 0a0a   RuntimeError...
-00053a20: 2020 2020 7a5f 6672 6163 7469 6f6e 3220      z_fraction2 
-00053a30: 3a20 666c 6f61 742c 2064 6566 6175 6c74  : float, default
-00053a40: 3d4e 6f6e 650a 2020 2020 2020 2020 506f  =None.        Po
-00053a50: 7369 7469 6f6e 2061 6c6f 6e67 207a 2061  sition along z a
-00053a60: 7869 7320 6f66 2073 6c69 6365 2074 6872  xis of slice thr
-00053a70: 6f75 6768 203c 726f 6932 3e20 6f6e 2077  ough <roi2> on w
-00053a80: 6869 6368 0a20 2020 2020 2020 2074 6f20  hich.        to 
-00053a90: 616c 6967 6e2e 2020 4966 204e 6f6e 652c  align.  If None,
-00053aa0: 2061 6c69 676e 6d65 6e74 2069 7320 746f   alignment is to
-00053ab0: 2074 6865 2063 656e 7472 6f69 6420 6f66   the centroid of
-00053ac0: 2074 6865 0a20 2020 2020 2020 2077 686f   the.        who
-00053ad0: 6c65 2052 4f49 2076 6f6c 756d 652e 2020  le ROI volume.  
-00053ae0: 4f74 6865 7277 6973 652c 2061 6c69 676e  Otherwise, align
-00053af0: 6d65 6e74 2069 7320 746f 2074 6865 0a20  ment is to the. 
-00053b00: 2020 2020 2020 2063 656e 7472 6f69 6420         centroid 
-00053b10: 6f66 2074 6865 2073 6c69 6365 2061 7420  of the slice at 
-00053b20: 7468 6520 7370 6563 6966 6965 6420 6469  the specified di
-00053b30: 7374 616e 6365 0a20 2020 2020 2020 2066  stance.        f
-00053b40: 726f 6d20 7468 6520 524f 4927 7320 6d6f  rom the ROI's mo
-00053b50: 7374 2d69 6e66 6572 696f 7220 706f 696e  st-inferior poin
-00053b60: 743a 2030 2063 6f72 7265 7370 6f6e 6473  t: 0 corresponds
-00053b70: 2074 6f0a 2020 2020 2020 2020 7468 6520   to.        the 
-00053b80: 6d6f 7374 2d69 6e66 6572 696f 7220 706f  most-inferior po
-00053b90: 696e 7420 286c 6f77 6573 7420 7a29 3b20  int (lowest z); 
-00053ba0: 3120 636f 7272 6573 706f 6e64 7320 746f  1 corresponds to
-00053bb0: 2074 6865 0a20 2020 2020 2020 206d 6f73   the.        mos
-00053bc0: 742d 7375 7065 7269 6f72 2070 6f69 6e74  t-superior point
-00053bd0: 2028 6869 6768 6573 7420 7a29 2e20 2056   (highest z).  V
-00053be0: 616c 7565 7320 666f 7220 7a5f 6672 6163  alues for z_frac
-00053bf0: 7469 6f6e 0a20 2020 2020 2020 206f 7574  tion.        out
-00053c00: 7369 6465 2074 6865 2069 6e74 6572 7661  side the interva
-00053c10: 6c20 5b30 2c20 315d 2072 6573 756c 7420  l [0, 1] result 
-00053c20: 696e 2061 2052 756e 7469 6d65 4572 726f  in a RuntimeErro
-00053c30: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-00053c40: 2020 2023 2043 7265 6174 6520 6c69 7374     # Create list
-00053c50: 206f 6620 7477 6f20 7369 6e67 6c65 2052   of two single R
-00053c60: 4f49 732e 0a20 2020 2072 6f69 7320 3d20  OIs..    rois = 
-00053c70: 5b5d 0a20 2020 2066 6f72 2072 6f69 2069  [].    for roi i
-00053c80: 6e20 5b72 6f69 312c 2072 6f69 325d 3a0a  n [roi1, roi2]:.
-00053c90: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00053ca0: 7461 6e63 6528 726f 692c 2052 4f49 293a  tance(roi, ROI):
-00053cb0: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00053cc0: 746f 7265 2073 696e 676c 6520 524f 4920  tore single ROI 
-00053cd0: 6469 7265 6374 6c79 2e0a 2020 2020 2020  directly..      
-00053ce0: 2020 2020 2020 726f 6973 2e61 7070 656e        rois.appen
-00053cf0: 6428 726f 6929 0a20 2020 2020 2020 2065  d(roi).        e
-00053d00: 6c69 6620 6973 696e 7374 616e 6365 2872  lif isinstance(r
-00053d10: 6f69 2c20 5374 7275 6374 7572 6553 6574  oi, StructureSet
-00053d20: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-00053d30: 2043 6f6d 6269 6e65 2052 4f49 7320 6f66   Combine ROIs of
-00053d40: 2053 7472 7563 7475 7265 5365 742e 0a20   StructureSet.. 
-00053d50: 2020 2020 2020 2020 2020 2072 6f69 732e             rois.
-00053d60: 6170 7065 6e64 2872 6f69 2e63 6f6d 6269  append(roi.combi
-00053d70: 6e65 5f72 6f69 7328 2929 0a20 2020 2020  ne_rois()).     
-00053d80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00053d90: 2020 2020 2023 2043 6f6d 6269 6e65 2052       # Combine R
-00053da0: 4f49 7320 6672 6f6d 206c 6973 742e 0a20  OIs from list.. 
-00053db0: 2020 2020 2020 2020 2020 2072 6f69 732e             rois.
-00053dc0: 6170 7065 6e64 2853 7472 7563 7475 7265  append(Structure
-00053dd0: 5365 7428 6765 745f 616c 6c5f 726f 6973  Set(get_all_rois
-00053de0: 2872 6f69 2929 2e63 6f6d 6269 6e65 5f72  (roi)).combine_r
-00053df0: 6f69 7328 2929 0a0a 2020 2020 2320 4361  ois())..    # Ca
-00053e00: 6c63 756c 6174 6520 616c 6967 6e6d 656e  lculate alignmen
-00053e10: 7420 706f 696e 7473 2e0a 2020 2020 6365  t points..    ce
-00053e20: 6e74 726f 6964 7320 3d20 5b5d 0a20 2020  ntroids = [].   
-00053e30: 2066 6f72 2072 6f69 2c20 7a5f 6672 6163   for roi, z_frac
-00053e40: 7469 6f6e 2069 6e20 7a69 7028 726f 6973  tion in zip(rois
-00053e50: 2c20 5b7a 5f66 7261 6374 696f 6e31 2c20  , [z_fraction1, 
-00053e60: 7a5f 6672 6163 7469 6f6e 325d 293a 0a20  z_fraction2]):. 
-00053e70: 2020 2020 2020 2023 2043 616c 6375 6c61         # Calcula
-00053e80: 7465 2063 656e 7472 6f69 6420 666f 7220  te centroid for 
-00053e90: 7468 6520 7768 6f6c 6520 524f 4920 766f  the whole ROI vo
-00053ea0: 6c75 6d65 2e0a 2020 2020 2020 2020 6966  lume..        if
-00053eb0: 207a 5f66 7261 6374 696f 6e20 6973 204e   z_fraction is N
-00053ec0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00053ed0: 2063 656e 7472 6f69 6473 2e61 7070 656e   centroids.appen
-00053ee0: 6428 726f 692e 6765 745f 6365 6e74 726f  d(roi.get_centro
-00053ef0: 6964 2829 290a 2020 2020 2020 2020 2320  id()).        # 
-00053f00: 4361 6c63 756c 6174 6520 6365 6e74 726f  Calculate centro
-00053f10: 6964 2066 6f72 2073 6c69 6365 2061 7420  id for slice at 
-00053f20: 7370 6563 6966 6965 6420 706f 7369 7469  specified positi
-00053f30: 6f6e 2e0a 2020 2020 2020 2020 656c 7365  on..        else
-00053f40: 3a0a 2020 2020 2020 2020 2020 2020 6365  :.            ce
-00053f50: 6e74 726f 6964 732e 6170 7065 6e64 2872  ntroids.append(r
-00053f60: 6f69 2e67 6574 5f72 6f69 5f73 6c69 6365  oi.get_roi_slice
-00053f70: 287a 5f66 7261 6374 696f 6e29 2e67 6574  (z_fraction).get
-00053f80: 5f63 656e 7472 6f69 6428 2929 0a0a 2020  _centroid())..  
-00053f90: 2020 7265 7475 726e 2074 7570 6c65 2863    return tuple(c
-00053fa0: 656e 7472 6f69 6473 5b31 5d20 2d20 6365  entroids[1] - ce
-00053fb0: 6e74 726f 6964 735b 305d 290a 0a64 6566  ntroids[0])..def
-00053fc0: 2067 6574 5f73 6c69 6365 5f70 6f73 6974   get_slice_posit
-00053fd0: 696f 6e73 2872 6f69 312c 2072 6f69 323d  ions(roi1, roi2=
-00053fe0: 4e6f 6e65 2c20 7669 6577 3d22 782d 7922  None, view="x-y"
-00053ff0: 2c20 706f 7369 7469 6f6e 5f61 735f 6964  , position_as_id
-00054000: 783d 4661 6c73 652c 0a20 2020 2020 2020  x=False,.       
-00054010: 206d 6574 686f 643d 4e6f 6e65 293a 0a20   method=None):. 
-00054020: 2020 2022 2222 0a20 2020 2047 6574 206f     """.    Get o
-00054030: 7264 6572 6564 206c 6973 7420 6f66 2073  rdered list of s
-00054040: 6c69 6365 2070 6f73 6974 696f 6e73 2066  lice positions f
-00054050: 6f72 2065 6974 6865 7220 6f72 2062 6f74  or either or bot
-00054060: 6820 6f66 2061 2070 6169 7220 6f66 2052  h of a pair of R
-00054070: 4f49 732e 0a0a 2020 2020 2a2a 5061 7261  OIs...    **Para
-00054080: 6d65 7465 7273 3a2a 2a0a 0a20 2020 2072  meters:**..    r
-00054090: 6f69 3120 3a20 736b 7274 2e73 7472 7563  oi1 : skrt.struc
-000540a0: 7475 7265 732e 524f 490a 2020 2020 2020  tures.ROI.      
-000540b0: 2020 524f 492c 206f 7220 6f6e 6520 6f66    ROI, or one of
-000540c0: 2061 2070 6169 7220 6f66 2052 4f49 732c   a pair of ROIs,
-000540d0: 2066 6f72 2077 6869 6368 2073 6c69 6365   for which slice
-000540e0: 2069 6e66 6f72 6d61 7469 6f6e 2069 7320   information is 
-000540f0: 746f 0a20 2020 2020 2020 2062 6520 6f62  to.        be ob
-00054100: 7461 696e 6564 2e0a 0a20 2020 2072 6f69  tained...    roi
-00054110: 3220 3a20 736b 7274 2e73 7472 7563 7475  2 : skrt.structu
-00054120: 7265 732e 524f 492c 2064 6566 6175 6c74  res.ROI, default
-00054130: 3d4e 6f6e 650a 2020 2020 2020 2020 4966  =None.        If
-00054140: 206e 6f74 204e 6f6e 652c 2073 6563 6f6e   not None, secon
-00054150: 6420 696e 2061 2070 6169 7220 6f66 2052  d in a pair of R
-00054160: 4f49 7320 666f 7220 7768 6963 6820 736c  OIs for which sl
-00054170: 6963 6520 696e 666f 726d 6174 696f 6e0a  ice information.
-00054180: 2020 2020 2020 2020 6973 2074 6f20 6265          is to be
-00054190: 206f 6274 6169 6e65 642e 0a0a 2020 2020   obtained...    
-000541a0: 7669 6577 203a 2073 7472 2c20 6465 6661  view : str, defa
-000541b0: 756c 743d 2278 2d79 220a 2020 2020 2020  ult="x-y".      
-000541c0: 2020 5669 6577 2069 6e20 7768 6963 6820    View in which 
-000541d0: 746f 206f 6274 6169 6e20 736c 6963 6573  to obtain slices
-000541e0: 2e0a 0a20 2020 2070 6f73 6974 696f 6e5f  ...    position_
-000541f0: 6173 5f69 6478 203a 2062 6f6f 6c2c 2064  as_idx : bool, d
-00054200: 6566 6175 6c74 3d46 616c 7365 0a20 2020  efault=False.   
-00054210: 2020 2020 2049 6620 5472 7565 2c20 7265       If True, re
-00054220: 7475 726e 2070 6f73 6974 696f 6e73 2061  turn positions a
-00054230: 7320 736c 6963 6520 696e 6469 6365 733b  s slice indices;
-00054240: 2069 6620 4661 6c73 652c 0a20 2020 2020   if False,.     
-00054250: 2020 2072 6574 7572 6e20 706f 7369 7469     return positi
-00054260: 6f6e 7320 6173 2073 6c69 6365 207a 2d63  ons as slice z-c
-00054270: 6f6f 7264 696e 6174 6573 2028 6d6d 292e  oordinates (mm).
-00054280: 0a0a 2020 2020 6d65 7468 6f64 3a20 7374  ..    method: st
-00054290: 722c 2064 6566 6175 6c74 3d4e 6f6e 650a  r, default=None.
-000542a0: 2020 2020 2020 2020 5374 7269 6e67 2073          String s
-000542b0: 7065 6369 6679 696e 6720 736c 6963 6573  pecifying slices
-000542c0: 2066 6f72 2077 6869 6368 2070 6f73 6974   for which posit
-000542d0: 696f 6e73 2061 7265 2074 6f20 6265 206f  ions are to be o
-000542e0: 6274 6169 6e65 642c 0a20 2020 2020 2020  btained,.       
-000542f0: 2066 6f72 2052 4f49 7320 726f 6931 2c20   for ROIs roi1, 
-00054300: 726f 6932 3a0a 0a20 2020 2020 2020 202d  roi2:..        -
-00054310: 2022 6c65 6674 2220 286f 7220 726f 6932   "left" (or roi2
-00054320: 2069 7320 4e6f 6e65 293a 2072 6574 7572   is None): retur
-00054330: 6e20 706f 7369 7469 6f6e 7320 6f66 2073  n positions of s
-00054340: 6c69 6365 7320 636f 6e74 6169 6e69 6e67  lices containing
-00054350: 2072 6f69 313b 0a20 2020 2020 2020 202d   roi1;.        -
-00054360: 2022 7269 6768 7422 3a20 7265 7475 726e   "right": return
-00054370: 2070 6f73 6974 696f 6e73 206f 6620 736c   positions of sl
-00054380: 6963 6573 2063 6f6e 7461 696e 696e 6720  ices containing 
-00054390: 726f 6932 3b0a 2020 2020 2020 2020 2d20  roi2;.        - 
-000543a0: 2275 6e69 6f6e 223a 2072 6574 7572 6e20  "union": return 
-000543b0: 706f 7369 7469 6f6e 7320 6f66 2073 6c69  positions of sli
-000543c0: 6365 7320 636f 6e74 6169 6e69 6e67 2065  ces containing e
-000543d0: 6974 6865 7220 726f 6931 206f 7220 726f  ither roi1 or ro
-000543e0: 6932 3b0a 2020 2020 2020 2020 2d20 2269  i2;.        - "i
-000543f0: 6e74 6572 7365 6374 696f 6e22 3a20 7265  ntersection": re
-00054400: 7475 726e 2070 6f73 6974 696f 6e73 206f  turn positions o
-00054410: 6620 736c 6963 6573 2063 6f6e 7461 696e  f slices contain
-00054420: 696e 6720 626f 7468 0a20 2020 2020 2020  ing both.       
-00054430: 2020 2072 6f69 3120 616e 6420 726f 6932     roi1 and roi2
-00054440: 2e0a 0a20 2020 2020 2020 2049 6620 4e6f  ...        If No
-00054450: 6e65 2c20 7661 6c75 6520 6f66 2073 6b72  ne, value of skr
-00054460: 742e 636f 7265 2e44 6566 6175 6c74 7328  t.core.Defaults(
-00054470: 292e 6279 5f73 6c69 6365 2069 7320 7573  ).by_slice is us
-00054480: 6564 2e0a 2020 2020 2222 220a 2020 2020  ed..    """.    
-00054490: 6d65 7468 6f64 203d 206d 6574 686f 6420  method = method 
-000544a0: 6f72 2073 6b72 742e 636f 7265 2e44 6566  or skrt.core.Def
-000544b0: 6175 6c74 7328 292e 6279 5f73 6c69 6365  aults().by_slice
-000544c0: 0a20 2020 2069 6620 6d65 7468 6f64 206e  .    if method n
-000544d0: 6f74 2069 6e20 6765 745f 6279 5f73 6c69  ot in get_by_sli
-000544e0: 6365 5f6d 6574 686f 6473 2829 3a0a 2020  ce_methods():.  
-000544f0: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-00054500: 696d 6545 7272 6f72 2866 224d 6574 686f  imeError(f"Metho
-00054510: 6420 6d75 7374 2062 6520 6f6e 6520 6f66  d must be one of
-00054520: 207b 6765 745f 6279 5f73 6c69 6365 5f6d   {get_by_slice_m
-00054530: 6574 686f 6473 2829 7d22 0a20 2020 2020  ethods()}".     
-00054540: 2020 2022 202d 206e 6f74 2027 7b6d 6574     " - not '{met
-00054550: 686f 647d 2722 290a 0a20 2020 2069 6e64  hod}'")..    ind
-00054560: 6963 6573 203d 204e 6f6e 650a 0a20 2020  ices = None..   
-00054570: 2069 6e64 6963 6573 3120 3d20 726f 6931   indices1 = roi1
-00054580: 2e67 6574 5f69 6e64 6963 6573 2876 6965  .get_indices(vie
-00054590: 773d 7669 6577 2c20 6d65 7468 6f64 3d22  w=view, method="
-000545a0: 6d61 736b 2229 0a20 2020 2069 6620 6e6f  mask").    if no
-000545b0: 7420 6973 7375 6263 6c61 7373 2874 7970  t issubclass(typ
-000545c0: 6528 726f 6932 292c 2052 4f49 2920 6f72  e(roi2), ROI) or
-000545d0: 2022 6c65 6674 2220 3d3d 206d 6574 686f   "left" == metho
-000545e0: 643a 0a20 2020 2020 2020 2069 6e64 6963  d:.        indic
-000545f0: 6573 203d 2069 6e64 6963 6573 310a 0a20  es = indices1.. 
-00054600: 2020 2069 6620 696e 6469 6365 7320 6973     if indices is
-00054610: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
-00054620: 6e64 6963 6573 3220 3d20 726f 6932 2e67  ndices2 = roi2.g
-00054630: 6574 5f69 6e64 6963 6573 2876 6965 773d  et_indices(view=
-00054640: 7669 6577 2c20 6d65 7468 6f64 3d22 6d61  view, method="ma
-00054650: 736b 2229 0a20 2020 2020 2020 2069 6620  sk").        if 
-00054660: 2272 6967 6874 2220 3d3d 206d 6574 686f  "right" == metho
-00054670: 643a 0a20 2020 2020 2020 2020 2020 2069  d:.            i
-00054680: 6e64 6963 6573 203d 2069 6e64 6963 6573  ndices = indices
-00054690: 320a 2020 2020 2020 2020 0a20 2020 2069  2.        .    i
-000546a0: 6620 696e 6469 6365 7320 6973 204e 6f6e  f indices is Non
-000546b0: 653a 0a20 2020 2020 2020 2069 6620 2275  e:.        if "u
-000546c0: 6e69 6f6e 2220 3d3d 206d 6574 686f 643a  nion" == method:
-000546d0: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
-000546e0: 6963 6573 203d 206c 6973 7428 7365 7428  ices = list(set(
-000546f0: 696e 6469 6365 7331 292e 756e 696f 6e28  indices1).union(
-00054700: 7365 7428 696e 6469 6365 7332 2929 290a  set(indices2))).
-00054710: 0a20 2020 2069 6620 696e 6469 6365 7320  .    if indices 
-00054720: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00054730: 2069 6620 2269 6e74 6572 7365 6374 696f   if "intersectio
-00054740: 6e22 203d 3d20 6d65 7468 6f64 3a0a 2020  n" == method:.  
-00054750: 2020 2020 2020 2020 2020 696e 6469 6365            indice
-00054760: 7320 3d20 6c69 7374 2873 6574 2869 6e64  s = list(set(ind
-00054770: 6963 6573 3129 2e69 6e74 6572 7365 6374  ices1).intersect
-00054780: 696f 6e28 7365 7428 696e 6469 6365 7332  ion(set(indices2
-00054790: 2929 290a 0a20 2020 2069 6620 696e 6469  )))..    if indi
-000547a0: 6365 7320 6973 206e 6f74 204e 6f6e 653a  ces is not None:
-000547b0: 0a20 2020 2020 2020 2069 6620 706f 7369  .        if posi
-000547c0: 7469 6f6e 5f61 735f 6964 783a 0a20 2020  tion_as_idx:.   
-000547d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000547e0: 736f 7274 6564 2869 6e64 6963 6573 290a  sorted(indices).
-000547f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00054800: 2020 2020 2020 2020 2020 6178 203d 2073            ax = s
-00054810: 6b72 742e 696d 6167 652e 5f73 6c69 6365  krt.image._slice
-00054820: 5f61 7865 735b 7669 6577 5d0a 2020 2020  _axes[view].    
-00054830: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00054840: 6f72 7465 6428 5b72 6f69 312e 6964 785f  orted([roi1.idx_
-00054850: 746f 5f70 6f73 2869 6478 2c20 6178 2920  to_pos(idx, ax) 
-00054860: 666f 7220 6964 7820 696e 2069 6e64 6963  for idx in indic
-00054870: 6573 5d29 0a0a 6465 6620 6578 7061 6e64  es])..def expand
-00054880: 5f73 6c69 6365 5f73 7461 7473 2873 6c69  _slice_stats(sli
-00054890: 6365 5f73 7461 7473 3d4e 6f6e 652c 2064  ce_stats=None, d
-000548a0: 6566 6175 6c74 5f62 795f 736c 6963 653d  efault_by_slice=
-000548b0: 4e6f 6e65 293a 0a20 2020 2022 2222 0a20  None):.    """. 
-000548c0: 2020 2045 7870 616e 6420 7370 6563 6966     Expand specif
-000548d0: 6963 6174 696f 6e20 6f66 2073 7461 7469  ication of stati
-000548e0: 7374 6963 7320 746f 2063 616c 6375 6c61  stics to calcula
-000548f0: 7465 2066 6f72 2052 4f49 2063 6f6d 7061  te for ROI compa
-00054900: 7269 736f 6e0a 2020 2020 6d65 7472 6963  rison.    metric
-00054910: 7320 6576 616c 7561 7465 6420 736c 6963  s evaluated slic
-00054920: 6520 6279 2073 6c69 6365 2e0a 0a20 2020  e by slice...   
-00054930: 2041 2064 6963 7469 6f6e 6172 7920 6973   A dictionary is
-00054940: 2072 6574 7572 6e65 642c 2077 6865 7265   returned, where
-00054950: 206b 6579 7320 6769 7665 2074 6865 2073   keys give the s
-00054960: 6c69 6365 7320 746f 2062 6520 636f 6e73  lices to be cons
-00054970: 6964 6572 6564 0a20 2020 2066 6f72 2063  idered.    for c
-00054980: 616c 6375 6c61 7469 6e67 2073 7461 7469  alculating stati
-00054990: 7374 6963 732c 2061 6e64 2076 616c 7565  stics, and value
-000549a0: 7320 6172 6520 6c69 7374 7320 6f66 206d  s are lists of m
-000549b0: 6574 7269 6373 2e0a 0a20 2020 202a 2a50  etrics...    **P
-000549c0: 6172 616d 6574 6572 733a 2a2a 0a0a 2020  arameters:**..  
-000549d0: 2020 736c 6963 655f 7374 6174 7320 3a20    slice_stats : 
-000549e0: 7374 722f 6c69 7374 2f64 6963 742c 2064  str/list/dict, d
-000549f0: 6566 6175 6c74 3d4e 6f6e 650a 2020 2020  efault=None.    
-00054a00: 2020 2020 5370 6563 6966 6963 6174 696f      Specificatio
-00054a10: 6e20 6f66 2073 7461 7469 7374 6963 7320  n of statistics 
-00054a20: 746f 2062 6520 6361 6c63 756c 6174 6564  to be calculated
-00054a30: 2072 656c 6174 6976 650a 2020 2020 2020   relative.      
-00054a40: 2020 746f 2073 6c69 6365 2d62 792d 736c    to slice-by-sl
-00054a50: 6963 6520 6d65 7472 6963 2076 616c 7565  ice metric value
-00054a60: 732e 0a0a 2020 2020 2020 2020 4120 7374  s...        A st
-00054a70: 6174 6973 7469 6320 6973 2073 7065 6369  atistic is speci
-00054a80: 6669 6564 2062 7920 7468 6520 6e61 6d65  fied by the name
-00054a90: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
-00054aa0: 2066 6f72 0a20 2020 2020 2020 2069 7473   for.        its
-00054ab0: 2063 616c 6375 6c61 7469 6f6e 2069 6e20   calculation in 
-00054ac0: 7468 6520 5079 7468 6f6e 2073 7461 7469  the Python stati
-00054ad0: 7374 6963 7320 6d6f 6475 6c65 3a0a 0a20  stics module:.. 
-00054ae0: 2020 2020 2020 2068 7474 7073 3a2f 2f64         https://d
-00054af0: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
-00054b00: 2f6c 6962 7261 7279 2f73 7461 7469 7374  /library/statist
-00054b10: 6963 732e 6874 6d6c 0a0a 2020 2020 2020  ics.html..      
-00054b20: 2020 466f 7220 6974 7320 7573 6520 6865    For its use he
-00054b30: 7265 2c20 7468 6520 7265 6c65 7661 6e74  re, the relevant
-00054b40: 2066 756e 6374 696f 6e20 6d75 7374 2072   function must r
-00054b50: 6571 7569 7265 0a20 2020 2020 2020 2061  equire.        a
-00054b60: 2073 696e 676c 652d 7661 7269 6162 6c65   single-variable
-00054b70: 2069 6e70 7574 2c20 6d75 7374 206e 6f74   input, must not
-00054b80: 2072 6571 7569 7265 2061 6e79 206b 6579   require any key
-00054b90: 776f 7264 0a20 2020 2020 2020 2061 7267  word.        arg
-00054ba0: 756d 656e 7473 2c20 616e 6420 6d75 7374  uments, and must
-00054bb0: 2072 6574 7572 6e20 6120 7369 6e67 6c65   return a single
-00054bc0: 206e 756d 6265 722e 0a0a 2020 2020 2020   number...      
-00054bd0: 2020 4176 6169 6c61 626c 6520 6f70 7469    Available opti
-00054be0: 6f6e 7320 696e 636c 7564 653a 2022 6d65  ons include: "me
-00054bf0: 616e 222c 2022 6d65 6469 616e 222c 2022  an", "median", "
-00054c00: 6d6f 6465 222c 0a20 2020 2020 2020 2022  mode",.        "
-00054c10: 7374 6465 7622 2e0a 0a20 2020 2020 2020  stdev"...       
-00054c20: 5374 6174 6973 7469 6373 2074 6f20 6265  Statistics to be
-00054c30: 2063 616c 6375 6c61 7465 6420 6361 6e20   calculated can 
-00054c40: 6265 2073 7065 6369 6669 6564 2075 7369  be specified usi
-00054c50: 6e67 2061 6e79 206f 660a 2020 2020 2020  ng any of.      
-00054c60: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
-00054c70: 0a20 2020 2020 2020 2d20 5374 7269 6e67  .       - String
-00054c80: 2073 7065 6369 6679 696e 6720 7369 6e67   specifying sing
-00054c90: 6c65 2073 7461 7469 7374 6963 2074 6f20  le statistic to 
-00054ca0: 6265 2063 616c 6375 6c61 7465 642c 0a20  be calculated,. 
-00054cb0: 2020 2020 2020 2020 7769 7468 2073 6c69          with sli
-00054cc0: 6365 7320 636f 6e73 6964 6572 6564 2061  ces considered a
-00054cd0: 7320 6769 7665 6e20 6279 203c 6465 6661  s given by <defa
-00054ce0: 756c 745f 6279 5f73 6c69 6365 3e2c 0a20  ult_by_slice>,. 
-00054cf0: 2020 2020 2020 2020 666f 7220 6578 616d          for exam
-00054d00: 706c 653a 2022 6d65 616e 223b 0a20 2020  ple: "mean";.   
-00054d10: 2020 2020 2d20 4c69 7374 2073 7065 6369      - List speci
-00054d20: 6679 696e 6720 6d75 6c74 6970 6c65 2073  fying multiple s
-00054d30: 7461 7469 7374 6963 7320 746f 2062 6520  tatistics to be 
-00054d40: 6361 6c63 756c 6174 6564 2c0a 2020 2020  calculated,.    
-00054d50: 2020 2020 2077 6974 6820 736c 6963 6573       with slices
-00054d60: 2063 6f6e 7369 6465 7265 6420 6173 2067   considered as g
-00054d70: 6976 656e 2062 7920 3c64 6566 6175 6c74  iven by <default
-00054d80: 5f62 795f 736c 6963 653e 2c0a 2020 2020  _by_slice>,.    
-00054d90: 2020 2020 2066 6f72 2065 7861 6d70 6c65       for example
-00054da0: 3a20 5b22 6d65 616e 222c 2022 7374 6465  : ["mean", "stde
-00054db0: 7622 5d3b 0a20 2020 2020 2020 2d20 4469  v"];.       - Di
-00054dc0: 6374 696f 6e61 7279 2077 6865 7265 206b  ctionary where k
-00054dd0: 6579 7320 7370 6563 6966 7920 736c 6963  eys specify slic
-00054de0: 6573 2074 6f20 6265 2063 6f6e 7369 6465  es to be conside
-00054df0: 7265 642c 0a20 2020 2020 2020 2020 616e  red,.         an
-00054e00: 6420 7661 6c75 6573 2073 7065 6369 6679  d values specify
-00054e10: 2073 7461 7469 7374 6963 7320 2873 7472   statistics (str
-00054e20: 696e 6720 6f72 206c 6973 7429 2c20 666f  ing or list), fo
-00054e30: 720a 2020 2020 2020 2020 2065 7861 6d70  r.         examp
-00054e40: 6c65 3a20 7b22 756e 696f 6e22 3a20 5b22  le: {"union": ["
-00054e50: 6d65 616e 222c 2022 7374 6465 7622 5d7d  mean", "stdev"]}
-00054e60: 2e20 2056 616c 6964 2073 6c69 6365 0a20  .  Valid slice. 
-00054e70: 2020 2020 2020 2020 7370 6563 6966 6963          specific
-00054e80: 6174 696f 6e73 2061 7265 2061 7320 6c69  ations are as li
-00054e90: 7374 6564 2066 6f72 203c 6465 6661 756c  sted for <defaul
-00054ea0: 745f 6279 5f73 6c69 6365 3e2e 0a0a 2020  t_by_slice>...  
-00054eb0: 2020 6465 6661 756c 745f 6279 5f73 6c69    default_by_sli
-00054ec0: 6365 3a20 7374 722c 2064 6566 6175 6c74  ce: str, default
-00054ed0: 3d4e 6f6e 650a 2020 2020 2020 2020 4465  =None.        De
-00054ee0: 6661 756c 7420 7370 6563 6966 6963 6174  fault specificat
-00054ef0: 696f 6e20 6f66 2073 6c69 6365 7320 746f  ion of slices to
-00054f00: 2062 6520 636f 6e73 6964 6572 6564 2077   be considered w
-00054f10: 6865 6e0a 2020 2020 2020 2020 6361 6c63  hen.        calc
-00054f20: 756c 6174 696e 6720 736c 6963 652d 6279  ulating slice-by
-00054f30: 2d73 6c69 6365 2073 7461 7469 7374 6963  -slice statistic
-00054f40: 7320 666f 7220 6120 6d65 7472 6963 2063  s for a metric c
-00054f50: 6f6d 7061 7269 6e67 0a20 2020 2020 2020  omparing.       
-00054f60: 2074 776f 2052 4f49 732c 2072 6f69 3120   two ROIs, roi1 
-00054f70: 616e 6420 726f 6932 2e20 2054 6865 2076  and roi2.  The v
-00054f80: 616c 6964 2073 7065 6369 6669 6361 7469  alid specificati
-00054f90: 6f6e 7320 6172 653a 0a0a 2020 2020 2020  ons are:..      
-00054fa0: 2020 2d20 226c 6566 7422 3a20 636f 6e73    - "left": cons
-00054fb0: 6964 6572 206f 6e6c 7920 736c 6963 6573  ider only slices
-00054fc0: 2063 6f6e 7461 696e 696e 6720 726f 6931   containing roi1
-00054fd0: 3b0a 2020 2020 2020 2020 2d20 2272 6967  ;.        - "rig
-00054fe0: 6874 223a 2063 6f6e 7369 6465 7220 6f6e  ht": consider on
-00054ff0: 6c79 2073 6c69 6365 7320 636f 6e74 6169  ly slices contai
-00055000: 6e69 6e67 2072 6f69 323b 0a20 2020 2020  ning roi2;.     
-00055010: 2020 202d 2022 756e 696f 6e22 3a20 636f     - "union": co
-00055020: 6e73 6964 6572 2073 6c69 6365 7320 636f  nsider slices co
-00055030: 6e74 6169 6e69 6e67 2065 6974 6865 7220  ntaining either 
-00055040: 6f66 2072 6f69 3120 616e 6420 726f 6932  of roi1 and roi2
-00055050: 3b0a 2020 2020 2020 2020 2d20 2269 6e74  ;.        - "int
-00055060: 6572 7365 6374 696f 6e22 3a20 636f 6e73  ersection": cons
-00055070: 6964 6572 2073 6c69 6365 7320 636f 6e74  ider slices cont
-00055080: 6169 6e69 6e67 2062 6f74 6820 726f 6931  aining both roi1
-00055090: 2061 6e64 2072 6f69 322e 0a0a 2020 2020   and roi2...    
-000550a0: 2020 2020 4966 204e 6f6e 652c 2075 7365      If None, use
-000550b0: 2073 6b72 742e 636f 7265 2e44 6566 6175   skrt.core.Defau
-000550c0: 6c74 7328 292e 6279 5f73 6c69 6365 0a20  lts().by_slice. 
-000550d0: 2020 2022 2222 0a20 2020 2069 6620 6e6f     """.    if no
-000550e0: 7420 736c 6963 655f 7374 6174 733a 0a20  t slice_stats:. 
-000550f0: 2020 2020 2020 2072 6574 7572 6e20 7b7d         return {}
-00055100: 0a0a 2020 2020 2320 5365 7420 6465 6661  ..    # Set defa
-00055110: 756c 7420 6d65 7468 6f64 2066 6f72 2073  ult method for s
-00055120: 6c69 6365 2073 656c 6563 7469 6f6e 2e0a  lice selection..
-00055130: 2020 2020 6465 6661 756c 745f 6279 5f73      default_by_s
-00055140: 6c69 6365 203d 2064 6566 6175 6c74 5f62  lice = default_b
-00055150: 795f 736c 6963 6520 6f72 2073 6b72 742e  y_slice or skrt.
-00055160: 636f 7265 2e44 6566 6175 6c74 7328 292e  core.Defaults().
-00055170: 6279 5f73 6c69 6365 0a0a 2020 2020 2320  by_slice..    # 
-00055180: 456e 7375 7265 2074 6861 7420 736c 6963  Ensure that slic
-00055190: 655f 7374 6174 7320 6973 2061 2064 6963  e_stats is a dic
-000551a0: 7469 6f6e 6172 792e 0a20 2020 2069 6620  tionary..    if 
-000551b0: 6973 696e 7374 616e 6365 2873 6c69 6365  isinstance(slice
-000551c0: 5f73 7461 7473 2c20 7374 7229 3a0a 2020  _stats, str):.  
-000551d0: 2020 2020 2020 736c 6963 655f 7374 6174        slice_stat
-000551e0: 7320 3d20 7b64 6566 6175 6c74 5f62 795f  s = {default_by_
-000551f0: 736c 6963 653a 205b 736c 6963 655f 7374  slice: [slice_st
-00055200: 6174 735d 7d0a 0a20 2020 2065 6c69 6620  ats]}..    elif 
-00055210: 736b 7274 2e63 6f72 652e 6973 5f6c 6973  skrt.core.is_lis
-00055220: 7428 736c 6963 655f 7374 6174 7329 3a0a  t(slice_stats):.
-00055230: 2020 2020 2020 2020 736c 6963 655f 7374          slice_st
-00055240: 6174 7320 3d20 7b64 6566 6175 6c74 5f62  ats = {default_b
-00055250: 795f 736c 6963 653a 2073 6c69 6365 5f73  y_slice: slice_s
-00055260: 7461 7473 7d0a 0a20 2020 2065 6c69 6620  tats}..    elif 
-00055270: 6973 696e 7374 616e 6365 2873 6c69 6365  isinstance(slice
-00055280: 5f73 7461 7473 2c20 6469 6374 293a 0a20  _stats, dict):. 
-00055290: 2020 2020 2020 2063 6865 636b 6564 5f73         checked_s
-000552a0: 6c69 6365 5f73 7461 7473 203d 207b 7d0a  lice_stats = {}.
-000552b0: 2020 2020 2020 2020 666f 7220 6279 5f73          for by_s
-000552c0: 6c69 6365 2c20 7374 6174 7320 696e 2073  lice, stats in s
-000552d0: 6c69 6365 5f73 7461 7473 2e69 7465 6d73  lice_stats.items
-000552e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000552f0: 6966 2069 7369 6e73 7461 6e63 6528 7374  if isinstance(st
-00055300: 6174 732c 2073 7472 293a 0a20 2020 2020  ats, str):.     
-00055310: 2020 2020 2020 2020 2020 2063 6865 636b             check
-00055320: 6564 5f73 6c69 6365 5f73 7461 7473 5b62  ed_slice_stats[b
-00055330: 795f 736c 6963 655d 203d 205b 7374 6174  y_slice] = [stat
-00055340: 735d 0a20 2020 2020 2020 2020 2020 2065  s].            e
-00055350: 6c69 6620 736b 7274 2e63 6f72 652e 6973  lif skrt.core.is
-00055360: 5f6c 6973 7428 7374 6174 7329 3a0a 2020  _list(stats):.  
-00055370: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00055380: 6563 6b65 645f 736c 6963 655f 7374 6174  ecked_slice_stat
-00055390: 735b 6279 5f73 6c69 6365 5d20 3d20 6c69  s[by_slice] = li
-000553a0: 7374 2873 7461 7473 290a 2020 2020 2020  st(stats).      
-000553b0: 2020 736c 6963 655f 7374 6174 7320 3d20    slice_stats = 
-000553c0: 6368 6563 6b65 645f 736c 6963 655f 7374  checked_slice_st
-000553d0: 6174 730a 0a20 2020 2069 6620 6973 696e  ats..    if isin
-000553e0: 7374 616e 6365 2873 6c69 6365 5f73 7461  stance(slice_sta
-000553f0: 7473 2c20 6469 6374 293a 0a20 2020 2020  ts, dict):.     
-00055400: 2020 2072 6574 7572 6e20 736c 6963 655f     return slice_
-00055410: 7374 6174 730a 0a20 2020 2072 6574 7572  stats..    retur
-00055420: 6e20 7b7d 0a                             n {}.
+000525c0: 226a 6163 6361 7264 222c 0a20 2020 2020  "jaccard",.     
+000525d0: 2020 2020 2020 2022 6a61 6363 6172 645f         "jaccard_
+000525e0: 666c 6174 222c 0a20 2020 2020 2020 2020  flat",.         
+000525f0: 2020 2022 6a61 6363 6172 645f 736c 6963     "jaccard_slic
+00052600: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00052610: 226a 6163 6361 7264 5f73 6c69 6365 5f73  "jaccard_slice_s
+00052620: 7461 7473 222c 0a20 2020 2020 2020 2020  tats",.         
+00052630: 2020 2022 6d65 616e 5f64 6973 7461 6e63     "mean_distanc
+00052640: 655f 746f 5f63 6f6e 666f 726d 6974 7922  e_to_conformity"
+00052650: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+00052660: 6561 6e5f 6469 7374 616e 6365 5f74 6f5f  ean_distance_to_
+00052670: 636f 6e66 6f72 6d69 7479 5f66 6c61 7422  conformity_flat"
+00052680: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+00052690: 6561 6e5f 7369 676e 6564 5f73 7572 6661  ean_signed_surfa
+000526a0: 6365 5f64 6973 7461 6e63 6522 2c0a 2020  ce_distance",.  
+000526b0: 2020 2020 2020 2020 2020 226d 6561 6e5f            "mean_
+000526c0: 7369 676e 6564 5f73 7572 6661 6365 5f64  signed_surface_d
+000526d0: 6973 7461 6e63 655f 666c 6174 222c 0a20  istance_flat",. 
+000526e0: 2020 2020 2020 2020 2020 2022 6d65 616e             "mean
+000526f0: 5f73 7572 6661 6365 5f64 6973 7461 6e63  _surface_distanc
+00052700: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00052710: 226d 6561 6e5f 7375 7266 6163 655f 6469  "mean_surface_di
+00052720: 7374 616e 6365 5f66 6c61 7422 2c0a 2020  stance_flat",.  
+00052730: 2020 2020 2020 2020 2020 226d 6561 6e5f            "mean_
+00052740: 6f76 6572 5f63 6f6e 746f 7572 696e 6722  over_contouring"
+00052750: 2c0a 2020 2020 2020 2020 2020 2020 226d  ,.            "m
+00052760: 6561 6e5f 6f76 6572 5f63 6f6e 746f 7572  ean_over_contour
+00052770: 696e 675f 666c 6174 222c 0a20 2020 2020  ing_flat",.     
+00052780: 2020 2020 2020 2022 6d65 616e 5f75 6e64         "mean_und
+00052790: 6572 5f63 6f6e 746f 7572 696e 6722 2c0a  er_contouring",.
+000527a0: 2020 2020 2020 2020 2020 2020 226d 6561              "mea
+000527b0: 6e5f 756e 6465 725f 636f 6e74 6f75 7269  n_under_contouri
+000527c0: 6e67 5f66 6c61 7422 2c0a 2020 2020 2020  ng_flat",.      
+000527d0: 2020 2020 2020 2272 656c 5f61 7265 615f        "rel_area_
+000527e0: 6469 6666 222c 0a20 2020 2020 2020 2020  diff",.         
+000527f0: 2020 2022 7265 6c5f 6172 6561 5f64 6966     "rel_area_dif
+00052800: 665f 666c 6174 222c 0a20 2020 2020 2020  f_flat",.       
+00052810: 2020 2020 2022 7265 6c5f 6172 6561 5f64       "rel_area_d
+00052820: 6966 665f 736c 6963 655f 7374 6174 7322  iff_slice_stats"
+00052830: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+00052840: 656c 5f76 6f6c 756d 655f 6469 6666 222c  el_volume_diff",
+00052850: 0a20 2020 2020 2020 2020 2020 2022 726d  .            "rm
+00052860: 735f 7369 676e 6564 5f73 7572 6661 6365  s_signed_surface
+00052870: 5f64 6973 7461 6e63 6522 2c0a 2020 2020  _distance",.    
+00052880: 2020 2020 2020 2020 2272 6d73 5f73 6967          "rms_sig
+00052890: 6e65 645f 7375 7266 6163 655f 6469 7374  ned_surface_dist
+000528a0: 616e 6365 5f66 6c61 7422 2c0a 2020 2020  ance_flat",.    
+000528b0: 2020 2020 2020 2020 2272 6d73 5f73 7572          "rms_sur
+000528c0: 6661 6365 5f64 6973 7461 6e63 6522 2c0a  face_distance",.
+000528d0: 2020 2020 2020 2020 2020 2020 2272 6d73              "rms
+000528e0: 5f73 7572 6661 6365 5f64 6973 7461 6e63  _surface_distanc
+000528f0: 655f 666c 6174 222c 0a20 2020 2020 2020  e_flat",.       
+00052900: 2020 2020 2022 766f 6c75 6d65 5f64 6966       "volume_dif
+00052910: 6622 2c0a 2020 2020 2020 2020 2020 2020  f",.            
+00052920: 2276 6f6c 756d 655f 7261 7469 6f22 2c0a  "volume_ratio",.
+00052930: 2020 2020 2020 2020 2020 2020 5d0a 0a20              ].. 
+00052940: 2020 2023 2052 6570 6c61 6365 2063 656e     # Replace cen
+00052950: 7472 6f69 6420 7665 6374 6f72 7320 6279  troid vectors by
+00052960: 2063 6f6d 706f 6e65 6e74 732e 0a20 2020   components..   
+00052970: 2069 6620 6365 6e74 726f 6964 5f63 6f6d   if centroid_com
+00052980: 706f 6e65 6e74 733a 0a20 2020 2020 2020  ponents:.       
+00052990: 2063 656e 7472 6f69 6473 203d 207b 0a20   centroids = {. 
+000529a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000529b0: 6365 6e74 726f 6964 223a 205b 2263 656e  centroid": ["cen
+000529c0: 7472 6f69 645f 7822 2c20 2263 656e 7472  troid_x", "centr
+000529d0: 6f69 645f 7922 2c20 2263 656e 7472 6f69  oid_y", "centroi
+000529e0: 645f 7a22 5d2c 0a20 2020 2020 2020 2020  d_z"],.         
+000529f0: 2020 2020 2020 2022 6365 6e74 726f 6964         "centroid
+00052a00: 5f73 6c69 6365 223a 205b 5d0a 2020 2020  _slice": [].    
+00052a10: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00052a20: 2020 2020 2020 6966 2073 6c69 6365 5f73        if slice_s
+00052a30: 7461 7473 2069 7320 6e6f 7420 4e6f 6e65  tats is not None
+00052a40: 3a0a 2020 2020 2020 2020 2020 2020 6365  :.            ce
+00052a50: 6e74 726f 6964 735b 2263 656e 7472 6f69  ntroids["centroi
+00052a60: 645f 736c 6963 655f 7374 6174 7322 5d20  d_slice_stats"] 
+00052a70: 3d20 5b5d 0a0a 2020 2020 2020 2020 666f  = []..        fo
+00052a80: 7220 695f 6178 2069 6e20 736b 7274 2e69  r i_ax in skrt.i
+00052a90: 6d61 6765 2e5f 706c 6f74 5f61 7865 735b  mage._plot_axes[
+00052aa0: 7669 6577 5d3a 0a20 2020 2020 2020 2020  view]:.         
+00052ab0: 2020 2061 7820 3d20 736b 7274 2e69 6d61     ax = skrt.ima
+00052ac0: 6765 2e5f 6178 6573 5b69 5f61 785d 0a20  ge._axes[i_ax]. 
+00052ad0: 2020 2020 2020 2020 2020 2063 656e 7472             centr
+00052ae0: 6f69 6473 5b22 6365 6e74 726f 6964 5f73  oids["centroid_s
+00052af0: 6c69 6365 225d 2e61 7070 656e 6428 6622  lice"].append(f"
+00052b00: 6365 6e74 726f 6964 5f73 6c69 6365 5f7b  centroid_slice_{
+00052b10: 6178 7d22 290a 0a20 2020 2020 2020 2020  ax}")..         
+00052b20: 2020 2069 6620 736c 6963 655f 7374 6174     if slice_stat
+00052b30: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00052b40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00052b50: 656e 7472 6f69 6473 5b22 6365 6e74 726f  entroids["centro
+00052b60: 6964 5f73 6c69 6365 5f73 7461 7473 225d  id_slice_stats"]
+00052b70: 2e61 7070 656e 6428 0a20 2020 2020 2020  .append(.       
+00052b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00052b90: 2066 2263 656e 7472 6f69 645f 7b61 787d   f"centroid_{ax}
+00052ba0: 5f73 6c69 6365 5f73 7461 7473 2229 0a0a  _slice_stats")..
+00052bb0: 2020 2020 2020 2020 666f 7220 7665 6374          for vect
+00052bc0: 6f72 2c20 636f 6d70 6f6e 656e 7473 2069  or, components i
+00052bd0: 6e20 6365 6e74 726f 6964 732e 6974 656d  n centroids.item
+00052be0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+00052bf0: 2069 6478 203d 206d 6574 7269 6373 2e69   idx = metrics.i
+00052c00: 6e64 6578 2876 6563 746f 7229 0a20 2020  ndex(vector).   
+00052c10: 2020 2020 2020 2020 206d 6574 7269 6373           metrics
+00052c20: 5b69 6478 203a 2069 6478 202b 2031 5d20  [idx : idx + 1] 
+00052c30: 3d20 636f 6d70 6f6e 656e 7473 0a0a 2020  = components..  
+00052c40: 2020 2320 5265 6d6f 7665 206d 6574 7269    # Remove metri
+00052c50: 6373 2077 6974 6820 7375 6666 6978 2022  cs with suffix "
+00052c60: 736c 6963 655f 7374 6174 7322 2c0a 2020  slice_stats",.  
+00052c70: 2020 2320 616e 6420 7265 706c 6163 6520    # and replace 
+00052c80: 7769 7468 2073 7065 6369 6669 6320 6d65  with specific me
+00052c90: 7472 6963 7320 7265 6c61 7469 6e67 2074  trics relating t
+00052ca0: 6f20 736c 6963 652d 6279 2d73 6c69 6365  o slice-by-slice
+00052cb0: 2073 7461 7469 7374 6963 732e 0a20 2020   statistics..   
+00052cc0: 2069 6620 736c 6963 655f 7374 6174 7320   if slice_stats 
+00052cd0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00052ce0: 2020 2020 2073 6c69 6365 5f73 7461 7473       slice_stats
+00052cf0: 5f6d 6574 7269 6373 203d 205b 5d0a 2020  _metrics = [].  
+00052d00: 2020 2020 2020 6d65 7472 6963 7332 203d        metrics2 =
+00052d10: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+00052d20: 6d65 7472 6963 2069 6e20 6d65 7472 6963  metric in metric
+00052d30: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00052d40: 6620 2273 6c69 6365 5f73 7461 7473 2220  f "slice_stats" 
+00052d50: 696e 206d 6574 7269 633a 0a20 2020 2020  in metric:.     
+00052d60: 2020 2020 2020 2020 2020 2073 6c69 6365             slice
+00052d70: 5f73 7461 7473 5f6d 6574 7269 6373 2e61  _stats_metrics.a
+00052d80: 7070 656e 6428 6d65 7472 6963 2e73 706c  ppend(metric.spl
+00052d90: 6974 2822 5f73 6c69 6365 5f73 7461 7473  it("_slice_stats
+00052da0: 2229 5b30 5d29 0a20 2020 2020 2020 2020  ")[0]).         
+00052db0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00052dc0: 2020 2020 2020 2020 206d 6574 7269 6373           metrics
+00052dd0: 322e 6170 7065 6e64 286d 6574 7269 6329  2.append(metric)
+00052de0: 0a0a 2020 2020 2020 2020 666f 7220 6279  ..        for by
+00052df0: 5f73 6c69 6365 2c20 7374 6174 7320 696e  _slice, stats in
+00052e00: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00052e10: 2020 2065 7870 616e 645f 736c 6963 655f     expand_slice_
+00052e20: 7374 6174 7328 736c 6963 655f 7374 6174  stats(slice_stat
+00052e30: 732c 2064 6566 6175 6c74 5f62 795f 736c  s, default_by_sl
+00052e40: 6963 6529 2e69 7465 6d73 2829 293a 0a20  ice).items()):. 
+00052e50: 2020 2020 2020 2020 2020 2066 6f72 206d             for m
+00052e60: 6574 7269 6320 696e 2073 6c69 6365 5f73  etric in slice_s
+00052e70: 7461 7473 5f6d 6574 7269 6373 3a0a 2020  tats_metrics:.  
+00052e80: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00052e90: 7220 7374 6174 2069 6e20 7374 6174 733a  r stat in stats:
+00052ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00052eb0: 2020 2020 206d 6574 7269 6373 322e 6170       metrics2.ap
+00052ec0: 7065 6e64 2866 227b 6d65 7472 6963 7d5f  pend(f"{metric}_
+00052ed0: 736c 6963 655f 7b62 795f 736c 6963 657d  slice_{by_slice}
+00052ee0: 5f7b 7374 6174 7d22 290a 2020 2020 2020  _{stat}").      
+00052ef0: 2020 6d65 7472 6963 7320 3d20 6d65 7472    metrics = metr
+00052f00: 6963 7332 0a0a 2020 2020 7265 7475 726e  ics2..    return
+00052f10: 2073 6f72 7465 6428 6d65 7472 6963 7329   sorted(metrics)
+00052f20: 0a0a 6465 6620 6765 745f 636f 6e73 656e  ..def get_consen
+00052f30: 7375 735f 7479 7065 7328 293a 0a20 2020  sus_types():.   
+00052f40: 2022 2222 0a20 2020 2047 6574 206c 6973   """.    Get lis
+00052f50: 7420 6f66 2063 6f6e 7365 6e73 7573 2074  t of consensus t
+00052f60: 7970 6573 2e0a 0a20 2020 2041 6c6c 2063  ypes...    All c
+00052f70: 6f6e 7365 6e73 7573 2074 7970 6573 206c  onsensus types l
+00052f80: 6973 7465 6420 6865 7265 2073 686f 756c  isted here shoul
+00052f90: 6420 6265 2072 6563 6f67 6e69 7365 6420  d be recognised 
+00052fa0: 6279 0a20 2020 2053 7472 7563 7475 7265  by.    Structure
+00052fb0: 5365 742e 6765 745f 636f 6e73 656e 7375  Set.get_consensu
+00052fc0: 7328 292c 2061 6e64 2061 6c6c 2063 6f6e  s(), and all con
+00052fd0: 7365 6e73 7573 2074 7970 6573 2072 6563  sensus types rec
+00052fe0: 6f67 6e69 7365 640a 2020 2020 6279 2053  ognised.    by S
+00052ff0: 7472 7563 7475 7265 5365 742e 6765 745f  tructureSet.get_
+00053000: 636f 6e73 656e 7375 7320 7368 6f75 6c64  consensus should
+00053010: 2062 6520 6c69 7374 6564 2068 6572 652e   be listed here.
+00053020: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+00053030: 7572 6e20 5b0a 2020 2020 2020 2020 2020  urn [.          
+00053040: 2020 226d 616a 6f72 6974 7922 2c0a 2020    "majority",.  
+00053050: 2020 2020 2020 2020 2020 226f 7665 726c            "overl
+00053060: 6170 222c 0a20 2020 2020 2020 2020 2020  ap",.           
+00053070: 2022 7374 6170 6c65 222c 0a20 2020 2020   "staple",.     
+00053080: 2020 2020 2020 2022 7375 6d22 2c0a 2020         "sum",.  
+00053090: 2020 2020 2020 2020 2020 5d0a 0a64 6566            ]..def
+000530a0: 2067 6574 5f62 795f 736c 6963 655f 6d65   get_by_slice_me
+000530b0: 7468 6f64 7328 293a 0a20 2020 2022 2222  thods():.    """
+000530c0: 0a20 2020 2047 6574 206c 6973 7420 6f66  .    Get list of
+000530d0: 206d 6574 686f 6473 2066 6f72 2064 6566   methods for def
+000530e0: 696e 696e 6720 736c 6963 6573 2074 6f20  ining slices to 
+000530f0: 6265 2063 6f6e 7369 6465 7265 640a 2020  be considered.  
+00053100: 2020 666f 7220 736c 6963 652d 6279 2d73    for slice-by-s
+00053110: 6c69 6365 2052 4f49 2063 6f6d 7061 7269  lice ROI compari
+00053120: 736f 6e73 2e0a 2020 2020 2222 220a 2020  sons..    """.  
+00053130: 2020 7265 7475 726e 205b 226c 6566 7422    return ["left"
+00053140: 2c20 2272 6967 6874 222c 2022 756e 696f  , "right", "unio
+00053150: 6e22 2c20 2269 6e74 6572 7365 6374 696f  n", "intersectio
+00053160: 6e22 5d0a 0a64 6566 2067 6574 5f61 6c6c  n"]..def get_all
+00053170: 5f72 6f69 7328 6f62 6a73 3d4e 6f6e 6529  _rois(objs=None)
+00053180: 3a0a 2020 2020 2222 220a 2020 2020 4372  :.    """.    Cr
+00053190: 6561 7465 206c 6973 7420 6f66 2052 4f49  eate list of ROI
+000531a0: 7320 6672 6f6d 2061 7262 6974 7261 7279  s from arbitrary
+000531b0: 2063 6f6d 6269 6e61 7469 6f6e 206f 6620   combination of 
+000531c0: 524f 4973 2061 6e64 2053 7472 7563 7475  ROIs and Structu
+000531d0: 7265 5365 7473 2e0a 0a20 2020 202a 2a50  reSets...    **P
+000531e0: 6172 616d 6574 6572 733a 2a2a 0a0a 2020  arameters:**..  
+000531f0: 2020 6f62 6a73 203a 2052 4f49 2f53 7472    objs : ROI/Str
+00053200: 7563 7475 7265 5365 742f 6c69 7374 2c20  uctureSet/list, 
+00053210: 6465 6661 756c 743d 4e6f 6e65 0a20 2020  default=None.   
+00053220: 2020 2020 204f 626a 6563 7428 7329 2066       Object(s) f
+00053230: 726f 6d20 7768 6963 6820 6120 6c69 7374  rom which a list
+00053240: 206f 6620 524f 4973 2069 7320 746f 2062   of ROIs is to b
+00053250: 6520 6372 6561 7465 642e 2020 5468 650a  e created.  The.
+00053260: 2020 2020 2020 2020 6f62 6a65 6374 2873          object(s
+00053270: 2920 6361 6e20 6265 2061 2073 696e 676c  ) can be a singl
+00053280: 6520 736b 7274 2e73 7472 7563 7475 7265  e skrt.structure
+00053290: 732e 524f 4920 6f62 6a65 6374 2c20 6120  s.ROI object, a 
+000532a0: 7369 6e67 6c65 0a20 2020 2020 2020 2073  single.        s
+000532b0: 6b72 742e 7374 7275 6374 7572 6573 2e53  krt.structures.S
+000532c0: 7472 7563 7475 7265 5365 7420 6f62 6a65  tructureSet obje
+000532d0: 6374 2c20 6f72 2061 206c 6973 7420 636f  ct, or a list co
+000532e0: 6e74 6169 6e69 6e67 2061 6e79 0a20 2020  ntaining any.   
+000532f0: 2020 2020 2063 6f6d 6269 6e61 7469 6f6e       combination
+00053300: 206f 6620 524f 4920 616e 6420 5374 7275   of ROI and Stru
+00053310: 6374 7572 6553 6574 206f 626a 6563 7473  ctureSet objects
+00053320: 2e0a 2020 2020 2222 220a 2020 2020 2320  ..    """.    # 
+00053330: 456e 7375 7265 2074 6861 7420 6f62 6a73  Ensure that objs
+00053340: 2069 7320 6120 6c69 7374 0a20 2020 2069   is a list.    i
+00053350: 6620 6973 7375 6263 6c61 7373 2874 7970  f issubclass(typ
+00053360: 6528 6f62 6a73 292c 2028 524f 492c 2053  e(objs), (ROI, S
+00053370: 7472 7563 7475 7265 5365 7429 293a 0a20  tructureSet)):. 
+00053380: 2020 2020 2020 206f 626a 7320 3d20 5b6f         objs = [o
+00053390: 626a 735d 0a20 2020 2065 6c69 6620 6f62  bjs].    elif ob
+000533a0: 6a73 2069 7320 4e6f 6e65 3a0a 2020 2020  js is None:.    
+000533b0: 2020 2020 6f62 6a73 203d 205b 5d0a 0a20      objs = [].. 
+000533c0: 2020 2023 2043 7265 6174 6520 6120 6c69     # Create a li
+000533d0: 7374 2063 6f6e 7461 696e 696e 6720 616c  st containing al
+000533e0: 6c20 756e 6971 7565 2072 6f69 732e 0a20  l unique rois.. 
+000533f0: 2020 2061 6c6c 5f72 6f69 7320 3d20 5b5d     all_rois = []
+00053400: 0a20 2020 2066 6f72 2069 7465 6d20 696e  .    for item in
+00053410: 206f 626a 733a 0a20 2020 2020 2020 2069   objs:.        i
+00053420: 6620 6973 7375 6263 6c61 7373 2874 7970  f issubclass(typ
+00053430: 6528 6974 656d 292c 2052 4f49 293a 0a20  e(item), ROI):. 
+00053440: 2020 2020 2020 2020 2020 2063 616e 6469             candi
+00053450: 6461 7465 5f72 6f69 7320 3d20 5b69 7465  date_rois = [ite
+00053460: 6d5d 0a20 2020 2020 2020 2065 6c69 6620  m].        elif 
+00053470: 6973 7375 6263 6c61 7373 2874 7970 6528  issubclass(type(
+00053480: 6974 656d 292c 2053 7472 7563 7475 7265  item), Structure
+00053490: 5365 7429 3a0a 2020 2020 2020 2020 2020  Set):.          
+000534a0: 2020 6361 6e64 6964 6174 655f 726f 6973    candidate_rois
+000534b0: 203d 2069 7465 6d2e 6765 745f 726f 6973   = item.get_rois
+000534c0: 2829 0a20 2020 2020 2020 2066 6f72 2072  ().        for r
+000534d0: 6f69 2069 6e20 6361 6e64 6964 6174 655f  oi in candidate_
+000534e0: 726f 6973 3a0a 2020 2020 2020 2020 2020  rois:.          
+000534f0: 2020 6966 206e 6f74 2072 6f69 2069 6e20    if not roi in 
+00053500: 616c 6c5f 726f 6973 3a0a 2020 2020 2020  all_rois:.      
+00053510: 2020 2020 2020 2020 2020 616c 6c5f 726f            all_ro
+00053520: 6973 2e61 7070 656e 6428 726f 6929 0a0a  is.append(roi)..
+00053530: 2020 2020 7265 7475 726e 2061 6c6c 5f72      return all_r
+00053540: 6f69 730a 0a64 6566 2067 6574 5f74 7261  ois..def get_tra
+00053550: 6e73 6c61 7469 6f6e 5f74 6f5f 616c 6967  nslation_to_alig
+00053560: 6e28 726f 6931 2c20 726f 6932 2c20 7a5f  n(roi1, roi2, z_
+00053570: 6672 6163 7469 6f6e 313d 4e6f 6e65 2c20  fraction1=None, 
+00053580: 7a5f 6672 6163 7469 6f6e 323d 4e6f 6e65  z_fraction2=None
+00053590: 293a 0a20 2020 2022 2222 0a20 2020 2044  ):.    """.    D
+000535a0: 6574 6572 6d69 6e65 2074 7261 6e73 6c61  etermine transla
+000535b0: 7469 6f6e 2066 6f72 2061 6c69 676e 696e  tion for alignin
+000535c0: 6720 3c72 6f69 313e 2074 6f20 3c72 6f69  g <roi1> to <roi
+000535d0: 323e 2e0a 0a20 2020 202a 2a50 6172 616d  2>...    **Param
+000535e0: 6574 6572 733a 2a2a 0a0a 2020 2020 726f  eters:**..    ro
+000535f0: 6931 203a 2052 4f49 2f53 7472 7563 7475  i1 : ROI/Structu
+00053600: 7265 5365 742f 6c69 7374 0a20 2020 2020  reSet/list.     
+00053610: 2020 2052 4f49 2074 6861 7420 6973 2074     ROI that is t
+00053620: 6f20 6265 2074 7261 6e73 6c61 7469 6f6e  o be translation
+00053630: 2074 6f20 6163 6869 6576 6520 7468 6520   to achieve the 
+00053640: 616c 6967 6e6d 656e 742e 2020 5468 6973  alignment.  This
+00053650: 0a20 2020 2020 2020 2063 616e 2062 6520  .        can be 
+00053660: 7370 6563 6966 6965 6420 6469 7265 6374  specified direct
+00053670: 6c79 2061 7320 6120 7369 6e67 6c65 2052  ly as a single R
+00053680: 4f49 2e20 2041 6c74 6572 6e61 7469 7665  OI.  Alternative
+00053690: 6c79 2c0a 2020 2020 2020 2020 6974 2063  ly,.        it c
+000536a0: 616e 2062 6520 6120 5374 7275 6374 7572  an be a Structur
+000536b0: 6553 6574 2c20 6f72 2061 206c 6973 7420  eSet, or a list 
+000536c0: 6f72 2052 4f49 2f53 7472 7563 7475 7265  or ROI/Structure
+000536d0: 5365 7420 6f62 6a65 6374 732c 0a20 2020  Set objects,.   
+000536e0: 2020 2020 2069 6e20 7768 6963 6820 6361       in which ca
+000536f0: 7365 2074 6865 2069 6e64 6976 6964 7561  se the individua
+00053700: 6c20 524f 4973 2077 696c 6c20 6265 2063  l ROIs will be c
+00053710: 6f6d 6269 6e65 642e 0a0a 2020 2020 726f  ombined...    ro
+00053720: 6932 203a 2052 4f49 2f53 7472 7563 7475  i2 : ROI/Structu
+00053730: 7265 5365 742f 6c69 7374 0a20 2020 2020  reSet/list.     
+00053740: 2020 2052 4f49 2077 6974 6820 7768 6963     ROI with whic
+00053750: 6820 616c 6967 6e6d 656e 7420 6973 2074  h alignment is t
+00053760: 6f20 6265 2070 6572 666f 726d 6564 2e20  o be performed. 
+00053770: 2054 6869 7320 6361 6e20 6265 0a20 2020   This can be.   
+00053780: 2020 2020 2073 7065 6369 6669 6564 2064       specified d
+00053790: 6972 6563 746c 7920 6173 2061 2073 696e  irectly as a sin
+000537a0: 676c 6520 524f 492e 2020 416c 7465 726e  gle ROI.  Altern
+000537b0: 6174 6976 656c 792c 2069 7420 6361 6e0a  atively, it can.
+000537c0: 2020 2020 2020 2020 6265 2061 2053 7472          be a Str
+000537d0: 7563 7475 7265 5365 742c 206f 7220 6120  uctureSet, or a 
+000537e0: 6c69 7374 206f 7220 524f 492f 5374 7275  list or ROI/Stru
+000537f0: 6374 7572 6553 6574 206f 626a 6563 7473  ctureSet objects
+00053800: 2c0a 2020 2020 2020 2020 696e 2077 6869  ,.        in whi
+00053810: 6368 2063 6173 6520 7468 6520 696e 6469  ch case the indi
+00053820: 7669 6475 616c 2052 4f49 7320 7769 6c6c  vidual ROIs will
+00053830: 2062 6520 636f 6d62 696e 6564 2e0a 0a20   be combined... 
+00053840: 2020 207a 5f66 7261 6374 696f 6e31 203a     z_fraction1 :
+00053850: 2066 6c6f 6174 2c20 6465 6661 756c 743d   float, default=
+00053860: 4e6f 6e65 0a20 2020 2020 2020 2050 6f73  None.        Pos
+00053870: 6974 696f 6e20 616c 6f6e 6720 7a20 6178  ition along z ax
+00053880: 6973 206f 6620 736c 6963 6520 7468 726f  is of slice thro
+00053890: 7567 6820 3c72 6f69 313e 206f 6e20 7768  ugh <roi1> on wh
+000538a0: 6963 680a 2020 2020 2020 2020 746f 2061  ich.        to a
+000538b0: 6c69 676e 2e20 2049 6620 4e6f 6e65 2c20  lign.  If None, 
+000538c0: 616c 6967 6e6d 656e 7420 6973 2074 6f20  alignment is to 
+000538d0: 7468 6520 6365 6e74 726f 6964 206f 6620  the centroid of 
+000538e0: 7468 650a 2020 2020 2020 2020 7768 6f6c  the.        whol
+000538f0: 6520 524f 4920 766f 6c75 6d65 2e20 204f  e ROI volume.  O
+00053900: 7468 6572 7769 7365 2c20 616c 6967 6e6d  therwise, alignm
+00053910: 656e 7420 6973 2074 6f20 7468 650a 2020  ent is to the.  
+00053920: 2020 2020 2020 6365 6e74 726f 6964 206f        centroid o
+00053930: 6620 7468 6520 736c 6963 6520 6174 2074  f the slice at t
+00053940: 6865 2073 7065 6369 6669 6564 2064 6973  he specified dis
+00053950: 7461 6e63 650a 2020 2020 2020 2020 6672  tance.        fr
+00053960: 6f6d 2074 6865 2052 4f49 2773 206d 6f73  om the ROI's mos
+00053970: 742d 696e 6665 7269 6f72 2070 6f69 6e74  t-inferior point
+00053980: 3a20 3020 636f 7272 6573 706f 6e64 7320  : 0 corresponds 
+00053990: 746f 0a20 2020 2020 2020 2074 6865 206d  to.        the m
+000539a0: 6f73 742d 696e 6665 7269 6f72 2070 6f69  ost-inferior poi
+000539b0: 6e74 2028 6c6f 7765 7374 207a 293b 2031  nt (lowest z); 1
+000539c0: 2063 6f72 7265 7370 6f6e 6473 2074 6f20   corresponds to 
+000539d0: 7468 650a 2020 2020 2020 2020 6d6f 7374  the.        most
+000539e0: 2d73 7570 6572 696f 7220 706f 696e 7420  -superior point 
+000539f0: 2868 6967 6865 7374 207a 292e 2020 5661  (highest z).  Va
+00053a00: 6c75 6573 2066 6f72 207a 5f66 7261 6374  lues for z_fract
+00053a10: 696f 6e0a 2020 2020 2020 2020 6f75 7473  ion.        outs
+00053a20: 6964 6520 7468 6520 696e 7465 7276 616c  ide the interval
+00053a30: 205b 302c 2031 5d20 7265 7375 6c74 2069   [0, 1] result i
+00053a40: 6e20 6120 5275 6e74 696d 6545 7272 6f72  n a RuntimeError
+00053a50: 2e0a 0a20 2020 207a 5f66 7261 6374 696f  ...    z_fractio
+00053a60: 6e32 203a 2066 6c6f 6174 2c20 6465 6661  n2 : float, defa
+00053a70: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
+00053a80: 2050 6f73 6974 696f 6e20 616c 6f6e 6720   Position along 
+00053a90: 7a20 6178 6973 206f 6620 736c 6963 6520  z axis of slice 
+00053aa0: 7468 726f 7567 6820 3c72 6f69 323e 206f  through <roi2> o
+00053ab0: 6e20 7768 6963 680a 2020 2020 2020 2020  n which.        
+00053ac0: 746f 2061 6c69 676e 2e20 2049 6620 4e6f  to align.  If No
+00053ad0: 6e65 2c20 616c 6967 6e6d 656e 7420 6973  ne, alignment is
+00053ae0: 2074 6f20 7468 6520 6365 6e74 726f 6964   to the centroid
+00053af0: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
+00053b00: 7768 6f6c 6520 524f 4920 766f 6c75 6d65  whole ROI volume
+00053b10: 2e20 204f 7468 6572 7769 7365 2c20 616c  .  Otherwise, al
+00053b20: 6967 6e6d 656e 7420 6973 2074 6f20 7468  ignment is to th
+00053b30: 650a 2020 2020 2020 2020 6365 6e74 726f  e.        centro
+00053b40: 6964 206f 6620 7468 6520 736c 6963 6520  id of the slice 
+00053b50: 6174 2074 6865 2073 7065 6369 6669 6564  at the specified
+00053b60: 2064 6973 7461 6e63 650a 2020 2020 2020   distance.      
+00053b70: 2020 6672 6f6d 2074 6865 2052 4f49 2773    from the ROI's
+00053b80: 206d 6f73 742d 696e 6665 7269 6f72 2070   most-inferior p
+00053b90: 6f69 6e74 3a20 3020 636f 7272 6573 706f  oint: 0 correspo
+00053ba0: 6e64 7320 746f 0a20 2020 2020 2020 2074  nds to.        t
+00053bb0: 6865 206d 6f73 742d 696e 6665 7269 6f72  he most-inferior
+00053bc0: 2070 6f69 6e74 2028 6c6f 7765 7374 207a   point (lowest z
+00053bd0: 293b 2031 2063 6f72 7265 7370 6f6e 6473  ); 1 corresponds
+00053be0: 2074 6f20 7468 650a 2020 2020 2020 2020   to the.        
+00053bf0: 6d6f 7374 2d73 7570 6572 696f 7220 706f  most-superior po
+00053c00: 696e 7420 2868 6967 6865 7374 207a 292e  int (highest z).
+00053c10: 2020 5661 6c75 6573 2066 6f72 207a 5f66    Values for z_f
+00053c20: 7261 6374 696f 6e0a 2020 2020 2020 2020  raction.        
+00053c30: 6f75 7473 6964 6520 7468 6520 696e 7465  outside the inte
+00053c40: 7276 616c 205b 302c 2031 5d20 7265 7375  rval [0, 1] resu
+00053c50: 6c74 2069 6e20 6120 5275 6e74 696d 6545  lt in a RuntimeE
+00053c60: 7272 6f72 2e0a 2020 2020 2020 2020 2222  rror..        ""
+00053c70: 220a 2020 2020 2320 4372 6561 7465 206c  ".    # Create l
+00053c80: 6973 7420 6f66 2074 776f 2073 696e 676c  ist of two singl
+00053c90: 6520 524f 4973 2e0a 2020 2020 726f 6973  e ROIs..    rois
+00053ca0: 203d 205b 5d0a 2020 2020 666f 7220 726f   = [].    for ro
+00053cb0: 6920 696e 205b 726f 6931 2c20 726f 6932  i in [roi1, roi2
+00053cc0: 5d3a 0a20 2020 2020 2020 2069 6620 6973  ]:.        if is
+00053cd0: 696e 7374 616e 6365 2872 6f69 2c20 524f  instance(roi, RO
+00053ce0: 4929 3a0a 2020 2020 2020 2020 2020 2020  I):.            
+00053cf0: 2320 5374 6f72 6520 7369 6e67 6c65 2052  # Store single R
+00053d00: 4f49 2064 6972 6563 746c 792e 0a20 2020  OI directly..   
+00053d10: 2020 2020 2020 2020 2072 6f69 732e 6170           rois.ap
+00053d20: 7065 6e64 2872 6f69 290a 2020 2020 2020  pend(roi).      
+00053d30: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00053d40: 6528 726f 692c 2053 7472 7563 7475 7265  e(roi, Structure
+00053d50: 5365 7429 3a0a 2020 2020 2020 2020 2020  Set):.          
+00053d60: 2020 2320 436f 6d62 696e 6520 524f 4973    # Combine ROIs
+00053d70: 206f 6620 5374 7275 6374 7572 6553 6574   of StructureSet
+00053d80: 2e0a 2020 2020 2020 2020 2020 2020 726f  ..            ro
+00053d90: 6973 2e61 7070 656e 6428 726f 692e 636f  is.append(roi.co
+00053da0: 6d62 696e 655f 726f 6973 2829 290a 2020  mbine_rois()).  
+00053db0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00053dc0: 2020 2020 2020 2020 2320 436f 6d62 696e          # Combin
+00053dd0: 6520 524f 4973 2066 726f 6d20 6c69 7374  e ROIs from list
+00053de0: 2e0a 2020 2020 2020 2020 2020 2020 726f  ..            ro
+00053df0: 6973 2e61 7070 656e 6428 5374 7275 6374  is.append(Struct
+00053e00: 7572 6553 6574 2867 6574 5f61 6c6c 5f72  ureSet(get_all_r
+00053e10: 6f69 7328 726f 6929 292e 636f 6d62 696e  ois(roi)).combin
+00053e20: 655f 726f 6973 2829 290a 0a20 2020 2023  e_rois())..    #
+00053e30: 2043 616c 6375 6c61 7465 2061 6c69 676e   Calculate align
+00053e40: 6d65 6e74 2070 6f69 6e74 732e 0a20 2020  ment points..   
+00053e50: 2063 656e 7472 6f69 6473 203d 205b 5d0a   centroids = [].
+00053e60: 2020 2020 666f 7220 726f 692c 207a 5f66      for roi, z_f
+00053e70: 7261 6374 696f 6e20 696e 207a 6970 2872  raction in zip(r
+00053e80: 6f69 732c 205b 7a5f 6672 6163 7469 6f6e  ois, [z_fraction
+00053e90: 312c 207a 5f66 7261 6374 696f 6e32 5d29  1, z_fraction2])
+00053ea0: 3a0a 2020 2020 2020 2020 2320 4361 6c63  :.        # Calc
+00053eb0: 756c 6174 6520 6365 6e74 726f 6964 2066  ulate centroid f
+00053ec0: 6f72 2074 6865 2077 686f 6c65 2052 4f49  or the whole ROI
+00053ed0: 2076 6f6c 756d 652e 0a20 2020 2020 2020   volume..       
+00053ee0: 2069 6620 7a5f 6672 6163 7469 6f6e 2069   if z_fraction i
+00053ef0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00053f00: 2020 2020 6365 6e74 726f 6964 732e 6170      centroids.ap
+00053f10: 7065 6e64 2872 6f69 2e67 6574 5f63 656e  pend(roi.get_cen
+00053f20: 7472 6f69 6428 2929 0a20 2020 2020 2020  troid()).       
+00053f30: 2023 2043 616c 6375 6c61 7465 2063 656e   # Calculate cen
+00053f40: 7472 6f69 6420 666f 7220 736c 6963 6520  troid for slice 
+00053f50: 6174 2073 7065 6369 6669 6564 2070 6f73  at specified pos
+00053f60: 6974 696f 6e2e 0a20 2020 2020 2020 2065  ition..        e
+00053f70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00053f80: 2063 656e 7472 6f69 6473 2e61 7070 656e   centroids.appen
+00053f90: 6428 726f 692e 6765 745f 726f 695f 736c  d(roi.get_roi_sl
+00053fa0: 6963 6528 7a5f 6672 6163 7469 6f6e 292e  ice(z_fraction).
+00053fb0: 6765 745f 6365 6e74 726f 6964 2829 290a  get_centroid()).
+00053fc0: 0a20 2020 2072 6574 7572 6e20 7475 706c  .    return tupl
+00053fd0: 6528 6365 6e74 726f 6964 735b 315d 202d  e(centroids[1] -
+00053fe0: 2063 656e 7472 6f69 6473 5b30 5d29 0a0a   centroids[0])..
+00053ff0: 6465 6620 6765 745f 736c 6963 655f 706f  def get_slice_po
+00054000: 7369 7469 6f6e 7328 726f 6931 2c20 726f  sitions(roi1, ro
+00054010: 6932 3d4e 6f6e 652c 2076 6965 773d 2278  i2=None, view="x
+00054020: 2d79 222c 2070 6f73 6974 696f 6e5f 6173  -y", position_as
+00054030: 5f69 6478 3d46 616c 7365 2c0a 2020 2020  _idx=False,.    
+00054040: 2020 2020 6d65 7468 6f64 3d4e 6f6e 6529      method=None)
+00054050: 3a0a 2020 2020 2222 220a 2020 2020 4765  :.    """.    Ge
+00054060: 7420 6f72 6465 7265 6420 6c69 7374 206f  t ordered list o
+00054070: 6620 736c 6963 6520 706f 7369 7469 6f6e  f slice position
+00054080: 7320 666f 7220 6569 7468 6572 206f 7220  s for either or 
+00054090: 626f 7468 206f 6620 6120 7061 6972 206f  both of a pair o
+000540a0: 6620 524f 4973 2e0a 0a20 2020 202a 2a50  f ROIs...    **P
+000540b0: 6172 616d 6574 6572 733a 2a2a 0a0a 2020  arameters:**..  
+000540c0: 2020 726f 6931 203a 2073 6b72 742e 7374    roi1 : skrt.st
+000540d0: 7275 6374 7572 6573 2e52 4f49 0a20 2020  ructures.ROI.   
+000540e0: 2020 2020 2052 4f49 2c20 6f72 206f 6e65       ROI, or one
+000540f0: 206f 6620 6120 7061 6972 206f 6620 524f   of a pair of RO
+00054100: 4973 2c20 666f 7220 7768 6963 6820 736c  Is, for which sl
+00054110: 6963 6520 696e 666f 726d 6174 696f 6e20  ice information 
+00054120: 6973 2074 6f0a 2020 2020 2020 2020 6265  is to.        be
+00054130: 206f 6274 6169 6e65 642e 0a0a 2020 2020   obtained...    
+00054140: 726f 6932 203a 2073 6b72 742e 7374 7275  roi2 : skrt.stru
+00054150: 6374 7572 6573 2e52 4f49 2c20 6465 6661  ctures.ROI, defa
+00054160: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
+00054170: 2049 6620 6e6f 7420 4e6f 6e65 2c20 7365   If not None, se
+00054180: 636f 6e64 2069 6e20 6120 7061 6972 206f  cond in a pair o
+00054190: 6620 524f 4973 2066 6f72 2077 6869 6368  f ROIs for which
+000541a0: 2073 6c69 6365 2069 6e66 6f72 6d61 7469   slice informati
+000541b0: 6f6e 0a20 2020 2020 2020 2069 7320 746f  on.        is to
+000541c0: 2062 6520 6f62 7461 696e 6564 2e0a 0a20   be obtained... 
+000541d0: 2020 2076 6965 7720 3a20 7374 722c 2064     view : str, d
+000541e0: 6566 6175 6c74 3d22 782d 7922 0a20 2020  efault="x-y".   
+000541f0: 2020 2020 2056 6965 7720 696e 2077 6869       View in whi
+00054200: 6368 2074 6f20 6f62 7461 696e 2073 6c69  ch to obtain sli
+00054210: 6365 732e 0a0a 2020 2020 706f 7369 7469  ces...    positi
+00054220: 6f6e 5f61 735f 6964 7820 3a20 626f 6f6c  on_as_idx : bool
+00054230: 2c20 6465 6661 756c 743d 4661 6c73 650a  , default=False.
+00054240: 2020 2020 2020 2020 4966 2054 7275 652c          If True,
+00054250: 2072 6574 7572 6e20 706f 7369 7469 6f6e   return position
+00054260: 7320 6173 2073 6c69 6365 2069 6e64 6963  s as slice indic
+00054270: 6573 3b20 6966 2046 616c 7365 2c0a 2020  es; if False,.  
+00054280: 2020 2020 2020 7265 7475 726e 2070 6f73        return pos
+00054290: 6974 696f 6e73 2061 7320 736c 6963 6520  itions as slice 
+000542a0: 7a2d 636f 6f72 6469 6e61 7465 7320 286d  z-coordinates (m
+000542b0: 6d29 2e0a 0a20 2020 206d 6574 686f 643a  m)...    method:
+000542c0: 2073 7472 2c20 6465 6661 756c 743d 4e6f   str, default=No
+000542d0: 6e65 0a20 2020 2020 2020 2053 7472 696e  ne.        Strin
+000542e0: 6720 7370 6563 6966 7969 6e67 2073 6c69  g specifying sli
+000542f0: 6365 7320 666f 7220 7768 6963 6820 706f  ces for which po
+00054300: 7369 7469 6f6e 7320 6172 6520 746f 2062  sitions are to b
+00054310: 6520 6f62 7461 696e 6564 2c0a 2020 2020  e obtained,.    
+00054320: 2020 2020 666f 7220 524f 4973 2072 6f69      for ROIs roi
+00054330: 312c 2072 6f69 323a 0a0a 2020 2020 2020  1, roi2:..      
+00054340: 2020 2d20 226c 6566 7422 2028 6f72 2072    - "left" (or r
+00054350: 6f69 3220 6973 204e 6f6e 6529 3a20 7265  oi2 is None): re
+00054360: 7475 726e 2070 6f73 6974 696f 6e73 206f  turn positions o
+00054370: 6620 736c 6963 6573 2063 6f6e 7461 696e  f slices contain
+00054380: 696e 6720 726f 6931 3b0a 2020 2020 2020  ing roi1;.      
+00054390: 2020 2d20 2272 6967 6874 223a 2072 6574    - "right": ret
+000543a0: 7572 6e20 706f 7369 7469 6f6e 7320 6f66  urn positions of
+000543b0: 2073 6c69 6365 7320 636f 6e74 6169 6e69   slices containi
+000543c0: 6e67 2072 6f69 323b 0a20 2020 2020 2020  ng roi2;.       
+000543d0: 202d 2022 756e 696f 6e22 3a20 7265 7475   - "union": retu
+000543e0: 726e 2070 6f73 6974 696f 6e73 206f 6620  rn positions of 
+000543f0: 736c 6963 6573 2063 6f6e 7461 696e 696e  slices containin
+00054400: 6720 6569 7468 6572 2072 6f69 3120 6f72  g either roi1 or
+00054410: 2072 6f69 323b 0a20 2020 2020 2020 202d   roi2;.        -
+00054420: 2022 696e 7465 7273 6563 7469 6f6e 223a   "intersection":
+00054430: 2072 6574 7572 6e20 706f 7369 7469 6f6e   return position
+00054440: 7320 6f66 2073 6c69 6365 7320 636f 6e74  s of slices cont
+00054450: 6169 6e69 6e67 2062 6f74 680a 2020 2020  aining both.    
+00054460: 2020 2020 2020 726f 6931 2061 6e64 2072        roi1 and r
+00054470: 6f69 322e 0a0a 2020 2020 2020 2020 4966  oi2...        If
+00054480: 204e 6f6e 652c 2076 616c 7565 206f 6620   None, value of 
+00054490: 736b 7274 2e63 6f72 652e 4465 6661 756c  skrt.core.Defaul
+000544a0: 7473 2829 2e62 795f 736c 6963 6520 6973  ts().by_slice is
+000544b0: 2075 7365 642e 0a20 2020 2022 2222 0a20   used..    """. 
+000544c0: 2020 206d 6574 686f 6420 3d20 6d65 7468     method = meth
+000544d0: 6f64 206f 7220 736b 7274 2e63 6f72 652e  od or skrt.core.
+000544e0: 4465 6661 756c 7473 2829 2e62 795f 736c  Defaults().by_sl
+000544f0: 6963 650a 2020 2020 6966 206d 6574 686f  ice.    if metho
+00054500: 6420 6e6f 7420 696e 2067 6574 5f62 795f  d not in get_by_
+00054510: 736c 6963 655f 6d65 7468 6f64 7328 293a  slice_methods():
+00054520: 0a20 2020 2020 2020 2072 6169 7365 2052  .        raise R
+00054530: 756e 7469 6d65 4572 726f 7228 6622 4d65  untimeError(f"Me
+00054540: 7468 6f64 206d 7573 7420 6265 206f 6e65  thod must be one
+00054550: 206f 6620 7b67 6574 5f62 795f 736c 6963   of {get_by_slic
+00054560: 655f 6d65 7468 6f64 7328 297d 220a 2020  e_methods()}".  
+00054570: 2020 2020 2020 2220 2d20 6e6f 7420 277b        " - not '{
+00054580: 6d65 7468 6f64 7d27 2229 0a0a 2020 2020  method}'")..    
+00054590: 696e 6469 6365 7320 3d20 4e6f 6e65 0a0a  indices = None..
+000545a0: 2020 2020 696e 6469 6365 7331 203d 2072      indices1 = r
+000545b0: 6f69 312e 6765 745f 696e 6469 6365 7328  oi1.get_indices(
+000545c0: 7669 6577 3d76 6965 772c 206d 6574 686f  view=view, metho
+000545d0: 643d 226d 6173 6b22 290a 2020 2020 6966  d="mask").    if
+000545e0: 206e 6f74 2069 7373 7562 636c 6173 7328   not issubclass(
+000545f0: 7479 7065 2872 6f69 3229 2c20 524f 4929  type(roi2), ROI)
+00054600: 206f 7220 226c 6566 7422 203d 3d20 6d65   or "left" == me
+00054610: 7468 6f64 3a0a 2020 2020 2020 2020 696e  thod:.        in
+00054620: 6469 6365 7320 3d20 696e 6469 6365 7331  dices = indices1
+00054630: 0a0a 2020 2020 6966 2069 6e64 6963 6573  ..    if indices
+00054640: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00054650: 2020 696e 6469 6365 7332 203d 2072 6f69    indices2 = roi
+00054660: 322e 6765 745f 696e 6469 6365 7328 7669  2.get_indices(vi
+00054670: 6577 3d76 6965 772c 206d 6574 686f 643d  ew=view, method=
+00054680: 226d 6173 6b22 290a 2020 2020 2020 2020  "mask").        
+00054690: 6966 2022 7269 6768 7422 203d 3d20 6d65  if "right" == me
+000546a0: 7468 6f64 3a0a 2020 2020 2020 2020 2020  thod:.          
+000546b0: 2020 696e 6469 6365 7320 3d20 696e 6469    indices = indi
+000546c0: 6365 7332 0a20 2020 2020 2020 200a 2020  ces2.        .  
+000546d0: 2020 6966 2069 6e64 6963 6573 2069 7320    if indices is 
+000546e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
+000546f0: 2022 756e 696f 6e22 203d 3d20 6d65 7468   "union" == meth
+00054700: 6f64 3a0a 2020 2020 2020 2020 2020 2020  od:.            
+00054710: 696e 6469 6365 7320 3d20 6c69 7374 2873  indices = list(s
+00054720: 6574 2869 6e64 6963 6573 3129 2e75 6e69  et(indices1).uni
+00054730: 6f6e 2873 6574 2869 6e64 6963 6573 3229  on(set(indices2)
+00054740: 2929 0a0a 2020 2020 6966 2069 6e64 6963  ))..    if indic
+00054750: 6573 2069 7320 4e6f 6e65 3a0a 2020 2020  es is None:.    
+00054760: 2020 2020 6966 2022 696e 7465 7273 6563      if "intersec
+00054770: 7469 6f6e 2220 3d3d 206d 6574 686f 643a  tion" == method:
+00054780: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
+00054790: 6963 6573 203d 206c 6973 7428 7365 7428  ices = list(set(
+000547a0: 696e 6469 6365 7331 292e 696e 7465 7273  indices1).inters
+000547b0: 6563 7469 6f6e 2873 6574 2869 6e64 6963  ection(set(indic
+000547c0: 6573 3229 2929 0a0a 2020 2020 6966 2069  es2)))..    if i
+000547d0: 6e64 6963 6573 2069 7320 6e6f 7420 4e6f  ndices is not No
+000547e0: 6e65 3a0a 2020 2020 2020 2020 6966 2070  ne:.        if p
+000547f0: 6f73 6974 696f 6e5f 6173 5f69 6478 3a0a  osition_as_idx:.
+00054800: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00054810: 726e 2073 6f72 7465 6428 696e 6469 6365  rn sorted(indice
+00054820: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
+00054830: 0a20 2020 2020 2020 2020 2020 2061 7820  .            ax 
+00054840: 3d20 736b 7274 2e69 6d61 6765 2e5f 736c  = skrt.image._sl
+00054850: 6963 655f 6178 6573 5b76 6965 775d 0a20  ice_axes[view]. 
+00054860: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00054870: 6e20 736f 7274 6564 285b 726f 6931 2e69  n sorted([roi1.i
+00054880: 6478 5f74 6f5f 706f 7328 6964 782c 2061  dx_to_pos(idx, a
+00054890: 7829 2066 6f72 2069 6478 2069 6e20 696e  x) for idx in in
+000548a0: 6469 6365 735d 290a 0a64 6566 2065 7870  dices])..def exp
+000548b0: 616e 645f 736c 6963 655f 7374 6174 7328  and_slice_stats(
+000548c0: 736c 6963 655f 7374 6174 733d 4e6f 6e65  slice_stats=None
+000548d0: 2c20 6465 6661 756c 745f 6279 5f73 6c69  , default_by_sli
+000548e0: 6365 3d4e 6f6e 6529 3a0a 2020 2020 2222  ce=None):.    ""
+000548f0: 220a 2020 2020 4578 7061 6e64 2073 7065  ".    Expand spe
+00054900: 6369 6669 6361 7469 6f6e 206f 6620 7374  cification of st
+00054910: 6174 6973 7469 6373 2074 6f20 6361 6c63  atistics to calc
+00054920: 756c 6174 6520 666f 7220 524f 4920 636f  ulate for ROI co
+00054930: 6d70 6172 6973 6f6e 0a20 2020 206d 6574  mparison.    met
+00054940: 7269 6373 2065 7661 6c75 6174 6564 2073  rics evaluated s
+00054950: 6c69 6365 2062 7920 736c 6963 652e 0a0a  lice by slice...
+00054960: 2020 2020 4120 6469 6374 696f 6e61 7279      A dictionary
+00054970: 2069 7320 7265 7475 726e 6564 2c20 7768   is returned, wh
+00054980: 6572 6520 6b65 7973 2067 6976 6520 7468  ere keys give th
+00054990: 6520 736c 6963 6573 2074 6f20 6265 2063  e slices to be c
+000549a0: 6f6e 7369 6465 7265 640a 2020 2020 666f  onsidered.    fo
+000549b0: 7220 6361 6c63 756c 6174 696e 6720 7374  r calculating st
+000549c0: 6174 6973 7469 6373 2c20 616e 6420 7661  atistics, and va
+000549d0: 6c75 6573 2061 7265 206c 6973 7473 206f  lues are lists o
+000549e0: 6620 6d65 7472 6963 732e 0a0a 2020 2020  f metrics...    
+000549f0: 2a2a 5061 7261 6d65 7465 7273 3a2a 2a0a  **Parameters:**.
+00054a00: 0a20 2020 2073 6c69 6365 5f73 7461 7473  .    slice_stats
+00054a10: 203a 2073 7472 2f6c 6973 742f 6469 6374   : str/list/dict
+00054a20: 2c20 6465 6661 756c 743d 4e6f 6e65 0a20  , default=None. 
+00054a30: 2020 2020 2020 2053 7065 6369 6669 6361         Specifica
+00054a40: 7469 6f6e 206f 6620 7374 6174 6973 7469  tion of statisti
+00054a50: 6373 2074 6f20 6265 2063 616c 6375 6c61  cs to be calcula
+00054a60: 7465 6420 7265 6c61 7469 7665 0a20 2020  ted relative.   
+00054a70: 2020 2020 2074 6f20 736c 6963 652d 6279       to slice-by
+00054a80: 2d73 6c69 6365 206d 6574 7269 6320 7661  -slice metric va
+00054a90: 6c75 6573 2e0a 0a20 2020 2020 2020 2041  lues...        A
+00054aa0: 2073 7461 7469 7374 6963 2069 7320 7370   statistic is sp
+00054ab0: 6563 6966 6965 6420 6279 2074 6865 206e  ecified by the n
+00054ac0: 616d 6520 6f66 2074 6865 2066 756e 6374  ame of the funct
+00054ad0: 696f 6e20 666f 720a 2020 2020 2020 2020  ion for.        
+00054ae0: 6974 7320 6361 6c63 756c 6174 696f 6e20  its calculation 
+00054af0: 696e 2074 6865 2050 7974 686f 6e20 7374  in the Python st
+00054b00: 6174 6973 7469 6373 206d 6f64 756c 653a  atistics module:
+00054b10: 0a0a 2020 2020 2020 2020 6874 7470 733a  ..        https:
+00054b20: 2f2f 646f 6373 2e70 7974 686f 6e2e 6f72  //docs.python.or
+00054b30: 672f 332f 6c69 6272 6172 792f 7374 6174  g/3/library/stat
+00054b40: 6973 7469 6373 2e68 746d 6c0a 0a20 2020  istics.html..   
+00054b50: 2020 2020 2046 6f72 2069 7473 2075 7365       For its use
+00054b60: 2068 6572 652c 2074 6865 2072 656c 6576   here, the relev
+00054b70: 616e 7420 6675 6e63 7469 6f6e 206d 7573  ant function mus
+00054b80: 7420 7265 7175 6972 650a 2020 2020 2020  t require.      
+00054b90: 2020 6120 7369 6e67 6c65 2d76 6172 6961    a single-varia
+00054ba0: 626c 6520 696e 7075 742c 206d 7573 7420  ble input, must 
+00054bb0: 6e6f 7420 7265 7175 6972 6520 616e 7920  not require any 
+00054bc0: 6b65 7977 6f72 640a 2020 2020 2020 2020  keyword.        
+00054bd0: 6172 6775 6d65 6e74 732c 2061 6e64 206d  arguments, and m
+00054be0: 7573 7420 7265 7475 726e 2061 2073 696e  ust return a sin
+00054bf0: 676c 6520 6e75 6d62 6572 2e0a 0a20 2020  gle number...   
+00054c00: 2020 2020 2041 7661 696c 6162 6c65 206f       Available o
+00054c10: 7074 696f 6e73 2069 6e63 6c75 6465 3a20  ptions include: 
+00054c20: 226d 6561 6e22 2c20 226d 6564 6961 6e22  "mean", "median"
+00054c30: 2c20 226d 6f64 6522 2c0a 2020 2020 2020  , "mode",.      
+00054c40: 2020 2273 7464 6576 222e 0a0a 2020 2020    "stdev"...    
+00054c50: 2020 2053 7461 7469 7374 6963 7320 746f     Statistics to
+00054c60: 2062 6520 6361 6c63 756c 6174 6564 2063   be calculated c
+00054c70: 616e 2062 6520 7370 6563 6966 6965 6420  an be specified 
+00054c80: 7573 696e 6720 616e 7920 6f66 0a20 2020  using any of.   
+00054c90: 2020 2020 7468 6520 666f 6c6c 6f77 696e      the followin
+00054ca0: 673a 0a0a 2020 2020 2020 202d 2053 7472  g:..       - Str
+00054cb0: 696e 6720 7370 6563 6966 7969 6e67 2073  ing specifying s
+00054cc0: 696e 676c 6520 7374 6174 6973 7469 6320  ingle statistic 
+00054cd0: 746f 2062 6520 6361 6c63 756c 6174 6564  to be calculated
+00054ce0: 2c0a 2020 2020 2020 2020 2077 6974 6820  ,.         with 
+00054cf0: 736c 6963 6573 2063 6f6e 7369 6465 7265  slices considere
+00054d00: 6420 6173 2067 6976 656e 2062 7920 3c64  d as given by <d
+00054d10: 6566 6175 6c74 5f62 795f 736c 6963 653e  efault_by_slice>
+00054d20: 2c0a 2020 2020 2020 2020 2066 6f72 2065  ,.         for e
+00054d30: 7861 6d70 6c65 3a20 226d 6561 6e22 3b0a  xample: "mean";.
+00054d40: 2020 2020 2020 202d 204c 6973 7420 7370         - List sp
+00054d50: 6563 6966 7969 6e67 206d 756c 7469 706c  ecifying multipl
+00054d60: 6520 7374 6174 6973 7469 6373 2074 6f20  e statistics to 
+00054d70: 6265 2063 616c 6375 6c61 7465 642c 0a20  be calculated,. 
+00054d80: 2020 2020 2020 2020 7769 7468 2073 6c69          with sli
+00054d90: 6365 7320 636f 6e73 6964 6572 6564 2061  ces considered a
+00054da0: 7320 6769 7665 6e20 6279 203c 6465 6661  s given by <defa
+00054db0: 756c 745f 6279 5f73 6c69 6365 3e2c 0a20  ult_by_slice>,. 
+00054dc0: 2020 2020 2020 2020 666f 7220 6578 616d          for exam
+00054dd0: 706c 653a 205b 226d 6561 6e22 2c20 2273  ple: ["mean", "s
+00054de0: 7464 6576 225d 3b0a 2020 2020 2020 202d  tdev"];.       -
+00054df0: 2044 6963 7469 6f6e 6172 7920 7768 6572   Dictionary wher
+00054e00: 6520 6b65 7973 2073 7065 6369 6679 2073  e keys specify s
+00054e10: 6c69 6365 7320 746f 2062 6520 636f 6e73  lices to be cons
+00054e20: 6964 6572 6564 2c0a 2020 2020 2020 2020  idered,.        
+00054e30: 2061 6e64 2076 616c 7565 7320 7370 6563   and values spec
+00054e40: 6966 7920 7374 6174 6973 7469 6373 2028  ify statistics (
+00054e50: 7374 7269 6e67 206f 7220 6c69 7374 292c  string or list),
+00054e60: 2066 6f72 0a20 2020 2020 2020 2020 6578   for.         ex
+00054e70: 616d 706c 653a 207b 2275 6e69 6f6e 223a  ample: {"union":
+00054e80: 205b 226d 6561 6e22 2c20 2273 7464 6576   ["mean", "stdev
+00054e90: 225d 7d2e 2020 5661 6c69 6420 736c 6963  "]}.  Valid slic
+00054ea0: 650a 2020 2020 2020 2020 2073 7065 6369  e.         speci
+00054eb0: 6669 6361 7469 6f6e 7320 6172 6520 6173  fications are as
+00054ec0: 206c 6973 7465 6420 666f 7220 3c64 6566   listed for <def
+00054ed0: 6175 6c74 5f62 795f 736c 6963 653e 2e0a  ault_by_slice>..
+00054ee0: 0a20 2020 2064 6566 6175 6c74 5f62 795f  .    default_by_
+00054ef0: 736c 6963 653a 2073 7472 2c20 6465 6661  slice: str, defa
+00054f00: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
+00054f10: 2044 6566 6175 6c74 2073 7065 6369 6669   Default specifi
+00054f20: 6361 7469 6f6e 206f 6620 736c 6963 6573  cation of slices
+00054f30: 2074 6f20 6265 2063 6f6e 7369 6465 7265   to be considere
+00054f40: 6420 7768 656e 0a20 2020 2020 2020 2063  d when.        c
+00054f50: 616c 6375 6c61 7469 6e67 2073 6c69 6365  alculating slice
+00054f60: 2d62 792d 736c 6963 6520 7374 6174 6973  -by-slice statis
+00054f70: 7469 6373 2066 6f72 2061 206d 6574 7269  tics for a metri
+00054f80: 6320 636f 6d70 6172 696e 670a 2020 2020  c comparing.    
+00054f90: 2020 2020 7477 6f20 524f 4973 2c20 726f      two ROIs, ro
+00054fa0: 6931 2061 6e64 2072 6f69 322e 2020 5468  i1 and roi2.  Th
+00054fb0: 6520 7661 6c69 6420 7370 6563 6966 6963  e valid specific
+00054fc0: 6174 696f 6e73 2061 7265 3a0a 0a20 2020  ations are:..   
+00054fd0: 2020 2020 202d 2022 6c65 6674 223a 2063       - "left": c
+00054fe0: 6f6e 7369 6465 7220 6f6e 6c79 2073 6c69  onsider only sli
+00054ff0: 6365 7320 636f 6e74 6169 6e69 6e67 2072  ces containing r
+00055000: 6f69 313b 0a20 2020 2020 2020 202d 2022  oi1;.        - "
+00055010: 7269 6768 7422 3a20 636f 6e73 6964 6572  right": consider
+00055020: 206f 6e6c 7920 736c 6963 6573 2063 6f6e   only slices con
+00055030: 7461 696e 696e 6720 726f 6932 3b0a 2020  taining roi2;.  
+00055040: 2020 2020 2020 2d20 2275 6e69 6f6e 223a        - "union":
+00055050: 2063 6f6e 7369 6465 7220 736c 6963 6573   consider slices
+00055060: 2063 6f6e 7461 696e 696e 6720 6569 7468   containing eith
+00055070: 6572 206f 6620 726f 6931 2061 6e64 2072  er of roi1 and r
+00055080: 6f69 323b 0a20 2020 2020 2020 202d 2022  oi2;.        - "
+00055090: 696e 7465 7273 6563 7469 6f6e 223a 2063  intersection": c
+000550a0: 6f6e 7369 6465 7220 736c 6963 6573 2063  onsider slices c
+000550b0: 6f6e 7461 696e 696e 6720 626f 7468 2072  ontaining both r
+000550c0: 6f69 3120 616e 6420 726f 6932 2e0a 0a20  oi1 and roi2... 
+000550d0: 2020 2020 2020 2049 6620 4e6f 6e65 2c20         If None, 
+000550e0: 7573 6520 736b 7274 2e63 6f72 652e 4465  use skrt.core.De
+000550f0: 6661 756c 7473 2829 2e62 795f 736c 6963  faults().by_slic
+00055100: 650a 2020 2020 2222 220a 2020 2020 6966  e.    """.    if
+00055110: 206e 6f74 2073 6c69 6365 5f73 7461 7473   not slice_stats
+00055120: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00055130: 207b 7d0a 0a20 2020 2023 2053 6574 2064   {}..    # Set d
+00055140: 6566 6175 6c74 206d 6574 686f 6420 666f  efault method fo
+00055150: 7220 736c 6963 6520 7365 6c65 6374 696f  r slice selectio
+00055160: 6e2e 0a20 2020 2064 6566 6175 6c74 5f62  n..    default_b
+00055170: 795f 736c 6963 6520 3d20 6465 6661 756c  y_slice = defaul
+00055180: 745f 6279 5f73 6c69 6365 206f 7220 736b  t_by_slice or sk
+00055190: 7274 2e63 6f72 652e 4465 6661 756c 7473  rt.core.Defaults
+000551a0: 2829 2e62 795f 736c 6963 650a 0a20 2020  ().by_slice..   
+000551b0: 2023 2045 6e73 7572 6520 7468 6174 2073   # Ensure that s
+000551c0: 6c69 6365 5f73 7461 7473 2069 7320 6120  lice_stats is a 
+000551d0: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
+000551e0: 6966 2069 7369 6e73 7461 6e63 6528 736c  if isinstance(sl
+000551f0: 6963 655f 7374 6174 732c 2073 7472 293a  ice_stats, str):
+00055200: 0a20 2020 2020 2020 2073 6c69 6365 5f73  .        slice_s
+00055210: 7461 7473 203d 207b 6465 6661 756c 745f  tats = {default_
+00055220: 6279 5f73 6c69 6365 3a20 5b73 6c69 6365  by_slice: [slice
+00055230: 5f73 7461 7473 5d7d 0a0a 2020 2020 656c  _stats]}..    el
+00055240: 6966 2073 6b72 742e 636f 7265 2e69 735f  if skrt.core.is_
+00055250: 6c69 7374 2873 6c69 6365 5f73 7461 7473  list(slice_stats
+00055260: 293a 0a20 2020 2020 2020 2073 6c69 6365  ):.        slice
+00055270: 5f73 7461 7473 203d 207b 6465 6661 756c  _stats = {defaul
+00055280: 745f 6279 5f73 6c69 6365 3a20 736c 6963  t_by_slice: slic
+00055290: 655f 7374 6174 737d 0a0a 2020 2020 656c  e_stats}..    el
+000552a0: 6966 2069 7369 6e73 7461 6e63 6528 736c  if isinstance(sl
+000552b0: 6963 655f 7374 6174 732c 2064 6963 7429  ice_stats, dict)
+000552c0: 3a0a 2020 2020 2020 2020 6368 6563 6b65  :.        checke
+000552d0: 645f 736c 6963 655f 7374 6174 7320 3d20  d_slice_stats = 
+000552e0: 7b7d 0a20 2020 2020 2020 2066 6f72 2062  {}.        for b
+000552f0: 795f 736c 6963 652c 2073 7461 7473 2069  y_slice, stats i
+00055300: 6e20 736c 6963 655f 7374 6174 732e 6974  n slice_stats.it
+00055310: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00055320: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00055330: 2873 7461 7473 2c20 7374 7229 3a0a 2020  (stats, str):.  
+00055340: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00055350: 6563 6b65 645f 736c 6963 655f 7374 6174  ecked_slice_stat
+00055360: 735b 6279 5f73 6c69 6365 5d20 3d20 5b73  s[by_slice] = [s
+00055370: 7461 7473 5d0a 2020 2020 2020 2020 2020  tats].          
+00055380: 2020 656c 6966 2073 6b72 742e 636f 7265    elif skrt.core
+00055390: 2e69 735f 6c69 7374 2873 7461 7473 293a  .is_list(stats):
+000553a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000553b0: 2063 6865 636b 6564 5f73 6c69 6365 5f73   checked_slice_s
+000553c0: 7461 7473 5b62 795f 736c 6963 655d 203d  tats[by_slice] =
+000553d0: 206c 6973 7428 7374 6174 7329 0a20 2020   list(stats).   
+000553e0: 2020 2020 2073 6c69 6365 5f73 7461 7473       slice_stats
+000553f0: 203d 2063 6865 636b 6564 5f73 6c69 6365   = checked_slice
+00055400: 5f73 7461 7473 0a0a 2020 2020 6966 2069  _stats..    if i
+00055410: 7369 6e73 7461 6e63 6528 736c 6963 655f  sinstance(slice_
+00055420: 7374 6174 732c 2064 6963 7429 3a0a 2020  stats, dict):.  
+00055430: 2020 2020 2020 7265 7475 726e 2073 6c69        return sli
+00055440: 6365 5f73 7461 7473 0a0a 2020 2020 7265  ce_stats..    re
+00055450: 7475 726e 207b 7d0a                      turn {}.
```

### Comparing `scikit-rt-0.4.1/src/skrt/viewer/core.py` & `scikit-rt-0.4.2/src/skrt/viewer/core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/src/skrt/viewer/viewer.py` & `scikit-rt-0.4.2/src/skrt/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_01_setup.py` & `scikit-rt-0.4.2/tests/test_01_setup.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_application.py` & `scikit-rt-0.4.2/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_core.py` & `scikit-rt-0.4.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_dose.py` & `scikit-rt-0.4.2/tests/test_dose.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_image.py` & `scikit-rt-0.4.2/tests/test_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import shutil
 import pydicom
 
 from pydicom._storage_sopclass_uids import\
         PositronEmissionTomographyImageStorage
 
 from skrt.core import File, fullpath
-from skrt.image import (Image, get_alignment_translation, get_geometry,
-                        get_mask_bbox, get_translation_to_align, match_images,
-                        match_image_voxel_sizes, checked_crop_limits)
+from skrt.image import (Image, checked_crop_limits, get_alignment_translation,
+                        get_geometry, get_mask_bbox, get_translation_to_align,
+                        match_images, match_image_voxel_sizes, rescale_images)
 from skrt.simulation import SyntheticImage
 
 try:
     import mahotas
     has_mahotas = True
 except ModuleNotFoundError:
     has_mahotas = False
@@ -818,21 +818,41 @@
 
     for i_ax, reductions in enumerate(dxyz):
         dv1, dv2 = reductions
         assert im1.get_extents()[i_ax][0] + dv1 == im2.get_extents()[i_ax][0]
         assert im1.get_extents()[i_ax][1] - dv2 == im2.get_extents()[i_ax][1]
 
 def test_crop_to_roi():
+    """Text cropping to ROI and StructureSet."""
+    # Create test image, featuring cuboid.
     sim = SyntheticImage((10, 12, 10), origin=(0.5, 0.5, 0.5), noise_std=100)
     sim.add_cuboid((4, 2, 6), name="cuboid")
+    ss = sim.get_structure_set()
     roi = sim.get_roi("cuboid")
-    im = sim.get_image()
-    im.crop_to_roi(roi)
-    for i in range(2):
-        assert set(roi.get_extents()[i]) == set(im.image_extent[i])
+
+    for obj in [roi, ss]:
+        # Check that image extents, after cropping to an ROI or StructureSet,
+        # are the same as the extents of the ROI or StructureSet.
+        im = sim.get_image().clone()
+        im.crop_to_roi(obj)
+        assert np.all(obj.get_extents()
+                      == [list(extent) for extent in im.get_extents()])
+
+        # Check that image extents, after cropping about the centre
+        # of an ROI or StructureSet, are as expected from the
+        # centre coordinates of the ROI or StructureSet plus margins.
+        im = sim.get_image().clone()
+        crop_margins = (2, 1, (-3, 3))
+        im.crop_to_roi(obj, crop_margins=crop_margins, crop_about_centre=True)
+        centre = obj.get_centre()
+        margins = checked_crop_limits(crop_margins)
+        assert np.all(im.get_centre() == centre)
+        extents = [(centre[idx] + margins[idx][0],
+                    centre[idx] + margins[idx][1]) for idx in range(3)]
+        assert np.all(extents == im.get_extents())
 
 def test_crop_to_image():
     # Create test images.
     sim1 = SyntheticImage((10, 12, 10), origin=(0.5, 0.5, 0.5))
     im1 = sim1.get_image()
     sim2 = SyntheticImage((12, 14, 12), origin=(5.5, 5.5, 5.5))
     im2 = sim2.get_image()
@@ -972,18 +992,22 @@
         assert np.all(mask1 == mask2)
 
 @needs_mahotas
 def test_translation_to_align():
     """Test calculation of translation to align pair of images."""
 
     # Create synthetic images featuring a sphere.
-    shapes = [(100, 100, 40), (80, 80, 50)]
-    origins = [(-50, 40, -20), (0, -10, 30)]
-    centres = [(30, 80, 0), (60, 40, 50)]
-    radii = (10, 15)
+    # shapes = [(100, 100, 40), (80, 80, 50)]
+    # origins = [(-50, 40, -20), (0, -10, 30)]
+    # centres = [(30, 80, 0), (60, 40, 50)]
+    # radii = (10, 15)
+    shapes = [(50, 50, 20), (40, 40, 25)]
+    origins = [(-25, 20, -10), (0, -5, 15)]
+    centres = [(15, 40, 0), (30, 20, 25)]
+    radii = (5, 8)
     intensity=50
     sims = []
     for idx in range(len(shapes)):
         sims.append(SyntheticImage(shapes[idx], origin=origins[idx]))
         sims[idx].add_sphere(radius=radii[idx], name="sphere",
                 centre=centres[idx], intensity=intensity)
 
@@ -1473,7 +1497,89 @@
     variants = [("mi", None), ("nmi", 2), ("iqr", 1), ("rajski", 0)]
     for variant, value in variants:
         for base in [None, 2, 10]:
             test_value = value if value is not None else pytest.approx(
                     math.log(4, (base or math.e)), small_number)
             assert (im1.get_mutual_information(im2, base=base, variant=variant)
                     == test_value)
+
+def test_rescale_images():
+    """Test rescaling of image greyscale values."""
+    
+    # Create test image, and obtain greyscale characteristics.
+    im = create_test_image(shape, voxel_size, origin)
+    im.data = im.data - (0.5 * im.get_max())
+    u_min = im.get_min(force=True)
+    u_max = im.get_max(force=True)
+    du = u_max - u_min
+    u_sum = im.data.sum()
+
+    # Rescale image.
+    v_min = 0.
+    v_max = 100.
+    constant = 50.
+    dv = v_max - v_min
+    im2 = rescale_images(im, v_min, v_max, constant, clone=False)[0]
+
+    # Check greyscale characteristics of rescaled image.
+    assert im2 is im
+    assert im2.get_min(force=True) == v_min
+    assert im2.get_max(force=True) == v_max
+    assert ((u_min + ((im2.data - v_min) * (du / dv))).sum()
+            == pytest.approx(u_sum, rel=0.001))
+
+    # Check greyscale value after rescaling,
+    # when initial greyscale values are all the same.
+    v_fill = 10
+    im.data.fill(v_fill)
+    im2 = rescale_images((im,), v_min, v_max, constant, clone=True)[0]
+    assert im2 is not im
+    assert np.all(im2.data == constant)
+    assert np.all(im2.data != im.data)
+
+    # Check that original image is returned
+    # when lower or upper bound for rescaling is None,
+    for v_min2, v_max2 in [(None, v_max), (v_min, None)]:
+        im2 = rescale_images([im], v_min2, v_max2, constant, clone=True)[0]
+        assert im2 is im
+        assert np.all(im2.data == v_fill)
+
+def test_get_relative_structural_content():
+    """Test calculation of relative structural content."""
+    # For image compared with itself,
+    # check that relative structural content is 1.
+    im1 = create_test_image(shape, voxel_size, origin)
+    for v_min, v_max in [(None, None), (0, 1)]:
+        assert im1.get_relative_structural_content(im1, v_min, v_max) == 1
+
+    # For image of zeros (after rescaling), compared with another image,
+    # check that relative structural content is 0.
+    im2 = im1.clone()
+    im2.data.fill(5)
+    assert im2.get_relative_structural_content(
+            im1, v_min=0, v_max=1, constant=0) == 0
+
+def test_get_fidelity():
+    """Test calculation of fidelity."""
+    # For image compared with itself, check that fidelity is 1.
+    im1 = create_test_image(shape, voxel_size, origin)
+    for v_min, v_max in [(None, None), (0, 1)]:
+        assert im1.get_fidelity(im1, v_min, v_max) == 1
+
+    # For image of zeros (after rescaling), compared with another image,
+    # check that fidelity is 0.
+    im2 = im1.clone()
+    im2.data.fill(5)
+    assert im2.get_fidelity(im1, v_min=0, v_max=1, constant=0) == 0
+
+def test_get_correlation_quality():
+    """Test calculation of correlation quality."""
+    # For image compared with itself, check that correlation_quality is 1.
+    im1 = create_test_image(shape, voxel_size, origin)
+    for v_min, v_max in [(None, None), (0, 1)]:
+        assert im1.get_correlation_quality(im1, v_min, v_max) == 1
+
+    # For image of zeros (after rescaling), compared with another image,
+    # check that correlation quality is 0.
+    im2 = im1.clone()
+    im2.data.fill(5)
+    assert im2.get_correlation_quality(im1, v_min=0, v_max=1, constant=0) == 0
```

### Comparing `scikit-rt-0.4.1/tests/test_multi.py` & `scikit-rt-0.4.2/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_patient.py` & `scikit-rt-0.4.2/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_qv_image.py` & `scikit-rt-0.4.2/tests/test_qv_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_qv_quickviewer.py` & `scikit-rt-0.4.2/tests/test_qv_quickviewer.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_qv_struct_loader.py` & `scikit-rt-0.4.2/tests/test_qv_struct_loader.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_qv_struct_metrics.py` & `scikit-rt-0.4.2/tests/test_qv_struct_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_qv_structs.py` & `scikit-rt-0.4.2/tests/test_qv_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_registration.py` & `scikit-rt-0.4.2/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_roi_metrics.py` & `scikit-rt-0.4.2/tests/test_roi_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_segmentation.py` & `scikit-rt-0.4.2/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_structs.py` & `scikit-rt-0.4.2/tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_synthetic_image.py` & `scikit-rt-0.4.2/tests/test_synthetic_image.py`

 * *Files identical despite different names*

### Comparing `scikit-rt-0.4.1/tests/test_viewer.py` & `scikit-rt-0.4.2/tests/test_viewer.py`

 * *Files identical despite different names*

