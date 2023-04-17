# Comparing `tmp/CamoTSS-0.1.4.tar.gz` & `tmp/CamoTSS-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CamoTSS-0.1.4.tar", last modified: Mon Apr 17 06:19:48 2023, max compression
+gzip compressed data, was "dist/CamoTSS-0.1.5.tar", last modified: Mon Apr 17 06:48:24 2023, max compression
```

## Comparing `CamoTSS-0.1.4.tar` & `CamoTSS-0.1.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1810 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/.gitignore
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       33 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/__init__.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/bin/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/bin/__init__.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     5403 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/bin/count.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/model/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      877 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/model/logistic_4feature_model.sav
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS/utils/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/__init__.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2484 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/build_ref.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    24204 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/get_counts.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2847 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/CamoTSS/utils/get_inputfile_toBrie.py
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       21 2023-04-17 06:18:25.000000 CamoTSS-0.1.4/CamoTSS/version.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS.egg-info/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/PKG-INFO
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1405 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/CamoTSS.egg-info/SOURCES.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        1 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/dependency_links.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       51 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/entry_points.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      191 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/requires.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        8 2023-04-17 06:19:47.000000 CamoTSS-0.1.4/CamoTSS.egg-info/top_level.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11357 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/LICENSE
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/PKG-INFO
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2401 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/README.rst
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/docs/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     6762 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/Makefile
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     9651 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/conf.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/docs/image/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   366757 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/image/classifier.png
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   289172 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/image/flow_chart.png
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1765 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/index.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      709 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/install.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3034 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/preprocess.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      100 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/release.rst
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      231 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/requirements.txt
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3582 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/docs/run_CamoTSS.rst
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/notebook/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   358197 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig1D_classifier.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2156 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig1E.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   127734 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig1H.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   583027 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2A.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   299812 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2E.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  2294709 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2F.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   148134 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2H.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   346423 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig2I.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  1205611 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig3_NPC.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109335 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    76297 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/Fig4I.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109166 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/notebook/runBRIE.ipynb
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       38 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/setup.cfg
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2339 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/setup.py
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  9240576 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/32_4_feature.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144) 25807864 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/Homo_sapiens.GRCh38.105.chr_test.gtf
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    31059 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/cellbarcode_to_CamoTSS.tsv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      999 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/logistic_36feature_model.sav
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/test_out/
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/test_out/count/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  3196749 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/fetch_reads.pkl
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11380 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/fourFeature.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  6498398 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/keepdict.pkl
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   626958 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/scTSS_count_all.h5ad
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   125160 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/count/scTSS_count_two.h5ad
-drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:19:48.000000 CamoTSS-0.1.4/test/test_out/ref_file/
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   161683 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/ref_file/ref_TSS.tsv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    35122 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/test_out/ref_file/ref_gene.tsv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   191754 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/train_fromSCAFE.csv
--rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    51540 2023-04-17 06:02:41.000000 CamoTSS-0.1.4/test/trian_ourself_dataset.csv
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1810 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/.gitignore
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       33 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/__init__.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/bin/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/bin/__init__.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     5403 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/bin/count.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/model/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      877 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/model/logistic_4feature_model.sav
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS/utils/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/__init__.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2484 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/build_ref.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    24214 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/get_counts.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2847 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/utils/get_inputfile_toBrie.py
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       22 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/CamoTSS/version.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS.egg-info/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/PKG-INFO
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1405 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/CamoTSS.egg-info/SOURCES.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        1 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/dependency_links.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       51 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/entry_points.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      191 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/requires.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)        8 2023-04-17 06:48:23.000000 CamoTSS-0.1.5/CamoTSS.egg-info/top_level.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11357 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/LICENSE
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2759 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/PKG-INFO
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2401 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/README.rst
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/docs/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     6762 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/Makefile
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     9651 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/conf.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/docs/image/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   366757 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/image/classifier.png
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   289172 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/image/flow_chart.png
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     1765 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/index.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      709 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/install.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3034 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/preprocess.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      100 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/release.rst
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      231 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/requirements.txt
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     3582 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/docs/run_CamoTSS.rst
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/notebook/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   358197 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig1D_classifier.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2156 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig1E.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   127734 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig1H.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   583027 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2A.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   299812 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2E.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  2294709 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2F.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   148134 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2H.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   346423 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig2I.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  1205611 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig3_NPC.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109335 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    76297 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/Fig4I.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   109166 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/notebook/runBRIE.ipynb
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)       38 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/setup.cfg
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)     2339 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/setup.py
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  9240576 2023-04-17 06:48:01.000000 CamoTSS-0.1.5/test/32_4_feature.csv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144) 25807864 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/Homo_sapiens.GRCh38.105.chr_test.gtf
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    31059 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/cellbarcode_to_CamoTSS.tsv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)      999 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/logistic_36feature_model.sav
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/test_out/
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/test_out/count/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  3196749 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/fetch_reads.pkl
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    11380 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/fourFeature.csv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)  6498398 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/keepdict.pkl
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   626958 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/scTSS_count_all.h5ad
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   125160 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/count/scTSS_count_two.h5ad
+drwxrwxr-x   0 houruiyan  (1122) houruiyan  (1144)        0 2023-04-17 06:48:24.000000 CamoTSS-0.1.5/test/test_out/ref_file/
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   161683 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/ref_file/ref_TSS.tsv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    35122 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/test_out/ref_file/ref_gene.tsv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)   191754 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/train_fromSCAFE.csv
+-rw-rw-r--   0 houruiyan  (1122) houruiyan  (1144)    51540 2023-04-17 06:48:02.000000 CamoTSS-0.1.5/test/trian_ourself_dataset.csv
```

### Comparing `CamoTSS-0.1.4/.gitignore` & `CamoTSS-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/CamoTSS/bin/count.py` & `CamoTSS-0.1.5/CamoTSS/bin/count.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/CamoTSS/model/logistic_4feature_model.sav` & `CamoTSS-0.1.5/CamoTSS/model/logistic_4feature_model.sav`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/CamoTSS/utils/build_ref.py` & `CamoTSS-0.1.5/CamoTSS/utils/build_ref.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/CamoTSS/utils/get_counts.py` & `CamoTSS-0.1.5/CamoTSS/utils/get_counts.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,23 +317,23 @@
         
         fourfeaturedf=pd.DataFrame(clusterdict).T 
         fourfeature_output=self.count_out_dir+'fourFeature.csv'
         fourfeaturedf.to_csv(fourfeature_output)
 
         print('one_gene_with_two_TSS_fourfeature : %i'%(len(fourfeaturedf)))
         test_X=fourfeaturedf.iloc[:,0:4]
-        print('hello')
+        # print('hello')
 
-        print(os.path.abspath(__file__))
+        # print(os.path.abspath(__file__))
 
-        print(os.path.dirname(os.path.abspath(__file__)))
+        # print(os.path.dirname(os.path.abspath(__file__)))
 
-        print(Path(os.path.dirname(os.path.abspath(__file__))))
+        # print(Path(os.path.dirname(os.path.abspath(__file__))))
 
-        print(Path(os.path.dirname(os.path.abspath(__file__))).parents[1])
+        # print(Path(os.path.dirname(os.path.abspath(__file__))).parents[1])
 
         pathstr=str(Path(os.path.dirname(os.path.abspath(__file__))).parents[0])+'/model/logistic_4feature_model.sav'
         loaded_model = pickle.load(open(pathstr, 'rb'))
         test_Y=loaded_model.predict(test_X.values)
 
         #do filtering, the result of this step should be output as final h5ad file display at single cell level. 
         afterfiltereddf=fourfeaturedf[test_Y==1]
```

