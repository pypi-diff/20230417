# Comparing `tmp/IMGTgeneDL-0.5.0.tar.gz` & `tmp/IMGTgeneDL-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMGTgeneDL-0.5.0.tar", last modified: Sun Apr 16 22:55:27 2023, max compression
+gzip compressed data, was "IMGTgeneDL-0.5.1.tar", last modified: Sun Apr 16 23:33:40 2023, max compression
```

## Comparing `IMGTgeneDL-0.5.0.tar` & `IMGTgeneDL-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:55:27.196055 IMGTgeneDL-0.5.0/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)     1073 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.0/LICENSE
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    12492 2023-04-16 22:55:27.196055 IMGTgeneDL-0.5.0/PKG-INFO
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    12139 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.0/README.md
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       97 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.0/pyproject.toml
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      846 2023-04-16 22:55:27.196055 IMGTgeneDL-0.5.0/setup.cfg
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:55:27.188055 IMGTgeneDL-0.5.0/src/
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:55:27.192055 IMGTgeneDL-0.5.0/src/IMGTgeneDL/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    36617 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL/IMGTgeneDL.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL/__init__.py
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      524 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL/c-region-variant-configs.tsv
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      527 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL/species.tsv
-drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:55:27.196055 IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/
--rw-rw-r--   0 jomen     (1000) jomen     (1000)    12492 2023-04-16 22:55:27.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/PKG-INFO
--rw-rw-r--   0 jomen     (1000) jomen     (1000)      399 2023-04-16 22:55:27.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/SOURCES.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)        1 2023-04-16 22:55:27.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/dependency_links.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       58 2023-04-16 22:55:27.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/entry_points.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       36 2023-04-16 22:55:27.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/requires.txt
--rw-rw-r--   0 jomen     (1000) jomen     (1000)       11 2023-04-16 22:55:27.000000 IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/top_level.txt
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)     1073 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/LICENSE
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    12478 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/PKG-INFO
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    12125 2023-04-16 23:07:58.000000 IMGTgeneDL-0.5.1/README.md
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       97 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/pyproject.toml
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      846 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/setup.cfg
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.117405 IMGTgeneDL-0.5.1/src/
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/src/IMGTgeneDL/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    36683 2023-04-16 23:27:06.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/IMGTgeneDL.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        0 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/__init__.py
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      524 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/c-region-variant-configs.tsv
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      527 2023-04-16 22:54:15.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL/species.tsv
+drwxrwxr-x   0 jomen     (1000) jomen     (1000)        0 2023-04-16 23:33:40.121405 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)    12478 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/PKG-INFO
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)      399 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/SOURCES.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)        1 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/dependency_links.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       58 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/entry_points.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       36 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/requires.txt
+-rw-rw-r--   0 jomen     (1000) jomen     (1000)       11 2023-04-16 23:33:40.000000 IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/top_level.txt
```

### Comparing `IMGTgeneDL-0.5.0/LICENSE` & `IMGTgeneDL-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `IMGTgeneDL-0.5.0/PKG-INFO` & `IMGTgeneDL-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: IMGTgeneDL
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python script to download data from IMGT/GENE-DB
 Home-page: https://github.com/JamieHeather/IMGTgeneDL
 Author: Jamie Heather
 Author-email: jheather@mgh.harvard.edu
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IMGTgeneDL
 
-## 0.5.0
+## 0.5.1
 ##### Jamie Heather | CCR @ MGH | 2023
 
-This script provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
+This tool provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
 
 ## Usage
 
 This script is tested on python >= 3.6.
 
 ### Installation
 
@@ -68,20 +68,20 @@
 
 Note that these can be combined, e.g. `-vdj` will just download the V, D, and J gene sequences. Alternatively users can apply the `-r / --get_all_regions` flag to just download all of these regions (equivalent to `-lvdjc`).
 
 #### Examples
 
 The following is the basic command to download all relevant human sequences for all chains:
 ```
-IMGTgeneDL.py -s Homo+sapiens -L TR -r
+IMGTgeneDL -s Homo+sapiens -L TR -r
 ```
 
 While this is a command to just download delta chain J genes from mice:
 ```
