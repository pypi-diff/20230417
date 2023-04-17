# Comparing `tmp/ranx-0.3.6.tar.gz` & `tmp/ranx-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ranx-0.3.6.tar", last modified: Tue Feb 21 13:46:03 2023, max compression
+gzip compressed data, was "ranx-0.3.7.tar", last modified: Mon Apr 17 09:43:02 2023, max compression
```

## Comparing `ranx-0.3.6.tar` & `ranx-0.3.7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.438869 ranx-0.3.6/
--rw-r--r--   0 elias      (501) staff       (20)     1070 2022-12-02 22:30:34.000000 ranx-0.3.6/LICENSE
--rw-r--r--   0 elias      (501) staff       (20)    15899 2023-02-21 13:46:03.438217 ranx-0.3.6/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)    15225 2023-02-13 16:41:37.000000 ranx-0.3.6/README.md
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.364829 ranx-0.3.6/ranx/
--rw-r--r--   0 elias      (501) staff       (20)      232 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/__init__.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.374857 ranx-0.3.6/ranx/data_structures/
--rw-r--r--   0 elias      (501) staff       (20)      509 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/data_structures/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     3241 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/data_structures/common.py
--rw-r--r--   0 elias      (501) staff       (20)      524 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/data_structures/frozenset_dict.py
--rw-r--r--   0 elias      (501) staff       (20)      639 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/data_structures/generic.py
--rw-r--r--   0 elias      (501) staff       (20)     3312 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/data_structures/optimization_report.py
--rw-r--r--   0 elias      (501) staff       (20)    11093 2023-01-26 20:56:50.000000 ranx-0.3.6/ranx/data_structures/qrels.py
--rw-r--r--   0 elias      (501) staff       (20)    11274 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/data_structures/report.py
--rw-r--r--   0 elias      (501) staff       (20)    10708 2023-02-21 13:42:11.000000 ranx-0.3.6/ranx/data_structures/run.py
--rw-r--r--   0 elias      (501) staff       (20)     2056 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/downloader.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.395447 ranx-0.3.6/ranx/fusion/
--rw-r--r--   0 elias      (501) staff       (20)     2821 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     4744 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/bayesfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     3243 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/bordafuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/comb_anz.py
--rw-r--r--   0 elias      (501) staff       (20)     2148 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/comb_gmnz.py
--rw-r--r--   0 elias      (501) staff       (20)     2138 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/comb_max.py
--rw-r--r--   0 elias      (501) staff       (20)     2212 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/comb_med.py
--rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/comb_min.py
--rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/comb_mnz.py
--rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/comb_sum.py
--rw-r--r--   0 elias      (501) staff       (20)     1703 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/common.py
--rw-r--r--   0 elias      (501) staff       (20)     4732 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/condorcet.py
--rw-r--r--   0 elias      (501) staff       (20)     2391 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/isr.py
--rw-r--r--   0 elias      (501) staff       (20)     2691 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/log_isr.py
--rw-r--r--   0 elias      (501) staff       (20)     2949 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/logn_isr.py
--rw-r--r--   0 elias      (501) staff       (20)     3018 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/mapfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2780 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/mixed.py
--rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/posfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     4446 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/probfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2632 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/rbc.py
--rw-r--r--   0 elias      (501) staff       (20)     2073 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/rrf.py
--rw-r--r--   0 elias      (501) staff       (20)     4044 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/segfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     3083 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/slidefuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1912 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/weighted_bordafuse.py
--rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/weighted_condorcet.py
--rw-r--r--   0 elias      (501) staff       (20)     2903 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/wmnz.py
--rw-r--r--   0 elias      (501) staff       (20)     1895 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion/wsum.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.409519 ranx-0.3.6/ranx/fusion_optimization/
--rw-r--r--   0 elias      (501) staff       (20)     2568 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)      240 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_bayesfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1183 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_comb_gmnz.py
--rw-r--r--   0 elias      (501) staff       (20)     1179 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_logn_isr.py
--rw-r--r--   0 elias      (501) staff       (20)      233 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_mapfuse.py
--rw-r--r--   0 elias      (501) staff       (20)      623 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_mixed.py
--rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_posfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1137 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_probfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1126 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_rbc.py
--rw-r--r--   0 elias      (501) staff       (20)      961 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_rrf.py
--rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_segfuse.py
--rw-r--r--   0 elias      (501) staff       (20)     1062 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_slidefuse.py
--rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_weighted_bordafuse.py
--rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_weighted_condorcet.py
--rw-r--r--   0 elias      (501) staff       (20)     1408 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_weights.py
--rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_wmnz.py
--rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/fusion_optimization/optimize_wsum.py
--rw-r--r--   0 elias      (501) staff       (20)     1661 2023-02-21 13:26:31.000000 ranx-0.3.6/ranx/io.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.414210 ranx-0.3.6/ranx/meta/
--rw-r--r--   0 elias      (501) staff       (20)      259 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/meta/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     4817 2023-02-03 09:44:46.000000 ranx-0.3.6/ranx/meta/compare.py
--rw-r--r--   0 elias      (501) staff       (20)     4862 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/meta/evaluate.py
--rw-r--r--   0 elias      (501) staff       (20)     1134 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/meta/fuse.py
--rw-r--r--   0 elias      (501) staff       (20)      158 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/meta/normalize.py
--rw-r--r--   0 elias      (501) staff       (20)     2469 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/meta/optimize_fusion.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.426149 ranx-0.3.6/ranx/metrics/
--rw-r--r--   0 elias      (501) staff       (20)     1564 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     2917 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/average_precision.py
--rw-r--r--   0 elias      (501) staff       (20)     2403 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/bpref.py
--rw-r--r--   0 elias      (501) staff       (20)      305 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/common.py
--rw-r--r--   0 elias      (501) staff       (20)     2509 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/f1.py
--rw-r--r--   0 elias      (501) staff       (20)     2433 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/get_hit_lists.py
--rw-r--r--   0 elias      (501) staff       (20)     2095 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/get_non_rel_lists.py
--rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/get_unjudged_lists.py
--rw-r--r--   0 elias      (501) staff       (20)     2313 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/hit_rate.py
--rw-r--r--   0 elias      (501) staff       (20)     2188 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/hits.py
--rw-r--r--   0 elias      (501) staff       (20)     6493 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/ndcg.py
--rw-r--r--   0 elias      (501) staff       (20)     2237 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/precision.py
--rw-r--r--   0 elias      (501) staff       (20)     1979 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/r_precision.py
--rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/rank_biased_precision.py
--rw-r--r--   0 elias      (501) staff       (20)     2405 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/recall.py
--rw-r--r--   0 elias      (501) staff       (20)     2225 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/metrics/reciprocal_rank.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.434348 ranx-0.3.6/ranx/normalization/
--rw-r--r--   0 elias      (501) staff       (20)      776 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     2057 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/borda_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1076 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/common.py
--rw-r--r--   0 elias      (501) staff       (20)     1426 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/max_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1701 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/min_max_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1322 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/rank_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1547 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/sum_norm.py
--rw-r--r--   0 elias      (501) staff       (20)     1511 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/normalization/zmuv_norm.py
--rw-r--r--   0 elias      (501) staff       (20)      412 2023-02-21 13:43:14.000000 ranx-0.3.6/ranx/ranxhub.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.437055 ranx-0.3.6/ranx/statistical_tests/
--rw-r--r--   0 elias      (501) staff       (20)     3441 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/statistical_tests/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     1368 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/statistical_tests/fisher_randomization_test.py
--rw-r--r--   0 elias      (501) staff       (20)      550 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/statistical_tests/paired_student_t_test.py
--rw-r--r--   0 elias      (501) staff       (20)      711 2023-02-13 16:35:22.000000 ranx-0.3.6/ranx/statistical_tests/tukey_hsd_test.py
--rw-r--r--   0 elias      (501) staff       (20)     1782 2022-12-02 22:30:35.000000 ranx-0.3.6/ranx/utils.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-21 13:46:03.368384 ranx-0.3.6/ranx.egg-info/
--rw-r--r--   0 elias      (501) staff       (20)    15899 2023-02-21 13:46:03.000000 ranx-0.3.6/ranx.egg-info/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)     2923 2023-02-21 13:46:03.000000 ranx-0.3.6/ranx.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (501) staff       (20)        1 2023-02-21 13:46:03.000000 ranx-0.3.6/ranx.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (501) staff       (20)       88 2023-02-21 13:46:03.000000 ranx-0.3.6/ranx.egg-info/requires.txt
--rw-r--r--   0 elias      (501) staff       (20)        5 2023-02-21 13:46:03.000000 ranx-0.3.6/ranx.egg-info/top_level.txt
--rw-r--r--   0 elias      (501) staff       (20)       38 2023-02-21 13:46:03.439097 ranx-0.3.6/setup.cfg
--rw-r--r--   0 elias      (501) staff       (20)     1227 2023-02-21 13:44:45.000000 ranx-0.3.6/setup.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.709992 ranx-0.3.7/
+-rw-r--r--   0 elias      (501) staff       (20)     1070 2022-12-02 22:30:34.000000 ranx-0.3.7/LICENSE
+-rw-r--r--   0 elias      (501) staff       (20)    15899 2023-04-17 09:43:02.709367 ranx-0.3.7/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)    15225 2023-02-13 16:41:37.000000 ranx-0.3.7/README.md
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.644794 ranx-0.3.7/ranx/
+-rw-r--r--   0 elias      (501) staff       (20)      232 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/__init__.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.653281 ranx-0.3.7/ranx/data_structures/
+-rw-r--r--   0 elias      (501) staff       (20)      509 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     3241 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/common.py
+-rw-r--r--   0 elias      (501) staff       (20)      524 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/frozenset_dict.py
+-rw-r--r--   0 elias      (501) staff       (20)      639 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/generic.py
+-rw-r--r--   0 elias      (501) staff       (20)     3312 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/optimization_report.py
+-rw-r--r--   0 elias      (501) staff       (20)    11093 2023-01-26 20:56:50.000000 ranx-0.3.7/ranx/data_structures/qrels.py
+-rw-r--r--   0 elias      (501) staff       (20)    11274 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/data_structures/report.py
+-rw-r--r--   0 elias      (501) staff       (20)    11288 2023-04-17 09:21:00.000000 ranx-0.3.7/ranx/data_structures/run.py
+-rw-r--r--   0 elias      (501) staff       (20)     2056 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/downloader.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.671092 ranx-0.3.7/ranx/fusion/
+-rw-r--r--   0 elias      (501) staff       (20)     2821 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     4744 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/bayesfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     3243 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/bordafuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_anz.py
+-rw-r--r--   0 elias      (501) staff       (20)     2148 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_gmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     2138 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_max.py
+-rw-r--r--   0 elias      (501) staff       (20)     2212 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_med.py
+-rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_min.py
+-rw-r--r--   0 elias      (501) staff       (20)     2226 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_mnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     2137 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/comb_sum.py
+-rw-r--r--   0 elias      (501) staff       (20)     1703 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/common.py
+-rw-r--r--   0 elias      (501) staff       (20)     4732 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/condorcet.py
+-rw-r--r--   0 elias      (501) staff       (20)     2391 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/isr.py
+-rw-r--r--   0 elias      (501) staff       (20)     2691 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/log_isr.py
+-rw-r--r--   0 elias      (501) staff       (20)     2949 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/logn_isr.py
+-rw-r--r--   0 elias      (501) staff       (20)     3018 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/mapfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2780 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/mixed.py
+-rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/posfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     4446 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/probfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2632 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/rbc.py
+-rw-r--r--   0 elias      (501) staff       (20)     2073 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/rrf.py
+-rw-r--r--   0 elias      (501) staff       (20)     4044 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/segfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     3083 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/slidefuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1912 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/weighted_bordafuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     2933 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/weighted_condorcet.py
+-rw-r--r--   0 elias      (501) staff       (20)     2903 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/wmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     1895 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion/wsum.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.683397 ranx-0.3.7/ranx/fusion_optimization/
+-rw-r--r--   0 elias      (501) staff       (20)     2568 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)      240 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_bayesfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1183 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_comb_gmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)     1179 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_logn_isr.py
+-rw-r--r--   0 elias      (501) staff       (20)      233 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_mapfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      623 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_mixed.py
+-rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_posfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1137 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_probfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1126 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_rbc.py
+-rw-r--r--   0 elias      (501) staff       (20)      961 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_rrf.py
+-rw-r--r--   0 elias      (501) staff       (20)      228 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_segfuse.py
+-rw-r--r--   0 elias      (501) staff       (20)     1062 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_slidefuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_bordafuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      675 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_condorcet.py
+-rw-r--r--   0 elias      (501) staff       (20)     1408 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_weights.py
+-rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_wmnz.py
+-rw-r--r--   0 elias      (501) staff       (20)      619 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/fusion_optimization/optimize_wsum.py
+-rw-r--r--   0 elias      (501) staff       (20)     1661 2023-02-21 13:26:31.000000 ranx-0.3.7/ranx/io.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.687834 ranx-0.3.7/ranx/meta/
+-rw-r--r--   0 elias      (501) staff       (20)      259 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     5017 2023-04-17 09:30:20.000000 ranx-0.3.7/ranx/meta/compare.py
+-rw-r--r--   0 elias      (501) staff       (20)     5312 2023-04-17 09:32:51.000000 ranx-0.3.7/ranx/meta/evaluate.py
+-rw-r--r--   0 elias      (501) staff       (20)     1134 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/fuse.py
+-rw-r--r--   0 elias      (501) staff       (20)      158 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/normalize.py
+-rw-r--r--   0 elias      (501) staff       (20)     2469 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/meta/optimize_fusion.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.699972 ranx-0.3.7/ranx/metrics/
+-rw-r--r--   0 elias      (501) staff       (20)     1564 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     2917 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/average_precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     2403 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/bpref.py
+-rw-r--r--   0 elias      (501) staff       (20)      305 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/common.py
+-rw-r--r--   0 elias      (501) staff       (20)     2509 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/f1.py
+-rw-r--r--   0 elias      (501) staff       (20)     2433 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/get_hit_lists.py
+-rw-r--r--   0 elias      (501) staff       (20)     2095 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/get_non_rel_lists.py
+-rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/get_unjudged_lists.py
+-rw-r--r--   0 elias      (501) staff       (20)     2313 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/hit_rate.py
+-rw-r--r--   0 elias      (501) staff       (20)     2188 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/hits.py
+-rw-r--r--   0 elias      (501) staff       (20)     6493 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/ndcg.py
+-rw-r--r--   0 elias      (501) staff       (20)     2237 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     1979 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/r_precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     1986 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/rank_biased_precision.py
+-rw-r--r--   0 elias      (501) staff       (20)     2405 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/recall.py
+-rw-r--r--   0 elias      (501) staff       (20)     2225 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/metrics/reciprocal_rank.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.705662 ranx-0.3.7/ranx/normalization/
+-rw-r--r--   0 elias      (501) staff       (20)      776 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     2057 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/borda_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1076 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/common.py
+-rw-r--r--   0 elias      (501) staff       (20)     1426 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/max_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1701 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/min_max_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1322 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/rank_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1547 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/sum_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)     1511 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/normalization/zmuv_norm.py
+-rw-r--r--   0 elias      (501) staff       (20)      412 2023-02-21 13:43:14.000000 ranx-0.3.7/ranx/ranxhub.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.708460 ranx-0.3.7/ranx/statistical_tests/
+-rw-r--r--   0 elias      (501) staff       (20)     3441 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/statistical_tests/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     1368 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/statistical_tests/fisher_randomization_test.py
+-rw-r--r--   0 elias      (501) staff       (20)      550 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/statistical_tests/paired_student_t_test.py
+-rw-r--r--   0 elias      (501) staff       (20)      711 2023-02-13 16:35:22.000000 ranx-0.3.7/ranx/statistical_tests/tukey_hsd_test.py
+-rw-r--r--   0 elias      (501) staff       (20)     1782 2022-12-02 22:30:35.000000 ranx-0.3.7/ranx/utils.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-17 09:43:02.648401 ranx-0.3.7/ranx.egg-info/
+-rw-r--r--   0 elias      (501) staff       (20)    15899 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)     2923 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (501) staff       (20)        1 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (501) staff       (20)       88 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/requires.txt
+-rw-r--r--   0 elias      (501) staff       (20)        5 2023-04-17 09:43:02.000000 ranx-0.3.7/ranx.egg-info/top_level.txt
+-rw-r--r--   0 elias      (501) staff       (20)       38 2023-04-17 09:43:02.710160 ranx-0.3.7/setup.cfg
+-rw-r--r--   0 elias      (501) staff       (20)     1227 2023-04-17 09:42:16.000000 ranx-0.3.7/setup.py
```

### Comparing `ranx-0.3.6/LICENSE` & `ranx-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/PKG-INFO` & `ranx-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranx
-Version: 0.3.6
+Version: 0.3.7
 Summary: ranx: A Blazing-Fast Python Library for Ranking Evaluation, Comparison, and Fusion
 Home-page: https://github.com/AmenRa/ranx
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: trec_eval,information retrieval,recommender systems,evaluation,ranking,fusion,metasearch,numba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ranx Version: 0.3.6 Summary: ranx: A Blazing-Fast
+Metadata-Version: 2.1 Name: ranx Version: 0.3.7 Summary: ranx: A Blazing-Fast
 Python Library for Ranking Evaluation, Comparison, and Fusion Home-page: https:
 //github.com/AmenRa/ranx Author: Elias Bassani Author-email:
 elias.bssn@gmail.com Keywords: trec_eval,information retrieval,recommender
 systems,evaluation,ranking,fusion,metasearch,numba Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing :: General Requires-
