# Comparing `tmp/wildlife-datasets-0.3.0.tar.gz` & `tmp/wildlife-datasets-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-4mbp8rt0/wildlife-datasets-0.3.0.tar", last modified: Mon Mar 20 09:44:21 2023, max compression
+gzip compressed data, was "/home/adamluk3/Projects/wildlife-datasets/dist/.tmp-63zv2_bj/wildlife-datasets-0.3.1.tar", last modified: Mon Apr 17 12:30:40 2023, max compression
```

## Comparing `wildlife-datasets-0.3.0.tar` & `wildlife-datasets-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.499507 wildlife-datasets-0.3.0/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.0/LICENSE
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     4992 2023-03-20 09:45:08.497886 wildlife-datasets-0.3.0/PKG-INFO
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2858 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.0/README.md
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-03-20 09:43:59.000000 wildlife-datasets-0.3.0/pyproject.toml
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-03-20 09:45:08.500972 wildlife-datasets-0.3.0/setup.cfg
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.364617 wildlife-datasets-0.3.0/wildlife_datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.0/wildlife_datasets/__init__.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.403797 wildlife-datasets-0.3.0/wildlife_datasets/analysis/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.0/wildlife_datasets/analysis/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.0/wildlife_datasets/analysis/plots.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.0/wildlife_datasets/analysis/statistics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.429878 wildlife-datasets-0.3.0/wildlife_datasets/datasets/
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.0/wildlife_datasets/datasets/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    49850 2023-03-17 16:59:05.000000 wildlife-datasets-0.3.0/wildlife_datasets/datasets/datasets.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.0/wildlife_datasets/datasets/metadata.csv
--rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.0/wildlife_datasets/datasets/metadata.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.0/wildlife_datasets/datasets/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.444658 wildlife-datasets-0.3.0/wildlife_datasets/downloads/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.0/wildlife_datasets/downloads/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)    24699 2023-03-17 16:06:21.000000 wildlife-datasets-0.3.0/wildlife_datasets/downloads/downloads.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.0/wildlife_datasets/downloads/utils.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.454638 wildlife-datasets-0.3.0/wildlife_datasets/loader/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.0/wildlife_datasets/loader/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.0/wildlife_datasets/loader/loader.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.464066 wildlife-datasets-0.3.0/wildlife_datasets/metrics/
--rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.0/wildlife_datasets/metrics/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     3269 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.0/wildlife_datasets/metrics/metrics.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.492582 wildlife-datasets-0.3.0/wildlife_datasets/splits/
--rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-03-15 15:44:44.000000 wildlife-datasets-0.3.0/wildlife_datasets/splits/__init__.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.0/wildlife_datasets/splits/analysis.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     5840 2023-02-28 09:08:53.000000 wildlife-datasets-0.3.0/wildlife_datasets/splits/balanced_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     6438 2023-02-15 11:54:05.000000 wildlife-datasets-0.3.0/wildlife_datasets/splits/identity_split.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.0/wildlife_datasets/splits/lcg.py
--rw-r--r--   0 adamluk3 (436797) ai         (501)     6571 2023-03-20 09:06:59.000000 wildlife-datasets-0.3.0/wildlife_datasets/splits/time_aware_split.py
-drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-03-20 09:45:08.388385 wildlife-datasets-0.3.0/wildlife_datasets.egg-info/
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     4992 2023-03-20 09:45:08.000000 wildlife-datasets-0.3.0/wildlife_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-03-20 09:45:08.000000 wildlife-datasets-0.3.0/wildlife_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-03-20 09:45:08.000000 wildlife-datasets-0.3.0/wildlife_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-03-20 09:45:08.000000 wildlife-datasets-0.3.0/wildlife_datasets.egg-info/requires.txt
--rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-03-20 09:45:08.000000 wildlife-datasets-0.3.0/wildlife_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.420299 wildlife-datasets-0.3.1/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1090 2023-02-15 08:36:46.000000 wildlife-datasets-0.3.1/LICENSE
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     5211 2023-04-17 12:31:37.418565 wildlife-datasets-0.3.1/PKG-INFO
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     3077 2023-04-17 10:03:35.000000 wildlife-datasets-0.3.1/README.md
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1645 2023-04-17 12:31:14.000000 wildlife-datasets-0.3.1/pyproject.toml
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       38 2023-04-17 12:31:37.421684 wildlife-datasets-0.3.1/setup.cfg
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.295062 wildlife-datasets-0.3.1/wildlife_datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      133 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.1/wildlife_datasets/__init__.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.330529 wildlife-datasets-0.3.1/wildlife_datasets/analysis/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      107 2023-02-14 10:36:30.000000 wildlife-datasets-0.3.1/wildlife_datasets/analysis/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     5059 2023-03-06 09:03:18.000000 wildlife-datasets-0.3.1/wildlife_datasets/analysis/plots.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2698 2023-02-28 08:53:31.000000 wildlife-datasets-0.3.1/wildlife_datasets/analysis/statistics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.353342 wildlife-datasets-0.3.1/wildlife_datasets/datasets/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2784 2023-03-17 15:45:48.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    49821 2023-04-17 12:03:18.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/datasets.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     8059 2023-03-17 12:53:50.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.csv
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      822 2023-02-14 14:45:05.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2843 2023-02-10 15:33:13.000000 wildlife-datasets-0.3.1/wildlife_datasets/datasets/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.367023 wildlife-datasets-0.3.1/wildlife_datasets/downloads/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       25 2023-03-11 08:49:06.000000 wildlife-datasets-0.3.1/wildlife_datasets/downloads/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    24699 2023-03-17 16:06:21.000000 wildlife-datasets-0.3.1/wildlife_datasets/downloads/downloads.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1495 2023-03-16 15:44:33.000000 wildlife-datasets-0.3.1/wildlife_datasets/downloads/utils.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.376419 wildlife-datasets-0.3.1/wildlife_datasets/loader/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       22 2023-02-14 10:26:57.000000 wildlife-datasets-0.3.1/wildlife_datasets/loader/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2958 2023-03-16 15:27:00.000000 wildlife-datasets-0.3.1/wildlife_datasets/loader/loader.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.385221 wildlife-datasets-0.3.1/wildlife_datasets/metrics/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)       23 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.1/wildlife_datasets/metrics/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     3269 2023-03-13 14:02:14.000000 wildlife-datasets-0.3.1/wildlife_datasets/metrics/metrics.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.412327 wildlife-datasets-0.3.1/wildlife_datasets/splits/
+-rw-r--r--   0 adamluk3 (436797) ai         (501)      191 2023-03-15 15:44:44.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/__init__.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     2653 2023-03-07 14:12:11.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/analysis.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1896 2023-04-17 11:37:36.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/balanced_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)    11625 2023-04-17 12:28:07.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/identity_split.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     1753 2023-03-07 14:02:45.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/lcg.py
+-rw-r--r--   0 adamluk3 (436797) ai         (501)     9516 2023-04-17 12:29:03.000000 wildlife-datasets-0.3.1/wildlife_datasets/splits/time_aware_split.py
+drwxrwxr-x   0 adamluk3 (436797) ai         (501)        0 2023-04-17 12:31:37.317283 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     5211 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)     1077 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)        1 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)      130 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/requires.txt
+-rw-rw-r--   0 adamluk3 (436797) ai         (501)       18 2023-04-17 12:31:37.000000 wildlife-datasets-0.3.1/wildlife_datasets.egg-info/top_level.txt
```

### Comparing `wildlife-datasets-0.3.0/LICENSE` & `wildlife-datasets-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/PKG-INFO` & `wildlife-datasets-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildlife-datasets
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for easier access and research of wildlife re-identification datasets
 Author-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 Maintainer-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 License: MIT License
         
         Copyright (c) 2023 Lukáš Adam and Vojtěch Čermák
         
