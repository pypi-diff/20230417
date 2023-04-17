# Comparing `tmp/CamoTSS-0.1.3.tar.gz` & `tmp/CamoTSS-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CamoTSS-0.1.3.tar", last modified: Wed Mar 29 12:01:42 2023, max compression
+gzip compressed data, was "dist/CamoTSS-0.1.4.tar", last modified: Mon Apr 17 06:19:48 2023, max compression
```

## Comparing `CamoTSS-0.1.3.tar` & `CamoTSS-0.1.4.tar`

### file list

```diff
@@ -1,56 +1,69 @@
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1810 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/.gitignore
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       33 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/CamoTSS/__init__.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS/bin/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/CamoTSS/bin/__init__.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     5605 2023-03-29 07:23:21.000000 CamoTSS-0.1.3/CamoTSS/bin/count.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS/model/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      877 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/CamoTSS/model/logistic_4feature_model.sav
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS/utils/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/CamoTSS/utils/__init__.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2484 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/CamoTSS/utils/build_ref.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    24204 2023-03-29 10:23:41.000000 CamoTSS-0.1.3/CamoTSS/utils/get_counts.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2847 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/CamoTSS/utils/get_inputfile_toBrie.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       21 2023-03-29 12:01:20.000000 CamoTSS-0.1.3/CamoTSS/version.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS.egg-info/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     4292 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS.egg-info/PKG-INFO
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1066 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS.egg-info/SOURCES.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        1 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS.egg-info/dependency_links.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       51 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS.egg-info/entry_points.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      190 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS.egg-info/requires.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        8 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/CamoTSS.egg-info/top_level.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11357 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/LICENSE
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     4292 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/PKG-INFO
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3934 2023-03-29 10:22:04.000000 CamoTSS-0.1.3/README.rst
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/doc/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      586 2023-03-28 02:00:02.000000 CamoTSS-0.1.3/doc/Makefile
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     5455 2023-03-28 02:23:26.000000 CamoTSS-0.1.3/doc/conf.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/doc/image/
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   366757 2023-03-28 08:07:48.000000 CamoTSS-0.1.3/doc/image/classifier.png
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   289172 2023-03-28 08:07:53.000000 CamoTSS-0.1.3/doc/image/flow_chart.png
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1777 2023-03-29 03:10:49.000000 CamoTSS-0.1.3/doc/index.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      534 2023-03-28 10:39:09.000000 CamoTSS-0.1.3/doc/install.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3022 2023-03-29 09:39:28.000000 CamoTSS-0.1.3/doc/preprocess.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      237 2023-03-28 13:16:24.000000 CamoTSS-0.1.3/doc/requirements.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2027 2023-03-29 03:27:15.000000 CamoTSS-0.1.3/doc/run_CamoTSS.rst
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/notebook/
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   358197 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig1D_classifier.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)     2156 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig1E.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   127734 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig1H.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   583027 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig2A.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   299812 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig2E.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)  2294709 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig2F.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   148134 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig2H.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   346423 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig2I.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  1205611 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig3_NPC.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)   109335 2023-03-27 12:40:14.000000 CamoTSS-0.1.3/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb
--rw-r--r--   0 houruiyan  (1122) houruiyan  (1144)    76297 2023-03-26 13:01:47.000000 CamoTSS-0.1.3/notebook/Fig4I.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       38 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/setup.cfg
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2405 2023-03-29 11:56:41.000000 CamoTSS-0.1.3/setup.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-03-29 12:01:42.000000 CamoTSS-0.1.3/test/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  9240576 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/test/32_4_feature.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144) 25807864 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/test/Homo_sapiens.GRCh38.105.chr_test.gtf
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      999 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/test/logistic_36feature_model.sav
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   191754 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/test/train_fromSCAFE.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    51540 2023-03-26 12:56:46.000000 CamoTSS-0.1.3/test/trian_ourself_dataset.csv
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1810 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/.gitignore
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       33 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/__init__.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/bin/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/bin/__init__.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     5403 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/bin/count.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/model/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      877 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/model/logistic_4feature_model.sav
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/utils/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/__init__.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2484 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/build_ref.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    24204 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/get_counts.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2847 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/get_inputfile_toBrie.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       21 2023-04-17 06:18:25.000000 CamoTSS-0.1.4/CamoTSS/version.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS.egg-info/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/PKG-INFO
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1405 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS.egg-info/SOURCES.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        1 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/dependency_links.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       51 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/entry_points.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      191 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/requires.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        8 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/top_level.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11357 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/LICENSE
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/PKG-INFO
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2401 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/README.rst
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/docs/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     6762 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/Makefile
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     9651 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/conf.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/docs/image/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   366757 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/image/classifier.png
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   289172 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/image/flow_chart.png
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1765 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/index.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      709 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/install.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3034 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/preprocess.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      100 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/release.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      231 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/requirements.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3582 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/run_CamoTSS.rst
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/notebook/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   358197 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig1D_classifier.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2156 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig1E.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   127734 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig1H.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   583027 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2A.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   299812 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2E.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  2294709 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2F.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   148134 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2H.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   346423 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2I.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  1205611 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig3_NPC.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109335 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    76297 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig4I.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109166 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/runBRIE.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       38 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/setup.cfg
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2339 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/setup.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  9240576 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/32_4_feature.csv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144) 25807864 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/Homo_sapiens.GRCh38.105.chr_test.gtf
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    31059 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/cellbarcode_to_CamoTSS.tsv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      999 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/logistic_36feature_model.sav
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/test_out/
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/test_out/count/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  3196749 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/fetch_reads.pkl
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11380 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/fourFeature.csv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  6498398 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/keepdict.pkl
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   626958 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/scTSS_count_all.h5ad
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   125160 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/scTSS_count_two.h5ad
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/test_out/ref_file/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   161683 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/ref_file/ref_TSS.tsv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    35122 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/ref_file/ref_gene.tsv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   191754 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/train_fromSCAFE.csv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    51540 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/trian_ourself_dataset.csv
```

### Comparing `CamoTSS-0.1.3/.gitignore` & `CamoTSS-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/CamoTSS/bin/count.py` & `CamoTSS-0.1.4/CamoTSS/bin/count.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 
 START_TIME = time.time()
 
 
 def main():
     parser = OptionParser()
     parser.add_option('--gtf','-g',dest='gtf_file',default=None,help='The annotation gtf file for your analysing species.')
