# Comparing `tmp/clumps-ptm-0.0.5.tar.gz` & `tmp/clumps-ptm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clumps-ptm-0.0.5.tar", last modified: Tue Feb 28 02:27:39 2023, max compression
+gzip compressed data, was "dist/clumps-ptm-0.0.6.tar", last modified: Mon Apr 17 14:31:29 2023, max compression
```

## Comparing `clumps-ptm-0.0.5.tar` & `clumps-ptm-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-02-28 02:27:39.050869 clumps-ptm-0.0.5/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1064 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/LICENSE
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     4458 2023-02-28 02:27:39.050869 clumps-ptm-0.0.5/PKG-INFO
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     3709 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/README.md
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-02-28 02:27:39.046869 clumps-ptm-0.0.5/clumps_ptm.egg-info/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     4458 2023-02-28 02:27:38.000000 clumps-ptm-0.0.5/clumps_ptm.egg-info/PKG-INFO
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      611 2023-02-28 02:27:39.000000 clumps-ptm-0.0.5/clumps_ptm.egg-info/SOURCES.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)        1 2023-02-28 02:27:38.000000 clumps-ptm-0.0.5/clumps_ptm.egg-info/dependency_links.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       54 2023-02-28 02:27:38.000000 clumps-ptm-0.0.5/clumps_ptm.egg-info/entry_points.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      151 2023-02-28 02:27:38.000000 clumps-ptm-0.0.5/clumps_ptm.egg-info/requires.txt
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       10 2023-02-28 02:27:38.000000 clumps-ptm-0.0.5/clumps_ptm.egg-info/top_level.txt
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-02-28 02:27:39.046869 clumps-ptm-0.0.5/clumpsptm/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      201 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     9669 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/__main__.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-02-28 02:27:39.046869 clumps-ptm-0.0.5/clumpsptm/clumps/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      110 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/clumps/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1594 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/clumps/engine.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1724 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/clumps/funcs.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-02-28 02:27:39.046869 clumps-ptm-0.0.5/clumpsptm/mapping/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      256 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/mapping/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     6591 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/mapping/blast.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    11913 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/mapping/ref.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)    12434 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/pdbstore.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-02-28 02:27:39.046869 clumps-ptm-0.0.5/clumpsptm/samplers/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       45 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/samplers/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1978 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/samplers/ptm.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     6833 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/utils.py
-drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-02-28 02:27:39.050869 clumps-ptm-0.0.5/clumpsptm/vis/
--rw-rw-r--   0 sanand    (1001) sanand    (1002)      109 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/vis/__init__.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     3740 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/vis/mol.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     3313 2023-02-28 01:08:23.000000 clumps-ptm-0.0.5/clumpsptm/vis/plotting.py
--rw-rw-r--   0 sanand    (1001) sanand    (1002)       38 2023-02-28 02:27:39.050869 clumps-ptm-0.0.5/setup.cfg
--rw-rw-r--   0 sanand    (1001) sanand    (1002)     1599 2023-02-28 02:27:24.000000 clumps-ptm-0.0.5/setup.py
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     1874 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/.gitignore
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)       77 2022-07-28 01:18:16.000000 clumps-ptm-0.0.6/.mailmap
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     1064 2021-01-14 19:31:23.000000 clumps-ptm-0.0.6/LICENSE
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     5140 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/PKG-INFO
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     3709 2023-02-28 01:09:29.000000 clumps-ptm-0.0.6/README.md
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/clumps_ptm.egg-info/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     5140 2023-04-17 14:31:27.000000 clumps-ptm-0.0.6/clumps_ptm.egg-info/PKG-INFO
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)      683 2023-04-17 14:31:28.000000 clumps-ptm-0.0.6/clumps_ptm.egg-info/SOURCES.txt
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)        1 2023-04-17 14:31:27.000000 clumps-ptm-0.0.6/clumps_ptm.egg-info/dependency_links.txt
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)       55 2023-04-17 14:31:27.000000 clumps-ptm-0.0.6/clumps_ptm.egg-info/entry_points.txt
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)      151 2023-04-17 14:31:27.000000 clumps-ptm-0.0.6/clumps_ptm.egg-info/requires.txt
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)       10 2023-04-17 14:31:27.000000 clumps-ptm-0.0.6/clumps_ptm.egg-info/top_level.txt
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/clumpsptm/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)      178 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/__init__.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     9817 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/__main__.py
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/clumpsptm/clumps/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)      110 2021-01-14 21:06:12.000000 clumps-ptm-0.0.6/clumpsptm/clumps/__init__.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     1594 2021-08-18 15:14:07.000000 clumps-ptm-0.0.6/clumpsptm/clumps/engine.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     1724 2021-08-18 15:25:04.000000 clumps-ptm-0.0.6/clumpsptm/clumps/funcs.py
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/clumpsptm/mapping/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)      256 2022-07-29 22:06:59.000000 clumps-ptm-0.0.6/clumpsptm/mapping/__init__.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     6619 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/mapping/blast.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)    11913 2022-07-30 16:42:36.000000 clumps-ptm-0.0.6/clumpsptm/mapping/ref.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)    16099 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/pdbstore.py
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/clumpsptm/samplers/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)       45 2022-07-31 17:35:55.000000 clumps-ptm-0.0.6/clumpsptm/samplers/__init__.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     2069 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/samplers/ptm.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     7361 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/utils.py
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/clumpsptm/vis/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)      109 2022-07-27 22:52:43.000000 clumps-ptm-0.0.6/clumpsptm/vis/__init__.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     4691 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/vis/mol.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     4742 2023-04-17 14:29:57.000000 clumps-ptm-0.0.6/clumpsptm/vis/plotting.py
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)   535777 2022-09-16 20:28:35.000000 clumps-ptm-0.0.6/clumpsptm.png
+drwxrwxr-x   0 sanand    (1001) sanand    (1002)        0 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/examples/
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)   108619 2022-07-27 03:49:31.000000 clumps-ptm-0.0.6/examples/CPTAC_Mapping_Workflow.ipynb
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)       38 2023-04-17 14:31:29.000000 clumps-ptm-0.0.6/setup.cfg
+-rw-rw-r--   0 sanand    (1001) sanand    (1002)     1599 2023-04-17 14:29:37.000000 clumps-ptm-0.0.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `clumps-ptm-0.0.5/LICENSE` & `clumps-ptm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clumps-ptm-0.0.5/PKG-INFO` & `clumps-ptm-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: clumps-ptm
-Version: 0.0.5
-Summary: CLUMPS-PTM driver gene discovery using 3D protein structure (Getz Lab).
-Home-page: https://github.com/getzlab/CLUMPS-PTM
-Author: Shankara Anand
-Author-email: sanand@broadinstitute.org
-Keywords: cancer,bioinformatics,genomics,proteomics,proteins,alphafold,post-translational modifications,phosphorylation,acetylation
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Typing :: Typed
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLUMPS-PTM
 
 An algorithm for identifying 3D clusters ("clumps") of post-translational modifications (PTMs). Developed for the Clinical Proteomic Tumor Atlas Consortium ([CPTAC](https://proteomics.cancer.gov/programs/cptac)). Full project repoistory for pan-cancer project can be found [here](https://github.com/getzlab/CPTAC_PanCan_2021).
 
 __Author__: Shankara Anand
 
 __Email__: sanand@broadinstitute.org
```