@@ -37,18 +37,19 @@
 License-File: LICENSE
 
 # Wildlife Re-Identification (Re-ID) Datasets
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/WildlifeDatasets/wildlife-datasets/blob/main/LICENSE)
 [![](https://img.shields.io/badge/docs-stable-blue.svg)](https://wildlifedatasets.github.io/wildlife-datasets/)
 
-This package provides:
+The aim of the project is to provide comprehensive overview of datasets for wildlife individual re-identification and an easy-to-use package for developers of machine learning methods. The core functionality includes:
+
 - overview of 31 publicly available wildlife re-identification datasets.
 - utilities to mass download and convert them into a unified format.
-- splitting functions for closed-set and open-set classification.
+- default splits for several machine learning tasks including the ability create additional splits.
 - evaluation metrics for closed-set and open-set classification.
 
 
 ## Summary of datasets
 
 The package is able to handle the following datasets. We include basic characteristics such as publication years, number of images, number of individuals, dataset time span (difference between the last and first image taken) and additional information such as source, number of poses, inclusion of timestamps, whether the animals were captured in the wild and whether the dataset contain multiple species.
 
@@ -68,15 +69,15 @@
 ## Basic functionality
 
 We show an example of downloading, extracting and processing the MacaqueFaces dataset.
 
 ```
 from wildlife_datasets import analysis, datasets
 
-datasets.MacaqueFaces.download().get_data('data')
+datasets.MacaqueFaces.get_data('data')
 dataset = datasets.MacaqueFaces('data/MacaqueFaces')
 ```
 
 The class `dataset` contains the summary of the dataset. The content depends on the dataset. Each dataset contains the identity and paths to images. This particular dataset also contains information about the date taken and contrast. Other datasets store information about bounding boxes, segmentation masks, position from which the image was taken, keypoints or various other information such as age or gender.
 
 ```
 dataset.df
```

### Comparing `wildlife-datasets-0.3.0/README.md` & `wildlife-datasets-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Wildlife Re-Identification (Re-ID) Datasets
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/WildlifeDatasets/wildlife-datasets/blob/main/LICENSE)
 [![](https://img.shields.io/badge/docs-stable-blue.svg)](https://wildlifedatasets.github.io/wildlife-datasets/)
 
-This package provides:
+The aim of the project is to provide comprehensive overview of datasets for wildlife individual re-identification and an easy-to-use package for developers of machine learning methods. The core functionality includes:
+
 - overview of 31 publicly available wildlife re-identification datasets.
 - utilities to mass download and convert them into a unified format.
-- splitting functions for closed-set and open-set classification.
+- default splits for several machine learning tasks including the ability create additional splits.
 - evaluation metrics for closed-set and open-set classification.
 
 
 ## Summary of datasets
 
 The package is able to handle the following datasets. We include basic characteristics such as publication years, number of images, number of individuals, dataset time span (difference between the last and first image taken) and additional information such as source, number of poses, inclusion of timestamps, whether the animals were captured in the wild and whether the dataset contain multiple species.
 
@@ -30,15 +31,15 @@
 ## Basic functionality
 
 We show an example of downloading, extracting and processing the MacaqueFaces dataset.
 
 ```
 from wildlife_datasets import analysis, datasets
 
-datasets.MacaqueFaces.download().get_data('data')
+datasets.MacaqueFaces.get_data('data')
 dataset = datasets.MacaqueFaces('data/MacaqueFaces')
 ```
 
 The class `dataset` contains the summary of the dataset. The content depends on the dataset. Each dataset contains the identity and paths to images. This particular dataset also contains information about the date taken and contrast. Other datasets store information about bounding boxes, segmentation masks, position from which the image was taken, keypoints or various other information such as age or gender.
 
 ```
 dataset.df
```

### Comparing `wildlife-datasets-0.3.0/pyproject.toml` & `wildlife-datasets-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wildlife-datasets"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
 ]
 maintainers = [
   { name="Lukáš Adam", email="lukas.adam.cr@gmail.com" },
   { name="Vojtěch Čermák", email="cermak.vojtech@seznam.cz" },
```

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/analysis/plots.py` & `wildlife-datasets-0.3.1/wildlife_datasets/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/analysis/statistics.py` & `wildlife-datasets-0.3.1/wildlife_datasets/analysis/statistics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/datasets/__init__.py` & `wildlife-datasets-0.3.1/wildlife_datasets/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/datasets/datasets.py` & `wildlife-datasets-0.3.1/wildlife_datasets/datasets/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,36 +68,37 @@
 
         raise NotImplementedError('Needs to be implemented by subclasses.')
     
     def add_splits(self) -> None:
         """Drops existing splits and adds automatically generated split.
 
         The split ignores individuals named `self.unknown_name`.
-        Some rows will not belong to a split.
+        These rows will not belong to a split.
         The added split is machine-independent.
         It is the closed-set (random) split with 80% in the training set.
         """
+
         # Drop already existing splits
         cols_to_drop = ['split', 'reid_split', 'segmentation_split']
         self.df = self.df.drop(cols_to_drop, axis=1, errors='ignore')
         
-        # Add the deafult split
-        splitter = splits.ClosedSetSplit(self.df, identity_skip=self.unknown_name)
-        self.add_split(3, 'split', splitter, 0.8)
+        # Add the default split
+        splitter = splits.ClosedSetSplit(0.8, identity_skip=self.unknown_name)
+        self.add_split(3, 'split', splitter)
 
-    def add_split(self, position: int, col_name: str, splitter: splits.BalancedSplit, *args, **kwargs) -> None:       
+    def add_split(self, position: int, col_name: str, splitter: splits.BalancedSplit) -> None:       
         """Adds a split to the column named col_name.
 
         Args:
             position (int): Where the split should be placed.
             col_name (str): Name of the column.
             splitter (splits.BalancedSplit): Any class with `split` method
                 returning training and testing set indices.                
         """
-        idx_train, idx_test = splitter.split(*args, **kwargs)
+        idx_train, idx_test = splitter.split(self.df)[0]
         add = {}
         for i in idx_train:
             add[i] = 'train'
         for i in idx_test:
             add[i] = 'test'
         n_col = min(position, len(self.df.columns))
         self.df.insert(n_col, col_name, pd.Series(add))
```

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/datasets/metadata.csv` & `wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.csv`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/datasets/metadata.py` & `wildlife-datasets-0.3.1/wildlife_datasets/datasets/metadata.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/datasets/utils.py` & `wildlife-datasets-0.3.1/wildlife_datasets/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/downloads/downloads.py` & `wildlife-datasets-0.3.1/wildlife_datasets/downloads/downloads.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/downloads/utils.py` & `wildlife-datasets-0.3.1/wildlife_datasets/downloads/utils.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/loader/loader.py` & `wildlife-datasets-0.3.1/wildlife_datasets/loader/loader.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/metrics/metrics.py` & `wildlife-datasets-0.3.1/wildlife_datasets/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/splits/analysis.py` & `wildlife-datasets-0.3.1/wildlife_datasets/splits/analysis.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets/splits/lcg.py` & `wildlife-datasets-0.3.1/wildlife_datasets/splits/lcg.py`

 * *Files identical despite different names*

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets.egg-info/PKG-INFO` & `wildlife-datasets-0.3.1/wildlife_datasets.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wildlife-datasets
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library for easier access and research of wildlife re-identification datasets
 Author-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 Maintainer-email: Lukáš Adam <lukas.adam.cr@gmail.com>, Vojtěch Čermák <cermak.vojtech@seznam.cz>
 License: MIT License
         
         Copyright (c) 2023 Lukáš Adam and Vojtěch Čermák
         
@@ -37,18 +37,19 @@
 License-File: LICENSE
 
 # Wildlife Re-Identification (Re-ID) Datasets
 
 [![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/WildlifeDatasets/wildlife-datasets/blob/main/LICENSE)
 [![](https://img.shields.io/badge/docs-stable-blue.svg)](https://wildlifedatasets.github.io/wildlife-datasets/)
 
-This package provides:
+The aim of the project is to provide comprehensive overview of datasets for wildlife individual re-identification and an easy-to-use package for developers of machine learning methods. The core functionality includes:
+
 - overview of 31 publicly available wildlife re-identification datasets.
 - utilities to mass download and convert them into a unified format.
-- splitting functions for closed-set and open-set classification.
+- default splits for several machine learning tasks including the ability create additional splits.
 - evaluation metrics for closed-set and open-set classification.
 
 
 ## Summary of datasets
 
 The package is able to handle the following datasets. We include basic characteristics such as publication years, number of images, number of individuals, dataset time span (difference between the last and first image taken) and additional information such as source, number of poses, inclusion of timestamps, whether the animals were captured in the wild and whether the dataset contain multiple species.
 
@@ -68,15 +69,15 @@
 ## Basic functionality
 
 We show an example of downloading, extracting and processing the MacaqueFaces dataset.
 
 ```
 from wildlife_datasets import analysis, datasets
 
-datasets.MacaqueFaces.download().get_data('data')
+datasets.MacaqueFaces.get_data('data')
 dataset = datasets.MacaqueFaces('data/MacaqueFaces')
 ```
 
 The class `dataset` contains the summary of the dataset. The content depends on the dataset. Each dataset contains the identity and paths to images. This particular dataset also contains information about the date taken and contrast. Other datasets store information about bounding boxes, segmentation masks, position from which the image was taken, keypoints or various other information such as age or gender.
 
 ```
 dataset.df
```

### Comparing `wildlife-datasets-0.3.0/wildlife_datasets.egg-info/SOURCES.txt` & `wildlife-datasets-0.3.1/wildlife_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

