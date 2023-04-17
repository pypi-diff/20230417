# Comparing `tmp/ncbi_db-0.0.8.tar.gz` & `tmp/ncbi_db-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbi_db-0.0.8.tar", last modified: Mon Apr 17 10:46:38 2023, max compression
+gzip compressed data, was "ncbi_db-0.1.0.tar", last modified: Mon Apr 17 11:10:02 2023, max compression
```

## Comparing `ncbi_db-0.0.8.tar` & `ncbi_db-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 10:46:38.929864 ncbi_db-0.0.8/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2454 2023-04-17 10:46:38.929864 ncbi_db-0.0.8/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1971 2023-04-17 09:01:17.000000 ncbi_db-0.0.8/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 ncbi_db-0.0.8/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      821 2023-04-17 10:46:38.929864 ncbi_db-0.0.8/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 ncbi_db-0.0.8/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 10:46:38.929864 ncbi_db-0.0.8/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 10:46:38.929864 ncbi_db-0.0.8/src/ncbi_db/
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341967 2021-12-10 14:50:03.000000 ncbi_db-0.0.8/src/ncbi_db/MMlib3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1030 2023-04-17 08:48:08.000000 ncbi_db-0.0.8/src/ncbi_db/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-17 10:40:43.000000 ncbi_db-0.0.8/src/ncbi_db/_version.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    27126 2023-04-17 09:57:17.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_assembly.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     2384 2023-04-17 09:50:18.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_db_info.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7629 2023-04-17 09:48:36.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_lib.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9362 2023-04-17 09:57:37.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_pubmed.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     5642 2023-04-17 09:59:03.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_search.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    13586 2023-04-17 10:06:22.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_sequences.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    14638 2023-04-17 10:10:26.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_taxonomy.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    31389 2023-04-17 10:36:03.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_taxonomy_tree.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4475 2023-04-17 10:24:05.000000 ncbi_db-0.0.8/src/ncbi_db/ncbi_taxonomy_tree_db.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9331 2023-03-29 15:54:33.000000 ncbi_db-0.0.8/src/ncbi_db/parse_genbank.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4479 2023-04-17 10:12:31.000000 ncbi_db-0.0.8/src/ncbi_db/search_ncbi_entries.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 10:46:38.929864 ncbi_db-0.0.8/src/ncbi_db.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2454 2023-04-17 10:46:38.000000 ncbi_db-0.0.8/src/ncbi_db.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      616 2023-04-17 10:46:38.000000 ncbi_db-0.0.8/src/ncbi_db.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-17 10:46:38.000000 ncbi_db-0.0.8/src/ncbi_db.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       39 2023-04-17 10:46:38.000000 ncbi_db-0.0.8/src/ncbi_db.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        8 2023-04-17 10:46:38.000000 ncbi_db-0.0.8/src/ncbi_db.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 11:10:02.551014 ncbi_db-0.1.0/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2454 2023-04-17 11:10:02.551014 ncbi_db-0.1.0/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1971 2023-04-17 09:01:17.000000 ncbi_db-0.1.0/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 ncbi_db-0.1.0/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      821 2023-04-17 11:10:02.551014 ncbi_db-0.1.0/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 ncbi_db-0.1.0/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 11:10:02.547014 ncbi_db-0.1.0/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 11:10:02.547014 ncbi_db-0.1.0/src/ncbi_db/
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341967 2021-12-10 14:50:03.000000 ncbi_db-0.1.0/src/ncbi_db/MMlib3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1030 2023-04-17 08:48:08.000000 ncbi_db-0.1.0/src/ncbi_db/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-17 11:01:10.000000 ncbi_db-0.1.0/src/ncbi_db/_version.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    27126 2023-04-17 09:57:17.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_assembly.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     2384 2023-04-17 09:50:18.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_db_info.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7629 2023-04-17 09:48:36.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_lib.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9395 2023-04-17 11:07:57.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_pubmed.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     5642 2023-04-17 09:59:03.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_search.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    13620 2023-04-17 10:53:35.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_sequences.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    14638 2023-04-17 10:10:26.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_taxonomy.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    31464 2023-04-17 10:59:12.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_taxonomy_tree.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4475 2023-04-17 10:24:05.000000 ncbi_db-0.1.0/src/ncbi_db/ncbi_taxonomy_tree_db.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9331 2023-03-29 15:54:33.000000 ncbi_db-0.1.0/src/ncbi_db/parse_genbank.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4479 2023-04-17 10:12:31.000000 ncbi_db-0.1.0/src/ncbi_db/search_ncbi_entries.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 11:10:02.551014 ncbi_db-0.1.0/src/ncbi_db.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2454 2023-04-17 11:10:02.000000 ncbi_db-0.1.0/src/ncbi_db.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      616 2023-04-17 11:10:02.000000 ncbi_db-0.1.0/src/ncbi_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-17 11:10:02.000000 ncbi_db-0.1.0/src/ncbi_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       39 2023-04-17 11:10:02.000000 ncbi_db-0.1.0/src/ncbi_db.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        8 2023-04-17 11:10:02.000000 ncbi_db-0.1.0/src/ncbi_db.egg-info/top_level.txt
```

### Comparing `ncbi_db-0.0.8/PKG-INFO` & `ncbi_db-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbi_db
-Version: 0.0.8
+Version: 0.1.0
 Summary: Collection of scripts that wrap the Entrez Bio python module, to query and download portions of NCBI databases
 Home-page: https://github.com/pypa/ncbi_db
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ncbi_db-0.0.8/README.md` & `ncbi_db-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/setup.cfg` & `ncbi_db-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/MMlib3.py` & `ncbi_db-0.1.0/src/ncbi_db/MMlib3.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/__init__.py` & `ncbi_db-0.1.0/src/ncbi_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_assembly.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_assembly.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_db_info.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_db_info.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_lib.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_lib.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_pubmed.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_pubmed.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,17 +203,17 @@
         
 
     
 
   if output_format=='html':  textout+='</body>'
 
   if output_format=='txt':