```

### Comparing `ranx-0.3.6/README.md` & `ranx-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/data_structures/common.py` & `ranx-0.3.7/ranx/data_structures/common.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/data_structures/frozenset_dict.py` & `ranx-0.3.7/ranx/data_structures/frozenset_dict.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/data_structures/generic.py` & `ranx-0.3.7/ranx/data_structures/generic.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/data_structures/optimization_report.py` & `ranx-0.3.7/ranx/data_structures/optimization_report.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/data_structures/qrels.py` & `ranx-0.3.7/ranx/data_structures/qrels.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/data_structures/report.py` & `ranx-0.3.7/ranx/data_structures/report.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/data_structures/run.py` & `ranx-0.3.7/ranx/data_structures/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from .common import (
     add_and_sort,
     create_and_sort,
     sort_dict_by_key,
     sort_dict_of_dict_by_value,
     to_typed_list,
 )
+from .generic import create_empty_results_dict
+from .qrels import Qrels
 
 
 class Run(object):
     """`Run` stores the relevance scores estimated by the model under evaluation.<\br>
     The preferred way for creating a `Run` istance is converting a Python dictionary as follows:
 
     ```python
@@ -133,14 +135,28 @@
     # Sort in place
     def sort(self):
         """Sort. Used internally."""
         self.run = sort_dict_by_key(self.run)
         self.run = sort_dict_of_dict_by_value(self.run)
         self.sorted = True
 
+    def make_comparable(self, qrels: Qrels):
+        """Adds empty results for queries missing from the run and removes those not appearing in qrels."""
+        # Adds empty results for missing queries
+        for q_id in qrels.qrels:
+            if q_id not in self.run:
+                self.run[q_id] = create_empty_results_dict()
+
+        # Remove results for additional queries
+        for q_id in self.run:
+            if q_id not in qrels.qrels:
+                del self.run[q_id]
+
+        return self
+
     def to_typed_list(self):
         """Convert Run to Numba Typed List. Used internally."""
         if self.sorted == False:
             self.sort()
         return to_typed_list(self.run)
 
     def to_dict(self):
@@ -228,15 +244,14 @@
 
         Returns:
             Run: ranx.Run
         """
         # Infer file extension -------------------------------------------------
         kind = get_file_kind(path, kind)
 