-    parser.add_option('--cdrFile','-c',dest='cdrFile',default=None,help='The file include cell barcode which users want to keep in the downstream analysis.Actually, it can be the same file input in the scTSS-quant')
+    parser.add_option('--cellbarcodeFile','-c',dest='cdrFile',default=None,help='The file include cell barcode which users want to keep in the downstream analysis.')
     parser.add_option('--bam','-b',dest='bam_file',default=None,help='The bam file of aligned from Cellranger or other single cell aligned software.')
     parser.add_option('--outdir','-o',dest='out_dir',default=None,help='The directory for output [default : $bam_file]') #what should be after $
-    parser.add_option('--refFasta','-r',dest='refFasta',default=None,help='The directory for reference fasta file') #what should be after $
+    parser.add_option('--refFasta','-r',dest='refFasta',default=None,help='The directory for reference genome fasta file') #what should be after $
     parser.add_option('--mode','-m',dest='mode',default=None,help='You can select run by finding novel TSS cluster mode [TC]. If you also want to detect CTSS within one cluster, you can use [CTSS] mode')
 
    
    
     group0=OptionGroup(parser,"Optional arguments")
 
     group0.add_option("--minCount",type="int",dest="minCount",default=50,
-    help="Minimum counts for each transcript in all cells [default: 50]")
-    # group0.add_option("--isoformNumber",type="int",dest="isoformNumber",default=2,
-    # help="No. of isoform keeping in for each gene [default: 2]")
+    help="Minimum UMI counts for TC in all cells [default: 50]")
+
     group0.add_option('--nproc','-p',type="int",dest='nproc',default=4,
     help='Number of subprocesses [default: 4]')
 
     group0.add_option('--maxReadCount',type="int",dest='maxReadCount',default=10000,
-    help='For each gene, the maxmium read count kept for clustering[default: 10000]')
+    help='For each gene, the maxmium read count kept for clustering [default: 10000]')
     
     group0.add_option('--clusterDistance',type="float",dest='clusterDistance',default=300,
     help="The minimum distance between two cluster transcription start site [default: 300]")
 
     group0.add_option('--InnerDistance',type="float",dest='InnerDistance',default=100,
     help="The resolution of each cluster [default: 100]")
