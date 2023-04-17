# Comparing `tmp/anoexpress-0.1.2.tar.gz` & `tmp/anoexpress-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anoexpress-0.1.2.tar", max compression
+gzip compressed data, was "anoexpress-0.1.3.tar", max compression
```

## Comparing `anoexpress-0.1.2.tar` & `anoexpress-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.2/LICENSE
--rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.2/anoexpress/__init__.py
--rw-r--r--   0        0        0    25139 2023-03-14 18:13:58.360116 anoexpress-0.1.2/anoexpress/anoexpress.py
--rw-r--r--   0        0        0      756 2023-03-26 16:58:51.752081 anoexpress-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      960 2023-03-26 17:00:12.370913 anoexpress-0.1.2/setup.py
--rw-r--r--   0        0        0      789 2023-03-26 17:00:12.371329 anoexpress-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-11-12 23:31:02.745561 anoexpress-0.1.3/LICENSE
+-rw-r--r--   0        0        0       66 2023-03-06 23:08:43.188006 anoexpress-0.1.3/anoexpress/__init__.py
+-rw-r--r--   0        0        0    25133 2023-04-05 12:34:58.715685 anoexpress-0.1.3/anoexpress/anoexpress.py
+-rw-r--r--   0        0        0      750 2023-04-17 13:36:20.788753 anoexpress-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 anoexpress-0.1.3/PKG-INFO
```

### Comparing `anoexpress-0.1.2/LICENSE` & `anoexpress-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anoexpress-0.1.2/anoexpress/anoexpress.py` & `anoexpress-0.1.3/anoexpress/anoexpress.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
   if sort_by is None:
      return df.copy()
   if sort_by == 'median':
     sort_idxs = np.argsort(df.set_index('GeneID').drop(columns='GeneName', errors='ignore').apply(np.nanmedian, axis=1)).values
   elif sort_by == 'mean':
     sort_idxs = np.argsort(df.set_index('GeneID').drop(columns='GeneName', errors='ignore').apply(np.nanmean, axis=1)).values
   elif sort_by == 'agap':
-    sort_idxs = np.argsort(df['GeneID'].values)[::-1]
+    sort_idxs = np.argsort(df['GeneID'].values)
   elif sort_by == 'position':
     assert analysis != 'fun', "funestus cannot be sorted by position yet"
     
     import malariagen_data
     ag3 = malariagen_data.Ag3()
     gff = ag3.genome_features().query("type == 'gene' & contig in @ag3.contigs")
     gene_ids = df['GeneID'].to_list()
```

### Comparing `anoexpress-0.1.2/pyproject.toml` & `anoexpress-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "anoexpress"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "anoexpress" }
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.10"
+python = ">=3.7.1"
 malariagen_data = "*"
 pandas = [
     {version="<1.4", python=">=3.7.1,<3.8"},
     {version="*", python=">=3.8,<3.11"}
 ]
 seaborn = "*"
 numpy = "*"
```

### Comparing `anoexpress-0.1.2/PKG-INFO` & `anoexpress-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: anoexpress
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to access insecticide resistance gene expression meta analyse in Anopheles mosquitoes
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.7.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: malariagen_data
 Requires-Dist: numpy
-Requires-Dist: pandas (<1.4); python_full_version >= "3.7.1" and python_version < "3.8"
-Requires-Dist: pandas; python_version >= "3.8" and python_version < "3.11"
+Requires-Dist: pandas (<1.4) ; python_full_version >= "3.7.1" and python_version < "3.8"
+Requires-Dist: pandas ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: plotly
 Requires-Dist: scipy
 Requires-Dist: seaborn
 Requires-Dist: statsmodels
 Requires-Dist: tqdm
```

