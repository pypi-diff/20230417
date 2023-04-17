# Comparing `tmp/lsaBGC-1.34.tar.gz` & `tmp/lsaBGC-1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsaBGC-1.34.tar", last modified: Sun Apr 16 16:19:05 2023, max compression
+gzip compressed data, was "lsaBGC-1.35.tar", last modified: Mon Apr 17 05:52:22 2023, max compression
```

## Comparing `lsaBGC-1.34.tar` & `lsaBGC-1.35.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.538323 lsaBGC-1.34/
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)     1517 2023-04-16 12:26:58.000000 lsaBGC-1.34/LICENSE
--rw-rw-r--   0 rauf      (1000) rauf      (1000)      398 2023-04-16 16:19:05.538323 lsaBGC-1.34/PKG-INFO
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)     6374 2023-04-16 12:26:58.000000 lsaBGC-1.34/README.md
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.534323 lsaBGC-1.34/bin/
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)     8651 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Cluster.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)    13310 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-DiscoVary.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)    10541 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Divergence.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)    14738 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Expansion.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    15751 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-MIBiGMapper.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)    12808 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-PopGene.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    37287 2023-04-16 13:01:21.000000 lsaBGC-1.34/bin/lsaBGC-Ready.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)     7734 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Refiner.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)    11168 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-See.py
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.534323 lsaBGC-1.34/lsaBGC/
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 12:26:58.000000 lsaBGC-1.34/lsaBGC/__init__.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)    14437 2023-04-16 12:26:58.000000 lsaBGC-1.34/lsaBGC/processing.py
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)   105244 2023-04-16 12:26:58.000000 lsaBGC-1.34/lsaBGC/util.py
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.534323 lsaBGC-1.34/lsaBGC.egg-info/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)      398 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/PKG-INFO
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     1020 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/SOURCES.txt
--rw-rw-r--   0 rauf      (1000) rauf      (1000)        1 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/dependency_links.txt
--rw-rw-r--   0 rauf      (1000) rauf      (1000)        1 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/not-zip-safe
--rw-rw-r--   0 rauf      (1000) rauf      (1000)        7 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/top_level.txt
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.538323 lsaBGC-1.34/scripts/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    23594 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/GSeeF.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     7624 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/compareBGCtoGenomeCodonUsage.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     2984 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/createPickleOfSampleAnnotationListingFile.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     6276 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/listAllBGCGenbanksInDirectory.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    10399 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/listAllGenomesInDirectory.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    16757 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/popSizeAndSampleSelector.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     7962 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/processAndReformatNCBIGenbanks.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     8298 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/readifyAdditionalGenomes.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     7465 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/runProdigalAndMakeProperGenbank.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     5055 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/setup_annotation_dbs.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     3185 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/setup_bigscape.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)     3447 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/simpleProteinExtraction.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    12961 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/visualize_BGC-Ome.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)       38 2023-04-16 16:19:05.538323 lsaBGC-1.34/setup.cfg
--rwxrwxr-x   0 rauf      (1000) rauf      (1000)     1749 2023-04-16 12:26:58.000000 lsaBGC-1.34/setup.py
-drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.538323 lsaBGC-1.34/workflows/
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    37391 2023-04-16 12:26:58.000000 lsaBGC-1.34/workflows/lsaBGC-AutoAnalyze.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    18148 2023-04-16 12:26:58.000000 lsaBGC-1.34/workflows/lsaBGC-AutoExpansion.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    43849 2023-04-16 13:09:44.000000 lsaBGC-1.34/workflows/lsaBGC-Easy.py
--rw-rw-r--   0 rauf      (1000) rauf      (1000)    37686 2023-04-16 13:09:44.000000 lsaBGC-1.34/workflows/lsaBGC-Euk-Easy.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.381701 lsaBGC-1.35/
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1517 2023-04-16 22:46:02.000000 lsaBGC-1.35/LICENSE
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-04-17 05:52:22.381701 lsaBGC-1.35/PKG-INFO
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     6494 2023-04-16 22:46:02.000000 lsaBGC-1.35/README.md
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.377701 lsaBGC-1.35/bin/
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     8651 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Cluster.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10729 2023-04-17 03:41:01.000000 lsaBGC-1.35/bin/lsaBGC-ComprehenSeeIve.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    13310 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-DiscoVary.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    10541 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Divergence.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14738 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Expansion.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    15751 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-MIBiGMapper.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    12808 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-PopGene.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    37287 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Ready.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     7734 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Refiner.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    11168 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-See.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.377701 lsaBGC-1.35/lsaBGC/
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-16 22:46:02.000000 lsaBGC-1.35/lsaBGC/__init__.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14437 2023-04-16 22:46:02.000000 lsaBGC-1.35/lsaBGC/processing.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)   105402 2023-04-17 04:47:50.000000 lsaBGC-1.35/lsaBGC/util.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.377701 lsaBGC-1.35/lsaBGC.egg-info/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/PKG-INFO
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     1050 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/SOURCES.txt
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/dependency_links.txt
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/not-zip-safe
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        7 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/top_level.txt
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.381701 lsaBGC-1.35/scripts/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    23594 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/GSeeF.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7624 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/compareBGCtoGenomeCodonUsage.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     2984 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/createPickleOfSampleAnnotationListingFile.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     6276 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/listAllBGCGenbanksInDirectory.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10399 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/listAllGenomesInDirectory.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    16757 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/popSizeAndSampleSelector.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7962 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/processAndReformatNCBIGenbanks.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     8298 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/readifyAdditionalGenomes.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7465 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/runProdigalAndMakeProperGenbank.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     5055 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/setup_annotation_dbs.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3185 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/setup_bigscape.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3447 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/simpleProteinExtraction.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    12818 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/visualize_BGC-Ome.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)       38 2023-04-17 05:52:22.381701 lsaBGC-1.35/setup.cfg
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1797 2023-04-17 01:52:56.000000 lsaBGC-1.35/setup.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.381701 lsaBGC-1.35/workflows/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    40240 2023-04-17 05:19:18.000000 lsaBGC-1.35/workflows/lsaBGC-AutoAnalyze.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    18332 2023-04-17 03:23:33.000000 lsaBGC-1.35/workflows/lsaBGC-AutoExpansion.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    44237 2023-04-17 03:32:24.000000 lsaBGC-1.35/workflows/lsaBGC-Easy.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    38073 2023-04-17 03:32:24.000000 lsaBGC-1.35/workflows/lsaBGC-Euk-Easy.py
```

### Comparing `lsaBGC-1.34/LICENSE` & `lsaBGC-1.35/LICENSE`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/README.md` & `lsaBGC-1.35/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,28 +61,32 @@
 A small test case is provided here and can be run after installation by simply issuing (takes around ~7 minutes using 4 cpus/threads):
 
 ```
 # Warning: uses 4 cpus/threads! 
 bash run_tests.sh
 ```
 
-Additionally, there are additional [test cases](https://github.com/Kalan-Lab/lsaBGC_Ckefir_Testing_Cases) to demonstrate usage of individual programs along with expected outputs from commands. We also have a [quick start + walk-through tutorial Wiki page](https://github.com/Kalan-Lab/lsaBGC/wiki/03.-Quick-Start-&-In-Depth-Tutorial:-Exploring-BGCs-in-Cutibacterium) to showcase the use of the suite and relations between core programs.
+There are also additional [test cases](https://github.com/Kalan-Lab/lsaBGC_Ckefir_Testing_Cases) to demonstrate usage of individual programs along with expected outputs from commands. We also have a [walk-through tutorial Wiki page](https://github.com/Kalan-Lab/lsaBGC/wiki/03.-Quick-Start-&-In-Depth-Tutorial:-Exploring-BGCs-in-Cutibacterium) to showcase the use of the suite and relations between core programs.
 
-The major outputs of the final `lsaBGC-AutoAnalyze.py` run are in the resulting folder `test_case/lsaBGC_AutoAnalyze_Results/Final_Results/` and described on [this wiki page](https://github.com/Kalan-Lab/lsaBGC/wiki/16.-Overview-of-lsaBGC-AutoAnalyze's-Final-Results). Examples for the final AutoAnalyze results from an `lsaBGC-Easy.py` run on Cutibacterium avidum can be found [here on Google Drive](https://drive.google.com/drive/u/1/folders/1jHFFOUTd4SbIO-xiGG8MWTZaP1U4RF1j). 
+The major outputs of the final `lsaBGC-AutoAnalyze.py` run are in the resulting folder `test_case/lsaBGC_AutoAnalyze_Results/Final_Results/` and described on [this wiki page](https://github.com/Kalan-Lab/lsaBGC/wiki/13.-Overview-of-lsaBGC-AutoAnalyze's-Final-Results). Examples for the final AutoAnalyze results from an `lsaBGC-Easy.py` run on Cutibacterium avidum can be found [here on Google Drive](https://drive.google.com/drive/u/1/folders/1jHFFOUTd4SbIO-xiGG8MWTZaP1U4RF1j). 
 
 ## Quick Start - using `lsaBGC-Easy.py` and `lsaBGC-Euk-Easy.py` 
 
 Check out how to use `lsaBGC-Easy.py` and `lsaBGC-Euk-Easy.py` on [their wiki page](https://github.com/Kalan-Lab/lsaBGC/wiki/14.-lsaBGC-Easy-Tutorial)!
 
 ![image](https://user-images.githubusercontent.com/4260723/181613839-df183cdc-1103-403f-b5d1-889484f52be9.png)
 
 ## Acknowledgements:
 
 We would like to thank members of the Kalan lab, Currie lab, Kwan lab, Anantharaman, and Pepperell labs at UW Madison for feedback on the development of lsaBGC.
 
+## Feedback:
+
+Issues or suggestions for new features / changes to approaches? Please create an issue/ticket on GitHub issues and let us know!
+
 ## License:
 
 ```
 BSD 3-Clause License
 
 Copyright (c) 2021, Kalan-Lab
 All rights reserved.
