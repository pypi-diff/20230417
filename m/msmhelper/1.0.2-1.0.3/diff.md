# Comparing `tmp/msmhelper-1.0.2.tar.gz` & `tmp/msmhelper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmhelper-1.0.2.tar", last modified: Mon Mar 13 13:09:37 2023, max compression
+gzip compressed data, was "msmhelper-1.0.3.tar", last modified: Mon Apr 17 15:33:59 2023, max compression
```

## Comparing `msmhelper-1.0.2.tar` & `msmhelper-1.0.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.462443 msmhelper-1.0.2/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1517 2023-01-16 20:46:41.000000 msmhelper-1.0.2/LICENSE
--rw-r--r--   0 braniii   (1000) braniii   (1001)       31 2022-08-01 13:42:38.000000 msmhelper-1.0.2/MANIFEST.in
--rw-r--r--   0 braniii   (1000) braniii   (1001)     9769 2023-03-13 13:09:37.462443 msmhelper-1.0.2/PKG-INFO
--rw-r--r--   0 braniii   (1000) braniii   (1001)     8669 2023-03-03 22:25:39.000000 msmhelper-1.0.2/README.md
--rw-r--r--   0 braniii   (1000) braniii   (1001)      606 2023-03-01 21:12:03.000000 msmhelper-1.0.2/extra-requirements.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)      917 2023-03-13 13:09:37.462443 msmhelper-1.0.2/setup.cfg
--rw-r--r--   0 braniii   (1000) braniii   (1001)     3370 2023-03-13 13:06:25.000000 msmhelper-1.0.2/setup.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.429105 msmhelper-1.0.2/src/
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.435772 msmhelper-1.0.2/src/msmhelper/
--rw-r--r--   0 braniii   (1000) braniii   (1001)      611 2023-03-13 13:06:40.000000 msmhelper-1.0.2/src/msmhelper/__init__.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1375 2023-03-13 13:05:54.000000 msmhelper-1.0.2/src/msmhelper/__main__.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.445774 msmhelper-1.0.2/src/msmhelper/_cli/
--rw-r--r--   0 braniii   (1000) braniii   (1001)        0 2023-02-19 19:19:30.000000 msmhelper-1.0.2/src/msmhelper/_cli/__init__.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     3391 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/_cli/ck_test.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     1167 2023-03-13 13:05:54.000000 msmhelper-1.0.2/src/msmhelper/_cli/compare_discretization.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     6398 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/_cli/contact_rep.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1619 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/_cli/dynamical_coring.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1811 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/_cli/gaussian_filter.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     4021 2023-03-08 20:28:26.000000 msmhelper-1.0.2/src/msmhelper/_cli/implied_timescales.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     3162 2023-03-08 20:28:26.000000 msmhelper-1.0.2/src/msmhelper/_cli/waiting_time_dist.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     4310 2023-03-08 20:28:26.000000 msmhelper-1.0.2/src/msmhelper/_cli/waiting_times.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     7487 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/io.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.449108 msmhelper-1.0.2/src/msmhelper/md/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1308 2023-02-19 19:19:30.000000 msmhelper-1.0.2/src/msmhelper/md/__init__.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4802 2023-03-13 13:05:54.000000 msmhelper-1.0.2/src/msmhelper/md/comparison.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4852 2023-02-01 19:56:18.000000 msmhelper-1.0.2/src/msmhelper/md/corrections.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     6160 2023-02-26 20:59:26.000000 msmhelper-1.0.2/src/msmhelper/md/timescales.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.449108 msmhelper-1.0.2/src/msmhelper/msm/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1507 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/msm/__init__.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     3650 2023-02-19 19:19:30.000000 msmhelper-1.0.2/src/msmhelper/msm/msm.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4485 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/msm/tests.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)    17035 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/msm/timescales.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.452442 msmhelper-1.0.2/src/msmhelper/msm/utils/
--rw-r--r--   0 braniii   (1000) braniii   (1001)       74 2023-03-13 13:05:54.000000 msmhelper-1.0.2/src/msmhelper/msm/utils/__init__.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     3850 2023-01-26 18:16:43.000000 msmhelper-1.0.2/src/msmhelper/msm/utils/linalg.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.452442 msmhelper-1.0.2/src/msmhelper/plot/
--rw-r--r--   0 braniii   (1000) braniii   (1001)      277 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/plot/__init__.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     4110 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/plot/_ck_test.py
--rwxr-xr-x   0 braniii   (1000) braniii   (1001)     3962 2023-03-08 20:28:26.000000 msmhelper-1.0.2/src/msmhelper/plot/_wtd.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)    15926 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/statetraj.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.455776 msmhelper-1.0.2/src/msmhelper/utils/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1240 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/utils/__init__.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)    10768 2023-01-26 18:16:43.000000 msmhelper-1.0.2/src/msmhelper/utils/_utils.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     6984 2023-02-26 20:59:26.000000 msmhelper-1.0.2/src/msmhelper/utils/datasets.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     2678 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/utils/filtering.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4706 2023-03-03 22:25:39.000000 msmhelper-1.0.2/src/msmhelper/utils/tests.py
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.439106 msmhelper-1.0.2/src/msmhelper.egg-info/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     9769 2023-03-13 13:09:37.000000 msmhelper-1.0.2/src/msmhelper.egg-info/PKG-INFO
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1623 2023-03-13 13:09:37.000000 msmhelper-1.0.2/src/msmhelper.egg-info/SOURCES.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)        1 2023-03-13 13:09:37.000000 msmhelper-1.0.2/src/msmhelper.egg-info/dependency_links.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)       48 2023-03-13 13:09:37.000000 msmhelper-1.0.2/src/msmhelper.egg-info/entry_points.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)      534 2023-03-13 13:09:37.000000 msmhelper-1.0.2/src/msmhelper.egg-info/requires.txt
--rw-r--r--   0 braniii   (1000) braniii   (1001)       10 2023-03-13 13:09:37.000000 msmhelper-1.0.2/src/msmhelper.egg-info/top_level.txt
-drwxr-xr-x   0 braniii   (1000) braniii   (1001)        0 2023-03-13 13:09:37.462443 msmhelper-1.0.2/test/
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4869 2023-03-13 13:05:54.000000 msmhelper-1.0.2/test/test___main__.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     5090 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_io.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     3267 2023-03-13 13:05:54.000000 msmhelper-1.0.2/test/test_md_comparison.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     5003 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_md_corrections.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1816 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_md_timescales.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     3674 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_msm_msm.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     2141 2023-03-03 22:25:39.000000 msmhelper-1.0.2/test/test_msm_tests.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     7504 2023-03-03 22:25:39.000000 msmhelper-1.0.2/test/test_msm_timescales.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     2271 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_msm_utils_linalg.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     1800 2023-03-03 22:25:39.000000 msmhelper-1.0.2/test/test_plot.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     8587 2023-02-01 19:56:18.000000 msmhelper-1.0.2/test/test_statetraj.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     5657 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_utils__utils.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     2010 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_utils_filtering.py
--rw-r--r--   0 braniii   (1000) braniii   (1001)     4295 2023-01-26 18:16:43.000000 msmhelper-1.0.2/test/test_utils_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-17 15:33:47.000000 msmhelper-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 15:33:47.000000 msmhelper-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-17 15:33:59.035167 msmhelper-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-04-17 15:33:47.000000 msmhelper-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-17 15:33:47.000000 msmhelper-1.0.3/extra-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-17 15:33:59.035167 msmhelper-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-17 15:33:47.000000 msmhelper-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/msmhelper/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/msmhelper/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/ck_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/compare_discretization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6398 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/contact_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/dynamical_coring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/gaussian_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4021 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/implied_timescales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3162 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/waiting_time_dist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4457 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/_cli/waiting_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/md/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/md/timescales.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/msm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/msm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17035 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/timescales.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/msm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/msm/utils/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/plot/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/plot/_ck_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3962 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/plot/_wtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/statetraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/src/msmhelper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-17 15:33:47.000000 msmhelper-1.0.3/src/msmhelper/utils/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.031167 msmhelper-1.0.3/src/msmhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 15:33:59.000000 msmhelper-1.0.3/src/msmhelper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:33:59.035167 msmhelper-1.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test___main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_md_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_md_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_md_timescales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_msm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_timescales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_msm_utils_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_statetraj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_utils__utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_utils_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-17 15:33:47.000000 msmhelper-1.0.3/test/test_utils_tests.py
```

### Comparing `msmhelper-1.0.2/LICENSE` & `msmhelper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/PKG-INFO` & `msmhelper-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmhelper
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper functions for Markov State Models.
 Home-page: https://github.com/moldyn/msmhelper
 Author: braniii
 License: BSD-3-Clause License
 Project-URL: Documentation, https://moldyn.github.io/msmhelper
 Project-URL: Source Code, https://github.com/moldyn/msmhelper
 Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