```

### Comparing `CamoTSS-0.1.3/CamoTSS/model/logistic_4feature_model.sav` & `CamoTSS-0.1.4/CamoTSS/model/logistic_4feature_model.sav`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/CamoTSS/utils/build_ref.py` & `CamoTSS-0.1.4/CamoTSS/utils/build_ref.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/CamoTSS/utils/get_counts.py` & `CamoTSS-0.1.4/CamoTSS/utils/get_counts.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/CamoTSS/utils/get_inputfile_toBrie.py` & `CamoTSS-0.1.4/CamoTSS/utils/get_inputfile_toBrie.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/CamoTSS.egg-info/SOURCES.txt` & `CamoTSS-0.1.4/CamoTSS.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,32 +13,42 @@
 CamoTSS/bin/__init__.py
 CamoTSS/bin/count.py
 CamoTSS/model/logistic_4feature_model.sav
 CamoTSS/utils/__init__.py
 CamoTSS/utils/build_ref.py
 CamoTSS/utils/get_counts.py
 CamoTSS/utils/get_inputfile_toBrie.py
-doc/Makefile
-doc/conf.py
-doc/index.rst
-doc/install.rst
-doc/preprocess.rst
-doc/requirements.txt
-doc/run_CamoTSS.rst
-doc/image/classifier.png
-doc/image/flow_chart.png
+docs/Makefile
+docs/conf.py
+docs/index.rst
+docs/install.rst
+docs/preprocess.rst
+docs/release.rst
+docs/requirements.txt
+docs/run_CamoTSS.rst
+docs/image/classifier.png
+docs/image/flow_chart.png
 notebook/Fig1D_classifier.ipynb
 notebook/Fig1E.ipynb
 notebook/Fig1H.ipynb
 notebook/Fig2A.ipynb
 notebook/Fig2E.ipynb
 notebook/Fig2F.ipynb
 notebook/Fig2H.ipynb
 notebook/Fig2I.ipynb
 notebook/Fig3_NPC.ipynb
 notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb
 notebook/Fig4I.ipynb
+notebook/runBRIE.ipynb
 test/32_4_feature.csv
 test/Homo_sapiens.GRCh38.105.chr_test.gtf
+test/cellbarcode_to_CamoTSS.tsv
 test/logistic_36feature_model.sav
 test/train_fromSCAFE.csv
-test/trian_ourself_dataset.csv
+test/trian_ourself_dataset.csv
+test/test_out/count/fetch_reads.pkl
+test/test_out/count/fourFeature.csv
+test/test_out/count/keepdict.pkl
+test/test_out/count/scTSS_count_all.h5ad
+test/test_out/count/scTSS_count_two.h5ad
+test/test_out/ref_file/ref_TSS.tsv
+test/test_out/ref_file/ref_gene.tsv
```

### Comparing `CamoTSS-0.1.3/LICENSE` & `CamoTSS-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/doc/image/classifier.png` & `CamoTSS-0.1.4/docs/image/classifier.png`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/doc/image/flow_chart.png` & `CamoTSS-0.1.4/docs/image/flow_chart.png`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/doc/index.rst` & `CamoTSS-0.1.4/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-|PyPI| |Docs| |Build Status|
+|PyPI| |Docs| 
 
 .. |PyPI| image:: https://badge.fury.io/py/CamoTSS.svg
        :target: https://pypi.org/project/CamoTSS/