### Comparing `clumps-ptm-0.0.5/clumps_ptm.egg-info/PKG-INFO` & `clumps-ptm-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,101 @@
 Metadata-Version: 2.1
 Name: clumps-ptm
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLUMPS-PTM driver gene discovery using 3D protein structure (Getz Lab).
 Home-page: https://github.com/getzlab/CLUMPS-PTM
 Author: Shankara Anand
 Author-email: sanand@broadinstitute.org
+License: UNKNOWN
+Description: # CLUMPS-PTM
+        
+        An algorithm for identifying 3D clusters ("clumps") of post-translational modifications (PTMs). Developed for the Clinical Proteomic Tumor Atlas Consortium ([CPTAC](https://proteomics.cancer.gov/programs/cptac)). Full project repoistory for pan-cancer project can be found [here](https://github.com/getzlab/CPTAC_PanCan_2021).
+        
+        __Author__: Shankara Anand
+        
+        __Email__: sanand@broadinstitute.org
+        
+        _Requires Python 3.6.0 or higher._
+        
+        ## Installation
+        
+        ##### PIP
+        
+        `pip3 install clumps-ptm`
+        
+        or
+        
+        ##### Git Clone
+        
+        ```
+        git clone git@github.com:getzlab/CLUMPS-PTM.git
+        cd CLUMPS-PTM
+        pip3 install -e .
+        ```
+        
+        ## Use
+        
+        CLUMPS-PTM has 3 general phases of analysis:
+        1. __Mapping__: taking input PTM proteomic data and mapping them onto PDB structural data.
+        
+          Mapping relies on the source data and involves programmatic calling of `blastp+` depending on the source data-base to map to UNIPROT and ultimately PDB structures. An example notebook that walks through the mapping and demonstrates use of `clumps-ptm` API for running these steps programmatically can be found [here](https://github.com/getzlab/CLUMPS-PTM/blob/main/examples/CPTAC_Mapping_Workflow.ipynb). Once the mapping is performed once for a new data-set, the mapping file is used as the `--maps` flag in `clumpsptm` command (below).
+        
+        2. __CLUMPS__: running the algorithm for identifying statistically significant clustering of PTM sites.
+        
+          CLUMPS-PTM was designed for use with differential expression proteomic data. Due to the nature of drop-out in Mass-Spectrometry data, we opt for using broad changes in PTM levels across sample groups to interrogate "clumping" of modifications. Thus, the input requires out-put from Limma-Voom differential expression.
+        
+        ```{python}
+        usage: clumpsptm [-h] -i INPUT -m MAPS -w WEIGHT -s PDBSTORE [-o OUTPUT_DIR]
+                         [-x XPO] [--threads THREADS] [-v]
+                         [-f [FEATURES [FEATURES ...]]] [-g GROUPING] [-q]
+                         [--min_sites MIN_SITES] [--subset {positive,negative}]
+                         [--protein_id PROTEIN_ID] [--site_id SITE_ID] [--alphafold]
+                         [--alphafold_threshold ALPHAFOLD_THRESHOLD]
+        
+        Run CLUMPS-PTM.
+        
+        optional arguments:
+          -h, --help            show this help message and exit
+          -i INPUT, --input INPUT
+                                <Required> Input file.
+          -m MAPS, --maps MAPS  <Required> Mapping with index as indices that overlap
+                                input.
+          -w WEIGHT, --weight WEIGHT
+                                <Required> Weighting for CLUMPS-PTM (ex. logFC).
+          -s PDBSTORE, --pdbstore PDBSTORE
+                                <Required> path to PDBStore directory.
+          -o OUTPUT_DIR, --output_dir OUTPUT_DIR
+                                Output directory.
+          -x XPO, --xpo XPO     Soft threshold parameter for truncated Gaussian.
+          --threads THREADS     Number of threads for sampling.
+          -v, --verbose         Verbosity.
+          -f [FEATURES [FEATURES ...]], --features [FEATURES [FEATURES ...]]
+                                Assays to subset for.
+          -g GROUPING, --grouping GROUPING
+                                DE group to use.
+          -q, --use_only_significant_sites
+                                Only use significant sites for CLUMPS-PTM.
+          --min_sites MIN_SITES
+                                Minimum number of sites.
+          --subset {positive,negative}
+                                Subset sites.
+          --protein_id PROTEIN_ID
+                                Unique protein id in input.
+          --site_id SITE_ID     Unique site id in input.
+          --alphafold           Run using alphafold structures.
+          --alphafold_threshold ALPHAFOLD_THRESHOLD
+                                Threshold confidence level for alphafold sites.
+                                
+        ```
+        
+        3. __Post-Processing__: post-processing (FDR correction) \& visualization in Pymol.
+        
 Keywords: cancer,bioinformatics,genomics,proteomics,proteins,alphafold,post-translational modifications,phosphorylation,acetylation
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CLUMPS-PTM
-
-An algorithm for identifying 3D clusters ("clumps") of post-translational modifications (PTMs). Developed for the Clinical Proteomic Tumor Atlas Consortium ([CPTAC](https://proteomics.cancer.gov/programs/cptac)). Full project repoistory for pan-cancer project can be found [here](https://github.com/getzlab/CPTAC_PanCan_2021).
-
-__Author__: Shankara Anand
-
-__Email__: sanand@broadinstitute.org
-
-_Requires Python 3.6.0 or higher._
-
-## Installation
-
-##### PIP
-
-`pip3 install clumps-ptm`
-
-or
-
-##### Git Clone
-
-```
-git clone git@github.com:getzlab/CLUMPS-PTM.git
-cd CLUMPS-PTM
-pip3 install -e .
-```
-
-## Use
-
-CLUMPS-PTM has 3 general phases of analysis:
-1. __Mapping__: taking input PTM proteomic data and mapping them onto PDB structural data.
-
-  Mapping relies on the source data and involves programmatic calling of `blastp+` depending on the source data-base to map to UNIPROT and ultimately PDB structures. An example notebook that walks through the mapping and demonstrates use of `clumps-ptm` API for running these steps programmatically can be found [here](https://github.com/getzlab/CLUMPS-PTM/blob/main/examples/CPTAC_Mapping_Workflow.ipynb). Once the mapping is performed once for a new data-set, the mapping file is used as the `--maps` flag in `clumpsptm` command (below).
-
-2. __CLUMPS__: running the algorithm for identifying statistically significant clustering of PTM sites.
-
-  CLUMPS-PTM was designed for use with differential expression proteomic data. Due to the nature of drop-out in Mass-Spectrometry data, we opt for using broad changes in PTM levels across sample groups to interrogate "clumping" of modifications. Thus, the input requires out-put from Limma-Voom differential expression.
-
-```{python}
-usage: clumpsptm [-h] -i INPUT -m MAPS -w WEIGHT -s PDBSTORE [-o OUTPUT_DIR]
-                 [-x XPO] [--threads THREADS] [-v]
-                 [-f [FEATURES [FEATURES ...]]] [-g GROUPING] [-q]
-                 [--min_sites MIN_SITES] [--subset {positive,negative}]
-                 [--protein_id PROTEIN_ID] [--site_id SITE_ID] [--alphafold]
-                 [--alphafold_threshold ALPHAFOLD_THRESHOLD]
-
-Run CLUMPS-PTM.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -i INPUT, --input INPUT
-                        <Required> Input file.
-  -m MAPS, --maps MAPS  <Required> Mapping with index as indices that overlap
-                        input.
-  -w WEIGHT, --weight WEIGHT
-                        <Required> Weighting for CLUMPS-PTM (ex. logFC).
-  -s PDBSTORE, --pdbstore PDBSTORE
-                        <Required> path to PDBStore directory.
-  -o OUTPUT_DIR, --output_dir OUTPUT_DIR
-                        Output directory.
-  -x XPO, --xpo XPO     Soft threshold parameter for truncated Gaussian.
-  --threads THREADS     Number of threads for sampling.
-  -v, --verbose         Verbosity.
-  -f [FEATURES [FEATURES ...]], --features [FEATURES [FEATURES ...]]
-                        Assays to subset for.
-  -g GROUPING, --grouping GROUPING
-                        DE group to use.
-  -q, --use_only_significant_sites
-                        Only use significant sites for CLUMPS-PTM.
-  --min_sites MIN_SITES
-                        Minimum number of sites.
-  --subset {positive,negative}
-                        Subset sites.
-  --protein_id PROTEIN_ID
-                        Unique protein id in input.
-  --site_id SITE_ID     Unique site id in input.
-  --alphafold           Run using alphafold structures.
-  --alphafold_threshold ALPHAFOLD_THRESHOLD
-                        Threshold confidence level for alphafold sites.
-                        
-```
-
-3. __Post-Processing__: post-processing (FDR correction) \& visualization in Pymol.
```

### Comparing `clumps-ptm-0.0.5/clumps_ptm.egg-info/SOURCES.txt` & `clumps-ptm-0.0.6/clumps_ptm.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+.gitignore
+.mailmap
 LICENSE
 README.md
+clumpsptm.png
 setup.py
 clumps_ptm.egg-info/PKG-INFO
 clumps_ptm.egg-info/SOURCES.txt
 clumps_ptm.egg-info/dependency_links.txt
 clumps_ptm.egg-info/entry_points.txt
 clumps_ptm.egg-info/requires.txt
 clumps_ptm.egg-info/top_level.txt
@@ -17,8 +20,9 @@
 clumpsptm/mapping/__init__.py
 clumpsptm/mapping/blast.py
 clumpsptm/mapping/ref.py
 clumpsptm/samplers/__init__.py
 clumpsptm/samplers/ptm.py
 clumpsptm/vis/__init__.py
 clumpsptm/vis/mol.py
-clumpsptm/vis/plotting.py
+clumpsptm/vis/plotting.py
+examples/CPTAC_Mapping_Workflow.ipynb
```

### Comparing `clumps-ptm-0.0.5/clumpsptm/__main__.py` & `clumps-ptm-0.0.6/clumpsptm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+# -- import packages: --------------------------------------------------------------------
 import pandas as pd
 import argparse
 import numpy as np
 import os
+from agutil.parallel import parallelize2
+
+# -- import local dependencies: ----------------------------------------------------------
 from .clumps import transform_dx, init_alg, clumps
 from .pdbstore import PdbStore, AlphaStore
 from .samplers import PTMSampler, PTMAlphaSampler
 from .utils import generate_clumpsptm_output
-from agutil.parallel import parallelize2
 
 def main():
     parser = argparse.ArgumentParser(description='Run CLUMPS-PTM.')
     parser.add_argument('-i', '--input', required=True, help='<Required> Input file.')
     parser.add_argument('-m','--maps', required=True, help='<Required> Mapping with index as indices that overlap input.')
     parser.add_argument('-w', '--weight', required=True, help='<Required> Weighting for CLUMPS-PTM (ex. logFC).')
     parser.add_argument('-s','--pdbstore',required=True, help='<Required> path to PDBStore directory.')
     parser.add_argument('-o','--output_dir', default=".", help='Output directory.')
-    parser.add_argument('-x', '--xpo', default=[3, 4.5, 6, 8, 10], type=list,
-        help='Soft threshold parameter for truncated Gaussian.')
+    parser.add_argument('-x', '--xpo', default=[6], type=list, help='Soft distance threshold (t).')
     parser.add_argument('--threads', type=int, default=1, help='Number of threads for sampling.')
-    parser.add_argument('-v', '--verbose', action='store_true', default=False, help='Verbosity.')
     parser.add_argument('-f', '--features', nargs="*", default=None, help='Assays to subset for.')
     parser.add_argument('-g', '--grouping', default=None, help='DE group to use.')
     parser.add_argument('-q', '--use_only_significant_sites', action='store_true', help='Only use significant sites for CLUMPS-PTM.')
     parser.add_argument('--min_sites', default=3, help='Minimum number of sites.')
     parser.add_argument('--subset', default=None, help='Subset sites.', choices=('positive','negative'))
     parser.add_argument('--protein_id', default="accession_number", help='Unique protein id in input.')
     parser.add_argument('--site_id', default="variableSites", help='Unique site id in input.')
     parser.add_argument('--alphafold', action='store_true', default=False, help='Run using alphafold structures.')
     parser.add_argument('--alphafold_threshold', type=float, default=75, help='Threshold confidence level for alphafold sites.')
+    parser.add_argument('-v', '--verbose', action='store_true', default=False, help='Verbosity.')
     args = parser.parse_args()
 
     print("---------------------------------------------------------")
     print("------------------ C L U M P S - P T M ------------------")
     print("---------------------------------------------------------")
 
     # ----------------------------------
@@ -173,15 +175,15 @@
 
             # Run CLUMPS
             pval, wap_scr, niter = clumps(init_dict, sam, DDt, args.xpo, max_rand=1e4, use_booster=False)
 
             # Output
             # print("     > {} - {} | p-value: {}".format(acc, feature, sum(pval) / (5*niter)))
             _inputs_df.loc[:,"clumpsptm_niter"] = niter
-            _inputs_df.loc[:,"clumpsptm_pval"] = sum(pval) / (5*niter)
+            _inputs_df.loc[:,"clumpsptm_pval"] = sum(pval) / (len(pval)*niter)
 
             res_input = [str(x) for x in _inputs_df['pdb_res_i']]
             res_sample = [str(x) for x in sam.ptm]
 
             _inputs_df.loc[:,"clumpsptm_input"] = "+".join(res_input)
             _inputs_df.loc[:,"clumpsptm_sample"] = "+".join(res_sample)
             _inputs_df.loc[:,"clumpsptm_input_n"] = len(res_input)
@@ -202,19 +204,19 @@
             try:
                 _run("ptm")
             except:
                 print("     > ERROR for {} - {}".format(acc, "ptm"))
 
     print("   * running using {} threads".format(args.threads))
 
-    # TODO: CHANGE
+    # Protein IDs to run
     protein_ids = np.unique(de_df[args.protein_id])
 
     tmp = [run_clumps(prot) for prot in protein_ids]
-    results = [callback() for callback in tmp]
+    _ = [callback() for callback in tmp]
 
     # ----------------------------------
     # Generate Output File
     # ----------------------------------
     results_df = generate_clumpsptm_output(
         os.path.join(args.output_dir, "clumpsptm"),
         args.protein_id,
```

### Comparing `clumps-ptm-0.0.5/clumpsptm/clumps/engine.py` & `clumps-ptm-0.0.6/clumpsptm/clumps/engine.py`

 * *Files identical despite different names*

### Comparing `clumps-ptm-0.0.5/clumpsptm/clumps/funcs.py` & `clumps-ptm-0.0.6/clumpsptm/clumps/funcs.py`

 * *Files identical despite different names*

### Comparing `clumps-ptm-0.0.5/clumpsptm/mapping/blast.py` & `clumps-ptm-0.0.6/clumpsptm/mapping/blast.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,16 @@
     def __str__(self):
         return "Blastp+ for {} | {} hits".format(self.query, self.nhits)
 
 def load_accession_blast(a_num, unique_sites_df):
     """
     a_num
     """
+    import numpy as np
+    
     an_dict = {}
     an_dict['accession_no'] = a_num
 
     if scraped_accessions[a_num] is not None:
         an_dict['accession_no_matched'] = scraped_accessions[a_num].split('/')[-1].split('.seq')[0]
 
         uns = unique_sites_df.loc[a_num,'site_position']
```

### Comparing `clumps-ptm-0.0.5/clumpsptm/mapping/ref.py` & `clumps-ptm-0.0.6/clumpsptm/mapping/ref.py`

 * *Files identical despite different names*

### Comparing `clumps-ptm-0.0.5/clumpsptm/pdbstore.py` & `clumps-ptm-0.0.6/clumpsptm/pdbstore.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,102 @@
-import importlib,sys
+# -- import packages: --------------------------------------------------------------------
 import os
-import pandas as pd
 import numpy as np
 from collections import defaultdict
 from typing import Union
 from scipy.spatial.distance import euclidean
-from .utils import AMINO_ACID_MAP, gunzipper
 from Bio import pairwise2
 import subprocess
 import glob
 from agutil.parallel import parallelize2
 
+# -- import local dependencies: ----------------------------------------------------------
+from .utils import AMINO_ACID_MAP, gunzipper
+from .mapping import Blast
+from .clumps import transform_dx
+
 class PdbStore(object):
     """
-    Protein Data Bank Direcotry Store
+    Protein Data Bank Directory Store
     ------------------
     This object is used to keep track of protein data bank files
     that are downloaded in a reference directory.
     """
     def __init__(self, path):
         """
-        Args:
-            * path: PDB directory
+        Parameters:
+        -----------
+        path [ required ]
+            path to pdb directory
+            type: str
 
         """
         self.pdb_root_dir = path
         self.pdb_dir = os.path.join(path, 'ftp.wwpdb.org/pub/pdb/data/structures/divided/pdb/')
 
     def __str__(self):
         return "PDBStore\n   * {} PDB files downloaded\n   * Directory Path: {}".format(len(self.downloaded_pdbs), self.pdb_root_dir)
 
     @property
     def downloaded_pdbs(self):
         """
-        Get Downloaded Structures.
-        ------------------
-        Iterates through pdb structure direcotry to find what
-        pdbs are already downloaded. Returns a set of downloaded PDBs.
+        Get Downloaded Structures: 
+        iterates through pdb structure directory to find downloaded pdbs. 
+        
+        Returns:
+        --------
+        downloaded pdbs
+            type: set
         """
         try:
             return {
                     i[3:7]
                     for j in os.listdir(self.pdb_dir)
                     for i in os.listdir(os.path.join(self.pdb_dir, j))
                     if i.endswith('.ent.gz') and os.path.getsize(os.path.join(self.pdb_dir, j, i)) > 0
                    }
         except:
             return set()
 
     def missing_pdbs(self, pdbs: set):
         """
-        Missing PDBs
-        ------------------
-        Set difference of input pdbs and all downloaded pdbs.
+        Missing PDBs: set difference of input pdbs and all downloaded pdbs.
+
+        Parameters:
+        -----------
+        pdbs
+            set of pdbs to query
+            type: set
 
-        Args:
-            * pdbs: set of PDBs
+        Returns:
+        --------
+        missing pdb structures
+            type: set
         """
         return pdbs - self.downloaded_pdbs
 
-    def download_missing_pdbs(self, pdbs_to_download: Union[set,list], n_threads=15):
+    def download_missing_pdbs(self, pdbs_to_download: Union[set,list], n_threads: int = 15):
         """
         Download Missing PDBs
-        ------------------
-        Args:
-            * pdbs_to_download: a list or set of PDBs to download
-            * n_threads: number of threads to use for downloads
+
+        Parameters:
+        -----------
+        pdbs_to_download
+            list or set of PDBs to download
+            type: [set, list]
+
+        n_threads [optional]
+            number of threads to use for download
+            type: int
+            default: 15
+
+        Returns:
+        --------
+        error msgs from downloads
+            type: set
         """
         if isinstance(pdbs_to_download, list):
             pdbs_to_download = set(pdbs_to_download)
 
         out_dir = self.pdb_root_dir
 
         @parallelize2(maximum=n_threads)
@@ -87,57 +114,115 @@
         tmp = [dl_pdb(pdb) for pdb in pdbs_to_download]
         pdb_err = {callback() for callback in tmp}
 
         print("   * Downloaded {} / {} successfully.".format(len(pdbs_to_download-pdb_err) , len(pdbs_to_download)))
 
         return pdb_err
 
-    def load(self, pdb, chain=None):
+    def load(self, pdb: str, chain: str = None):
         """
-        Load residues - amino acids.
+        Load PDBstream from structure.
+
+        Parameters:
+        -----------
+        pdb
+            pdb string
+            type: str
+
+        chain [optional]
+            chain string
+            type: str
 
         Returns:
-            * PDBStream
+        --------
+        loaded pdb stream
+            type: PDBStream
+
         """
         from prody import parsePDBStream
 
         pdb_file = os.path.join(self.pdb_dir, pdb[1:3], "pdb{}.ent.gz".format(pdb))
 
         with gunzipper(pdb_file) as pfile:
             aa = parsePDBStream(pfile, chain=chain)
 
         return aa
 
-    def load_header(self, pdb, chain=None):
+    def load_header(self, pdb: str, chain: str = None):
         """
-        Load PDB header
+        Load PDBHeader from structure.
+
+        Parameters:
+        -----------
+        pdb
+            pdb string
+            type: str
+
+        chain [optional]
+            chain string
+            type: str
 
         Returns:
-            * dict
+        --------
+        loaded pdb header
+            type: PDBHeader
         """
         from prody import parsePDBHeader
 
         pdb_file = os.path.join(self.pdb_dir, pdb[1:3], "pdb{}.ent.gz".format(pdb))
         return parsePDBHeader(pdb_file)
 
-    def load_rd(self, pdb, chain=None):
+    def load_rd(self, pdb: str, chain: str = None):
         """
-        Load residue dict
+        Load residue dictionary from pdb/chain.
+
+        Parameters:
+        -----------
+        pdb
+            pdb str
+            type: str
+
+        chain [optional]
+            chain str
+            type: str
+
+        Returns:
+        --------
+        residue dictionary mapping residue number -> residue name
+            type: dict
         """
         aa = self.load(pdb,chain)
         res_map = dict(zip(aa.getResnums(),aa.getResnames()))
         return {k:v for k,v in res_map.items() if v in AMINO_ACID_MAP}
 
-    def load_dm(self, pdb, chain=None, point='centroid', return_centroid_coord=False):
+    def load_dm(self, pdb: str, chain:str = None, return_centroid_coord: bool = False):
         """
-        Load distance matrix for pdb.
-        """
-        from scipy.spatial.distance import euclidean
-        import numpy as np
+        Load distance matrix for pdb/chain.
+
+        Parameters:
+        -----------
+        pdb
+            pdb str
+            type: str
+
+        chain [optional]
+            chain str
+            type: str
+
+        return_centroid_coord [optional]
+            whether or not to include centroid coordinate
+            type: bool
+            default: False
 
+        Returns:
+        --------
+        euclidean distance matrix, pdb residue IDs, idx to AA mapping, and centroid (optional)
+            type: tuple
+        
+        """
         aa = self.load(pdb,chain=chain)
 
         xx = aa.getResnums()
         yy = aa.getCoords()
         zz = aa.getResnames()
 
         pdb_resids = {}
@@ -180,19 +265,30 @@
 
 class AlphaStore(object):
     """
     Alpha Fold Data Bank Directory Store
     ------------------
     This object is used to keep track of protein data bank files
     that are downloaded in a reference directory.
+
+        $ mkdir alphafold_structures
+        $ cd alphafold_structures
+        $ wget https://ftp.ebi.ac.uk/pub/databases/alphafold/latest/UP000005640_9606_HUMAN_v4.tar
+        $ tar -xf UP000005640_9606_HUMAN_v4.tar
+        $ cd ..
+        $ AlphaStore.("alphafold_structures")
+
     """
-    def __init__(self, path):
+    def __init__(self, path: str):
         """
-        Args:
-            * path: PDB directory
+        Parameters:
+        -----------
+        path
+            path to directory with pdbfiles downloaded
+            type: str
 
         """
         self.pdb_dir = path
         self.uniprot_dict = {x.split("-")[1]:x for x in glob.glob(os.path.join(self.pdb_dir, "*.pdb.gz"))}
 
         try:
             self.tar_file = glob.glob(os.path.join(self.pdb_dir, "*.tar"))[0]
@@ -202,49 +298,82 @@
 
     def __str__(self):
         return "AlphaStore\n   * {} PDB files downloaded\n   * Directory Path: {}".format(len(self.uniprots), self.pdb_dir)
 
     @property
     def uniprots(self):
         """
-        Return downloaded uniprot models.
+        Downloaded uniprot proteins.
+
+        Returns:
+        --------
+        uniprots
+            type: list
+
         """
         return list(self.uniprot_dict.keys())
 
-    def load(self, uniprot):
+    def load(self, uniprot: str):
         """
-        Load residues - amino acids.
+        Load PDBStream from uniprot string.
+
+        Parameters:
+        -----------
+        uniprot
+            uniprot str
+            type: str
 
         Returns:
-            * PDBStream
+        --------
+        AlphaFold structure stream
+            type: PDBStream
         """
         from prody import parsePDBStream
 
         pdb_file = self.uniprot_dict[uniprot]
 
         with gunzipper(pdb_file) as pfile:
             aa = parsePDBStream(pfile)
 
         return aa
 
-    def load_header(self, uniprot):
+    def load_header(self, uniprot: str):
         """
-        Load PDB header
+        Load AlphaFold PDBHeader from uniprot string.
+
+        Parameters:
+        -----------
+        uniprot
+            uniprot str
+            type: str
 
         Returns:
-            * dict
+        --------
+        AlphaFold structure header
+            type: PDBHeader
         """
         from prody import parsePDBHeader
 
         pdb_file = self.uniprot_dict[uniprot]
         return parsePDBHeader(pdb_file)
 
-    def scrape_header(self, uniprot):
+    def scrape_header(self, uniprot: str):
         """
-        Scrape PDB header. Just gets alignment information for pdb.
+        Scrape PDB header to get database alignment information.
+
+        Parameters:
+        -----------
+        uniprot
+            uniprot str
+            type: str
+
+        Returns:
+        --------
+        Header information for AlphaFold structure
+            type: dict
         """
         import re
         import gzip
 
         header = dict()
         header[uniprot] = dict()
         
@@ -256,17 +385,34 @@
                     header[uniprot]["db_first_from"] = int(l[3])
                     header[uniprot]["db_first_to"] = int(l[8])
                     header[uniprot]["db_accession"] = l[6]
                     header[uniprot]["db_ref"] = l[5].replace("UNP","UniProt")
 
         return header
 
-    def load_rd(self, uniprot, return_model_confidence=False):
+    def load_rd(self, uniprot: str , return_model_confidence: bool = False):
         """
-        Load residue dict
+        Load residue dictionary from uniprot.
+
+        Parameters:
+        -----------
+        uniprot
+            uniprot str
+            type: str
+
+        return_model_confidence [optional]
+            flag to include model confidence (pLDDT)
+            type: bool
+            default: False
+            note: see https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3799472/
+
+        Returns:
+        --------
+        residue dictionary mapping residue number -> residue name, model confidence (optional)
+            type: [dict, tuple]
         """
         aa = self.load(uniprot)
         res_map = dict(zip(aa.getResnums(),aa.getResnames()))
         rd = {k:v for k,v in res_map.items() if v in AMINO_ACID_MAP}
 
         if return_model_confidence:
             xx = aa.getResnums()
@@ -274,21 +420,34 @@
             model_confidence = {}
             for idx,num in enumerate(xx):
                 model_confidence[num] = bb[idx]
             return rd, model_confidence
         else:
             return rd
 
-    def load_dm(self, uniprot, point='centroid', return_centroid_coord=False):
+    def load_dm(self, uniprot, return_centroid_coord=False):
         """
-        Load distance matrix for pdb.
-        """
-        from scipy.spatial.distance import euclidean
-        import numpy as np
+        Load AlphaFold distance matrix from uniprot.
+
+        Parameters:
+        -----------
+        uniprot
+            uniprot str
+            type: str
+
+        return_centroid_coord [optional]
+            flag to include centroid cooridnate
+            type: bool
+            default: False
 
+        Returns:
+        --------
+        euclidean distance matrix, pdb residue IDs, idx to AA mapping, model_confidence, and centroid (optional)
+            type: tuple
+        """
         aa = self.load(uniprot)
 
         xx = aa.getResnums()
         yy = aa.getCoords()
         zz = aa.getResnames()
 
         # Model confidence
@@ -336,44 +495,43 @@
             return (D, pdb_resids, mapped_pdb_to_aa, model_confidence)
 
 class AccessionNo(object):
     """
     Accession Number Object.
     ---------------
     Stores Accession Number -> PDB mapping.
+
+    <<<<DEPRECATED>>>>
     """
     def __init__(
         self,
         accession_number,
         blast_dir="ref/refseq_blasted",
         pdb_dir="../../../getzlab-CLUMPS2/clumps/db/ref/pdbs"
     ):
-        """
-        Args:
-            * x
-        """
+        """Previously used class."""
         xpo_param=(3,4.5,6,8,10)
 
         self.accession_number = accession_number
         self.blast_dir = blast_dir
         self.pdb_dir = pdb_dir
 
         # Get Blasted PDB
-        self.blast = clumpsptm.mp.Blast(os.path.join(self.blast_dir,"{}.blasted.seq.gz".format(self.accession_number)))
+        self.blast = Blast(os.path.join(self.blast_dir,"{}.blasted.seq.gz".format(self.accession_number)))
         self.hit = self.blast.hits.iloc[0]
         self.pdb,self.chain = self.hit['Hit_def'].split(' ')[0].split("_")
 
         # Get PDB Info
-        pdbstore = clumpsptm.PdbStore(self.pdb_dir)
+        pdbstore = PdbStore(self.pdb_dir)
         self.D,self.x,self.pdb_resnames = pdbstore.load_dm(self.pdb,self.chain)
-        self.DDt = clumpsptm.transform_dx(self.D, xpo_param)
+        self.DDt = transform_dx(self.D, xpo_param)
 
         # Align PDB Fasta to PDB SEQATOMS
         self.pdb_structure_idx = np.arange(max(list(self.pdb_resnames.keys())))+1
-        self.pdb_structure_res = np.array(["."]*pdb_idx.shape[0])
+        self.pdb_structure_res = np.array(["."]*self.pdb_structure_idx.shape[0])
 
         for idx in self.pdb_structure_idx-1:
             pdb_i = self.pdb_structure_idx[idx]
             try:
                 self.pdb_structure_res[idx] = AMINO_ACID_MAP[list(self.pdb_resnames[pdb_i])[0]]
             except:
                 pass
```

### Comparing `clumps-ptm-0.0.5/clumpsptm/samplers/ptm.py` & `clumps-ptm-0.0.6/clumpsptm/samplers/ptm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -- import packages: --------------------------------------------------------------------
 import numpy as np
 import random
 
 class PTMSampler(object):
     """
     Samples only modifiable residues.
     --------------------------
```

### Comparing `clumps-ptm-0.0.5/clumpsptm/utils.py` & `clumps-ptm-0.0.6/clumpsptm/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+# -- import packages: --------------------------------------------------------------------
 import os
-from gzip import GzipFile
 import contextlib
 import tempfile
 import subprocess
 import glob
 import pandas as pd
 import numpy as np
 
@@ -26,21 +26,22 @@
     gz_file [ required ]
         gzipped file
         type: str
 
     Returns:
     --------
     temporary file
-    tempfile.NamedTemporaryFile
+        type: tempfile.NamedTemporaryFile
+
     """
     with tempfile.NamedTemporaryFile('r', suffix=os.path.splitext(gz_file)[1]) as temp_file:
         subprocess.check_call("gzip -dc {} >> {}".format(gz_file, temp_file.name), executable='/bin/bash', shell=True)
         yield temp_file
 
-def add_corrected_fdr(results_df: pd.DataFrame, thresh_num: float = 0.25):
+def add_corrected_fdr(results_df: pd.DataFrame, thresh_num: float = 0.1, weight_thresh_by_n: bool = False):
     """
     Creates corrected FDR for clumps-ptm results.
     Due to the sparsity of PTM modifications possible on a given
     protein, we perform FDR on the subset of structures that can
     yield a theoretical p-value < threshold
 
     Parameters:
@@ -49,31 +50,41 @@
         results dataframe from clumps-ptm
         type: pd.DataFrame
 
     thresh_num [ required ]
         threshold for minimum theoretical p-value to consider for FDR
         type: float
 
+    weight_thresh_by_n [ required ]
+        whether to weight threshold for minimum theoretical p-value by hypothesis tested
+        type: bool
+
     Returns:
     --------
     results_df with additional columns for corrected FDR
-    pd.DataFrame
+        type: pd.DataFrame
 
     """
     from scipy.special import comb
     from statsmodels.stats.multitest import multipletests
 
     corr_df = list()
 
     for sam in np.unique(results_df['clumpsptm_sampler']):
         _df_sam = results_df[results_df['clumpsptm_sampler']==sam].copy()
 
         _df_sam['fdr_max_pval'] = _df_sam.apply(lambda row: 1/comb(row['clumpsptm_sample_n'], row['clumpsptm_input_n']), 1)
-        _df_sam['fdr_pass'] = _df_sam['fdr_max_pval'] <= thresh_num
+        if weight_thresh_by_n:
+            _df_sam['fdr_thresh'] = thresh_num / _df_sam.shape[0]
+            _df_sam['fdr_pass'] = _df_sam['fdr_max_pval'] <= thresh_num / _df_sam.shape[0]
+        else:
+            _df_sam['fdr_thresh'] = thresh_num
+            _df_sam['fdr_pass'] = _df_sam['fdr_max_pval'] <= thresh_num
         _df_sam['fdr_corr'] = 1
+
         _,_df_sam.loc[_df_sam['fdr_pass'],'fdr_corr'],_,_ = multipletests(
             _df_sam[_df_sam['fdr_pass']]['clumpsptm_pval'], method='fdr_bh',
         )
 
         corr_df.append(_df_sam)
 
     return pd.concat(corr_df)
@@ -110,15 +121,15 @@
     thresh_min_pval [ optional ]
         whether to threshold empirical pvalues = 0 (due to insufficient permutations) to 1/n_permutations^e-1
         type: bool
 
     Returns:
     --------
     results dataframe
-    pd.DataFrame
+        type: pd.DataFrame
 
     """
     def _collapse_sites(df):
         """Collapser per feature type."""
         from statsmodels.stats.multitest import multipletests
 
         if alphafold:
```

### Comparing `clumps-ptm-0.0.5/clumpsptm/vis/mol.py` & `clumps-ptm-0.0.6/clumpsptm/vis/mol.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+# -- import packages: --------------------------------------------------------------------
 import os
-import sys
 from typing import Union
 import pandas as pd
 from tqdm import tqdm
 
 def buildPymol(
     pdb: str,
     chain: str,
@@ -11,15 +11,57 @@
     phosph_residues: Union[None, list] = None,
     acetyl_residues: Union[None, list] = None,
     chain_color: str = 'palecyan',
     phosph_color: str = 'deeppurple',
     acetyl_color: str = 'hotpink'
     ):
     """
-    Build Pymol Session
+    Create a PyMol session using python API.
+
+    Parameters:
+    -----------
+    pdb
+        pdb protein name
+        type: str
+    
+    chain
+        chain of pdb structure
+        type: str
+
+    session_name
+        file name to save as (will append .pse)
+        type: str
+
+    phosph_residues [optional]
+        protein residues to highlight in pymol structure
+        type: [None, list]
+
+    acetyl_residues [optional]
+        protein residues to highlight in pymol structure
+        type: [None, list]
+
+    chain_color [optional]
+        color of entire protein structure
+        type: str
+        default: palecyan
+
+    phosph_color [optional]
+        color of phosph highlighted spheres
+        type: str
+        default: deeppurple
+
+    acetyl_color [optional]
+        color of acetyl highlighted spheres
+        type: str
+        default: hotpink
+
+    Returns:
+    --------
+    None
+
     """
     import __main__
     import tempfile
     import os
 
     # Quiet and no GUI
     __main__.pymol_argv = [ 'pymol', '-qc']
```

### Comparing `clumps-ptm-0.0.5/setup.py` & `clumps-ptm-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Load the README file.
 with open(file="README.md", mode="r") as readme_handle:
     long_description = readme_handle.read()
 
 setup(
     name='clumps-ptm',
     author='Shankara Anand',
-    version="0.0.5",
+    version="0.0.6",
     author_email='sanand@broadinstitute.org',
     description='CLUMPS-PTM driver gene discovery using 3D protein structure (Getz Lab).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/getzlab/CLUMPS-PTM',
     keywords='cancer, bioinformatics, genomics, proteomics, proteins, alphafold, post-translational modifications, phosphorylation, acetylation',
     python_requires='>=3.6',
```

