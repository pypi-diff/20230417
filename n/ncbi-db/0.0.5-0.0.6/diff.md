# Comparing `tmp/ncbi_db-0.0.5.tar.gz` & `tmp/ncbi_db-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbi_db-0.0.5.tar", last modified: Wed Mar 29 21:07:17 2023, max compression
+gzip compressed data, was "ncbi_db-0.0.6.tar", last modified: Mon Apr 17 08:57:00 2023, max compression
```

## Comparing `ncbi_db-0.0.5.tar` & `ncbi_db-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-29 21:07:17.968354 ncbi_db-0.0.5/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1316 2023-03-29 21:07:17.968354 ncbi_db-0.0.5/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      833 2023-03-29 20:55:58.000000 ncbi_db-0.0.5/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 ncbi_db-0.0.5/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      821 2023-03-29 21:07:17.968354 ncbi_db-0.0.5/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 ncbi_db-0.0.5/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-29 21:07:17.968354 ncbi_db-0.0.5/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-29 21:07:17.968354 ncbi_db-0.0.5/src/ncbi_db/
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341967 2021-12-10 14:50:03.000000 ncbi_db-0.0.5/src/ncbi_db/MMlib3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      461 2023-03-29 20:41:31.000000 ncbi_db-0.0.5/src/ncbi_db/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-03-29 20:56:20.000000 ncbi_db-0.0.5/src/ncbi_db/_version.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    26296 2023-03-29 15:52:55.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_assembly.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     2247 2023-03-29 20:50:56.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_db_info.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     6522 2023-03-29 16:00:01.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_lib.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9233 2023-03-29 15:53:59.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_pubmed.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     5453 2023-03-29 20:44:46.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_search.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    13514 2023-03-29 21:05:21.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_sequences.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    14375 2023-03-29 15:54:21.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_taxonomy.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    30717 2023-03-29 20:04:38.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_taxonomy_tree.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4210 2023-03-29 20:15:52.000000 ncbi_db-0.0.5/src/ncbi_db/ncbi_taxonomy_tree_db.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9331 2023-03-29 15:54:33.000000 ncbi_db-0.0.5/src/ncbi_db/parse_genbank.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4524 2023-03-29 20:26:39.000000 ncbi_db-0.0.5/src/ncbi_db/search_ncbi_entries.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-03-29 21:07:17.968354 ncbi_db-0.0.5/src/ncbi_db.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1316 2023-03-29 21:07:17.000000 ncbi_db-0.0.5/src/ncbi_db.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      616 2023-03-29 21:07:17.000000 ncbi_db-0.0.5/src/ncbi_db.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-03-29 21:07:17.000000 ncbi_db-0.0.5/src/ncbi_db.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       39 2023-03-29 21:07:17.000000 ncbi_db-0.0.5/src/ncbi_db.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        8 2023-03-29 21:07:17.000000 ncbi_db-0.0.5/src/ncbi_db.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2440 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1957 2023-04-17 08:35:04.000000 ncbi_db-0.0.6/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 ncbi_db-0.0.6/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      821 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 ncbi_db-0.0.6/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.842920 ncbi_db-0.0.6/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.842920 ncbi_db-0.0.6/src/ncbi_db/
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341967 2021-12-10 14:50:03.000000 ncbi_db-0.0.6/src/ncbi_db/MMlib3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1030 2023-04-17 08:48:08.000000 ncbi_db-0.0.6/src/ncbi_db/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-17 08:55:09.000000 ncbi_db-0.0.6/src/ncbi_db/_version.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    26296 2023-03-29 15:52:55.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_assembly.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     2247 2023-03-29 20:50:56.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_db_info.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7031 2023-04-17 08:54:55.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_lib.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9233 2023-03-29 15:53:59.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_pubmed.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     5542 2023-04-11 15:52:04.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_search.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    13514 2023-03-29 21:05:21.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_sequences.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    14375 2023-03-29 15:54:21.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    30717 2023-03-29 20:04:38.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy_tree.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9331 2023-03-29 15:54:33.000000 ncbi_db-0.0.6/src/ncbi_db/parse_genbank.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4524 2023-03-29 20:26:39.000000 ncbi_db-0.0.6/src/ncbi_db/search_ncbi_entries.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/src/ncbi_db.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2440 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      579 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       39 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        8 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/top_level.txt
```

### Comparing `ncbi_db-0.0.5/setup.cfg` & `ncbi_db-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/MMlib3.py` & `ncbi_db-0.0.6/src/ncbi_db/MMlib3.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_assembly.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_assembly.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_db_info.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_db_info.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_lib.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 from string import *
 import sys
 from .MMlib3 import *
