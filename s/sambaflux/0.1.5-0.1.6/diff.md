# Comparing `tmp/sambaflux-0.1.5.tar.gz` & `tmp/sambaflux-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/juliette/these/code/git/SAMBA/SAMBAflux/sambaflux/dist/.tmp-poujofe9/sambaflux-0.1.5.tar", last modified: Wed Mar 29 12:26:09 2023, max compression
+gzip compressed data, was "/home/juliette/these/code/git/SAMBA/SAMBAflux/sambaflux/dist/.tmp-ov7wt5jj/sambaflux-0.1.6.tar", last modified: Mon Apr 17 14:07:50 2023, max compression
```

## Comparing `sambaflux-0.1.5.tar` & `sambaflux-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     1073 2022-03-08 14:30:09.000000 sambaflux-0.1.5/LICENSE
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     3345 2023-03-29 12:26:09.000000 sambaflux-0.1.5/PKG-INFO
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     2791 2023-03-29 12:17:34.000000 sambaflux-0.1.5/README.md
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     1012 2022-08-05 09:07:28.000000 sambaflux-0.1.5/pyproject.toml
--rw-rw-r--   0 juliette  (1000) juliette  (1000)      714 2023-03-29 12:26:09.000000 sambaflux-0.1.5/setup.cfg
--rw-rw-r--   0 juliette  (1000) juliette  (1000)       98 2023-03-29 12:23:20.000000 sambaflux-0.1.5/setup.py
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/samba/
--rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-03 14:51:03.000000 sambaflux-0.1.5/src/samba/__init__.py
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/samba/fva/
--rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:20:32.000000 sambaflux-0.1.5/src/samba/fva/__init__.py
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     3338 2023-03-29 12:20:32.000000 sambaflux-0.1.5/src/samba/fva/fva_functions.py
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/samba/iopy/
--rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-05 09:20:03.000000 sambaflux-0.1.5/src/samba/iopy/__init__.py
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     3108 2023-03-29 12:20:32.000000 sambaflux-0.1.5/src/samba/iopy/export.py
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     1126 2022-03-10 10:38:39.000000 sambaflux-0.1.5/src/samba/iopy/read_model.py
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/samba/sampling/
--rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-03 14:51:03.000000 sambaflux-0.1.5/src/samba/sampling/__init__.py
--rw-rw-r--   0 juliette  (1000) juliette  (1000)      454 2022-03-10 11:28:59.000000 sambaflux-0.1.5/src/samba/sampling/sample_functions.py
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     1389 2022-03-10 11:03:12.000000 sambaflux-0.1.5/src/samba/sampling/wtopt.py
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/samba/setup/
--rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-03 14:51:03.000000 sambaflux-0.1.5/src/samba/setup/__init__.py
--rw-rw-r--   0 juliette  (1000) juliette  (1000)      543 2022-07-25 14:55:31.000000 sambaflux-0.1.5/src/samba/setup/prepare_reactions.py
-drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/sambaflux.egg-info/
--rw-rw-r--   0 juliette  (1000) juliette  (1000)     3345 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/sambaflux.egg-info/PKG-INFO
--rw-rw-r--   0 juliette  (1000) juliette  (1000)      558 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/sambaflux.egg-info/SOURCES.txt
--rw-rw-r--   0 juliette  (1000) juliette  (1000)        1 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/sambaflux.egg-info/dependency_links.txt
--rw-rw-r--   0 juliette  (1000) juliette  (1000)       14 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/sambaflux.egg-info/requires.txt
--rw-rw-r--   0 juliette  (1000) juliette  (1000)        6 2023-03-29 12:26:09.000000 sambaflux-0.1.5/src/sambaflux.egg-info/top_level.txt
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     1073 2022-03-08 14:30:09.000000 sambaflux-0.1.6/LICENSE
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     3345 2023-04-17 14:07:50.000000 sambaflux-0.1.6/PKG-INFO
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     2791 2023-03-29 12:17:34.000000 sambaflux-0.1.6/README.md
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     1012 2022-08-05 09:07:28.000000 sambaflux-0.1.6/pyproject.toml
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)      714 2023-04-17 14:07:50.000000 sambaflux-0.1.6/setup.cfg
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)       98 2023-04-17 14:03:25.000000 sambaflux-0.1.6/setup.py
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/samba/
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-03 14:51:03.000000 sambaflux-0.1.6/src/samba/__init__.py
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/samba/fva/
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2023-03-29 12:20:32.000000 sambaflux-0.1.6/src/samba/fva/__init__.py
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     3338 2023-03-29 12:20:32.000000 sambaflux-0.1.6/src/samba/fva/fva_functions.py
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/samba/iopy/
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-05 09:20:03.000000 sambaflux-0.1.6/src/samba/iopy/__init__.py
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     3238 2023-04-17 13:23:18.000000 sambaflux-0.1.6/src/samba/iopy/export.py
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     1126 2022-03-10 10:38:39.000000 sambaflux-0.1.6/src/samba/iopy/read_model.py
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/samba/sampling/
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-03 14:51:03.000000 sambaflux-0.1.6/src/samba/sampling/__init__.py
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)      454 2022-03-10 11:28:59.000000 sambaflux-0.1.6/src/samba/sampling/sample_functions.py
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     1389 2022-03-10 11:03:12.000000 sambaflux-0.1.6/src/samba/sampling/wtopt.py
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/samba/setup/
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)        0 2022-08-03 14:51:03.000000 sambaflux-0.1.6/src/samba/setup/__init__.py
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)      543 2023-04-17 12:34:55.000000 sambaflux-0.1.6/src/samba/setup/prepare_reactions.py
+drwxrwxr-x   0 juliette  (1000) juliette  (1000)        0 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/sambaflux.egg-info/
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)     3345 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/sambaflux.egg-info/PKG-INFO
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)      558 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/sambaflux.egg-info/SOURCES.txt
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)        1 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/sambaflux.egg-info/dependency_links.txt
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)       14 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/sambaflux.egg-info/requires.txt
+-rw-rw-r--   0 juliette  (1000) juliette  (1000)        6 2023-04-17 14:07:50.000000 sambaflux-0.1.6/src/sambaflux.egg-info/top_level.txt
```

### Comparing `sambaflux-0.1.5/LICENSE` & `sambaflux-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sambaflux-0.1.5/PKG-INFO` & `sambaflux-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sambaflux
-Version: 0.1.5
+Version: 0.1.6
 Summary: Sampling Biomarker Analysis using flux sampling
 Home-page: https://forgemia.inra.fr/metexplore/cbm/samba/-/tree/main/sambaflux
 Author: Juliette Cooke
 Author-email: juliette.cooke@inrae.fr
 Project-URL: Bug Tracker, https://forgemia.inra.fr/metexplore/cbm/samba/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sambaflux-0.1.5/README.md` & `sambaflux-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sambaflux-0.1.5/pyproject.toml` & `sambaflux-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sambaflux-0.1.5/setup.cfg` & `sambaflux-0.1.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sambaflux