@@ -29,14 +29,16 @@
 License-File: LICENSE
 
 <div align="center">
   
   <img class="lightmode" style="width: 400px;" src="https://github.com/moldyn/msmhelper/blob/main/docs/logo_large_light.svg?raw=true#gh-light-mode-only" />
 
   <p>
+    <a href="https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd">
+        <img src="https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd/status.svg" /></a>
     <a href="https://github.com/wemake-services/wemake-python-styleguide" alt="wemake-python-styleguide">
         <img src="https://img.shields.io/badge/style-wemake-000000.svg" /></a>
     <a href="https://pypi.org/project/msmhelper" alt="PyPI">
         <img src="https://img.shields.io/pypi/v/msmhelper" /></a>
     <a href="https://anaconda.org/conda-forge/msmhelper" alt="conda version">
         <img src="https://img.shields.io/conda/vn/conda-forge/msmhelper" /></a>
     <a href="https://pepy.tech/project/msmhelper" alt="Downloads">
@@ -74,26 +76,26 @@
 
 We kindly ask you to cite this article in case you use this software package for published works.
 
 ## Features
 - Simple usage with sleek function-based API
 - High performance due to [numba](https://numba.pydata.org/)-optimized source code, checkout the [benchmark comparing to PyEMMA](https://moldyn.github.io/msmhelper/benchmark)
 - [Documentation](https://moldyn.github.io/msmhelper) including tutorials
-- Powerful command line interface (CLI) to create publication-ready figures
+- Powerful command-line interface (CLI) to create publication-ready figures
 - Supports Python 3.7-3.10
-- Many helpful functions for dealing with state trajectories
 
 ## Implemented Key Functionalities
 - Hummer-Szabo projection of optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/10.1021/jp508375q)
 - Dynamical coring by [Nagel et al. 2019](https://doi.org/10.1063/1.5081767)
 - Fast extraction of pathways and MSM-based prediction of pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/doi/10.1021/acs.jctc.0c00774)
 - Fast calculation of waiting times based on both, state trajectories and MSMs
 - Blazing fast [Chapman-Kolmogorov](https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation
-- Entropy-based comparison of different state discretizations
-- Contact representation by Nagel et al. 2023 (submitted) for a compact structural representation of the states
+- Entropy-based similarity measure to compare different state discretizations, this method will be published soon in Nagel 2023
+- Contact representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact structural representation of the states
+- Command-line interface providing both, visualization and analysis methods
 - Provide (non-reversible) transition matrix of all states (corresponds in pyemma to `connectivity='none', 'all'` which will (probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/_msm_estimator_base.py#L110))
 
 ## Getting started
 ### Installation
 The package is called `msmhelper` and is available via [PyPI](https://pypi.org/project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install it, simply call:
 ```bash
 python3 -m pip install --upgrade msmhelper
@@ -122,27 +124,27 @@
 ```
 In general one can call the module directly by its entry point `$ msmhelper`
 or by calling the module `$ python -m msmhelper`. The latter method is
 preferred to ensure using the desired python environment. For enabling
 the shell completion, the entry point needs to be used.
 
 ## Usage
-This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/reference/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the (following section)[#Hummer-Szabo-Projection].
+This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the [following section](#hummer-szabo-projection).
 ```python
 import msmhelper as mh
 
 # open text files
 traj = mh.openmicrostates(filename, limitsfile)
 # create markov state model
 tmat, states = mh.estimate_markov_model(traj, lagtime=1)
 ...
 ```
 
 ## Hummer-Szabo Projection
-In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
+In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
 
 | Method | MSM | Hummer-Szabo MSM |
 | :---: | :---: | :---: |
 | Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) |
 | Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) |
 | Waiting Time Distributions | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) |
 | Waiting Times | [![waiting times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wts.jpg)](reference/cli/#msmhelper-waiting-times) | [![waiting times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wts.jpg)](reference/cli/#msmhelper-waiting-times) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msmhelper Version: 1.0.2 Summary: Helper functions
+Metadata-Version: 2.1 Name: msmhelper Version: 1.0.3 Summary: Helper functions
 for Markov State Models. Home-page: https://github.com/moldyn/msmhelper Author:
 braniii License: BSD-3-Clause License Project-URL: Documentation, https://
 moldyn.github.io/msmhelper Project-URL: Source Code, https://github.com/moldyn/
 msmhelper Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
 Project-URL: Bug Tracker, https://github.com/moldyn/msmhelper/issues Keywords:
 MSM,Markov model,Markov state model,MD analysis Classifier: License :: OSI
 Approved :: BSD License Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,15 @@
 Topic :: Scientific/Engineering :: Physics Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.7 Description-Content-Type:
 text/markdown Provides-Extra: testing Provides-Extra: docs Provides-Extra: all
 License-File: LICENSE
              [https://github.com/moldyn/msmhelper/blob/main/docs/
                logo_large_light.svg?raw=true#gh-light-mode-only]
+ [https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd/status.svg]
 [https://img.shields.io/badge/style-wemake-000000.svg] [https://img.shields.io/
   pypi/v/msmhelper] [https://img.shields.io/conda/vn/conda-forge/msmhelper]
   [https://pepy.tech/badge/msmhelper] [https://img.shields.io/github/actions/
  workflow/status/moldyn/msmhelper/pytest.yml?branch=main] [https://codecov.io/
   gh/moldyn/msmhelper/branch/main/graph/badge.svg?token=Ce2eW5JICI] [https://
 github.com/moldyn/msmhelper/actions/workflows/codeql.yml/badge.svg?branch=main]
   [https://img.shields.io/pypi/pyversions/msmhelper] [https://img.shields.io/
@@ -37,30 +38,31 @@
 published soon: > D. Nagel, and G. Stock, > *msmhelper: A Python Package for
 Markov State Modeling of Protein Dynamics*, > in preparation We kindly ask you
 to cite this article in case you use this software package for published works.
 ## Features - Simple usage with sleek function-based API - High performance due
 to [numba](https://numba.pydata.org/)-optimized source code, checkout the
 [benchmark comparing to PyEMMA](https://moldyn.github.io/msmhelper/benchmark) -
 [Documentation](https://moldyn.github.io/msmhelper) including tutorials -
-Powerful command line interface (CLI) to create publication-ready figures -
-Supports Python 3.7-3.10 - Many helpful functions for dealing with state
-trajectories ## Implemented Key Functionalities - Hummer-Szabo projection of
-optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/
-10.1021/jp508375q) - Dynamical coring by [Nagel et al. 2019](https://doi.org/
-10.1063/1.5081767) - Fast extraction of pathways and MSM-based prediction of
-pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/
-doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times based on
-both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov](https://
-www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation -
-Entropy-based comparison of different state discretizations - Contact
-representation by Nagel et al. 2023 (submitted) for a compact structural
-representation of the states - Provide (non-reversible) transition matrix of
-all states (corresponds in pyemma to `connectivity='none', 'all'` which will
-(probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/
-5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
+Powerful command-line interface (CLI) to create publication-ready figures -
+Supports Python 3.7-3.10 ## Implemented Key Functionalities - Hummer-Szabo
+projection of optimal dimensionality reduction by [Hummer and Szabo 2014]
+(https://doi.org/10.1021/jp508375q) - Dynamical coring by [Nagel et al. 2019]
+(https://doi.org/10.1063/1.5081767) - Fast extraction of pathways and MSM-based
+prediction of pathways based on the definition of [Nagel et al. 2020](https://
+pubs.acs.org/doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times
+based on both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov]
+(https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test
+implementation - Entropy-based similarity measure to compare different state
+discretizations, this method will be published soon in Nagel 2023 - Contact
+representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact
+structural representation of the states - Command-line interface providing
+both, visualization and analysis methods - Provide (non-reversible) transition
+matrix of all states (corresponds in pyemma to `connectivity='none', 'all'`
+which will (probably) [never be implemented](https://github.com/markovmodel/
+PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
 _msm_estimator_base.py#L110)) ## Getting started ### Installation The package
 is called `msmhelper` and is available via [PyPI](https://pypi.org/project/
 msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install
 it, simply call: ```bash python3 -m pip install --upgrade msmhelper ``` or ```
 conda install -c conda-forge msmhelper ``` or for the latest dev version
 ```bash # via ssh key python3 -m pip install git+ssh://git@github.com/moldyn/
 msmhelper.git # or via password-based login python3 -m pip install git+https://
@@ -71,44 +73,45 @@
 `~/.bashrc` ```bash eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In
 general one can call the module directly by its entry point `$ msmhelper` or by
 calling the module `$ python -m msmhelper`. The latter method is preferred to
 ensure using the desired python environment. For enabling the shell completion,
 the entry point needs to be used. ## Usage This package offers either a
 [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to
 run standalone analysis and to create commonly-used figures, or its much more
-powerful [API](https://moldyn.github.io/msmhelper/reference/msmhelper) can be
+powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be
 used to embedded it into an existing Python workflow. Check out the
 documentation for an overview over all modules and some example workflows, and
-for some examples see the (following section)[#Hummer-Szabo-Projection].
+for some examples see the [following section](#hummer-szabo-projection).
 ```python import msmhelper as mh # open text files traj = mh.openmicrostates
 (filename, limitsfile) # create markov state model tmat, states =
 mh.estimate_markov_model(traj, lagtime=1) ... ``` ## Hummer-Szabo Projection In
 the following we show some sample figures produced directly with the command
-line tools. For more information on that, there is a [tutorial](tutorials/
-hummerszabo) explaining the methods more in depth. In general we can see, that
-applying the HS-projection removes most projection artifacts based on coarse-
-graining many microstates into a few macrostates. | Method | MSM | Hummer-Szabo
-MSM | | :---: | :---: | :---: | | Implied Timescales | [![Implied Timescales]
-(https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)]
-(reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/
-#msmhelper-implied-timescales) | | Chapman-Kolmogorov test | [![Chapman-
-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/
-8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [!
-[Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/
-8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | |
-Waiting Time Distributions | [![waiting time distribution](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/
-#msmhelper-waiting-time-dist) | [![waiting time distribution](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/
-#msmhelper-waiting-time-dist) | | Waiting Times | [![waiting times](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.wts.jpg)](reference/cli/
-#msmhelper-waiting-times) | [![waiting times](https://moldyn.github.io/
-msmhelper/assets/8state_macrotraj.sh.wts.jpg)](reference/cli/#msmhelper-
-waiting-times) | | Contact Representation | [![contact representation](https://
-moldyn.github.io/msmhelper/assets/hp35.contactRep.state1-12.jpg)](reference/
-cli/#msmhelper-contact-rep) | | For more examples checkout the [tutorials]
-(https://moldyn.github.io/msmhelper/tutorials). ## Roadmap - Add [Buchete-
-Hummer test](https://doi.org/10.1021/jp0761665) as alternative for the Chapman-
-Kolmogorov test. - Add a numba implementation of a parallelized autocorrelation
-function estimation. - Use static type hints together with [beartype](https://
-github.com/beartype/beartype)
+line tools. For more information on that, there is a [tutorial](https://
+moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more
+in depth. In general we can see, that applying the HS-projection removes most
+projection artifacts based on coarse-graining many microstates into a few
+macrostates. | Method | MSM | Hummer-Szabo MSM | | :---: | :---: | :---: | |
+Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/
+assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales)
+| [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | |
+Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
+msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/
+#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
+msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/
+#msmhelper-ck-test) | | Waiting Time Distributions | [![waiting time
+distribution](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [!
+[waiting time distribution](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | |
+Waiting Times | [![waiting times](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.wts.jpg)](reference/cli/#msmhelper-waiting-times) | [![waiting
+times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wts.jpg)]
+(reference/cli/#msmhelper-waiting-times) | | Contact Representation | [!
+[contact representation](https://moldyn.github.io/msmhelper/assets/
+hp35.contactRep.state1-12.jpg)](reference/cli/#msmhelper-contact-rep) | | For
+more examples checkout the [tutorials](https://moldyn.github.io/msmhelper/
+tutorials). ## Roadmap - Add [Buchete-Hummer test](https://doi.org/10.1021/
+jp0761665) as alternative for the Chapman-Kolmogorov test. - Add a numba
+implementation of a parallelized autocorrelation function estimation. - Use
+static type hints together with [beartype](https://github.com/beartype/
+beartype)
```

### Comparing `msmhelper-1.0.2/README.md` & `msmhelper-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 <div align="center">
   <img class="darkmode" style="width: 400px;" src="https://github.com/moldyn/msmhelper/blob/main/docs/logo_large_dark.svg?raw=true#gh-dark-mode-only" />
   <img class="lightmode" style="width: 400px;" src="https://github.com/moldyn/msmhelper/blob/main/docs/logo_large_light.svg?raw=true#gh-light-mode-only" />
 
   <p>
+    <a href="https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd">
+        <img src="https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd/status.svg" /></a>
     <a href="https://github.com/wemake-services/wemake-python-styleguide" alt="wemake-python-styleguide">
         <img src="https://img.shields.io/badge/style-wemake-000000.svg" /></a>
     <a href="https://pypi.org/project/msmhelper" alt="PyPI">
         <img src="https://img.shields.io/pypi/v/msmhelper" /></a>
     <a href="https://anaconda.org/conda-forge/msmhelper" alt="conda version">
         <img src="https://img.shields.io/conda/vn/conda-forge/msmhelper" /></a>
     <a href="https://pepy.tech/project/msmhelper" alt="Downloads">
@@ -44,26 +46,26 @@
 
 We kindly ask you to cite this article in case you use this software package for published works.
 
 ## Features
 - Simple usage with sleek function-based API
 - High performance due to [numba](https://numba.pydata.org/)-optimized source code, checkout the [benchmark comparing to PyEMMA](https://moldyn.github.io/msmhelper/benchmark)
 - [Documentation](https://moldyn.github.io/msmhelper) including tutorials
-- Powerful command line interface (CLI) to create publication-ready figures
+- Powerful command-line interface (CLI) to create publication-ready figures
 - Supports Python 3.7-3.10
-- Many helpful functions for dealing with state trajectories
 
 ## Implemented Key Functionalities
 - Hummer-Szabo projection of optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/10.1021/jp508375q)
 - Dynamical coring by [Nagel et al. 2019](https://doi.org/10.1063/1.5081767)
 - Fast extraction of pathways and MSM-based prediction of pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/doi/10.1021/acs.jctc.0c00774)
 - Fast calculation of waiting times based on both, state trajectories and MSMs
 - Blazing fast [Chapman-Kolmogorov](https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation
-- Entropy-based comparison of different state discretizations
-- Contact representation by Nagel et al. 2023 (submitted) for a compact structural representation of the states
+- Entropy-based similarity measure to compare different state discretizations, this method will be published soon in Nagel 2023
+- Contact representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact structural representation of the states
+- Command-line interface providing both, visualization and analysis methods
 - Provide (non-reversible) transition matrix of all states (corresponds in pyemma to `connectivity='none', 'all'` which will (probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/_msm_estimator_base.py#L110))
 
 ## Getting started
 ### Installation
 The package is called `msmhelper` and is available via [PyPI](https://pypi.org/project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install it, simply call:
 ```bash
 python3 -m pip install --upgrade msmhelper
@@ -92,27 +94,27 @@
 ```
 In general one can call the module directly by its entry point `$ msmhelper`
 or by calling the module `$ python -m msmhelper`. The latter method is
 preferred to ensure using the desired python environment. For enabling
 the shell completion, the entry point needs to be used.
 
 ## Usage
-This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/reference/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the (following section)[#Hummer-Szabo-Projection].
+This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the [following section](#hummer-szabo-projection).
 ```python
 import msmhelper as mh
 
 # open text files
 traj = mh.openmicrostates(filename, limitsfile)
 # create markov state model
 tmat, states = mh.estimate_markov_model(traj, lagtime=1)
 ...
 ```
 
 ## Hummer-Szabo Projection
-In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
+In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
 
 | Method | MSM | Hummer-Szabo MSM |
 | :---: | :---: | :---: |
 | Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) |
 | Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) |
 | Waiting Time Distributions | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) |
 | Waiting Times | [![waiting times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wts.jpg)](reference/cli/#msmhelper-waiting-times) | [![waiting times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wts.jpg)](reference/cli/#msmhelper-waiting-times) |
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
              [https://github.com/moldyn/msmhelper/blob/main/docs/
   logo_large_dark.svg?raw=true#gh-dark-mode-only] [https://github.com/moldyn/
   msmhelper/blob/main/docs/logo_large_light.svg?raw=true#gh-light-mode-only]
+ [https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd/status.svg]
 [https://img.shields.io/badge/style-wemake-000000.svg] [https://img.shields.io/
   pypi/v/msmhelper] [https://img.shields.io/conda/vn/conda-forge/msmhelper]
   [https://pepy.tech/badge/msmhelper] [https://img.shields.io/github/actions/
  workflow/status/moldyn/msmhelper/pytest.yml?branch=main] [https://codecov.io/
   gh/moldyn/msmhelper/branch/main/graph/badge.svg?token=Ce2eW5JICI] [https://
 github.com/moldyn/msmhelper/actions/workflows/codeql.yml/badge.svg?branch=main]
   [https://img.shields.io/pypi/pyversions/msmhelper] [https://img.shields.io/
@@ -21,30 +22,31 @@
 published soon: > D. Nagel, and G. Stock, > *msmhelper: A Python Package for
 Markov State Modeling of Protein Dynamics*, > in preparation We kindly ask you
 to cite this article in case you use this software package for published works.
 ## Features - Simple usage with sleek function-based API - High performance due
 to [numba](https://numba.pydata.org/)-optimized source code, checkout the
 [benchmark comparing to PyEMMA](https://moldyn.github.io/msmhelper/benchmark) -
 [Documentation](https://moldyn.github.io/msmhelper) including tutorials -
-Powerful command line interface (CLI) to create publication-ready figures -
-Supports Python 3.7-3.10 - Many helpful functions for dealing with state
-trajectories ## Implemented Key Functionalities - Hummer-Szabo projection of
-optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/
-10.1021/jp508375q) - Dynamical coring by [Nagel et al. 2019](https://doi.org/
-10.1063/1.5081767) - Fast extraction of pathways and MSM-based prediction of
-pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/
-doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times based on
-both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov](https://
-www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation -
-Entropy-based comparison of different state discretizations - Contact
-representation by Nagel et al. 2023 (submitted) for a compact structural
-representation of the states - Provide (non-reversible) transition matrix of
-all states (corresponds in pyemma to `connectivity='none', 'all'` which will
-(probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/
-5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
+Powerful command-line interface (CLI) to create publication-ready figures -
+Supports Python 3.7-3.10 ## Implemented Key Functionalities - Hummer-Szabo
+projection of optimal dimensionality reduction by [Hummer and Szabo 2014]
+(https://doi.org/10.1021/jp508375q) - Dynamical coring by [Nagel et al. 2019]
+(https://doi.org/10.1063/1.5081767) - Fast extraction of pathways and MSM-based
+prediction of pathways based on the definition of [Nagel et al. 2020](https://
+pubs.acs.org/doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times
+based on both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov]
+(https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test
+implementation - Entropy-based similarity measure to compare different state
+discretizations, this method will be published soon in Nagel 2023 - Contact
+representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact
+structural representation of the states - Command-line interface providing
+both, visualization and analysis methods - Provide (non-reversible) transition
+matrix of all states (corresponds in pyemma to `connectivity='none', 'all'`
+which will (probably) [never be implemented](https://github.com/markovmodel/
+PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
 _msm_estimator_base.py#L110)) ## Getting started ### Installation The package
 is called `msmhelper` and is available via [PyPI](https://pypi.org/project/
 msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install
 it, simply call: ```bash python3 -m pip install --upgrade msmhelper ``` or ```
 conda install -c conda-forge msmhelper ``` or for the latest dev version
 ```bash # via ssh key python3 -m pip install git+ssh://git@github.com/moldyn/
 msmhelper.git # or via password-based login python3 -m pip install git+https://
@@ -55,44 +57,45 @@
 `~/.bashrc` ```bash eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In
 general one can call the module directly by its entry point `$ msmhelper` or by
 calling the module `$ python -m msmhelper`. The latter method is preferred to
 ensure using the desired python environment. For enabling the shell completion,
 the entry point needs to be used. ## Usage This package offers either a
 [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to
 run standalone analysis and to create commonly-used figures, or its much more
-powerful [API](https://moldyn.github.io/msmhelper/reference/msmhelper) can be
+powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be
 used to embedded it into an existing Python workflow. Check out the
 documentation for an overview over all modules and some example workflows, and
-for some examples see the (following section)[#Hummer-Szabo-Projection].
+for some examples see the [following section](#hummer-szabo-projection).
 ```python import msmhelper as mh # open text files traj = mh.openmicrostates
 (filename, limitsfile) # create markov state model tmat, states =
 mh.estimate_markov_model(traj, lagtime=1) ... ``` ## Hummer-Szabo Projection In
 the following we show some sample figures produced directly with the command
-line tools. For more information on that, there is a [tutorial](tutorials/
-hummerszabo) explaining the methods more in depth. In general we can see, that
-applying the HS-projection removes most projection artifacts based on coarse-
-graining many microstates into a few macrostates. | Method | MSM | Hummer-Szabo
-MSM | | :---: | :---: | :---: | | Implied Timescales | [![Implied Timescales]
-(https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)]
-(reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/
-#msmhelper-implied-timescales) | | Chapman-Kolmogorov test | [![Chapman-
-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/
-8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [!
-[Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/
-8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | |
-Waiting Time Distributions | [![waiting time distribution](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/
-#msmhelper-waiting-time-dist) | [![waiting time distribution](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/
-#msmhelper-waiting-time-dist) | | Waiting Times | [![waiting times](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.wts.jpg)](reference/cli/
-#msmhelper-waiting-times) | [![waiting times](https://moldyn.github.io/
-msmhelper/assets/8state_macrotraj.sh.wts.jpg)](reference/cli/#msmhelper-
-waiting-times) | | Contact Representation | [![contact representation](https://
-moldyn.github.io/msmhelper/assets/hp35.contactRep.state1-12.jpg)](reference/
-cli/#msmhelper-contact-rep) | | For more examples checkout the [tutorials]
-(https://moldyn.github.io/msmhelper/tutorials). ## Roadmap - Add [Buchete-
-Hummer test](https://doi.org/10.1021/jp0761665) as alternative for the Chapman-
-Kolmogorov test. - Add a numba implementation of a parallelized autocorrelation
-function estimation. - Use static type hints together with [beartype](https://
-github.com/beartype/beartype)
+line tools. For more information on that, there is a [tutorial](https://
+moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more
+in depth. In general we can see, that applying the HS-projection removes most
+projection artifacts based on coarse-graining many microstates into a few
+macrostates. | Method | MSM | Hummer-Szabo MSM | | :---: | :---: | :---: | |
+Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/
+assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales)
+| [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | |
+Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
+msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/
+#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
+msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/
+#msmhelper-ck-test) | | Waiting Time Distributions | [![waiting time
+distribution](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [!
+[waiting time distribution](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | |
+Waiting Times | [![waiting times](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.wts.jpg)](reference/cli/#msmhelper-waiting-times) | [![waiting
+times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wts.jpg)]
+(reference/cli/#msmhelper-waiting-times) | | Contact Representation | [!
+[contact representation](https://moldyn.github.io/msmhelper/assets/
+hp35.contactRep.state1-12.jpg)](reference/cli/#msmhelper-contact-rep) | | For
+more examples checkout the [tutorials](https://moldyn.github.io/msmhelper/
+tutorials). ## Roadmap - Add [Buchete-Hummer test](https://doi.org/10.1021/
+jp0761665) as alternative for the Chapman-Kolmogorov test. - Add a numba
+implementation of a parallelized autocorrelation function estimation. - Use
+static type hints together with [beartype](https://github.com/beartype/
+beartype)
```

### Comparing `msmhelper-1.0.2/extra-requirements.txt` & `msmhelper-1.0.3/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/setup.cfg` & `msmhelper-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/setup.py` & `msmhelper-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 README = remove_gh_dark_mode_only_tags(
     (HERE / 'README.md').read_text(),
 )
 
 # This call to setup() does all the work
 setuptools.setup(
     name='msmhelper',
-    version='1.0.2',
+    version='1.0.3',
     description='Helper functions for Markov State Models.',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords=[
         'MSM',
         'Markov model',
         'Markov state model',
```

### Comparing `msmhelper-1.0.2/src/msmhelper/__init__.py` & `msmhelper-1.0.3/src/msmhelper/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 from .utils import (
     rename_by_population,
     rename_by_index,
     shift_data,
     unique,
 )
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
```

### Comparing `msmhelper-1.0.2/src/msmhelper/__main__.py` & `msmhelper-1.0.3/src/msmhelper/__main__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/ck_test.py` & `msmhelper-1.0.3/src/msmhelper/_cli/ck_test.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/compare_discretization.py` & `msmhelper-1.0.3/src/msmhelper/_cli/compare_discretization.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/contact_rep.py` & `msmhelper-1.0.3/src/msmhelper/_cli/contact_rep.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/dynamical_coring.py` & `msmhelper-1.0.3/src/msmhelper/_cli/dynamical_coring.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/gaussian_filter.py` & `msmhelper-1.0.3/src/msmhelper/_cli/gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/implied_timescales.py` & `msmhelper-1.0.3/src/msmhelper/_cli/implied_timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/waiting_time_dist.py` & `msmhelper-1.0.3/src/msmhelper/_cli/waiting_time_dist.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/_cli/waiting_times.py` & `msmhelper-1.0.3/src/msmhelper/_cli/waiting_times.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     nsteps,
     frames_per_unit,
     unit,
 ):
     """Estimation and visualization of the waiting times."""
     # setup matplotlib
     pplt.use_style(
-        figsize=2.4, true_black=True, colors='pastel_autunm', latex=False,
+        figsize=2.2, true_black=True, colors='pastel_autunm', latex=False,
     )
 
     # load file
     trajs = mh.openmicrostates(filename, limits_file=concat_limits)
     if microfilename:
         microtrajs = mh.openmicrostates(
             microfilename, limits_file=concat_limits,
@@ -131,33 +131,34 @@
         start=start,
         final=final,
     )
 
     _, ax = plt.subplots()
 
     # ensure using bins as multiple of frames
-    n_bins = 50
+    n_bins = 20
     bins = np.arange(
         0,
         wts_md.max() + 1,
         np.ceil(wts_md.max() / n_bins).astype(int),
     )
     md_hist, md_time = np.histogram(wts_md, bins=bins, density=True)
     ax.stairs(
         md_hist,
         md_time / frames_per_unit,
         fill=True,
         color='k',
         label='MD',
     )
-    for lagtime in lagtimes:
+    for idx, lagtime in enumerate(lagtimes):
         ax.stairs(
             wts[lagtime][0],
             wts[lagtime][1] / frames_per_unit,
             label=f'{lagtime / frames_per_unit}',
+            color=f'C{idx + 1}',
         )
 
     # set legend and labels
     pplt.legend(
         ax=ax,
         outside='right',
         frameon=False,
@@ -168,14 +169,20 @@
 
     # use scientific notation for small values
     ax.ticklabel_format(
         axis='y', style='scientific', scilimits=[-1, 1], useMathText=True,
     )
     ax.get_yaxis().get_offset_text().set_ha('right')
 
+    # set x limits
+    ax.set_xlim(
+        0,
+        wts_md.max() * 2 / frames_per_unit,
+    )
+
     if output is None:
         basename = f'{filename}.sh' if microfilename else filename
         output = f'{basename}.wts.pdf'
     pplt.savefig(output)
 
 
 if __name__ == '__main__':
```

### Comparing `msmhelper-1.0.2/src/msmhelper/io.py` & `msmhelper-1.0.3/src/msmhelper/io.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/md/__init__.py` & `msmhelper-1.0.3/src/msmhelper/md/__init__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/md/comparison.py` & `msmhelper-1.0.3/src/msmhelper/md/comparison.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/md/corrections.py` & `msmhelper-1.0.3/src/msmhelper/md/corrections.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/md/timescales.py` & `msmhelper-1.0.3/src/msmhelper/md/timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/msm/__init__.py` & `msmhelper-1.0.3/src/msmhelper/msm/__init__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/msm/msm.py` & `msmhelper-1.0.3/src/msmhelper/msm/msm.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/msm/tests.py` & `msmhelper-1.0.3/src/msmhelper/msm/tests.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/msm/timescales.py` & `msmhelper-1.0.3/src/msmhelper/msm/timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/msm/utils/linalg.py` & `msmhelper-1.0.3/src/msmhelper/msm/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/plot/_ck_test.py` & `msmhelper-1.0.3/src/msmhelper/plot/_ck_test.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/plot/_wtd.py` & `msmhelper-1.0.3/src/msmhelper/plot/_wtd.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/statetraj.py` & `msmhelper-1.0.3/src/msmhelper/statetraj.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 # Copyright (c) 2019-2023, Daniel Nagel
 # All rights reserved.
 r"""Classes for handling discrete state trajectories.
 
-- [`StateTraj`][#msmhelper.statetraj.StateTraj] is a fast implementation
+- [**StateTraj**][msmhelper.statetraj.StateTraj] is a fast implementation
   of a state trajectory and should be used for microstate dynamics.
 
-- [`LumpedStateTraj`][#msmhelper.statetraj.LumpedStateTraj] is an
+- [**LumpedStateTraj**][msmhelper.statetraj.LumpedStateTraj] is an
   implementation of the Hummer-Szabo projection[^1] and allows to reproduce
   the microstates dynamics on the macrostates space.
 
 !!! note
     One should also mention that for bad coarse-graining one can get negative
     entries in the transition matrix $T_{ij} < 0$. To prevent this, one can
     explicitly force $T_{ij} \ge 0$ by setting the flag `positive=True`.
@@ -419,14 +419,30 @@
         return mh.shift_data(
             self._trajs,
             np.arange(self.nmicrostates),
             self._state_assignment,
         )
 
     @property
+    def index_trajs(self):
+        """Return index trajectory.
+
+        Returns
+        -------
+        trajs : list of ndarrays
+            List of ndarrays holding the input data.
+
+        """
+        return mh.shift_data(
+            self._trajs,
+            np.arange(self.nmicrostates),
+            self._state_assignment_idx,
+        )
+
+    @property
     def microstates(self):
         """Return active set of microstates.
 
         Returns
         -------
         states : ndarray
             Numpy array holding active set of states.
```

### Comparing `msmhelper-1.0.2/src/msmhelper/utils/__init__.py` & `msmhelper-1.0.3/src/msmhelper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/utils/_utils.py` & `msmhelper-1.0.3/src/msmhelper/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/utils/datasets.py` & `msmhelper-1.0.3/src/msmhelper/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/utils/filtering.py` & `msmhelper-1.0.3/src/msmhelper/utils/filtering.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper/utils/tests.py` & `msmhelper-1.0.3/src/msmhelper/utils/tests.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper.egg-info/PKG-INFO` & `msmhelper-1.0.3/src/msmhelper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmhelper
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper functions for Markov State Models.
 Home-page: https://github.com/moldyn/msmhelper
 Author: braniii
 License: BSD-3-Clause License
 Project-URL: Documentation, https://moldyn.github.io/msmhelper
 Project-URL: Source Code, https://github.com/moldyn/msmhelper
 Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
@@ -29,14 +29,16 @@
 License-File: LICENSE
 
 <div align="center">
   
   <img class="lightmode" style="width: 400px;" src="https://github.com/moldyn/msmhelper/blob/main/docs/logo_large_light.svg?raw=true#gh-light-mode-only" />
 
   <p>
+    <a href="https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd">
+        <img src="https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd/status.svg" /></a>
     <a href="https://github.com/wemake-services/wemake-python-styleguide" alt="wemake-python-styleguide">
         <img src="https://img.shields.io/badge/style-wemake-000000.svg" /></a>
     <a href="https://pypi.org/project/msmhelper" alt="PyPI">
         <img src="https://img.shields.io/pypi/v/msmhelper" /></a>
     <a href="https://anaconda.org/conda-forge/msmhelper" alt="conda version">
         <img src="https://img.shields.io/conda/vn/conda-forge/msmhelper" /></a>
     <a href="https://pepy.tech/project/msmhelper" alt="Downloads">
@@ -74,26 +76,26 @@
 
 We kindly ask you to cite this article in case you use this software package for published works.
 
 ## Features
 - Simple usage with sleek function-based API
 - High performance due to [numba](https://numba.pydata.org/)-optimized source code, checkout the [benchmark comparing to PyEMMA](https://moldyn.github.io/msmhelper/benchmark)
 - [Documentation](https://moldyn.github.io/msmhelper) including tutorials
-- Powerful command line interface (CLI) to create publication-ready figures
+- Powerful command-line interface (CLI) to create publication-ready figures
 - Supports Python 3.7-3.10
-- Many helpful functions for dealing with state trajectories
 
 ## Implemented Key Functionalities
 - Hummer-Szabo projection of optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/10.1021/jp508375q)
 - Dynamical coring by [Nagel et al. 2019](https://doi.org/10.1063/1.5081767)
 - Fast extraction of pathways and MSM-based prediction of pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/doi/10.1021/acs.jctc.0c00774)
 - Fast calculation of waiting times based on both, state trajectories and MSMs
 - Blazing fast [Chapman-Kolmogorov](https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation
-- Entropy-based comparison of different state discretizations
-- Contact representation by Nagel et al. 2023 (submitted) for a compact structural representation of the states
+- Entropy-based similarity measure to compare different state discretizations, this method will be published soon in Nagel 2023
+- Contact representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact structural representation of the states
+- Command-line interface providing both, visualization and analysis methods
 - Provide (non-reversible) transition matrix of all states (corresponds in pyemma to `connectivity='none', 'all'` which will (probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/_msm_estimator_base.py#L110))
 
 ## Getting started
 ### Installation
 The package is called `msmhelper` and is available via [PyPI](https://pypi.org/project/msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install it, simply call:
 ```bash
 python3 -m pip install --upgrade msmhelper
@@ -122,27 +124,27 @@
 ```
 In general one can call the module directly by its entry point `$ msmhelper`
 or by calling the module `$ python -m msmhelper`. The latter method is
 preferred to ensure using the desired python environment. For enabling
 the shell completion, the entry point needs to be used.
 
 ## Usage
-This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/reference/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the (following section)[#Hummer-Szabo-Projection].
+This package offers either a [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to run standalone analysis and to create commonly-used figures, or its much more powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be used to embedded it into an existing Python workflow. Check out the documentation for an overview over all modules and some example workflows, and for some examples see the [following section](#hummer-szabo-projection).
 ```python
 import msmhelper as mh
 
 # open text files
 traj = mh.openmicrostates(filename, limitsfile)
 # create markov state model
 tmat, states = mh.estimate_markov_model(traj, lagtime=1)
 ...
 ```
 
 ## Hummer-Szabo Projection
-In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
+In the following we show some sample figures produced directly with the command line tools. For more information on that, there is a [tutorial](https://moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more in depth. In general we can see, that applying the HS-projection removes most projection artifacts based on coarse-graining many microstates into a few macrostates.
 
 | Method | MSM | Hummer-Szabo MSM |
 | :---: | :---: | :---: |
 | Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) |
 | Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) |
 | Waiting Time Distributions | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [![waiting time distribution](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) |
 | Waiting Times | [![waiting times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.wts.jpg)](reference/cli/#msmhelper-waiting-times) | [![waiting times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wts.jpg)](reference/cli/#msmhelper-waiting-times) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msmhelper Version: 1.0.2 Summary: Helper functions
+Metadata-Version: 2.1 Name: msmhelper Version: 1.0.3 Summary: Helper functions
 for Markov State Models. Home-page: https://github.com/moldyn/msmhelper Author:
 braniii License: BSD-3-Clause License Project-URL: Documentation, https://
 moldyn.github.io/msmhelper Project-URL: Source Code, https://github.com/moldyn/
 msmhelper Project-URL: Changelog, https://moldyn.github.io/msmhelper/changelog
 Project-URL: Bug Tracker, https://github.com/moldyn/msmhelper/issues Keywords:
 MSM,Markov model,Markov state model,MD analysis Classifier: License :: OSI
 Approved :: BSD License Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,15 @@
 Topic :: Scientific/Engineering :: Physics Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.7 Description-Content-Type:
 text/markdown Provides-Extra: testing Provides-Extra: docs Provides-Extra: all
 License-File: LICENSE
              [https://github.com/moldyn/msmhelper/blob/main/docs/
                logo_large_light.svg?raw=true#gh-light-mode-only]
+ [https://joss.theoj.org/papers/0c2a2cd2ca10b5c0bdca4d0234eb94fd/status.svg]
 [https://img.shields.io/badge/style-wemake-000000.svg] [https://img.shields.io/
   pypi/v/msmhelper] [https://img.shields.io/conda/vn/conda-forge/msmhelper]
   [https://pepy.tech/badge/msmhelper] [https://img.shields.io/github/actions/
  workflow/status/moldyn/msmhelper/pytest.yml?branch=main] [https://codecov.io/
   gh/moldyn/msmhelper/branch/main/graph/badge.svg?token=Ce2eW5JICI] [https://
 github.com/moldyn/msmhelper/actions/workflows/codeql.yml/badge.svg?branch=main]
   [https://img.shields.io/pypi/pyversions/msmhelper] [https://img.shields.io/
@@ -37,30 +38,31 @@
 published soon: > D. Nagel, and G. Stock, > *msmhelper: A Python Package for
 Markov State Modeling of Protein Dynamics*, > in preparation We kindly ask you
 to cite this article in case you use this software package for published works.
 ## Features - Simple usage with sleek function-based API - High performance due
 to [numba](https://numba.pydata.org/)-optimized source code, checkout the
 [benchmark comparing to PyEMMA](https://moldyn.github.io/msmhelper/benchmark) -
 [Documentation](https://moldyn.github.io/msmhelper) including tutorials -
-Powerful command line interface (CLI) to create publication-ready figures -
-Supports Python 3.7-3.10 - Many helpful functions for dealing with state
-trajectories ## Implemented Key Functionalities - Hummer-Szabo projection of
-optimal dimensionality reduction by [Hummer and Szabo 2014](https://doi.org/
-10.1021/jp508375q) - Dynamical coring by [Nagel et al. 2019](https://doi.org/
-10.1063/1.5081767) - Fast extraction of pathways and MSM-based prediction of
-pathways based on the definition of [Nagel et al. 2020](https://pubs.acs.org/
-doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times based on
-both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov](https://
-www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test implementation -
-Entropy-based comparison of different state discretizations - Contact
-representation by Nagel et al. 2023 (submitted) for a compact structural
-representation of the states - Provide (non-reversible) transition matrix of
-all states (corresponds in pyemma to `connectivity='none', 'all'` which will
-(probably) [never be implemented](https://github.com/markovmodel/PyEMMA/blob/
-5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
+Powerful command-line interface (CLI) to create publication-ready figures -
+Supports Python 3.7-3.10 ## Implemented Key Functionalities - Hummer-Szabo
+projection of optimal dimensionality reduction by [Hummer and Szabo 2014]
+(https://doi.org/10.1021/jp508375q) - Dynamical coring by [Nagel et al. 2019]
+(https://doi.org/10.1063/1.5081767) - Fast extraction of pathways and MSM-based
+prediction of pathways based on the definition of [Nagel et al. 2020](https://
+pubs.acs.org/doi/10.1021/acs.jctc.0c00774) - Fast calculation of waiting times
+based on both, state trajectories and MSMs - Blazing fast [Chapman-Kolmogorov]
+(https://www.wikiwand.com/en/Chapman%E2%80%93Kolmogorov_equation) test
+implementation - Entropy-based similarity measure to compare different state
+discretizations, this method will be published soon in Nagel 2023 - Contact
+representation by [Nagel et al. 2023](arxiv.org/abs/2303.03814) for a compact
+structural representation of the states - Command-line interface providing
+both, visualization and analysis methods - Provide (non-reversible) transition
+matrix of all states (corresponds in pyemma to `connectivity='none', 'all'`
+which will (probably) [never be implemented](https://github.com/markovmodel/
+PyEMMA/blob/5315b8699eff2941e84577932921f694dca76f59/pyemma/msm/estimators/
 _msm_estimator_base.py#L110)) ## Getting started ### Installation The package
 is called `msmhelper` and is available via [PyPI](https://pypi.org/project/
 msmhelper) or [conda](https://anaconda.org/conda-forge/msmhelper). To install
 it, simply call: ```bash python3 -m pip install --upgrade msmhelper ``` or ```
 conda install -c conda-forge msmhelper ``` or for the latest dev version
 ```bash # via ssh key python3 -m pip install git+ssh://git@github.com/moldyn/
 msmhelper.git # or via password-based login python3 -m pip install git+https://
@@ -71,44 +73,45 @@
 `~/.bashrc` ```bash eval "$(_MSMHELPER_COMPLETE=bash_source msmhelper)" ``` In
 general one can call the module directly by its entry point `$ msmhelper` or by
 calling the module `$ python -m msmhelper`. The latter method is preferred to
 ensure using the desired python environment. For enabling the shell completion,
 the entry point needs to be used. ## Usage This package offers either a
 [command line interface](https://moldyn.github.io/msmhelper/reference/cli) to
 run standalone analysis and to create commonly-used figures, or its much more
-powerful [API](https://moldyn.github.io/msmhelper/reference/msmhelper) can be
+powerful [API](https://moldyn.github.io/msmhelper/tutorials/msmhelper) can be
 used to embedded it into an existing Python workflow. Check out the
 documentation for an overview over all modules and some example workflows, and
-for some examples see the (following section)[#Hummer-Szabo-Projection].
+for some examples see the [following section](#hummer-szabo-projection).
 ```python import msmhelper as mh # open text files traj = mh.openmicrostates
 (filename, limitsfile) # create markov state model tmat, states =
 mh.estimate_markov_model(traj, lagtime=1) ... ``` ## Hummer-Szabo Projection In
 the following we show some sample figures produced directly with the command
-line tools. For more information on that, there is a [tutorial](tutorials/
-hummerszabo) explaining the methods more in depth. In general we can see, that
-applying the HS-projection removes most projection artifacts based on coarse-
-graining many microstates into a few macrostates. | Method | MSM | Hummer-Szabo
-MSM | | :---: | :---: | :---: | | Implied Timescales | [![Implied Timescales]
-(https://moldyn.github.io/msmhelper/assets/8state_macrotraj.impl.jpg)]
-(reference/cli/#msmhelper-implied-timescales) | [![Implied Timescales](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.impl.jpg)](reference/cli/
-#msmhelper-implied-timescales) | | Chapman-Kolmogorov test | [![Chapman-
-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/
-8state_macrotraj.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | [!
-[Chapman-Kolmogorov Test](https://moldyn.github.io/msmhelper/assets/
-8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/#msmhelper-ck-test) | |
-Waiting Time Distributions | [![waiting time distribution](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.wtd.jpg)](reference/cli/
-#msmhelper-waiting-time-dist) | [![waiting time distribution](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wtd.jpg)](reference/cli/
-#msmhelper-waiting-time-dist) | | Waiting Times | [![waiting times](https://
-moldyn.github.io/msmhelper/assets/8state_macrotraj.wts.jpg)](reference/cli/
-#msmhelper-waiting-times) | [![waiting times](https://moldyn.github.io/
-msmhelper/assets/8state_macrotraj.sh.wts.jpg)](reference/cli/#msmhelper-
-waiting-times) | | Contact Representation | [![contact representation](https://
-moldyn.github.io/msmhelper/assets/hp35.contactRep.state1-12.jpg)](reference/
-cli/#msmhelper-contact-rep) | | For more examples checkout the [tutorials]
-(https://moldyn.github.io/msmhelper/tutorials). ## Roadmap - Add [Buchete-
-Hummer test](https://doi.org/10.1021/jp0761665) as alternative for the Chapman-
-Kolmogorov test. - Add a numba implementation of a parallelized autocorrelation
-function estimation. - Use static type hints together with [beartype](https://
-github.com/beartype/beartype)
+line tools. For more information on that, there is a [tutorial](https://
+moldyn.github.io/msmhelper/tutorials/hummerszabo) explaining the methods more
+in depth. In general we can see, that applying the HS-projection removes most
+projection artifacts based on coarse-graining many microstates into a few
+macrostates. | Method | MSM | Hummer-Szabo MSM | | :---: | :---: | :---: | |
+Implied Timescales | [![Implied Timescales](https://moldyn.github.io/msmhelper/
+assets/8state_macrotraj.impl.jpg)](reference/cli/#msmhelper-implied-timescales)
+| [![Implied Timescales](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.sh.impl.jpg)](reference/cli/#msmhelper-implied-timescales) | |
+Chapman-Kolmogorov test | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
+msmhelper/assets/8state_macrotraj.cktest.state1-4.jpg)](reference/cli/
+#msmhelper-ck-test) | [![Chapman-Kolmogorov Test](https://moldyn.github.io/
+msmhelper/assets/8state_macrotraj.sh.cktest.state1-4.jpg)](reference/cli/
+#msmhelper-ck-test) | | Waiting Time Distributions | [![waiting time
+distribution](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | [!
+[waiting time distribution](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.sh.wtd.jpg)](reference/cli/#msmhelper-waiting-time-dist) | |
+Waiting Times | [![waiting times](https://moldyn.github.io/msmhelper/assets/
+8state_macrotraj.wts.jpg)](reference/cli/#msmhelper-waiting-times) | [![waiting
+times](https://moldyn.github.io/msmhelper/assets/8state_macrotraj.sh.wts.jpg)]
+(reference/cli/#msmhelper-waiting-times) | | Contact Representation | [!
+[contact representation](https://moldyn.github.io/msmhelper/assets/
+hp35.contactRep.state1-12.jpg)](reference/cli/#msmhelper-contact-rep) | | For
+more examples checkout the [tutorials](https://moldyn.github.io/msmhelper/
+tutorials). ## Roadmap - Add [Buchete-Hummer test](https://doi.org/10.1021/
+jp0761665) as alternative for the Chapman-Kolmogorov test. - Add a numba
+implementation of a parallelized autocorrelation function estimation. - Use
+static type hints together with [beartype](https://github.com/beartype/
+beartype)
```

### Comparing `msmhelper-1.0.2/src/msmhelper.egg-info/SOURCES.txt` & `msmhelper-1.0.3/src/msmhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/src/msmhelper.egg-info/requires.txt` & `msmhelper-1.0.3/src/msmhelper.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 pandas
 decorit
 scipy
 click
 prettypyplot
 
 [all]
-mkdocs-section-index
 pytest-rerunfailures
-pytest-mpl
-jupyter_contrib_nbextensions
-pyemma
-pytest-cov
-flake8
+mkdocs-literate-nav
 mkdocs-material
+mkdocs-jupyter
+pyemma
+jupyter_contrib_nbextensions
+pytest-mpl
 mkdocstrings-python
-mkdocs-literate-nav
-pytest
-mkdocs-gen-files
 mkdocstrings
+pytest
 mkdocs-click
-mkdocs-jupyter
+mkdocs-gen-files
+flake8
+pytest-cov
+mkdocs-section-index
 
 [docs]
-mkdocs-section-index
-jupyter_contrib_nbextensions
-pyemma
+mkdocs-literate-nav
 mkdocs-material
+mkdocs-jupyter
+pyemma
+jupyter_contrib_nbextensions
 mkdocstrings-python
-mkdocs-literate-nav
-mkdocs-gen-files
 mkdocstrings
 mkdocs-click
-mkdocs-jupyter
+mkdocs-gen-files
+mkdocs-section-index
 
 [testing]
 pytest-rerunfailures
 pytest-mpl
-pytest-cov
-flake8
 pytest
+flake8
+pytest-cov
```

### Comparing `msmhelper-1.0.2/test/test___main__.py` & `msmhelper-1.0.3/test/test___main__.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_io.py` & `msmhelper-1.0.3/test/test_io.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_md_comparison.py` & `msmhelper-1.0.3/test/test_md_comparison.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_md_corrections.py` & `msmhelper-1.0.3/test/test_md_corrections.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_md_timescales.py` & `msmhelper-1.0.3/test/test_md_timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_msm_msm.py` & `msmhelper-1.0.3/test/test_msm_msm.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_msm_tests.py` & `msmhelper-1.0.3/test/test_msm_tests.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_msm_timescales.py` & `msmhelper-1.0.3/test/test_msm_timescales.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_msm_utils_linalg.py` & `msmhelper-1.0.3/test/test_msm_utils_linalg.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_plot.py` & `msmhelper-1.0.3/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_statetraj.py` & `msmhelper-1.0.3/test/test_statetraj.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,23 @@
     return np.array(
         [1, 1, 1, 2, 2, 2, 2, 2, 2, 2, 2, 2, 1, 2, 2, 2, 2, 2],
         dtype=np.int32,
     )
 
 
 @pytest.fixture
+def macro_indextraj():
+    """Define state trajectory."""
+    return np.array(
+        [0, 0, 0, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 1, 1, 1, 1],
+        dtype=np.int32,
+    )
+
+
+@pytest.fixture
 def macro_traj():
     """Define index trajectory."""
     traj = np.array(
         [1, 1, 1, 2, 2, 2, 3, 3, 3, 2, 2, 2, 1, 3, 2, 3, 3, 3],
         dtype=np.int32,
     )
     macrotraj = np.array(
@@ -143,14 +152,26 @@
 
     with pytest.raises(AttributeError):
         state_traj.trajs = 5
     with pytest.raises(AttributeError):
         state_traj.index_trajs = 5
 
 
+def test_macroindex_trajs(macro_traj, indextraj, macro_indextraj):
+    """Test index trajs property."""
+    np.testing.assert_array_equal(
+        macro_traj.index_trajs_flatten,
+        macro_indextraj,
+    )
+    np.testing.assert_array_equal(
+        macro_traj.microstate_index_trajs_flatten,
+        indextraj,
+    )
+
+
 def test_trajs_flatten(state_traj, index_traj):
     """Test flatten index trajectory."""
     np.testing.assert_array_equal(
         index_traj.trajs[0],
         index_traj.trajs_flatten,
     )
     np.testing.assert_array_equal(
```

### Comparing `msmhelper-1.0.2/test/test_utils__utils.py` & `msmhelper-1.0.3/test/test_utils__utils.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_utils_filtering.py` & `msmhelper-1.0.3/test/test_utils_filtering.py`

 * *Files identical despite different names*

### Comparing `msmhelper-1.0.2/test/test_utils_tests.py` & `msmhelper-1.0.3/test/test_utils_tests.py`

 * *Files identical despite different names*