### Comparing `CamoTSS-0.1.4/CamoTSS/utils/get_inputfile_toBrie.py` & `CamoTSS-0.1.5/CamoTSS/utils/get_inputfile_toBrie.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/CamoTSS.egg-info/PKG-INFO` & `CamoTSS-0.1.5/CamoTSS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamoTSS
-Version: 0.1.4
+Version: 0.1.5
 Summary: CamoTSS: Detection alternative TSS in single cells
 Home-page: https://github.com/StatBiomed/CamoTSS
 Author: ['Ruiyan Hou']
 Author-email: ruiyan@connect.hku.hk
 License: Apache-2.0
 Keywords: Transcript Start Site,single-cell RNA-seq
 Requires-Python: >=3.5
```

### Comparing `CamoTSS-0.1.4/CamoTSS.egg-info/SOURCES.txt` & `CamoTSS-0.1.5/CamoTSS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/LICENSE` & `CamoTSS-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/PKG-INFO` & `CamoTSS-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CamoTSS
-Version: 0.1.4
+Version: 0.1.5
 Summary: CamoTSS: Detection alternative TSS in single cells
 Home-page: https://github.com/StatBiomed/CamoTSS
 Author: ['Ruiyan Hou']
 Author-email: ruiyan@connect.hku.hk
 License: Apache-2.0
 Keywords: Transcript Start Site,single-cell RNA-seq
 Requires-Python: >=3.5
