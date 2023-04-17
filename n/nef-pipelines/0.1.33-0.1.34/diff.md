# Comparing `tmp/nef_pipelines-0.1.33.tar.gz` & `tmp/nef_pipelines-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.33.tar", last modified: Sat Apr 15 16:26:08 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.34.tar", last modified: Mon Apr 17 20:51:08 2023, max compression
```

## Comparing `nef_pipelines-0.1.33.tar` & `nef_pipelines-0.1.34.tar`

### file list

```diff
@@ -1,334 +1,341 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.697196 nef_pipelines-0.1.33/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.587116 nef_pipelines-0.1.33/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.651299 nef_pipelines-0.1.33/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.33/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.669834 nef_pipelines-0.1.33/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.33/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.33/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.674463 nef_pipelines-0.1.33/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.33/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      404 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.33/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.33/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.33/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     2595 2023-03-19 15:56:44.000000 nef_pipelines-0.1.33/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.33/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.33/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-15 16:26:08.697457 nef_pipelines-0.1.33/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.33/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.33/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.33/pyproject.toml
--rw-r--r--   0 garythompson   (501) staff       (20)     1002 2023-04-15 16:20:01.000000 nef_pipelines-0.1.33/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      352 2023-04-15 16:14:41.000000 nef_pipelines-0.1.33/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1575 2023-04-15 16:26:08.699523 nef_pipelines-0.1.33/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.33/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.588472 nef_pipelines-0.1.33/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.684162 nef_pipelines-0.1.33/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.33/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.720287 nef_pipelines-0.1.33/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-01-31 10:45:30.000000 nef_pipelines-0.1.33/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.766706 nef_pipelines-0.1.33/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2636 2023-03-20 08:57:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16036 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    13851 2023-03-20 21:01:51.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    19514 2023-03-18 23:11:49.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3828 2023-03-19 15:41:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8776 2023-02-05 14:12:26.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.769913 nef_pipelines-0.1.33/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20435 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5239 2023-03-24 21:55:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.773118 nef_pipelines-0.1.33/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.795419 nef_pipelines-0.1.33/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.807378 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.811151 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.821369 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.824399 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.825363 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.834704 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.844240 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.848060 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)    64962 2023-04-15 12:23:49.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/ubiquitin_short.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_delete.py
--rwxr--r--   0 garythompson   (501) staff       (20)     1123 2022-12-16 21:06:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_rename.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_tabulate.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.857626 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.880762 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.909017 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.959303 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14354 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.005104 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.072936 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.110021 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.113827 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.115316 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.135901 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.142044 nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.147039 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.174141 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.181592 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/test_agv.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7643 2023-03-18 23:11:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/test_test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.215656 nef_pipelines-0.1.33/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.239313 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.303883 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.337562 nef_pipelines-0.1.33/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.362146 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2592 2022-12-13 19:17:42.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.368950 nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.387406 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7769 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6717 2023-04-15 16:16:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.394934 nef_pipelines-0.1.33/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.399812 nef_pipelines-0.1.33/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10429 2023-04-15 16:17:03.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-03-11 19:52:51.000000 nef_pipelines-0.1.33/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.403390 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.405781 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.409635 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.414249 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.418012 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.441394 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-01-16 22:41:06.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.446899 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.463966 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.468506 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11481 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.494129 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.504422 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3373 2023-02-07 21:14:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3019 2023-02-07 21:08:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20232 2022-11-27 19:45:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.508925 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.544689 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.556385 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2196 2022-11-27 19:45:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5647 2023-02-07 23:05:11.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.559407 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.566616 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10789 2023-01-30 23:23:18.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.590782 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.594354 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.600157 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.604192 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.607510 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.611914 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6315 2023-02-08 23:35:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.615278 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      727 2023-03-20 21:00:52.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.646853 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17136 2023-03-24 20:03:59.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.654545 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14367 2023-03-21 20:30:29.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.657627 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.660883 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.682099 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.687390 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:08.696048 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-15 16:26:07.696172 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    12466 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-04-15 16:26:07.000000 nef_pipelines-0.1.33/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.33/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.354593 nef_pipelines-0.1.34/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.034724 nef_pipelines-0.1.34/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.103095 nef_pipelines-0.1.34/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.34/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.127668 nef_pipelines-0.1.34/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.34/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.34/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.34/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.133732 nef_pipelines-0.1.34/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.34/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.34/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.34/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      404 2023-04-17 20:49:49.000000 nef_pipelines-0.1.34/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.34/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.34/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.34/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     2595 2023-03-19 15:56:44.000000 nef_pipelines-0.1.34/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.34/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.34/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-17 20:51:08.354925 nef_pipelines-0.1.34/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.34/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.34/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.34/pyproject.toml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.202513 nef_pipelines-0.1.34/references/
+-rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.34/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.34/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garythompson   (501) staff       (20)     1193 2023-04-15 16:42:43.000000 nef_pipelines-0.1.34/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.34/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1575 2023-04-17 20:51:08.358011 nef_pipelines-0.1.34/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.34/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.035538 nef_pipelines-0.1.34/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.273186 nef_pipelines-0.1.34/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.34/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.305261 nef_pipelines-0.1.34/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-01-31 10:45:30.000000 nef_pipelines-0.1.34/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.365141 nef_pipelines-0.1.34/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2782 2023-04-17 20:22:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16143 2023-04-15 16:57:10.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14630 2023-04-17 20:22:42.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    19514 2023-03-18 23:11:49.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3828 2023-03-19 15:41:24.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8776 2023-02-05 14:12:26.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.370948 nef_pipelines-0.1.34/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    22250 2023-04-17 20:19:05.000000 nef_pipelines-0.1.34/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5239 2023-03-24 21:55:44.000000 nef_pipelines-0.1.34/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.372752 nef_pipelines-0.1.34/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.394120 nef_pipelines-0.1.34/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.413478 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.418757 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.434206 nef_pipelines-0.1.34/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.436828 nef_pipelines-0.1.34/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.437311 nef_pipelines-0.1.34/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.440924 nef_pipelines-0.1.34/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.474121 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.477156 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1123 2023-04-15 16:57:25.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_tabulate.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.486258 nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.491034 nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.517031 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.573592 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14354 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.618155 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.685043 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.696100 nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.699912 nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.722936 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.734829 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.735585 nef_pipelines-0.1.34/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.740064 nef_pipelines-0.1.34/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.785038 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.833431 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.838502 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7643 2023-03-18 23:11:48.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/test_test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.844077 nef_pipelines-0.1.34/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.900908 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.949710 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.977894 nef_pipelines-0.1.34/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.996652 nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2592 2022-12-13 19:17:42.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.010637 nef_pipelines-0.1.34/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.025176 nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6996 2023-04-15 16:55:03.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.031431 nef_pipelines-0.1.34/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.036151 nef_pipelines-0.1.34/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7071 2023-04-17 20:30:43.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.34/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.048209 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.051348 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.055331 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.058983 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.062172 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.064562 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-01-16 22:41:06.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.070169 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.112321 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.118891 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11481 2023-03-19 00:07:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.128298 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.162317 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3373 2023-02-07 21:14:19.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3019 2023-02-07 21:08:19.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20232 2022-11-27 19:45:21.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.169373 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.184349 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.217451 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2196 2022-11-27 19:45:21.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5647 2023-02-07 23:05:11.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.220288 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.228155 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10789 2023-01-30 23:23:18.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.231585 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.234340 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.245018 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.248969 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.256968 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.263047 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6315 2023-02-08 23:35:44.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.268982 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      727 2023-03-20 21:00:52.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.273303 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17136 2023-03-24 20:03:59.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.281386 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14367 2023-03-21 20:30:29.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.285123 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.289571 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.332867 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.340294 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:08.352886 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-17 20:51:07.286361 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-17 20:51:06.000000 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    12685 2023-04-17 20:51:07.000000 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-04-17 20:51:06.000000 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-04-17 20:51:06.000000 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-04-17 20:51:06.000000 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-04-17 20:51:06.000000 nef_pipelines-0.1.34/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.34/tox.ini
```

### Comparing `nef_pipelines-0.1.33/.github/workflows/ci.yml` & `nef_pipelines-0.1.34/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.34/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/.pre-commit-config.yaml` & `nef_pipelines-0.1.34/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/CHANGELOG.md` & `nef_pipelines-0.1.34/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/CONTRIBUTING.md` & `nef_pipelines-0.1.34/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/LICENSE.txt` & `nef_pipelines-0.1.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/PKG-INFO` & `nef_pipelines-0.1.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.33
+Version: 0.1.34
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.33/README.md` & `nef_pipelines-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/TODO.md` & `nef_pipelines-0.1.34/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/release_to_pypi.sh` & `nef_pipelines-0.1.34/release_to_pypi.sh`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # add check for uncommitted or auto stash
 git update-index --refresh >/dev/null
 git diff-index --quiet HEAD --
 
-test $? -eq 0 || echo "ERROR: the repo is dirty clean it before building!"; exit 1
+
+if [[ $? -ne 0 ]]; then
+	echo "ERROR: the repo is dirty clean it before building!"
+    exit 1
+fi
+
+echo got here
 
 # define where the version file is found
 VERSION_FILE=src/nef_pipelines/VERSION
 
 # cheange to the correct working directory
 cd /Users/garythompson/Dropbox/nef_pipelines/nef_pipelines
 
@@ -24,15 +30,19 @@
 # update the version  in the repo
 git add src/nef_pipelines/VERSION
 git commit -m "updated version to $VERSION" --no-verify
 
 ver  --file $VERSION_FILE tag
 
 # stash any uncommited changes to avoid version+1 errors
-git stash
+stash_message="stashed-for-pypi-drop-${VERSION}-`date +%s`"
+git stash --message ${stash_message}
 
 #build and publish
 tox -e build  # to build your package distribution
 tox -e publish -- --repository pypi
 
-# unstash uncommitted changes
-git stash pop
+git stash list  | grep -q ${stash_message}
+if [[ $? -eq 0 ]]; then
+  # unstash uncommitted changes
+  git stash pop
+fi
```

