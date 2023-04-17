# Comparing `tmp/pyroe-0.9.0.tar.gz` & `tmp/pyroe-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroe-0.9.0.tar", last modified: Thu Feb 23 05:20:58 2023, max compression
+gzip compressed data, was "pyroe-0.9.1.tar", last modified: Mon Apr 17 03:07:00 2023, max compression
```

## Comparing `pyroe-0.9.0.tar` & `pyroe-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:20:58.980739 pyroe-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-02-23 05:20:47.000000 pyroe-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-23 05:20:58.980739 pyroe-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-02-23 05:20:47.000000 pyroe-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:20:58.972740 pyroe-0.9.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9829 2023-02-23 05:20:47.000000 pyroe-0.9.0/bin/pyroe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-23 05:20:47.000000 pyroe-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-02-23 05:20:58.980739 pyroe-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:20:58.972740 pyroe-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:20:58.976740 pyroe-0.9.0/src/pyroe/
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/ProcessedQuant.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:20:58.976740 pyroe-0.9.0/src/pyroe/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/data/available_datasets.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/fetch_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/id_to_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/load_fry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/load_processed_quant.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24577 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/make_splici_txome.py
--rw-r--r--   0 runner    (1001) docker     (123)    50262 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/make_txome.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-23 05:20:47.000000 pyroe-0.9.0/src/pyroe/pyroe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:20:58.976740 pyroe-0.9.0/src/pyroe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-23 05:20:58.000000 pyroe-0.9.0/src/pyroe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-23 05:20:58.000000 pyroe-0.9.0/src/pyroe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 05:20:58.000000 pyroe-0.9.0/src/pyroe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-23 05:20:58.000000 pyroe-0.9.0/src/pyroe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-23 05:20:58.000000 pyroe-0.9.0/src/pyroe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 05:20:58.980739 pyroe-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-02-23 05:20:47.000000 pyroe-0.9.0/tests/test_ProcessedQuant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-02-23 05:20:47.000000 pyroe-0.9.0/tests/test_fetch_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-23 05:20:47.000000 pyroe-0.9.0/tests/test_load_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-02-23 05:20:47.000000 pyroe-0.9.0/tests/test_make_spliceu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-02-23 05:20:47.000000 pyroe-0.9.0/tests/test_make_splici.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 03:06:48.000000 pyroe-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-17 03:07:00.005496 pyroe-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-17 03:06:48.000000 pyroe-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.001496 pyroe-0.9.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10146 2023-04-17 03:06:48.000000 pyroe-0.9.1/bin/pyroe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 03:06:48.000000 pyroe-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 03:07:00.005496 pyroe-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.001496 pyroe-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/src/pyroe/
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/ProcessedQuant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/src/pyroe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/data/available_datasets.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/fetch_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/id_to_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/load_fry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/load_processed_quant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24577 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/make_splici_txome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50262 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/make_txome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/pyroe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/src/pyroe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-17 03:07:00.000000 pyroe-0.9.1/src/pyroe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_ProcessedQuant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_fetch_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_load_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_make_spliceu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_make_splici.py
```

### Comparing `pyroe-0.9.0/LICENSE` & `pyroe-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/PKG-INFO` & `pyroe-0.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroe
-Version: 0.9.0
+Version: 0.9.1
 Summary: utilities of alevin-fry
 Home-page: https://github.com/COMBINE-lab/pyroe
 Author: Dongze He, Rob Patro
 Author-email: dhe17@umd.edu, rob@cs.umd.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroe-0.9.0/README.md` & `pyroe-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/bin/pyroe` & `pyroe-0.9.1/bin/pyroe`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,29 @@
     parser = argparse.ArgumentParser(
         description="The pyroe package provides useful functions to support alevin-fry ecosystem.",
         prog="pyroe",
     )
     parser.add_argument(
         "-v", "--version", action="version", version=f"pyroe {__version__}"
     )
-    
+
     subparsers = parser.add_subparsers(
         title="subcommands",
         dest="command",
         description="valid subcommands",
         help="additional help",
     )
-    
+
     # make-splici
     parser_makeSplici = subparsers.add_parser(
-        "make-spliced+intronic", 
+        "make-spliced+intronic",
         help="Make spliced + intronic reference",
-        aliases=['make-splici']
+        aliases=["make-splici"],
     )
+    parser_makeSplici.set_defaults(command="make-spliced+intronic")
     parser_makeSplici.add_argument(
         "genome_path",
         metavar="genome-path",
         type=str,
         help="The path to a genome fasta file.",
     )
     parser_makeSplici.add_argument(
@@ -101,16 +102,17 @@
         help="A flag indicates whether flank lengths will be considered when merging introns.",
     )
 
     # make-spliceu
     parser_makeSpliceu = subparsers.add_parser(
         "make-spliced+unspliced",
         help="Make spliced + unspliced reference",
-        aliases=['make-spliceu']
+        aliases=["make-spliceu"],
     )
+    parser_makeSpliceu.set_defaults(command="make-spliced+unspliced")
     parser_makeSpliceu.add_argument(
         "genome_path",
         metavar="genome-path",
         type=str,
         help="The path to a genome fasta file.",
     )
     parser_makeSpliceu.add_argument(
@@ -170,14 +172,15 @@
 
     parser_fetchQuant = subparsers.add_parser(
         "fetch-quant",
         help="Fetch processed quant results",
         epilog=epilog,
         formatter_class=RawTextHelpFormatter,
     )
+    parser_fetchQuant.set_defaults(command="fetch-quant")
     parser_fetchQuant.add_argument(
         "dataset_ids",
         metavar="dataset-ids",
         nargs="+",
         type=int,
         help="The ids of the datasets to fetch",
     )
@@ -202,28 +205,30 @@
         action="store_true",
         help="A flag indicates whether help messaged should not be printed.",
     )
 
     parser_id_to_name = subparsers.add_parser(
         "id-to-name", help="Generate a gene id to gene name mapping file from a GTF."
     )
+    parser_id_to_name.set_defaults(command="id-to-name")
     parser_id_to_name.add_argument("gtf_file", help="The GTF input file.")
     parser_id_to_name.add_argument(
         "output", help="The path to where the output tsv file will be written."
     )
     parser_id_to_name.add_argument(
         "--format",
         help="The input format of the file (must be either GTF or GFF3). This will be inferred from the filename, but if that fails it can be provided explicitly.",
         default=None,
     )
 
     out_formats = output_formats()
     parser_convert = subparsers.add_parser(
         "convert", help="Convert alevin-fry quantification result to another format."
     )
+    parser_convert.set_defaults(command="convert")
     parser_convert.add_argument(
         "quant_dir",
         metavar="quant_dir",
         type=str,
         help="The input quantification directory containing the matrix to be converted.",
     )
     parser_convert.add_argument(
@@ -246,30 +251,30 @@
         help="A 2 column tab-separated list of gene ID to gene name mappings. Providing this file will project gene IDs to gene names in the output.",
     )
 
     logging.basicConfig(level=logging.INFO)
 
     # Execute the parse_args() method
     args = parser.parse_args()
-    if args.command == "make-splici":
+    if args.command == "make-spliced+intronic":
         make_splici_txome(
             genome_path=args.genome_path,
             gtf_path=args.gtf_path,
             read_length=args.read_length,
             output_dir=args.output_dir,
             flank_trim_length=args.flank_trim_length,
             filename_prefix=args.filename_prefix,
             extra_spliced=args.extra_spliced,
             extra_unspliced=args.extra_unspliced,
             dedup_seqs=args.dedup_seqs,
             no_bt=args.no_bt,
             bt_path=args.bt_path,
             no_flanking_merge=args.no_flanking_merge,
         )
-    elif args.command == "make-spliceu":
+    elif args.command == "make-spliced+unspliced":
         make_spliceu_txome(
             genome_path=args.genome_path,
             gtf_path=args.gtf_path,
             output_dir=args.output_dir,
             filename_prefix=args.filename_prefix,
             extra_spliced=args.extra_spliced,
             extra_unspliced=args.extra_unspliced,
```

