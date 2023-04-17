# Comparing `tmp/pyiohat-1.8.8.tar.gz` & `tmp/pyiohat-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiohat-1.8.8.tar", last modified: Wed Mar 15 12:27:39 2023, max compression
+gzip compressed data, was "pyiohat-1.8.9.tar", last modified: Mon Mar 27 14:52:50 2023, max compression
```

## Comparing `pyiohat-1.8.8.tar` & `pyiohat-1.8.9.tar`

### file list

```diff
@@ -1,107 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.276689 pyiohat-1.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-15 12:27:31.000000 pyiohat-1.8.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.256688 pyiohat-1.8.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-15 12:27:31.000000 pyiohat-1.8.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.256688 pyiohat-1.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-15 12:27:31.000000 pyiohat-1.8.8/.github/workflows/build_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-15 12:27:31.000000 pyiohat-1.8.8/.github/workflows/pypi_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-15 12:27:31.000000 pyiohat-1.8.8/.github/workflows/tox_ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-15 12:27:31.000000 pyiohat-1.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-15 12:27:31.000000 pyiohat-1.8.8/AUTHORS.TXT
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 12:27:31.000000 pyiohat-1.8.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-15 12:27:31.000000 pyiohat-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-15 12:27:31.000000 pyiohat-1.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-15 12:27:31.000000 pyiohat-1.8.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-15 12:27:39.276689 pyiohat-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-15 12:27:31.000000 pyiohat-1.8.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.256688 pyiohat-1.8.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:31.000000 pyiohat-1.8.8/docs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.256688 pyiohat-1.8.8/pyiohat/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.260688 pyiohat-1.8.8/pyiohat/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/base_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.260688 pyiohat-1.8.8/pyiohat/parsers/ident/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/comet_2020_01_4_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/dummy_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/mascot_2_6_2_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/msamanda_2_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/msfragger_3_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/msgfplus_2021_03_22_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/omssa_2_1_9_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident/xtandem_alanine.py
--rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/ident_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.260688 pyiohat-1.8.8/pyiohat/parsers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/models/base_parser_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/models/ident_parser_model.json
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/models/quant_parser_model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.260688 pyiohat-1.8.8/pyiohat/parsers/quant/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/quant/flash_lfq_1_2_0_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/parsers/quant_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/unify.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyiohat/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-15 12:27:38.000000 pyiohat-1.8.8/pyiohat/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.260688 pyiohat-1.8.8/pyiohat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-15 12:27:39.000000 pyiohat-1.8.8/pyiohat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-15 12:27:39.000000 pyiohat-1.8.8/pyiohat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 12:27:39.000000 pyiohat-1.8.8/pyiohat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-15 12:27:39.000000 pyiohat-1.8.8/pyiohat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-15 12:27:39.000000 pyiohat-1.8.8/pyiohat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-15 12:27:31.000000 pyiohat-1.8.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-15 12:27:39.280689 pyiohat-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-15 12:27:31.000000 pyiohat-1.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.260688 pyiohat-1.8.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.276689 pyiohat-1.8.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA.fasta
--rw-r--r--   0 runner    (1001) docker     (123)    78801 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_comet_2020_01_4.mzid
--rw-r--r--   0 runner    (1001) docker     (123)  2545955 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_mascot_2_6_2.dat
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_msamanda_2_0_0_17442.csv
--rw-r--r--   0 runner    (1001) docker     (123)   778898 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_msfragger_3.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   186828 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_msgfplus_2021_03_22.mzid
--rw-r--r--   0 runner    (1001) docker     (123)   186575 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_msgfplus_2021_03_22_unknown_mod.mzid
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_open_search.msfragger.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    73367 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_ursgal_lookup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_ursgal_lookup_no_precursor_mz.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA1_xtandem_alanine.xml
--rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/BSA2_ursgal_lookup.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/_ursgal_lookup.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/custom_mod.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/flash_lfq_1_2_0_quantified_peaks.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/human_ecoli_test_target_decoy.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.276689 pyiohat-1.8.8/tests/data/mapping_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/mapping_data/trunc_comet.mzid
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/mapping_data/trunc_fasta.protein.faa
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/mapping_data/trunc_meta.spectra_meta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/mapping_data/trunc_msfragger.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/mapping_data/trunc_msgfplus.mzid
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/mapping_data/trunc_omssa.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15214 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/mapping_data/trunc_xtandem.xml
--rw-r--r--   0 runner    (1001) docker     (123)    24428 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/multiple_psms_xtandem.xml
--rw-r--r--   0 runner    (1001) docker     (123)   778898 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/test_Creinhardtii_QE_pH11_msfragger_3.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    51125 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/test_Creinhardtii_QE_pH11_omssa_2_1_9.csv
--rw-r--r--   0 runner    (1001) docker     (123)   515024 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/test_Creinhardtii_QE_pH11_xtandem_alanine.xml
--rw-r--r--   0 runner    (1001) docker     (123)  1927170 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/test_Creinhardtii_target_decoy.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/data/test_positions_msfragger.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.276689 pyiohat-1.8.8/tests/ident/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/ident/test_engine_parser_comet_2020_01_04.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/ident/test_engine_parser_mascot_2_6_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/ident/test_engine_parser_msamanda.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/ident/test_engine_parser_msfragger_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/ident/test_engine_parser_msgfplus_2021_03_22.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/ident/test_engine_parser_omssa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/ident/test_engine_parser_xtandem_alanine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.276689 pyiohat-1.8.8/tests/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/mapping/test_TMTpro_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.256688 pyiohat-1.8.8/tests/parsers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.276689 pyiohat-1.8.8/tests/parsers/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/parsers/misc/test_get_atom_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 12:27:39.276689 pyiohat-1.8.8/tests/quant/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/quant/test_engine_parser_flash_lfq_1_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/test_engine_parser_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/test_engine_parser_ident_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/test_engine_parser_quant_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-03-15 12:27:31.000000 pyiohat-1.8.8/tests/test_unify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.517501 pyiohat-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-27 14:52:38.000000 pyiohat-1.8.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.501502 pyiohat-1.8.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-27 14:52:38.000000 pyiohat-1.8.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.501502 pyiohat-1.8.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-27 14:52:38.000000 pyiohat-1.8.9/.github/workflows/build_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-27 14:52:38.000000 pyiohat-1.8.9/.github/workflows/pypi_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-27 14:52:38.000000 pyiohat-1.8.9/.github/workflows/tox_ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-27 14:52:38.000000 pyiohat-1.8.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 14:52:38.000000 pyiohat-1.8.9/AUTHORS.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:52:38.000000 pyiohat-1.8.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-27 14:52:38.000000 pyiohat-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-27 14:52:38.000000 pyiohat-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-27 14:52:38.000000 pyiohat-1.8.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-27 14:52:50.517501 pyiohat-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-27 14:52:38.000000 pyiohat-1.8.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.501502 pyiohat-1.8.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:38.000000 pyiohat-1.8.9/docs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.501502 pyiohat-1.8.9/pyiohat/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.505502 pyiohat-1.8.9/pyiohat/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/base_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.505502 pyiohat-1.8.9/pyiohat/parsers/ident/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/comet_2020_01_4_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/dummy_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/mascot_2_6_2_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/msamanda_2_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/msfragger_3_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/msgfplus_2021_03_22_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/omssa_2_1_9_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident/xtandem_alanine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14483 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/ident_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.505502 pyiohat-1.8.9/pyiohat/parsers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/models/base_parser_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/models/ident_parser_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/models/quant_parser_model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.505502 pyiohat-1.8.9/pyiohat/parsers/quant/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/quant/flash_lfq_1_2_0_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/quant/tmt_quant_parser_1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/parsers/quant_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/unify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyiohat/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 14:52:50.000000 pyiohat-1.8.9/pyiohat/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.501502 pyiohat-1.8.9/pyiohat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-27 14:52:50.000000 pyiohat-1.8.9/pyiohat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-03-27 14:52:50.000000 pyiohat-1.8.9/pyiohat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:52:50.000000 pyiohat-1.8.9/pyiohat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-27 14:52:50.000000 pyiohat-1.8.9/pyiohat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-27 14:52:50.000000 pyiohat-1.8.9/pyiohat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-27 14:52:38.000000 pyiohat-1.8.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-27 14:52:50.517501 pyiohat-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-27 14:52:38.000000 pyiohat-1.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.505502 pyiohat-1.8.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.513502 pyiohat-1.8.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)    78801 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_comet_2020_01_4.mzid
+-rw-r--r--   0 runner    (1001) docker     (123)  2545955 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_mascot_2_6_2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_msamanda_2_0_0_17442.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   778898 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_msfragger_3.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   186828 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_msgfplus_2021_03_22.mzid
+-rw-r--r--   0 runner    (1001) docker     (123)   186575 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_msgfplus_2021_03_22_unknown_mod.mzid
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_open_search.msfragger.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    73367 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_ursgal_lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_ursgal_lookup_no_precursor_mz.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA1_xtandem_alanine.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    73433 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/BSA2_ursgal_lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/TMT16_ursgal_lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/_ursgal_lookup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/custom_mod.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/flash_lfq_1_2_0_quantified_peaks.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/human_ecoli_test_target_decoy.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.513502 pyiohat-1.8.9/tests/data/mapping_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_comet.mzid
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_fasta.protein.faa
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_meta.spectra_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_msfragger.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_msgfplus.mzid
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_omssa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_tmt_quant.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15214 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/mapping_data/trunc_xtandem.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24428 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/multiple_psms_xtandem.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   778898 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/test_Creinhardtii_QE_pH11_msfragger_3.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    51125 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/test_Creinhardtii_QE_pH11_omssa_2_1_9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   515024 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/test_Creinhardtii_QE_pH11_xtandem_alanine.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  1927170 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/test_Creinhardtii_target_decoy.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/data/test_positions_msfragger.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.517501 pyiohat-1.8.9/tests/ident/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/ident/test_engine_parser_comet_2020_01_04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/ident/test_engine_parser_mascot_2_6_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/ident/test_engine_parser_msamanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/ident/test_engine_parser_msfragger_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/ident/test_engine_parser_msgfplus_2021_03_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/ident/test_engine_parser_omssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/ident/test_engine_parser_xtandem_alanine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.517501 pyiohat-1.8.9/tests/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/mapping/test_TMTpro_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.501502 pyiohat-1.8.9/tests/parsers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.517501 pyiohat-1.8.9/tests/parsers/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/parsers/misc/test_get_atom_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:52:50.517501 pyiohat-1.8.9/tests/quant/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/quant/test_engine_parser_flash_lfq_1_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/quant/test_tmt_quant_1_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/test_engine_parser_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21178 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/test_engine_parser_ident_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/test_engine_parser_quant_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-03-27 14:52:38.000000 pyiohat-1.8.9/tests/test_unify.py
```

### Comparing `pyiohat-1.8.8/.github/workflows/build_docs.yml` & `pyiohat-1.8.9/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/.github/workflows/tox_ci.yml` & `pyiohat-1.8.9/.github/workflows/tox_ci.yml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/.gitignore` & `pyiohat-1.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/LICENSE` & `pyiohat-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/PKG-INFO` & `pyiohat-1.8.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiohat
-Version: 1.8.8
+Version: 1.8.9
 Summary: Python Mass Spectrometry Input Output Harmonization Tool
 Home-page: https://github.com/computational-ms/pyiohat
 Author: Tristan Ranff, Manuel Kösters, Artyom Vlasov, Christian Fufezan
 Author-email: christian@fufezan.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pyiohat-1.8.8/README.rst` & `pyiohat-1.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/base_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/comet_2020_01_4_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/comet_2020_01_4_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/dummy_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/dummy_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/mascot_2_6_2_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/mascot_2_6_2_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/msamanda_2_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/msamanda_2_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/msfragger_3_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/msfragger_3_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/msgfplus_2021_03_22_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/msgfplus_2021_03_22_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/omssa_2_1_9_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/omssa_2_1_9_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident/xtandem_alanine.py` & `pyiohat-1.8.9/pyiohat/parsers/ident/xtandem_alanine.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/ident_base_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/ident_base_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/misc.py` & `pyiohat-1.8.9/pyiohat/parsers/misc.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/models/base_parser_model.json` & `pyiohat-1.8.9/pyiohat/parsers/models/base_parser_model.json`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/models/ident_parser_model.json` & `pyiohat-1.8.9/pyiohat/parsers/models/ident_parser_model.json`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/parsers/models/quant_parser_model.json` & `pyiohat-1.8.9/pyiohat/parsers/models/quant_parser_model.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {'insert': "[(1, OrderedDict([('name', 'reported_mz'), ('description', 'mz reported by quant "*

 * *           "engine'), ('dtype', 'float')])), (2, OrderedDict([('name', 'theoretical_mz'), "*

 * *           "('description', 'theoretical mz of quantified molecule'), ('dtype', 'float')])), (11, "*

 * *           "OrderedDict([('name', 'quant_engine'), ('description', 'Name of the quantification "*

 * *           "engine.'), ('dtype', 'str')]))]"}*