```

### Comparing `lsaBGC-1.34/bin/lsaBGC-Cluster.py` & `lsaBGC-1.35/bin/lsaBGC-Cluster.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-DiscoVary.py` & `lsaBGC-1.35/bin/lsaBGC-DiscoVary.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-Divergence.py` & `lsaBGC-1.35/bin/lsaBGC-Divergence.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-Expansion.py` & `lsaBGC-1.35/bin/lsaBGC-Expansion.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-MIBiGMapper.py` & `lsaBGC-1.35/bin/lsaBGC-MIBiGMapper.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-PopGene.py` & `lsaBGC-1.35/bin/lsaBGC-PopGene.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-Ready.py` & `lsaBGC-1.35/bin/lsaBGC-Ready.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-Refiner.py` & `lsaBGC-1.35/bin/lsaBGC-Refiner.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/bin/lsaBGC-See.py` & `lsaBGC-1.35/bin/lsaBGC-See.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/lsaBGC/processing.py` & `lsaBGC-1.35/lsaBGC/processing.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/lsaBGC/util.py` & `lsaBGC-1.35/lsaBGC/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1887,80 +1887,83 @@
 def incorporateBGCProteinsIntoProteomesAndGenbanks(sample_bgc_proteins, sample_genomes, protein_annotations,
 												   bgc_prot_directory,
 												   proteomes_directory, final_proteomes_directory,
 												   final_genbanks_directory,
 												   sample_listing_file, bgc_listing_file, logObject):
 	sample_listing_handle = open(sample_listing_file, 'w')
 	bgc_listing_handle = open(bgc_listing_file, 'w')
+
 	try:
-		for sample in sample_bgc_proteins:
+		for sample in sample_genomes:
 
 			gw_prot_file = proteomes_directory + sample + '.faa'
 			gw_prot_to_location = {}
 			scaff_glts = defaultdict(set)
 			with open(gw_prot_file) as ogpf:
 				for rec in SeqIO.parse(ogpf, 'fasta'):
 					gw_prot_to_location[rec.id] = [rec.description.split()[1], int(rec.description.split()[2]),
 												   int(rec.description.split()[3])]
 					scaff_glts[rec.description.split()[1]].add(rec.id)
 
 			sample_lts_to_prune = set([])
 			sample_lts_to_add_protein_sequences = {}
 			sample_lts_to_add_genbank_features = defaultdict(list)
-			for bgc in sample_bgc_proteins[sample]:
 
-				bgc_listing_handle.write(sample + '\t' + bgc + '\n')
+			if sample in sample_bgc_proteins:
+				for bgc in sample_bgc_proteins[sample]:
+
+					bgc_listing_handle.write(sample + '\t' + bgc + '\n')
 
-				bgc_prots = sample_bgc_proteins[sample][bgc]
-				bgc_prots_1x = set([x for x in bgc_prots if x.split('_')[1][0] == '1'])
+					bgc_prots = sample_bgc_proteins[sample][bgc]
+					bgc_prots_1x = set([x for x in bgc_prots if x.split('_')[1][0] == '1'])
 
-				scaff_start = None
-				with open(bgc) as obf:
-					for rec in SeqIO.parse(obf, 'genbank'):
-						scaff_id = rec.id
-						scaff_start = int(rec.description.split()[-1].strip())
-						for feature in rec.features:
-							if feature.type == 'CDS':
-								prot_lt = feature.qualifiers.get('locus_tag')[0]
-								if prot_lt in bgc_prots_1x:
-									all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
-									fls = []
-									for sc, ec, dc in all_coords:
-										dir = 1
-										if dc == '-': dir = -1
-										fls.append(FeatureLocation(sc - 1, ec, strand=dir))
-									feat_loc = fls[0]
-									if len(fls) > 1:
-										feat_loc = sum(fls)
-									feature.location = feat_loc
-									sample_lts_to_add_genbank_features[scaff_id].append(feature)
-
-				bgc_prot_file = bgc_prot_directory + sample + '.faa'
-				bgc_prot_to_location = {}
-				with open(bgc_prot_file) as obpf:
-					for rec in SeqIO.parse(obpf, 'fasta'):
-						bgc_prot_to_location[rec.id] = [rec.description.split()[1],
-														int(rec.description.split()[2]),
-														int(rec.description.split()[3])]
-						if rec.id in bgc_prots_1x:
-							sample_lts_to_add_protein_sequences[rec.id] = [
-								rec.id + ' ' + rec.description.split()[1] + ' ' + str(
-									int(rec.description.split()[2]) + scaff_start) + ' ' + str(
-									int(rec.description.split()[3]) + scaff_start), str(rec.seq)]
-
-				for blt in bgc_prots_1x:
-					blt_scaff, blt_start, blt_end = bgc_prot_to_location[blt]
-					blt_range = set(range(blt_start + scaff_start, blt_end + scaff_start + 1))
-					for glt in scaff_glts[blt_scaff]:
-						glt_scaff, glt_start, glt_end = gw_prot_to_location[glt]
-						glt_range = set(range(glt_start, glt_end + 1))
-						if glt_scaff == blt_scaff and float(len(blt_range.intersection(glt_range))) / float(
-								len(glt_range)) >= 0.25:
-							if not glt in bgc_prots:
-								sample_lts_to_prune.add(glt)
+					scaff_start = None
+					with open(bgc) as obf:
+						for rec in SeqIO.parse(obf, 'genbank'):
+							scaff_id = rec.id
+							scaff_start = int(rec.description.split()[-1].strip())
+							for feature in rec.features:
+								if feature.type == 'CDS':
+									prot_lt = feature.qualifiers.get('locus_tag')[0]
+									if prot_lt in bgc_prots_1x:
+										all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
+										fls = []
+										for sc, ec, dc in all_coords:
+											dir = 1
+											if dc == '-': dir = -1
+											fls.append(FeatureLocation(sc - 1, ec, strand=dir))
+										feat_loc = fls[0]
+										if len(fls) > 1:
+											feat_loc = sum(fls)
+										feature.location = feat_loc
+										sample_lts_to_add_genbank_features[scaff_id].append(feature)
+
+					bgc_prot_file = bgc_prot_directory + sample + '.faa'
+					bgc_prot_to_location = {}
+					with open(bgc_prot_file) as obpf:
+						for rec in SeqIO.parse(obpf, 'fasta'):
+							bgc_prot_to_location[rec.id] = [rec.description.split()[1],
+															int(rec.description.split()[2]),
+															int(rec.description.split()[3])]
+							if rec.id in bgc_prots_1x:
+								sample_lts_to_add_protein_sequences[rec.id] = [
+									rec.id + ' ' + rec.description.split()[1] + ' ' + str(
+										int(rec.description.split()[2]) + scaff_start) + ' ' + str(
+										int(rec.description.split()[3]) + scaff_start), str(rec.seq)]
+
+					for blt in bgc_prots_1x:
+						blt_scaff, blt_start, blt_end = bgc_prot_to_location[blt]
+						blt_range = set(range(blt_start + scaff_start, blt_end + scaff_start + 1))
+						for glt in scaff_glts[blt_scaff]:
+							glt_scaff, glt_start, glt_end = gw_prot_to_location[glt]
+							glt_range = set(range(glt_start, glt_end + 1))
+							if glt_scaff == blt_scaff and float(len(blt_range.intersection(glt_range))) / float(
+									len(glt_range)) >= 0.25:
+								if not glt in bgc_prots:
+									sample_lts_to_prune.add(glt)
 
 			final_gw_sample_faa = final_proteomes_directory + sample + '.faa'
 			final_gw_sample_gbk = final_genbanks_directory + sample + '.gbk'
 
 			sample_listing_handle.write(sample + '\t' + final_gw_sample_gbk + '\t' + final_gw_sample_faa + '\n')
 
 			faa_handle = open(final_gw_sample_faa, 'w')