-IMGTgeneDL.py -n -s mouse -j -L D
+IMGTgeneDL -n -s mouse -j -L D
 ```
 
 ### Download whole database
 
 If no locus and gene type flags are used, or if the `-a / --get_all` flag is used, then the script will just download [the whole of GENE-DB](http://www.imgt.org/download/GENE-DB/) - all species, all genes, all loci. By default this downloads the [ungapped nucleotide file, with all pseudogenes](http://www.imgt.org/download/GENE-DB/IMGTGENEDB-ReferenceSequences.fasta-nt-WithoutGaps-F+ORF+allP), and saves this to a file named with the date and the [IMGT release](http://www.imgt.org/download/GENE-DB/RELEASE) used. This can be changed using the following flags:
 
 * `-gap / --gapped`: downloads the gapped FASTA instead of the ungapped
@@ -112,16 +112,16 @@
     * Contains automatically inferred in-frame constant region peptide sequences, for use in finding the correct frame of stitched sequences
 * `TR[A/B/G/D].fasta`
     * FASTA files of the individual loci's genes
 
 It is simply run by specifying the mode and the desired species, either using common or scientific names:
 
 ```
-IMGTgeneDL.py -s human -m stitchr -n
-IMGTgeneDL.py -s Homo+sapiens -m stitchr
+IMGTgeneDL -s human -m stitchr -n
+IMGTgeneDL -s Homo+sapiens -m stitchr
 ```
 
 The script will only output a FASTA file for a specific locus if there is sufficient information for `stitchr` to use, i.e. there must be at least one leader, variable, joining, and constant region sequence, which are not currently available for all sequences that are listed in the database. In order to be used by `stitchr` it also appends an additional field to the end of the IMGT-provided FASTA header after a '~' character, labeling it's sequence type (LEADER/VARIABLE/JOINING/CONSTANT), allowing for explicit type declaration in the face of potentially variable IMGT-provided fields.
 
 However note that while this script will generate files if those conditions are met, these data may not be sufficient for functional `stitchr` operation without manually adding sequences (e.g. if no matching leader/variable regions are found). It's recommended that users take care when using these tools for species with relatively little banked data. 
 
 Also note that `stitchr` mode will filter out any FASTA reads containing ambiguous or non-DNA residues, which are present for some species. All TRDV genes are also included in the `TRA.fasta` files by default, as (at least in humans) all can be found rearranged with TRAJ genes.
```

### Comparing `IMGTgeneDL-0.5.0/README.md` & `IMGTgeneDL-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # IMGTgeneDL
 
-## 0.5.0
+## 0.5.1
 ##### Jamie Heather | CCR @ MGH | 2023
 
-This script provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
+This tool provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
 
 ## Usage
 
 This script is tested on python >= 3.6.
 
 ### Installation
 