-from Bio import Entrez 
+from Bio import Entrez
 from urllib.error import URLError
 from ftplib import FTP
 import gzip
 import shutil
 from time import strptime, sleep
 import traceback
+import easyterm
+from pathlib import Path
 Entrez.email = None
 
+ncbi_config=easyterm.commandlineopt.CommandLineOptions({
+  'ncbi_taxdb':'',
+  'email':'',
+  })
+
+def load_ncbi_config():
+  #nonlocal ncbi_config
+  ncbi_config_file=Path( Path.home()+'/.ncbi_db' )
+  if ncbi_config_file.is_file():
+    ncbi_config.update(
+      easyterm.read_config_file(str(ncbi_config_file))
+      )
+
+def save_ncbi_config():
+  #nonlocal ncbi_config
+  ncbi_config_file=Path( Path.home()+'/.ncbi_db' )
+  ncbi_config.write_config_file(str(ncbi_config_file))
+
 #### NOTE some values must be defined in MMlib.opt:
 # sleep_time
 # retmax
 # max_attempts
 set_MMlib_var('opt', options( {'retmax':250, 'max_attempts':10, 'sleep_time':5, 'v':0}))  ## this is to make this lib work without MMlib command line calls
 
 """ Wrapping default Entrez methods to connect to ncbi to allow network problems and batch requests"""
 def esearch(**keyargs):
-  """ Generic wrap. You should use term=..  and db=..  and field=..  
+  """ Generic wrap. You should use term=..  and db=..  and field=..
   Note: these will be used:  opt['max_attempts']   opt['sleep_time']; opt['retmax']
    where opt is get_MMlib_var('opt')   [you can set it with  set_MMlib_var('opt', opt) ]
   Returns a list of uids (strings) """
   opt=get_MMlib_var('opt');  max_attempts=opt['max_attempts']; sleep_time=opt['sleep_time']; retmax=opt['retmax']
   uid_list=[]; retstart=0
   while not uid_list or (int(searched_g['Count']) > len(uid_list) ):  ## to manage when more results are returned than the allowed number
     if  uid_list:    retstart+=int(searched_g['RetMax'])  ## same as setting it to len(genome_uid_list)
```

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_pubmed.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_pubmed.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_search.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 #########################################################
 ############ loading options
   global opt
   if not args:
       opt=command_line(def_opt, help_msg, 'd', synonyms=command_line_synonyms, nowarning=1)
   else:
       opt=args
+      for k in def_opt:
+          if k not in opt:
+              opt[k]=def_opt[k]      
   
   set_MMlib_var('opt', opt)
   #global temp_folder; temp_folder=Folder(random_folder(opt['temp'])); test_writeable_folder(temp_folder, 'temp_folder'); set_MMlib_var('temp_folder', temp_folder)
   #global split_folder;    split_folder=Folder(opt['temp']);               test_writeable_folder(split_folder); set_MMlib_var('split_folder', split_folder) 
   #checking input
 
   if opt['list']:
```

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_sequences.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_sequences.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_taxonomy.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/ncbi_taxonomy_tree.py` & `ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy_tree.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/parse_genbank.py` & `ncbi_db-0.0.6/src/ncbi_db/parse_genbank.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db/search_ncbi_entries.py` & `ncbi_db-0.0.6/src/ncbi_db/search_ncbi_entries.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.5/src/ncbi_db.egg-info/SOURCES.txt` & `ncbi_db-0.0.6/src/ncbi_db.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 src/ncbi_db/ncbi_db_info.py
 src/ncbi_db/ncbi_lib.py
 src/ncbi_db/ncbi_pubmed.py
 src/ncbi_db/ncbi_search.py
 src/ncbi_db/ncbi_sequences.py
 src/ncbi_db/ncbi_taxonomy.py
 src/ncbi_db/ncbi_taxonomy_tree.py
-src/ncbi_db/ncbi_taxonomy_tree_db.py
 src/ncbi_db/parse_genbank.py
 src/ncbi_db/search_ncbi_entries.py
 src/ncbi_db.egg-info/PKG-INFO
 src/ncbi_db.egg-info/SOURCES.txt
 src/ncbi_db.egg-info/dependency_links.txt
 src/ncbi_db.egg-info/requires.txt
 src/ncbi_db.egg-info/top_level.txt
```