-.. |Docs| image:: https://readthedocs.org/projects/CamoTSS/badge/?version=latest
-      :target: https://CamoTSS.readthedocs.io
-.. |Build Status| image:: https://travis-ci.org/huangyh09/brie.svg?branch=master
-      :target: https://travis-ci.org/huangyh09/brie
+.. |Docs| image:: https://readthedocs.org/projects/camotss/badge/?version=latest
+      :target: https://camotss.readthedocs.io/en/latest/?badge=latest
+
 
 
 
 ====
 Home
 ====
 
 
 
 About CamoTSS
 ==================
 
 CamoTSS can  precisely identify TSS and quantify its expression by leveraging the cDNA on read 1, which enables effective detection of alternative TSS usage.
 
-CamoTSS supports the analysis of alternative TSS at two levels, TSS cluster (TC mode) and CTSS (CTSS mode). 
-The input files of CamoTSS include alignment file (bam file), annotation file (gtf file), cell list file and reference genome file (fasta file). 
-The output files of CamoTSS include cell by all TSSs matrix (h5ad), cell by two TSSs matrix (h5ad), cell by CTSS matrix (h5ad) and cell by CTSS matrix (h5ad). 
+CamoTSS supports the analysis of alternative TSS at two levels, TSS cluster (**TC mode**) and CTSS (**CTSS mode**). 
+The input files of CamoTSS include alignment file (`bam file`), annotation file (`gtf file`), cell list file and reference genome file (`fasta file`). 
+The output files of CamoTSS include cell by all TSSs matrix (`h5ad`), cell by two TSSs matrix (`h5ad`), cell by CTSS matrix (`h5ad`) and cell by CTSS matrix (`h5ad`). 
 
 CamoTSS identify TSS through the following steps.
 
 .. image:: image/flow_chart.png
    :width: 600
    :alt: flow chart for CamoTSS
    :align: center
@@ -38,26 +37,36 @@
    :width: 600
    :alt: classifier
    :align: center
 
 
 
 
-It includes 3 steps to identify alternative TSS or CTSS usage: preprocessing, running CamoTSS and running Brie2.
+It includes 3 steps to identify alternative TSS or CTSS usage: preprocessing, running CamoTSS and running BRIE2.
 
 Please refer to our tutorial for details.
 
 
 * `Preprocess for one sample and multiple samples`_.
 
 * `Run CamoTSS`_.
 
 * `Run Brie2`_.
 
-.. _Preprocess for one sample and multiple samples: melanoma.ipynb
+.. _Preprocess for one sample and multiple samples: preprocess.rst
+
+.. _Run CamoTSS: run_CamoTSS.rst
 
-.. _Run CamoTSS: differential_test_intestine.ipynb
+.. _Run Brie2: runBRIE.ipynb
 
-.. _Run Brie2: differential_test_intestine.ipynb
 
+.. toctree::
+   :caption: Main
+   :maxdepth: 1
+   :hidden:
 
-    
+   index
+   install
+   preprocess
+   run_CamoTSS
+   runBRIE
+   release
```

### Comparing `CamoTSS-0.1.3/doc/install.rst` & `CamoTSS-0.1.4/docs/install.rst`

 * *Files 23% similar despite different names*

```diff
@@ -13,7 +13,10 @@
 
 .. code-block:: bash
 
    pip install -U git+https://github.com/StatBiomed/CamoTSS
 
 In either case, add --user if you don’t have the write permission for your Python environment.
 