@@ -1981,28 +1984,28 @@
 			for rec in SeqIO.parse(og, 'genbank'):
 				updated_features = []
 				cds_iter = 0
 				starts = []
 				for feature in rec.features:
 					if feature.type == 'CDS':
 						prot_lt = feature.qualifiers.get('locus_tag')[0]
-						if protein_annotations == None:
+						if protein_annotations == None or (not sample in protein_annotations):
 							feature.qualifiers['product'] = 'hypothetical protein'
 						else:
 							feature.qualifiers['product'] = [protein_annotations[sample][prot_lt]]
 						feature.qualifiers.move_to_end('translation')
 						if prot_lt in sample_lts_to_prune: continue
 						updated_features.append(feature)
 						all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 						starts.append([cds_iter, start])
 						cds_iter += 1
 				for feature in sample_lts_to_add_genbank_features[rec.id]:
 					if feature.type == 'CDS':
 						prot_lt = feature.qualifiers.get('locus_tag')[0]
-						if protein_annotations == None:
+						if protein_annotations == None or (not sample in protein_annotations):
 							feature.qualifiers['product'] = 'hypothetical protein'
 						else:
 							feature.qualifiers['product'] = [protein_annotations[sample][prot_lt]]
 						feature.qualifiers.move_to_end('translation')
 						updated_features.append(feature)
 						all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 						starts.append([cds_iter, start])
```

### Comparing `lsaBGC-1.34/lsaBGC.egg-info/SOURCES.txt` & `lsaBGC-1.35/lsaBGC.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 bin/lsaBGC-Cluster.py
+bin/lsaBGC-ComprehenSeeIve.py
 bin/lsaBGC-DiscoVary.py
 bin/lsaBGC-Divergence.py
 bin/lsaBGC-Expansion.py
 bin/lsaBGC-MIBiGMapper.py
 bin/lsaBGC-PopGene.py
 bin/lsaBGC-Ready.py
 bin/lsaBGC-Refiner.py
```

### Comparing `lsaBGC-1.34/scripts/GSeeF.py` & `lsaBGC-1.35/scripts/GSeeF.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/compareBGCtoGenomeCodonUsage.py` & `lsaBGC-1.35/scripts/compareBGCtoGenomeCodonUsage.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/createPickleOfSampleAnnotationListingFile.py` & `lsaBGC-1.35/scripts/createPickleOfSampleAnnotationListingFile.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/listAllBGCGenbanksInDirectory.py` & `lsaBGC-1.35/scripts/listAllBGCGenbanksInDirectory.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/listAllGenomesInDirectory.py` & `lsaBGC-1.35/scripts/listAllGenomesInDirectory.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/popSizeAndSampleSelector.py` & `lsaBGC-1.35/scripts/popSizeAndSampleSelector.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/processAndReformatNCBIGenbanks.py` & `lsaBGC-1.35/scripts/processAndReformatNCBIGenbanks.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/readifyAdditionalGenomes.py` & `lsaBGC-1.35/scripts/readifyAdditionalGenomes.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/runProdigalAndMakeProperGenbank.py` & `lsaBGC-1.35/scripts/runProdigalAndMakeProperGenbank.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/setup_annotation_dbs.py` & `lsaBGC-1.35/scripts/setup_annotation_dbs.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/setup_bigscape.py` & `lsaBGC-1.35/scripts/setup_bigscape.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/simpleProteinExtraction.py` & `lsaBGC-1.35/scripts/simpleProteinExtraction.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.34/scripts/visualize_BGC-Ome.py` & `lsaBGC-1.35/scripts/visualize_BGC-Ome.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 	
 	- For antiSMASH predictions: Discrete. "rule-based" key domain for detection containing genes are gold, rest are grey.  
 	- For DeepBGC predictions: Continuous. score by model for BGC-likeness. 
 	- For GECCO predictions: Continuous. score by model for BGC-likeness.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
 	parser.add_argument('-b', '--bgc_results_dir', help='Sample-specific results directory from antiSMASH, DeepBGC, or GECCO.', required=True)
-	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH. Will only work for GECCO and DeepBGC if\n-l and -g arguments are used (a.k.a. in lsaBGC mode) to provide paths to genomes and BGC predictions.', default='antismash', required=False)
+	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO) [Default is antiSMASH].', default='antismash', required=False)
 	parser.add_argument('-o', '--output_pdf', help='Path to output PDF file [Default is ./Sample_BGC-ome.pdf].')
 	parser.add_argument('-t', '--tmp_dir', help='Path to temporary dir. [Default is ./tmp_dir_$INDIR_BASE_NAME].', required=False, default=None)
 	parser.add_argument('-l', '--length', type=int, help='Specify the height/length of the heatmap plot. [Default is 7].', required=False, default=7)
 	parser.add_argument('-w', '--width', type=int, help='Specify the width of the heatmap plot. [Default is 10].', required=False, default=14)
 
 	args = parser.parse_args()
 	return args
```

### Comparing `lsaBGC-1.34/setup.py` & `lsaBGC-1.35/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='lsaBGC',
-      version='1.34',
+      version='1.35',
       description='Suite for comparative genomic, population genetics and evolutionary analysis, as well as metagenomic mining of micro-evolutionary novelty in BGCs all in the context of a single lineage of interest.',
       url='http://github.com/Kalan-Lab/lsaBGC/',
       author='Rauf Salamzade',
       author_email='salamzader@gmail.com',
       license='BSD-3',
       packages=['lsaBGC'],
       scripts=['scripts/setup_annotation_dbs.py',
@@ -24,14 +24,15 @@
                'workflows/lsaBGC-Easy.py',
                'workflows/lsaBGC-Euk-Easy.py',
                'workflows/lsaBGC-AutoAnalyze.py',
                'workflows/lsaBGC-AutoExpansion.py',
                'bin/lsaBGC-Ready.py',
                'bin/lsaBGC-Cluster.py',
                'bin/lsaBGC-See.py',
+               'bin/lsaBGC-ComprehenSeeIve.py',
                'bin/lsaBGC-PopGene.py', 
                'bin/lsaBGC-Refiner.py', 
                'bin/lsaBGC-Expansion.py', 
                'bin/lsaBGC-Divergence.py', 
                'bin/lsaBGC-DiscoVary.py',
                'bin/lsaBGC-MIBiGMapper.py'],
       zip_safe=False)
