# Comparing `tmp/dexom_python-1.0.tar.gz` & `tmp/dexom_python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexom_python-1.0.tar", max compression
+gzip compressed data, was "dexom_python-1.0.1.tar", max compression
```

## Comparing `dexom_python-1.0.tar` & `dexom_python-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35086 2023-04-03 11:22:31.225006 dexom_python-1.0/LICENSE
--rw-r--r--   0        0        0    12001 2023-04-05 14:57:06.542755 dexom_python-1.0/README.md
--rw-r--r--   0        0        0      559 2023-04-05 14:23:27.777934 dexom_python-1.0/dexom_python/__init__.py
--rw-r--r--   0        0        0     6006 2023-04-04 13:54:14.100172 dexom_python-1.0/dexom_python/cluster_utils/Snakefile
--rw-r--r--   0        0        0        0 2023-04-03 11:22:31.225006 dexom_python-1.0/dexom_python/cluster_utils/__init__.py
--rw-r--r--   0        0        0     2741 2023-04-04 13:54:14.100172 dexom_python-1.0/dexom_python/cluster_utils/cluster_config.yaml
--rw-r--r--   0        0        0      452 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/cluster_utils/cluster_install_dexom_python.sh
--rw-r--r--   0        0        0        0 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/cluster_utils/legacy/__init__.py
--rw-r--r--   0        0        0     7487 2023-04-04 11:35:30.565481 dexom_python-1.0/dexom_python/cluster_utils/legacy/dexom_cluster_results.py
--rw-r--r--   0        0        0    16971 2023-04-04 11:35:30.565481 dexom_python-1.0/dexom_python/cluster_utils/legacy/write_cluster_scripts.py
--rw-r--r--   0        0        0     1006 2023-04-04 11:35:30.565481 dexom_python-1.0/dexom_python/cluster_utils/slurm_example_gpr.sh
--rw-r--r--   0        0        0     1253 2023-04-04 13:54:14.100172 dexom_python-1.0/dexom_python/cluster_utils/snakemake_utils.smk
--rw-r--r--   0        0        0     1145 2023-04-04 11:35:30.565481 dexom_python-1.0/dexom_python/cluster_utils/solution_compilation.py
--rw-r--r--   0        0        0      803 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/cluster_utils/submit.py
--rw-r--r--   0        0        0      436 2023-04-04 11:35:30.565481 dexom_python-1.0/dexom_python/cluster_utils/submit_slurm.sh
--rw-r--r--   0        0        0      423 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/default_parameter_values.py
--rw-r--r--   0        0        0      219 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/enum_functions/__init__.py
--rw-r--r--   0        0        0    11182 2023-04-04 11:35:30.569481 dexom_python-1.0/dexom_python/enum_functions/diversity_enum_functions.py
--rw-r--r--   0        0        0     7662 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/enum_functions/enumeration.py
--rw-r--r--   0        0        0     9335 2023-04-04 11:35:30.569481 dexom_python-1.0/dexom_python/enum_functions/icut_functions.py
--rw-r--r--   0        0        0    11129 2023-04-04 11:35:30.569481 dexom_python-1.0/dexom_python/enum_functions/maxdist_functions.py
--rw-r--r--   0        0        0    13950 2023-04-04 11:35:30.569481 dexom_python-1.0/dexom_python/enum_functions/rxn_enum_functions.py
--rw-r--r--   0        0        0    11359 2023-04-05 14:23:27.777934 dexom_python-1.0/dexom_python/gpr_rules.py
--rw-r--r--   0        0        0    11789 2023-04-05 14:23:27.777934 dexom_python-1.0/dexom_python/imat_functions.py
--rw-r--r--   0        0        0     2487 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/main.py
--rw-r--r--   0        0        0     7382 2023-04-05 14:23:27.777934 dexom_python-1.0/dexom_python/model_functions.py
--rw-r--r--   0        0        0     7925 2023-04-04 11:35:30.569481 dexom_python-1.0/dexom_python/pathway_enrichment.py
--rw-r--r--   0        0        0     8878 2023-04-04 11:35:30.573481 dexom_python-1.0/dexom_python/result_functions.py
--rw-r--r--   0        0        0    10064 2023-04-03 11:22:31.229006 dexom_python-1.0/dexom_python/toy_models.py
--rw-r--r--   0        0        0      692 2023-04-05 15:02:22.872907 dexom_python-1.0/pyproject.toml
--rw-r--r--   0        0        0    12986 1970-01-01 00:00:00.000000 dexom_python-1.0/PKG-INFO
+-rw-r--r--   0        0        0    35086 2023-04-17 07:19:51.515506 dexom_python-1.0.1/LICENSE
+-rw-r--r--   0        0        0    12001 2023-04-17 07:19:51.515506 dexom_python-1.0.1/README.md
+-rw-r--r--   0        0        0      559 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/__init__.py
+-rw-r--r--   0        0        0     6006 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/Snakefile
+-rw-r--r--   0        0        0        0 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/__init__.py
+-rw-r--r--   0        0        0     2741 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/cluster_config.yaml
+-rw-r--r--   0        0        0      452 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/cluster_install_dexom_python.sh
+-rw-r--r--   0        0        0        0 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/legacy/__init__.py
+-rw-r--r--   0        0        0     7487 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/legacy/dexom_cluster_results.py
+-rw-r--r--   0        0        0    16971 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/legacy/write_cluster_scripts.py
+-rw-r--r--   0        0        0     1006 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/slurm_example_gpr.sh
+-rw-r--r--   0        0        0     1253 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/snakemake_utils.smk
+-rw-r--r--   0        0        0     1145 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/solution_compilation.py
+-rw-r--r--   0        0        0      803 2023-04-17 07:19:51.515506 dexom_python-1.0.1/dexom_python/cluster_utils/submit.py
+-rw-r--r--   0        0        0      436 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/cluster_utils/submit_slurm.sh
+-rw-r--r--   0        0        0      423 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/default_parameter_values.py
+-rw-r--r--   0        0        0      219 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/__init__.py
+-rw-r--r--   0        0        0    11182 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/diversity_enum_functions.py
+-rw-r--r--   0        0        0     7662 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/enumeration.py
+-rw-r--r--   0        0        0     9335 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/icut_functions.py
+-rw-r--r--   0        0        0    11129 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/maxdist_functions.py
+-rw-r--r--   0        0        0    13950 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/enum_functions/rxn_enum_functions.py
+-rw-r--r--   0        0        0    10988 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/gpr_rules.py
+-rw-r--r--   0        0        0    11789 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/imat_functions.py
+-rw-r--r--   0        0        0     2487 2023-04-17 07:19:51.519506 dexom_python-1.0.1/dexom_python/main.py
+-rw-r--r--   0        0        0     7382 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/model_functions.py
+-rw-r--r--   0        0        0     7925 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/pathway_enrichment.py
+-rw-r--r--   0        0        0     8878 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/result_functions.py
+-rw-r--r--   0        0        0    10064 2023-04-17 07:19:51.523507 dexom_python-1.0.1/dexom_python/toy_models.py
+-rw-r--r--   0        0        0      696 2023-04-17 07:19:51.547509 dexom_python-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12992 1970-01-01 00:00:00.000000 dexom_python-1.0.1/PKG-INFO
```

### Comparing `dexom_python-1.0/LICENSE` & `dexom_python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/README.md` & `dexom_python-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/__init__.py` & `dexom_python-1.0.1/dexom_python/__init__.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/Snakefile` & `dexom_python-1.0.1/dexom_python/cluster_utils/Snakefile`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/cluster_config.yaml` & `dexom_python-1.0.1/dexom_python/cluster_utils/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/legacy/dexom_cluster_results.py` & `dexom_python-1.0.1/dexom_python/cluster_utils/legacy/dexom_cluster_results.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/legacy/write_cluster_scripts.py` & `dexom_python-1.0.1/dexom_python/cluster_utils/legacy/write_cluster_scripts.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/slurm_example_gpr.sh` & `dexom_python-1.0.1/dexom_python/cluster_utils/slurm_example_gpr.sh`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/snakemake_utils.smk` & `dexom_python-1.0.1/dexom_python/cluster_utils/snakemake_utils.smk`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/solution_compilation.py` & `dexom_python-1.0.1/dexom_python/cluster_utils/solution_compilation.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/cluster_utils/submit.py` & `dexom_python-1.0.1/dexom_python/cluster_utils/submit.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/enum_functions/diversity_enum_functions.py` & `dexom_python-1.0.1/dexom_python/enum_functions/diversity_enum_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/enum_functions/enumeration.py` & `dexom_python-1.0.1/dexom_python/enum_functions/enumeration.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/enum_functions/icut_functions.py` & `dexom_python-1.0.1/dexom_python/enum_functions/icut_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/enum_functions/maxdist_functions.py` & `dexom_python-1.0.1/dexom_python/enum_functions/maxdist_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/enum_functions/rxn_enum_functions.py` & `dexom_python-1.0.1/dexom_python/enum_functions/rxn_enum_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/gpr_rules.py` & `dexom_python-1.0.1/dexom_python/gpr_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,27 @@
         elif expression.__class__ == Pow:
             return replace_MulMax_AddMin(expression.args[0])
         else:
             raise TypeError(f"Unsupported operation: {repr(expression)}")
             # return expression.func(*replaced_args)
 
 
-def expression2qualitative(genes, column_list=None, proportion=0.25, method='keep', significant_genes='both',
-                           save=True, outpath='geneweights'):
+def expression2qualitative(genes, column_list=None, proportion=0.25, significant_genes='both', save=True,
+                           outpath='geneweights'):
     """
     Transforms gene expression values/ gene scores into qualitative gene weights
 
     Parameters
     ----------
     genes: pandas.DataFrame or pandas.Series
         dataframe with gene IDs in the index and gene expression values in a later column
     column_list: list
         column indexes containing gene expression values to be transformed. If empty, all columns will be transformed
     proportion: tuple or float
         proportion of genes to be used for determining low and high gene expression
-    method: str
-        one of "max", "mean" or "keep". chooses how to deal with genes containing multiple conflicting expression values
     significant_genes: str
         one of "high", "low" or "both". chooses whether the conversion is applied only for the genes with
         highest expression, lowest epxression, or both
     save: bool
         if True, saves the resulting gene weights
     outpath: str
         if save=True, the .csv file will be saved to this path
@@ -58,49 +56,45 @@
     -------
     gene_weights: a pandas DataFrame containing qualitative gene weights
         (-1 for low expression, 1 for high expression, 0 for in-between or no information)
     """
     if isinstance(genes, pd.Series):
         genes = pd.DataFrame(genes)
         column_list = list(genes.columns)
-    genes = genes[genes.index == genes.index]  # eliminates NaN values in index
     if column_list is None:
         column_list = list(genes.columns)
     elif len(column_list) == 0:
         column_list = list(genes.columns)
     else:
         for col in column_list:
             if col not in genes.columns:
                 raise KeyError('Column %s is not present in gene expression file' % col)
     if isinstance(proportion, float):
         lowthreshold = proportion
         highthreshold = 1-proportion
     else:
         lowthreshold, highthreshold = proportion
+    genes = genes.reset_index().dropna()
     for col in column_list:
         genecol = genes[col].copy()
         newgenes = genes[col].copy()
-        if method == 'max':
-            for x in set(newgenes.index):
-                newgenes[x] = newgenes[x].max()
-        elif method == 'mean':
-            for x in set(newgenes.index):
-                newgenes[x] = newgenes[x].mean()
         newgenes.sort_values(inplace=True)
         genecol.sort_values(inplace=True)
+        print(genecol)
         newgenes[genecol < genecol.quantile(lowthreshold)] = -1.
         newgenes[(genecol >= genecol.quantile(lowthreshold)) & (genecol < genecol.quantile(highthreshold))] = 0.
         newgenes[genecol >= genecol.quantile(highthreshold)] = 1.
         if significant_genes == 'high':
             print('applying expression2qualitative only on genes with highest expression')
             newgenes[newgenes == -1.] = 0.
         elif significant_genes == 'low':
             print('applying expression2qualitative only on genes with lowest expression')
             newgenes[newgenes == 1.] = 0.
         genes[col] = newgenes
+    genes.set_index(genes.columns[0], inplace=True)
     for x in genes.index:
         if isinstance(x, float):
             genes.index = genes.index.astype(int)
             break
     if save:
         genes[column_list].to_csv(outpath+'.csv')
     return genes
@@ -222,15 +216,15 @@
         elif proportion[1] == '':
             proportion = (0., float(proportion[1]))
         elif len(proportion) == 2:
             proportion = (float(proportion[0]), float(proportion[1]))
         else:
             ValueError('The quantiles argument was provided in an incorrect format.')
         print(proportion)
-        genes = expression2qualitative(genes=genes, column_list=score_columns, proportion=proportion, method='keep',
+        genes = expression2qualitative(genes=genes, column_list=score_columns, proportion=proportion,
                                        significant_genes=args.significant, save=True,
                                        outpath=args.output+'_qual_geneweights')
     if len(score_columns) == 1:
         gene_weights = pd.Series(genes[score_columns[0]].values, index=genes.index)
     else:
         gene_weights = genes[score_columns].copy()
     reaction_weights = apply_gpr(model=model, gene_weights=gene_weights, save=True, filename=args.output,
```