+If you run into any issues or errors are raised during the installation process, feel free to contact us at GitHub_.
+
+.. _GitHub: https://github.com/StatBiomed/CamoTSS/issues
```

### Comparing `CamoTSS-0.1.3/doc/preprocess.rst` & `CamoTSS-0.1.4/docs/preprocess.rst`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 Here, we try to filter 10x Genomic BAM file (i.e. possorted_genome_bam.bam) to
 make it cooperate with filtered_feature_bc_matrix. 
 
 Filtering UMI according to the specific criteria:
 
 .. code-block:: html
 
-* Have a MAPQ score of 255
-* Maps to exactly one gene
-* Overlaps an exon by at least 50% in a way consistent with annotated splice junctions and strand annotation. Records that align to exons will have an RE:A:E tag.
-* Remove any records with matching UMI and Barcode values that map to different genes.
+   * Have a MAPQ score of 255
+   * Maps to exactly one gene
+   * Overlaps an exon by at least 50% in a way consistent with annotated splice junctions and strand annotation. Records that align to exons will have an RE:A:E tag.
+   * Remove any records with matching UMI and Barcode values that map to different genes.
 
 
 For more information, you can check this material_ .
 
 .. _material: https://www.10xgenomics.com/resources/analysis-guides/tutorial-navigating-10x-barcoded-bam-files 
 
 To get cleaner bam, you can process possorted_genome_bam.bam according to the following steps.
```

### Comparing `CamoTSS-0.1.3/notebook/Fig1D_classifier.ipynb` & `CamoTSS-0.1.4/notebook/Fig1D_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig1E.ipynb` & `CamoTSS-0.1.4/notebook/Fig1E.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig1H.ipynb` & `CamoTSS-0.1.4/notebook/Fig1H.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig2A.ipynb` & `CamoTSS-0.1.4/notebook/Fig2A.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig2E.ipynb` & `CamoTSS-0.1.4/notebook/Fig2E.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig2F.ipynb` & `CamoTSS-0.1.4/notebook/Fig2F.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig2H.ipynb` & `CamoTSS-0.1.4/notebook/Fig2H.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig2I.ipynb` & `CamoTSS-0.1.4/notebook/Fig2I.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig3_NPC.ipynb` & `CamoTSS-0.1.4/notebook/Fig3_NPC.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb` & `CamoTSS-0.1.4/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/notebook/Fig4I.ipynb` & `CamoTSS-0.1.4/notebook/Fig4I.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/setup.py` & `CamoTSS-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Set __version__ for the project.
 exec(open("./CamoTSS/version.py").read())
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
     
-reqs = ['numpy>=1.9.0', 'scipy>=1.4.0', 'matplotlib','anndata>=0.6','pyranges>=0.0.115'
+reqs = ['numpy>=1.9.0', 'scipy>=1.4.0', 'matplotlib','anndata>=0.6','pyranges>=0.0.115',
 'scanpy>=1.5','pysam>=0.15.2','brie>=2.2.0','pandas>=0.23.0','scikit-learn>=0.23','editdistance>=0.3.1']
 
 setup(
     name='CamoTSS',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
@@ -50,16 +50,15 @@
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
 
 
 
 
     packages=find_packages(),
-    # packages='CamoTSS',
-    # package_dir={'CamoTSS': 'CamoTSS/'},
+
     package_data={'CamoTSS': ['model/*.sav']},
 
     entry_points={
           'console_scripts': [
             'CamoTSS = CamoTSS.bin.count:main',
             ],
           }, 
@@ -78,8 +77,8 @@
             #'sphinx == 1.8.3',
             'sphinx_bootstrap_theme']},
 
     py_modules = ['CamoTSS']
 
     # buid the distribution: python setup.py sdist
     # upload to pypi: twine upload dist/...
-)
+)
```

### Comparing `CamoTSS-0.1.3/test/32_4_feature.csv` & `CamoTSS-0.1.4/test/32_4_feature.csv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/test/Homo_sapiens.GRCh38.105.chr_test.gtf` & `CamoTSS-0.1.4/test/Homo_sapiens.GRCh38.105.chr_test.gtf`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/test/logistic_36feature_model.sav` & `CamoTSS-0.1.4/test/logistic_36feature_model.sav`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/test/train_fromSCAFE.csv` & `CamoTSS-0.1.4/test/train_fromSCAFE.csv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.3/test/trian_ourself_dataset.csv` & `CamoTSS-0.1.4/test/trian_ourself_dataset.csv`

 * *Files identical despite different names*