-
         # Load Run -------------------------------------------------------------
         if kind == "json":
             run = load_json(path)
         elif kind == "lz4":
             run = load_lz4(path)
         else:
             run = defaultdict(dict)
```

### Comparing `ranx-0.3.6/ranx/downloader.py` & `ranx-0.3.7/ranx/downloader.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/__init__.py` & `ranx-0.3.7/ranx/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/bayesfuse.py` & `ranx-0.3.7/ranx/fusion/bayesfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/bordafuse.py` & `ranx-0.3.7/ranx/fusion/bordafuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/comb_anz.py` & `ranx-0.3.7/ranx/fusion/comb_anz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/comb_gmnz.py` & `ranx-0.3.7/ranx/fusion/comb_gmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/comb_max.py` & `ranx-0.3.7/ranx/fusion/comb_max.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/comb_med.py` & `ranx-0.3.7/ranx/fusion/comb_med.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/comb_min.py` & `ranx-0.3.7/ranx/fusion/comb_min.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/comb_mnz.py` & `ranx-0.3.7/ranx/fusion/comb_mnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/comb_sum.py` & `ranx-0.3.7/ranx/fusion/comb_sum.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/common.py` & `ranx-0.3.7/ranx/fusion/common.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/condorcet.py` & `ranx-0.3.7/ranx/fusion/condorcet.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/isr.py` & `ranx-0.3.7/ranx/fusion/isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/log_isr.py` & `ranx-0.3.7/ranx/fusion/log_isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/logn_isr.py` & `ranx-0.3.7/ranx/fusion/logn_isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/mapfuse.py` & `ranx-0.3.7/ranx/fusion/mapfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/mixed.py` & `ranx-0.3.7/ranx/fusion/mixed.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/posfuse.py` & `ranx-0.3.7/ranx/fusion/posfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/probfuse.py` & `ranx-0.3.7/ranx/fusion/probfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/rbc.py` & `ranx-0.3.7/ranx/fusion/rbc.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/rrf.py` & `ranx-0.3.7/ranx/fusion/rrf.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/segfuse.py` & `ranx-0.3.7/ranx/fusion/segfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/slidefuse.py` & `ranx-0.3.7/ranx/fusion/slidefuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/weighted_bordafuse.py` & `ranx-0.3.7/ranx/fusion/weighted_bordafuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/weighted_condorcet.py` & `ranx-0.3.7/ranx/fusion/weighted_condorcet.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/wmnz.py` & `ranx-0.3.7/ranx/fusion/wmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion/wsum.py` & `ranx-0.3.7/ranx/fusion/wsum.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/__init__.py` & `ranx-0.3.7/ranx/fusion_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_comb_gmnz.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_comb_gmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_logn_isr.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_logn_isr.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_mixed.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_mixed.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_probfuse.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_probfuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_rbc.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_rbc.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_rrf.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_rrf.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_slidefuse.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_slidefuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_weighted_bordafuse.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_bordafuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_weighted_condorcet.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_weighted_condorcet.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_weights.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_weights.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_wmnz.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_wmnz.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/fusion_optimization/optimize_wsum.py` & `ranx-0.3.7/ranx/fusion_optimization/optimize_wsum.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/io.py` & `ranx-0.3.7/ranx/io.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/meta/compare.py` & `ranx-0.3.7/ranx/meta/compare.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     stat_test: str = "student",
     n_permutations: int = 1000,
     max_p: float = 0.01,
     random_seed: int = 42,
     threads: int = 0,
     rounding_digits: int = 3,
     show_percentages: bool = False,