```

### Comparing `lsaBGC-1.34/workflows/lsaBGC-AutoAnalyze.py` & `lsaBGC-1.35/workflows/lsaBGC-AutoAnalyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,30 +63,32 @@
 	parser = argparse.ArgumentParser(description="""
 	Program: lsaBGC-AutoAnalyze.py
 	Author: Rauf Salamzade
 	Affiliation: Kalan Lab, UW Madison, Department of Medical Microbiology and Immunology
 
 	Wrapper program to automate running lsaBGC analytical programs for each GCF. 
 	
-	Iteratively runs lsaBGC-See.py, lsaBGC-PopGene.py, lsaBGC-Divergence.py, and optionally lsaBGC-DiscoVary.py for
-	each GCF in a GCF listings directory, produced by lsaBGC-Ready, lsaBGC-Cluster, or lsaBGC-AutoExpansion.py.
+	Iteratively runs lsaBGC-See.py, lsaBGC-PopGene.py, lsaBGC-Divergence.py, lsaBGC-MIBiGMapper, lsaBGC-ComprehenSeeIve, 
+	and optionally lsaBGC-DiscoVary.py for each GCF in a GCF listings directory, produced by lsaBGC-Ready, 
+	lsaBGC-Cluster, or lsaBGC-AutoExpansion.py.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
 	parser.add_argument('-i', '--input_listing', help="Path to tab delimited file listing: (1) sample name\n(2) path to whole-genome Genbank and (3) path to whole-genome predicted proteome\n(an output of lsaBGC-Ready.py or lsaBGC-AutoExpansion.py).", required=True)
 	parser.add_argument('-g', '--gcf_listing_dir', help='Directory with GCF listing files.', required=True)
 	parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder homolog group by sample matrix.", required=True)
 	parser.add_argument('-o', '--output_directory', help="Parent output/workspace directory.", required=True)
 	parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with one sample\nid per line.", required=False, default=None)
 	parser.add_argument('-s', '--species_phylogeny', help="Path to species phylogeny. If not provided a FastANI based neighborjoining\ntree will be constructed and used.", default=None, required=False)
 	parser.add_argument('-w', '--expected_similarities', help="Path to file listing expected similarities between genomes/samples. This is\ncomputed most easily by running lsaBGC-Ready.py with '-t' specified, which will estimate\nsample to sample similarities based on alignment used to create species phylogeny.", required=True)
 	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO)\n[Default is antiSMASH].', default='antiSMASH', required=False)
 	parser.add_argument('-u', '--populations', help='Path to user defined populations/groupings file. Tab delimited with 2 columns: (1) sample name and (2) group identifier.', required=False, default=None)
 	parser.add_argument('-l', '--discovary_input_listing', help="Sequencing readsets for DiscoVary analysis. Tab delimited file listing:\n(1) sample name, (2) forward readset, (3) reverse readset for metagenomic/isolate\nsequencing data.", required=False, default=None)
 	parser.add_argument('-n', '--discovary_analysis_name', help="Identifier/name for DiscoVary. Not providing this parameter will avoid\nrunning lsaBGC-DiscoVary step.", required=False, default=None)
 	parser.add_argument('-mb', '--run_mibig_mapper', action='store_true', help="Run MIBiG mapping analysis.", default=False, required=False)
+	parser.add_argument('-ogm', '--og_orthofinder_matrix', help="The original OrthoFinder homolog group by sample matrix - prior to possible expansion.", required=False, default=None)
 	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 1].", required=False, default=1)
 
 	args = parser.parse_args()
 	return args
 
 def lsaBGC_AutoAnalyze():
 	"""
@@ -96,19 +98,19 @@
 	"""
 	PARSE REQUIRED INPUTS
 	"""
 	myargs = create_parser()
 
 	outdir = os.path.abspath(myargs.output_directory) + '/'
 	gcf_listing_dir = os.path.abspath(myargs.gcf_listing_dir) + '/'
-	original_orthofinder_matrix_file = os.path.abspath(myargs.orthofinder_matrix)
+	orthofinder_matrix_file = os.path.abspath(myargs.orthofinder_matrix)
 	input_listing_file = os.path.abspath(myargs.input_listing)
 
 	try:
-		assert(os.path.isdir(gcf_listing_dir) and os.path.isfile(original_orthofinder_matrix_file) and os.path.isfile(input_listing_file))
+		assert(os.path.isdir(gcf_listing_dir) and os.path.isfile(orthofinder_matrix_file) and os.path.isfile(input_listing_file))
 	except:
 		raise RuntimeError('Input directory with GCF listings does not exist, sample annotation file, or the OrthoFinder matrix does not exist. Exiting now ...')
 
 	all_samples = set([])
 	try:
 		with open(input_listing_file) as oilf:
 			for line in oilf:
@@ -132,15 +134,15 @@
 						assert(util.is_genbank(bgc_path))
 				gcf_listings += 1
 		assert(gcf_listings > 0)
 	except:
 		raise RuntimeError("Issue with validating at least single GCF listing file in the GCF listings directory.")
 
 	try:
-		with open(original_orthofinder_matrix_file) as omf:
+		with open(orthofinder_matrix_file) as omf:
 			for i, line in enumerate(omf):
 				line = line.strip('\n')
 				ls = line.split('\t')
 				if i == 0:
 					for samp in ls[1:]:
 						if samp != '':
 							assert(samp in all_samples)
@@ -158,16 +160,32 @@
 	bgc_prediction_software = myargs.bgc_prediction_software.upper()
 	species_phylogeny_file = myargs.species_phylogeny
 	expected_distances = myargs.expected_similarities
 	population_listing_file = myargs.populations
 	discovary_analysis_id = myargs.discovary_analysis_name
 	discovary_input_listing = myargs.discovary_input_listing
 	run_mibig_mapper = myargs.run_mibig_mapper
+	original_orthofinder_matrix_file = myargs.og_orthofinder_matrix
 	cpus = myargs.cpus
 
+	if original_orthofinder_matrix_file != None:
+		try:
+			with open(original_orthofinder_matrix_file) as omf:
+				for i, line in enumerate(omf):
+					line = line.strip('\n')
+					ls = line.split('\t')
+					if i == 0:
+						for samp in ls[1:]:
+							if samp != '':
+								assert (samp in all_samples)
+					else:
+						assert (ls[0].startswith("OG") or ls[0].startswith("HOG"))
+		except:
+			raise RuntimeError("Issue with validating the original OrthoFinder matrix is in correct format.")
+
 	try:
 		assert (bgc_prediction_software in set(['ANTISMASH', 'DEEPBGC', 'GECCO']))
 	except:
 		raise RuntimeError('BGC prediction software option is not a valid option.')
 
 	if species_phylogeny_file != None:
 		try:
@@ -221,24 +239,25 @@
 	logObject = util.createLoggerObject(log_file)
 	version_string = util.parseVersionFromSetupPy()
 	logObject.info('Running version %s' % version_string)
 
 	# Step 0: Log input arguments and update reference and query FASTA files.
 	logObject.info("Saving parameters for easier determination of results basis in the future.")
 	parameters_file = outdir + 'Parameter_Inputs.txt'
-	parameter_values = [gcf_listing_dir, input_listing_file, original_orthofinder_matrix_file, outdir,
+	parameter_values = [gcf_listing_dir, input_listing_file, orthofinder_matrix_file, outdir,
 						species_phylogeny_file, expected_distances, population_listing_file,
 						discovary_analysis_id, discovary_input_listing, bgc_prediction_software,
-						sample_set_file, run_mibig_mapper, cpus]
+						sample_set_file, run_mibig_mapper, original_orthofinder_matrix_file, cpus]
 	parameter_names = ["GCF Listings Directory", "Listing File of Sample Annotation Files for Initial Set of Samples",
 					   "OrthoFinder Homolog Matrix", "Output Directory", "Species Phylogeny File in Newick Format",
 					   "File with Expected Sample to Sample Amino Acid Distance Estimations",
 					   "Clade/Population Listings File", "DiscoVary Analysis ID",
 					   "DiscoVary Sequencing Data Location Specification File", "BGC Prediction Software",
-					   "Sample Retention Set", "Run MIBiG Mapping Analysis?", "CPUs"]
+					   "Sample Retention Set", "Run MIBiG Mapping Analysis?", "Original OrthoFinder Homolog Matrix",
+					   "CPUs"]
 	util.logParametersToFile(parameters_file, parameter_names, parameter_values)
 	logObject.info("Done saving parameters!")
 
 	# Step 0: (Optional) Parse sample set retention specifications file, if provided by the user.
 	sample_retention_set = util.getSampleRetentionSet(sample_set_file)
 
 	if sample_retention_set != None:
@@ -311,18 +330,21 @@
 		with open(population_listing_file) as oplf:
 			for line in oplf:
 				line = line.strip()
 				samp, pop = line.split('\t')
 				pop_size[pop] += 1
 
 	see_outdir = outdir + 'See/'
+	csee_outdir = outdir + 'ComprehenSeeIve/'
 	pop_outdir = outdir + 'PopGene/'
 	div_outdir = outdir + 'Divergence/'
 	mbmap_outdir = outdir + 'MIBiG_Mapping/'
 
