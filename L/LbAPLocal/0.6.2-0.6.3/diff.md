# Comparing `tmp/LbAPLocal-0.6.2.tar.gz` & `tmp/LbAPLocal-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbAPLocal-0.6.2.tar", last modified: Mon Mar 20 22:36:20 2023, max compression
+gzip compressed data, was "LbAPLocal-0.6.3.tar", last modified: Mon Apr 17 14:31:34 2023, max compression
```

## Comparing `LbAPLocal-0.6.2.tar` & `LbAPLocal-0.6.3.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.844000 LbAPLocal-0.6.2/
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     2083 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2261 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      963 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     3027 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    32472 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7363 2023-03-20 22:36:20.844000 LbAPLocal-0.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6552 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/README.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/environment.yaml
--rw-r--r--   0 root         (0) root         (0)     1590 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/example.json
--rw-r--r--   0 root         (0) root         (0)      207 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      277 2023-03-20 22:36:20.844000 LbAPLocal-0.6.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2677 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.824000 LbAPLocal-0.6.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.828000 LbAPLocal-0.6.2/src/LbAPLocal/
--rw-r--r--   0 root         (0) root         (0)      800 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/src/LbAPLocal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5971 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/src/LbAPLocal/checks.py
--rw-r--r--   0 root         (0) root         (0)    23819 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/src/LbAPLocal/cli.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/src/LbAPLocal/log_parsing.py
--rw-r--r--   0 root         (0) root         (0)    10905 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/src/LbAPLocal/testing.py
--rw-r--r--   0 root         (0) root         (0)    10024 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/src/LbAPLocal/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.828000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7363 2023-03-20 22:36:20.000000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5932 2023-03-20 22:36:20.000000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 22:36:20.000000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-03-20 22:36:20.000000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 22:36:20.000000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      182 2023-03-20 22:36:20.000000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-03-20 22:36:20.000000 LbAPLocal-0.6.2/src/LbAPLocal.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.832000 LbAPLocal-0.6.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.824000 LbAPLocal-0.6.2/tests/cassettes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.832000 LbAPLocal-0.6.2/tests/cassettes/test_execute/
--rw-r--r--   0 root         (0) root         (0)     2775 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml
--rw-r--r--   0 root         (0) root         (0)     2536 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml
--rw-r--r--   0 root         (0) root         (0)      908 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml
--rw-r--r--   0 root         (0) root         (0)     5430 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.828000 LbAPLocal-0.6.2/tests/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.832000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/
--rw-r--r--   0 root         (0) root         (0)      622 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/.gitignore
--rw-r--r--   0 root         (0) root         (0)      837 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)      405 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/AnalysisProductions.xenv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.832000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/
--rw-r--r--   0 root         (0) root         (0)     4485 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py
--rw-r--r--   0 root         (0) root         (0)     4320 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py
--rw-r--r--   0 root         (0) root         (0)      341 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar_stripping.py
--rw-r--r--   0 root         (0) root         (0)     5996 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py
--rw-r--r--   0 root         (0) root         (0)     3988 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py
--rw-r--r--   0 root         (0) root         (0)     4315 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py
--rw-r--r--   0 root         (0) root         (0)     4905 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py
--rw-r--r--   0 root         (0) root         (0)     3597 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus_stripping.py
--rw-r--r--   0 root         (0) root         (0)      178 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/LbJpsipK.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.832000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py
--rw-r--r--   0 root         (0) root         (0)     8845 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)    20265 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml
--rw-r--r--   0 root         (0) root         (0)     1013 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py
--rw-r--r--   0 root         (0) root         (0)    35149 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/COPYING
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.832000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/
--rw-r--r--   0 root         (0) root         (0)      212 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/README.md
--rw-r--r--   0 root         (0) root         (0)      831 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/Run1_Signal.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/Run2_Signal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.836000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8972 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/info.yaml
--rw-r--r--   0 root         (0) root         (0)     6380 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.836000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/2011_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/2012_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/2015_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/2016_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/2017_datatype.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/2018_datatype.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/B0ToK0ee.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/B0ToK0mumu.py
--rw-r--r--   0 root         (0) root         (0)      240 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/BpToKee.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/BpToKmumu.py
--rw-r--r--   0 root         (0) root         (0)      228 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/LbToL0ee.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/LbToL0eeSS.py
--rw-r--r--   0 root         (0) root         (0)      230 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/LbToL0emu.py
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/LbToL0emuSS.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/LbToL0mumu.py
--rw-r--r--   0 root         (0) root         (0)      232 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/LbToL0mumuSS.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/__init__.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/general_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.840000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7993 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/locations.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py
--rw-r--r--   0 root         (0) root         (0)     3733 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py
--rw-r--r--   0 root         (0) root         (0)    56910 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/tags.py
--rw-r--r--   0 root         (0) root         (0)    20824 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py
--rw-r--r--   0 root         (0) root         (0)     2093 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/info.yaml
--rw-r--r--   0 root         (0) root         (0)      149 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_DST.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_FDST.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_FMDST.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_general_options_MDST.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.840000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/
--rw-r--r--   0 root         (0) root         (0)      121 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_ee.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_mm.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksee.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksmm.py
--rw-r--r--   0 root         (0) root         (0)      121 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_ee.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_mm.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_ee.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_mm.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_ee.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_mm.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lee.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lem.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lmm.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_ee.py
--rw-r--r--   0 root         (0) root         (0)      120 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_mm.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/sequence_setup.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/stripping_seq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.840000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/executabletests/
--rw-r--r--   0 root         (0) root         (0)      348 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/executabletests/2016_MagDown_PromptMC_D02KK_autoconf.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/executabletests/2016_MagUp_PromptMC_D02KK_autoconf.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/executabletests/info.yaml
--rw-r--r--   0 root         (0) root         (0)     1393 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/data-pkg-repo/executabletests/ntuple_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 22:36:20.844000 LbAPLocal-0.6.2/tests/data/example-logs/
--rw-r--r--   0 root         (0) root         (0)   516613 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/error-failed-to-read-file.log
--rw-r--r--   0 root         (0) root         (0)   344567 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/error-illegal-instruction.log
--rw-r--r--   0 root         (0) root         (0)     3373 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/error-missing-shared-library.log
--rw-r--r--   0 root         (0) root         (0)     2723 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/error-platform-unsupported.log
--rw-r--r--   0 root         (0) root         (0)   584650 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/error-related-info-missing.log
--rw-r--r--   0 root         (0) root         (0)   135940 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log
--rw-r--r--   0 root         (0) root         (0)   139869 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log
--rw-r--r--   0 root         (0) root         (0)   751141 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/data/example-logs/good-Gauss_00104988_00000011_1.log
--rw-r--r--   0 root         (0) root         (0)     4057 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/test_execute.py
--rw-r--r--   0 root         (0) root         (0)     2724 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/test_local_datapkg.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-03-20 22:36:05.000000 LbAPLocal-0.6.2/tests/test_log_parse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.544000 LbAPLocal-0.6.3/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      963 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    32472 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7363 2023-04-17 14:31:34.544000 LbAPLocal-0.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6552 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/environment.yaml
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/example.json
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-17 14:31:34.544000 LbAPLocal-0.6.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.516000 LbAPLocal-0.6.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.520000 LbAPLocal-0.6.3/src/LbAPLocal/
+-rw-r--r--   0 root         (0) root         (0)      800 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/src/LbAPLocal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/src/LbAPLocal/checks.py
+-rw-r--r--   0 root         (0) root         (0)    23965 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/src/LbAPLocal/cli.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/src/LbAPLocal/log_parsing.py
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/src/LbAPLocal/testing.py
+-rw-r--r--   0 root         (0) root         (0)    10024 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/src/LbAPLocal/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.524000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7363 2023-04-17 14:31:34.000000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5932 2023-04-17 14:31:34.000000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:31:34.000000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-17 14:31:34.000000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:31:34.000000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-17 14:31:34.000000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-17 14:31:34.000000 LbAPLocal-0.6.3/src/LbAPLocal.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.524000 LbAPLocal-0.6.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.516000 LbAPLocal-0.6.3/tests/cassettes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.524000 LbAPLocal-0.6.3/tests/cassettes/test_execute/
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml
+-rw-r--r--   0 root         (0) root         (0)      908 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml
+-rw-r--r--   0 root         (0) root         (0)     5430 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.520000 LbAPLocal-0.6.3/tests/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.524000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/
+-rw-r--r--   0 root         (0) root         (0)      622 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      837 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)      405 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/AnalysisProductions.xenv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.528000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py
+-rw-r--r--   0 root         (0) root         (0)      341 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar_stripping.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py
+-rw-r--r--   0 root         (0) root         (0)     3988 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py
+-rw-r--r--   0 root         (0) root         (0)     4315 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py
+-rw-r--r--   0 root         (0) root         (0)     4905 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus_stripping.py
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/LbJpsipK.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.528000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py
+-rw-r--r--   0 root         (0) root         (0)     8845 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)    20265 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/COPYING
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.528000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/README.md
+-rw-r--r--   0 root         (0) root         (0)      831 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/Run1_Signal.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/Run2_Signal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.528000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8972 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/info.yaml
+-rw-r--r--   0 root         (0) root         (0)     6380 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.536000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/2011_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/2012_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/2015_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/2016_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/2017_datatype.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/2018_datatype.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/B0ToK0ee.py
+-rw-r--r--   0 root         (0) root         (0)      235 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/B0ToK0mumu.py
+-rw-r--r--   0 root         (0) root         (0)      240 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/BpToKee.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/BpToKmumu.py
+-rw-r--r--   0 root         (0) root         (0)      228 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/LbToL0ee.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/LbToL0eeSS.py
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/LbToL0emu.py
+-rw-r--r--   0 root         (0) root         (0)      233 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/LbToL0emuSS.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/LbToL0mumu.py
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/LbToL0mumuSS.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/general_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.536000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7993 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/locations.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py
+-rw-r--r--   0 root         (0) root         (0)     3733 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py
+-rw-r--r--   0 root         (0) root         (0)    56910 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/tags.py
+-rw-r--r--   0 root         (0) root         (0)    20824 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/info.yaml
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_DST.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_FDST.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_FMDST.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_general_options_MDST.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.540000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_ee.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2JpsiKs_mm.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksee.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2Ksmm.py
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_ee.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bd2PsiKs_mm.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_ee.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Bu2JpsiK_mm.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_ee.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2JpsiL_mm.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lee.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lem.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2Lmm.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_ee.py
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/mc_samples/MC_Lb2PsiL_mm.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/sequence_setup.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/stripping_seq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.540000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/executabletests/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/executabletests/2016_MagDown_PromptMC_D02KK_autoconf.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/executabletests/2016_MagUp_PromptMC_D02KK_autoconf.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/executabletests/info.yaml
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/data-pkg-repo/executabletests/ntuple_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:31:34.544000 LbAPLocal-0.6.3/tests/data/example-logs/
+-rw-r--r--   0 root         (0) root         (0)   516613 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/error-failed-to-read-file.log
+-rw-r--r--   0 root         (0) root         (0)   344567 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/error-illegal-instruction.log
+-rw-r--r--   0 root         (0) root         (0)     3373 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/error-missing-shared-library.log
+-rw-r--r--   0 root         (0) root         (0)     2723 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/error-platform-unsupported.log
+-rw-r--r--   0 root         (0) root         (0)   584650 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/error-related-info-missing.log
+-rw-r--r--   0 root         (0) root         (0)   135940 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log
+-rw-r--r--   0 root         (0) root         (0)   139869 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log
+-rw-r--r--   0 root         (0) root         (0)   751141 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/data/example-logs/good-Gauss_00104988_00000011_1.log
+-rw-r--r--   0 root         (0) root         (0)     4057 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/test_execute.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/test_local_datapkg.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-17 14:31:12.000000 LbAPLocal-0.6.3/tests/test_log_parse.py
```

### Comparing `LbAPLocal-0.6.2/.gitignore` & `LbAPLocal-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/.gitlab-ci.yml` & `LbAPLocal-0.6.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/.pre-commit-config.yaml` & `LbAPLocal-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/CONTRIBUTING.md` & `LbAPLocal-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/LICENSE` & `LbAPLocal-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/PKG-INFO` & `LbAPLocal-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPLocal
-Version: 0.6.2
+Version: 0.6.3
 Summary: Tool to locally run tests for AnalysisProductions
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal/-/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Keywords: LHCb AnalysisProductions DIRAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbAPLocal-0.6.2/README.md` & `LbAPLocal-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/example.json` & `LbAPLocal-0.6.3/example.json`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/setup.py` & `LbAPLocal-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     packages=find_packages("src"),
     package_dir={"": "src"},
     python_requires=">=3.9",
     setup_requires=["setuptools_scm"],
     install_requires=[
         "click",
         "consolemd",
-        "LbAPCommon>=0.9.1",
+        "LbAPCommon>=0.9.3",
         "apd~=0.4.0",
         "LbEnv",
         "LbDiracWrappers",
         "requests",
         "setuptools",
         "mplhep",
         "LbProdRun~=1.3",
```

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal/__init__.py` & `LbAPLocal-0.6.3/src/LbAPLocal/__init__.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal/checks.py` & `LbAPLocal-0.6.3/src/LbAPLocal/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,42 +23,44 @@
 from LbAPCommon import parse_yaml, render_yaml, validate_yaml
 from LbAPCommon.checks import run_job_checks
 from LbAPCommon.checks_utils import checks_to_JSON, hist_to_root
 
 from .utils import check_production
 
 