+    make_comparable: bool = False,
 ) -> Report:
     """Evaluate multiple `runs` and compute statistical tests.
 
     Usage example:
     ```python
     from ranx import compare
 
@@ -54,38 +55,39 @@
         n_permutations (int, optional): Number of permutation to perform during statistical testing (Fisher's Randomization Test is used by default). Defaults to 1000.
         max_p (float, optional): Maximum p-value to consider an increment as statistically significant. Defaults to 0.01.
         stat_test (str, optional): Statistical test to perform. Use "fisher" for _Fisher's Randomization Test_, "student" for _Two-sided Paired Student's t-Test_, or "Tukey" for _Tukey's HSD test_. Defaults to "student".
         random_seed (int, optional): Random seed to use for generating the permutations. Defaults to 42.
         threads (int, optional): Number of threads to use, zero means all the available threads. Defaults to 0.
         rounding_digits (int, optional): Number of digits to round to and to show in the Report. Defaults to 3.
         show_percentages (bool, optional): Whether to show percentages instead of floats in the Report. Defaults to False.
+        make_comparable (bool, optional): Adds empty results for queries missing from the runs and removes those not appearing in qrels. Defaults to False.
 
     Returns:
         Report: See report.
     """
     metrics = format_metrics(metrics)
     assert all(type(m) == str for m in metrics), "Metrics error"
 
     model_names = []
     results = defaultdict(dict)