+	if original_orthofinder_matrix_file != None:
+		if not os.path.isdir(csee_outdir): os.system('mkdir %s' % csee_outdir)
 	if not os.path.isdir(see_outdir): os.system('mkdir %s' % see_outdir)
 	if not os.path.isdir(pop_outdir): os.system('mkdir %s' % pop_outdir)
 	if not os.path.isdir(div_outdir): os.system('mkdir %s' % div_outdir)
 
 	if discovary_analysis_id and discovary_input_listing:
 		dis_outdir = outdir + 'DiscoVary_' + '_'.join(discovary_analysis_id.split()) + '/'
 		if not os.path.isdir(dis_outdir): os.system('mkdir %s' % dis_outdir)
@@ -337,15 +359,14 @@
 		gcf_samples = set([])
 		with open(gcf_listing_file) as oglf:
 			for line in oglf:
 				line = line.strip()
 				sample, bgc_gbk = line.split('\t')
 				gcf_samples.add(sample)
 
-		orthofinder_matrix_file = original_orthofinder_matrix_file
 		logObject.info("Beginning analysis for GCF %s" % gcf_id)
 		sys.stderr.write("Beginning analysis for GCF %s\n" % gcf_id)
 
 		# 1. Run lsaBGC-See.py
 		gcf_see_outdir = see_outdir + gcf_id + '/'
 		lsabgc_see_checkpoint = gcf_see_outdir + 'CHECKPOINT.txt'
 		if not os.path.isfile(lsabgc_see_checkpoint):
@@ -356,15 +377,32 @@
 				#print(' '.join(cmd))
 				util.run_cmd(cmd, logObject)
 				assert(os.path.isfile(lsabgc_see_checkpoint))
 			except Exception as e:
 				logObject.warning("lsaBGC-See.py was unsuccessful for GCF %s" % gcf_id)
 				sys.stderr.write("Warning: lsaBGC-See.py was unsuccessful for GCF %s\n" % gcf_id)
 
-		# 2. Run lsaBGC-PopGene.py
+		# 2. Run lsaBGC-ComprehenSeeIve.py
+		if original_orthofinder_matrix_file != None:
+			gcf_csee_outdir = csee_outdir + gcf_id + '/'
+			lsabgc_csee_checkpoint = gcf_csee_outdir + 'CHECKPOINT.txt'
+			if not os.path.isfile(lsabgc_csee_checkpoint):
+				os.system('rm -rf %s' % gcf_csee_outdir)
+				cmd = ['lsaBGC-ComprehenSeeIve.py', '-g', gcf_listing_file, '-m', original_orthofinder_matrix_file, '-o',
+					   gcf_csee_outdir, '-i', gcf_id, '-s', species_phylogeny_file, '-p', bgc_prediction_software, '-c',
+					   str(cpus)]
+				try:
+					#print(' '.join(cmd))
+					util.run_cmd(cmd, logObject)
+					assert(os.path.isfile(lsabgc_csee_checkpoint))
+				except Exception as e:
+					logObject.warning("lsaBGC-ComprehenSeeIve.py was unsuccessful for GCF %s" % gcf_id)
+					sys.stderr.write("Warning: lsaBGC-ComprehenSeeIve.py was unsuccessful for GCF %s\n" % gcf_id)
+
+		# 3. Run lsaBGC-PopGene.py
 		gcf_pop_outdir = pop_outdir + gcf_id + '/'
 		lsabgc_popgene_checkpoint = gcf_pop_outdir + 'CHECKPOINT.txt'
 		if not os.path.isfile(lsabgc_popgene_checkpoint):
 			os.system('rm -rf %s' % gcf_pop_outdir)
 			cmd = ['lsaBGC-PopGene.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-o', gcf_pop_outdir,
 				   '-i', gcf_id, '-p', bgc_prediction_software, '-c', str(cpus)]
 			if expected_distances != None:
@@ -375,15 +413,15 @@
 				#print(' '.join(cmd))
 				util.run_cmd(cmd, logObject, stderr=sys.stderr, stdout=sys.stdout)
 				assert(os.path.isfile(lsabgc_popgene_checkpoint))
 			except Exception as e:
 				logObject.warning("lsaBGC-PopGene.py was unsuccessful for GCF %s" % gcf_id)
 				sys.stderr.write("Warning: lsaBGC-PopGene.py was unsuccessful for GCF %s\n" % gcf_id)
 
-		# 3. Run lsaBGC-Divergence.py
+		# 4. Run lsaBGC-Divergence.py
 		gcf_div_outdir = div_outdir + gcf_id + '/'
 		lsabgc_divergence_checkpoint = gcf_div_outdir + 'CHECKPOINT.txt'
 		if (not os.path.isfile(lsabgc_divergence_checkpoint)) and expected_distances and len(gcf_samples) > 1:
 			os.system('rm -rf %s' % gcf_div_outdir)
 			cmd = ['lsaBGC-Divergence.py', '-g', gcf_listing_file, '-l', input_listing_file, '-o', gcf_div_outdir,
 				   '-i', gcf_id, '-a',	gcf_pop_outdir + 'Codon_Alignments_Listings.txt', '-c', str(cpus),'-w',
 				   expected_distances]
@@ -391,30 +429,30 @@
 				#print(' '.join(cmd))
 				util.run_cmd(cmd, logObject)
 				assert(os.path.isfile(lsabgc_divergence_checkpoint))
 			except Exception as e:
 				logObject.warning("lsaBGC-Divergence.py was unsuccessful for GCF %s" % gcf_id)
 				sys.stderr.write("Warning: lsaBGC-Divergence.py was unsuccessful for GCF %s\n" % gcf_id)
 
-		# 4. Run lsaBGC-MIBiGMapper.py
+		# 5. Run lsaBGC-MIBiGMapper.py
 		gcf_mbm_outdir = mbmap_outdir + gcf_id + '/'
 		lsabgc_mibigmap_checkpoint = gcf_mbm_outdir + 'CHECKPOINT.txt'
 		if not os.path.isfile(lsabgc_mibigmap_checkpoint) and run_mibig_mapper:
 			os.system('rm -rf %s' % gcf_mbm_outdir)
 			cmd = ['lsaBGC-MIBiGMapper.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-o', gcf_mbm_outdir,
 				   '-i', gcf_id,  '-c', str(cpus)]
 			try:
 				#print(' '.join(cmd))
 				util.run_cmd(cmd, logObject)
 				assert(os.path.isfile(lsabgc_mibigmap_checkpoint))
 			except Exception as e:
 				logObject.warning("lsaBGC-MIBiGMapper.py was unsuccessful for GCF %s" % gcf_id)
 				sys.stderr.write("Warning: lsaBGC-MIBiGMapper.py was unsuccessful for GCF %s\n" % gcf_id)
 