```

### Comparing `CamoTSS-0.1.4/README.rst` & `CamoTSS-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/Makefile` & `CamoTSS-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/conf.py` & `CamoTSS-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/image/classifier.png` & `CamoTSS-0.1.5/docs/image/classifier.png`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/image/flow_chart.png` & `CamoTSS-0.1.5/docs/image/flow_chart.png`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/index.rst` & `CamoTSS-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/install.rst` & `CamoTSS-0.1.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/preprocess.rst` & `CamoTSS-0.1.5/docs/preprocess.rst`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/docs/run_CamoTSS.rst` & `CamoTSS-0.1.5/docs/run_CamoTSS.rst`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig1D_classifier.ipynb` & `CamoTSS-0.1.5/notebook/Fig1D_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig1E.ipynb` & `CamoTSS-0.1.5/notebook/Fig1E.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig1H.ipynb` & `CamoTSS-0.1.5/notebook/Fig1H.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig2A.ipynb` & `CamoTSS-0.1.5/notebook/Fig2A.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig2E.ipynb` & `CamoTSS-0.1.5/notebook/Fig2E.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig2F.ipynb` & `CamoTSS-0.1.5/notebook/Fig2F.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig2H.ipynb` & `CamoTSS-0.1.5/notebook/Fig2H.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig2I.ipynb` & `CamoTSS-0.1.5/notebook/Fig2I.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig3_NPC.ipynb` & `CamoTSS-0.1.5/notebook/Fig3_NPC.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb` & `CamoTSS-0.1.5/notebook/Fig3_detect_TSS_shift_in_NPC_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/Fig4I.ipynb` & `CamoTSS-0.1.5/notebook/Fig4I.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/notebook/runBRIE.ipynb` & `CamoTSS-0.1.5/notebook/runBRIE.ipynb`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/setup.py` & `CamoTSS-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/32_4_feature.csv` & `CamoTSS-0.1.5/test/32_4_feature.csv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/Homo_sapiens.GRCh38.105.chr_test.gtf` & `CamoTSS-0.1.5/test/Homo_sapiens.GRCh38.105.chr_test.gtf`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/cellbarcode_to_CamoTSS.tsv` & `CamoTSS-0.1.5/test/cellbarcode_to_CamoTSS.tsv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/logistic_36feature_model.sav` & `CamoTSS-0.1.5/test/logistic_36feature_model.sav`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/test_out/count/fetch_reads.pkl` & `CamoTSS-0.1.5/test/test_out/count/fetch_reads.pkl`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/test_out/count/fourFeature.csv` & `CamoTSS-0.1.5/test/test_out/count/fourFeature.csv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/test_out/count/keepdict.pkl` & `CamoTSS-0.1.5/test/test_out/count/keepdict.pkl`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/test_out/count/scTSS_count_all.h5ad` & `CamoTSS-0.1.5/test/test_out/count/scTSS_count_all.h5ad`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/test_out/count/scTSS_count_two.h5ad` & `CamoTSS-0.1.5/test/test_out/count/scTSS_count_two.h5ad`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/test_out/ref_file/ref_TSS.tsv` & `CamoTSS-0.1.5/test/test_out/ref_file/ref_TSS.tsv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/test_out/ref_file/ref_gene.tsv` & `CamoTSS-0.1.5/test/test_out/ref_file/ref_gene.tsv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/train_fromSCAFE.csv` & `CamoTSS-0.1.5/test/train_fromSCAFE.csv`

 * *Files identical despite different names*

### Comparing `CamoTSS-0.1.4/test/trian_ourself_dataset.csv` & `CamoTSS-0.1.5/test/trian_ourself_dataset.csv`

 * *Files identical despite different names*