### Comparing `pyroe-0.9.0/setup.cfg` & `pyroe-0.9.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroe
-version = 0.9.0
+version = 0.9.1
 author = Dongze He, Rob Patro
 author_email = dhe17@umd.edu, rob@cs.umd.edu
 description = utilities of alevin-fry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/COMBINE-lab/pyroe
 classifiers = 
@@ -17,15 +17,15 @@
 package_dir = 
 	= src
 scripts = 
 	bin/pyroe
 python_requires = >=3.7
 include_package_data = True
 install_requires = 
-	pandas >= 1.3.0
+	pandas >= 1.3.0, < 2.0.0
 	pyranges >= 0.0.120
 	biopython >= 1.77
 	packaging >= 21.0
 	scanpy >= 1.8.2
 
 [options.packages.find]
 where = src
```

### Comparing `pyroe-0.9.0/src/pyroe/ProcessedQuant.py` & `pyroe-0.9.1/src/pyroe/ProcessedQuant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/convert.py` & `pyroe-0.9.1/src/pyroe/convert.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/data/available_datasets.tsv` & `pyroe-0.9.1/src/pyroe/data/available_datasets.tsv`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/fetch_processed_quant.py` & `pyroe-0.9.1/src/pyroe/fetch_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/id_to_name.py` & `pyroe-0.9.1/src/pyroe/id_to_name.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/load_fry.py` & `pyroe-0.9.1/src/pyroe/load_fry.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/load_processed_quant.py` & `pyroe-0.9.1/src/pyroe/load_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/make_splici_txome.py` & `pyroe-0.9.1/src/pyroe/make_splici_txome.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/make_txome.py` & `pyroe-0.9.1/src/pyroe/make_txome.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe/pyroe_utils.py` & `pyroe-0.9.1/src/pyroe/pyroe_utils.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/src/pyroe.egg-info/PKG-INFO` & `pyroe-0.9.1/src/pyroe.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroe
-Version: 0.9.0
+Version: 0.9.1
 Summary: utilities of alevin-fry
 Home-page: https://github.com/COMBINE-lab/pyroe
 Author: Dongze He, Rob Patro
 Author-email: dhe17@umd.edu, rob@cs.umd.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroe-0.9.0/src/pyroe.egg-info/SOURCES.txt` & `pyroe-0.9.1/src/pyroe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/tests/test_ProcessedQuant.py` & `pyroe-0.9.1/tests/test_ProcessedQuant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/tests/test_fetch_processed_quant.py` & `pyroe-0.9.1/tests/test_fetch_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/tests/test_load_processed_quant.py` & `pyroe-0.9.1/tests/test_load_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/tests/test_make_spliceu.py` & `pyroe-0.9.1/tests/test_make_spliceu.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.0/tests/test_make_splici.py` & `pyroe-0.9.1/tests/test_make_splici.py`

 * *Files identical despite different names*