### Comparing `nef_pipelines-0.1.33/setup.cfg` & `nef_pipelines-0.1.34/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/setup.py` & `nef_pipelines-0.1.34/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.34/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,165 +1,174 @@
-00000000: 5350 4543 5452 554d 5f46 5241 4d45 5f43  SPECTRUM_FRAME_C
-00000010: 4154 4547 4f52 5920 3d20 226e 6566 5f6e  ATEGORY = "nef_n
-00000020: 6d72 5f73 7065 6374 7275 6d22 0a53 5045  mr_spectrum".SPE
-00000030: 4354 5255 4d5f 4449 4d45 4e53 494f 4e5f  CTRUM_DIMENSION_
-00000040: 4c4f 4f50 5f43 4154 4547 4f52 5920 3d20  LOOP_CATEGORY = 
-00000050: 226e 6566 5f73 7065 6374 7275 6d5f 6469  "nef_spectrum_di
-00000060: 6d65 6e73 696f 6e22 0a53 5045 4354 5255  mension".SPECTRU
-00000070: 4d5f 4449 4d45 4e53 494f 4e5f 5452 414e  M_DIMENSION_TRAN
-00000080: 5346 4552 5f4c 4f4f 505f 4341 5445 474f  SFER_LOOP_CATEGO
-00000090: 5259 203d 2028 0a20 2020 2066 227b 5350  RY = (.    f"{SP
-000000a0: 4543 5452 554d 5f44 494d 454e 5349 4f4e  ECTRUM_DIMENSION
-000000b0: 5f4c 4f4f 505f 4341 5445 474f 5259 7d5f  _LOOP_CATEGORY}_
-000000c0: 7472 616e 7366 6572 220a 290a 5350 4543  transfer".).SPEC
-000000d0: 5452 554d 5f50 4541 4b5f 4c4f 4f50 5f43  TRUM_PEAK_LOOP_C
-000000e0: 4154 4547 4f52 5920 3d20 226e 6566 5f70  ATEGORY = "nef_p
-000000f0: 6561 6b22 0a0a 5346 5f43 4154 4547 4f52  eak"..SF_CATEGOR
-00000100: 5920 3d20 2273 665f 6361 7465 676f 7279  Y = "sf_category
-00000110: 220a 5346 5f46 5241 4d45 434f 4445 203d  ".SF_FRAMECODE =
-00000120: 2022 7366 5f66 7261 6d65 636f 6465 220a   "sf_framecode".
-00000130: 4e55 4d5f 4449 4d45 4e53 494f 4e53 203d  NUM_DIMENSIONS =
-00000140: 2022 6e75 6d5f 6469 6d65 6e73 696f 6e73   "num_dimensions
-00000150: 220a 4348 454d 4943 414c 5f53 4849 4654  ".CHEMICAL_SHIFT
-00000160: 5f4c 4953 5420 3d20 2263 6865 6d69 6361  _LIST = "chemica
-00000170: 6c5f 7368 6966 745f 6c69 7374 220a 4558  l_shift_list".EX
-00000180: 5045 5249 4d45 4e54 5f54 5950 4520 3d20  PERIMENT_TYPE = 
-00000190: 2265 7870 6572 696d 656e 745f 7479 7065  "experiment_type
-000001a0: 220a 4558 5045 5249 4d45 4e54 5f43 4c41  ".EXPERIMENT_CLA
-000001b0: 5353 4946 4943 4154 494f 4e20 3d20 2265  SSIFICATION = "e
-000001c0: 7870 6572 696d 656e 745f 636c 6173 7369  xperiment_classi
-000001d0: 6669 6361 7469 6f6e 220a 0a53 5045 4354  fication"..SPECT
-000001e0: 5255 4d5f 4652 414d 455f 5441 4753 203d  RUM_FRAME_TAGS =
-000001f0: 2028 0a20 2020 2053 465f 4341 5445 474f   (.    SF_CATEGO
-00000200: 5259 2c0a 2020 2020 5346 5f46 5241 4d45  RY,.    SF_FRAME
-00000210: 434f 4445 2c0a 2020 2020 4e55 4d5f 4449  CODE,.    NUM_DI
-00000220: 4d45 4e53 494f 4e53 2c0a 2020 2020 4348  MENSIONS,.    CH
-00000230: 454d 4943 414c 5f53 4849 4654 5f4c 4953  EMICAL_SHIFT_LIS
-00000240: 542c 0a20 2020 2045 5850 4552 494d 454e  T,.    EXPERIMEN
-00000250: 545f 434c 4153 5349 4649 4341 5449 4f4e  T_CLASSIFICATION
-00000260: 2c0a 2020 2020 4558 5045 5249 4d45 4e54  ,.    EXPERIMENT
-00000270: 5f54 5950 452c 0a29 0a0a 4449 4d45 4e53  _TYPE,.)..DIMENS
-00000280: 494f 4e5f 4944 203d 2022 6469 6d65 6e73  ION_ID = "dimens
-00000290: 696f 6e5f 6964 220a 4158 4953 5f55 4e49  ion_id".AXIS_UNI
-000002a0: 5420 3d20 2261 7869 735f 756e 6974 220a  T = "axis_unit".
-000002b0: 4158 4953 5f43 4f44 4520 3d20 2261 7869  AXIS_CODE = "axi
-000002c0: 735f 636f 6465 220a 0a53 5045 4354 524f  s_code"..SPECTRO
-000002d0: 4d45 5445 525f 4652 4551 5545 4e43 5920  METER_FREQUENCY 
-000002e0: 3d20 2273 7065 6374 726f 6d65 7465 725f  = "spectrometer_
-000002f0: 6672 6571 7565 6e63 7922 0a53 5045 4354  frequency".SPECT
-00000300: 5241 4c5f 5749 4454 4820 3d20 2273 7065  RAL_WIDTH = "spe
-00000310: 6374 7261 6c5f 7769 6474 6822 0a56 414c  ctral_width".VAL
-00000320: 5545 5f46 4952 5354 5f50 4f49 4e54 203d  UE_FIRST_POINT =
-00000330: 2022 7661 6c75 655f 6669 7273 745f 706f   "value_first_po
-00000340: 696e 7422 0a46 4f4c 4449 4e47 203d 2022  int".FOLDING = "
-00000350: 666f 6c64 696e 6722 0a41 4253 4f4c 5554  folding".ABSOLUT
-00000360: 455f 5045 414b 5f50 4f53 4954 494f 4e53  E_PEAK_POSITIONS
-00000370: 203d 2022 6162 736f 6c75 7465 5f70 6561   = "absolute_pea
-00000380: 6b5f 706f 7369 7469 6f6e 7322 0a49 535f  k_positions".IS_
-00000390: 4143 5155 4953 4954 494f 4e20 3d20 2269  ACQUISITION = "i
-000003a0: 735f 6163 7175 6973 6974 696f 6e22 0a0a  s_acquisition"..
-000003b0: 0a44 494d 454e 5349 4f4e 5f4c 4f4f 505f  .DIMENSION_LOOP_
-000003c0: 5441 4753 203d 2028 0a20 2020 2023 206d  TAGS = (.    # m
-000003d0: 616e 6461 746f 7279 2070 6172 616d 6574  andatory paramet
-000003e0: 6572 730a 2020 2020 4449 4d45 4e53 494f  ers.    DIMENSIO
-000003f0: 4e5f 4944 2c0a 2020 2020 4158 4953 5f55  N_ID,.    AXIS_U
-00000400: 4e49 542c 0a20 2020 2041 5849 535f 434f  NIT,.    AXIS_CO
-00000410: 4445 2c0a 2020 2020 2320 2320 6f70 7469  DE,.    # # opti
-00000420: 6f6e 616c 2070 6172 616d 6574 6572 730a  onal parameters.
-00000430: 2020 2020 5350 4543 5452 4f4d 4554 4552      SPECTROMETER
-00000440: 5f46 5245 5155 454e 4359 2c0a 2020 2020  _FREQUENCY,.    
-00000450: 5350 4543 5452 414c 5f57 4944 5448 2c0a  SPECTRAL_WIDTH,.
-00000460: 2020 2020 5641 4c55 455f 4649 5253 545f      VALUE_FIRST_
-00000470: 504f 494e 542c 0a20 2020 2046 4f4c 4449  POINT,.    FOLDI
-00000480: 4e47 2c0a 2020 2020 4142 534f 4c55 5445  NG,.    ABSOLUTE
-00000490: 5f50 4541 4b5f 504f 5349 5449 4f4e 532c  _PEAK_POSITIONS,
-000004a0: 0a20 2020 2049 535f 4143 5155 4953 4954  .    IS_ACQUISIT
-000004b0: 494f 4e2c 0a29 0a0a 4449 4d45 4e53 494f  ION,.)..DIMENSIO
-000004c0: 4e5f 494e 4445 5820 3d20 2264 696d 656e  N_INDEX = "dimen
-000004d0: 7369 6f6e 5f69 6e64 6578 220a 4449 4d45  sion_index".DIME
-000004e0: 4e53 494f 4e5f 5f44 494d 454e 5349 4f4e  NSION__DIMENSION
-000004f0: 5f49 4e44 4558 203d 2022 6469 6d65 6e73  _INDEX = "dimens
-00000500: 696f 6e5f 7b64 696d 656e 7369 6f6e 5f69  ion_{dimension_i
-00000510: 6e64 6578 7d22 0a54 5241 4e53 4645 525f  ndex}".TRANSFER_
-00000520: 5459 5045 203d 2022 7472 616e 7366 6572  TYPE = "transfer
-00000530: 5f74 7970 6522 0a49 535f 494e 4449 5245  _type".IS_INDIRE
-00000540: 4354 203d 2022 6973 5f69 6e64 6972 6563  CT = "is_indirec
-00000550: 7422 0a0a 4f4e 455f 424f 4e44 203d 2022  t"..ONE_BOND = "
-00000560: 6f6e 6562 6f6e 6422 0a4e 4546 5f50 504d  onebond".NEF_PPM
-00000570: 203d 2022 7070 6d22 0a0a 5452 414e 5346   = "ppm"..TRANSF
-00000580: 4552 5f4c 4f4f 505f 5441 4753 203d 205b  ER_LOOP_TAGS = [
-00000590: 0a20 2020 2023 206d 616e 6461 746f 7279  .    # mandatory
-000005a0: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
-000005b0: 4449 4d45 4e53 494f 4e5f 5f44 494d 454e  DIMENSION__DIMEN
-000005c0: 5349 4f4e 5f49 4e44 4558 2c0a 2020 2020  SION_INDEX,.    
-000005d0: 5452 414e 5346 4552 5f54 5950 452c 0a20  TRANSFER_TYPE,. 
-000005e0: 2020 2023 206f 7074 696f 6e61 6c20 7061     # optional pa
-000005f0: 7261 6d65 7465 720a 2020 2020 4953 5f49  rameter.    IS_I
-00000600: 4e44 4952 4543 542c 0a5d 0a0a 4348 4149  NDIRECT,.]..CHAI
-00000610: 4e5f 434f 4445 203d 2022 6368 6169 6e5f  N_CODE = "chain_
-00000620: 636f 6465 220a 5345 5155 454e 4345 5f43  code".SEQUENCE_C
-00000630: 4f44 4520 3d20 2273 6571 7565 6e63 655f  ODE = "sequence_
-00000640: 636f 6465 220a 5245 5349 4455 455f 4e41  code".RESIDUE_NA
-00000650: 4d45 203d 2022 7265 7369 6475 655f 6e61  ME = "residue_na
-00000660: 6d65 220a 4154 4f4d 5f4e 414d 4520 3d20  me".ATOM_NAME = 
-00000670: 2261 746f 6d5f 6e61 6d65 220a 504f 5349  "atom_name".POSI
-00000680: 5449 4f4e 203d 2022 706f 7369 7469 6f6e  TION = "position
-00000690: 220a 504f 5349 5449 4f4e 5f55 4e43 4552  ".POSITION_UNCER
-000006a0: 5441 494e 5459 203d 2022 706f 7369 7469  TAINTY = "positi
-000006b0: 6f6e 5f75 6e63 6572 7461 696e 7479 220a  on_uncertainty".
-000006c0: 0a43 4841 494e 5f43 4f44 455f 5f44 494d  .CHAIN_CODE__DIM
-000006d0: 454e 5349 4f4e 5f49 4e44 4558 203d 2066  ENSION_INDEX = f
-000006e0: 227b 4348 4149 4e5f 434f 4445 7d5f 7b7b  "{CHAIN_CODE}_{{
-000006f0: 6469 6d65 6e73 696f 6e5f 696e 6465 787d  dimension_index}
-00000700: 7d22 0a53 4551 5545 4e43 455f 434f 4445  }".SEQUENCE_CODE
-00000710: 5f5f 4449 4d45 4e53 494f 4e5f 494e 4445  __DIMENSION_INDE
-00000720: 5820 3d20 6622 7b53 4551 5545 4e43 455f  X = f"{SEQUENCE_
-00000730: 434f 4445 7d5f 7b7b 6469 6d65 6e73 696f  CODE}_{{dimensio
-00000740: 6e5f 696e 6465 787d 7d22 0a52 4553 4944  n_index}}".RESID
-00000750: 5545 5f4e 414d 455f 5f44 494d 454e 5349  UE_NAME__DIMENSI
-00000760: 4f4e 5f49 4e44 4558 203d 2066 227b 5245  ON_INDEX = f"{RE
-00000770: 5349 4455 455f 4e41 4d45 7d5f 7b7b 6469  SIDUE_NAME}_{{di
-00000780: 6d65 6e73 696f 6e5f 696e 6465 787d 7d22  mension_index}}"
-00000790: 0a41 544f 4d5f 4e41 4d45 5f5f 4449 4d45  .ATOM_NAME__DIME
-000007a0: 4e53 494f 4e5f 494e 4445 5820 3d20 6622  NSION_INDEX = f"
-000007b0: 7b41 544f 4d5f 4e41 4d45 7d5f 7b7b 6469  {ATOM_NAME}_{{di
-000007c0: 6d65 6e73 696f 6e5f 696e 6465 787d 7d22  mension_index}}"
-000007d0: 0a50 4f53 4954 494f 4e5f 5f44 494d 454e  .POSITION__DIMEN
-000007e0: 5349 4f4e 5f49 4e44 4558 203d 2066 227b  SION_INDEX = f"{
-000007f0: 504f 5349 5449 4f4e 7d5f 7b7b 6469 6d65  POSITION}_{{dime
-00000800: 6e73 696f 6e5f 696e 6465 787d 7d22 0a50  nsion_index}}".P
-00000810: 4f53 4954 494f 4e5f 554e 4345 5254 4149  OSITION_UNCERTAI
-00000820: 4e54 595f 5f44 494d 454e 5349 4f4e 5f49  NTY__DIMENSION_I
-00000830: 4e44 4558 203d 2066 227b 504f 5349 5449  NDEX = f"{POSITI
-00000840: 4f4e 5f55 4e43 4552 5441 494e 5459 7d5f  ON_UNCERTAINTY}_
-00000850: 7b7b 6469 6d65 6e73 696f 6e5f 696e 6465  {{dimension_inde
-00000860: 787d 7d22 0a0a 0a50 4541 4b5f 4944 203d  x}}"...PEAK_ID =
-00000870: 2022 7065 616b 5f69 6422 0a49 4e44 4558   "peak_id".INDEX
-00000880: 203d 2022 696e 6465 7822 0a0a 4845 4947   = "index"..HEIG
-00000890: 4854 203d 2022 6865 6967 6874 220a 4845  HT = "height".HE
-000008a0: 4947 4854 5f55 4e43 4552 5441 494e 5459  IGHT_UNCERTAINTY
-000008b0: 203d 2022 6865 6967 6874 5f75 6e63 6572   = "height_uncer
-000008c0: 7461 696e 7479 220a 564f 4c55 4d45 203d  tainty".VOLUME =
-000008d0: 2022 766f 6c75 6d65 220a 564f 4c55 4d45   "volume".VOLUME
-000008e0: 5f55 4e43 4552 5441 494e 5459 203d 2022  _UNCERTAINTY = "
-000008f0: 766f 6c75 6d65 5f75 6e63 6572 7461 696e  volume_uncertain
-00000900: 7479 220a 0a50 4541 4b5f 4c4f 4f50 5f54  ty"..PEAK_LOOP_T
-00000910: 4147 5320 3d20 5b0a 2020 2020 494e 4445  AGS = [.    INDE
-00000920: 582c 0a20 2020 2050 4541 4b5f 4944 2c0a  X,.    PEAK_ID,.
-00000930: 2020 2020 4348 4149 4e5f 434f 4445 5f5f      CHAIN_CODE__
-00000940: 4449 4d45 4e53 494f 4e5f 494e 4445 582c  DIMENSION_INDEX,
-00000950: 0a20 2020 2053 4551 5545 4e43 455f 434f  .    SEQUENCE_CO
-00000960: 4445 5f5f 4449 4d45 4e53 494f 4e5f 494e  DE__DIMENSION_IN
-00000970: 4445 582c 0a20 2020 2052 4553 4944 5545  DEX,.    RESIDUE
-00000980: 5f4e 414d 455f 5f44 494d 454e 5349 4f4e  _NAME__DIMENSION
-00000990: 5f49 4e44 4558 2c0a 2020 2020 4154 4f4d  _INDEX,.    ATOM
-000009a0: 5f4e 414d 455f 5f44 494d 454e 5349 4f4e  _NAME__DIMENSION
-000009b0: 5f49 4e44 4558 2c0a 2020 2020 504f 5349  _INDEX,.    POSI
-000009c0: 5449 4f4e 5f5f 4449 4d45 4e53 494f 4e5f  TION__DIMENSION_
-000009d0: 494e 4445 582c 0a20 2020 2050 4f53 4954  INDEX,.    POSIT
-000009e0: 494f 4e5f 554e 4345 5254 4149 4e54 595f  ION_UNCERTAINTY_
-000009f0: 5f44 494d 454e 5349 4f4e 5f49 4e44 4558  _DIMENSION_INDEX
-00000a00: 2c0a 2020 2020 4845 4947 4854 2c0a 2020  ,.    HEIGHT,.  
-00000a10: 2020 4845 4947 4854 5f55 4e43 4552 5441    HEIGHT_UNCERTA
-00000a20: 494e 5459 2c0a 2020 2020 564f 4c55 4d45  INTY,.    VOLUME
-00000a30: 2c0a 2020 2020 564f 4c55 4d45 5f55 4e43  ,.    VOLUME_UNC
-00000a40: 4552 5441 494e 5459 2c0a 5d0a            ERTAINTY,.].
+00000000: 4e45 4620 3d20 226e 6566 220a 5346 203d  NEF = "nef".SF =
+00000010: 2022 7366 220a 0a53 4849 4654 5f4c 4953   "sf"..SHIFT_LIS
+00000020: 545f 4652 414d 455f 4341 5445 474f 5259  T_FRAME_CATEGORY
+00000030: 203d 2066 227b 4e45 467d 5f63 6865 6d69   = f"{NEF}_chemi
+00000040: 6361 6c5f 7368 6966 745f 6c69 7374 220a  cal_shift_list".
+00000050: 0a53 5045 4354 5255 4d5f 4652 414d 455f  .SPECTRUM_FRAME_
+00000060: 4341 5445 474f 5259 203d 2066 227b 4e45  CATEGORY = f"{NE
+00000070: 467d 5f6e 6d72 5f73 7065 6374 7275 6d22  F}_nmr_spectrum"
+00000080: 0a53 5045 4354 5255 4d5f 4449 4d45 4e53  .SPECTRUM_DIMENS
+00000090: 494f 4e5f 4c4f 4f50 5f43 4154 4547 4f52  ION_LOOP_CATEGOR
+000000a0: 5920 3d20 6622 7b4e 4546 7d5f 7370 6563  Y = f"{NEF}_spec
+000000b0: 7472 756d 5f64 696d 656e 7369 6f6e 220a  trum_dimension".
+000000c0: 5350 4543 5452 554d 5f44 494d 454e 5349  SPECTRUM_DIMENSI
+000000d0: 4f4e 5f54 5241 4e53 4645 525f 4c4f 4f50  ON_TRANSFER_LOOP
+000000e0: 5f43 4154 4547 4f52 5920 3d20 280a 2020  _CATEGORY = (.  
+000000f0: 2020 6622 7b53 5045 4354 5255 4d5f 4449    f"{SPECTRUM_DI
+00000100: 4d45 4e53 494f 4e5f 4c4f 4f50 5f43 4154  MENSION_LOOP_CAT
+00000110: 4547 4f52 597d 5f74 7261 6e73 6665 7222  EGORY}_transfer"
+00000120: 0a29 0a53 5045 4354 5255 4d5f 5045 414b  .).SPECTRUM_PEAK
+00000130: 5f4c 4f4f 505f 4341 5445 474f 5259 203d  _LOOP_CATEGORY =
+00000140: 2066 227b 4e45 467d 5f70 6561 6b22 0a0a   f"{NEF}_peak"..
+00000150: 5346 5f43 4154 4547 4f52 5920 3d20 6622  SF_CATEGORY = f"
+00000160: 7b53 467d 5f63 6174 6567 6f72 7922 0a53  {SF}_category".S
+00000170: 465f 4652 414d 4543 4f44 4520 3d20 6622  F_FRAMECODE = f"
+00000180: 7b53 467d 5f66 7261 6d65 636f 6465 220a  {SF}_framecode".
+00000190: 4e55 4d5f 4449 4d45 4e53 494f 4e53 203d  NUM_DIMENSIONS =
+000001a0: 2022 6e75 6d5f 6469 6d65 6e73 696f 6e73   "num_dimensions
+000001b0: 220a 4348 454d 4943 414c 5f53 4849 4654  ".CHEMICAL_SHIFT
+000001c0: 5f4c 4953 5420 3d20 2263 6865 6d69 6361  _LIST = "chemica
+000001d0: 6c5f 7368 6966 745f 6c69 7374 220a 4558  l_shift_list".EX
+000001e0: 5045 5249 4d45 4e54 5f54 5950 4520 3d20  PERIMENT_TYPE = 
+000001f0: 2265 7870 6572 696d 656e 745f 7479 7065  "experiment_type
+00000200: 220a 4558 5045 5249 4d45 4e54 5f43 4c41  ".EXPERIMENT_CLA
+00000210: 5353 4946 4943 4154 494f 4e20 3d20 2265  SSIFICATION = "e
+00000220: 7870 6572 696d 656e 745f 636c 6173 7369  xperiment_classi
+00000230: 6669 6361 7469 6f6e 220a 0a53 5045 4354  fication"..SPECT
+00000240: 5255 4d5f 4652 414d 455f 5441 4753 203d  RUM_FRAME_TAGS =
+00000250: 2028 0a20 2020 2053 465f 4341 5445 474f   (.    SF_CATEGO
+00000260: 5259 2c0a 2020 2020 5346 5f46 5241 4d45  RY,.    SF_FRAME
+00000270: 434f 4445 2c0a 2020 2020 4e55 4d5f 4449  CODE,.    NUM_DI
+00000280: 4d45 4e53 494f 4e53 2c0a 2020 2020 4348  MENSIONS,.    CH
+00000290: 454d 4943 414c 5f53 4849 4654 5f4c 4953  EMICAL_SHIFT_LIS
+000002a0: 542c 0a20 2020 2045 5850 4552 494d 454e  T,.    EXPERIMEN
+000002b0: 545f 434c 4153 5349 4649 4341 5449 4f4e  T_CLASSIFICATION
+000002c0: 2c0a 2020 2020 4558 5045 5249 4d45 4e54  ,.    EXPERIMENT
+000002d0: 5f54 5950 452c 0a29 0a0a 4449 4d45 4e53  _TYPE,.)..DIMENS
+000002e0: 494f 4e5f 4944 203d 2022 6469 6d65 6e73  ION_ID = "dimens
+000002f0: 696f 6e5f 6964 220a 4158 4953 5f55 4e49  ion_id".AXIS_UNI
+00000300: 5420 3d20 2261 7869 735f 756e 6974 220a  T = "axis_unit".
+00000310: 4158 4953 5f43 4f44 4520 3d20 2261 7869  AXIS_CODE = "axi
+00000320: 735f 636f 6465 220a 0a53 5045 4354 524f  s_code"..SPECTRO
+00000330: 4d45 5445 525f 4652 4551 5545 4e43 5920  METER_FREQUENCY 
+00000340: 3d20 2273 7065 6374 726f 6d65 7465 725f  = "spectrometer_
+00000350: 6672 6571 7565 6e63 7922 0a53 5045 4354  frequency".SPECT
+00000360: 5241 4c5f 5749 4454 4820 3d20 2273 7065  RAL_WIDTH = "spe
+00000370: 6374 7261 6c5f 7769 6474 6822 0a56 414c  ctral_width".VAL
+00000380: 5545 5f46 4952 5354 5f50 4f49 4e54 203d  UE_FIRST_POINT =
+00000390: 2022 7661 6c75 655f 6669 7273 745f 706f   "value_first_po
+000003a0: 696e 7422 0a46 4f4c 4449 4e47 203d 2022  int".FOLDING = "
+000003b0: 666f 6c64 696e 6722 0a41 4253 4f4c 5554  folding".ABSOLUT
+000003c0: 455f 5045 414b 5f50 4f53 4954 494f 4e53  E_PEAK_POSITIONS
+000003d0: 203d 2022 6162 736f 6c75 7465 5f70 6561   = "absolute_pea
+000003e0: 6b5f 706f 7369 7469 6f6e 7322 0a49 535f  k_positions".IS_
+000003f0: 4143 5155 4953 4954 494f 4e20 3d20 2269  ACQUISITION = "i
+00000400: 735f 6163 7175 6973 6974 696f 6e22 0a0a  s_acquisition"..
+00000410: 0a44 494d 454e 5349 4f4e 5f4c 4f4f 505f  .DIMENSION_LOOP_
+00000420: 5441 4753 203d 2028 0a20 2020 2023 206d  TAGS = (.    # m
+00000430: 616e 6461 746f 7279 2070 6172 616d 6574  andatory paramet
+00000440: 6572 730a 2020 2020 4449 4d45 4e53 494f  ers.    DIMENSIO
+00000450: 4e5f 4944 2c0a 2020 2020 4158 4953 5f55  N_ID,.    AXIS_U
+00000460: 4e49 542c 0a20 2020 2041 5849 535f 434f  NIT,.    AXIS_CO
+00000470: 4445 2c0a 2020 2020 2320 2320 6f70 7469  DE,.    # # opti
+00000480: 6f6e 616c 2070 6172 616d 6574 6572 730a  onal parameters.
+00000490: 2020 2020 5350 4543 5452 4f4d 4554 4552      SPECTROMETER
+000004a0: 5f46 5245 5155 454e 4359 2c0a 2020 2020  _FREQUENCY,.    
+000004b0: 5350 4543 5452 414c 5f57 4944 5448 2c0a  SPECTRAL_WIDTH,.
+000004c0: 2020 2020 5641 4c55 455f 4649 5253 545f      VALUE_FIRST_
+000004d0: 504f 494e 542c 0a20 2020 2046 4f4c 4449  POINT,.    FOLDI
+000004e0: 4e47 2c0a 2020 2020 4142 534f 4c55 5445  NG,.    ABSOLUTE
+000004f0: 5f50 4541 4b5f 504f 5349 5449 4f4e 532c  _PEAK_POSITIONS,
+00000500: 0a20 2020 2049 535f 4143 5155 4953 4954  .    IS_ACQUISIT
+00000510: 494f 4e2c 0a29 0a0a 4449 4d45 4e53 494f  ION,.)..DIMENSIO
+00000520: 4e5f 494e 4445 5820 3d20 2264 696d 656e  N_INDEX = "dimen
+00000530: 7369 6f6e 5f69 6e64 6578 220a 4449 4d45  sion_index".DIME
+00000540: 4e53 494f 4e5f 5f44 494d 454e 5349 4f4e  NSION__DIMENSION
+00000550: 5f49 4e44 4558 203d 2022 6469 6d65 6e73  _INDEX = "dimens
+00000560: 696f 6e5f 7b64 696d 656e 7369 6f6e 5f69  ion_{dimension_i
+00000570: 6e64 6578 7d22 0a54 5241 4e53 4645 525f  ndex}".TRANSFER_
+00000580: 5459 5045 203d 2022 7472 616e 7366 6572  TYPE = "transfer
+00000590: 5f74 7970 6522 0a49 535f 494e 4449 5245  _type".IS_INDIRE
+000005a0: 4354 203d 2022 6973 5f69 6e64 6972 6563  CT = "is_indirec
+000005b0: 7422 0a0a 4f4e 455f 424f 4e44 203d 2022  t"..ONE_BOND = "
+000005c0: 6f6e 6562 6f6e 6422 0a4e 4546 5f50 504d  onebond".NEF_PPM
+000005d0: 203d 2022 7070 6d22 0a0a 5452 414e 5346   = "ppm"..TRANSF
+000005e0: 4552 5f4c 4f4f 505f 5441 4753 203d 205b  ER_LOOP_TAGS = [
+000005f0: 0a20 2020 2023 206d 616e 6461 746f 7279  .    # mandatory
+00000600: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
+00000610: 4449 4d45 4e53 494f 4e5f 5f44 494d 454e  DIMENSION__DIMEN
+00000620: 5349 4f4e 5f49 4e44 4558 2c0a 2020 2020  SION_INDEX,.    
+00000630: 5452 414e 5346 4552 5f54 5950 452c 0a20  TRANSFER_TYPE,. 
+00000640: 2020 2023 206f 7074 696f 6e61 6c20 7061     # optional pa
+00000650: 7261 6d65 7465 720a 2020 2020 4953 5f49  rameter.    IS_I
+00000660: 4e44 4952 4543 542c 0a5d 0a0a 4348 4149  NDIRECT,.]..CHAI
+00000670: 4e5f 434f 4445 203d 2022 6368 6169 6e5f  N_CODE = "chain_
+00000680: 636f 6465 220a 5345 5155 454e 4345 5f43  code".SEQUENCE_C
+00000690: 4f44 4520 3d20 2273 6571 7565 6e63 655f  ODE = "sequence_
+000006a0: 636f 6465 220a 5245 5349 4455 455f 4e41  code".RESIDUE_NA
+000006b0: 4d45 203d 2022 7265 7369 6475 655f 6e61  ME = "residue_na
+000006c0: 6d65 220a 4154 4f4d 5f4e 414d 4520 3d20  me".ATOM_NAME = 
+000006d0: 2261 746f 6d5f 6e61 6d65 220a 504f 5349  "atom_name".POSI
+000006e0: 5449 4f4e 203d 2022 706f 7369 7469 6f6e  TION = "position
+000006f0: 220a 504f 5349 5449 4f4e 5f55 4e43 4552  ".POSITION_UNCER
+00000700: 5441 494e 5459 203d 2022 706f 7369 7469  TAINTY = "positi
+00000710: 6f6e 5f75 6e63 6572 7461 696e 7479 220a  on_uncertainty".
+00000720: 0a43 4841 494e 5f43 4f44 455f 5f44 494d  .CHAIN_CODE__DIM
+00000730: 454e 5349 4f4e 5f49 4e44 4558 203d 2066  ENSION_INDEX = f
+00000740: 227b 4348 4149 4e5f 434f 4445 7d5f 7b7b  "{CHAIN_CODE}_{{
+00000750: 6469 6d65 6e73 696f 6e5f 696e 6465 787d  dimension_index}
+00000760: 7d22 0a53 4551 5545 4e43 455f 434f 4445  }".SEQUENCE_CODE
+00000770: 5f5f 4449 4d45 4e53 494f 4e5f 494e 4445  __DIMENSION_INDE
+00000780: 5820 3d20 6622 7b53 4551 5545 4e43 455f  X = f"{SEQUENCE_
+00000790: 434f 4445 7d5f 7b7b 6469 6d65 6e73 696f  CODE}_{{dimensio
+000007a0: 6e5f 696e 6465 787d 7d22 0a52 4553 4944  n_index}}".RESID
+000007b0: 5545 5f4e 414d 455f 5f44 494d 454e 5349  UE_NAME__DIMENSI
+000007c0: 4f4e 5f49 4e44 4558 203d 2066 227b 5245  ON_INDEX = f"{RE
+000007d0: 5349 4455 455f 4e41 4d45 7d5f 7b7b 6469  SIDUE_NAME}_{{di
+000007e0: 6d65 6e73 696f 6e5f 696e 6465 787d 7d22  mension_index}}"
+000007f0: 0a41 544f 4d5f 4e41 4d45 5f5f 4449 4d45  .ATOM_NAME__DIME
+00000800: 4e53 494f 4e5f 494e 4445 5820 3d20 6622  NSION_INDEX = f"
+00000810: 7b41 544f 4d5f 4e41 4d45 7d5f 7b7b 6469  {ATOM_NAME}_{{di
+00000820: 6d65 6e73 696f 6e5f 696e 6465 787d 7d22  mension_index}}"
+00000830: 0a50 4f53 4954 494f 4e5f 5f44 494d 454e  .POSITION__DIMEN
+00000840: 5349 4f4e 5f49 4e44 4558 203d 2066 227b  SION_INDEX = f"{
+00000850: 504f 5349 5449 4f4e 7d5f 7b7b 6469 6d65  POSITION}_{{dime
+00000860: 6e73 696f 6e5f 696e 6465 787d 7d22 0a50  nsion_index}}".P
+00000870: 4f53 4954 494f 4e5f 554e 4345 5254 4149  OSITION_UNCERTAI
+00000880: 4e54 595f 5f44 494d 454e 5349 4f4e 5f49  NTY__DIMENSION_I
+00000890: 4e44 4558 203d 2066 227b 504f 5349 5449  NDEX = f"{POSITI
+000008a0: 4f4e 5f55 4e43 4552 5441 494e 5459 7d5f  ON_UNCERTAINTY}_
+000008b0: 7b7b 6469 6d65 6e73 696f 6e5f 696e 6465  {{dimension_inde
+000008c0: 787d 7d22 0a0a 0a50 4541 4b5f 4944 203d  x}}"...PEAK_ID =
+000008d0: 2022 7065 616b 5f69 6422 0a49 4e44 4558   "peak_id".INDEX
+000008e0: 203d 2022 696e 6465 7822 0a0a 4845 4947   = "index"..HEIG
+000008f0: 4854 203d 2022 6865 6967 6874 220a 4845  HT = "height".HE
+00000900: 4947 4854 5f55 4e43 4552 5441 494e 5459  IGHT_UNCERTAINTY
+00000910: 203d 2022 6865 6967 6874 5f75 6e63 6572   = "height_uncer
+00000920: 7461 696e 7479 220a 564f 4c55 4d45 203d  tainty".VOLUME =
+00000930: 2022 766f 6c75 6d65 220a 564f 4c55 4d45   "volume".VOLUME
+00000940: 5f55 4e43 4552 5441 494e 5459 203d 2022  _UNCERTAINTY = "
+00000950: 766f 6c75 6d65 5f75 6e63 6572 7461 696e  volume_uncertain
+00000960: 7479 220a 0a50 4541 4b5f 4c4f 4f50 5f54  ty"..PEAK_LOOP_T
+00000970: 4147 5320 3d20 5b0a 2020 2020 494e 4445  AGS = [.    INDE
+00000980: 582c 0a20 2020 2050 4541 4b5f 4944 2c0a  X,.    PEAK_ID,.
+00000990: 2020 2020 5b0a 2020 2020 2020 2020 4348      [.        CH
+000009a0: 4149 4e5f 434f 4445 5f5f 4449 4d45 4e53  AIN_CODE__DIMENS
+000009b0: 494f 4e5f 494e 4445 582c 0a20 2020 2020  ION_INDEX,.     
+000009c0: 2020 2053 4551 5545 4e43 455f 434f 4445     SEQUENCE_CODE
+000009d0: 5f5f 4449 4d45 4e53 494f 4e5f 494e 4445  __DIMENSION_INDE
+000009e0: 582c 0a20 2020 2020 2020 2052 4553 4944  X,.        RESID
+000009f0: 5545 5f4e 414d 455f 5f44 494d 454e 5349  UE_NAME__DIMENSI
+00000a00: 4f4e 5f49 4e44 4558 2c0a 2020 2020 2020  ON_INDEX,.      
+00000a10: 2020 4154 4f4d 5f4e 414d 455f 5f44 494d    ATOM_NAME__DIM
+00000a20: 454e 5349 4f4e 5f49 4e44 4558 2c0a 2020  ENSION_INDEX,.  
+00000a30: 2020 5d2c 0a20 2020 205b 0a20 2020 2020    ],.    [.     
+00000a40: 2020 2050 4f53 4954 494f 4e5f 5f44 494d     POSITION__DIM
+00000a50: 454e 5349 4f4e 5f49 4e44 4558 2c0a 2020  ENSION_INDEX,.  
+00000a60: 2020 2020 2020 504f 5349 5449 4f4e 5f55        POSITION_U
+00000a70: 4e43 4552 5441 494e 5459 5f5f 4449 4d45  NCERTAINTY__DIME
+00000a80: 4e53 494f 4e5f 494e 4445 582c 0a20 2020  NSION_INDEX,.   
+00000a90: 205d 2c0a 2020 2020 4845 4947 4854 2c0a   ],.    HEIGHT,.
+00000aa0: 2020 2020 4845 4947 4854 5f55 4e43 4552      HEIGHT_UNCER
+00000ab0: 5441 494e 5459 2c0a 2020 2020 564f 4c55  TAINTY,.    VOLU
+00000ac0: 4d45 2c0a 2020 2020 564f 4c55 4d45 5f55  ME,.    VOLUME_U
+00000ad0: 4e43 4552 5441 494e 5459 2c0a 5d0a       NCERTAINTY,.].
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/nef_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,17 +342,20 @@
     star_filters = [f"*{filter}*" for filter in filters]
     filters = list(filters)
     filters.extend(star_filters)
 
     result = {}
     for frame in entry.frame_dict.values():
 