### Comparing `dexom_python-1.0/dexom_python/imat_functions.py` & `dexom_python-1.0.1/dexom_python/imat_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/main.py` & `dexom_python-1.0.1/dexom_python/main.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/model_functions.py` & `dexom_python-1.0.1/dexom_python/model_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/pathway_enrichment.py` & `dexom_python-1.0.1/dexom_python/pathway_enrichment.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/result_functions.py` & `dexom_python-1.0.1/dexom_python/result_functions.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/dexom_python/toy_models.py` & `dexom_python-1.0.1/dexom_python/toy_models.py`

 * *Files identical despite different names*

### Comparing `dexom_python-1.0/pyproject.toml` & `dexom_python-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "dexom_python"
-version = "1.0"
+version = "1.0.1"
 description = "DEXOM implementation in python using cobrapy"
 authors = ["Maximilian Stingl <maximilian.stingl@inrae.fr>"]
 license = "GPL-3.0"
 readme="README.md"
 include=["LICENSE"]
 repository = "https://forgemia.inra.fr/metexplore/cbm/dexom-python"
 homepage = "https://forgemia.inra.fr/metexplore/cbm/dexom-python"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
-cobra = "^0.25"
+cobra = "^0.26.3"
 numpy = "1.20"
 six = "^1.16"
 scipy = "1.7"
 symengine = "^0.9.2"
 matplotlib = "^3.5.1"
 scikit-learn = "^1.0.2"
 statsmodels = "^0.13.2"
```

### Comparing `dexom_python-1.0/PKG-INFO` & `dexom_python-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: dexom-python
-Version: 1.0
+Version: 1.0.1
 Summary: DEXOM implementation in python using cobrapy
 Home-page: https://forgemia.inra.fr/metexplore/cbm/dexom-python
 License: GPL-3.0
 Author: Maximilian Stingl
 Author-email: maximilian.stingl@inrae.fr
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: cobra (>=0.25,<0.26)
+Requires-Dist: cobra (>=0.26.3,<0.27.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
 Requires-Dist: numpy (==1.20)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (==1.7)
 Requires-Dist: six (>=1.16,<2.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: symengine (>=0.9.2,<0.10.0)
```

