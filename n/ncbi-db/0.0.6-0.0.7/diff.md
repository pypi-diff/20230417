# Comparing `tmp/ncbi_db-0.0.6.tar.gz` & `tmp/ncbi_db-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbi_db-0.0.6.tar", last modified: Mon Apr 17 08:57:00 2023, max compression
+gzip compressed data, was "ncbi_db-0.0.7.tar", last modified: Mon Apr 17 09:02:51 2023, max compression
```

## Comparing `ncbi_db-0.0.6.tar` & `ncbi_db-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2440 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1957 2023-04-17 08:35:04.000000 ncbi_db-0.0.6/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 ncbi_db-0.0.6/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      821 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 ncbi_db-0.0.6/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.842920 ncbi_db-0.0.6/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.842920 ncbi_db-0.0.6/src/ncbi_db/
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341967 2021-12-10 14:50:03.000000 ncbi_db-0.0.6/src/ncbi_db/MMlib3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1030 2023-04-17 08:48:08.000000 ncbi_db-0.0.6/src/ncbi_db/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-17 08:55:09.000000 ncbi_db-0.0.6/src/ncbi_db/_version.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    26296 2023-03-29 15:52:55.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_assembly.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     2247 2023-03-29 20:50:56.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_db_info.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7031 2023-04-17 08:54:55.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_lib.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9233 2023-03-29 15:53:59.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_pubmed.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     5542 2023-04-11 15:52:04.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_search.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    13514 2023-03-29 21:05:21.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_sequences.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    14375 2023-03-29 15:54:21.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    30717 2023-03-29 20:04:38.000000 ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy_tree.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9331 2023-03-29 15:54:33.000000 ncbi_db-0.0.6/src/ncbi_db/parse_genbank.py
--rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4524 2023-03-29 20:26:39.000000 ncbi_db-0.0.6/src/ncbi_db/search_ncbi_entries.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 08:57:00.846920 ncbi_db-0.0.6/src/ncbi_db.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2440 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      579 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       39 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        8 2023-04-17 08:57:00.000000 ncbi_db-0.0.6/src/ncbi_db.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 09:02:51.447357 ncbi_db-0.0.7/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2454 2023-04-17 09:02:51.447357 ncbi_db-0.0.7/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1971 2023-04-17 09:01:17.000000 ncbi_db-0.0.7/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 ncbi_db-0.0.7/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      821 2023-04-17 09:02:51.447357 ncbi_db-0.0.7/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 ncbi_db-0.0.7/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 09:02:51.443357 ncbi_db-0.0.7/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 09:02:51.443357 ncbi_db-0.0.7/src/ncbi_db/
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)   341967 2021-12-10 14:50:03.000000 ncbi_db-0.0.7/src/ncbi_db/MMlib3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1030 2023-04-17 08:48:08.000000 ncbi_db-0.0.7/src/ncbi_db/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-04-17 09:02:22.000000 ncbi_db-0.0.7/src/ncbi_db/_version.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    26296 2023-03-29 15:52:55.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_assembly.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     2247 2023-03-29 20:50:56.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_db_info.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     7031 2023-04-17 08:54:55.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_lib.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9233 2023-03-29 15:53:59.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_pubmed.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     5542 2023-04-11 15:52:04.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_search.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    13514 2023-03-29 21:05:21.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_sequences.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    14375 2023-03-29 15:54:21.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_taxonomy.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)    30717 2023-03-29 20:04:38.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_taxonomy_tree.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4210 2023-03-29 20:15:52.000000 ncbi_db-0.0.7/src/ncbi_db/ncbi_taxonomy_tree_db.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     9331 2023-03-29 15:54:33.000000 ncbi_db-0.0.7/src/ncbi_db/parse_genbank.py
+-rwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)     4524 2023-03-29 20:26:39.000000 ncbi_db-0.0.7/src/ncbi_db/search_ncbi_entries.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-04-17 09:02:51.447357 ncbi_db-0.0.7/src/ncbi_db.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     2454 2023-04-17 09:02:51.000000 ncbi_db-0.0.7/src/ncbi_db.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      616 2023-04-17 09:02:51.000000 ncbi_db-0.0.7/src/ncbi_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-04-17 09:02:51.000000 ncbi_db-0.0.7/src/ncbi_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       39 2023-04-17 09:02:51.000000 ncbi_db-0.0.7/src/ncbi_db.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        8 2023-04-17 09:02:51.000000 ncbi_db-0.0.7/src/ncbi_db.egg-info/top_level.txt
```

### Comparing `ncbi_db-0.0.6/PKG-INFO` & `ncbi_db-0.0.7/src/ncbi_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: ncbi_db
-Version: 0.0.6
+Name: ncbi-db
+Version: 0.0.7
 Summary: Collection of scripts that wrap the Entrez Bio python module, to query and download portions of NCBI databases
 Home-page: https://github.com/pypa/ncbi_db
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # ncbi_db
 Collection of commands to query or process NCBI data
 
 ## Installation