-		# 5. Run lsaBGC-DiscoVary.py
+		# 6. Run lsaBGC-DiscoVary.py
 		if discovary_analysis_id and discovary_input_listing:
 			gcf_dis_outdir = dis_outdir + gcf_id + '/'
 			lsabgc_discovary_checkpoint = gcf_dis_outdir + 'CHECKPOINT.txt'
 			if not os.path.isfile(lsabgc_discovary_checkpoint):
 				os.system('rm -rf %s' % gcf_dis_outdir)
 				cmd = ['lsaBGC-DiscoVary.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-o',
 					   gcf_dis_outdir, '-i', gcf_id, '-c', str(cpus), '-p', discovary_input_listing, '-a',
@@ -422,14 +460,15 @@
 				try:
 					util.run_cmd(cmd, logObject, stderr=sys.stderr, stdout=sys.stdout)
 					assert (os.path.isfile(lsabgc_discovary_checkpoint))
 				except Exception as e:
 					logObject.warning("lsaBGC-DiscoVary.py was unsuccessful for GCF %s" % gcf_id)
 					sys.stderr.write("Warning: lsaBGC-DiscoVary.py was unsuccessful for GCF %s\n" % gcf_id)
 
+
 	combined_tajimd_plot_input_file = outdir + 'Tajimas_D_Plotting_Input.txt'
 	combined_betard_plot_input_file = outdir + 'Beta-RD_Plotting_Input.txt'
 	combined_conser_plot_input_file = outdir + 'HG_Conservation_Plotting_Input.txt'
 	combined_pmcopy_plot_input_file = outdir + 'HG_Proportion_MultiCopy_Plotting_Input.txt'
 	combined_consensus_similarity_file = outdir + 'GCF_Homolog_Group_Consensus_Sequence_Similarity.txt'
 	combined_divergence_results_file = outdir + 'GCF_Divergences.txt'
 	consolidated_popgene_report_file = outdir + 'GCF_Homolog_Group_Information.txt'
@@ -666,25 +705,28 @@
 	cprf_df.to_excel(writer, sheet_name='Overview - Full', index=False, na_rep="NA")
 
 	# format overview simple sheet
 	worksheet = writer.sheets['Overview - Simple']
 	num_rows, num_cols = scprf_df.shape
 
 	warn_format = workbook.add_format({'bg_color': '#bf241f', 'bold': True, 'font_color': '#FFFFFF'})
+	core_format = workbook.add_format({'bg_color': '#606896', 'bold': True, 'font_color': '#FFFFFF'})
 	na_format = workbook.add_format({'font_color': '#a6a6a6', 'bg_color': '#FFFFFF', 'italic': True})
-	header_format = workbook.add_format(
-		{'bold': True, 'text_wrap': True, 'valign': 'top', 'fg_color': '#D7E4BC', 'border': 1})
+	header_format = workbook.add_format({'bold': True, 'text_wrap': True, 'valign': 'top', 'fg_color': '#D7E4BC', 'border': 1})
 
 	worksheet.conditional_format('A2:BA' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"NA"', 'format': na_format})
 	worksheet.conditional_format('A1:BA1', {'type': 'cell', 'criteria': '!=', 'value': 'NA', 'format': header_format})
 
 	if run_mibig_mapper:
 		# warn against non-single-copy in GCF context
 		worksheet.conditional_format('I2:I' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"False"', 'format': warn_format})
 
+		# highlight 'key' homolog groups in detection process of BGC
+		worksheet.conditional_format('K2:K' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"True"', 'format': core_format})
+
 		# prop gene-clusters with hg
 		worksheet.conditional_format('N2:N' + str(num_rows),
 								 {'type': '2_color_scale', 'min_color': "#f7de99", 'max_color': "#c29006",
 								  "min_value": 0.0, "max_value": 1.0, 'min_type': 'num', 'max_type': 'num'})
 		# gene-lengths
 		worksheet.conditional_format('J2:J' + str(num_rows),
 									 {'type': '2_color_scale', 'min_color': "#a3dee3", 'max_color': "#1ebcc9",
@@ -708,14 +750,17 @@
 									  'min_type': 'num', 'max_type': 'num', 'mid_type': 'num',
 									  'max_color': "#9eb888", "min_value": 0.75, "mid_value": 1.0, "max_value": 1.25})
 
 	else:
 		# warn against non-single-copy in GCF context
 		worksheet.conditional_format('H2:H' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"False"', 'format': warn_format})
 
+		# highlight 'key' homolog groups in detection process of BGC
+		worksheet.conditional_format('J2:J' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"True"', 'format': core_format})
+
 		# prop gene-clusters with hg
 		worksheet.conditional_format('M2:M' + str(num_rows),
 								 {'type': '2_color_scale', 'min_color': "#f7de99", 'max_color': "#c29006",
 								  "min_value": 0.0, "max_value": 1.0, 'min_type': 'num', 'max_type': 'num'})
 		# gene-lengths
 		worksheet.conditional_format('I2:I' + str(num_rows),
 									 {'type': '2_color_scale', 'min_color': "#a3dee3", 'max_color': "#1ebcc9",
@@ -755,14 +800,24 @@
 	lsabgc_see_outdir = outdir + 'See/'
 	for gcf in os.listdir(lsabgc_see_outdir):
 		see_species_pdf_result = lsabgc_see_outdir + gcf + '/BGC_Visualization.species_phylogeny.pdf'
 		if os.path.isfile(see_species_pdf_result):
 			new_name = final_results_see_dir + gcf + '.pdf'
 			os.system('cp %s %s' % (see_species_pdf_result, new_name))
 
+	if original_orthofinder_matrix_file != None:
+		final_results_csee_dir = final_results_dir + 'GCFs_across_Species_Tree_Views_from_lsaBGC-ComprehenSeeIve/'
+		util.setupReadyDirectory([final_results_csee_dir])
+		lsabgc_csee_outdir = outdir + 'ComprehenSeeIve/'
+		for gcf in os.listdir(lsabgc_csee_outdir):
+			csee_species_pdf_result = lsabgc_csee_outdir + gcf + '/BGC_Visualization.species_phylogeny.pdf'
+			if os.path.isfile(csee_species_pdf_result):
+				new_name = final_results_csee_dir + gcf + '.pdf'
+				os.system('cp %s %s' % (csee_species_pdf_result, new_name))
+
 	# Close logging object and exit
 	util.closeLoggerObject(logObject)
 	sys.exit(0)
 
 def writeToOpenHandle(gcf_results_file, combined_results_handle, include_header):
 	with open(gcf_results_file) as ogrf:
 		for i, line in enumerate(ogrf):
```

### Comparing `lsaBGC-1.34/workflows/lsaBGC-AutoExpansion.py` & `lsaBGC-1.35/workflows/lsaBGC-AutoExpansion.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,18 +302,22 @@
 
 								logObject.info("Overlap found between BGCs %s (%s) and %s (%s), %s." % (bgc1, gcf1, bgc2, gcf2, address))
 
 	# create updated general listings file
 	updated_listings_file = outdir + 'Sample_Annotation_Files.txt'
 	updated_listings_handle = open(updated_listings_file, 'w')
 	all_samples = set([])
+	primary_initial_samples = set([])
 	with open(initial_listing_file) as oilf:
 		for line in oilf:
-			all_samples.add(util.cleanUpSampleName(line.strip().split('\t')[0]))
+			cleaned_sample_name = util.cleanUpSampleName(line.strip().split('\t')[0])
+			all_samples.add(cleaned_sample_name)
+			primary_initial_samples.add(cleaned_sample_name)
 			updated_listings_handle.write(line)
+
 	with open(expansion_listing_file) as oelf:
 		for line in oelf:
 			if not util.cleanUpSampleName(line.strip().split('\t')[0]) in all_samples:
 				all_samples.add(util.cleanUpSampleName(line.strip().split('\t')[0]))
 				updated_listings_handle.write(line)
 	updated_listings_handle.close()
 
@@ -340,14 +344,15 @@
 				line = line.strip()
 				sample, bgc_gbk_path = line.split('\t')
 				if (sample_has_bgc_with_functional_core_lt[sample][gcf] == False) and (not bgc_gbk_path in original_gcfs):
 					logObject.info("GCF %s presence in sample %s disregarded, because BGC instance with functionally core homolog group was removed due to overlap with BGC from another GCF." % (gcf, sample))
 					continue
 				if (bgc_gbk_path in bgcs_to_discard) and (not bgc_gbk_path in original_gcfs): continue
 				final_expanded_gcf_listing_handle.write(line + '\n')
+				if sample in primary_initial_samples: continue
 				if bgc_gbk_path in original_gcfs: continue
 				expansion_flag = False
 				if '_Expansion_BGC' in bgc_gbk_path:
 					expansion_flag = True
 				BGC_Object = BGC(bgc_gbk_path, bgc_gbk_path, expansion_flag, prediction_method=bgc_prediction_software)
 				BGC_Object.parseGenbanks(comprehensive_parsing=False)
 				curr_bgc_lts = set(BGC_Object.gene_information.keys())
```

### Comparing `lsaBGC-1.34/workflows/lsaBGC-Easy.py` & `lsaBGC-1.35/workflows/lsaBGC-Easy.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 	parser.add_argument('-x', '--ignore_limits', action='store_true', help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
 	parser.add_argument('-gtm', '--gtotree_model', help="SCG model for secondary GToTree analysis and what would be used for dereplication. [Default is \"Bacteria\"].", default='Bacteria', required=False)
 	parser.add_argument('-iib', '--include_incomplete_bgcs', action='store_true', help="Whether to account for incomplete BGCs (those near contig edges) prior to clustering.", default=False, required=False)
 	parser.add_argument('-b', '--use_bigscape', action='store_true', help="Use BiG-SCAPE for BGC clustering into GCFs instead of lsaBGC-Cluster. Recommended if\nyou want to include incomplete BGCs for clustering and are using antiSMASH.", required=False, default=False)
 	parser.add_argument('-lci', '--lsabgc_cluster_inflation', type=float, help='Value for MCL inflation parameter to use in lsaBGC-Cluster [Default is 4.0].', required=False, default=4.0)
 	parser.add_argument('-lcj', '--lsabgc_cluster_jaccard', type=float, help='Minimal Jaccard Index cutoff to regard two BGCs as potentially homologous\nin lsaBGC-Cluster [Default is 20.0].', required=False, default=20.0)
 	parser.add_argument('-lcr', '--lsabgc_cluster_synteny', type=float, help='Minimal absolute correlation coefficient to measure syntenic similarity and\nregard two BGCs as potentially homologous in lsaBGC-Cluster [Default is 0.7].', required=False, default=0.7)
-	parser.add_argument('-sae', '--skip_auto_expansion', action='store_true', help="Skip lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly fragmentation.", required=False, default=False)
+	parser.add_argument('-pae', '--perform_auto_expansion', action='store_true', help="Perform lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly\nfragmentation. Will increase sensitivity at the potential cost of false positives, recommended for\ntaxa with <10 BGCs per genome or more constrained lineages/species. For genus-wide analyses,\nespecially of BGC-rich organisms, please use expansion manually and assess lsaBGC-See reports\nto filter false positives.", required=False, default=False)
 	parser.add_argument('-sd', '--skip_dereplication', action='store_true', help="Whether to skip dereplication based on GToTree alignments of SCGs - not\nrecommended and can cause issues if there are a lot of\ngenomes for the taxa of interest.", default=False, required=False)
 	parser.add_argument('-dt', '--dereplicate_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as redundant [Default is 0.999].", default=0.999, required=False)
 	parser.add_argument('-pt', '--population_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as belonging to the same population [Default is 0.99].", default=0.99, required=False)
 	parser.add_argument('-py', '--use_pyrodigal', action='store_true', help='Use pyrodigal instead of prodigal.', required=False, default=False)
 	parser.add_argument('-om', '--orthofinder_mode', help="Method for running OrthoFinder2. (Options: Genome_Wide, BGC_Only).\nBGC_Only is experimental but much faster and should work especially well for\ntaxa with many BGCs [Default is Genome_Wide].", default='Genome_Wide', required=False)
 	parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true', help='Use coarse clustering of homolog groups in OrthoFinder instead of more\nresolute hierarchical determined homolog groups. There are some advantages to coarse\nOGs, including their construction being deterministic.', required=False, default=False)
 	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 4].", required=False, default=4)
@@ -129,15 +129,15 @@
 	cpus = myargs.cpus
 	bgc_prediction_cpus = myargs.antismash_prediction_cpus
 	user_genomes_directory = myargs.user_genomes_directory
 	bgc_prediction_software = myargs.bgc_prediction_software.upper()
 	gtotree_model = myargs.gtotree_model
 	skip_dereplication_flag = myargs.skip_dereplication
 	include_incomplete_bgcs_flag = myargs.include_incomplete_bgcs
-	skip_auto_expansion_flag = myargs.skip_auto_expansion
+	perform_auto_expansion_flag = myargs.perform_auto_expansion
 	dereplicate_threshold = myargs.dereplicate_threshold
 	population_threshold = myargs.population_threshold
 	run_coarse_orthofinder = myargs.run_coarse_orthofinder
 	orthofinder_mode = myargs.orthofinder_mode.upper()
 	use_bigscape_flag = myargs.use_bigscape
 	ignore_limits_flag = myargs.ignore_limits
 	use_pyrodigal = myargs.use_pyrodigal
@@ -623,34 +623,34 @@
 		if os.path.isfile(db_listing_file):
 			lsabgc_ready_cmd += ['-a']
 		runCmdViaSubprocess(lsabgc_ready_cmd, logObject,
 							check_directories=[lsabgc_ready_results_directory, gcf_listing_dir],
 							check_files=[annotation_listing_file, orthogroups_matrix_file])
 
 	# Step 6: Run lsaBGC-AutoExpansion.py polishing to find GCF instances fragmented on multiple scaffolds
-	if not skip_auto_expansion_flag:
-		logObject.info('\n--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances from completed instances using lsaBGC-AutoExpansion.')
-		sys.stdout.write('--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances from completed instances using lsaBGC-AutoExpansion.\n')
+	if perform_auto_expansion_flag:
+		logObject.info('\n--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances using completed instances as references with lsaBGC-AutoExpansion.')
+		sys.stdout.write('--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances using completed instances as references with lsaBGC-AutoExpansion.\n')
 
 	checkLsaBGCInputsExist(annotation_listing_file, gcf_listing_dir, orthogroups_matrix_file)
 
 	lsabgc_autoexpansion_results_directory = outdir + 'lsaBGC_AutoExpansion_Results/'
 	exp_annotation_listing_file = lsabgc_autoexpansion_results_directory + 'Sample_Annotation_Files.txt'
 	exp_orthogroups_matrix_file = lsabgc_autoexpansion_results_directory + 'Orthogroups.expanded.tsv'
 	exp_gcf_listing_dir = lsabgc_autoexpansion_results_directory + 'Updated_GCF_Listings/'
 
-	if not os.path.isdir(exp_gcf_listing_dir) and (not skip_auto_expansion_flag):
+	if not os.path.isdir(exp_gcf_listing_dir) and perform_auto_expansion_flag:
 		lsabgc_expansion_cmd = ['lsaBGC-AutoExpansion.py', '-g', gcf_listing_dir, '-m', orthogroups_matrix_file, '-l',
 								annotation_listing_file, '-e', annotation_listing_file, '-q', '-c', str(cpus),
 								'-o', lsabgc_autoexpansion_results_directory, '-p', bgc_prediction_software]
 		runCmdViaSubprocess(lsabgc_expansion_cmd, logObject,
 							check_directories=[lsabgc_autoexpansion_results_directory, exp_gcf_listing_dir],
 							check_files=[exp_orthogroups_matrix_file, exp_orthogroups_matrix_file])
 
-	if skip_auto_expansion_flag:
+	if not perform_auto_expansion_flag:
 		exp_annotation_listing_file = annotation_listing_file
 		exp_orthogroups_matrix_file = orthogroups_matrix_file
 		exp_gcf_listing_dir = gcf_listing_dir
 
 	# Step 7: Run lsaBGC-AutoAnalyze.py
 	logObject.info('\n--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoAnalyze (which runs lsaBGC-See.py, lsaBGC-PopGene.py, and lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
 	sys.stdout.write('--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoAnalyze (which runs lsaBGC-See.py, lsaBGC-PopGene.py,\nand lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
@@ -665,15 +665,16 @@
 	lsabgc_autoanalyze_dir = outdir + 'lsaBGC_AutoAnalyze_Results/'
 	lsabgc_autoanalyze_results_dir = lsabgc_autoanalyze_dir + 'Final_Results/'
 	if not os.path.isdir(lsabgc_autoanalyze_results_dir):
 		os.system('rm -rf %s' % lsabgc_autoanalyze_dir)
 		lsabgc_autoanalyze_cmd = ['lsaBGC-AutoAnalyze.py', '-i', exp_annotation_listing_file, '-g', exp_gcf_listing_dir,
 								  '-mb', '-m', exp_orthogroups_matrix_file, '-s', species_tree_file, '-w',
 								  expected_similarities_file, '-k', samples_to_keep_file, '-c', str(cpus), '-o',
-								  lsabgc_autoanalyze_dir, '-p', bgc_prediction_software, '-u', population_file]
+								  lsabgc_autoanalyze_dir, '-p', bgc_prediction_software, '-u', population_file,
+								  '-ogm', orthogroups_matrix_file]
 		runCmdViaSubprocess(lsabgc_autoanalyze_cmd, logObject, check_directories=[lsabgc_autoanalyze_results_dir])
 
 
 	# Step 8: Run lsaBGC-AutoAnalyze.py
 	logObject.info('\n--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
 	sys.stdout.write('--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
```

### Comparing `lsaBGC-1.34/workflows/lsaBGC-Euk-Easy.py` & `lsaBGC-1.35/workflows/lsaBGC-Euk-Easy.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 	parser.add_argument('-o', '--output_directory', help='Parent output/workspace directory.', required=True)
 	parser.add_argument('-x', '--ignore_limits', action='store_true', help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
 	parser.add_argument('-iib', '--include_incomplete_bgcs', action='store_true', help="Whether to account for incomplete BGCs prior to clustering -\nnot recommended.", default=False, required=False)
 	parser.add_argument('-b', '--use_bigscape', action='store_true', help="Use BiG-SCAPE for BGC clustering into GCFs instead of lsaBGC-Cluster.\nRecommended if you want to include incomplete BGCs for clustering and are using\nantiSMASH.", required=False, default=False)
 	parser.add_argument('-lci', '--lsabgc_cluster_inflation', type=float, help='Value for MCL inflation parameter to use in lsaBGC-Cluster [Default is 4.0].', required=False, default=4.0)
 	parser.add_argument('-lcj', '--lsabgc_cluster_jaccard', type=float, help='Minimal Jaccard Index cutoff to regard two BGCs as potentially homologous\nin lsaBGC-Cluster [Default is 20.0].', required=False, default=20.0)
 	parser.add_argument('-lcr', '--lsabgc_cluster_synteny', type=float, help='Minimal absolute correlation coefficient to measure syntenic similarity and\nregard two BGCs as potentially homologous in lsaBGC-Cluster [Default is 0.7].', required=False, default=0.7)
-	parser.add_argument('-sae', '--skip_auto_expansion', action='store_true', help="Skip lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly\nfragmentation.", required=False, default=False)
+	parser.add_argument('-pae', '--perform_auto_expansion', action='store_true', help="Perform lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly\nfragmentation. Will increase sensitivity at the potential cost of false positives, recommended for\ntaxa with <10 BGCs per genome or more constrained lineages/species. For genus-wide analyses,\nespecially of BGC-rich organisms, please use expansion manually and assess lsaBGC-See reports\nto filter false positives.", required=False, default=False)
 	parser.add_argument('-dt', '--dereplicate_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as redundant [Default is 0.999].", default=0.999, required=False)
 	parser.add_argument('-sd', '--skip_dereplication', action='store_true', help="Whether to skip dereplication based on GToTree alignments of SCGs - not\nrecommended and can cause issues if there are a lot of genomes for the taxa\nof interest.", default=False, required=False)
 	parser.add_argument('-pt', '--population_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as belonging to the same population [Default is 0.99].", default=0.99, required=False)
 	parser.add_argument('-om', '--orthofinder_mode', help="Method for running OrthoFinder2. (Options: Genome_Wide, BGC_Only).\nDefault is Genome_Wide (BGC_Only is slightly experimental but much faster and should work\nespecially well for taxa with many BGCs).", default='Genome_Wide', required=False)
 	parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true', help='Use coarse clustering of homolog groups in OrthoFinder instead\nof more resolute hierarchical determined homolog groups. There are some advantages to\ncoarse OGs, including their construction being deterministic.', required=False, default=False)
 	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 4].", required=False, default=4)
 	parser.add_argument('-a', '--antismash_prediction_cpus', type=int, help="Number of CPUs to specify for each antiSMASH command in\ntask file [Default is 4].", required=False, default=4)
@@ -113,15 +113,15 @@
 
 	outdir = os.path.abspath(myargs.output_directory) + '/'
 	cpus = myargs.cpus
 	bgc_prediction_cpus = myargs.antismash_prediction_cpus
 	genomes_directory = myargs.genomes_directory
 	skip_dereplication_flag = myargs.skip_dereplication
 	include_incomplete_bgcs_flag = myargs.include_incomplete_bgcs
-	skip_auto_expansion_flag = myargs.skip_auto_expansion
+	perform_auto_expansion_flag = myargs.perform_auto_expansion
 	dereplicate_threshold = myargs.dereplicate_threshold
 	population_threshold = myargs.population_threshold
 	run_coarse_orthofinder = myargs.run_coarse_orthofinder
 	orthofinder_mode = myargs.orthofinder_mode.upper()
 	use_bigscape_flag = myargs.use_bigscape
 	ignore_limits_flag = myargs.ignore_limits
 	lsabgc_cluster_inflation = myargs.lsabgc_cluster_inflation
@@ -520,34 +520,34 @@
 		if os.path.isfile(db_listing_file):
 			lsabgc_ready_cmd += ['-a']
 		runCmdViaSubprocess(lsabgc_ready_cmd, logObject,
 							check_directories=[lsabgc_ready_results_directory, gcf_listing_dir],
 							check_files=[annotation_listing_file, orthogroups_matrix_file])
 
 	# Step 6: Run lsaBGC-AutoExpansion.py polishing to find GCF instances fragmented on multiple scaffolds
-	if not skip_auto_expansion_flag:
-		logObject.info('\n--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances from completed instances using lsaBGC-AutoExpansion.')
-		sys.stdout.write('--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances from completed instances using lsaBGC-AutoExpansion.\n')
+	if perform_auto_expansion_flag:
+		logObject.info('\n--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances using completed instances as references with lsaBGC-AutoExpansion.')
+		sys.stdout.write('--------------------\nStep 6\n--------------------\nBeginning identification of fragmented BGC instances using completed instances as references with lsaBGC-AutoExpansion.\n')
 
 	checkLsaBGCInputsExist(annotation_listing_file, gcf_listing_dir, orthogroups_matrix_file)
 
 	lsabgc_autoexpansion_results_directory = outdir + 'lsaBGC_AutoExpansion_Results/'
 	exp_annotation_listing_file = lsabgc_autoexpansion_results_directory + 'Sample_Annotation_Files.txt'
 	exp_orthogroups_matrix_file = lsabgc_autoexpansion_results_directory + 'Orthogroups.expanded.tsv'
 	exp_gcf_listing_dir = lsabgc_autoexpansion_results_directory + 'Updated_GCF_Listings/'
 
-	if not os.path.isdir(exp_gcf_listing_dir) and (not skip_auto_expansion_flag):
+	if not os.path.isdir(exp_gcf_listing_dir) and perform_auto_expansion_flag:
 		lsabgc_expansion_cmd = ['lsaBGC-AutoExpansion.py', '-g', gcf_listing_dir, '-m', orthogroups_matrix_file, '-l',
 								annotation_listing_file, '-e', annotation_listing_file, '-q', '-c', str(cpus),
 								'-o', lsabgc_autoexpansion_results_directory, '-p', 'antiSMASH']
 		runCmdViaSubprocess(lsabgc_expansion_cmd, logObject,
 							check_directories=[lsabgc_autoexpansion_results_directory, exp_gcf_listing_dir],
 							check_files=[exp_orthogroups_matrix_file, exp_orthogroups_matrix_file])
 
-	if skip_auto_expansion_flag:
+	if not perform_auto_expansion_flag:
 		exp_annotation_listing_file = annotation_listing_file
 		exp_orthogroups_matrix_file = orthogroups_matrix_file
 		exp_gcf_listing_dir = gcf_listing_dir
 
 	# Step 7: Run lsaBGC-AutoAnalyze.py
 	logObject.info('\n--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoAnalyze (which runs lsaBGC-See.py, lsaBGC-PopGene.py, and lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
 	sys.stdout.write('--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoAnalyze (which runs lsaBGC-See.py, lsaBGC-PopGene.py,\nand lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
@@ -562,15 +562,16 @@
 	lsabgc_autoanalyze_dir = outdir + 'lsaBGC_AutoAnalyze_Results/'
 	lsabgc_autoanalyze_results_dir = lsabgc_autoanalyze_dir + 'Final_Results/'
 	if not os.path.isdir(lsabgc_autoanalyze_results_dir):
 		os.system('rm -rf %s' % lsabgc_autoanalyze_dir)
 		lsabgc_autoanalyze_cmd = ['lsaBGC-AutoAnalyze.py', '-i', exp_annotation_listing_file, '-g', exp_gcf_listing_dir,
 								  '-m', exp_orthogroups_matrix_file, '-mb', '-s', species_tree_file, '-w',
 								  expected_similarities_file, '-k', samples_to_keep_file, '-c', str(cpus), '-o',
-								  lsabgc_autoanalyze_dir, '-p', 'antiSMASH', '-u', population_file]
+								  lsabgc_autoanalyze_dir, '-p', 'antiSMASH', '-u', population_file,
+								  '-ogm', orthogroups_matrix_file]
 		runCmdViaSubprocess(lsabgc_autoanalyze_cmd, logObject, check_directories=[lsabgc_autoanalyze_results_dir])
 
 
 	# Step 8: Run lsaBGC-AutoAnalyze.py
 	logObject.info('\n--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
 	sys.stdout.write('--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
```