@@ -56,20 +56,20 @@
 
 Note that these can be combined, e.g. `-vdj` will just download the V, D, and J gene sequences. Alternatively users can apply the `-r / --get_all_regions` flag to just download all of these regions (equivalent to `-lvdjc`).
 
 #### Examples
 
 The following is the basic command to download all relevant human sequences for all chains:
 ```
-IMGTgeneDL.py -s Homo+sapiens -L TR -r
+IMGTgeneDL -s Homo+sapiens -L TR -r
 ```
 
 While this is a command to just download delta chain J genes from mice:
 ```
-IMGTgeneDL.py -n -s mouse -j -L D
+IMGTgeneDL -n -s mouse -j -L D
 ```
 
 ### Download whole database
 
 If no locus and gene type flags are used, or if the `-a / --get_all` flag is used, then the script will just download [the whole of GENE-DB](http://www.imgt.org/download/GENE-DB/) - all species, all genes, all loci. By default this downloads the [ungapped nucleotide file, with all pseudogenes](http://www.imgt.org/download/GENE-DB/IMGTGENEDB-ReferenceSequences.fasta-nt-WithoutGaps-F+ORF+allP), and saves this to a file named with the date and the [IMGT release](http://www.imgt.org/download/GENE-DB/RELEASE) used. This can be changed using the following flags:
 
 * `-gap / --gapped`: downloads the gapped FASTA instead of the ungapped
@@ -100,16 +100,16 @@
     * Contains automatically inferred in-frame constant region peptide sequences, for use in finding the correct frame of stitched sequences
 * `TR[A/B/G/D].fasta`
     * FASTA files of the individual loci's genes
 
 It is simply run by specifying the mode and the desired species, either using common or scientific names:
 
 ```
-IMGTgeneDL.py -s human -m stitchr -n
-IMGTgeneDL.py -s Homo+sapiens -m stitchr
+IMGTgeneDL -s human -m stitchr -n
+IMGTgeneDL -s Homo+sapiens -m stitchr
 ```
 
 The script will only output a FASTA file for a specific locus if there is sufficient information for `stitchr` to use, i.e. there must be at least one leader, variable, joining, and constant region sequence, which are not currently available for all sequences that are listed in the database. In order to be used by `stitchr` it also appends an additional field to the end of the IMGT-provided FASTA header after a '~' character, labeling it's sequence type (LEADER/VARIABLE/JOINING/CONSTANT), allowing for explicit type declaration in the face of potentially variable IMGT-provided fields.
 
 However note that while this script will generate files if those conditions are met, these data may not be sufficient for functional `stitchr` operation without manually adding sequences (e.g. if no matching leader/variable regions are found). It's recommended that users take care when using these tools for species with relatively little banked data. 
 
 Also note that `stitchr` mode will filter out any FASTA reads containing ambiguous or non-DNA residues, which are present for some species. All TRDV genes are also included in the `TRA.fasta` files by default, as (at least in humans) all can be found rearranged with TRAJ genes.
```

### Comparing `IMGTgeneDL-0.5.0/setup.cfg` & `IMGTgeneDL-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IMGTgeneDL
-version = 0.5.0
+version = 0.5.1
 author = Jamie Heather
 author_email = jheather@mgh.harvard.edu
 description = Python script to download data from IMGT/GENE-DB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JamieHeather/IMGTgeneDL
 project_urls =
```

### Comparing `IMGTgeneDL-0.5.0/src/IMGTgeneDL/IMGTgeneDL.py` & `IMGTgeneDL-0.5.1/src/IMGTgeneDL/IMGTgeneDL.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Ensure correct importlib-resources function imported
 if sys.version_info < (3, 9):
     import importlib_resources                              # PyPI
 else:
     import importlib.resources as importlib_resources       # importlib.resources
 
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 __author__ = 'Jamie Heather'
 __email__ = 'jheather@mgh.harvard.edu'
 
 warnings.filterwarnings('ignore', message='Unverified HTTPS request')
 
 
 def args():
@@ -259,14 +259,17 @@
         if in_args['get_d']:
             genes_to_dl.append('D')
         if in_args['get_j']:
             genes_to_dl.append('J')
         if in_args['get_c']:
             genes_to_dl.append('C')
 
+    if not genes_to_dl:
+        raise IOError("No gene regions detected for download - please use the appropriate -l/-v/-d/-j/-c/-r flags. ")
+
     warnings.warn("Detected " + str(len(genes_to_dl)) + " gene types to download: " + ', '.join(genes_to_dl) + '.')
 
     return genes_to_dl
 
 
 def get_specific_items(search_loci, search_genes, species_constants, basic_gene_types, search_species):
     """
@@ -861,16 +864,14 @@
 
 def main():
 
     # Sort input/output file details
     pkg_files = importlib_resources.files("IMGTgeneDL")
     c_region_variants_file = str(pkg_files / 'c-region-variant-configs.tsv')
     default_species_path = str(pkg_files / 'species.tsv')
-    print(str(pkg_files))
-    print(importlib_resources.files("IMGTgeneDL"))
     input_args = process_input_args(vars(args()), default_species_path)
 
     with warnings.catch_warnings(record=True) as warnings_list:
         warnings.simplefilter("always")
 
         if input_args['get_all']:
             url, out_suffix = get_url(input_args, base_url)
```

### Comparing `IMGTgeneDL-0.5.0/src/IMGTgeneDL/c-region-variant-configs.tsv` & `IMGTgeneDL-0.5.1/src/IMGTgeneDL/c-region-variant-configs.tsv`

 * *Files identical despite different names*

### Comparing `IMGTgeneDL-0.5.0/src/IMGTgeneDL/species.tsv` & `IMGTgeneDL-0.5.1/src/IMGTgeneDL/species.tsv`

 * *Files identical despite different names*

### Comparing `IMGTgeneDL-0.5.0/src/IMGTgeneDL.egg-info/PKG-INFO` & `IMGTgeneDL-0.5.1/src/IMGTgeneDL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: IMGTgeneDL
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python script to download data from IMGT/GENE-DB
 Home-page: https://github.com/JamieHeather/IMGTgeneDL
 Author: Jamie Heather
 Author-email: jheather@mgh.harvard.edu
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IMGTgeneDL
 
-## 0.5.0
+## 0.5.1
 ##### Jamie Heather | CCR @ MGH | 2023
 
-This script provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
+This tool provides an alternative way to access TCR and IG genes stored in [IMGT/GENE-DB](http://www.imgt.org/genedb/). It was mostly built to download human and mouse TCR sequences, so that's what is most tested, but it's readily adaptable to other species and loci.
 
 ## Usage
 
 This script is tested on python >= 3.6.
 
 ### Installation
 
@@ -68,20 +68,20 @@
 
 Note that these can be combined, e.g. `-vdj` will just download the V, D, and J gene sequences. Alternatively users can apply the `-r / --get_all_regions` flag to just download all of these regions (equivalent to `-lvdjc`).
 
 #### Examples
 
 The following is the basic command to download all relevant human sequences for all chains:
 ```
-IMGTgeneDL.py -s Homo+sapiens -L TR -r
+IMGTgeneDL -s Homo+sapiens -L TR -r
 ```
 
 While this is a command to just download delta chain J genes from mice:
 ```
-IMGTgeneDL.py -n -s mouse -j -L D
+IMGTgeneDL -n -s mouse -j -L D
 ```
 
 ### Download whole database
 
 If no locus and gene type flags are used, or if the `-a / --get_all` flag is used, then the script will just download [the whole of GENE-DB](http://www.imgt.org/download/GENE-DB/) - all species, all genes, all loci. By default this downloads the [ungapped nucleotide file, with all pseudogenes](http://www.imgt.org/download/GENE-DB/IMGTGENEDB-ReferenceSequences.fasta-nt-WithoutGaps-F+ORF+allP), and saves this to a file named with the date and the [IMGT release](http://www.imgt.org/download/GENE-DB/RELEASE) used. This can be changed using the following flags:
 
 * `-gap / --gapped`: downloads the gapped FASTA instead of the ungapped
@@ -112,16 +112,16 @@
     * Contains automatically inferred in-frame constant region peptide sequences, for use in finding the correct frame of stitched sequences
 * `TR[A/B/G/D].fasta`
     * FASTA files of the individual loci's genes
 
 It is simply run by specifying the mode and the desired species, either using common or scientific names:
 
 ```
-IMGTgeneDL.py -s human -m stitchr -n
-IMGTgeneDL.py -s Homo+sapiens -m stitchr
+IMGTgeneDL -s human -m stitchr -n
+IMGTgeneDL -s Homo+sapiens -m stitchr
 ```
 
 The script will only output a FASTA file for a specific locus if there is sufficient information for `stitchr` to use, i.e. there must be at least one leader, variable, joining, and constant region sequence, which are not currently available for all sequences that are listed in the database. In order to be used by `stitchr` it also appends an additional field to the end of the IMGT-provided FASTA header after a '~' character, labeling it's sequence type (LEADER/VARIABLE/JOINING/CONSTANT), allowing for explicit type declaration in the face of potentially variable IMGT-provided fields.
 
 However note that while this script will generate files if those conditions are met, these data may not be sufficient for functional `stitchr` operation without manually adding sequences (e.g. if no matching leader/variable regions are found). It's recommended that users take care when using these tools for species with relatively little banked data. 
 
 Also note that `stitchr` mode will filter out any FASTA reads containing ambiguous or non-DNA residues, which are present for some species. All TRDV genes are also included in the `TRA.fasta` files by default, as (at least in humans) all can be found rearranged with TRAJ genes.
```

