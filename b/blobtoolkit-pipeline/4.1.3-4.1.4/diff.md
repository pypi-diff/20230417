# Comparing `tmp/blobtoolkit-pipeline-4.1.3.tar.gz` & `tmp/blobtoolkit-pipeline-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blobtoolkit-pipeline-4.1.3.tar", last modified: Tue Apr  4 14:46:46 2023, max compression
+gzip compressed data, was "blobtoolkit-pipeline-4.1.4.tar", last modified: Mon Apr 17 08:35:28 2023, max compression
```

## Comparing `blobtoolkit-pipeline-4.1.3.tar` & `blobtoolkit-pipeline-4.1.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:46:46.075755 blobtoolkit-pipeline-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-04 14:46:46.075755 blobtoolkit-pipeline-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 14:46:46.075755 blobtoolkit-pipeline-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:46:46.067754 blobtoolkit-pipeline-4.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:46:46.071754 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/add_reads.smk
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/blastn.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/blobtoolkit.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/blobtools.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/busco.smk
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/chunk_stats.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/cov_stats.smk
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/diamond.smk
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/diamond_blastp.smk
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/minimap.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:46:46.071754 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/_transfer_dataset.smk
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/add_cov_to_tsv.smk
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/add_summary_to_metadata.smk
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/checksum_files.smk
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/chunk_fasta.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/chunk_fasta_by_busco.smk
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/chunk_nohit_fasta.smk
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/combine_stats.smk
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/count_busco_genes.smk
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/extract_busco_genes.smk
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/extract_nohit_fasta.smk
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/generate_images.smk
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/generate_summary.smk
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/get_chunked_stats.smk
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/get_window_stats.smk
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_bamtools_stats.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blastn.smk
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blobtk_depth.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blobtools_add.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blobtools_create.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_busco5.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_diamond_blastp.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_diamond_blastx.smk
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_minimap2_align.smk
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_minimap2_index.smk
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_mosdepth.smk
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_sub_pipeline.smk
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_windowmasker.smk
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/skip_windowmasker.smk
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/unchunk_blastn.smk
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/unchunk_blastx.smk
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/unzip_assembly_fasta.smk
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/validate_dataset.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/view.smk
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/window_stats.smk
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/windowmasker.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:46:46.075755 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-04 14:46:46.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-04 14:46:46.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:46:46.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-04 14:46:46.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 14:46:46.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-04 14:46:46.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 14:46:46.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 14:46:46.075755 blobtoolkit-pipeline-4.1.3/src/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4687 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/add_summary_to_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11611 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/chunk_fasta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3820 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/count_busco_genes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/extract_busco_genes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7194 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25176 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/generate_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      327 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/generate_configs.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     5208 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/generate_static_images.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1973 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/lsf_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4837 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/resume_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3290 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/run_btk_pipeline.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4052 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/track_bioproject_accessions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6145 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/transfer_completed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2594 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/unchunk_blast.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7220 2023-04-04 14:46:37.000000 blobtoolkit-pipeline-4.1.3/src/lib/window_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:35:28.787879 blobtoolkit-pipeline-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-17 08:35:28.787879 blobtoolkit-pipeline-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:35:28.787879 blobtoolkit-pipeline-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:35:28.779879 blobtoolkit-pipeline-4.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:35:28.779879 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/add_reads.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/blastn.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/blobtoolkit.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/blobtools.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/busco.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/chunk_stats.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/cov_stats.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/diamond.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/diamond_blastp.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/minimap.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:35:28.783879 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/_transfer_dataset.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/add_cov_to_tsv.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/add_summary_to_metadata.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/checksum_files.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/chunk_fasta.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/chunk_fasta_by_busco.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/chunk_nohit_fasta.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/combine_stats.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/count_busco_genes.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/extract_busco_genes.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/extract_nohit_fasta.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/generate_images.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/generate_summary.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/get_chunked_stats.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/get_window_stats.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_bamtools_stats.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blastn.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blobtk_depth.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blobtools_add.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blobtools_create.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_busco5.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_diamond_blastp.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_diamond_blastx.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_minimap2_align.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_minimap2_index.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_mosdepth.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_sub_pipeline.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_windowmasker.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/skip_windowmasker.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/unchunk_blastn.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/unchunk_blastx.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/unzip_assembly_fasta.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/validate_dataset.smk
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/view.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/window_stats.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/windowmasker.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:35:28.783879 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-17 08:35:28.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-17 08:35:28.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:35:28.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-17 08:35:28.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:35:28.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-17 08:35:28.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-17 08:35:28.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:35:28.787879 blobtoolkit-pipeline-4.1.4/src/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4687 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/add_summary_to_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11611 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/chunk_fasta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3820 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/count_busco_genes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3656 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/extract_busco_genes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7194 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25176 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/generate_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      327 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/generate_configs.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5208 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/generate_static_images.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1973 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/lsf_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4837 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/resume_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3290 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1487 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/run_btk_pipeline.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4052 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/track_bioproject_accessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6145 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/transfer_completed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2594 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/unchunk_blast.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7220 2023-04-17 08:35:10.000000 blobtoolkit-pipeline-4.1.4/src/lib/window_stats.py
```

### Comparing `blobtoolkit-pipeline-4.1.3/PKG-INFO` & `blobtoolkit-pipeline-4.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtoolkit-pipeline
-Version: 4.1.3
+Version: 4.1.4
 Summary: blobtoolkit-pipeline
 Home-page: https://github.com/blobtoolkit/blobtoolkit
 Author: blobtoolkit
 Author-email: blobtoolkit@genomehubs.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blobtoolkit/blobtoolkit/issues
 Project-URL: Source, https://github.com/blobtoolkit/blobtoolkit