-    print(textout.encode('utf8', errors='replace'))
+    print(textout.encode('utf8', errors='replace').decode('utf8')  )
   elif output_format=='html':
-    print(textout.encode('ascii', 'xmlcharrefreplace'))
+    print(textout.encode('ascii', 'xmlcharrefreplace').decode('ascii'))
 
   ###############
```

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_search.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_search.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_sequences.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 from string import *
 import sys
 from subprocess import *
 from .MMlib3 import *
 from .ncbi_taxonomy import main as run_ncbi_taxonomy
+from .ncbi_lib import email_setup
 from Bio import Entrez, SeqIO
 import time
 
 help_msg="""Program to fetch entries from the ncbi sequence databases through the internet and print information such as its sequence or the source organism. It wraps Bio->Entrez and Bio->SeqIO.
 
 ncbi_sequences  [mode] [ids] [options]
```

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_taxonomy.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_taxonomy_tree.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_taxonomy_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python3
 import sys,os
 import json
 import sqlite3
 import argparse
-from ete3 import Tree
 from collections import defaultdict
 from .MMlib3 import bbash, unmask_characters, mask_characters, get_taxids_from_ncbi_db, printerr, random_folder
 import shutil, os
 from easyterm import NoTracebackError
 from .ncbi_taxonomy_tree_db import main as run_ncbi_taxonomy_tree_db
 from .ncbi_lib import load_ncbi_config, save_ncbi_config
 from pathlib import Path
 
+import warnings
+warnings.filterwarnings("ignore", category=SyntaxWarning)
+from ete3 import Tree
+
 def get_parser():
     """returns the argparse parser object with the argument option requirements"""
 
     parser     = argparse.ArgumentParser(description='Get the phylogenetic tree from a list of species (based on NCBI taxonomy)')
     taxid_file = parser.add_argument_group('input')
     tree       = parser.add_argument_group('output')
     render     = parser.add_argument_group('render')
```

### Comparing `ncbi_db-0.0.8/src/ncbi_db/ncbi_taxonomy_tree_db.py` & `ncbi_db-0.1.0/src/ncbi_db/ncbi_taxonomy_tree_db.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/parse_genbank.py` & `ncbi_db-0.1.0/src/ncbi_db/parse_genbank.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db/search_ncbi_entries.py` & `ncbi_db-0.1.0/src/ncbi_db/search_ncbi_entries.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.8/src/ncbi_db.egg-info/PKG-INFO` & `ncbi_db-0.1.0/src/ncbi_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbi-db
-Version: 0.0.8
+Version: 0.1.0
 Summary: Collection of scripts that wrap the Entrez Bio python module, to query and download portions of NCBI databases
 Home-page: https://github.com/pypa/ncbi_db
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ncbi_db-0.0.8/src/ncbi_db.egg-info/SOURCES.txt` & `ncbi_db-0.1.0/src/ncbi_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