-        accept_frame_category = any(
-            [fnmatch(frame.category, filter) for filter in filters]
-        )
+        if frame.category is not None:
+            accept_frame_category = any(
+                [fnmatch(frame.category, filter) for filter in filters]
+            )
+        else:
+            accept_frame_category = False
         accept_frame_name = any([fnmatch(frame.name, filter) for filter in filters])
 
         if (
             selector_type in (SelectionType.NAME, SelectionType.ANY)
             and accept_frame_name
         ):
             result[frame.category, frame.name] = frame
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/peak_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import copy
 from textwrap import dedent
 from typing import Any, Dict, List, Tuple, Union
 
+from frozendict import frozendict
+from ordered_set import OrderedSet
 from pynmrstar import Loop, Saveframe
 
 from nef_pipelines.lib.isotope_lib import GAMMA_RATIOS, Isotope
 from nef_pipelines.lib.nef_frames_lib import (
     ABSOLUTE_PEAK_POSITIONS,
     ATOM_NAME,
     ATOM_NAME__DIMENSION_INDEX,
@@ -135,53 +137,67 @@
     :param value: an int of a float
     :return: a formatted string
     """
     return f"{value:7.3f}".strip()
 
 
 def _expand_templates(
-    templates: List[str], values_list: List[Dict[str, Any]]
+    template: List[Union[str, List[str]]], values_list: List[Dict[str, Any]]
 ) -> List[str]:
     """
     expand a list of templates into strings using a list of sets (dicts) of values
     :param templates: the tags to format
     :param values_list: a list of dictionaries of values
     :return: a list of formatted strings
     """
-    result = set()
-    for tag in templates:
-        for values in values_list:
-            result.add(tag.format(**values))
+    result = OrderedSet()
+    for tag_or_tag_list in template:
+        if isinstance(tag_or_tag_list, str):
+            for values in values_list:
+                result.add(tag_or_tag_list.format(**values))
+        elif isinstance(tag_or_tag_list, list):
+            for values in values_list:
+                for tag in tag_or_tag_list:
+                    result.add(tag.format(**values))
 
     return list(result)
 
 
+DEFAULT_EXTRA_TAGS = {
+    CHEMICAL_SHIFT_LIST: UNUSED,
+    EXPERIMENT_CLASSIFICATION: UNUSED,
+    EXPERIMENT_TYPE: UNUSED,
+}
+
+
 def peaks_to_frame(
     peaks: List[NewPeak],
     dimensions: List[DimensionInfo],
     spectrometer_frequency: float,
-    frame_code="peaks",
-    shift_list_name=UNUSED,
-    source="unknown",
+    frame_code: str = "peaks",
+    extra_tags: Dict[str, str] = frozendict(DEFAULT_EXTRA_TAGS),
+    source: str = "unknown",
 ) -> Saveframe:
 
     # TODO needs a list of transfers
     """
     convert a list of peaks to a nef spectrum frame
     :param peaks: the peaks
     :param dimensions: the dimensions of the peak list
     :param spectrometer_frequency: the 1H spectrometer frequency of the peak list
     :param frame_code: the name for the frame
-    :param shift_list_name: the name of the companion shift list frame, note the default results in
-                            a non-conforming NEF file, howvever we allowno conforming files as we buil up
-                            nef files in pieces
+    :param extra_tags: extra tags to be used in the frame, non nef tags will be appended
     :param source: the source of the data for error reporting
     :return: a NEF Spectrum save frame
     """
 
+    mutable_extra_tags = {**DEFAULT_EXTRA_TAGS}
+    mutable_extra_tags.update(extra_tags)
+    extra_tags = mutable_extra_tags
+
     frame_code = f"{SPECTRUM_FRAME_CATEGORY}_{frame_code}"
 
     frame = Saveframe.from_scratch(frame_code, SPECTRUM_FRAME_CATEGORY)
 
     frame.add_tag(SF_CATEGORY, SPECTRUM_FRAME_CATEGORY)
     frame.add_tag(SF_FRAMECODE, frame_code)
 
@@ -196,24 +212,37 @@
         msg = f"""\
             unexpected! in the file {source} there are peaks with different numbers of different dimensions
             the dimensions were: {' '.join([str(dimension) for dimension in peak_dimensions])}
         """
         exit_error(msg)
 
     frame.add_tag(NUM_DIMENSIONS, peak_dimensions[0])
+
+    shift_list_name = (
+        extra_tags[CHEMICAL_SHIFT_LIST] if CHEMICAL_SHIFT_LIST in extra_tags else UNUSED
+    )
     frame.add_tag(
         CHEMICAL_SHIFT_LIST, shift_list_name
-    )  # technically not correct but this is a nef file building
+    )  # technically not correct to use unused bye default here but this is a nef file building
     # tool kit so an empty shift list maybe what we need
-    # we may need to add a flag to build the shift list
+    # we may need to add a flag to build the shift list on the fly at a later date...
 
+    experiment_classification = (
+        extra_tags[EXPERIMENT_CLASSIFICATION]
+        if EXPERIMENT_CLASSIFICATION in extra_tags
+        else UNUSED
+    )
     frame.add_tag(
-        EXPERIMENT_CLASSIFICATION, UNUSED
-    )  # add via an experiment info structure?
-    frame.add_tag(EXPERIMENT_TYPE, UNUSED)
+        EXPERIMENT_CLASSIFICATION, experiment_classification
+    )  # add via an experiment info structure currently uses extra tags?
+
+    experiment_type = (
+        extra_tags[EXPERIMENT_TYPE] if EXPERIMENT_TYPE in extra_tags else UNUSED
+    )
+    frame.add_tag(EXPERIMENT_TYPE, experiment_type)
 
     dimension_loop = Loop.from_scratch(SPECTRUM_DIMENSION_LOOP_CATEGORY)
     frame.add_loop(dimension_loop)
 
     dimension_loop.add_tag(DIMENSION_LOOP_TAGS)
 
     dimensions = copy.deepcopy(dimensions)
@@ -277,19 +306,14 @@
         )
 
     peak_loop = Loop.from_scratch(SPECTRUM_PEAK_LOOP_CATEGORY)
     frame.add_loop(peak_loop)
 
     peak_loop_tags = _expand_templates(PEAK_LOOP_TAGS, dimension_indices)
 
-    # for dim_index in range(1,len(dimensions)+1):
-    #     for template_string in peak_loop_tag_templates:
-    #         template = FStringTemplate(template_string)
-    #         peak_loop_tags.append(str(template))
-
     peak_loop.add_tag(peak_loop_tags)
 
     for index, peak in enumerate(peaks):
         peak_data = {
             INDEX: index,
             PEAK_ID: index,
             HEIGHT: peak.height,
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/structures.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.34/src/nef_pipelines/lib/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import inspect
 import io
 import os
 import sys
 import traceback
 from argparse import Namespace
 from enum import auto
+from math import floor
 from pathlib import Path
 from textwrap import dedent
 from typing import Any, Dict, Iterator, List, Optional, TextIO, TypeVar, Union
 
 import click
 from cacheable_iter import iter_cache
 from pynmrstar import Entry, Loop, Saveframe
@@ -25,14 +26,16 @@
 from nef_pipelines.lib.header_lib import (
     create_header_frame,
     get_creation_time,
     get_uuid,
 )
 from nef_pipelines.lib.structures import LineInfo
 
+FOUR_SPACES = " " * 4
+
 STDIN = Path("-")
 STDOUT = Path("-")
 
 
 def _get_loop_by_category_or_none(frame: Saveframe, category: str) -> Loop:
 
     result = None
@@ -409,17 +412,18 @@
     print(file=sys.stderr)
 
     script = script_name(__file__)
 
     command = _script_to_command(script)
 
     print(f"ERROR [in: {command}]: {msg[0]}", file=sys.stderr)
+    print(file=sys.stderr)
 
     for line in msg[1:]:
-        print(f"       {line}", file=sys.stderr)
+        print(f"  {line}", file=sys.stderr)
     print("exiting...", file=sys.stderr)
     sys.exit(EXIT_ERROR)
 
 
 def process_stream_and_add_frames(
     frames: List[Saveframe], input_args: Namespace
 ) -> Entry:
@@ -779,7 +783,64 @@
     values = [
         headers,
     ]
     for key, value in rows.items():
         values.append([key, value])
     value_string = tabulate(values, headers="firstrow")
     return value_string
+
+
+def strings_to_table_terminal_sensitive(
+    strings: str,
+    used_width: int = 0,
+    min_width: int = 20,
+    fallback_terminal_width: int = 100,
+):
+    """
+    given a list of strings convert them to a table where the number of columns os compatible with the terminal width
+    :param strings: a list of strings to tabulate
+    :param used_width: any width of the terminal already used
+    :param min_width: the minum width for a table column
+    :param fallback_terminal_width: if the terminal width can't be determined use this width
+    :return: a list of list where each sub list is a row, which is  suitable for formatting with tabulate.tabulate
+    """
+    try:
+        width, _ = os.get_terminal_size()
+    except Exception:
+        width = fallback_terminal_width
+
+    width -= used_width
+
+    # apply a sensible minimum width
+    if width < min_width:
+        width = min_width
+
+    if len(strings) > 0:
+        frame_name_widths = [len(frame_name) for frame_name in strings]
+        max_frame_name_width = max(frame_name_widths)
+
+        columns = int(floor(width / (max_frame_name_width + 1)))
+        column_width = int(floor(width / columns))
+
+        columns = 1 if columns == 0 else columns
+
+        strings = [frame_name.rjust(column_width) for frame_name in strings]
+        table_list = chunks(strings, columns)
+    else:
+        table_list = [
+            [],
+        ]
+
+    return list(table_list)
+
+
+def strings_to_tabulated_terminal_sensitive(
+    strings: str,
+    used_width: int = 0,
+    min_width: int = 20,
+    fallback_terminal_width: int = 100,
+):
+
+    table = strings_to_table_terminal_sensitive(
+        strings, used_width, min_width, fallback_terminal_width
+    )
+    return tabulate(table, tablefmt="plain")
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/main.py` & `nef_pipelines-0.1.34/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files 1% similar despite different names*

```diff
@@ -69,38 +69,37 @@
          _nef_chemical_shift.value_uncertainty
          _nef_chemical_shift.element
          _nef_chemical_shift.isotope_number
          _nef_chemical_shift.ccpn_figure_of_merit
          _nef_chemical_shift.ccpn_static
          _nef_chemical_shift.ccpn_comment
 
-         '#18'  @8      .  C    174.3804861  .                C  13  1  false  .
-         '#18'  @8      .  CA   56.48782652  .                C  13  1  false  .
-         '#18'  @8      .  CB   43.65587091  .                C  13  1  false  .
-         '#18'  @8      .  H    8.840075572  0.002464490125   H  1   1  false  .
-         '#18'  @8      .  N    124.8196102  0.01850293408    N  15  1  false  .
-         '#18'  @8-1    .  C    175.6031412  0.09064164946    C  13  1  false  .
-         '#18'  @8-1    .  CA   58.98480044  0.009964601556   C  13  1  false  .
-         '#18'  @8-1    .  CB   41.09278206  0.04550905905    C  13  1  false  .
-         '#18'  @10     .  C    175.8022086  .                C  13  1  false  .
-         '#18'  @10     .  CA   53.01487203  .                C  13  1  false  .
-         '#18'  @10     .  CB   45.72915971  .                C  13  1  false  .
-         '#18'  @10     .  H    8.798078008  0.0008574539324  H  1   1  false  .
-         '#18'  @10     .  N    124.5633376  0.03804289742    N  15  1  false  .
-         '#18'  @10-1   .  C    173.7316297  0.0928329695     C  13  1  false  .
-         '#18'  @10-1   .  CA   55.18115946  0.00191545255    C  13  1  false  .
-         '#18'  @10-1   .  CB   31.68450238  0.02225590709    C  13  1  false  .
          '#18'  @19     .  C    174.0787518  .                C  13  1  false  .
          '#18'  @19     .  CA   55.19626104  .                C  13  1  false  .
          '#18'  @19     .  CB   42.78262913  .                C  13  1  false  .
          '#18'  @19     .  H    8.507345563  0.003149388014   H  1   1  false  .
          '#18'  @19     .  N    123.3654109  0.1052522259     N  15  1  false  .
          '#18'  @19-1   .  C    175.947447   0.08720577414    C  13  1  false  .
          '#18'  @19-1   .  CA   56.6890552   0.0499432144     C  13  1  false  .
          '#18'  @19-1   .  CB   31.54304891  0.1003766534     C  13  1  false  .
+         @-     @9     .  C      177.0907867  .               C  13  1  false  .
+         @-     @9     .  CA     57.45044906  .               C  13  1  false  .
+         @-     @9     .  CB     40.259399    .               C  13  1  false  .
+         @-     @9     .  H      7.956588347  0.0027175082    H  1   1  false  .
+         @-     @9     .  N      124.7144569  0.1199761464    N  15  1  false  .
+         @-     @9-1   .  C      178.1212954  0.3397487528    C  13  1  false  .
+         @-     @9-1   .  CA     61.14832291  0.0266869088    C  13  1  false  .
+         @-     @9-1   .  CB     62.57084641  0.0514681685    C  13  1  false  .
+         A      10    Ala  H     8.11125646   0.0019229051    H  1  1  false   .
+         A      10    Ala  N     102.4535755  0.0925289285    N  15  1  false  .
+         A      10-1  Ala  C     177.2619806  0.0133395288    C  13  1  false  .
+         A      10-1  Ala  CA    52.49098528  0               C  13  1  false  .
+         A      10-1  Ala  CB    16.42772942  0.1141368283    C  13  1  false  .
+
+
       stop_
    save_
 
 
    save_nef_nmr_spectrum_k_ubi_n_hsqc`1`
 
       _nef_nmr_spectrum.sf_category                   nef_nmr_spectrum
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-from math import floor
 from pathlib import Path
 from textwrap import dedent
 from typing import List, Optional
 
 import typer
 from pynmrstar import Entry
 from tabulate import tabulate
@@ -11,15 +9,15 @@
 from nef_pipelines.lib.nef_lib import (
     SelectionType,
     read_or_create_entry_exit_error_on_bad_file,
     select_frames,
 )
 from nef_pipelines.lib.sequence_lib import count_residues, frame_to_chains
 from nef_pipelines.lib.typer_utils import get_args
-from nef_pipelines.lib.util import chunks, exit_error
+from nef_pipelines.lib.util import exit_error, strings_to_table_terminal_sensitive
 from nef_pipelines.tools.frames import frames_app
 
 UNDERSCORE = "_"
 
 parser = None
 
 
@@ -116,29 +114,29 @@
         frame_names = [frame.name for frame in frames]
         if number:
             frame_names = [
                 f"{i}. {frame_name}"
                 for i, frame_name in enumerate(frame_names, start=1)
             ]
 
-        frame_list = _string_list_to_tabulation(frame_names)
+        frame_list = strings_to_table_terminal_sensitive(frame_names)
         print(tabulate(frame_list, tablefmt="plain"))
 
     else:
 
         for frame in enumerate(frames, start=1):
 
             filters = [f"*{filter}*" for filter in filters]
 
             if verbose == 0:
                 frame_names = [
                     f"{i}. {frame.name}" for i, frame_name in enumerate(frames, start=1)
                 ]
 
-                frame_list = _string_list_to_tabulation(frame_names)
+                frame_list = strings_to_table_terminal_sensitive(frame_names)
                 print(tabulate(frame_list, tablefmt="plain"))
 
                 print(f"    category: {frame.category}")
                 if len(frame.name) != len(frame.category):
                     print(
                         f"    name: {frame.name[len(frame.category):].lstrip(UNDERSCORE)}"
                     )
@@ -191,15 +189,15 @@
                             counts_and_percentages.append(
                                 f"{residue}: {count} [{percentage}%]"
                             )
 
                         pre_string = f"              {chain}. "
                         pre_string_width = len(pre_string)
 
-                        tabulation = _string_list_to_tabulation(
+                        tabulation = strings_to_table_terminal_sensitive(
                             counts_and_percentages, pre_string_width
                         )
                         table = tabulate(tabulation, tablefmt="plain")
 
                         print(_indent_with_prestring(table, pre_string))
 
     print()
@@ -211,36 +209,7 @@
     for i, string in enumerate(text_block.split("\n")):
         if i == 0:
             raw_result.append(f"{pre_string}{string}")
         else:
             raw_result.append(f"{empty_prestring}{string}")
 
     return "\n".join(raw_result)
-
-
-def _string_list_to_tabulation(frame_names, used_columns=0):
-    try:
-        width, _ = os.get_terminal_size()
-    except Exception:
-        width = 100
-
-    width -= used_columns
-
-    # apply a sensible minimum width
-    if width < 20:
-        width = 20
-
-    if len(frame_names) > 0:
-        frame_name_widths = [len(frame_name) for frame_name in frame_names]
-        max_frame_name_width = max(frame_name_widths)
-
-        columns = int(floor(width / (max_frame_name_width + 1)))
-        column_width = int(floor(width / columns))
-
-        columns = 1 if columns == 0 else columns
-
-        frame_names = [frame_name.rjust(column_width) for frame_name in frame_names]
-        frame_name_list = chunks(frame_names, columns)
-    else:
-        frame_name_list = [[]]
-
-    return frame_name_list
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/rename.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,23 @@
 from tabulate import tabulate
 
 from nef_pipelines.lib.nef_lib import (
     read_entry_from_file_or_stdin_or_exit_error,
     select_frames_by_name,
 )
 from nef_pipelines.lib.util import (
+    FOUR_SPACES,
     STDIN,
     chunks,
     exit_error,
     parse_comma_separated_options,
     strings_to_table_terminal_sensitive,
 )
 from nef_pipelines.tools.frames import frames_app
 
-FOUR_SPACES = " " * 4
-
 # TODO: add mmv like semantics as an option [https://manpages.ubuntu.com/manpages/bionic/man1/mmv.1.html]
 
 
 @frames_app.command()
 def rename(
     input: Path = typer.Option(
         STDIN, "-i", "--in", help="sequence_text to read input from [- is stdin]"
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.34/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/pdbx/importers/sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.34/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.34/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef-pipelines
-Version: 0.1.33
+Version: 0.1.34
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.33/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.34/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 .idea/.gitignore
 .idea/.name
 .idea/NFC.iml
 .idea/modules.xml
 .idea/vcs.xml
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
+references/Nmr Experiment Nomenclature v2.docx
+references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
 src/nef_pipelines/VERSION
 src/nef_pipelines/__init__.py
 src/nef_pipelines/__main__.py
 src/nef_pipelines/main.py
 src/nef_pipelines.egg-info/PKG-INFO
 src/nef_pipelines.egg-info/SOURCES.txt
 src/nef_pipelines.egg-info/dependency_links.txt
@@ -37,14 +39,15 @@
 src/nef_pipelines/lib/header_lib.py
 src/nef_pipelines/lib/isotope_lib.py
 src/nef_pipelines/lib/nef_frames_lib.py
 src/nef_pipelines/lib/nef_lib.py
 src/nef_pipelines/lib/peak_lib.py
 src/nef_pipelines/lib/sequence_lib.py
 src/nef_pipelines/lib/shift_lib.py
+src/nef_pipelines/lib/spectra_lib.py
 src/nef_pipelines/lib/structures.py
 src/nef_pipelines/lib/test_lib.py
 src/nef_pipelines/lib/typer_utils.py
 src/nef_pipelines/lib/util.py
 src/nef_pipelines/lib/translation/__init__.py
 src/nef_pipelines/nef_app/__init__.py
 src/nef_pipelines/tests/conftest.py
@@ -69,15 +72,14 @@
 src/nef_pipelines/tests/frames/__init__.py
 src/nef_pipelines/tests/frames/test_delete.py
 src/nef_pipelines/tests/frames/test_list.py
 src/nef_pipelines/tests/frames/test_rename.py
 src/nef_pipelines/tests/frames/test_tabulate.py
 src/nef_pipelines/tests/frames/test_data/frames.nef
 src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
-src/nef_pipelines/tests/frames/test_data/ubiquitin_short.nef
 src/nef_pipelines/tests/mars/__init__.py
 src/nef_pipelines/tests/mars/test_export_shifts.py
 src/nef_pipelines/tests/mars/test_import_shifts.py
 src/nef_pipelines/tests/mars/test_data/sec5_short.neff
 src/nef_pipelines/tests/mars/test_data/sec5_short.txt
 src/nef_pipelines/tests/nmrpipe/__init__.py
 src/nef_pipelines/tests/nmrpipe/test_gdb.py
@@ -128,14 +130,16 @@
 src/nef_pipelines/tests/pdbx/test_sequence.py
 src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
 src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
 src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
 src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
 src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
 src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+src/nef_pipelines/tests/shifts/__init__.py
+src/nef_pipelines/tests/shifts/test_make_peaks.py
 src/nef_pipelines/tests/shifty/__init__.py
 src/nef_pipelines/tests/shifty/test_export_shifts.py
 src/nef_pipelines/tests/sparky/test_export_peaks.py
 src/nef_pipelines/tests/sparky/test_import_shifts.py
 src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
 src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
 src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
@@ -147,14 +151,15 @@
 src/nef_pipelines/tests/test_data/3a_ab.neff
 src/nef_pipelines/tests/test_data/empty.nef
 src/nef_pipelines/tests/test_data/header.nef
 src/nef_pipelines/tests/test_data/multi_chain.nef
 src/nef_pipelines/tests/test_data/nef_3_peaks.nef
 src/nef_pipelines/tests/test_data/tailin_seq_short.nef
 src/nef_pipelines/tests/test_data/test_agv.neff
+src/nef_pipelines/tests/test_data/ubiquitin_short.nef
 src/nef_pipelines/tests/xcamshift/test_export_shifts.py
 src/nef_pipelines/tests/xplor/test_dihedrals.py
 src/nef_pipelines/tests/xplor/test_distances.py
 src/nef_pipelines/tests/xplor/test_export_rdcs.py
 src/nef_pipelines/tests/xplor/test_import_sequence.py
 src/nef_pipelines/tests/xplor/test_psf_lib.py
 src/nef_pipelines/tests/xplor/test_xplor_lib.py
```

### Comparing `nef_pipelines-0.1.33/tox.ini` & `nef_pipelines-0.1.34/tox.ini`

 * *Files identical despite different names*