-    # comparisons = FrozensetDict()
 
     metric_scores = {}
 
     # Compute scores for each run for each query -------------------------------
     for i, run in enumerate(runs):
         model_name = run.name if run.name is not None else f"run_{i+1}"
         model_names.append(model_name)
 
         metric_scores[model_name] = evaluate(
             qrels=qrels,
             run=run,
             metrics=metrics,
             return_mean=False,
             threads=threads,
+            make_comparable=make_comparable,
         )
 
         if len(metrics) == 1:
             metric_scores[model_name] = {metrics[0]: metric_scores[model_name]}
 
         for m in metrics:
             results[model_name][m] = float(
```

### Comparing `ranx-0.3.6/ranx/meta/evaluate.py` & `ranx-0.3.7/ranx/meta/evaluate.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,15 +56,17 @@
         return run.to_typed_list()
     elif type(run) == dict:
         return python_dict_to_typed_list(run, sort=True)
     return run
 
 
 def check_keys(qrels, run):
-    assert qrels.keys() == run.keys(), "Qrels and Run query ids do not match"
+    assert (
+        qrels.keys() == run.keys()
+    ), "Qrels and Run query ids do not match. Pass `make_comparable=True` to add empty results for queries missing from the run and remove those not appearing in qrels."
 
 
 def evaluate(
     qrels: Union[
         Qrels,
         Dict[str, Dict[str, Number]],
         nb.typed.typedlist.List,
@@ -75,15 +77,16 @@
         Dict[str, Dict[str, Number]],
         nb.typed.typedlist.List,
         np.ndarray,
     ],
     metrics: Union[List[str], str],
     return_mean: bool = True,
     threads: int = 0,
-    save_results_in_run=True,
+    save_results_in_run: bool = True,
+    make_comparable: bool = False,
 ) -> Union[Dict[str, float], float]:
     """Compute the performance scores for the provided `qrels` and `run` for all the specified metrics.
 
     Usage examples:
 
     ```python
     from ranx import evaluate
@@ -110,24 +113,28 @@
     Args:
         qrels (Union[ Qrels, Dict[str, Dict[str, Number]], nb.typed.typedlist.List, np.ndarray, ]): Qrels.
         run (Union[ Run, Dict[str, Dict[str, Number]], nb.typed.typedlist.List, np.ndarray, ]): Run.
         metrics (Union[List[str], str]): Metrics or list of metric to compute.
         return_mean (bool, optional): Wether to return the metric scores averaged over the query set or the scores for individual queries. Defaults to True.
         threads (int, optional): Number of threads to use, zero means all the available threads. Defaults to 0.
         save_results_in_run (bool, optional): Save metric scores for each query in the input `run`. Defaults to True.
+        make_comparable (bool, optional): Adds empty results for queries missing from the run and removes those not appearing in qrels. Defaults to False.
 
     Returns:
         Union[Dict[str, float], float]: Results.
     """
 
     if len(qrels) < 10:
         set_num_threads(1)
     elif threads != 0:
         set_num_threads(threads)
 
+    if make_comparable and type(qrels) == Qrels and type(run) == Run:
+        run = run.make_comparable(qrels)
+
     if type(qrels) in [Qrels, dict] and type(run) in [Run, dict]:
         check_keys(qrels, run)
 
     _qrels = convert_qrels(qrels)
     _run = convert_run(run)
     metrics = format_metrics(metrics)
     assert all(type(m) == str for m in metrics), "Metrics error"
```

### Comparing `ranx-0.3.6/ranx/meta/fuse.py` & `ranx-0.3.7/ranx/meta/fuse.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/meta/optimize_fusion.py` & `ranx-0.3.7/ranx/meta/optimize_fusion.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/__init__.py` & `ranx-0.3.7/ranx/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/average_precision.py` & `ranx-0.3.7/ranx/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/bpref.py` & `ranx-0.3.7/ranx/metrics/bpref.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/f1.py` & `ranx-0.3.7/ranx/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/get_hit_lists.py` & `ranx-0.3.7/ranx/metrics/get_hit_lists.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/get_non_rel_lists.py` & `ranx-0.3.7/ranx/metrics/get_non_rel_lists.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/get_unjudged_lists.py` & `ranx-0.3.7/ranx/metrics/get_unjudged_lists.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/hit_rate.py` & `ranx-0.3.7/ranx/metrics/hit_rate.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/hits.py` & `ranx-0.3.7/ranx/metrics/hits.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/ndcg.py` & `ranx-0.3.7/ranx/metrics/ndcg.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/precision.py` & `ranx-0.3.7/ranx/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/r_precision.py` & `ranx-0.3.7/ranx/metrics/r_precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/rank_biased_precision.py` & `ranx-0.3.7/ranx/metrics/rank_biased_precision.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/recall.py` & `ranx-0.3.7/ranx/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/metrics/reciprocal_rank.py` & `ranx-0.3.7/ranx/metrics/reciprocal_rank.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/__init__.py` & `ranx-0.3.7/ranx/normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/borda_norm.py` & `ranx-0.3.7/ranx/normalization/borda_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/common.py` & `ranx-0.3.7/ranx/normalization/common.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/max_norm.py` & `ranx-0.3.7/ranx/normalization/max_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/min_max_norm.py` & `ranx-0.3.7/ranx/normalization/min_max_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/rank_norm.py` & `ranx-0.3.7/ranx/normalization/rank_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/sum_norm.py` & `ranx-0.3.7/ranx/normalization/sum_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/normalization/zmuv_norm.py` & `ranx-0.3.7/ranx/normalization/zmuv_norm.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/statistical_tests/__init__.py` & `ranx-0.3.7/ranx/statistical_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/statistical_tests/fisher_randomization_test.py` & `ranx-0.3.7/ranx/statistical_tests/fisher_randomization_test.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/statistical_tests/paired_student_t_test.py` & `ranx-0.3.7/ranx/statistical_tests/paired_student_t_test.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/statistical_tests/tukey_hsd_test.py` & `ranx-0.3.7/ranx/statistical_tests/tukey_hsd_test.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx/utils.py` & `ranx-0.3.7/ranx/utils.py`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/ranx.egg-info/PKG-INFO` & `ranx-0.3.7/ranx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranx
-Version: 0.3.6
+Version: 0.3.7
 Summary: ranx: A Blazing-Fast Python Library for Ranking Evaluation, Comparison, and Fusion
 Home-page: https://github.com/AmenRa/ranx
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: trec_eval,information retrieval,recommender systems,evaluation,ranking,fusion,metasearch,numba
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ranx Version: 0.3.6 Summary: ranx: A Blazing-Fast
+Metadata-Version: 2.1 Name: ranx Version: 0.3.7 Summary: ranx: A Blazing-Fast
 Python Library for Ranking Evaluation, Comparison, and Fusion Home-page: https:
 //github.com/AmenRa/ranx Author: Elias Bassani Author-email:
 elias.bssn@gmail.com Keywords: trec_eval,information retrieval,recommender
 systems,evaluation,ranking,fusion,metasearch,numba Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing :: General Requires-
```

### Comparing `ranx-0.3.6/ranx.egg-info/SOURCES.txt` & `ranx-0.3.7/ranx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ranx-0.3.6/setup.py` & `ranx-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ranx",
-    version="0.3.6",
+    version="0.3.7",
     author="Elias Bassani",
     author_email="elias.bssn@gmail.com",
     description="ranx: A Blazing-Fast Python Library for Ranking Evaluation, Comparison, and Fusion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AmenRa/ranx",
     packages=setuptools.find_packages(),
```

