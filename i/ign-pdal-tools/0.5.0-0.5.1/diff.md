# Comparing `tmp/ign-pdal-tools-0.5.0.tar.gz` & `tmp/ign-pdal-tools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-pdal-tools-0.5.0.tar", last modified: Mon Apr  3 06:54:00 2023, max compression
+gzip compressed data, was "ign-pdal-tools-0.5.1.tar", last modified: Mon Apr 17 16:03:29 2023, max compression
```

## Comparing `ign-pdal-tools-0.5.0.tar` & `ign-pdal-tools-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-03 06:54:00.431112 ign-pdal-tools-0.5.0/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2427 2023-04-03 06:54:00.431112 ign-pdal-tools-0.5.0/PKG-INFO
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2208 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/README.md
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-03 06:54:00.423112 ign-pdal-tools-0.5.0/ign_pdal_tools.egg-info/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2427 2023-04-03 06:54:00.000000 ign-pdal-tools-0.5.0/ign_pdal_tools.egg-info/PKG-INFO
--rw-r--r--   0 LVauchier (24820) usernis  (10000)      632 2023-04-03 06:54:00.000000 ign-pdal-tools-0.5.0/ign_pdal_tools.egg-info/SOURCES.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)        1 2023-04-03 06:54:00.000000 ign-pdal-tools-0.5.0/ign_pdal_tools.egg-info/dependency_links.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)       10 2023-04-03 06:54:00.000000 ign-pdal-tools-0.5.0/ign_pdal_tools.egg-info/top_level.txt
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-03 06:54:00.427112 ign-pdal-tools-0.5.0/pdaltools/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)       73 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/pdaltools/_version.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     8269 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/pdaltools/color.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2870 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/pdaltools/count_occurences_for_attribute.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     4619 2023-03-09 13:14:27.000000 ign-pdal-tools-0.5.0/pdaltools/las_add_buffer.py
--rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     1193 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.0/pdaltools/las_clip.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2998 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.0/pdaltools/las_info.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     3212 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.0/pdaltools/las_merge.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     4742 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/pdaltools/replace_attribute_in_las.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2385 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/pdaltools/standardize_format.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)      353 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/pyproject.toml
--rw-r--r--   0 LVauchier (24820) usernis  (10000)       38 2023-04-03 06:54:00.431112 ign-pdal-tools-0.5.0/setup.cfg
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-03 06:54:00.431112 ign-pdal-tools-0.5.0/test/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     3306 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.0/test/test_color.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)      802 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/test/test_count_occurences_for_attribute.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2179 2023-03-09 13:14:27.000000 ign-pdal-tools-0.5.0/test/test_las_add_buffer.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     1828 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.0/test/test_las_clip.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     1698 2023-03-09 13:14:27.000000 ign-pdal-tools-0.5.0/test/test_las_merge.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2771 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/test/test_replace_attribute_in_las.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2366 2023-03-31 16:35:05.000000 ign-pdal-tools-0.5.0/test/test_standardize_format.py
+drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-17 16:03:29.379737 ign-pdal-tools-0.5.1/
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2709 2023-04-17 16:03:29.379737 ign-pdal-tools-0.5.1/PKG-INFO
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2490 2023-04-17 16:02:15.000000 ign-pdal-tools-0.5.1/README.md
+drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-17 16:03:29.367737 ign-pdal-tools-0.5.1/ign_pdal_tools.egg-info/
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2709 2023-04-17 16:03:29.000000 ign-pdal-tools-0.5.1/ign_pdal_tools.egg-info/PKG-INFO
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)      544 2023-04-17 16:03:29.000000 ign-pdal-tools-0.5.1/ign_pdal_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)        1 2023-04-17 16:03:29.000000 ign-pdal-tools-0.5.1/ign_pdal_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)       10 2023-04-17 16:03:29.000000 ign-pdal-tools-0.5.1/ign_pdal_tools.egg-info/top_level.txt
+drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-17 16:03:29.371737 ign-pdal-tools-0.5.1/pdaltools/
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)       73 2023-04-17 16:02:54.000000 ign-pdal-tools-0.5.1/pdaltools/_version.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     8269 2023-04-05 07:50:05.000000 ign-pdal-tools-0.5.1/pdaltools/color.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     4619 2023-04-17 16:02:54.000000 ign-pdal-tools-0.5.1/pdaltools/las_add_buffer.py
+-rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     1193 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.1/pdaltools/las_clip.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2998 2023-04-17 16:02:54.000000 ign-pdal-tools-0.5.1/pdaltools/las_info.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     3212 2023-04-17 16:02:54.000000 ign-pdal-tools-0.5.1/pdaltools/las_merge.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     4742 2023-04-05 07:50:05.000000 ign-pdal-tools-0.5.1/pdaltools/replace_attribute_in_las.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2385 2023-04-05 07:50:05.000000 ign-pdal-tools-0.5.1/pdaltools/standardize_format.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)      353 2023-04-05 07:50:05.000000 ign-pdal-tools-0.5.1/pyproject.toml
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)       38 2023-04-17 16:03:29.383737 ign-pdal-tools-0.5.1/setup.cfg
+drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2023-04-17 16:03:29.379737 ign-pdal-tools-0.5.1/test/
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     3306 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.1/test/test_color.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2179 2023-04-05 07:50:05.000000 ign-pdal-tools-0.5.1/test/test_las_add_buffer.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     1828 2023-02-10 10:26:06.000000 ign-pdal-tools-0.5.1/test/test_las_clip.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     1698 2023-04-05 07:50:05.000000 ign-pdal-tools-0.5.1/test/test_las_merge.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2788 2023-04-17 16:02:15.000000 ign-pdal-tools-0.5.1/test/test_replace_attribute_in_las.py
+-rw-r--r--   0 LVauchier (24820) usernis  (10000)     2366 2023-04-05 07:50:05.000000 ign-pdal-tools-0.5.1/test/test_standardize_format.py
```

### Comparing `ign-pdal-tools-0.5.0/PKG-INFO` & `ign-pdal-tools-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 
 # Pdal tools
 
 Bibliothèque python qui réalise des opérations simples en utilisant pdal:
@@ -27,17 +27,21 @@
 
 **WARNING**: Pour `las_merge.py` et `las_add_buffer.py`, les noms de fichiers sont parsés pour trouver les voisins.
 Le format de nom de fichiers attendu est : `{prefix1}_{prefix2}_{xcoord}_{ycoord}_{postfix})}`, eg. `Semis_2021_0770_6278_LA93_IGN69.laz`
 
 ## Standardisation
 
 * `standardize_format.py`: réécrit un fichier las dans un format standard (cf. code)
-* `count_occurences_for_attribute.py`: pour un attribut donné (développé en premier
+* `count_occurences`: pour un attribut donné (développé en premier
 lieu pour de la classification), compte les occurences de chaque valeur sur un
 ensemble de fichiers las.
+    * `count_occurences_for_attribute.py`: compte les occurences sur un ou plusieurs fichiers et les
+et les sauve dans un fichier json
+    * `merge_occurences_counts.py` : permet d'assembler des comptes (fichiers json) en un seul fichier
+de compte d'occurences (utilisé en cas de parallélisation)
 * `replace_attribute_in_las.py`: à partir d'un fichier json contenant un tableau de
 correspondances, remplace les occurences de chaque valeur par la valeur associée
 dans le tableau.
 
 # Installation / Usage
 
 ## Bibliothèque
```

### Comparing `ign-pdal-tools-0.5.0/README.md` & `ign-pdal-tools-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,17 +20,21 @@
 
 **WARNING**: Pour `las_merge.py` et `las_add_buffer.py`, les noms de fichiers sont parsés pour trouver les voisins.
 Le format de nom de fichiers attendu est : `{prefix1}_{prefix2}_{xcoord}_{ycoord}_{postfix})}`, eg. `Semis_2021_0770_6278_LA93_IGN69.laz`
 
 ## Standardisation
 
 * `standardize_format.py`: réécrit un fichier las dans un format standard (cf. code)
-* `count_occurences_for_attribute.py`: pour un attribut donné (développé en premier
+* `count_occurences`: pour un attribut donné (développé en premier
 lieu pour de la classification), compte les occurences de chaque valeur sur un
 ensemble de fichiers las.
+    * `count_occurences_for_attribute.py`: compte les occurences sur un ou plusieurs fichiers et les
+et les sauve dans un fichier json
+    * `merge_occurences_counts.py` : permet d'assembler des comptes (fichiers json) en un seul fichier
+de compte d'occurences (utilisé en cas de parallélisation)
 * `replace_attribute_in_las.py`: à partir d'un fichier json contenant un tableau de
 correspondances, remplace les occurences de chaque valeur par la valeur associée
 dans le tableau.
 
 # Installation / Usage
 
 ## Bibliothèque
```

### Comparing `ign-pdal-tools-0.5.0/ign_pdal_tools.egg-info/PKG-INFO` & `ign-pdal-tools-0.5.1/ign_pdal_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ign-pdal-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Library for common LAS files manipulation with PDAL
 Author-email: Guillaume Liegard <guillaume.liegard@ign.fr>
 Description-Content-Type: text/markdown
 
 # Pdal tools
 
 Bibliothèque python qui réalise des opérations simples en utilisant pdal:
@@ -27,17 +27,21 @@
 
 **WARNING**: Pour `las_merge.py` et `las_add_buffer.py`, les noms de fichiers sont parsés pour trouver les voisins.
 Le format de nom de fichiers attendu est : `{prefix1}_{prefix2}_{xcoord}_{ycoord}_{postfix})}`, eg. `Semis_2021_0770_6278_LA93_IGN69.laz`
 
 ## Standardisation
 
 * `standardize_format.py`: réécrit un fichier las dans un format standard (cf. code)
-* `count_occurences_for_attribute.py`: pour un attribut donné (développé en premier
+* `count_occurences`: pour un attribut donné (développé en premier
 lieu pour de la classification), compte les occurences de chaque valeur sur un
 ensemble de fichiers las.
+    * `count_occurences_for_attribute.py`: compte les occurences sur un ou plusieurs fichiers et les
+et les sauve dans un fichier json
+    * `merge_occurences_counts.py` : permet d'assembler des comptes (fichiers json) en un seul fichier
+de compte d'occurences (utilisé en cas de parallélisation)
 * `replace_attribute_in_las.py`: à partir d'un fichier json contenant un tableau de
 correspondances, remplace les occurences de chaque valeur par la valeur associée
 dans le tableau.
 
 # Installation / Usage
 
 ## Bibliothèque
```

### Comparing `ign-pdal-tools-0.5.0/ign_pdal_tools.egg-info/SOURCES.txt` & `ign-pdal-tools-0.5.1/ign_pdal_tools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 pyproject.toml
 ign_pdal_tools.egg-info/PKG-INFO
 ign_pdal_tools.egg-info/SOURCES.txt
 ign_pdal_tools.egg-info/dependency_links.txt
 ign_pdal_tools.egg-info/top_level.txt
 pdaltools/_version.py
 pdaltools/color.py
-pdaltools/count_occurences_for_attribute.py
 pdaltools/las_add_buffer.py
 pdaltools/las_clip.py
 pdaltools/las_info.py
 pdaltools/las_merge.py
 pdaltools/replace_attribute_in_las.py
 pdaltools/standardize_format.py
 test/test_color.py
-test/test_count_occurences_for_attribute.py
 test/test_las_add_buffer.py
 test/test_las_clip.py
 test/test_las_merge.py
 test/test_replace_attribute_in_las.py
 test/test_standardize_format.py
```

### Comparing `ign-pdal-tools-0.5.0/pdaltools/color.py` & `ign-pdal-tools-0.5.1/pdaltools/color.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/pdaltools/las_add_buffer.py` & `ign-pdal-tools-0.5.1/pdaltools/las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/pdaltools/las_clip.py` & `ign-pdal-tools-0.5.1/pdaltools/las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/pdaltools/las_info.py` & `ign-pdal-tools-0.5.1/pdaltools/las_info.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/pdaltools/las_merge.py` & `ign-pdal-tools-0.5.1/pdaltools/las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/pdaltools/replace_attribute_in_las.py` & `ign-pdal-tools-0.5.1/pdaltools/replace_attribute_in_las.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/pdaltools/standardize_format.py` & `ign-pdal-tools-0.5.1/pdaltools/standardize_format.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/test/test_color.py` & `ign-pdal-tools-0.5.1/test/test_color.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/test/test_las_add_buffer.py` & `ign-pdal-tools-0.5.1/test/test_las_add_buffer.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/test/test_las_clip.py` & `ign-pdal-tools-0.5.1/test/test_las_clip.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/test/test_las_merge.py` & `ign-pdal-tools-0.5.1/test/test_las_merge.py`

 * *Files identical despite different names*

### Comparing `ign-pdal-tools-0.5.0/test/test_replace_attribute_in_las.py` & `ign-pdal-tools-0.5.1/test/test_replace_attribute_in_las.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import Counter
 import json
 import os
 from pdaltools.replace_attribute_in_las import replace_values, parse_replacement_map_from_path_or_json_string
-from pdaltools.count_occurences_for_attribute import compute_count_one_file
+from pdaltools.count_occurences.count_occurences_for_attribute import compute_count_one_file
 import pytest
 import shutil
 from test.utils import get_pdal_infos_summary
 from typing import Dict
 
 
 test_path = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `ign-pdal-tools-0.5.0/test/test_standardize_format.py` & `ign-pdal-tools-0.5.1/test/test_standardize_format.py`

 * *Files identical despite different names*