```diff
@@ -1,14 +1,24 @@
 [
     {
         "description": "Trivial compound name",
         "dtype": "str",
         "name": "trivial_name"
     },
     {
+        "description": "mz reported by quant engine",
+        "dtype": "float",
+        "name": "reported_mz"
+    },
+    {
+        "description": "theoretical mz of quantified molecule",
+        "dtype": "float",
+        "name": "theoretical_mz"
+    },
+    {
         "description": "Quantification result value",
         "dtype": "float32",
         "name": "quant_value"
     },
     {
         "description": "Quantification score value (e.g. m-score)",
         "dtype": "float32",
@@ -39,9 +49,14 @@
         "dtype": "Int32",
         "name": "ident_reference"
     },
     {
         "description": "Full width at half maximum",
         "dtype": "float32",
         "name": "fwhm"
+    },
+    {
+        "description": "Name of the quantification engine.",
+        "dtype": "str",
+        "name": "quant_engine"
     }
 ]
```

### Comparing `pyiohat-1.8.8/pyiohat/parsers/quant/flash_lfq_1_2_0_parser.py` & `pyiohat-1.8.9/pyiohat/parsers/quant/flash_lfq_1_2_0_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,37 +92,41 @@
         Returns:
             self.df (pd.DataFrame): unified dataframe
         """
         # TODO: fill this
         # raise NotImplementedError
         # do column conversion here
         self.df["spectrum_id"] = -1
-        self.df["linked_spectrum_id"] = -1
+        self.df["ident_reference"] = -1
         self.df["retention_time_seconds"] = -1
         self.df["accuracy_ppm_C12"] = -1
         self.df["quant_score"] = -1
         self.df["fwhm"] = -1
         self.df["label"] = "LabelFree"
         self.df["quant_group"] = ""
+        self.df["ccs"] = -1
+        self.df.loc[self.df["flashlfq:mbr_score"].isna(), "flashlfq:mbr_score"] = -1
 
         self.get_chemical_composition()
         self.get_meta_info()
+        self.calculate_accuracy()
         self.df["quant_run_id"] = "FlashLFQ"
+        self.df["quant_engines"] = "FlashLFQ_1_2_0"
 
         self.process_unify_style()
         return self.df
 
     def get_meta_info(self):
         self.df["raw_filename"] = self.df["raw_filename"].map(self.filestem_to_path)
         rounded_rts = (self.df["flashlfq:ms2_retention_time"] / 60).apply(
             round, args=(self.round_precision,)
         )
         rounded_rts = pd.DataFrame({"file": self.df["raw_filename"], "rt": rounded_rts})
 
-        self.df["linked_spectrum_id"] = [
+        self.df["ident_reference"] = [
             self.rt_to_spec_id[f][r] for i, (f, r) in rounded_rts.iterrows()
         ]
 
     def get_chemical_composition(self):
         mods = self.df["flashlfq:full_sequence"].apply(self.translate_mods)
         seqs = self.df["trivial_name"]
```

### Comparing `pyiohat-1.8.8/pyiohat/unify.py` & `pyiohat-1.8.9/pyiohat/unify.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat/utils.py` & `pyiohat-1.8.9/pyiohat/utils.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/pyiohat.egg-info/PKG-INFO` & `pyiohat-1.8.9/pyiohat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiohat
-Version: 1.8.8
+Version: 1.8.9
 Summary: Python Mass Spectrometry Input Output Harmonization Tool
 Home-page: https://github.com/computational-ms/pyiohat
 Author: Tristan Ranff, Manuel Kösters, Artyom Vlasov, Christian Fufezan
 Author-email: christian@fufezan.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pyiohat-1.8.8/pyiohat.egg-info/SOURCES.txt` & `pyiohat-1.8.9/pyiohat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 pyiohat/parsers/ident/omssa_2_1_9_parser.py
 pyiohat/parsers/ident/xtandem_alanine.py
 pyiohat/parsers/models/base_parser_model.json
 pyiohat/parsers/models/ident_parser_model.json
 pyiohat/parsers/models/quant_parser_model.json
 pyiohat/parsers/quant/__init__.py
 pyiohat/parsers/quant/flash_lfq_1_2_0_parser.py
+pyiohat/parsers/quant/tmt_quant_parser_1_0_0.py
 tests/conftest.py
 tests/test_engine_parser_base_parser.py
 tests/test_engine_parser_ident_base_parser.py
 tests/test_engine_parser_quant_base_parser.py
 tests/test_unify.py
 tests/data/BSA.fasta
 tests/data/BSA1_comet_2020_01_4.mzid
@@ -55,14 +56,15 @@
 tests/data/BSA1_msgfplus_2021_03_22.mzid
 tests/data/BSA1_msgfplus_2021_03_22_unknown_mod.mzid
 tests/data/BSA1_open_search.msfragger.tsv
 tests/data/BSA1_ursgal_lookup.csv
 tests/data/BSA1_ursgal_lookup_no_precursor_mz.csv
 tests/data/BSA1_xtandem_alanine.xml
 tests/data/BSA2_ursgal_lookup.csv
+tests/data/TMT16_ursgal_lookup.csv
 tests/data/_ursgal_lookup.csv
 tests/data/custom_mod.xml
 tests/data/flash_lfq_1_2_0_quantified_peaks.tsv
 tests/data/human_ecoli_test_target_decoy.fasta
 tests/data/multiple_psms_xtandem.xml
 tests/data/test_Creinhardtii_QE_pH11_msfragger_3.tsv
 tests/data/test_Creinhardtii_QE_pH11_omssa_2_1_9.csv
@@ -71,18 +73,20 @@
 tests/data/test_positions_msfragger.tsv
 tests/data/mapping_data/trunc_comet.mzid
 tests/data/mapping_data/trunc_fasta.protein.faa
 tests/data/mapping_data/trunc_meta.spectra_meta.csv
 tests/data/mapping_data/trunc_msfragger.tsv
 tests/data/mapping_data/trunc_msgfplus.mzid
 tests/data/mapping_data/trunc_omssa.csv
+tests/data/mapping_data/trunc_tmt_quant.csv
 tests/data/mapping_data/trunc_xtandem.xml
 tests/ident/test_engine_parser_comet_2020_01_04.py
 tests/ident/test_engine_parser_mascot_2_6_2.py
 tests/ident/test_engine_parser_msamanda.py
 tests/ident/test_engine_parser_msfragger_3.py
 tests/ident/test_engine_parser_msgfplus_2021_03_22.py
 tests/ident/test_engine_parser_omssa.py
 tests/ident/test_engine_parser_xtandem_alanine.py
 tests/mapping/test_TMTpro_mapping.py
 tests/parsers/misc/test_get_atom_counts.py
-tests/quant/test_engine_parser_flash_lfq_1_2_0.py
+tests/quant/test_engine_parser_flash_lfq_1_2_0.py
+tests/quant/test_tmt_quant_1_0_0.py
```

### Comparing `pyiohat-1.8.8/pyproject.toml` & `pyiohat-1.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/setup.cfg` & `pyiohat-1.8.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 	peptide-mapper~=0.4.3
 	chemical-composition~=1.0.6
 	pyahocorasick>=1.4.4,<2.1.0
 	pandas>=1.4.3,<1.6.0
 	numpy>=1.22.0
 	loguru~=0.6.0
 	tqdm>=4.64,<4.66
-	regex>=2022.7.25,<2022.11.0
+	regex>=2022.7.25,<2023.4.0
 	uparma>=0.9.15,<1.1.0
 	IsoSpecPy~=2.2.0
 
 [options.package_data]
 * = *.txt
 
 [options.extras_require]
```

### Comparing `pyiohat-1.8.8/setup.py` & `pyiohat-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA.fasta` & `pyiohat-1.8.9/tests/data/BSA.fasta`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_comet_2020_01_4.mzid` & `pyiohat-1.8.9/tests/data/BSA1_comet_2020_01_4.mzid`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_mascot_2_6_2.dat` & `pyiohat-1.8.9/tests/data/BSA1_mascot_2_6_2.dat`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_msamanda_2_0_0_17442.csv` & `pyiohat-1.8.9/tests/data/BSA1_msamanda_2_0_0_17442.csv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_msfragger_3.tsv` & `pyiohat-1.8.9/tests/data/BSA1_msfragger_3.tsv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_msgfplus_2021_03_22.mzid` & `pyiohat-1.8.9/tests/data/BSA1_msgfplus_2021_03_22.mzid`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_msgfplus_2021_03_22_unknown_mod.mzid` & `pyiohat-1.8.9/tests/data/BSA1_msgfplus_2021_03_22_unknown_mod.mzid`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_open_search.msfragger.tsv` & `pyiohat-1.8.9/tests/data/BSA1_open_search.msfragger.tsv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_ursgal_lookup.csv` & `pyiohat-1.8.9/tests/data/BSA1_ursgal_lookup.csv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA1_xtandem_alanine.xml` & `pyiohat-1.8.9/tests/data/BSA1_xtandem_alanine.xml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/BSA2_ursgal_lookup.csv` & `pyiohat-1.8.9/tests/data/BSA2_ursgal_lookup.csv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/_ursgal_lookup.csv` & `pyiohat-1.8.9/tests/data/_ursgal_lookup.csv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/custom_mod.xml` & `pyiohat-1.8.9/tests/data/custom_mod.xml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/flash_lfq_1_2_0_quantified_peaks.tsv` & `pyiohat-1.8.9/tests/data/flash_lfq_1_2_0_quantified_peaks.tsv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/human_ecoli_test_target_decoy.fasta` & `pyiohat-1.8.9/tests/data/human_ecoli_test_target_decoy.fasta`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/mapping_data/trunc_comet.mzid` & `pyiohat-1.8.9/tests/data/mapping_data/trunc_comet.mzid`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/mapping_data/trunc_fasta.protein.faa` & `pyiohat-1.8.9/tests/data/mapping_data/trunc_fasta.protein.faa`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/mapping_data/trunc_meta.spectra_meta.csv` & `pyiohat-1.8.9/tests/data/mapping_data/trunc_meta.spectra_meta.csv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/mapping_data/trunc_msfragger.tsv` & `pyiohat-1.8.9/tests/data/mapping_data/trunc_msfragger.tsv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/mapping_data/trunc_msgfplus.mzid` & `pyiohat-1.8.9/tests/data/mapping_data/trunc_msgfplus.mzid`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/mapping_data/trunc_xtandem.xml` & `pyiohat-1.8.9/tests/data/mapping_data/trunc_xtandem.xml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/multiple_psms_xtandem.xml` & `pyiohat-1.8.9/tests/data/multiple_psms_xtandem.xml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/test_Creinhardtii_QE_pH11_msfragger_3.tsv` & `pyiohat-1.8.9/tests/data/test_Creinhardtii_QE_pH11_msfragger_3.tsv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/test_Creinhardtii_QE_pH11_omssa_2_1_9.csv` & `pyiohat-1.8.9/tests/data/test_Creinhardtii_QE_pH11_omssa_2_1_9.csv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/test_Creinhardtii_QE_pH11_xtandem_alanine.xml` & `pyiohat-1.8.9/tests/data/test_Creinhardtii_QE_pH11_xtandem_alanine.xml`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/test_Creinhardtii_target_decoy.fasta` & `pyiohat-1.8.9/tests/data/test_Creinhardtii_target_decoy.fasta`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/data/test_positions_msfragger.tsv` & `pyiohat-1.8.9/tests/data/test_positions_msfragger.tsv`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/ident/test_engine_parser_comet_2020_01_04.py` & `pyiohat-1.8.9/tests/ident/test_engine_parser_comet_2020_01_04.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/ident/test_engine_parser_mascot_2_6_2.py` & `pyiohat-1.8.9/tests/ident/test_engine_parser_mascot_2_6_2.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/ident/test_engine_parser_msamanda.py` & `pyiohat-1.8.9/tests/ident/test_engine_parser_msamanda.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/ident/test_engine_parser_msfragger_3.py` & `pyiohat-1.8.9/tests/ident/test_engine_parser_msfragger_3.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/ident/test_engine_parser_msgfplus_2021_03_22.py` & `pyiohat-1.8.9/tests/ident/test_engine_parser_msgfplus_2021_03_22.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/ident/test_engine_parser_omssa.py` & `pyiohat-1.8.9/tests/ident/test_engine_parser_omssa.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/ident/test_engine_parser_xtandem_alanine.py` & `pyiohat-1.8.9/tests/ident/test_engine_parser_xtandem_alanine.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/mapping/test_TMTpro_mapping.py` & `pyiohat-1.8.9/tests/mapping/test_TMTpro_mapping.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/parsers/misc/test_get_atom_counts.py` & `pyiohat-1.8.9/tests/parsers/misc/test_get_atom_counts.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/quant/test_engine_parser_flash_lfq_1_2_0.py` & `pyiohat-1.8.9/tests/quant/test_engine_parser_flash_lfq_1_2_0.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/test_engine_parser_base_parser.py` & `pyiohat-1.8.9/tests/test_engine_parser_base_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/test_engine_parser_ident_base_parser.py` & `pyiohat-1.8.9/tests/test_engine_parser_ident_base_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/test_engine_parser_quant_base_parser.py` & `pyiohat-1.8.9/tests/test_engine_parser_quant_base_parser.py`

 * *Files identical despite different names*

### Comparing `pyiohat-1.8.8/tests/test_unify.py` & `pyiohat-1.8.9/tests/test_unify.py`

 * *Files identical despite different names*

