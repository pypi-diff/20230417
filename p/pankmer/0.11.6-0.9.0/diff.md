# Comparing `tmp/pankmer-0.11.6.tar.gz` & `tmp/pankmer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pankmer-0.11.6.tar", last modified: Sun Apr 16 22:51:51 2023, max compression
+gzip compressed data, was "pankmer-0.9.0.tar", last modified: Sat Feb  4 08:39:36 2023, max compression
```

## Comparing `pankmer-0.11.6.tar` & `pankmer-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,34 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-04-16 22:51:51.423071 pankmer-0.11.6/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1582 2023-02-04 07:58:07.000000 pankmer-0.11.6/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5007 2023-04-16 22:51:51.422423 pankmer-0.11.6/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4260 2023-04-16 20:15:17.000000 pankmer-0.11.6/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-04-16 22:51:51.406187 pankmer-0.11.6/pankmer.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5007 2023-04-16 22:51:51.000000 pankmer-0.11.6/pankmer.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      685 2023-04-16 22:51:51.000000 pankmer-0.11.6/pankmer.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-04-16 22:51:51.000000 pankmer-0.11.6/pankmer.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       49 2023-04-16 22:51:51.000000 pankmer-0.11.6/pankmer.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       71 2023-04-16 22:51:51.000000 pankmer-0.11.6/pankmer.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        8 2023-04-16 22:51:51.000000 pankmer-0.11.6/pankmer.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1178 2023-04-16 22:50:20.000000 pankmer-0.11.6/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-04-16 22:51:51.423211 pankmer-0.11.6/setup.cfg
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      450 2023-01-16 17:12:04.000000 pankmer-0.11.6/setup.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-04-16 22:51:51.401337 pankmer-0.11.6/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-04-16 22:51:51.420256 pankmer-0.11.6/src/pankmer/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      294 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1832 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/adjacency_matrix.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3009 2023-02-04 07:49:15.000000 pankmer-0.11.6/src/pankmer/clustermap.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      907 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/count.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1493 2023-02-04 07:49:15.000000 pankmer-0.11.6/src/pankmer/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    17939 2023-02-04 07:49:15.000000 pankmer-0.11.6/src/pankmer/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      213 2023-02-04 07:49:15.000000 pankmer-0.11.6/src/pankmer/get_lower_bound.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      364 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/gzip_agnostic_open.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    13154 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/index.pyx
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    50267 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/pankmer.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      355 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/populate.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    17507 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/reg_coverage.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3950 2023-04-16 20:15:18.000000 pankmer-0.11.6/src/pankmer/saturation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6062 2023-02-04 07:49:15.000000 pankmer-0.11.6/src/pankmer/tree.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1794 2023-04-16 22:50:20.000000 pankmer-0.11.6/src/pankmer/upset.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       82 2023-04-16 22:50:20.000000 pankmer-0.11.6/src/pankmer/version.py
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-04-16 22:51:51.421558 pankmer-0.11.6/test/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4263 2023-04-16 20:15:18.000000 pankmer-0.11.6/test/test_compiled.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    10190 2023-04-16 20:15:18.000000 pankmer-0.11.6/test/test_slow.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2255 2023-01-16 17:12:04.000000 pankmer-0.11.6/test/test_tree.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.228165 pankmer-0.9.0/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1582 2023-02-04 07:58:07.000000 pankmer-0.9.0/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5077 2023-02-04 08:39:36.227417 pankmer-0.9.0/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4331 2023-02-04 07:49:14.000000 pankmer-0.9.0/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.187702 pankmer-0.9.0/pankmer.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5077 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      638 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       49 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       68 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        8 2023-02-04 08:39:36.000000 pankmer-0.9.0/pankmer.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1174 2023-02-04 08:27:05.000000 pankmer-0.9.0/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-02-04 08:39:36.228268 pankmer-0.9.0/setup.cfg
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      450 2023-01-16 17:12:04.000000 pankmer-0.9.0/setup.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.180795 pankmer-0.9.0/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.218482 pankmer-0.9.0/src/pankmer/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      257 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1832 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/adjacency_matrix.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3009 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/clustermap.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      907 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/count.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1493 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    17939 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      213 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/get_lower_bound.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      364 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/gzip_agnostic_open.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    13154 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/index.pyx
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    46421 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/pankmer.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      355 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/populate.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    17507 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/reg_coverage.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6062 2023-02-04 07:49:15.000000 pankmer-0.9.0/src/pankmer/tree.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       81 2023-02-04 08:26:57.000000 pankmer-0.9.0/src/pankmer/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-02-04 08:39:36.224115 pankmer-0.9.0/test/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4278 2023-01-16 17:12:04.000000 pankmer-0.9.0/test/test_compiled.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6969 2023-02-04 07:49:15.000000 pankmer-0.9.0/test/test_slow.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2255 2023-01-16 17:12:04.000000 pankmer-0.9.0/test/test_tree.py
```

### Comparing `pankmer-0.11.6/LICENSE` & `pankmer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/PKG-INFO` & `pankmer-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pankmer
-Version: 0.11.6
+Version: 0.9.0
 Summary: Generate a PanGenome given a set of genomes
 Author: Semar Petrus, Allen Mamerto, Nolan Hartwick
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/pankmer
 Project-URL: Documentation, https://salk-tm.gitlab.io/pankmer
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
@@ -21,33 +21,31 @@
 # PanKmer
 
 _k_-mer based and reference-free pangenome analysis. See the quickstart below, or read the [documentation](https://salk-tm.gitlab.io/pankmer/index.html).
 
 ## Installation
 ### With pip
 ```
-pip install pankmer
+pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### In a conda environment
 First create an environment that includes all dependencies:
 ```
-conda create -c bioconda -c conda-forge -n pankmer python==3.10 \
-  biopython==1.79 cython setuptools seaborn urllib3 wheel python-newick \
-  pyfaidx gff2bed upsetplot
+conda create -c conda-forge -c bioconda -n pankmer python==3.10 biopython==1.79 cython pandas setuptools seaborn urllib3 wheel python-newick pyfaidx gff2bed
 ```
 If running on OSX, a few additional packages will be required:
 ```
 conda activate pankmer
 conda install -c conda-forge clang_osx-64 clangxx_osx-64 gfortran_osx-64
 ```
 Then install PanKmer with pip:
 ```
 conda activate pankmer
-pip install pankmer
+pip install pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### Check installation
 Check that the installation was successful by running:
 ```
 pankmer --version
 ```
```

### Comparing `pankmer-0.11.6/README.md` & `pankmer-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,33 +3,31 @@
 # PanKmer
 
 _k_-mer based and reference-free pangenome analysis. See the quickstart below, or read the [documentation](https://salk-tm.gitlab.io/pankmer/index.html).
 
 ## Installation
 ### With pip
 ```
-pip install pankmer
+pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### In a conda environment
 First create an environment that includes all dependencies:
 ```
-conda create -c bioconda -c conda-forge -n pankmer python==3.10 \
-  biopython==1.79 cython setuptools seaborn urllib3 wheel python-newick \
-  pyfaidx gff2bed upsetplot
+conda create -c conda-forge -c bioconda -n pankmer python==3.10 biopython==1.79 cython pandas setuptools seaborn urllib3 wheel python-newick pyfaidx gff2bed
 ```
 If running on OSX, a few additional packages will be required:
 ```
 conda activate pankmer
 conda install -c conda-forge clang_osx-64 clangxx_osx-64 gfortran_osx-64
 ```
 Then install PanKmer with pip:
 ```
 conda activate pankmer
-pip install pankmer
+pip install pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### Check installation
 Check that the installation was successful by running:
 ```
 pankmer --version
 ```
```

### Comparing `pankmer-0.11.6/pankmer.egg-info/PKG-INFO` & `pankmer-0.9.0/pankmer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pankmer
-Version: 0.11.6
+Version: 0.9.0
 Summary: Generate a PanGenome given a set of genomes
 Author: Semar Petrus, Allen Mamerto, Nolan Hartwick
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/pankmer
 Project-URL: Documentation, https://salk-tm.gitlab.io/pankmer
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
@@ -21,33 +21,31 @@
 # PanKmer
 
 _k_-mer based and reference-free pangenome analysis. See the quickstart below, or read the [documentation](https://salk-tm.gitlab.io/pankmer/index.html).
 
 ## Installation
 ### With pip
 ```
-pip install pankmer
+pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### In a conda environment
 First create an environment that includes all dependencies:
 ```
-conda create -c bioconda -c conda-forge -n pankmer python==3.10 \
-  biopython==1.79 cython setuptools seaborn urllib3 wheel python-newick \
-  pyfaidx gff2bed upsetplot
+conda create -c conda-forge -c bioconda -n pankmer python==3.10 biopython==1.79 cython pandas setuptools seaborn urllib3 wheel python-newick pyfaidx gff2bed
 ```
 If running on OSX, a few additional packages will be required:
 ```
 conda activate pankmer
 conda install -c conda-forge clang_osx-64 clangxx_osx-64 gfortran_osx-64
 ```
 Then install PanKmer with pip:
 ```
 conda activate pankmer
-pip install pankmer
+pip install pip install git+https://gitlab.com/salk-tm/pankmer.git
 ```
 
 ### Check installation
 Check that the installation was successful by running:
 ```
 pankmer --version
 ```
```

### Comparing `pankmer-0.11.6/pankmer.egg-info/SOURCES.txt` & `pankmer-0.9.0/pankmer.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,12 @@
 src/pankmer/env.py
 src/pankmer/get_lower_bound.py
 src/pankmer/gzip_agnostic_open.py
 src/pankmer/index.pyx
 src/pankmer/pankmer.py
 src/pankmer/populate.py
 src/pankmer/reg_coverage.py
-src/pankmer/saturation.py
 src/pankmer/tree.py
-src/pankmer/upset.py
 src/pankmer/version.py
 test/test_compiled.py
 test/test_slow.py
 test/test_tree.py
```

### Comparing `pankmer-0.11.6/pyproject.toml` & `pankmer-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "Cython", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pankmer"
-version = "0.11.6" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.9.0" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
   { name="Anthony Aylward", email="aaylward@salk.edu" },
   { name="Semar Petrus" },
   { name="Allen Mamerto" },
   { name="Nolan Hartwick" },
 ]
 description = "Generate a PanGenome given a set of genomes"
@@ -22,19 +22,19 @@
     "Operating System :: OS Independent",
     "License :: OSI Approved :: BSD License",
 ]
 dependencies = [
     "biopython<=1.79",
     "gff2bed",
     "newick",
+    "pandas",
     "pyfaidx",
     "scipy",
     "seaborn",
-    "urllib3",
-    "upsetplot"
+    "urllib3"
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/salk-tm/pankmer"
 "Documentation" = "https://salk-tm.gitlab.io/pankmer"
 
 [project.scripts]
```

### Comparing `pankmer-0.11.6/src/pankmer/adjacency_matrix.py` & `pankmer-0.9.0/src/pankmer/adjacency_matrix.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/src/pankmer/clustermap.py` & `pankmer-0.9.0/src/pankmer/clustermap.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/src/pankmer/count.py` & `pankmer-0.9.0/src/pankmer/count.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/src/pankmer/download.py` & `pankmer-0.9.0/src/pankmer/download.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/src/pankmer/env.py` & `pankmer-0.9.0/src/pankmer/env.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/src/pankmer/index.pyx` & `pankmer-0.9.0/src/pankmer/index.pyx`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/src/pankmer/pankmer.py` & `pankmer-0.9.0/src/pankmer/pankmer.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 # from pankmer.index import (print_err, genome_name, break_seq, get_kmers,
 #                    score_byte_to_blist, kmer_byte_to_blist, kmer_byte_to_long)
 from pankmer.index import (print_err, break_seq, get_kmers, score_byte_to_blist,
                            run_index)
 from pankmer.env import EXAMPLE_DATA_DIR
 from pankmer.download import download_example
 from pankmer.count import count_kmers
-from pankmer.saturation import saturation
-from pankmer.upset import upset
 from pankmer.adjacency_matrix import get_adjacency_matrix
 from pankmer.tree import tree
 from pankmer.clustermap import clustermap
 from pankmer.reg_coverage import (COLOR_PALETTE, reg_coverage, genome_coverage,
                                   genome_coverage_plot, coverage_heatmap)
 from pankmer.version import __version__
 from pankmer.gzip_agnostic_open import gzip_agnostic_open
@@ -722,37 +720,14 @@
 
 
 def run_count(args):
     kmer_counts = count_kmers(*(PKResults(i) for i in args.index), names=args.index)
     kmer_counts.to_csv(sys.stdout, sep='\t', index=False)
 
 
-def run_saturation(args):
-    sat_df = saturation(PKResults(args.index), args.output, title=args.title,
-                        width=args.width, height=args.height,
-                        palette=args.color_palette, alpha=args.alpha,
-                        linewidth=args.linewidth, conf=args.conf)
-    if args.table:
-        sat_df.to_csv(args.table, sep='\t', index=False)
-
-
-def run_upset(args):
-    if args.time:
-        start = time.time()
-    upset(PKResults(args.input), args.output, args.genomes,
-          specific=args.specific,
-          vertical=args.vertical,
-          show_counts=args.show_counts,
-          min_subset_size=args.min_subset_size,
-          max_subset_size=args.max_subset_size)
-    if args.time:
-        stop = time.time()
-        print(f'UpSet plot generated in {(stop - start) / 60:.2f} minutes')
-
-
 def run_adjacency_matrix(args):
     if args.time:
         start = time.time()
     results = PKResults(args.input_dir)
     output = args.output
     df = get_adjacency_matrix(results)
     df.to_csv(output)
@@ -874,98 +849,33 @@
     count_parser = subparsers.add_parser('count',
         help='count k-mers in one or more indexes')
     count_parser.add_argument(
         '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
         dest='index', required=True, nargs='+', help='a k-mer index')
     count_parser.set_defaults(func=run_count)
 
-    saturation_parser = subparsers.add_parser('saturation',
-        help='calculate k-mer saturation curve')
-    saturation_parser.add_argument(
-        '-i', '--index', metavar='<index[.tar]>', type=str, action='store',
-        required=True, help='a k-mer index')
-    saturation_parser.add_argument(
-        '-o', '--output', metavar='<output.{pdf,png,svg}>', type=str,
-        action='store', dest='output',
-        help='destination file for plot')
-    saturation_parser.add_argument(
-        '-t', '--table', metavar='<output-table.tsv>',
-        help='output TSV file containing plotted data')
-    saturation_parser.add_argument('--title', metavar='<"Plot title">',
-        help='set the title for the plot')
-    saturation_parser.add_argument('--width', metavar='<float>', type=float,
-        default=4.0, help='set width of figure in inches [4]')
-    saturation_parser.add_argument('--height', metavar='<float>', type=float,
-        default=3.0, help='set height of figure in inches [3]')
-    saturation_parser.add_argument('--color-palette', metavar='<#color>', nargs='+',
-        default=COLOR_PALETTE[:2], help='color palette to use')
-    saturation_parser.add_argument('--alpha', metavar='<float>', type=float,
-        default=1.0, help='transparency value for lines [1.0]')
-    saturation_parser.add_argument('--linewidth', metavar='<int>', type=int,
-        default=3, help='line width for plot [3]')
-    saturation_parser.add_argument('--conf', action='store_true',
-        help='calculate confidence intervals for saturation curves')
-    saturation_parser.set_defaults(func=run_saturation)
-
-    upset_parser = subparsers.add_parser('upset', help='generate upset plot')
-    upset_parser.add_argument(
-        '-i', '--input', metavar='<index[.tar]>',
-        required=True, help='a k-mer index')
-    upset_parser.add_argument(
-        '-o', '--output', metavar='<output.{pdf,png,svg}>', required=True,
-        help='destination file for upset plot')
-    upset_parser.add_argument(
-        '-g', '--genomes', metavar='<genome>', required=True, nargs='+',
-        help='List of genomes to include '
-    )
-    upset_parser.add_argument(
-        '-s', '--specific', action='store_true',
-        help='Include only k-mers specific to the input genome set'
-    )
-    upset_parser.add_argument(
-        '-v', '--vertical', action='store_true',
-        help='Draw the plot vertically'
-    )
-    upset_parser.add_argument(
-        '--show-counts', action='store_true',
-        help='Show counts for each subset'
-    )
-    upset_parser.add_argument(
-        '--min-subset-size', metavar='<int>', type=int,
-        help='Show only subsets larger than a minimum size'
-    )
-    upset_parser.add_argument(
-        '--max-subset-size', metavar='<int>', type=int,
-        help='Show only subsets smaller than a maximum size'
-    )
-    upset_parser.add_argument(
-        '--time', action='store_true',
-        help='Report the time required to execute'
-    )
-    upset_parser.set_defaults(func=run_upset)
-
     adjmat_parser = subparsers.add_parser('adj-matrix',
         help='generate adjacency matrix')
     adjmat_parser.add_argument(
-        '-i', '--input', metavar='<index[.tar]>',
+        '-i', '--input', metavar='<index[.tar]>', type=str, action='store',
         dest='input_dir', required=True, help='a k-mer index')
     adjmat_parser.add_argument(
-        '-o', '--output', metavar='<adjmatrix.csv>',
+        '-o', '--output', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='output', required=True,
         help='destination file for adjacency matrix')
     adjmat_parser.add_argument(
         '--time', action='store_true',
         help='Report the time required to execute'
     )
     adjmat_parser.set_defaults(func=run_adjacency_matrix)
 
     tree_parser = subparsers.add_parser('tree',
         help='generate a heirarchical clustering tree from an adjacency matrix')
     tree_parser.add_argument(
-        '-i', '--input', metavar='<adjmatrix.csv>',
+        '-i', '--input', metavar='<adjmatrix.csv>', type=str, action='store',
         dest='input', required=True, help='adjacency matrix file')
     tree_parser.add_argument(
         '-n', '--newick', action='store_true', dest='newick',
         help='output tree in NEWICK format'
     )
     tree_parser.add_argument(
         '--metric', choices=('intersection', 'jaccard', 'overlap'),
@@ -1172,15 +1082,15 @@
         '-d', '--dir', metavar='<dir/>', type=str, action='store',
         dest='dir', default=EXAMPLE_DATA_DIR,
         help='destination directory for example data')
     download_parser.add_argument(
         '-b', '--bacterial', action='store_true', dest='bacterial',
         help='if True, download bacterial genomes')
     download_parser.add_argument(
-        '-n', '--n-samples', metavar='<int>', type=int, default=1, action='store', dest='n_samples',
+        '-n', '--n-samples', metavar='<int>', type=int, action='store', dest='n_samples',
         help='number of bacterial samples to download, max 164 [1]')
     download_parser.set_defaults(func=run_download_example)
 
     args = parser.parse_args()
     if args.version:
         print(__version__)
         sys.exit()
```

### Comparing `pankmer-0.11.6/src/pankmer/reg_coverage.py` & `pankmer-0.9.0/src/pankmer/reg_coverage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -356,16 +356,16 @@
                             borderaxespad=0, title=legend_title)
         else:
             leg = ax.legend(loc=legend_loc, title=legend_title)
         for line in leg.get_lines():
             line.set_linewidth(linewidth)
             line.set_alpha(alpha)
     fig = ax.get_figure()
-    fig.set_figwidth(width)
     fig.set_figheight(height)
+    fig.set_figwidth(width)
     fig.tight_layout()
     fig.savefig(output)
     fig.clf()
 
 
 def genome_coverage(*pk_results, output: str, ref: str, chromosomes: list,
                     output_table=None, summary_func=mean, groups=None, loci=None,
```

### Comparing `pankmer-0.11.6/src/pankmer/tree.py` & `pankmer-0.9.0/src/pankmer/tree.py`

 * *Files identical despite different names*

### Comparing `pankmer-0.11.6/test/test_compiled.py` & `pankmer-0.9.0/test/test_compiled.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,11 +25,12 @@
 def test_score_byte_to_blist():
     assert score_byte_to_blist(b'\x05', 3) == [1, 0, 1]
 
 def test_add_score_mat_np(mat_result):
     score_multi = np.array([1, 1, 0]) * 2
     mat = np.array([[4, 0, 4], [0, 0, 0], [4, 0, 4]])
     mat = add_score_mat_np(score_multi, mat)
+    print(mat)
     for i, j in product(range(3), repeat=2):
         assert mat[i, j] == mat_result[i, j]
```

### Comparing `pankmer-0.11.6/test/test_tree.py` & `pankmer-0.9.0/test/test_tree.py`

 * *Files identical despite different names*