+# TODO this is no longer needed as we will always have some default checks now for general validation
 def checks_exist(checks_data):
     """
     Return true if any checks have been defined in the config file for this production
     Otherwise returns false
     """
     return len(checks_data) > 0
 
 
-def perform_checks(production_name, job_name, test_ntuple_path_list, checks_output_dir):
+def perform_checks(
+    production_name, jobs_data, job_name, test_ntuple_path_list, checks_output_dir
+):
     """
     Run all stages of checks
     """
     job_data, checks_data = prepare_checks(
         production_name, job_name, test_ntuple_path_list, checks_output_dir
     )
 
-    if "checks" in job_data.keys():
-        click.secho("Running checks", fg="green")
-        check_results = run_job_checks(
-            job_data["checks"], checks_data, test_ntuple_path_list
-        )
-        output_check_results(job_name, checks_data, check_results, checks_output_dir)
+    click.secho("Running checks", fg="green")
+    check_results = run_job_checks(
+        jobs_data, job_name, job_data["checks"], checks_data, test_ntuple_path_list
+    )
+    output_check_results(job_name, checks_data, check_results, checks_output_dir)
 
-        if all([check_results[cr].passed for cr in check_results]):
-            click.secho(
-                f"All checks passed! Any output can be found in {checks_output_dir}",
-                fg="green",
-            )
+    if all([check_results[cr].passed for cr in check_results]):
+        click.secho(
+            f"All checks passed! Any output can be found in {checks_output_dir}",
+            fg="green",
+        )
 
 
 def prepare_checks(production_name, job_name, test_ntuple_path_list, checks_output_dir):
     """
     For a specific job's checks, run anything required before the checks themselves are executed.
     This includes:
     * Parsing & validating the config file
@@ -138,8 +140,8 @@
                             ax.set_ylabel(_histo.axes[1].name)
                     tree_name = "_".join(key.split("/"))
                     fig_name = f"{job_name}_{tree_name}_{cr}_{hist_counter-1}.pdf"
                     plt.savefig(join(checks_out_dir, fig_name))
         else:
             click.secho(f"Check '{cr}' failed!", fg="red")
         for msg in check_results[cr].messages:
-            print(f"{cr}: {msg}")
+            click.secho(f"{cr}: {msg}", fg="yellow")
```

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal/cli.py` & `LbAPLocal-0.6.3/src/LbAPLocal/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,15 @@
 
     if result.returncode != 0:
         raise click.ClickException("Execution failed, see above for details")
 
     # Obtain the right output file name
     with open(os.path.join(production_name, "info.yaml"), "rt") as fp:
         raw_yaml = fp.read()
+    # TODO do we really need to redo parsing and validating when prepare test already does it?
     prod_data, checks_data = parse_yaml(render_yaml(raw_yaml))
     yaml_warnings = validate_yaml(prod_data, checks_data, ".", production_name)
     try:
         job_data = prod_data[job_name]
     except KeyError:
         raise click.ClickException(
             f"Job {job_name} is not found for production {production_name}!"
@@ -495,20 +496,22 @@
         )
     if not any([warnings, errors]):
         click.secho(
             "No problems found while validating the options and output file!",
             fg="green",
         )
 
-    from .checks import checks_exist, perform_checks
+    from .checks import perform_checks
 
     # Run checks
-    if checks_exist(checks_data):
-        checks_output_dir = join(out_dir, "checks")
-        perform_checks(production_name, job_name, [test_ntuple_path], checks_output_dir)
+    # if checks_exist(checks_data):
+    checks_output_dir = join(out_dir, "checks")
+    perform_checks(
+        production_name, prod_data, job_name, [test_ntuple_path], checks_output_dir
+    )
 
     # The functionality of job-dependent job testing relies on out_dir being written
     # in the line below as the final word so please be careful if changing the below line
     click.secho(f"Success! Output can be found in {out_dir}", fg="green")
 
 
 @main.command()
@@ -538,19 +541,20 @@
             click.secho(f"WARNING: {warning}", fg="yellow")
         click.secho("YAML parsed and validated successfully", fg="green")
 
     # If checks_output_dir not specified, set it to a "checks" dir in the same directory as the input file
     if not checks_output_dir:
         checks_output_dir = join(os.path.dirname(test_ntuple_path), "checks")
 
-    from .checks import checks_exist, perform_checks
+    from .checks import perform_checks
 
     # Run checks
-    if checks_exist(checks_data):
-        perform_checks(production_name, job_name, [test_ntuple_path], checks_output_dir)
+    perform_checks(
+        production_name, prod_data, job_name, [test_ntuple_path], checks_output_dir
+    )
 
 
 @main.command()
 @click.argument("checks_data_file", type=str, nargs=1)
 @click.argument("input_ntuple", type=str, nargs=1)
 @click.argument("output_dir", type=str, nargs=1)
 @click.argument("job_index", type=int, nargs=1)
@@ -561,14 +565,16 @@
 
     from .checks import run_job_checks
 
     click.secho("Starting checks!", fg="green")
     with open(checks_data_file, "r") as inf:
         test_info = json.load(inf)
     check_results = run_job_checks(
+        test_info["jobs"],
+        test_info["jobs"][job_index]["name"],
         test_info["jobs"][job_index]["checks"],
         test_info["jobs"][job_index]["checks_data"],
         [input_ntuple],
     )
 
     from LbAPCommon.checks_utils import checks_to_JSON, hist_to_root
```

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal/log_parsing.py` & `LbAPLocal-0.6.3/src/LbAPLocal/log_parsing.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal/testing.py` & `LbAPLocal-0.6.3/src/LbAPLocal/testing.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal/utils.py` & `LbAPLocal-0.6.3/src/LbAPLocal/utils.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal.egg-info/PKG-INFO` & `LbAPLocal-0.6.3/src/LbAPLocal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbAPLocal
-Version: 0.6.2
+Version: 0.6.3
 Summary: Tool to locally run tests for AnalysisProductions
 Home-page: https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Author: LHCb
 Project-URL: Bug Reports, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal/-/issues
 Project-URL: Source, https://gitlab.cern.ch/lhcb-dpa/analysis-productions/lbaplocal
 Keywords: LHCb AnalysisProductions DIRAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LbAPLocal-0.6.2/src/LbAPLocal.egg-info/SOURCES.txt` & `LbAPLocal-0.6.3/src/LbAPLocal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml` & `LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK-2444].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml` & `LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagDown_PromptMC_D02KK_noautoconf-2444].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml` & `LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK-2393].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml` & `LbAPLocal-0.6.3/tests/cassettes/test_execute/test_run_test[2016_MagUp_PromptMC_D02KK_noautoconf-2393].yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/conftest.py` & `LbAPLocal-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/.gitignore` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/.gitignore`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/.gitlab-ci.yml` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bc2Bspi2JpsiPhi.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bd2JpsiKstar.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2DsPi.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Prompt_PVMixer.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bs2JpsiPhi_Swave.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/Bu2JpsiKplus.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/README.md` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/stripping.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/helpers/tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/BsToJpsiPhi/sequence_setup.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/COPYING` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/COPYING`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/Run1_Signal.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/Run1_Signal.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/Run2_Signal.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/Run2_Signal.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/helpers/signal_tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/RDs/info.yaml` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/RDs/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/README.md` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/README.md` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/README.md`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/MC_tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/decay_descriptors.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/locations.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/locations.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/related_info.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/stripping.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/tags.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/tags.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/helpers/tuple_maker.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/info.yaml` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/sequence_setup.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/sequence_setup.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/cbtesting/stripping_seq.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/cbtesting/stripping_seq.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/executabletests/info.yaml` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/executabletests/info.yaml`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/data-pkg-repo/executabletests/ntuple_options.py` & `LbAPLocal-0.6.3/tests/data/data-pkg-repo/executabletests/ntuple_options.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/error-failed-to-read-file.log` & `LbAPLocal-0.6.3/tests/data/example-logs/error-failed-to-read-file.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/error-illegal-instruction.log` & `LbAPLocal-0.6.3/tests/data/example-logs/error-illegal-instruction.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/error-missing-shared-library.log` & `LbAPLocal-0.6.3/tests/data/example-logs/error-missing-shared-library.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/error-platform-unsupported.log` & `LbAPLocal-0.6.3/tests/data/example-logs/error-platform-unsupported.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/error-related-info-missing.log` & `LbAPLocal-0.6.3/tests/data/example-logs/error-related-info-missing.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log` & `LbAPLocal-0.6.3/tests/data/example-logs/good-DaVinci_00110296_00000038_1.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log` & `LbAPLocal-0.6.3/tests/data/example-logs/good-DaVinci_00110296_00000194_1.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/data/example-logs/good-Gauss_00104988_00000011_1.log` & `LbAPLocal-0.6.3/tests/data/example-logs/good-Gauss_00104988_00000011_1.log`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/test_cli.py` & `LbAPLocal-0.6.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/test_execute.py` & `LbAPLocal-0.6.3/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/test_local_datapkg.py` & `LbAPLocal-0.6.3/tests/test_local_datapkg.py`

 * *Files identical despite different names*

### Comparing `LbAPLocal-0.6.2/tests/test_log_parse.py` & `LbAPLocal-0.6.3/tests/test_log_parse.py`

 * *Files identical despite different names*