-version = 0.1.5
+version = 0.1.6
 author = Juliette Cooke
 author_email = juliette.cooke@inrae.fr
 description = Sampling Biomarker Analysis using flux sampling
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://forgemia.inra.fr/metexplore/cbm/samba/-/tree/main/sambaflux
 project_urls =
```

### Comparing `sambaflux-0.1.5/src/samba/fva/fva_functions.py` & `sambaflux-0.1.6/src/samba/fva/fva_functions.py`

 * *Files identical despite different names*

### Comparing `sambaflux-0.1.5/src/samba/iopy/export.py` & `sambaflux-0.1.6/src/samba/iopy/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,22 @@
                 n_samples) + "_" + type + ".csv.gz"
     fva_results.to_csv(final_path, index=True, compression='gzip')
     print("Wrote to "+final_path)
 
 
 def extract_results(s, results, model):
     # Extract from results
-    if results is None:
+    if results == "exchanges":
         if model.exchanges is not None:
             results_columns = [rxn.id for rxn in model.exchanges]
         else:
             results_columns = [col for col in s if col.startswith('EX_')]
-    else:
+    elif results == "all":
+        results_columns = [rxn.id for rxn in model.reactions]
+    else:  # File containing reaction IDs
         results_columns = parse_rxns(results)
     s_results = s[results_columns].round(3)
     return s_results
 
 
 def extract_fva_results(s, results, model):
     # Extract from results
```

### Comparing `sambaflux-0.1.5/src/samba/iopy/read_model.py` & `sambaflux-0.1.6/src/samba/iopy/read_model.py`

 * *Files identical despite different names*

### Comparing `sambaflux-0.1.5/src/samba/sampling/wtopt.py` & `sambaflux-0.1.6/src/samba/sampling/wtopt.py`

 * *Files identical despite different names*

### Comparing `sambaflux-0.1.5/src/samba/setup/prepare_reactions.py` & `sambaflux-0.1.6/src/samba/setup/prepare_reactions.py`

 * *Files identical despite different names*

### Comparing `sambaflux-0.1.5/src/sambaflux.egg-info/PKG-INFO` & `sambaflux-0.1.6/src/sambaflux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sambaflux
-Version: 0.1.5
+Version: 0.1.6
 Summary: Sampling Biomarker Analysis using flux sampling
 Home-page: https://forgemia.inra.fr/metexplore/cbm/samba/-/tree/main/sambaflux
 Author: Juliette Cooke
 Author-email: juliette.cooke@inrae.fr
 Project-URL: Bug Tracker, https://forgemia.inra.fr/metexplore/cbm/samba/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sambaflux-0.1.5/src/sambaflux.egg-info/SOURCES.txt` & `sambaflux-0.1.6/src/sambaflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