```

### Comparing `blobtoolkit-pipeline-4.1.3/setup.py` & `blobtoolkit-pipeline-4.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="blobtoolkit-pipeline",  # Required
-    version="4.1.3",
+    version="4.1.4",
     description="blobtoolkit-pipeline",  # Optional
     long_description="blobtoolkit-pipeline",  # Optional
     long_description_content_type="text/markdown",
     url="https://github.com/blobtoolkit/blobtoolkit",  # Optional
     # This should be your name or the name of the organization which owns the
     # project.
     author="blobtoolkit",  # Optional
```

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/add_reads.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/add_reads.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/blastn.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/blastn.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/blobtoolkit.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/blobtoolkit.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/blobtools.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/blobtools.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/busco.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/busco.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/chunk_stats.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/chunk_stats.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/cov_stats.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/cov_stats.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/diamond.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/diamond.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/diamond_blastp.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/diamond_blastp.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/minimap.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/minimap.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/_transfer_dataset.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/_transfer_dataset.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/add_cov_to_tsv.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/add_cov_to_tsv.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/checksum_files.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/checksum_files.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/chunk_fasta.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/chunk_fasta.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/chunk_fasta_by_busco.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/chunk_fasta_by_busco.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/chunk_nohit_fasta.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/chunk_nohit_fasta.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/combine_stats.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/combine_stats.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/count_busco_genes.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/count_busco_genes.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/extract_busco_genes.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/extract_busco_genes.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/extract_nohit_fasta.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/extract_nohit_fasta.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/generate_images.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/generate_images.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/get_chunked_stats.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/get_chunked_stats.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/get_window_stats.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/get_window_stats.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blastn.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blastn.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blobtk_depth.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blobtk_depth.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blobtools_add.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blobtools_add.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_blobtools_create.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_blobtools_create.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_busco5.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_busco5.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_diamond_blastp.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_diamond_blastp.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_diamond_blastx.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_diamond_blastx.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_minimap2_align.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_minimap2_align.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_minimap2_index.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_minimap2_index.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_mosdepth.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_mosdepth.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_sub_pipeline.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_sub_pipeline.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/run_windowmasker.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/run_windowmasker.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/unchunk_blastn.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/unchunk_blastn.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/unchunk_blastx.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/unchunk_blastx.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/rules/validate_dataset.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/rules/validate_dataset.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/view.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/view.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/window_stats.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/window_stats.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit-snakefiles/windowmasker.smk` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit-snakefiles/windowmasker.smk`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/PKG-INFO` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtoolkit-pipeline
-Version: 4.1.3
+Version: 4.1.4
 Summary: blobtoolkit-pipeline
 Home-page: https://github.com/blobtoolkit/blobtoolkit
 Author: blobtoolkit
 Author-email: blobtoolkit@genomehubs.org
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blobtoolkit/blobtoolkit/issues
 Project-URL: Source, https://github.com/blobtoolkit/blobtoolkit
```

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/SOURCES.txt` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.egg-info/entry_points.txt` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/blobtoolkit_pipeline.py` & `blobtoolkit-pipeline-4.1.4/src/blobtoolkit_pipeline.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/add_summary_to_metadata.py` & `blobtoolkit-pipeline-4.1.4/src/lib/add_summary_to_metadata.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/chunk_fasta.py` & `blobtoolkit-pipeline-4.1.4/src/lib/chunk_fasta.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/count_busco_genes.py` & `blobtoolkit-pipeline-4.1.4/src/lib/count_busco_genes.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/data.py` & `blobtoolkit-pipeline-4.1.4/src/lib/data.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/functions.py` & `blobtoolkit-pipeline-4.1.4/src/lib/functions.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/generate_config.py` & `blobtoolkit-pipeline-4.1.4/src/lib/generate_config.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/generate_static_images.py` & `blobtoolkit-pipeline-4.1.4/src/lib/generate_static_images.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/lsf_wrapper.sh` & `blobtoolkit-pipeline-4.1.4/src/lib/lsf_wrapper.sh`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/resume_pipeline.py` & `blobtoolkit-pipeline-4.1.4/src/lib/resume_pipeline.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/run.py` & `blobtoolkit-pipeline-4.1.4/src/lib/run.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/run_btk_pipeline.sh` & `blobtoolkit-pipeline-4.1.4/src/lib/run_btk_pipeline.sh`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/track_bioproject_accessions.py` & `blobtoolkit-pipeline-4.1.4/src/lib/track_bioproject_accessions.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/transfer_completed.py` & `blobtoolkit-pipeline-4.1.4/src/lib/transfer_completed.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/unchunk_blast.py` & `blobtoolkit-pipeline-4.1.4/src/lib/unchunk_blast.py`

 * *Files identical despite different names*

### Comparing `blobtoolkit-pipeline-4.1.3/src/lib/window_stats.py` & `blobtoolkit-pipeline-4.1.4/src/lib/window_stats.py`

 * *Files identical despite different names*