-conda install -c mmariotti -c conda-forge ncbi_db
+conda install -c mmariotti -c conda-forge -c etetoolkit ncbi_db
 
 ## Tools
 These command line tools are available:
 
 - **ncbi_assembly**       search and download assemblies/genomes for any species/lineage, or its annotation/proteome
 - **ncbi_sequences**      search and download nucleotide/protein sequences or their metadata
 - **ncbi_pubmed**         search and format ncbi pubmed entries
```

### Comparing `ncbi_db-0.0.6/README.md` & `ncbi_db-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ncbi_db
 Collection of commands to query or process NCBI data
 
 ## Installation
-conda install -c mmariotti -c conda-forge ncbi_db
+conda install -c mmariotti -c conda-forge -c etetoolkit ncbi_db
 
 ## Tools
 These command line tools are available:
 
 - **ncbi_assembly**       search and download assemblies/genomes for any species/lineage, or its annotation/proteome
 - **ncbi_sequences**      search and download nucleotide/protein sequences or their metadata
 - **ncbi_pubmed**         search and format ncbi pubmed entries
```

### Comparing `ncbi_db-0.0.6/setup.cfg` & `ncbi_db-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/MMlib3.py` & `ncbi_db-0.0.7/src/ncbi_db/MMlib3.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/__init__.py` & `ncbi_db-0.0.7/src/ncbi_db/__init__.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_assembly.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_assembly.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_db_info.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_db_info.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_lib.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_lib.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_pubmed.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_pubmed.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_search.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_search.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_sequences.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_sequences.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/ncbi_taxonomy_tree.py` & `ncbi_db-0.0.7/src/ncbi_db/ncbi_taxonomy_tree.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/parse_genbank.py` & `ncbi_db-0.0.7/src/ncbi_db/parse_genbank.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db/search_ncbi_entries.py` & `ncbi_db-0.0.7/src/ncbi_db/search_ncbi_entries.py`

 * *Files identical despite different names*

### Comparing `ncbi_db-0.0.6/src/ncbi_db.egg-info/PKG-INFO` & `ncbi_db-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
-Name: ncbi-db
-Version: 0.0.6
+Name: ncbi_db
+Version: 0.0.7
 Summary: Collection of scripts that wrap the Entrez Bio python module, to query and download portions of NCBI databases
 Home-page: https://github.com/pypa/ncbi_db
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # ncbi_db
 Collection of commands to query or process NCBI data
 
 ## Installation
-conda install -c mmariotti -c conda-forge ncbi_db
+conda install -c mmariotti -c conda-forge -c etetoolkit ncbi_db
 
 ## Tools
 These command line tools are available:
 
 - **ncbi_assembly**       search and download assemblies/genomes for any species/lineage, or its annotation/proteome
 - **ncbi_sequences**      search and download nucleotide/protein sequences or their metadata
 - **ncbi_pubmed**         search and format ncbi pubmed entries
```

### Comparing `ncbi_db-0.0.6/src/ncbi_db.egg-info/SOURCES.txt` & `ncbi_db-0.0.7/src/ncbi_db.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/ncbi_db/ncbi_db_info.py
 src/ncbi_db/ncbi_lib.py
 src/ncbi_db/ncbi_pubmed.py
 src/ncbi_db/ncbi_search.py
 src/ncbi_db/ncbi_sequences.py
 src/ncbi_db/ncbi_taxonomy.py
 src/ncbi_db/ncbi_taxonomy_tree.py
+src/ncbi_db/ncbi_taxonomy_tree_db.py
 src/ncbi_db/parse_genbank.py
 src/ncbi_db/search_ncbi_entries.py
 src/ncbi_db.egg-info/PKG-INFO
 src/ncbi_db.egg-info/SOURCES.txt
 src/ncbi_db.egg-info/dependency_links.txt
 src/ncbi_db.egg-info/requires.txt
 src/ncbi_db.egg-info/top_level.txt
```

